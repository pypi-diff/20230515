# Comparing `tmp/publish_to_zhihu-0.1.3.tar.gz` & `tmp/publish_to_zhihu-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "publish_to_zhihu-0.1.3.tar", max compression
+gzip compressed data, was "publish_to_zhihu-0.1.4.tar", max compression
```

## Comparing `publish_to_zhihu-0.1.3.tar` & `publish_to_zhihu-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1090 2023-05-11 23:45:42.640554 publish_to_zhihu-0.1.3/LICENSE
--rw-r--r--   0        0        0       23 2023-05-11 23:45:42.645559 publish_to_zhihu-0.1.3/publish_to_zhihu/__init__.py
--rw-r--r--   0        0        0      338 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.3/publish_to_zhihu/console.py
--rw-r--r--   0        0        0     1177 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.3/publish_to_zhihu/convert_latex.py
--rw-r--r--   0        0        0     3994 2023-05-15 18:57:50.023921 publish_to_zhihu-0.1.3/publish_to_zhihu/prepare_md.py
--rw-r--r--   0        0        0     2725 2023-05-11 23:45:42.647555 publish_to_zhihu-0.1.3/publish_to_zhihu/upload_images.py
--rw-r--r--   0        0        0      932 2023-05-15 18:55:40.316282 publish_to_zhihu-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4711 2023-05-15 18:55:32.470296 publish_to_zhihu-0.1.3/README.md
--rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 publish_to_zhihu-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-11 23:45:42.640554 publish_to_zhihu-0.1.4/LICENSE
+-rw-r--r--   0        0        0       23 2023-05-11 23:45:42.645559 publish_to_zhihu-0.1.4/publish_to_zhihu/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.4/publish_to_zhihu/console.py
+-rw-r--r--   0        0        0     1177 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.4/publish_to_zhihu/convert_latex.py
+-rw-r--r--   0        0        0     4319 2023-05-15 19:10:13.211364 publish_to_zhihu-0.1.4/publish_to_zhihu/prepare_md.py
+-rw-r--r--   0        0        0     2725 2023-05-11 23:45:42.647555 publish_to_zhihu-0.1.4/publish_to_zhihu/upload_images.py
+-rw-r--r--   0        0        0      932 2023-05-15 19:10:17.698186 publish_to_zhihu-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4742 2023-05-15 19:09:43.644840 publish_to_zhihu-0.1.4/README.md
+-rw-r--r--   0        0        0     5356 1970-01-01 00:00:00.000000 publish_to_zhihu-0.1.4/PKG-INFO
```

### Comparing `publish_to_zhihu-0.1.3/LICENSE` & `publish_to_zhihu-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `publish_to_zhihu-0.1.3/publish_to_zhihu/convert_latex.py` & `publish_to_zhihu-0.1.4/publish_to_zhihu/convert_latex.py`

 * *Files identical despite different names*

### Comparing `publish_to_zhihu-0.1.3/publish_to_zhihu/prepare_md.py` & `publish_to_zhihu-0.1.4/publish_to_zhihu/prepare_md.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 import re
 
 from .upload_images import upload_images
 
 OBSIDIAN_IMAGE_LINK_RE = re.compile(r"!\[\[([^\]]*)\]\]")
 
 
+def has_higher_level_directory(md_content):
+    pattern = r"^#{3,}"
+    matches = re.findall(pattern, md_content, re.MULTILINE)
+    return len(matches) > 0
+
+
 def append_newline_to_list_items(markdown_string):
     # Regular expression pattern to match unordered and ordered list items
     pattern = r"(^[-*+]\s|\d+\.\s)"
 
     # Split the markdown string into lines
     lines = markdown_string.split("\n")
 
@@ -94,14 +100,17 @@
 
     for file_path in files:
         output_file_path = os.path.join(output_folder, os.path.split(file_path)[1])
         with open(file_path, encoding="utf-8") as in_f, open(
             output_file_path, "w", encoding="utf-8"
         ) as out_f:
             content = in_f.read()
+            if has_higher_level_directory(content):
+                print(f"Skip {file_path} because it has higher level directory")
+                continue
             new_content = ensure_image_link_newline(content)
             new_content = OBSIDIAN_IMAGE_LINK_RE.sub(
                 lambda m: process_image_link(
                     container, conn_str, image_link_root, m, args.mdnice
                 ),
                 new_content,
             )
```

### Comparing `publish_to_zhihu-0.1.3/publish_to_zhihu/upload_images.py` & `publish_to_zhihu-0.1.4/publish_to_zhihu/upload_images.py`

 * *Files identical despite different names*

### Comparing `publish_to_zhihu-0.1.3/pyproject.toml` & `publish_to_zhihu-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "publish_to_zhihu"
-version = "0.1.3"
+version = "0.1.4"
 description = "Publish markdown to Zhihu"
 authors = ["Anselm Wang <anselmwang@gmail.com>"]
 homepage = "https://github.com/anselmwang/publish_to_zhihu"
 repository = "https://github.com/anselmwang/publish_to_zhihu"
 readme= "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `publish_to_zhihu-0.1.3/README.md` & `publish_to_zhihu-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Inconvenience
 
+## 选择mdnice或zhihu格式
 今天这个项目依赖mdnice来转化公式，但是从mdnice复制到知乎编辑器时，所有H1、H2、H3标题通通会被变成H1。mdnice没有做错，应该是知乎编辑器的问题。
 
 所以，对于没有公式的文章，请不加"--mdnice" flag，直接上传生成的md到知乎。
 
 对于有公式的文章，用上"--mdnice" flag。
```

### Comparing `publish_to_zhihu-0.1.3/PKG-INFO` & `publish_to_zhihu-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: publish-to-zhihu
-Version: 0.1.3
+Version: 0.1.4
 Summary: Publish markdown to Zhihu
 Home-page: https://github.com/anselmwang/publish_to_zhihu
 Author: Anselm Wang
 Author-email: anselmwang@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -15,14 +15,15 @@
 Requires-Dist: azure-storage-blob (>=12.12.0,<13.0.0)
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Project-URL: Repository, https://github.com/anselmwang/publish_to_zhihu
 Description-Content-Type: text/markdown
 
 # Inconvenience
 
+## 选择mdnice或zhihu格式
 今天这个项目依赖mdnice来转化公式，但是从mdnice复制到知乎编辑器时，所有H1、H2、H3标题通通会被变成H1。mdnice没有做错，应该是知乎编辑器的问题。
 
 所以，对于没有公式的文章，请不加"--mdnice" flag，直接上传生成的md到知乎。
 
 对于有公式的文章，用上"--mdnice" flag。
```

