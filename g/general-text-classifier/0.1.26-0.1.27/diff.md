# Comparing `tmp/general_text_classifier-0.1.26-py3-none-any.whl.zip` & `tmp/general_text_classifier-0.1.27-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12905 bytes, number of entries: 6
--rw-r--r--  2.0 unx    56550 b- defN 23-May-08 11:06 general_text_classifier/__init__.py
--rw-------  2.0 unx     1062 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1188 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 23-May-08 11:07 general_text_classifier-0.1.26.dist-info/RECORD
-6 files, 59484 bytes uncompressed, 11861 bytes compressed:  80.1%
+Zip file size: 12846 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    56115 b- defN 23-May-12 20:24 general_text_classifier/__init__.py
+-rw-------  2.0 unx     1062 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1188 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      568 b- defN 23-May-12 20:24 general_text_classifier-0.1.27.dist-info/RECORD
+6 files, 59049 bytes uncompressed, 11802 bytes compressed:  80.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: general_text_classifier/__init__.py
 Comment: 
 
-Filename: general_text_classifier-0.1.26.dist-info/LICENSE.txt
+Filename: general_text_classifier-0.1.27.dist-info/LICENSE.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.26.dist-info/METADATA
+Filename: general_text_classifier-0.1.27.dist-info/METADATA
 Comment: 
 
-Filename: general_text_classifier-0.1.26.dist-info/WHEEL
+Filename: general_text_classifier-0.1.27.dist-info/WHEEL
 Comment: 
 
-Filename: general_text_classifier-0.1.26.dist-info/top_level.txt
+Filename: general_text_classifier-0.1.27.dist-info/top_level.txt
 Comment: 
 
-Filename: general_text_classifier-0.1.26.dist-info/RECORD
+Filename: general_text_classifier-0.1.27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## general_text_classifier/__init__.py

```diff
@@ -348,17 +348,15 @@
         classification_type: Optional[str] = "single",
         model_type: Optional[str] = "roberta",
         model_version: Optional[str] = "ty_roberta",
         gpus_to_use: Optional[List[str]] = [],
         exp_args: Optional[dict] = {},
         do_lowercase: Optional[bool] = True,
         data_lang: Optional[str] = "tr",
-        split_val_data: Optional[bool] = True,
-        split_size: Optional[float] = 0.2,
-        save_onnx_model: Optional[bool] = False,
+        save_onnx_model: Optional[bool] = True,
         random_state: Optional[int] = 2022,
         train_only_final_layer: Optional[bool] = False,
         freeze_layers_dict: Optional[List] = None,
         gcloud_project_id: Optional[str] = None,
         gcloud_bucket_name: Optional[str] = None,
         gcloud_blob_name: Optional[str] = None,
         gcloud_credentials_path: Optional[str] = None,
@@ -401,20 +399,14 @@
 
         do_lowercase: bool, optional
             Whether to convert text to lowercase or not.
         
         data_lang: str, optional
             Language of the data to be trained on.
 
-        split_val_data : bool, optional
-            Whether to split training data into training & validation data for model training or not.
-
-        split_size : bool, optional
-            Data split size into training & validation sets. Valid if split_val_data == True.
-
         save_onnx_model : bool, optional
             Whether to upload only the ONNX model to GCS or not.
 
         random_state : int, optional
             Random seed for reproducibility
 
         train_only_last_layer: bool, optional
@@ -508,18 +500,16 @@
         if self.do_train:
             # create model arguments
             assert classification_type in [
                 "single",
                 "multi",
             ], self.print_error_messages(1)
             self.classification_type = classification_type
-            self.split_val_data = split_val_data
-            self.split_size = split_size
             self.random_state = random_state
-
+            
             if self.classification_type == "single":
                 self.classification_model_obj = ClassificationModel
                 self.classification_args_obj = ClassificationArgs
 
             elif self.classification_type == "multi":
                 self.classification_model_obj = MultiLabelClassificationModel
                 self.classification_args_obj = MultiLabelClassificationArgs
@@ -533,33 +523,35 @@
                 "early_stopping_metric_minimize": True,
                 "early_stopping_patience": 5,
                 "eval_batch_size": 16,
                 "train_batch_size": 16,
                 "n_gpu": len(self.gpus_to_use),
                 "evaluate_during_training": True,
                 "evaluate_during_training_silent": False,
-                "save_model_every_epoch": False,
                 "fp16": True,
                 "num_train_epochs": 3,
                 "reprocess_input_data": True,
                 "output_dir": os.path.join(self.model_dir, "outputs/"),
                 "best_model_dir": os.path.join(self.model_dir, "best_model/"),
                 "cache_dir": os.path.join(self.model_dir, "cache_dir/"),
                 "overwrite_output_dir": True,
                 "use_multiprocessing": False,
                 "use_multiprocessing_for_evaluation": False,
                 "manual_seed": self.random_state,
-                "save_eval_checkpoints": True
+                "save_model_every_epoch": False,
+                "save_eval_checkpoints": False,
+                "save_steps": -1,
+                "save_best_model": True
             }
 
             self.model_args = {**self.model_args, **exp_args}
             self.model_type = model_type
             self.model_version = model_version
             self.save_onnx_model = save_onnx_model
-            self.split_size = split_size
+            self.split_size = 0.2
 
             # create BigQ directories
             if self.model_version in ["ty_bert", "ty_roberta"]:
                 assert nlp_credentials_path is not None, self.print_error_messages(2)
                 assert os.path.exists(nlp_credentials_path), self.print_error_messages(
                     3
                 )
@@ -598,29 +590,29 @@
 
             # arrange directory parameters
             self.model_dir_splitted = os.path.split(self.model_dir)
 
             self.label_encoder_dir = os.path.join(
                 self.model_dir_splitted[0],
                 self.model_dir_splitted[-1],
-                "best_model" if self.split_val_data else "outputs",
+                "best_model",
                 "label_encoder.joblib",
             )
 
             self.model_metadata_dir = os.path.join(
                 self.model_dir_splitted[0],
                 self.model_dir_splitted[-1],
-                "best_model" if self.split_val_data else "outputs",
+                "best_model",
                 "model_metadata.joblib",
             )
 
             if gcloud_blob_name is not None:
                 self.model_bigq_dir = os.path.join(
                     gcloud_blob_name,
-                    "best_model.tar.gz" if self.split_val_data else "outputs.tar.gz",
+                    "best_model.tar.gz",
                 )
 
             if save_onnx_model:
                 self.onnx_model_dir = os.path.join(
                     self.model_dir_splitted[0],
                     self.model_dir_splitted[-1],
                     "onnx_model",
@@ -969,22 +961,21 @@
         if self.do_lowercase and self.data_lang == "tr":
             self.train_data["text"] = self.train_data["text"].apply(
                 self.lowercase_turkish
             )
 
         if self.val_data is not None:
             self.val_data["text"] = self.val_data["text"].astype(str)
-            self.split_val_data = False
 
             if self.do_lowercase and self.data_lang == "tr":
                 self.val_data["text"] = self.val_data["text"].apply(
                     self.lowercase_turkish
                 )
 
-        if self.split_val_data:
+        if self.do_train and self.val_data is None:
             self.print_log_messages(3)
 
             if self.classification_type == "single":
                 try:
                     x_train, x_val, y_train, y_val = train_test_split(
                         self.train_data["text"],
                         self.train_data["labels"],
@@ -1086,15 +1077,15 @@
         val_data: Optional[pd.DataFrame] = None,
         print_model_card: Optional[bool] = True,
         **kwargs,
     ) -> None:
         """Function to fit the model. If the model is multilabel, data must be a dataframe with two columns:
         | text    | labels                      |
          ---------  ----------------------------
-        | <text>  | <label_1>, <label_2>, ...   |
+        | <text>  | <label_1>;<label_2>;...     |
 
         Parameters
         ----------
         train_table_name : str, optional
             Name of the BigQ table for training data
 
         train_data : pd.DataFrame, optional
@@ -1319,15 +1310,14 @@
         # save onnx model
         if self.save_onnx_model:
             if os.path.exists(self.onnx_model_dir):
                 self.print_log_messages(8)
                 shutil.rmtree(self.onnx_model_dir)
 
             copy.deepcopy(self.model).convert_to_onnx(self.onnx_model_dir)
-
             make_archive(self.onnx_model_dir, "gztar", root_dir=self.onnx_model_dir)
 
             if self.gcloud_bucket_name is not None:
                 self.upload_to_gcs(
                     self.storage_client,
                     self.onnx_model_dir + ".tar.gz",
                     self.gcloud_bucket_name,
@@ -1342,15 +1332,15 @@
         test_data: Optional[pd.DataFrame] = None,
         result_save_path: Optional[str] = None,
     ) -> str:
         """Function to get predictions from the model.
         If the model is multilabel, data must be a dataframe with two columns:
         | text    | labels                      |
          ---------  ----------------------------
-        | <text>  | <label_1>, <label_2>, ...   |
+        | <text>  | <label_1>;<label_2>;...     |
 
         Parameters
         ----------
         test_table_name : str
             Name of the BigQ table for test data
 
         test_data : pd.DataFrame
@@ -1437,15 +1427,15 @@
             )
         else:
             predictions_raw = []
             confidence_scores = []
 
             for i in range(len(self.raw_outputs)):
                 predictions_raw.append(
-                    ";".join(
+                    ", ".join(
                         self.label_encoder.inverse_transform(
                             np.array(self.predictions[i]).reshape(1, -1)
                         )[0]
                     )
                 )
                 confidence_scores.append(
                     self.raw_outputs[i][np.nonzero(self.predictions[i])[0]]
@@ -1483,20 +1473,22 @@
                     str(elem) for elem in self.label_encoder.classes_.tolist()
                 ],
                 digits=4,
                 output_dict=True,
             )
 
             self.cls_report = pd.DataFrame(self.cls_report).T
-            self.cls_report_path = (
-                os.path.join(self.model_dir, "best_model", "cls_report.csv")
-                if self.model_metadata["do_eval"]
-                else os.path.join(self.model_dir, "outputs", "cls_report.csv")
-            )
-            self.cls_report.to_csv(self.cls_report_path)
+            
+            if self.do_train:
+                self.cls_report_path = (
+                    os.path.join(self.model_dir, "best_model", "cls_report.csv")
+                    if self.model_metadata["do_eval"]
+                    else os.path.join(self.model_dir, "outputs", "cls_report.csv")
+                )
+                self.cls_report.to_csv(self.cls_report_path)
 
             self.print_log_messages(16)
 
             reindex_cols = ["text", "labels_original"] + [
                 elem
                 for elem in self.test_data.columns.tolist()
                 if elem not in ["text", "labels_original"]
@@ -1504,7 +1496,9 @@
             self.test_data = self.test_data[reindex_cols]
 
         if result_save_path is not None:
             self.test_data.to_csv(result_save_path, index=False)
             self.print_log_messages(14)
 
         self.print_log_messages(15)
+
+
```

## Comparing `general_text_classifier-0.1.26.dist-info/LICENSE.txt` & `general_text_classifier-0.1.27.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `general_text_classifier-0.1.26.dist-info/METADATA` & `general_text_classifier-0.1.27.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-text-classifier
-Version: 0.1.26
+Version: 0.1.27
 Summary: General Text Classification Library
 Home-page: UNKNOWN
 Author: Trendyol NLP Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `general_text_classifier-0.1.26.dist-info/RECORD` & `general_text_classifier-0.1.27.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-general_text_classifier/__init__.py,sha256=ZbtFd3MqUNGXaHpJ34zElbodQ7TMByx5ms4YujhiMtQ,56550
-general_text_classifier-0.1.26.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
-general_text_classifier-0.1.26.dist-info/METADATA,sha256=3XBuxxHta0gEH0oEEHTUEeqYYz7np3mlYDnPHxgiJIY,1188
-general_text_classifier-0.1.26.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-general_text_classifier-0.1.26.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
-general_text_classifier-0.1.26.dist-info/RECORD,,
+general_text_classifier/__init__.py,sha256=rJ4veaBT44L1t5dhW7BhkkKyVcDeOp9Gg1AmWa1JdfM,56115
+general_text_classifier-0.1.27.dist-info/LICENSE.txt,sha256=39ifOUz0fv0QxPoscWvZ9z9ZkO1xtfvb8ze-KnkO3EE,1062
+general_text_classifier-0.1.27.dist-info/METADATA,sha256=hvvWvjQnoBS288AvKaBCB5JR323cSqVli16X7dGz3qQ,1188
+general_text_classifier-0.1.27.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+general_text_classifier-0.1.27.dist-info/top_level.txt,sha256=8byuMM000m_1XjdHiOSw1VvLuoY7o1e8hk5siED7p_0,24
+general_text_classifier-0.1.27.dist-info/RECORD,,
```

