# Comparing `tmp/vl_datasets-0.0.4-py3.9-none-any.whl.zip` & `tmp/vl_datasets-0.0.5-py3.9-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11778 bytes, number of entries: 8
--rw-r--r--  2.0 unx       99 b- defN 23-May-09 06:35 vl_datasets/__init__.py
--rw-r--r--  2.0 unx     3127 b- defN 23-May-09 06:35 vl_datasets/food101.py
--rw-r--r--  2.0 unx     2352 b- defN 23-May-09 06:35 vl_datasets/image_folder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    15297 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      650 b- defN 23-May-09 06:35 vl_datasets-0.0.4.dist-info/RECORD
-8 files, 33002 bytes uncompressed, 10646 bytes compressed:  67.7%
+Zip file size: 12624 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       99 b- defN 23-May-15 06:06 vl_datasets/__init__.py
+-rw-r--r--  2.0 unx     4734 b- defN 23-May-15 06:06 vl_datasets/food101.py
+-rw-r--r--  2.0 unx     2352 b- defN 23-May-15 06:06 vl_datasets/image_folder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    16358 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      650 b- defN 23-May-15 06:06 vl_datasets-0.0.5.dist-info/RECORD
+8 files, 35670 bytes uncompressed, 11492 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vl_datasets/food101.py
 Comment: 
 
 Filename: vl_datasets/image_folder.py
 Comment: 
 
-Filename: vl_datasets-0.0.4.dist-info/LICENSE
+Filename: vl_datasets-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: vl_datasets-0.0.4.dist-info/METADATA
+Filename: vl_datasets-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: vl_datasets-0.0.4.dist-info/WHEEL
+Filename: vl_datasets-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: vl_datasets-0.0.4.dist-info/top_level.txt
+Filename: vl_datasets-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: vl_datasets-0.0.4.dist-info/RECORD
+Filename: vl_datasets-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vl_datasets/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 from .image_folder import CleanImageFolder
 from .food101 import CleanFood101
```

## vl_datasets/food101.py

```diff
@@ -1,14 +1,36 @@
 # Code adapted from https://github.com/pytorch/vision/blob/main/torchvision/datasets/utils.py
 
 from torchvision.datasets import Food101
-from typing import Any, Callable, Optional, Tuple, TypeVar, Iterable
+from typing import Any, Callable, Optional, TypeVar, Iterable
 from pathlib import Path
 import json
 import pandas as pd
+import requests
+
+import torchvision.transforms as transforms
+
+train_transform = transforms.Compose(
+    [
+        transforms.RandomResizedCrop(224),
+        transforms.RandomHorizontalFlip(),
+        transforms.ToTensor(),
+        transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
+    ]
+)
+
+valid_transform = transforms.Compose(
+    [
+        transforms.Resize(256),
+        transforms.CenterCrop(224),
+        transforms.ToTensor(),
+        transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
+    ]
+)
+
 
 class CleanFood101(Food101):
     def __init__(
         self,
         root: str,
         split: str = "train",
         transform: Optional[Callable] = None,
@@ -29,22 +51,51 @@
         self._image_files = []
         with open(self._meta_folder / f"{split}.json") as f:
             metadata = json.loads(f.read())
 
         self.classes = sorted(metadata.keys())
         self.class_to_idx = dict(zip(self.classes, range(len(self.classes))))
 
+        # Default tranform
+        if transform is None:
+            if split == 'train':
+                self.transform = train_transform
+
+            elif split == 'test':
+                self.transform = valid_transform
+
+        # If user specifies a csv file use it
         if exclude_csv:
+            print(f"Using provided CSV file: {exclude_csv}")
             self.exclude_df = pd.read_csv(exclude_csv, header=0)
             self.exclude_set = set(self.exclude_df["filename"].tolist())
+        
+        # Otherwise, download the csv file
+        elif exclude_csv is None:
+            print("Downloading CSV file")
+            url = "https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw" 
+            filename = "food-101.csv"
+
+            try:
+                response = requests.get(url, stream=True)
+                with open(filename, "wb") as f:
+                    for chunk in response.iter_content(chunk_size=1024):
+                        f.write(chunk)
+
+                self.exclude_df = pd.read_csv(filename, header=0)
+                self.exclude_set = set(self.exclude_df["filename"].tolist())
+
+            except Exception as e:
+                print("Error parsing CSV file")
+                print(e)
 
         self.excluded_files = []
         for class_label, im_rel_paths in metadata.items():
             for im_rel_path in im_rel_paths:
-                if exclude_csv is not None and f"{im_rel_path}.jpg" in self.exclude_set:
+                if f"{im_rel_path}.jpg" in self.exclude_set:
                     # print(f"Excluding {im_rel_path}.jpg")
                     self.excluded_files.append(f"{im_rel_path}.jpg")
                     continue
                 self._labels += [self.class_to_idx[class_label]]
                 self._image_files += [self._images_folder.joinpath(*f"{im_rel_path}.jpg".split("/"))]
 
         print(f"Excluded {len(self.excluded_files)} from the {split} set")
```

## Comparing `vl_datasets-0.0.4.dist-info/LICENSE` & `vl_datasets-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vl_datasets-0.0.4.dist-info/METADATA` & `vl_datasets-0.0.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vl-datasets
-Version: 0.0.4
+Version: 0.0.5
 Summary: Open, Clean Datasets for Computer Vision.
 Home-page: https://github.com/visual-layer/vl-datasets
 Author: Visual Layer
 Author-email: info@visual-layer.com
 License: Apache-2.0
 Keywords: machine learning,computer vision,data-centric
 Platform: UNKNOWN
@@ -66,15 +66,15 @@
     🔥 We use
     <a href="https://github.com/visual-layer/fastdup">fastdup</a> - a free tool to clean all datasets shared in this repo.
     <br />
     <a href="https://visual-layer.readme.io/" target="_blank" rel="noopener noreferrer"><strong>Explore the docs »</strong></a>
     <br />
     <a href="https://github.com/visual-layer/vl-datasets/issues" target="_blank" rel="noopener noreferrer">Report Issues</a>
     ·
-    <a href="https://medium.com/@amiralush/large-image-datasets-today-are-a-mess-e3ea4c9e8d22" target="_blank" rel="noopener noreferrer">Read Blog</a>
+    <a href="https://medium.com/@visual-layer/" target="_blank" rel="noopener noreferrer">Read Blog</a>
     ·
     <a href="mailto:info@visual-layer.com?subject=Sign-up%20for%20access" target="_blank" rel="noopener noreferrer">Get In Touch</a>
     ·
     <a href="https://visual-layer.com/" target="_blank" rel="noopener noreferrer">About Us</a>
     <br />
     <br /> 
     <a href="https://visualdatabase.slack.com/join/shared_invite/zt-19jaydbjn-lNDEDkgvSI1QwbTXSY6dlA#/shared-invite/email" target="_blank" rel="noopener noreferrer">
@@ -118,24 +118,24 @@
 We believe that access to clean and high-quality computer vision datasets leads to accurate, non-biased, and efficient model.
 By providing public access to `vl-datasets` we hope it helps advance the field of computer vision.
 
 ## Datasets & Access
 We're a startup and we'd like to offer free access to the datasets as much as we can afford to. But in doing so, we'd also need your support.
 
 We're offering select `.csv` files completely free with no strings attached. 
-For access to our complete dataset and exclusive beta features, all we ask is that you sign up to be a beta tester – it's completely free and your feedback will help shape the future of our platform. 
+For access to our complete dataset and exclusive beta features, all we ask is that you [sign up]((https://forms.gle/8jxPkyzeKj82kPed8)) to be a beta tester – it's completely free and your feedback will help shape the future of our platform. 
 
 Join us in unlocking the full potential of our data and revolutionizing the industry!
 
 Here is a table of widely used computer vision datasets, issues we found and a link to access the `.csv` file.
 
 
 | Dataset                                                                 | Issues (WIP)                                                                                                                                                                                 | CSV            |
 |-------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|
-| [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download [here](./notebooks/csv_files/food_101_vl-datasets_analysis.csv). |
+| [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download [here](https://drive.google.com/uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). |
 | [Oxford-IIIT Pet](https://www.robots.ox.ac.uk/~vgg/data/pets/)          | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download here. |
 | [Imagenette](https://github.com/fastai/imagenette)                      | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Download here. |
 | [LAION-1B](https://laion.ai/blog/laion-5b/)                             | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
 | [Imagenet-21k](https://www.image-net.org/)                              | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
 | [Imagenet-1k](https://www.image-net.org/)                               | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
 | [KITTI](https://www.cvlibs.net/datasets/kitti/)                         | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
 | [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html)    | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8).  |
@@ -176,39 +176,42 @@
 ## Usage
 To start using `vl-datasets`, you can import the clean version of the dataset with:
 
 ```python
 from vl_datasets import CleanFood101
 ```
 
-This should import the clean version of the Food101 dataset.
+This should import the clean version of the `Food101` dataset.
 
-Next, you can load the dataset as a PyTorch `DataLoader`.
+Next, you can load the dataset as a PyTorch `Dataset`.
 
 ```python
-train_dataset = CleanFood101('./', split='train', exclude_csv='food_101_vl-datasets_analysis.csv', transform=train_transform)
-valid_dataset = CleanFood101('./', split='test', exclude_csv='food_101_vl-datasets_analysis.csv', transform=valid_transform)
+train_dataset = CleanFood101('./', split='train')
+valid_dataset = CleanFood101('./', split='test')
 ```
 
-Now you can use the dataset in a PyTorch training loop. Refer to our sample training notebooks for details.
+
+> **NOTE**: Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8) for free to be our beta testers and get full access to the all the `.csv` files for the dataset listed in this repo. 
+
+With the dataset loaded you can train a model using PyTorch training loop.
 
 ## Learn from Examples
 
 <table>
   <tr>
       <td rowspan="3" width="160">
       <a href="https://visual-layer.readme.io/docs/getting-started">
               <img src="./imgs/food.jpg" width="256">
       </a>
       </td>    
       <td rowspan="3">
         <ul>
             <li> <b>Dataset:</b> <code>CleanFood101</code></li>
             <li> <b>Framework:</b> PyTorch.</li>
-            <li> <b>Description:</b> Train a simple PyTorch model with the CleanFood101 dataset.</li>
+            <li> <b>Description:</b> Load a dataset and train a PyTorch model.</li>
         </ul>
       </td>
       <td align="center" width="80">
           <a href="https://nbviewer.org/github/visual-layer/vl-datasets/blob/main/notebooks/train-pytorch.ipynb">
               <img src="./imgs/nbviewer_logo.svg" height="34">
           </a>
       </td>
@@ -236,15 +239,15 @@
               <img src="./imgs/pet.jpg" width="256">
       </a>
       </td>    
       <td rowspan="3">
         <ul>
             <li> <b>Dataset:</b> <code>CleanPets</code></li>
             <li> <b>Framework:</b> fast.ai.</li>
-            <li> <b>Description:</b> Train a simple TIMM model using fastai.</li>
+            <li> <b>Description:</b> Finetune a pretrained DINOv2 model using fastai.</li>
         </ul>
       </td>
       <td align="center" width="80">
           <a href="https://nbviewer.org/github/visual-layer/vl-datasets/blob/main/notebooks/train-fastai.ipynb">
               <img src="./imgs/nbviewer_logo.svg" height="34">
           </a>
       </td>
@@ -269,8 +272,26 @@
 </table>
 
 ## License
 `vl-datasets` is licensed under the Apache 2.0 License. See [LICENSE](./LICENSE).
 
 However, you are bound to the usage license of the original dataset. It is your responsibility to determine whether you have permission to use the dataset under the dataset's license. We provide no warranty or guarantee of accuracy or completeness.
 
+## Getting Help
+Get help from the Visual Layer team or community members via the following channels -
++ [Slack](https://visualdatabase.slack.com/join/shared_invite/zt-19jaydbjn-lNDEDkgvSI1QwbTXSY6dlA#/shared-invite/email).
++ GitHub [issues](https://github.com/visual-layer/vl-datasets/issues).
++ Discussion [forum](https://visual-layer.readme.io/discuss).
+
+## About Visual-Layer
+
+<div align="center">
+<a href="https://www.visual-layer.com">
+  <img alt="Visual Layer Logo" src="https://raw.githubusercontent.com/visual-layer/fastdup/main/gallery/visual_layer_logo.png" alt="Logo" width="250">
+</a>
+</div>
+
+
+Visual Layer is founded by the authors of [XGBoost](https://github.com/apache/tvm), [Apache TVM](https://github.com/apache/tvm) & [Turi Create](https://github.com/apple/turicreate) - [Danny Bickson](https://www.linkedin.com/in/dr-danny-bickson-835b32), [Carlos Guestrin](https://www.linkedin.com/in/carlos-guestrin-5352a869) and [Amir Alush](https://www.linkedin.com/in/amiralush).
+
+Learn more about Visual Layer [here](https://visual-layer.com).
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.4 Summary: Open, Clean
+Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.5 Summary: Open, Clean
 Datasets for Computer Vision. Home-page: https://github.com/visual-layer/vl-
 datasets Author: Visual Layer Author-email: info@visual-layer.com License:
 Apache-2.0 Keywords: machine learning,computer vision,data-centric Platform:
 UNKNOWN Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
@@ -44,32 +44,34 @@
 resources. We believe that access to clean and high-quality computer vision
 datasets leads to accurate, non-biased, and efficient model. By providing
 public access to `vl-datasets` we hope it helps advance the field of computer
 vision. ## Datasets & Access We're a startup and we'd like to offer free access
 to the datasets as much as we can afford to. But in doing so, we'd also need
 your support. We're offering select `.csv` files completely free with no
 strings attached. For access to our complete dataset and exclusive beta
-features, all we ask is that you sign up to be a beta tester â it's
-completely free and your feedback will help shape the future of our platform.
-Join us in unlocking the full potential of our data and revolutionizing the
-industry! Here is a table of widely used computer vision datasets, issues we
-found and a link to access the `.csv` file. | Dataset | Issues (WIP) | CSV | |-
-------------------------------------------------------------------------|------
+features, all we ask is that you [sign up]((https://forms.gle/
+8jxPkyzeKj82kPed8)) to be a beta tester â it's completely free and your
+feedback will help shape the future of our platform. Join us in unlocking the
+full potential of our data and revolutionizing the industry! Here is a table of
+widely used computer vision datasets, issues we found and a link to access the
+`.csv` file. | Dataset | Issues (WIP) | CSV | |--------------------------------
+-----------------------------------------|-------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
---------------------------|----------------| | [Food-101](https://
-data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) |
+--------------------------------------------------------------------------|----
+------------| | [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/
+food-101/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| Download [here](./notebooks/csv_files/food_101_vl-datasets_analysis.csv). | |
-[Oxford-IIIT Pet](https://www.robots.ox.ac.uk/~vgg/data/pets/) |
+| Download [here](https://drive.google.com/
+uc?export=download&id=1ZG5GvU342l4YmSeYo6v6LeKbMM5fwjjw). | | [Oxford-IIIT Pet]
+(https://www.robots.ox.ac.uk/~vgg/data/pets/) |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
 | Download here. | | [Imagenette](https://github.com/fastai/imagenette) |
@@ -152,28 +154,40 @@
     * Bright - 0.85% (456)
 | Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8). |  ## Installation
 **Option 1** - Install `vl_datasets` package from PyPI. ```shell pip install
 vl-datasets ``` **Option 2** - Install the bleeding edge version on GitHub ```
 pip install git+https://github.com/visual-layer/vl-datasets.git@main --upgrade
 ``` ## Usage To start using `vl-datasets`, you can import the clean version of
 the dataset with: ```python from vl_datasets import CleanFood101 ``` This
-should import the clean version of the Food101 dataset. Next, you can load the
-dataset as a PyTorch `DataLoader`. ```python train_dataset = CleanFood101('./',
-split='train', exclude_csv='food_101_vl-datasets_analysis.csv',
-transform=train_transform) valid_dataset = CleanFood101('./', split='test',
-exclude_csv='food_101_vl-datasets_analysis.csv', transform=valid_transform) ```
-Now you can use the dataset in a PyTorch training loop. Refer to our sample
-training notebooks for details. ## Learn from Examples
+should import the clean version of the `Food101` dataset. Next, you can load
+the dataset as a PyTorch `Dataset`. ```python train_dataset = CleanFood101('./
+', split='train') valid_dataset = CleanFood101('./', split='test') ``` >
+**NOTE**: Sign up [here](https://forms.gle/8jxPkyzeKj82kPed8) for free to be
+our beta testers and get full access to the all the `.csv` files for the
+dataset listed in this repo. With the dataset loaded you can train a model
+using PyTorch training loop. ## Learn from Examples
                       * Dataset: CleanFood101       [./imgs/nbviewer_logo.svg]
-                      * Framework: PyTorch.          [./imgs/github_logo.png]
-[./imgs/food.jpg]     * Description: Train a simple
-                        PyTorch model with the        [./imgs/colab_logo.png]
-                        CleanFood101 dataset.
+[./imgs/food.jpg]     * Framework: PyTorch.          [./imgs/github_logo.png]
+                      * Description: Load a dataset   [./imgs/colab_logo.png]
+                        and train a PyTorch model.
                       * Dataset: CleanPets          [./imgs/nbviewer_logo.svg]
-[./imgs/pet.jpg]      * Framework: fast.ai.          [./imgs/github_logo.png]
-                      * Description: Train a simple   [./imgs/colab_logo.png]
-                        TIMM model using fastai.
+                      * Framework: fast.ai.          [./imgs/github_logo.png]
+[./imgs/pet.jpg]      * Description: Finetune a
+                        pretrained DINOv2 model       [./imgs/colab_logo.png]
+                        using fastai.
 ## License `vl-datasets` is licensed under the Apache 2.0 License. See
 [LICENSE](./LICENSE). However, you are bound to the usage license of the
 original dataset. It is your responsibility to determine whether you have
 permission to use the dataset under the dataset's license. We provide no
-warranty or guarantee of accuracy or completeness.
+warranty or guarantee of accuracy or completeness. ## Getting Help Get help
+from the Visual Layer team or community members via the following channels - +
+[Slack](https://visualdatabase.slack.com/join/shared_invite/zt-19jaydbjn-
+lNDEDkgvSI1QwbTXSY6dlA#/shared-invite/email). + GitHub [issues](https://
+github.com/visual-layer/vl-datasets/issues). + Discussion [forum](https://
+visual-layer.readme.io/discuss). ## About Visual-Layer
+                              [Visual_Layer_Logo]
+Visual Layer is founded by the authors of [XGBoost](https://github.com/apache/
+tvm), [Apache TVM](https://github.com/apache/tvm) & [Turi Create](https://
+github.com/apple/turicreate) - [Danny Bickson](https://www.linkedin.com/in/dr-
+danny-bickson-835b32), [Carlos Guestrin](https://www.linkedin.com/in/carlos-
+guestrin-5352a869) and [Amir Alush](https://www.linkedin.com/in/amiralush).
+Learn more about Visual Layer [here](https://visual-layer.com).
```

