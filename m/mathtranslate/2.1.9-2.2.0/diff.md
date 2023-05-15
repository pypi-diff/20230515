# Comparing `tmp/mathtranslate-2.1.9.tar.gz` & `tmp/mathtranslate-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.1.9.tar", last modified: Mon Apr  3 02:34:30 2023, max compression
+gzip compressed data, was "mathtranslate-2.2.0.tar", last modified: Mon May 15 01:29:50 2023, max compression
```

## Comparing `mathtranslate-2.1.9.tar` & `mathtranslate-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/tencent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/mathtranslate/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-03 02:34:30.000000 mathtranslate-2.1.9/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 02:34:30.210226 mathtranslate-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-03 02:34:05.000000 mathtranslate-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.237236 mathtranslate-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-15 01:29:50.237236 mathtranslate-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.233236 mathtranslate-2.2.0/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.233236 mathtranslate-2.2.0/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.233236 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.233236 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.237236 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.237236 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.237236 mathtranslate-2.2.0/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.237236 mathtranslate-2.2.0/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:29:50.233236 mathtranslate-2.2.0/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-15 01:29:50.000000 mathtranslate-2.2.0/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-15 01:29:50.000000 mathtranslate-2.2.0/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:29:50.000000 mathtranslate-2.2.0/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-15 01:29:50.000000 mathtranslate-2.2.0/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 01:29:50.000000 mathtranslate-2.2.0/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 01:29:50.000000 mathtranslate-2.2.0/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 01:29:50.237236 mathtranslate-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-15 01:29:34.000000 mathtranslate-2.2.0/setup.py
```

### Comparing `mathtranslate-2.1.9/LICENSE` & `mathtranslate-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.1.9/PKG-INFO` & `mathtranslate-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.1.9
+Version: 2.2.0
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
-Author: Jiace Sun
+Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MathTranslate
@@ -43,32 +43,28 @@
 </p>
 
 <p float="left">
 <img src="https://github.com/SUSYUSTC/MathTranslate/blob/main/example/screenshot.png" width="300">
 <img src="https://github.com/SUSYUSTC/MathTranslate/blob/main/example/translated.png" width="400">
 </p>
 
-Although it is currently a small project, we are aware that this project has received much more attention that we expected. We are planning more developments for better user experience.
-
 ## Releases
 ### Mar 24, 2023
 We add the ability to directly translate arxiv papers.
 ### Mar 21, 2023
 We add tencent translation option for users with IP in China mainland.
 ### Mar 16, 2023
 We are now supporting all operating systems! Now you can install simply by `pip install --upgrade mathtranslate`.
 
 ## Requirements
 1. Python3 and pip. [Anaconda](https://www.anaconda.com) is recommended.
 2. (For users with IP in Mainland China): [Tencent Translation API](https://cloud.tencent.com/product/tmt) account. After registration, you can get the secret ID (not the APP ID!) and secret Key in [Tencent Console](https://console.cloud.tencent.com/cam/capi). Tencent Translate is the translation API with the highest free quota to our knowledge besides Google Translate, with a free quota of 5 million characters per month, and no fee will be deducted if there is no manual recharge (that is, there is no need to worry about misuse).
 
 ## Installation & Update
-`pip install --upgrade mathtranslate -i https://pypi.org/simple`
-
-**We suggest the users to always check update before using because we update frequently**
+`pip install --upgrade mathtranslate`
 
 ## Usage
 1. Prepare or generate a tex file. You can get the tex file by the following two ways:
      - For most [arxiv](https://arxiv.org/) papers, you can download the latex source code (Download - Other formats - Source). If the file you downloaded has no suffix, in most cases it is in .tar format, you may need to add the suffix manually. After decompression you can get a latex project, and then you can translate the .tex files in it.
      - Use [mathpix](https://mathpix.com/) to convert the pdf you want to translate into latex code. mathpix can directly convert pdf page into latex code or convert screenshots into code. We can handle both of these methods. Unfortunately, mathpix charges after a certain amount of usage, here is the [price](https://mathpix.com/pricing).
 2. (Tencent Translate API users) run `translate_tex --setkey` to store the API secretID and secretKey.
 3. Translate the tex file by `translate_tex input.tex -o output.tex`.
```

#### html2text {}

```diff
@@ -1,70 +1,67 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.1.9 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.0 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
-Jiace Sun Author-email: susyustc@gmail.com Classifier: Programming Language ::
-Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE # MathTranslate
+MathTranslate developers Author-email: susyustc@gmail.com Classifier:
+Programming Language :: Python :: 3 Classifier: Operating System :: OS
+Independent Description-Content-Type: text/markdown License-File: LICENSE #
+MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
                                   [logo.jpg]
                             English | ç®ä½ä¸­æ
 This is a project to provide translation of scientific papers with heavy math
 symbols from any language to any language while keeping the math symbols
 unchanged. In most translation softwares you wouldn't be able to keep equations
 and it would annoy you. The main work of this project is to translate LaTex
 files based on Google Translate in plain text, and finally realize the
 translation of pdf. Here's an example of what you get finally.
 [https://user-images.githubusercontent.com/30529122/227698548-1cc19f7c-00e7-
 4312-9d58-2a7237656b51.png]
 [https://github.com/SUSYUSTC/MathTranslate/blob/main/example/screenshot.png]
 [https://github.com/SUSYUSTC/MathTranslate/blob/main/example/translated.png]
-Although it is currently a small project, we are aware that this project has
-received much more attention that we expected. We are planning more
-developments for better user experience. ## Releases ### Mar 24, 2023 We add
-the ability to directly translate arxiv papers. ### Mar 21, 2023 We add tencent
-translation option for users with IP in China mainland. ### Mar 16, 2023 We are
-now supporting all operating systems! Now you can install simply by `pip
-install --upgrade mathtranslate`. ## Requirements 1. Python3 and pip.
-[Anaconda](https://www.anaconda.com) is recommended. 2. (For users with IP in
-Mainland China): [Tencent Translation API](https://cloud.tencent.com/product/
-tmt) account. After registration, you can get the secret ID (not the APP ID!)
-and secret Key in [Tencent Console](https://console.cloud.tencent.com/cam/
-capi). Tencent Translate is the translation API with the highest free quota to
-our knowledge besides Google Translate, with a free quota of 5 million
-characters per month, and no fee will be deducted if there is no manual
-recharge (that is, there is no need to worry about misuse). ## Installation &
-Update `pip install --upgrade mathtranslate -i https://pypi.org/simple` **We
-suggest the users to always check update before using because we update
-frequently** ## Usage 1. Prepare or generate a tex file. You can get the tex
-file by the following two ways: - For most [arxiv](https://arxiv.org/) papers,
-you can download the latex source code (Download - Other formats - Source). If
-the file you downloaded has no suffix, in most cases it is in .tar format, you
-may need to add the suffix manually. After decompression you can get a latex
-project, and then you can translate the .tex files in it. - Use [mathpix]
-(https://mathpix.com/) to convert the pdf you want to translate into latex
-code. mathpix can directly convert pdf page into latex code or convert
-screenshots into code. We can handle both of these methods. Unfortunately,
-mathpix charges after a certain amount of usage, here is the [price](https://
-mathpix.com/pricing). 2. (Tencent Translate API users) run `translate_tex --
-setkey` to store the API secretID and secretKey. 3. Translate the tex file by
-`translate_tex input.tex -o output.tex`. 4. Compile your tex file. You can
-compile it with the [texlive](https://www.tug.org/texlive/) command `xelatex
-output.tex`. For Chinese you need the xeCJK package. If it is a downloaded
-arxiv project, we recommend compressing all files into a zip file and uploading
-it to [overleaf](https://www.overleaf.com/project) for online compilation.
-**Note, you need to set the XeLatex compiler in `Menu - Compiler`, otherwise it
-cannot handle other languages.** 5. You can change the default settings of the
-translation language and engine through the command line arguments `-engine`,
-`-from`, `-to`. For example `translate_tex -engine tencent input.tex -
-o output.tex`. You can also permanently change the setting via `translate_tex -
--setdefault`. You can see more details with `translate_tex --help`. ## Examples
-In the example directory, you can see `main.txt` which is the mathpix output of
-a part of `paper.pdf`. Run `translate_tex main.txt` and you will get the
-`main.tex` and `main.pdf`. `translated.png` is what you should expect to see in
-the `main.pdf`. ## Known Issues 1. If `\begin{env} \end{env}` is reset with
-`\newcommand` in latex, it will not be translated correctly. 2. There is a
-small probability to get something like "XMATHX_1_2" or wrong formula during
-translation. The accuracy rate of Tencent translation is slightly lower than
-that of Google translation. ## Further developments 1. Fix bugs in the latex
-translations. 2. A more user-friendly interface. If you have any questions or
-have interests in making contributions, please contact me by susyustc@gmail.com
-or joining QQ group 288646946.
+## Releases ### Mar 24, 2023 We add the ability to directly translate arxiv
+papers. ### Mar 21, 2023 We add tencent translation option for users with IP in
+China mainland. ### Mar 16, 2023 We are now supporting all operating systems!
+Now you can install simply by `pip install --upgrade mathtranslate`. ##
+Requirements 1. Python3 and pip. [Anaconda](https://www.anaconda.com) is
+recommended. 2. (For users with IP in Mainland China): [Tencent Translation
+API](https://cloud.tencent.com/product/tmt) account. After registration, you
+can get the secret ID (not the APP ID!) and secret Key in [Tencent Console]
+(https://console.cloud.tencent.com/cam/capi). Tencent Translate is the
+translation API with the highest free quota to our knowledge besides Google
+Translate, with a free quota of 5 million characters per month, and no fee will
+be deducted if there is no manual recharge (that is, there is no need to worry
+about misuse). ## Installation & Update `pip install --upgrade mathtranslate`
+## Usage 1. Prepare or generate a tex file. You can get the tex file by the
+following two ways: - For most [arxiv](https://arxiv.org/) papers, you can
+download the latex source code (Download - Other formats - Source). If the file
+you downloaded has no suffix, in most cases it is in .tar format, you may need
+to add the suffix manually. After decompression you can get a latex project,
+and then you can translate the .tex files in it. - Use [mathpix](https://
+mathpix.com/) to convert the pdf you want to translate into latex code. mathpix
+can directly convert pdf page into latex code or convert screenshots into code.
+We can handle both of these methods. Unfortunately, mathpix charges after a
+certain amount of usage, here is the [price](https://mathpix.com/pricing). 2.
+(Tencent Translate API users) run `translate_tex --setkey` to store the API
+secretID and secretKey. 3. Translate the tex file by `translate_tex input.tex -
+o output.tex`. 4. Compile your tex file. You can compile it with the [texlive]
+(https://www.tug.org/texlive/) command `xelatex output.tex`. For Chinese you
+need the xeCJK package. If it is a downloaded arxiv project, we recommend
+compressing all files into a zip file and uploading it to [overleaf](https://
+www.overleaf.com/project) for online compilation. **Note, you need to set the
+XeLatex compiler in `Menu - Compiler`, otherwise it cannot handle other
+languages.** 5. You can change the default settings of the translation language
+and engine through the command line arguments `-engine`, `-from`, `-to`. For
+example `translate_tex -engine tencent input.tex -o output.tex`. You can also
+permanently change the setting via `translate_tex --setdefault`. You can see
+more details with `translate_tex --help`. ## Examples In the example directory,
+you can see `main.txt` which is the mathpix output of a part of `paper.pdf`.
+Run `translate_tex main.txt` and you will get the `main.tex` and `main.pdf`.
+`translated.png` is what you should expect to see in the `main.pdf`. ## Known
+Issues 1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it
+will not be translated correctly. 2. There is a small probability to get
+something like "XMATHX_1_2" or wrong formula during translation. The accuracy
+rate of Tencent translation is slightly lower than that of Google translation.
+## Further developments 1. Fix bugs in the latex translations. 2. A more user-
+friendly interface. If you have any questions or have interests in making
+contributions, please contact me by susyustc@gmail.com or joining QQ group
+288646946.
```

### Comparing `mathtranslate-2.1.9/README.md` & `mathtranslate-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,32 +31,28 @@
 </p>
 
 <p float="left">
 <img src="https://github.com/SUSYUSTC/MathTranslate/blob/main/example/screenshot.png" width="300">
 <img src="https://github.com/SUSYUSTC/MathTranslate/blob/main/example/translated.png" width="400">
 </p>
 
-Although it is currently a small project, we are aware that this project has received much more attention that we expected. We are planning more developments for better user experience.
-
 ## Releases
 ### Mar 24, 2023
 We add the ability to directly translate arxiv papers.
 ### Mar 21, 2023
 We add tencent translation option for users with IP in China mainland.
 ### Mar 16, 2023
 We are now supporting all operating systems! Now you can install simply by `pip install --upgrade mathtranslate`.
 
 ## Requirements
 1. Python3 and pip. [Anaconda](https://www.anaconda.com) is recommended.
 2. (For users with IP in Mainland China): [Tencent Translation API](https://cloud.tencent.com/product/tmt) account. After registration, you can get the secret ID (not the APP ID!) and secret Key in [Tencent Console](https://console.cloud.tencent.com/cam/capi). Tencent Translate is the translation API with the highest free quota to our knowledge besides Google Translate, with a free quota of 5 million characters per month, and no fee will be deducted if there is no manual recharge (that is, there is no need to worry about misuse).
 
 ## Installation & Update
-`pip install --upgrade mathtranslate -i https://pypi.org/simple`
-
-**We suggest the users to always check update before using because we update frequently**
+`pip install --upgrade mathtranslate`
 
 ## Usage
 1. Prepare or generate a tex file. You can get the tex file by the following two ways:
      - For most [arxiv](https://arxiv.org/) papers, you can download the latex source code (Download - Other formats - Source). If the file you downloaded has no suffix, in most cases it is in .tar format, you may need to add the suffix manually. After decompression you can get a latex project, and then you can translate the .tex files in it.
      - Use [mathpix](https://mathpix.com/) to convert the pdf you want to translate into latex code. mathpix can directly convert pdf page into latex code or convert screenshots into code. We can handle both of these methods. Unfortunately, mathpix charges after a certain amount of usage, here is the [price](https://mathpix.com/pricing).
 2. (Tencent Translate API users) run `translate_tex --setkey` to store the API secretID and secretKey.
 3. Translate the tex file by `translate_tex input.tex -o output.tex`.
```

#### html2text {}

```diff
@@ -9,58 +9,54 @@
 and it would annoy you. The main work of this project is to translate LaTex
 files based on Google Translate in plain text, and finally realize the
 translation of pdf. Here's an example of what you get finally.
 [https://user-images.githubusercontent.com/30529122/227698548-1cc19f7c-00e7-
 4312-9d58-2a7237656b51.png]
 [https://github.com/SUSYUSTC/MathTranslate/blob/main/example/screenshot.png]
 [https://github.com/SUSYUSTC/MathTranslate/blob/main/example/translated.png]
-Although it is currently a small project, we are aware that this project has
-received much more attention that we expected. We are planning more
-developments for better user experience. ## Releases ### Mar 24, 2023 We add
-the ability to directly translate arxiv papers. ### Mar 21, 2023 We add tencent
-translation option for users with IP in China mainland. ### Mar 16, 2023 We are
-now supporting all operating systems! Now you can install simply by `pip
-install --upgrade mathtranslate`. ## Requirements 1. Python3 and pip.
-[Anaconda](https://www.anaconda.com) is recommended. 2. (For users with IP in
-Mainland China): [Tencent Translation API](https://cloud.tencent.com/product/
-tmt) account. After registration, you can get the secret ID (not the APP ID!)
-and secret Key in [Tencent Console](https://console.cloud.tencent.com/cam/
-capi). Tencent Translate is the translation API with the highest free quota to
-our knowledge besides Google Translate, with a free quota of 5 million
-characters per month, and no fee will be deducted if there is no manual
-recharge (that is, there is no need to worry about misuse). ## Installation &
-Update `pip install --upgrade mathtranslate -i https://pypi.org/simple` **We
-suggest the users to always check update before using because we update
-frequently** ## Usage 1. Prepare or generate a tex file. You can get the tex
-file by the following two ways: - For most [arxiv](https://arxiv.org/) papers,
-you can download the latex source code (Download - Other formats - Source). If
-the file you downloaded has no suffix, in most cases it is in .tar format, you
-may need to add the suffix manually. After decompression you can get a latex
-project, and then you can translate the .tex files in it. - Use [mathpix]
-(https://mathpix.com/) to convert the pdf you want to translate into latex
-code. mathpix can directly convert pdf page into latex code or convert
-screenshots into code. We can handle both of these methods. Unfortunately,
-mathpix charges after a certain amount of usage, here is the [price](https://
-mathpix.com/pricing). 2. (Tencent Translate API users) run `translate_tex --
-setkey` to store the API secretID and secretKey. 3. Translate the tex file by
-`translate_tex input.tex -o output.tex`. 4. Compile your tex file. You can
-compile it with the [texlive](https://www.tug.org/texlive/) command `xelatex
-output.tex`. For Chinese you need the xeCJK package. If it is a downloaded
-arxiv project, we recommend compressing all files into a zip file and uploading
-it to [overleaf](https://www.overleaf.com/project) for online compilation.
-**Note, you need to set the XeLatex compiler in `Menu - Compiler`, otherwise it
-cannot handle other languages.** 5. You can change the default settings of the
-translation language and engine through the command line arguments `-engine`,
-`-from`, `-to`. For example `translate_tex -engine tencent input.tex -
-o output.tex`. You can also permanently change the setting via `translate_tex -
--setdefault`. You can see more details with `translate_tex --help`. ## Examples
-In the example directory, you can see `main.txt` which is the mathpix output of
-a part of `paper.pdf`. Run `translate_tex main.txt` and you will get the
-`main.tex` and `main.pdf`. `translated.png` is what you should expect to see in
-the `main.pdf`. ## Known Issues 1. If `\begin{env} \end{env}` is reset with
-`\newcommand` in latex, it will not be translated correctly. 2. There is a
-small probability to get something like "XMATHX_1_2" or wrong formula during
-translation. The accuracy rate of Tencent translation is slightly lower than
-that of Google translation. ## Further developments 1. Fix bugs in the latex
-translations. 2. A more user-friendly interface. If you have any questions or
-have interests in making contributions, please contact me by susyustc@gmail.com
-or joining QQ group 288646946.
+## Releases ### Mar 24, 2023 We add the ability to directly translate arxiv
+papers. ### Mar 21, 2023 We add tencent translation option for users with IP in
+China mainland. ### Mar 16, 2023 We are now supporting all operating systems!
+Now you can install simply by `pip install --upgrade mathtranslate`. ##
+Requirements 1. Python3 and pip. [Anaconda](https://www.anaconda.com) is
+recommended. 2. (For users with IP in Mainland China): [Tencent Translation
+API](https://cloud.tencent.com/product/tmt) account. After registration, you
+can get the secret ID (not the APP ID!) and secret Key in [Tencent Console]
+(https://console.cloud.tencent.com/cam/capi). Tencent Translate is the
+translation API with the highest free quota to our knowledge besides Google
+Translate, with a free quota of 5 million characters per month, and no fee will
+be deducted if there is no manual recharge (that is, there is no need to worry
+about misuse). ## Installation & Update `pip install --upgrade mathtranslate`
+## Usage 1. Prepare or generate a tex file. You can get the tex file by the
+following two ways: - For most [arxiv](https://arxiv.org/) papers, you can
+download the latex source code (Download - Other formats - Source). If the file
+you downloaded has no suffix, in most cases it is in .tar format, you may need
+to add the suffix manually. After decompression you can get a latex project,
+and then you can translate the .tex files in it. - Use [mathpix](https://
+mathpix.com/) to convert the pdf you want to translate into latex code. mathpix
+can directly convert pdf page into latex code or convert screenshots into code.
+We can handle both of these methods. Unfortunately, mathpix charges after a
+certain amount of usage, here is the [price](https://mathpix.com/pricing). 2.
+(Tencent Translate API users) run `translate_tex --setkey` to store the API
+secretID and secretKey. 3. Translate the tex file by `translate_tex input.tex -
+o output.tex`. 4. Compile your tex file. You can compile it with the [texlive]
+(https://www.tug.org/texlive/) command `xelatex output.tex`. For Chinese you
+need the xeCJK package. If it is a downloaded arxiv project, we recommend
+compressing all files into a zip file and uploading it to [overleaf](https://
+www.overleaf.com/project) for online compilation. **Note, you need to set the
+XeLatex compiler in `Menu - Compiler`, otherwise it cannot handle other
+languages.** 5. You can change the default settings of the translation language
+and engine through the command line arguments `-engine`, `-from`, `-to`. For
+example `translate_tex -engine tencent input.tex -o output.tex`. You can also
+permanently change the setting via `translate_tex --setdefault`. You can see
+more details with `translate_tex --help`. ## Examples In the example directory,
+you can see `main.txt` which is the mathpix output of a part of `paper.pdf`.
+Run `translate_tex main.txt` and you will get the `main.tex` and `main.pdf`.
+`translated.png` is what you should expect to see in the `main.pdf`. ## Known
+Issues 1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it
+will not be translated correctly. 2. There is a small probability to get
+something like "XMATHX_1_2" or wrong formula during translation. The accuracy
+rate of Tencent translation is slightly lower than that of Google translation.
+## Further developments 1. Fix bugs in the latex translations. 2. A more user-
+friendly interface. If you have any questions or have interests in making
+contributions, please contact me by susyustc@gmail.com or joining QQ group
+288646946.
```

### Comparing `mathtranslate-2.1.9/mathtranslate/process_latex.py` & `mathtranslate-2.2.0/mathtranslate/process_latex.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 import re
 import regex
-from .config import math_code, test_environment
+from .config import config
+math_code = config.math_code
+test_environment = config.test_environment
 
 match_code = r"(" + math_code + r"_\d+(?:_\d+)*)"
 match_code_replace = math_code + r"_(\d+(?:_\d+)*)*"
 
 #options = r"\[[a-zA-Z\s,\\\*\.\+\-=_{}\(\)\!]*?\]"  # ,\*.+-=_{}!
 options = r"\[.*?\]"
 spaces = r"[ \t]*"
 
 get_pattern_brace = lambda index: rf"\{{((?:[^{{}}]++|(?{index}))++)\}}"
-get_pattern_env = lambda name: rf"\\begin{spaces}\{{({name})\}}{spaces}({options})?(.*?)\\end{spaces}\{{\1\}}".replace('options', options)
-get_pattern_command_full = lambda name: rf'\\({name}){spaces}({options})?{spaces}({get_pattern_brace(3)})'
+get_pattern_env = lambda name: rf"\\begin{spaces}\{{({name})\}}{spaces}({options})?(.*?)\\end{spaces}\{{\1\}}"
+
+
+def get_pattern_command_full(name, n=None):
+    pattern = rf'\\({name})'
+    if n is None:
+        pattern += rf'{spaces}({options})?'
+        n = 1
+        begin_brace = 3
+    else:
+        begin_brace = 2
+    for i in range(n):
+        tmp = get_pattern_brace(i*2+begin_brace)
+        pattern += rf'{spaces}({tmp})'
+    if n == 0:
+        pattern += r'(?=[^a-zA-Z])'
+    return pattern
+
+
 match_command_name = r'[a-zA-Z]+\*?'
 
 pattern_env = get_pattern_env(r'.*?')  # \begin{xxx} \end{xxx}, group 1: name, group 2: option, group 3: content
 pattern_command_full = get_pattern_command_full(match_command_name)   # \xxx[xxx]{xxx} and \xxx{xxx}, group 1: name, group 2: option, group 4: content
 pattern_command_simple = rf'\\({match_command_name})'  # \xxx, group 1: name
 pattern_brace = get_pattern_brace(0)  # {xxx}, group 1: content
+pattern_newcommand = rf'\\(?:newcommand|def){spaces}(?:\{{\\([a-zA-Z]+)\}}|\\([a-zA-Z]+)){spaces}(?:\[(\d)\])?{spaces}({get_pattern_brace(4)})'  # \newcommand{name}[n_arguments]{content}, group 1/2: name, group 3: n_arguments, group 5: content
 
 pattern_theorem = r"\\newtheorem[ \t]*\{(.+?)\}"  # \newtheorem{xxx}, group 1: name
 pattern_accent = r"\\([`'\"^~=.])(?:\{([a-zA-Z])\}|([a-zA-Z]))"  # match special characters with accents, group 1: accent, group 2/3: normal character
-match_code_accent = rf'{math_code}([A-Z]{{2}})([a-zA-Z])'  # group 1: accent name, group 2: normal character
+match_code_accent = rf'{math_code}([A-Z]{{2}})([a-zA-Z])'  # group 1: accent name, group 2: normal character, e.g. \"o or \"{o}
 list_special = ['\\', '%', '&', '#', '$', '{', '}', ' ']  # all special characters in form of \x
 
 special_character_forward = {
     '\\': 'BS',
     '%': 'PC',
     '&': 'AD',
     '#': 'NB',
@@ -75,35 +95,37 @@
 def modify_after(text):
     # the "_" in the text should be replaced to "\_"
     pattern = r"(?<!\\)_"
     text = re.sub(pattern, r"\\_", text)
     return text
 
 
-def replace_latex_objects(text):
+def replace_latex_objects(text, brace=True):
     r"""
     Replaces all LaTeX objects in a given text with the format "{math_code}_{digit1}_{digit2}_..._{digit_last}",
     applies a given function to the resulting text (excluding the "{math_code}_{digit1}_{digit2}_..._{digit_last}" parts),
     and returns both the processed text and a list of replaced LaTeX objects.
     Supported LaTeX objects: \[ xxx \], \begin{xxx} \end{xxx}, $$ $$,
     $ $, \( xxx \), \xxx[xxx]{xxx}, \xxx{xxx}, and \xxx.
     Returns the processed text and a list of replaced LaTeX objects.
     """
 
+    # You need to make sure that the input does not contain {math_code}
     # define regular expressions for each LaTeX object
     latex_obj_regex = [
         r"\$\$(.*?)\$\$",  # $$ $$
         r"\$(.*?)\$",  # $ $
         r"\\\[(.*?)\\\]",  # \[ xxx \]
         r"\\\((.*?)\\\)",  # \( xxx \)
         pattern_env,  # \begin{xxx} \end{xxx}
         pattern_command_full,  # \xxx[xxx]{xxx}
         pattern_command_simple,  # \xxx
-        pattern_brace,  # {xxx}
     ]
+    if brace:
+        latex_obj_regex.append(pattern_brace)
 
     # iterate through each LaTeX object and replace with "{math_code}_{digit1}_{digit2}_..._{digit_last}"
     count = 0
     replaced_objs = []
     for regex_symbol in latex_obj_regex:
         pattern = regex.compile(regex_symbol, regex.DOTALL)
         while pattern.search(text):
@@ -112,30 +134,32 @@
             text = pattern.sub(' ' + variable_code(count) + ' ', text, 1)
             count += 1
 
     text = modify_text(text, modify_before)
     return text, replaced_objs
 
 
-def recover_latex_objects(text, replaced_objs, final=False):
+def recover_latex_objects(text, replaced_objs, tolerate_error=False):
+    # recover the latex objects from "replace_latex_objects"
     nobjs = len(replaced_objs)
     matched_indices = []
 
     def get_obj(digit_str):
         index = int(''.join(digit_str.split('_')))
         matched_indices.append(index)
         if index < nobjs:
             return replaced_objs[index]
         else:
             if test_environment:
-                assert final
+                assert tolerate_error
             return '???'
 
     text = modify_text(text, modify_after)
     pattern = re.compile(match_code_replace)
+    # count number of mismatch
     total_num = 0
     while True:
         text, num_modify = pattern.subn(lambda match: get_obj(match.group(1)), text)
         total_num += num_modify
         if num_modify == 0:
             break
     n_good = len(set(matched_indices).intersection(set(range(nobjs))))
@@ -170,63 +194,81 @@
     pre = text[:begin_doc_index + len(begin_code)]
     body = text[begin_doc_index + len(begin_code):end_doc_index]
     post = text[end_doc_index:]
     return body, pre, post
 
 
 def process_specific_env(latex, function, env_name):
+    # find all patterns of \begin{env_name}[options] content \end{env_name}
+    # then replace `content` by `function(content)`
     pattern = regex.compile(get_pattern_env(env_name), regex.DOTALL)
 
     def process_function(match):
-        # \begin{env_name}[options] content \end{env_name}
         name = match.group(1)
         assert re.match(env_name, name)
         options = match.group(2)
         if options is None:
             options = ''
         content = match.group(3)
         processed_content = function(content)
         return rf'\begin{{{env_name}}}{options}{processed_content}\end{{{env_name}}}'
     return pattern.sub(process_function, latex)
 
 
 def process_specific_command(latex, function, command_name):
+    # find all patterns of # \{command_name}[options]{content}
+    # then replace `content` by `function(content)`
     pattern = regex.compile(get_pattern_command_full(command_name), regex.DOTALL)
 
     def process_function(match):
-        # \{command_name}[options]{content}
         name = match.group(1)
         assert re.match(command_name, name)
         options = match.group(2)
         if options is None:
             options = ''
         content = match.group(4)
         processed_content = function(content)
         return rf'\{command_name}{options}{{{processed_content}}}'
     return pattern.sub(process_function, latex)
 
 
+def process_leading_level_brace(latex, function):
+    # leading level means that the {xxx} is not inside other objects, i.e. \command{} or \begin{xxx} \end{xxx}
+    # replace `{ content }` by `{ function(content) }`
+    text, envs = replace_latex_objects(latex, brace=False)
+
+    def process_function(match):
+        content = match.group(1)
+        # function here is translate_paragraph_latex, which cannot contain replaced environments
+        processed_content = function(recover_latex_objects(content, envs)[0])
+        return rf'{{ {processed_content} }}'
+
+    text = regex.compile(pattern_brace, regex.DOTALL).sub(process_function, text)
+    latex = recover_latex_objects(text, envs)[0]
+    return latex
+
+
 def remove_blank_lines(text):
     pattern = re.compile(r'\n\n+')
     text = pattern.sub('\n', text)
     return text
 
 
 def insert_macro(text, macro):
-    pattern = re.compile(r"\\documentclass(\[.*?\])?\{(.*?)\}", re.DOTALL)
+    pattern = re.compile(r"\\document(class|style)(\[.*?\])?\{(.*?)\}", re.DOTALL)
     match = pattern.search(text)
     assert match is not None
     start, end = match.span()
     new_text = text[:end] + f"\n{macro}\n" + text[end:]
     return new_text
 
 
 def is_complete(latex_code):
     # Define regular expressions for \documentclass, \begin{document}, and \end{document}
-    documentclass_pattern = re.compile(r"\\documentclass(\[.*?\])?\{.*?\}", re.DOTALL)
+    documentclass_pattern = re.compile(r"\\document(class|style)(\[.*?\])?\{.*?\}", re.DOTALL)
     begin_pattern = re.compile(r"\\begin\{document\}")
     end_pattern = re.compile(r"\\end\{document\}")
 
     # Check if \documentclass is present
     if not documentclass_pattern.search(latex_code):
         return False
 
@@ -252,14 +294,20 @@
 def get_theorems(text):
     pattern = re.compile(pattern_theorem, re.DOTALL)
     matches = re.finditer(pattern, text)
     theorems = [match.group(1) for match in matches]
     return theorems
 
 
+def get_nonNone(*args):
+    result = [arg for arg in args if arg is not None]
+    assert len(result) == 1
+    return result[0]
+
+
 def replace_special(text):
     for special in list_special:
         # add space around
         text = text.replace(f'\\{special}', f' {math_code}{special_character_forward[special]} ')
 
     return text
 
@@ -269,23 +317,20 @@
         text = text.replace(math_code + special_character_forward[special], f'\\{special}')
 
     return text
 
 
 def replace_accent(text):
     def replace_function(match):
+        # if it is \"{o}, then special is ", char1 is o, char2 is None
+        # if it is \"o, then special is ", char1 is None, char2 is o
         special = match.group(1)
         char1 = match.group(2)
         char2 = match.group(3)
-        if char1 is None:
-            assert char2 is not None
-            char = char2
-        else:
-            assert char2 is None
-            char = char1
+        char = get_nonNone(char1, char2)
         # do not add space around
         return math_code + special_character_forward[special] + f'{char}'
 
     text = re.compile(pattern_accent).sub(replace_function, text)
 
     return text
 
@@ -298,18 +343,67 @@
 
     text = re.compile(match_code_accent).sub(replace_function, text)
 
     return text
 
 
 def combine_split_to_sentences(text):
+    # if two lines are separately by only one \n, in latex they are in the same paragraph so we combine them in the same line
+    # However we don't combine them if the second line does not start from normal letters (so usually some latex commands)
     n = len(math_code)
     pattern = re.compile(r'\n(\s*([^\s]+))')
 
     def process_function(match):
         string = match.group(2)
         if string[0:n] == math_code:
             return match.group(0)
         else:
-            return ' '+match.group(1)
+            return ' ' + match.group(1)
 
     return pattern.sub(process_function, text)
+
+
+def delete_specific_format(latex, format_name):
+    pattern = regex.compile(get_pattern_command_full(format_name), regex.DOTALL)
+    return pattern.sub(lambda m: m.group(4), latex)
+
+
+def replace_newcommand(newcommand, latex):
+    command_name, n_arguments, content = newcommand
+    pattern = regex.compile(get_pattern_command_full(command_name, n_arguments), regex.DOTALL)
+
+    def replace_function(match):
+        this_content = content
+        name = match.group(1)
+        assert re.match(command_name, name)
+        for i in range(n_arguments):
+            text = match.group(3 + i * 2)
+            this_content = this_content.replace(f'#{i+1}', f' {text} ')
+        return this_content
+
+    return pattern.sub(replace_function, latex)
+
+
+def process_newcommands(latex):
+    pattern = regex.compile(pattern_newcommand, regex.DOTALL)
+    count = 0
+    full_newcommands = []
+    while True:
+        match = pattern.search(latex)
+        if not match:
+            break
+        name1 = match.group(1)
+        name2 = match.group(2)
+        name = get_nonNone(name1, name2)
+        n_arguments = match.group(3)
+        if n_arguments is None:
+            n_arguments = 0
+        else:
+            n_arguments = int(n_arguments)
+        content = match.group(5)
+        latex = pattern.sub(f'XMATH_REPLACE{count}_NEWCOMMAND', latex, 1)
+        full_newcommands.append(match.group(0))
+        latex = replace_newcommand((name, n_arguments, content), latex)
+        count += 1
+    for i in range(count):
+        latex = latex.replace(f'XMATH_REPLACE{i}_NEWCOMMAND', full_newcommands[i])
+    return latex
```

### Comparing `mathtranslate-2.1.9/mathtranslate/process_text.py` & `mathtranslate-2.2.0/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.1.9/mathtranslate/translate.py` & `mathtranslate-2.2.0/mathtranslate/translate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 from . import process_latex
 from . import process_text
 from .process_text import char_limit
+from .encoding import get_file_encoding
 import time
 import re
 import tqdm
 
 default_begin = r'''
 \documentclass[UTF8]{article}
 \usepackage{xeCJK}
@@ -13,30 +14,33 @@
 \begin{document}
 '''
 default_end = r'''
 \end{document}
 '''
 
 # TODO: add more here
-environment_list = ['abstract', 'acknowledgments', 'itemize', 'enumerate', 'description', 'list', 'proof']
+environment_list = ['abstract', 'acknowledgments', 'itemize', 'enumerate', 'description', 'list', 'proof', 'quote']
 command_list = ['section', 'subsection', 'subsubsection', 'caption', 'subcaption', 'footnote', 'paragraph']
+format_list = ['textbf', 'textit', 'emph']
 
 
 class TextTranslator:
     def __init__(self, engine, language_to, language_from):
         if engine == 'google':
             import mtranslate as translator
         elif engine == 'tencent':
             from mathtranslate.tencent import Translator
             translator = Translator()
         else:
             assert False, "engine must be google or tencent"
         self.translator = translator
         self.language_to = language_to
         self.language_from = language_from
+        self.number_of_calls = 0
+        self.tot_char = 0
 
     def try_translate(self, text):
         return self.translator.translate(text, self.language_to, self.language_from)
 
     def translate(self, text):
         if not re.match(re.compile(r'.*[a-zA-Z].*', re.DOTALL), text):
             # no meaningful word inside
@@ -46,14 +50,16 @@
                 result = self.try_translate(text)
                 break
             except BaseException as e:
                 if hasattr(self.translator, "is_error_request_frequency") and self.translator.is_error_request_frequency(e):
                     time.sleep(0.5)
                 else:
                     raise e
+        self.number_of_calls += 1
+        self.tot_char += len(text)
         return result
 
 
 class LatexTranslator:
     def __init__(self, translator: TextTranslator, debug=False):
         self.translator = translator
         self.debug = debug
@@ -87,18 +93,23 @@
         parts.append(part)
         parts_translated = []
         for part in parts:
             parts_translated.append(self.translator.translate(part))
         text_translated = '\n'.join(parts_translated)
         return text_translated.replace("\u200b", "")
 
-    def translate_paragraph_latex(self, latex_original_paragraph):
+    def translate_text_in_paragraph_latex(self, latex_original_paragraph):
         '''
         Translate a latex paragraph, which means that it could contain latex objects
         '''
+
+        # remove format about textbf, emph and textit
+        for format_name in format_list:
+            latex_original_paragraph = process_latex.delete_specific_format(latex_original_paragraph, format_name)
+
         text_original_paragraph, objs = process_latex.replace_latex_objects(latex_original_paragraph)
         # Since \n is equivalent to space in latex, we change \n back to space
         # otherwise the translators view them as separate sentences
         text_original_paragraph = process_latex.combine_split_to_sentences(text_original_paragraph)
         text_original_paragraph = process_text.split_too_long_paragraphs(text_original_paragraph)
         if not self.complete:
             text_original_paragraph = process_text.split_titles(text_original_paragraph)
@@ -111,93 +122,122 @@
         if self.debug:
             print(f'\n\nParagraph {self.num}\n\n', file=self.f_new)
             print(text_translated_paragraph, file=self.f_new)
             print(f'\n\nParagraph {self.num}\n\n', file=self.f_obj)
             for i, obj in enumerate(objs):
                 print(f'obj {i}', file=self.f_obj)
                 print(obj, file=self.f_obj)
-        latex_translated_paragraph, nbad, ntotal = process_latex.recover_latex_objects(text_translated_paragraph, objs, final=True)
+        latex_translated_paragraph, nbad, ntotal = process_latex.recover_latex_objects(text_translated_paragraph, objs, tolerate_error=True)
         self.nbad += nbad
         self.ntotal += ntotal
         return latex_translated_paragraph
 
+    def translate_latex_all_objects(self, latex):
+        '''
+        Terminology:
+        env: '\\begin{xxx} \\end{xxx}'
+        command: '\\command[options]{text}
+        object: env or command
+        '''
+        translate_function = self.translate_text_in_paragraph_latex_and_leading_brace
+        for env_name in environment_list + self.theorems:
+            latex = process_latex.process_specific_env(latex, translate_function, env_name)
+            latex = process_latex.process_specific_env(latex, translate_function, env_name + r'\*')
+        for command_name in command_list:
+            latex = process_latex.process_specific_command(latex, translate_function, command_name)
+            latex = process_latex.process_specific_command(latex, translate_function, command_name + r'\*')
+        return latex
+
+    def translate_text_in_paragraph_latex_and_leading_brace(self, latex_original_paragraph):
+        # it acts recursively, i.e. it also translates braces inside braces
+        latex_translated_paragraph = self.translate_text_in_paragraph_latex(latex_original_paragraph)
+        latex_translated_paragraph = process_latex.process_leading_level_brace(latex_translated_paragraph, self.translate_text_in_paragraph_latex_and_leading_brace)
+        return latex_translated_paragraph
+
+    def translate_paragraph_latex(self, latex_original_paragraph):
+        latex_translated_paragraph = self.translate_text_in_paragraph_latex_and_leading_brace(latex_original_paragraph)
+        latex_translated_paragraph = self.translate_latex_all_objects(latex_translated_paragraph)
+        return latex_translated_paragraph
+
     def split_latex_to_paragraphs(self, latex):
         '''
         1. convert latex to text and objects
         2. split text
         3. convert text back to objects
         '''
         text, objs = process_latex.replace_latex_objects(latex)
         paragraphs_text = re.split(r'\n\n+', text)
         paragraphs_latex = [process_latex.recover_latex_objects(paragraph_text, objs)[0] for paragraph_text in paragraphs_text]
         return paragraphs_latex
 
-    def translate_latex_all_objects(self, latex, envs, commands):
-        '''
-        Terminology:
-        env: '\\begin{xxx} \\end{xxx}'
-        command: '\\command[options]{text}
-        object: env or command
-        '''
-        for env_name in envs:
-            latex = process_latex.process_specific_env(latex, self.translate_paragraph_latex, env_name)
-            latex = process_latex.process_specific_env(latex, self.translate_paragraph_latex, env_name + r'\*')
-        for command_name in commands:
-            latex = process_latex.process_specific_command(latex, self.translate_paragraph_latex, command_name)
-            latex = process_latex.process_specific_command(latex, self.translate_paragraph_latex, command_name + r'\*')
-        return latex
-
-    def translate_full_latex(self, latex_original):
+    def translate_full_latex(self, latex_original, make_complete=True):
         self.nbad = 0
         self.ntotal = 0
 
         latex_original = process_latex.remove_tex_comments(latex_original)
+        latex_original = process_latex.process_newcommands(latex_original)
 
         latex_original = process_latex.replace_accent(latex_original)
         latex_original = process_latex.replace_special(latex_original)
 
         self.complete = process_latex.is_complete(latex_original)
-        theorems = process_latex.get_theorems(latex_original)
+        self.theorems = process_latex.get_theorems(latex_original)
         if self.complete:
             print('It is a full latex document')
             latex_original, tex_begin, tex_end = process_latex.split_latex_document(latex_original, r'\begin{document}', r'\end{document}')
             tex_begin = process_latex.remove_blank_lines(tex_begin)
-            # TODO: change xeCJK to be compatible with other compiler & languages
             tex_begin = process_latex.insert_macro(tex_begin, r'\usepackage{xeCJK}')
         else:
             print('It is not a full latex document')
             latex_original = process_text.connect_paragraphs(latex_original)
-            tex_begin = default_begin
-            tex_end = default_end
+            if make_complete:
+                tex_begin = default_begin
+                tex_end = default_end
+            else:
+                tex_begin = ''
+                tex_end = ''
 
         latex_original_paragraphs = self.split_latex_to_paragraphs(latex_original)
         latex_translated_paragraphs = []
 
         self.num = 0
         for latex_original_paragraph in tqdm.tqdm(latex_original_paragraphs):
             try:
                 latex_translated_paragraph = self.translate_paragraph_latex(latex_original_paragraph)
-                latex_translated_paragraph = self.translate_latex_all_objects(latex_translated_paragraph, environment_list + theorems, command_list)
                 latex_translated_paragraphs.append(latex_translated_paragraph)
             except BaseException as e:
                 print('Error found in Parapragh', self.num)
                 print('Content')
                 print(latex_original_paragraph)
                 raise e
             self.num += 1
 
         latex_translated = '\n\n'.join(latex_translated_paragraphs)
 
         latex_translated = tex_begin + '\n' + latex_translated + '\n' + tex_end
 
         # Title is probably outside the body part
         self.num = 'title'
-        latex_translated = process_latex.process_specific_command(latex_translated, self.translate_paragraph_latex, 'title')
+        latex_translated = process_latex.process_specific_command(latex_translated, self.translate_text_in_paragraph_latex, 'title')
 
         latex_translated = process_latex.recover_special(latex_translated)
         latex_translated = process_latex.recover_accent(latex_translated)
 
         self.close()
 
         print(self.ntotal - self.nbad, '/',  self.ntotal, 'latex object are correctly translated')
 
         return latex_translated
+
+
+def translate_single_tex_file(input_path, output_path, engine, l_from, l_to, debug):
+    text_translator = TextTranslator(engine, l_to, l_from)
+    latex_translator = LatexTranslator(text_translator, debug)
+
+    input_encoding = get_file_encoding(input_path)
+    text_original = open(input_path, encoding=input_encoding).read()
+    text_final = latex_translator.translate_full_latex(text_original)
+    with open(output_path, "w", encoding='utf-8') as file:
+        print(text_final, file=file)
+    print('Number of translation called:', text_translator.number_of_calls)
+    print('Total characters translated:', text_translator.tot_char)
+    print('saved to', output_path)
```

### Comparing `mathtranslate-2.1.9/mathtranslate/translate_tex.py` & `mathtranslate-2.2.0/mathtranslate/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-#!/usr/bin/env python
-import os
+from . import __version__
+from .config import config
+from .update import get_latest_version
 import sys
+import re
 language_list = '''
 Afrikaans            af
 Irish                ga
 Albanian             sq
 Italian              it
 Arabic               ar
 Japanese             ja
@@ -64,45 +66,39 @@
 Vietnamese           vi
 Icelandic            is
 Welsh                cy
 Indonesian           id
 Yiddish              yi
 '''
 
+split = lambda s: re.split(r'\s+', s)
 
-def main():
-    import mathtranslate
-    from mathtranslate import config
-    from mathtranslate.config import default_engine, default_language_from, default_language_to
-    from mathtranslate.encoding import get_file_encoding
-    from mathtranslate.translate import TextTranslator, LatexTranslator
-    from mathtranslate.update import get_latest_version
+
+def check_update(require_updated=True):
     latest = get_latest_version()
-    updated = mathtranslate.__version__ == latest
+    updated = __version__ == latest
     if updated:
         print("The current mathtranslate is latest")
     else:
-        print("The current mathtranslate is not latest, please update by `pip install --upgrade mathtranslate -i https://pypi.org/simple`")
-        if not config.test_environment:
+        print("The current mathtranslate is not latest, please update by `pip install --upgrade mathtranslate`")
+        if (not config.test_environment) and require_updated:
             sys.exit()
 
-    import argparse
-    parser = argparse.ArgumentParser()
-    parser.add_argument("file", nargs='?', type=str, help='input file')
-    parser.add_argument("-o", type=str, help='output path')
-    parser.add_argument("-engine", default=default_engine, help=f'translation engine, avaiable options include google and tencent. default is {default_engine}')
-    parser.add_argument("-from", default=default_language_from, dest='l_from', help=f'language from, default is {default_language_from}')
-    parser.add_argument("-to", default=default_language_to, dest='l_to', help=f'language to, default is {default_language_to}')
+
+def add_arguments(parser):
+    parser.add_argument("-engine", default=config.default_engine, help=f'translation engine, avaiable options include google and tencent. default is {config.default_engine}')
+    parser.add_argument("-from", default=config.default_language_from, dest='l_from', help=f'language from, default is {config.default_language_from}')
+    parser.add_argument("-to", default=config.default_language_to, dest='l_to', help=f'language to, default is {config.default_language_to}')
     parser.add_argument("--list", action='store_true', help='list codes for languages')
     parser.add_argument("--setkey", action='store_true', help='set id and key of tencent translator')
     parser.add_argument("--setdefault", action='store_true', help='set default translation engine and languages')
     parser.add_argument("--debug", action='store_true')
-    parser.add_argument("--compile", action='store_true')
-    options = parser.parse_args()
 
+
+def process_options(options):
     if options.setkey:
         print('Tencent secretID')
         config.set_variable(config.tencent_secret_id_path, config.tencent_secret_id_default)
         print('Tencent secretKey')
         config.set_variable(config.tencent_secret_key_path, config.tencent_secret_key_default)
         print('saved!')
         config.reread()
@@ -125,56 +121,23 @@
         sys.exit()
 
     if options.list:
         print(language_list)
         print('tencent translator does not support some of them')
         sys.exit()
 
-    if options.file is None:
-        parser.print_help()
-        sys.exit()
-
     if options.engine == 'tencent':
-        haskey = (mathtranslate.config.tencent_secret_id is not None) and (mathtranslate.config.tencent_secret_key is not None)
+        haskey = (config.tencent_secret_id is not None) and (config.tencent_secret_key is not None)
         if not haskey:
             print('Please save ID and key for tencent translation api first by')
             print('translate_tex --setkey')
             sys.exit()
         if options.l_from == 'zh-CN':
             options.l_from = 'zh'
         if options.l_to == 'zh-CN':
             options.l_to = 'zh'
 
     print("Start")
     print('engine', options.engine)
     print('language from', options.l_from)
     print('language to', options.l_to)
-    input_path = options.file
-    if options.o is None:
-        input_path_base, input_path_ext = os.path.splitext(input_path)
-        if input_path_ext == '.tex':
-            print("The input file ends with .tex, it will be overwritten.")
-            print("If you confirm this action, please press enter, otherwise ctrl+C to cancel")
-            input()
-            print('OK I will continue')
-        output_path = input_path_base + '.tex'
-    else:
-        output_path = options.o
-
-    text_translator = TextTranslator(options.engine, options.l_to, options.l_from)
-    latex_translator = LatexTranslator(text_translator, options.debug)
-
-    input_encoding = get_file_encoding(input_path)
-    text_original = open(input_path, encoding=input_encoding).read()
-    text_final = latex_translator.translate_full_latex(text_original)
-    with open(output_path, "w", encoding='utf-8') as file:
-        print(text_final, file=file)
-    print(output_path, 'is generated')
-
-    if options.compile:
-        os.system(f'xelatex {output_path}')
-    else:
-        print(f"You can then compile it locally by running 'xelatex {output_path}' or compile it online on overleaf")
-
-
-if __name__ == '__main__':
-    main()
+    print()
```

### Comparing `mathtranslate-2.1.9/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.2.0/mathtranslate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.1.9
+Version: 2.2.0
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
-Author: Jiace Sun
+Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MathTranslate
@@ -43,32 +43,28 @@
 </p>
 
 <p float="left">
 <img src="https://github.com/SUSYUSTC/MathTranslate/blob/main/example/screenshot.png" width="300">
 <img src="https://github.com/SUSYUSTC/MathTranslate/blob/main/example/translated.png" width="400">
 </p>
 
-Although it is currently a small project, we are aware that this project has received much more attention that we expected. We are planning more developments for better user experience.
-
 ## Releases
 ### Mar 24, 2023
 We add the ability to directly translate arxiv papers.
 ### Mar 21, 2023
 We add tencent translation option for users with IP in China mainland.
 ### Mar 16, 2023
 We are now supporting all operating systems! Now you can install simply by `pip install --upgrade mathtranslate`.
 
 ## Requirements
 1. Python3 and pip. [Anaconda](https://www.anaconda.com) is recommended.
 2. (For users with IP in Mainland China): [Tencent Translation API](https://cloud.tencent.com/product/tmt) account. After registration, you can get the secret ID (not the APP ID!) and secret Key in [Tencent Console](https://console.cloud.tencent.com/cam/capi). Tencent Translate is the translation API with the highest free quota to our knowledge besides Google Translate, with a free quota of 5 million characters per month, and no fee will be deducted if there is no manual recharge (that is, there is no need to worry about misuse).
 
 ## Installation & Update
-`pip install --upgrade mathtranslate -i https://pypi.org/simple`
-
-**We suggest the users to always check update before using because we update frequently**
+`pip install --upgrade mathtranslate`
 
 ## Usage
 1. Prepare or generate a tex file. You can get the tex file by the following two ways:
      - For most [arxiv](https://arxiv.org/) papers, you can download the latex source code (Download - Other formats - Source). If the file you downloaded has no suffix, in most cases it is in .tar format, you may need to add the suffix manually. After decompression you can get a latex project, and then you can translate the .tex files in it.
      - Use [mathpix](https://mathpix.com/) to convert the pdf you want to translate into latex code. mathpix can directly convert pdf page into latex code or convert screenshots into code. We can handle both of these methods. Unfortunately, mathpix charges after a certain amount of usage, here is the [price](https://mathpix.com/pricing).
 2. (Tencent Translate API users) run `translate_tex --setkey` to store the API secretID and secretKey.
 3. Translate the tex file by `translate_tex input.tex -o output.tex`.
```

#### html2text {}

```diff
@@ -1,70 +1,67 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.1.9 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.0 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
-Jiace Sun Author-email: susyustc@gmail.com Classifier: Programming Language ::
-Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE # MathTranslate
+MathTranslate developers Author-email: susyustc@gmail.com Classifier:
+Programming Language :: Python :: 3 Classifier: Operating System :: OS
+Independent Description-Content-Type: text/markdown License-File: LICENSE #
+MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
                                   [logo.jpg]
                             English | ç®ä½ä¸­æ
 This is a project to provide translation of scientific papers with heavy math
 symbols from any language to any language while keeping the math symbols
 unchanged. In most translation softwares you wouldn't be able to keep equations
 and it would annoy you. The main work of this project is to translate LaTex
 files based on Google Translate in plain text, and finally realize the
 translation of pdf. Here's an example of what you get finally.
 [https://user-images.githubusercontent.com/30529122/227698548-1cc19f7c-00e7-
 4312-9d58-2a7237656b51.png]
 [https://github.com/SUSYUSTC/MathTranslate/blob/main/example/screenshot.png]
 [https://github.com/SUSYUSTC/MathTranslate/blob/main/example/translated.png]
-Although it is currently a small project, we are aware that this project has
-received much more attention that we expected. We are planning more
-developments for better user experience. ## Releases ### Mar 24, 2023 We add
-the ability to directly translate arxiv papers. ### Mar 21, 2023 We add tencent
-translation option for users with IP in China mainland. ### Mar 16, 2023 We are
-now supporting all operating systems! Now you can install simply by `pip
-install --upgrade mathtranslate`. ## Requirements 1. Python3 and pip.
-[Anaconda](https://www.anaconda.com) is recommended. 2. (For users with IP in
-Mainland China): [Tencent Translation API](https://cloud.tencent.com/product/
-tmt) account. After registration, you can get the secret ID (not the APP ID!)
-and secret Key in [Tencent Console](https://console.cloud.tencent.com/cam/
-capi). Tencent Translate is the translation API with the highest free quota to
-our knowledge besides Google Translate, with a free quota of 5 million
-characters per month, and no fee will be deducted if there is no manual
-recharge (that is, there is no need to worry about misuse). ## Installation &
-Update `pip install --upgrade mathtranslate -i https://pypi.org/simple` **We
-suggest the users to always check update before using because we update
-frequently** ## Usage 1. Prepare or generate a tex file. You can get the tex
-file by the following two ways: - For most [arxiv](https://arxiv.org/) papers,
-you can download the latex source code (Download - Other formats - Source). If
-the file you downloaded has no suffix, in most cases it is in .tar format, you
-may need to add the suffix manually. After decompression you can get a latex
-project, and then you can translate the .tex files in it. - Use [mathpix]
-(https://mathpix.com/) to convert the pdf you want to translate into latex
-code. mathpix can directly convert pdf page into latex code or convert
-screenshots into code. We can handle both of these methods. Unfortunately,
-mathpix charges after a certain amount of usage, here is the [price](https://
-mathpix.com/pricing). 2. (Tencent Translate API users) run `translate_tex --
-setkey` to store the API secretID and secretKey. 3. Translate the tex file by
-`translate_tex input.tex -o output.tex`. 4. Compile your tex file. You can
-compile it with the [texlive](https://www.tug.org/texlive/) command `xelatex
-output.tex`. For Chinese you need the xeCJK package. If it is a downloaded
-arxiv project, we recommend compressing all files into a zip file and uploading
-it to [overleaf](https://www.overleaf.com/project) for online compilation.
-**Note, you need to set the XeLatex compiler in `Menu - Compiler`, otherwise it
-cannot handle other languages.** 5. You can change the default settings of the
-translation language and engine through the command line arguments `-engine`,
-`-from`, `-to`. For example `translate_tex -engine tencent input.tex -
-o output.tex`. You can also permanently change the setting via `translate_tex -
--setdefault`. You can see more details with `translate_tex --help`. ## Examples
-In the example directory, you can see `main.txt` which is the mathpix output of
-a part of `paper.pdf`. Run `translate_tex main.txt` and you will get the
-`main.tex` and `main.pdf`. `translated.png` is what you should expect to see in
-the `main.pdf`. ## Known Issues 1. If `\begin{env} \end{env}` is reset with
-`\newcommand` in latex, it will not be translated correctly. 2. There is a
-small probability to get something like "XMATHX_1_2" or wrong formula during
-translation. The accuracy rate of Tencent translation is slightly lower than
-that of Google translation. ## Further developments 1. Fix bugs in the latex
-translations. 2. A more user-friendly interface. If you have any questions or
-have interests in making contributions, please contact me by susyustc@gmail.com
-or joining QQ group 288646946.
+## Releases ### Mar 24, 2023 We add the ability to directly translate arxiv
+papers. ### Mar 21, 2023 We add tencent translation option for users with IP in
+China mainland. ### Mar 16, 2023 We are now supporting all operating systems!
+Now you can install simply by `pip install --upgrade mathtranslate`. ##
+Requirements 1. Python3 and pip. [Anaconda](https://www.anaconda.com) is
+recommended. 2. (For users with IP in Mainland China): [Tencent Translation
+API](https://cloud.tencent.com/product/tmt) account. After registration, you
+can get the secret ID (not the APP ID!) and secret Key in [Tencent Console]
+(https://console.cloud.tencent.com/cam/capi). Tencent Translate is the
+translation API with the highest free quota to our knowledge besides Google
+Translate, with a free quota of 5 million characters per month, and no fee will
+be deducted if there is no manual recharge (that is, there is no need to worry
+about misuse). ## Installation & Update `pip install --upgrade mathtranslate`
+## Usage 1. Prepare or generate a tex file. You can get the tex file by the
+following two ways: - For most [arxiv](https://arxiv.org/) papers, you can
+download the latex source code (Download - Other formats - Source). If the file
+you downloaded has no suffix, in most cases it is in .tar format, you may need
+to add the suffix manually. After decompression you can get a latex project,
+and then you can translate the .tex files in it. - Use [mathpix](https://
+mathpix.com/) to convert the pdf you want to translate into latex code. mathpix
+can directly convert pdf page into latex code or convert screenshots into code.
+We can handle both of these methods. Unfortunately, mathpix charges after a
+certain amount of usage, here is the [price](https://mathpix.com/pricing). 2.
+(Tencent Translate API users) run `translate_tex --setkey` to store the API
+secretID and secretKey. 3. Translate the tex file by `translate_tex input.tex -
+o output.tex`. 4. Compile your tex file. You can compile it with the [texlive]
+(https://www.tug.org/texlive/) command `xelatex output.tex`. For Chinese you
+need the xeCJK package. If it is a downloaded arxiv project, we recommend
+compressing all files into a zip file and uploading it to [overleaf](https://
+www.overleaf.com/project) for online compilation. **Note, you need to set the
+XeLatex compiler in `Menu - Compiler`, otherwise it cannot handle other
+languages.** 5. You can change the default settings of the translation language
+and engine through the command line arguments `-engine`, `-from`, `-to`. For
+example `translate_tex -engine tencent input.tex -o output.tex`. You can also
+permanently change the setting via `translate_tex --setdefault`. You can see
+more details with `translate_tex --help`. ## Examples In the example directory,
+you can see `main.txt` which is the mathpix output of a part of `paper.pdf`.
+Run `translate_tex main.txt` and you will get the `main.tex` and `main.pdf`.
+`translated.png` is what you should expect to see in the `main.pdf`. ## Known
+Issues 1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it
+will not be translated correctly. 2. There is a small probability to get
+something like "XMATHX_1_2" or wrong formula during translation. The accuracy
+rate of Tencent translation is slightly lower than that of Google translation.
+## Further developments 1. Fix bugs in the latex translations. 2. A more user-
+friendly interface. If you have any questions or have interests in making
+contributions, please contact me by susyustc@gmail.com or joining QQ group
+288646946.
```

### Comparing `mathtranslate-2.1.9/setup.py` & `mathtranslate-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     description="Translate math-heavy papers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SUSYUSTC/MathTranslate",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=["mtranslate",
-                      "tencentcloud-sdk-python",
                       "chardet",
                       "requests",
                       "regex",
                       "tqdm",
                       ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
             'translate_tex=mathtranslate.translate_tex:main',
+            'translate_arxiv=mathtranslate.translate_arxiv:main',
         ]
     },
 )
```

