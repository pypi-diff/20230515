# Comparing `tmp/publish_to_zhihu-0.1.2.tar.gz` & `tmp/publish_to_zhihu-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "publish_to_zhihu-0.1.2.tar", max compression
+gzip compressed data, was "publish_to_zhihu-0.1.3.tar", max compression
```

## Comparing `publish_to_zhihu-0.1.2.tar` & `publish_to_zhihu-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1090 2023-05-11 23:45:42.640554 publish_to_zhihu-0.1.2/LICENSE
--rw-r--r--   0        0        0       23 2023-05-11 23:45:42.645559 publish_to_zhihu-0.1.2/publish_to_zhihu/__init__.py
--rw-r--r--   0        0        0      338 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.2/publish_to_zhihu/console.py
--rw-r--r--   0        0        0     1177 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.2/publish_to_zhihu/convert_latex.py
--rw-r--r--   0        0        0     3632 2023-05-13 22:08:57.679141 publish_to_zhihu-0.1.2/publish_to_zhihu/prepare_md.py
--rw-r--r--   0        0        0     2725 2023-05-11 23:45:42.647555 publish_to_zhihu-0.1.2/publish_to_zhihu/upload_images.py
--rw-r--r--   0        0        0      932 2023-05-13 22:09:51.798818 publish_to_zhihu-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4329 2023-05-13 22:06:47.223028 publish_to_zhihu-0.1.2/README.md
--rw-r--r--   0        0        0     4953 1970-01-01 00:00:00.000000 publish_to_zhihu-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-11 23:45:42.640554 publish_to_zhihu-0.1.3/LICENSE
+-rw-r--r--   0        0        0       23 2023-05-11 23:45:42.645559 publish_to_zhihu-0.1.3/publish_to_zhihu/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.3/publish_to_zhihu/console.py
+-rw-r--r--   0        0        0     1177 2023-05-11 23:45:42.646554 publish_to_zhihu-0.1.3/publish_to_zhihu/convert_latex.py
+-rw-r--r--   0        0        0     3994 2023-05-15 18:57:50.023921 publish_to_zhihu-0.1.3/publish_to_zhihu/prepare_md.py
+-rw-r--r--   0        0        0     2725 2023-05-11 23:45:42.647555 publish_to_zhihu-0.1.3/publish_to_zhihu/upload_images.py
+-rw-r--r--   0        0        0      932 2023-05-15 18:55:40.316282 publish_to_zhihu-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4711 2023-05-15 18:55:32.470296 publish_to_zhihu-0.1.3/README.md
+-rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 publish_to_zhihu-0.1.3/PKG-INFO
```

### Comparing `publish_to_zhihu-0.1.2/LICENSE` & `publish_to_zhihu-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `publish_to_zhihu-0.1.2/publish_to_zhihu/convert_latex.py` & `publish_to_zhihu-0.1.3/publish_to_zhihu/convert_latex.py`

 * *Files identical despite different names*

### Comparing `publish_to_zhihu-0.1.2/publish_to_zhihu/prepare_md.py` & `publish_to_zhihu-0.1.3/publish_to_zhihu/prepare_md.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,29 +36,29 @@
         markdown_string = markdown_string.replace(
             f"![[{image_link}]]", "\n" + f"![[{image_link}]]"
         )
 
     return markdown_string
 
 
-def process_image_link(container, conn_str, image_folder, re_match):
+def process_image_link(container, conn_str, image_folder, re_match, is_mdnice):
     image_link = re_match.group(1)
     if not image_link.startswith("http://") and not image_link.startswith("https://"):
         uploaded_urls = upload_images(
             container,
             conn_str,
             image_folder,
             [image_link],
             overwrite=True,
         )
         image_link = uploaded_urls[0]
-    return f"![]({image_link})"
-
-    # not needed for mdnice
-    # return f'<img src="{image_link}" class="origin_image zh-lightbox-thumb lazy">\n'
+    if is_mdnice:
+        return f"![]({image_link})"
+    else:
+        return f'<img src="{image_link}" class="origin_image zh-lightbox-thumb lazy">\n'
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="""
     Convert standard Markdown file to mdnice Format
     1. Upload all the images
@@ -68,14 +68,19 @@
     )
 
     parser.add_argument(
         "--container",
         help="The Container which the file will be uploaded to.",
         default="imagehost",
     )
+    parser.add_argument(
+        "--mdnice",
+        action="store_true",
+        help="Convert to mdnice format, default is zhihu format",
+    )
     parser.add_argument("image_link_root", help="The root folder of image links.")
     parser.add_argument("output_folder", help="The folder to store converted md files")
     parser.add_argument(
         "files", nargs="+", help="The file to be uploaded. Must Include at least one."
     )
 
     args = parser.parse_args()
@@ -91,17 +96,21 @@
         output_file_path = os.path.join(output_folder, os.path.split(file_path)[1])
         with open(file_path, encoding="utf-8") as in_f, open(
             output_file_path, "w", encoding="utf-8"
         ) as out_f:
             content = in_f.read()
             new_content = ensure_image_link_newline(content)
             new_content = OBSIDIAN_IMAGE_LINK_RE.sub(
-                lambda m: process_image_link(container, conn_str, image_link_root, m),
+                lambda m: process_image_link(
+                    container, conn_str, image_link_root, m, args.mdnice
+                ),
                 new_content,
             )
-            # not needed for mdnice
-            # new_content = append_newline_to_list_items(new_content)
+            if not args.mdnice:
+                # if append newline before list items for mdnice,
+                # there will be extra newline between items after rendering
+                new_content = append_newline_to_list_items(new_content)
             out_f.write(new_content)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `publish_to_zhihu-0.1.2/publish_to_zhihu/upload_images.py` & `publish_to_zhihu-0.1.3/publish_to_zhihu/upload_images.py`

 * *Files identical despite different names*

### Comparing `publish_to_zhihu-0.1.2/pyproject.toml` & `publish_to_zhihu-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "publish_to_zhihu"
-version = "0.1.2"
+version = "0.1.3"
 description = "Publish markdown to Zhihu"
 authors = ["Anselm Wang <anselmwang@gmail.com>"]
 homepage = "https://github.com/anselmwang/publish_to_zhihu"
 repository = "https://github.com/anselmwang/publish_to_zhihu"
 readme= "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `publish_to_zhihu-0.1.2/README.md` & `publish_to_zhihu-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,25 @@
+# Inconvenience
+
+今天这个项目依赖mdnice来转化公式，但是从mdnice复制到知乎编辑器时，所有H1、H2、H3标题通通会被变成H1。mdnice没有做错，应该是知乎编辑器的问题。
+
+所以，对于没有公式的文章，请不加"--mdnice" flag，直接上传生成的md到知乎。
+
+对于有公式的文章，用上"--mdnice" flag。
+
+
+
 # 功能
 这个工具帮助将Obsidian风格的Markdown文件转化为mdnice的格式，主要有以下功能
 - 自动上传本地图片到Azure blob storage
 - 保证每个image link都在每行的最开始，没有额外的空格
-
-
-想要转化为知乎格式，其实还需要下面几个工作，不过我们依赖mdnice来做下面的转换。
 - 自动为每个list item前面增加额外的回车，不然知乎不识别
 - 转换Obsidian的图片链接`![[attachments/Pasted image 20230511181810.png]]`到知乎格式
+
+想要转化为知乎格式，其实还需要下面几个工作，不过我们依赖mdnice来做下面的转换。
 - 自动转换latex公式
 # 安装
 首先自行创造Azure storage account和blob container
 
 设置环境变量IMAGEHOST_CONN_STR，这个变量要求包含形如`AccountName=(.*?);.*EndpointSuffix=(.*?)($|;)")`的信息
 
 安装工具
```

### Comparing `publish_to_zhihu-0.1.2/PKG-INFO` & `publish_to_zhihu-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: publish-to-zhihu
-Version: 0.1.2
+Version: 0.1.3
 Summary: Publish markdown to Zhihu
 Home-page: https://github.com/anselmwang/publish_to_zhihu
 Author: Anselm Wang
 Author-email: anselmwang@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -13,23 +13,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-storage-blob (>=12.12.0,<13.0.0)
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Project-URL: Repository, https://github.com/anselmwang/publish_to_zhihu
 Description-Content-Type: text/markdown
 
+# Inconvenience
+
+今天这个项目依赖mdnice来转化公式，但是从mdnice复制到知乎编辑器时，所有H1、H2、H3标题通通会被变成H1。mdnice没有做错，应该是知乎编辑器的问题。
+
+所以，对于没有公式的文章，请不加"--mdnice" flag，直接上传生成的md到知乎。
+
+对于有公式的文章，用上"--mdnice" flag。
+
+
+
 # 功能
 这个工具帮助将Obsidian风格的Markdown文件转化为mdnice的格式，主要有以下功能
 - 自动上传本地图片到Azure blob storage
 - 保证每个image link都在每行的最开始，没有额外的空格
-
-
-想要转化为知乎格式，其实还需要下面几个工作，不过我们依赖mdnice来做下面的转换。
 - 自动为每个list item前面增加额外的回车，不然知乎不识别
 - 转换Obsidian的图片链接`![[attachments/Pasted image 20230511181810.png]]`到知乎格式
+
+想要转化为知乎格式，其实还需要下面几个工作，不过我们依赖mdnice来做下面的转换。
 - 自动转换latex公式
 # 安装
 首先自行创造Azure storage account和blob container
 
 设置环境变量IMAGEHOST_CONN_STR，这个变量要求包含形如`AccountName=(.*?);.*EndpointSuffix=(.*?)($|;)")`的信息
 
 安装工具
```

