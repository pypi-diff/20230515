# Comparing `tmp/cerebrium-0.4.9.tar.gz` & `tmp/cerebrium-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-0.4.9.tar", max compression
+gzip compressed data, was "cerebrium-0.5.0.tar", max compression
```

## Comparing `cerebrium-0.4.9.tar` & `cerebrium-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0    34594 2023-02-21 14:55:13.514897 cerebrium-0.4.9/LICENSE
--rw-r--r--   0        0        0     3321 2023-02-21 14:55:13.514897 cerebrium-0.4.9/README.md
--rw-r--r--   0        0        0      258 2023-02-21 14:59:12.597668 cerebrium-0.4.9/cerebrium/__init__.py
--rw-r--r--   0        0        0    19297 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/conduit.py
--rw-r--r--   0        0        0     2248 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/core.py
--rw-r--r--   0        0        0     2524 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/errors.py
--rw-r--r--   0        0        0    11252 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/flow.py
--rw-r--r--   0        0        0     2804 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      807 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/base.py
--rw-r--r--   0        0        0      202 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/hf_transformer.py
--rw-r--r--   0        0        0      417 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/torch.py
--rw-r--r--   0        0        0     4568 2023-02-21 14:55:13.518897 cerebrium-0.4.9/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-02-21 14:55:13.518897 cerebrium-0.4.9/cerebrium/utils.py
--rw-r--r--   0        0        0     1584 2023-02-21 14:59:12.597668 cerebrium-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 cerebrium-0.4.9/setup.py
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 cerebrium-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-05-15 14:43:19.864846 cerebrium-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3055 2023-05-15 14:43:19.868846 cerebrium-0.5.0/README.md
+-rw-r--r--   0        0        0      285 2023-05-15 14:48:30.153519 cerebrium-0.5.0/cerebrium/__init__.py
+-rw-r--r--   0        0        0    29484 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/conduit.py
+-rw-r--r--   0        0        0     4451 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/core.py
+-rw-r--r--   0        0        0     2524 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/errors.py
+-rw-r--r--   0        0        0    10839 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      801 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     4555 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-05-15 14:43:19.868846 cerebrium-0.5.0/cerebrium/utils.py
+-rw-r--r--   0        0        0     2227 2023-05-15 14:48:30.153519 cerebrium-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 cerebrium-0.5.0/PKG-INFO
```

### Comparing `cerebrium-0.4.9/LICENSE` & `cerebrium-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.9/README.md` & `cerebrium-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -70,17 +70,10 @@
 aws codeartifact login --tool pip --repository cerebrium-pypi --domain cerebrium --domain-owner 288552132534 --region eu-west-1
 ```
 Then, pip install:
 ```bash
 pip install --pre cerebrium
 ```
 
-## Exporting Requirements for Cerebrium Server
-You should export the requirements for the Cerebrium server by running the following command:
-```bash
-poetry export >> cerebrium-requirements.txt
-```
-Once this is done, add them to the `cerebrium-conduit-server` repo.
-
 ### Resources for Poetry/CodeArtifact
 - https://repost.aws/questions/QURD7aFNj_R9-8odJY5mfgrw/npm-publish-for-a-package-to-aws-code-artifact-repo-fails-with-error-the-provided-package-is-configured-to-block-new-version-publishes
 - https://docs.aws.amazon.com/codeartifact/latest/ug/python-configure-pip.html
```

### Comparing `cerebrium-0.4.9/cerebrium/errors.py` & `cerebrium-0.5.0/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.9/cerebrium/logging/arize.py` & `cerebrium-0.5.0/cerebrium/logging/arize.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         self.space_key = platform_authentication["space_key"]
         self.api_key = platform_args["api_key"]
         self.model_type = platform_args["model_type"]
         self.features = platform_args["features"]
         self.schema = platform_args["schema"]
         self.metrics_validation = platform_args.get("metrics_validation", [])
-        self.environmet = platform_args.get("environmet", Environments.PRODUCTION)
+        self.environment = platform_args.get("environment", Environments.PRODUCTION)
         self.platform_args = platform_args
         self.client = Client(space_key=self.space_key, api_key=self.api_key)
 
     def check_ready(self, model_version: str, model_name: str) -> str:
         self.model_name = model_name
         self.model_version = model_version
 
@@ -64,13 +64,13 @@
                 df["embedding_features"] = self.platform_args["embedding_features"]
 
         response = self.client.log(
             model_id=self.model_name,
             model_version=self.model_version,
             model_type=self.model_type,
             metrics_validation=self.metrics_validation,
-            environment=self.environmet,
+            environment=self.environment,
             dataframe=pd.DataFrame([df], columns=df.keys()),
             schema=self.schema,
             sync=True,
         )
         return response
```

### Comparing `cerebrium-0.4.9/cerebrium/logging/base.py` & `cerebrium-0.5.0/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.9/cerebrium/logging/censius.py` & `cerebrium-0.5.0/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.9/cerebrium/models/base.py` & `cerebrium-0.5.0/cerebrium/models/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     XGBOOST_REGRESSOR = "xgboost_regressor"
     TORCH = "torch"
     SKLEARN = "sklearn"
     SKLEARN_CLASSIFIER = "sklearn_classifier"
     ONNX = "onnx"
     SKLEARN_PREPROCESSOR = "sklearn_preprocessor"
     PREBUILT = "prebuilt"
-    HUGGINGFACE_TRANSFORMER = "hf_transformer"
     SPACY = "spacy"
+    HUGGINGFACE_PIPELINE = "hf_pipeline"
 
 
 class BaseModel(ABC):
     def __init__(self, model: Union[BaseEstimator, TorchModule]):
         self.model = model
 
     @abstractmethod
```

### Comparing `cerebrium-0.4.9/cerebrium/models/sklearn.py` & `cerebrium-0.5.0/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.9/cerebrium/requests.py` & `cerebrium-0.5.0/cerebrium/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import Tuple
 from tenacity import retry, stop_after_delay, wait_fixed
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 from cerebrium.errors import CerebriumRequestError, CerebriumDeploymentError
 
 
-env = os.getenv("DEVELOPMENT_ENV", "prod")
-if env == "dev":
+ENV = os.getenv("DEVELOPMENT_ENV", "prod")
+if ENV == "dev":
     print("Using development environment")
     BASE_CEREBRIUM_URL = "https://dev-rest-api.cerebrium.ai"
 else:
     BASE_CEREBRIUM_URL = "https://rest-api.cerebrium.ai"
 
 
 def _check_payload(method: str, payload: dict) -> bool:
@@ -113,15 +113,15 @@
     ) as spinner:
         response = _cerebrium_request(
             "checkDeploymentStatus",
             api_key,
             payload={"arguments": {"name": conduit_name}},
         )
     if response["data"]["status"] == "deployed":
-        endpoint = response["data"]["endpoint"] + "/predict"
+        endpoint = response["data"]["endpoint"]
         print("✅ Conduit deployed!")
         return endpoint
     elif response["data"]["status"] == "failed":
         print("❌ Conduit deployment failed.")
         raise CerebriumDeploymentError(response["data"]["failureMessage"])
     else:
         print("⏳ Conduit deployment in progress...")
```

### Comparing `cerebrium-0.4.9/pyproject.toml` & `cerebrium-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "cerebrium"
-version = "0.4.9"
+version = "0.5.0"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
+exclude = ["tests/*", "dist/*", "worker/*"]
 
 [tool.poetry.urls]
 "Homepage" = "https://www.cerebrium.ai"
 "Documentation" = "https://docs.cerebrium.ai/"
 
 [[tool.poetry.source]]
 name = "cerebrium"
@@ -17,30 +18,40 @@
 secondary = false
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-xgboost = ">=1.7,<1.8"
-numpy = ">=1.23,<1.25"
-torch = ">=1.13,<1.14"
-scikit-learn = ">=1.2,<1.3"
+xgboost = "^1.7"
+numpy = "^1.20"
+torch = ">=1.13,<3.0"
+scikit-learn = "^1.2"
 cloudpickle = ">=2.0,<2.1"
-requests = ">=2.28,<2.29"
+requests = "^2.28"
 tqdm = ">=4.64,<4.65"
 tenacity = ">=8.2,<8.3"
 yaspin = ">=2.3,<2.4"
 censius = "^1.6"
 arize = ">=6.0.2,<7.0"
-pandas = ">=1.5,<1.6"
-onnxruntime = { version = ">=1.13,<1.15", optional= true }
-onnxruntime-gpu = { version = ">=1.14,<1.15", optional = true }
-transformers = ">=4.26, <4.27"
-spacy = ">=3.5.0,<3.6.0"
+pandas = ">=1.5,<3.0"
+onnxruntime = { version = "^1.13", optional= true }
+onnxruntime-gpu = { version = "^1.14", optional = true }
+transformers = "^4.26"
+spacy = "^3.5.0"
+boto3 = "^1.26.96"
+loguru = { version = ">=0.5,<0.6", optional= true }
+ddtrace = { version = ">=1.10.0,<1.11.0", optional= true }
+datadog = { version = ">=0.45.0,<0.51.0", optional= true }
+Pillow = { version = ">=9.4,<10.0.0", optional= true }
+chitra = { version = ">=0.2.0,<0.3.0", optional= true }
+datasets = { version = ">=2.10.0,<2.11.0", optional= true }
+celery = { version = ">=5.2.0,<5.3.0", optional= true }
+accelerate = { version = ">=0.18.0,<0.19.0", optional= true }
+bitsandbytes = { version = ">=0.38.0,<0.39.0", optional= true }
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.1,<23.2"
 ipython = ">=8.9,<8.10"
 ipykernel = ">=6.21,<6.22"
 poetry-dotenv = "0.3.0"
 poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21,<0.22"}
@@ -50,11 +61,12 @@
 pytest-cov = ">=4.0,<4.1"
 notebook = ">=6.5,<6.6"
 torchinfo = ">=1.7,<1.8"
 
 [tool.poetry.extras]
 onnxruntime = ["onnxruntime"]
 onnxruntime-gpu = ["onnxruntime-gpu"]
+worker = ["loguru", "ddtrace", "datadog", "Pillow", "chitra", "datasets", "celery", "accelerate", "bitsandbytes"]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `cerebrium-0.4.9/PKG-INFO` & `cerebrium-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 0.4.9
+Version: 0.5.0
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: onnxruntime
 Provides-Extra: onnxruntime-gpu
+Provides-Extra: worker
+Requires-Dist: Pillow (>=9.4,<10.0.0) ; extra == "worker"
+Requires-Dist: accelerate (>=0.18.0,<0.19.0) ; extra == "worker"
 Requires-Dist: arize (>=6.0.2,<7.0)
+Requires-Dist: bitsandbytes (>=0.38.0,<0.39.0) ; extra == "worker"
+Requires-Dist: boto3 (>=1.26.96,<2.0.0)
+Requires-Dist: celery (>=5.2.0,<5.3.0) ; extra == "worker"
 Requires-Dist: censius (>=1.6,<2.0)
+Requires-Dist: chitra (>=0.2.0,<0.3.0) ; extra == "worker"
 Requires-Dist: cloudpickle (>=2.0,<2.1)
-Requires-Dist: numpy (>=1.23,<1.25)
-Requires-Dist: onnxruntime (>=1.13,<1.15) ; extra == "onnxruntime"
-Requires-Dist: onnxruntime-gpu (>=1.14,<1.15) ; extra == "onnxruntime-gpu"
-Requires-Dist: pandas (>=1.5,<1.6)
-Requires-Dist: requests (>=2.28,<2.29)
-Requires-Dist: scikit-learn (>=1.2,<1.3)
-Requires-Dist: spacy (>=3.5.0,<3.6.0)
+Requires-Dist: datadog (>=0.45.0,<0.51.0) ; extra == "worker"
+Requires-Dist: datasets (>=2.10.0,<2.11.0) ; extra == "worker"
+Requires-Dist: ddtrace (>=1.10.0,<1.11.0) ; extra == "worker"
+Requires-Dist: loguru (>=0.5,<0.6) ; extra == "worker"
+Requires-Dist: numpy (>=1.20,<2.0)
+Requires-Dist: onnxruntime (>=1.13,<2.0) ; extra == "onnxruntime"
+Requires-Dist: onnxruntime-gpu (>=1.14,<2.0) ; extra == "onnxruntime-gpu"
+Requires-Dist: pandas (>=1.5,<3.0)
+Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: scikit-learn (>=1.2,<2.0)
+Requires-Dist: spacy (>=3.5.0,<4.0.0)
 Requires-Dist: tenacity (>=8.2,<8.3)
-Requires-Dist: torch (>=1.13,<1.14)
+Requires-Dist: torch (>=1.13,<3.0)
 Requires-Dist: tqdm (>=4.64,<4.65)
-Requires-Dist: transformers (>=4.26,<4.27)
-Requires-Dist: xgboost (>=1.7,<1.8)
+Requires-Dist: transformers (>=4.26,<5.0)
+Requires-Dist: xgboost (>=1.7,<2.0)
 Requires-Dist: yaspin (>=2.3,<2.4)
 Project-URL: Documentation, https://docs.cerebrium.ai/
 Project-URL: Homepage, https://www.cerebrium.ai
 Description-Content-Type: text/markdown
 
 # Cerebrium
 
@@ -105,17 +116,10 @@
 aws codeartifact login --tool pip --repository cerebrium-pypi --domain cerebrium --domain-owner 288552132534 --region eu-west-1
 ```
 Then, pip install:
 ```bash
 pip install --pre cerebrium
 ```
 
-## Exporting Requirements for Cerebrium Server
-You should export the requirements for the Cerebrium server by running the following command:
-```bash
-poetry export >> cerebrium-requirements.txt
-```
-Once this is done, add them to the `cerebrium-conduit-server` repo.
-
 ### Resources for Poetry/CodeArtifact
 - https://repost.aws/questions/QURD7aFNj_R9-8odJY5mfgrw/npm-publish-for-a-package-to-aws-code-artifact-repo-fails-with-error-the-provided-package-is-configured-to-block-new-version-publishes
 - https://docs.aws.amazon.com/codeartifact/latest/ug/python-configure-pip.html
```

