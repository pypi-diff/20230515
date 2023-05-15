# Comparing `tmp/edman-2023.5.15.1.tar.gz` & `tmp/edman-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman-2023.5.15.1.tar", last modified: Mon May 15 07:05:12 2023, max compression
+gzip compressed data, was "edman-2023.5.8.tar", last modified: Mon May  8 02:04:22 2023, max compression
```

## Comparing `edman-2023.5.15.1.tar` & `edman-2023.5.8.tar`

### file list

```diff
@@ -1,60 +1,30 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.468086 edman-2023.5.15.1/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.458086 edman-2023.5.15.1/.github/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.458086 edman-2023.5.15.1/.github/workflows/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1379 2023-05-10 06:43:20.000000 edman-2023.5.15.1/.github/workflows/unittest.yml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2022-07-27 01:25:38.000000 edman-2023.5.15.1/.gitignore
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.458086 edman-2023.5.15.1/.idea/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      238 2022-04-13 07:00:02.000000 edman-2023.5.15.1/.idea/.gitignore
--rw-r--r--   0 ohno      (1000) ohno      (1000)      557 2023-04-10 07:58:11.000000 edman-2023.5.15.1/.idea/edman.iml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.458086 edman-2023.5.15.1/.idea/inspectionProfiles/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      179 2022-04-13 07:00:02.000000 edman-2023.5.15.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      254 2023-04-10 07:58:11.000000 edman-2023.5.15.1/.idea/misc.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      269 2022-04-13 07:00:02.000000 edman-2023.5.15.1/.idea/modules.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      185 2022-04-13 07:00:02.000000 edman-2023.5.15.1/.idea/vcs.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.5.15.1/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7615 2023-05-15 07:05:12.468086 edman-2023.5.15.1/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.5.15.1/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.458086 edman-2023.5.15.1/edman/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2023-05-09 07:38:50.000000 edman-2023.5.15.1/edman/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1373 2023-03-15 05:16:00.000000 edman-2023.5.15.1/edman/config.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16457 2023-05-15 01:46:07.000000 edman-2023.5.15.1/edman/convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    47547 2023-05-15 05:19:21.000000 edman-2023.5.15.1/edman/db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.5.15.1/edman/exceptions.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    23473 2023-05-15 07:03:35.000000 edman-2023.5.15.1/edman/file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1520 2023-03-09 05:51:32.000000 edman-2023.5.15.1/edman/json_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     9907 2023-04-10 07:58:11.000000 edman-2023.5.15.1/edman/search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10958 2023-03-09 05:51:32.000000 edman-2023.5.15.1/edman/utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.468086 edman-2023.5.15.1/edman.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7615 2023-05-15 07:05:12.000000 edman-2023.5.15.1/edman.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      971 2023-05-15 07:05:12.000000 edman-2023.5.15.1/edman.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-15 07:05:12.000000 edman-2023.5.15.1/edman.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-05-15 07:05:12.000000 edman-2023.5.15.1/edman.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2023-05-15 07:05:12.000000 edman-2023.5.15.1/edman.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1071 2023-05-15 07:03:35.000000 edman-2023.5.15.1/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      859 2023-05-10 06:13:28.000000 edman-2023.5.15.1/requirements.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-15 07:05:12.468086 edman-2023.5.15.1/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.468086 edman-2023.5.15.1/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2022-04-13 07:00:02.000000 edman-2023.5.15.1/tests/__init__.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.468086 edman-2023.5.15.1/tests/ini/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      166 2022-11-15 02:42:20.000000 edman-2023.5.15.1/tests/ini/test_db.ini.sample
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.5.15.1/tests/test_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    86854 2023-04-20 03:03:49.000000 edman-2023.5.15.1/tests/test_db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    42557 2023-05-15 07:03:35.000000 edman-2023.5.15.1/tests/test_file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.5.15.1/tests/test_multiuser.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.5.15.1/tests/test_search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.5.15.1/tests/test_utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.458086 edman-2023.5.15.1/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-15 07:05:12.468086 edman-2023.5.15.1/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2023-04-07 00:37:51.000000 edman-2023.5.15.1/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      632 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      754 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1089 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      831 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      654 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      820 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     2176 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      639 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      675 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      911 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      640 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      708 2023-05-10 00:30:10.000000 edman-2023.5.15.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.5.8/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2022-04-13 07:00:02.000000 edman-2023.5.8/MANIFEST.in
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:22.028113 edman-2023.5.8/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.5.8/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1373 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/config.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16457 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    47757 2023-04-05 05:00:36.000000 edman-2023.5.8/edman/db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/exceptions.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    21800 2023-05-08 02:02:11.000000 edman-2023.5.8/edman/file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1520 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/json_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     9907 2023-04-10 07:58:11.000000 edman-2023.5.8/edman/search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10958 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      470 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        6 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      707 2023-05-08 02:04:22.028113 edman-2023.5.8/setup.cfg
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2022-04-13 07:00:02.000000 edman-2023.5.8/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    86854 2023-04-20 03:03:49.000000 edman-2023.5.8/tests/test_db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    36850 2023-05-08 02:02:11.000000 edman-2023.5.8/tests/test_file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.5.8/tests/test_multiuser.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.5.8/tests/test_search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_utils.py
```

### Comparing `edman-2023.5.15.1/LICENSE.txt` & `edman-2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/PKG-INFO` & `edman-2023.5.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.5.15.1
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Author-email: Masaki Ohno <masakio@post.kek.jp>
+Home-page: https://github.com/ryde/edman
+Author: Masaki Ohno
+Author-email: masakio@post.kek.jp
 License: MIT License
-        
-        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: documentation, https://ryde.github.io/edman/
-Project-URL: repository, https://github.com/ryde/edman
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman
 =====
```

### Comparing `edman-2023.5.15.1/README.rst` & `edman-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/edman/config.py` & `edman-2023.5.8/edman/config.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/edman/convert.py` & `edman-2023.5.8/edman/convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/edman/db.py` & `edman-2023.5.8/edman/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,16 @@
                         f'インサートに失敗しました:{e.details}\nインサート結果:{results}')
                 results.append({collection: result.inserted_ids})
 
         return results
 
     def find_collection_from_objectid(self,
                                       oid: Union[str,
-                                      ObjectId]) -> Union[str, None]:
+                                      ObjectId]) -> Union[str,
+    None]:
         """
         | DB内のコレクションから指定のObjectIDを探し、所属しているコレクションを返す
         | DBに負荷がかかるので使用は注意が必要
 
         :param oid:
         :type oid: ObjectId or str
         :return: collection
@@ -340,15 +341,17 @@
         :type oid: ObjectId or str
         :param query:
         :type query: list or None
         :param bool reference_delete: default True
         :return: result
         :rtype: dict
         """
-        doc = self.db[collection].find_one({'_id': Utils.conv_objectid(oid)})
+
+        oid = Utils.conv_objectid(oid)
+        doc = self.db[collection].find_one({'_id': oid})
 
         if doc is None:
             result = None
         else:
             # embの場合は指定階層のドキュメントを引き抜く
             # refの場合はdocの結果をそのまま入れる
             try:
@@ -646,26 +649,27 @@
 
         :param DBRef ref:
         :param ObjectId del_oid:
         :return:
         """
         parent_doc = self.db[ref.collection].find_one({'_id': ref.id})
         children = parent_doc[self.child]
+
         target = None
         for child in children:
             if child.id == del_oid:
                 target = child
                 break
         if target is None:
             raise ValueError(
                 f'親となる{parent_doc["id"]}に{str(del_oid)}が登録されていません')
         else:
             children.remove(target)
 
-            # 子要素が登録されていればself.childを更新
+            # 他に子要素が登録されていればself.childを更新
             if len(children) > 0:
                 result = self.db[ref.collection].update_one(
                     {'_id': ref.id},
                     {'$set': {self.child: children}})
             # 他に子要素がなければself.child自体を削除
             else:
                 del parent_doc[self.child]
@@ -680,50 +684,57 @@
         コレクション別の、oidとファイルリファレンスリストを取り出す
 
         :param dict doc:
         :param str collection:
         :return:
         :rtype: dict
         """
-        return {collection: {
-            doc['_id']: {self.file_ref: doc.get(self.file_ref, {})}}}
+        file_ref_buff = {}
+        if doc.get(self.file_ref) is not None:
+            file_ref_buff = {self.file_ref: doc[self.file_ref]}
+
+        return {collection: {doc['_id']: file_ref_buff}}
 
     def _recursive_extract_elements_from_doc(self, doc: dict,
                                              collection: str) -> dict:
         """
         再帰処理で
         コレクション別の、oidとファイルリファレンスの辞書を取り出すジェネレータ
 
         :param dict doc:
         :param str collection:
         :return:
         :rtype: dict
         """
         yield self._extract_elements_from_doc(doc, collection)
+
         if doc.get(self.child):
             for child_ref in doc[self.child]:
                 yield from self._recursive_extract_elements_from_doc(
                     self.db.dereference(child_ref), child_ref.collection)
 
     def _collect_emb_file_ref(self, doc: dict, request_key: str) -> list:
         """
         emb構造のデータからファイルリファレンスのリストだけを取り出すジェネレータ
 
         :param dict doc:
         :param str request_key:
         :return: value
         :rtype: list
         """
+
         for key, value in doc.items():
             if isinstance(value, dict):
                 yield from self._collect_emb_file_ref(value, request_key)
+
             elif isinstance(value, list) and Utils.item_literal_check(value):
                 if key == request_key:
                     yield value
                 continue
+
             elif isinstance(value, list):
                 if key == request_key:
                     yield value
                 else:
                     for i in value:
                         yield from self._collect_emb_file_ref(i, request_key)
             else:
@@ -746,25 +757,25 @@
 
     def get_structure(self, collection: str, oid: ObjectId) -> str:
         """
         対象のドキュメントの構造を取得する
 
         :param str collection:
         :param ObjectId oid:
-        :return: result
+        :return: ref or emb
         :rtype: str
         """
         doc = self.db[collection].find_one({'_id': Utils.conv_objectid(oid)})
         if doc is None:
             raise EdmanInternalError('該当するドキュメントは存在しません')
+
         if any(key in doc for key in (self.parent, self.child)):
-            result = 'ref'
+            return 'ref'
         else:
-            result = 'emb'
-        return result
+            return 'emb'
 
     def structure(self, collection: str, oid: ObjectId,
                   structure_mode: str, new_collection: str) -> list:
         """
         構造をrefからembへ、またはembからrefへ変更する
 
         :param str collection:
@@ -772,22 +783,22 @@
         :param str structure_mode:
         :param str new_collection:
         :return: structured_result
         :rtype: list
         """
         oid = Utils.conv_objectid(oid)
 
-        convert = Convert()
         # refデータをembに変換する
         if structure_mode == 'emb':
             # 自分データ取り出し
             ref_result = self.doc(collection, oid, query=None,
                                   reference_delete=False)
             if ref_result is None:
                 raise EdmanInternalError("ドキュメントが存在しません")
+
             reference_point_result = self.get_reference_point(
                 ref_result)
             if reference_point_result[self.child]:
                 # 子データを取り出し
                 children = self.get_child_all({collection: ref_result})
 
                 # 自分のリファレンスデータとidを削除
@@ -798,31 +809,34 @@
                 # 子のリファレンスデータ削除
                 non_ref_children = self.delete_reference(children,
                                                          ('_id', self.parent,
                                                           self.child))
                 # 自分と子要素をマージする
                 ref_result.update(non_ref_children)
 
+                convert = Convert()
                 converted_edman = convert.dict_to_edman(
                     {new_collection: ref_result}, mode='emb')
                 structured_result = self.insert(converted_edman)
             # 子が存在しないドキュメントの場合(新たなコレクションとして切り出す)
             else:
                 # 自分のリファレンスデータとidを削除
                 for del_key in (self.parent, '_id'):
                     if del_key in ref_result:
                         del ref_result[del_key]
+                convert = Convert()
                 converted_edman = convert.dict_to_edman(
                     {new_collection: ref_result}, mode='emb')
                 structured_result = self.insert(converted_edman)
 
         # embからrefに変換
         elif structure_mode == 'ref':
             emb_result = self.db[collection].find_one({'_id': oid})
             del emb_result['_id']
+            convert = Convert()
             converted_edman = convert.dict_to_edman(
                 {new_collection: emb_result}, mode='ref')
             structured_result = self.insert(converted_edman)
             structured_result.reverse()
 
         else:
             raise EdmanFormatError('structureはrefまたはembの指定が必要です')
@@ -890,21 +904,22 @@
         |
         | 同じコレクションの場合は子データをリストで囲む
 
         :param dict doc:
         :return: children
         :rtype: list
         """
+        doc = list(doc.values())[0]
         children = []
         # 単純にリスト内に辞書データを入れたい場合
-        doc = list(doc.values())[0]
         if self.child in doc:
             children = [
                 {child_ref.collection: self.db.dereference(child_ref)}
                 for child_ref in doc[self.child]]
+
         return children
 
     def _build_to_doc_child(self, find_result: list) -> dict:
         """
         子の検索結果（リスト）を入れ子辞書に組み立てる
 
         :param list find_result:
@@ -1022,21 +1037,22 @@
         if self.db[collection].estimated_document_count() == 0:
             raise EdmanInternalError('該当するドキュメントは存在しません')
 
         id_list = [doc['_id'] for doc in self.db[collection].find() if
                    self.get_structure(collection, doc['_id']) == 'emb']
 
         result_list = []
-        convert = Convert()
         for oid in id_list:
             emb_result = self.db[collection].find_one({'_id': oid})
             del emb_result['_id']
+            convert = Convert()
             pull_result = convert.pullout_key(emb_result, key)
             if not pull_result:
                 raise EdmanInternalError(f'{key}は存在しません')
+
             if exclusion:
                 result = convert.exclusion_key(pull_result, exclusion)
                 if pull_result == result:
                     raise EdmanInternalError(f'{list(exclusion)}は存在しません')
             else:
                 result = pull_result
 
@@ -1059,14 +1075,15 @@
                        self.db.list_collection_names(filter=coll_filter)]
         if gf_filter:
             result = list(
                 set(collections) - {Config.fs_files, Config.fs_chunks})
         else:
             result = collections
         result.sort()
+
         return result
 
     @staticmethod
     def pack_list(types: list, target: list) -> list:
         """
         typesが少ない時に、最後の値で足りない分を埋める
         例
```

### Comparing `edman-2023.5.15.1/edman/exceptions.py` & `edman-2023.5.8/edman/exceptions.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/edman/file.py` & `edman-2023.5.8/edman/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import shutil
 import copy
+import gzip
 from tempfile import TemporaryDirectory, NamedTemporaryFile
 import datetime
 import zipfile
 from typing import Union, Tuple, Iterator, List, Any
 from pathlib import Path
 import gridfs
 from gridfs.errors import NoFile, GridFSError
@@ -57,40 +58,46 @@
         :param str structure:
         :param query:
         :type query: list or None
         :return:
         :rtype: bool
         """
         oid = Utils.conv_objectid(oid)
-        if structure not in ['ref', 'emb']:
-            raise EdmanFormatError('structureはrefまたはembの指定が必要です')
 
         # ドキュメント存在確認&コレクション存在確認&対象ドキュメント取得
-        if (doc := self.db[collection].find_one({'_id': oid})) is None:
+        doc = self.db[collection].find_one({'_id': oid})
+        if doc is None:
             raise EdmanInternalError('対象のコレクション、またはドキュメントが存在しません')
 
         # ファイルリスト取得
         files_list = self.get_file_ref(doc, structure, query)
-        if len(files_list) == 0:
-            raise EdmanDbProcessError('ファイルが存在しません')
 
         # リファレンスデータを編集
-        # 何らかの原因で重複があった場合を避けるため一度setにする
-        files_list = list(set(files_list))
-        files_list.remove(delete_oid)
+        if len(files_list) > 0:
+            # 何らかの原因で重複があった場合を避けるため一度setにする
+            files_list = list(set(files_list))
+            files_list.remove(delete_oid)
+        else:
+            raise EdmanDbProcessError('ファイルが存在しません')
 
         # ドキュメントを新しいファイルリファレンスに置き換える
-        try:
-            if structure == 'ref':
+        if structure == 'ref':
+            try:
                 new_doc = self.file_list_replace(doc, files_list)
-            else:
+            except Exception:
+                raise
+        elif structure == 'emb':
+            try:
                 new_doc = Utils.doc_traverse(doc, files_list, query,
                                              self.file_list_replace)
-        except Exception:
-            raise
+            except Exception:
+                raise
+        else:
+            raise EdmanFormatError('structureはrefまたはembの指定が必要です')
+
         replace_result = self.db[collection].replace_one({'_id': oid}, new_doc)
         # fsから該当ファイルを削除
         if replace_result.modified_count:
             self.fs_delete([delete_oid])
 
         # ファイルが削除されればOK
         return False if self.fs.exists(delete_oid) else True
@@ -169,28 +176,30 @@
                 result.update({file_oid: fs_out.filename})
         return result
 
     def download(self, file_oid: list[ObjectId],
                  path: Union[str, Path]) -> bool:
         """
         Gridfsからデータをダウンロードし、ファイルに保存
+        metadataに圧縮指定があれば伸長する
 
         :param list file_oid:
         :param path:
         :type path: str or Path
         :return: result
         :rtype: bool
         """
         # 定型的な前処理があればここに追加する
         return self._grid_out(file_oid, path)
 
     def _grid_out(self, file_oid_list: List[ObjectId],
                   path: Union[str, Path]) -> bool:
         """
         Gridfsからデータを取得し、ファイルに保存
+        metadataに圧縮指定があれば伸長する
         複数のファイルを指定すると、複数のファイルが作成される
 
         :param list file_oid_list:
         :param path:
         :type path: str or Path
         :return: result
         :rtype: bool
@@ -201,96 +210,105 @@
 
         # パスが正しいか検証
         if not p.exists():
             raise FileNotFoundError
         # ファイルが存在するか検証
         if False in map(self.fs.exists, file_oid_list):
             raise EdmanDbProcessError('指定のファイルはDBに存在しません')
-
-        # ダウンロード処理
-        results = []
-        for file_oid in file_oid_list:
-            fs_out = self.fs.get(file_oid)
-            save_path = p / fs_out.filename
-            try:
-                with save_path.open('wb') as f:
-                    tmp = fs_out.read()
-                    f.write(tmp)
-                    f.flush()
-                    os.fsync(f.fileno())
-            except IOError:
-                raise
-            results.append(save_path.exists())
-
+        else:
+            # ダウンロード処理
+            results = []
+            for file_oid in file_oid_list:
+                fs_out = self.fs.get(file_oid)
+                save_path = p / fs_out.filename
+                try:
+                    with save_path.open('wb') as f:
+                        tmp = fs_out.read()
+                        if hasattr(fs_out,
+                                   'compress') and fs_out.compress == 'gzip':
+                            tmp = gzip.decompress(tmp)
+                        f.write(tmp)
+                        f.flush()
+                        os.fsync(f.fileno())
+                except IOError:
+                    raise
+                results.append(save_path.exists())
         return all(results)
 
     def upload(self, collection: str, oid: Union[ObjectId, str],
                file_path: Tuple[Tuple[Any, bool]], structure: str,
                query=None) -> bool:
         """
         ドキュメントにファイルリファレンスを追加する
-        ファイルのインサート処理なども行う
+        ファイルのインサート処理、圧縮処理なども行う
         :param str collection:
         :param oid:
         :type oid: ObjectId or str
-        :param tuple file_path:ドキュメントに添付する単数or複数のファイルパス
+        :param tuple file_path:ドキュメントに添付する単数or複数のファイルパスと圧縮可否のタプル
         :param str structure:
         :param query:
         :type query: list or None
         :return:
         :rtype: bool
         """
+
         oid = Utils.conv_objectid(oid)
-        if structure not in ['ref', 'emb']:
-            raise EdmanFormatError('構造はrefかembが必要です')
 
         # ドキュメント存在確認&対象ドキュメント取得
         doc = self.db[collection].find_one({'_id': oid})
         if doc is None:
             raise EdmanInternalError('対象のドキュメントが存在しません')
         if structure == 'emb':
             # クエリーがドキュメントのキーとして存在するかチェック
             if not Utils.query_check(query, doc):
                 raise EdmanFormatError('対象のドキュメントに対してクエリーが一致しません.')
 
         # ファイルのインサート
         inserted_file_oids = self.grid_in(file_path)
         if structure == 'ref':
             new_doc = self.file_list_attachment(doc, inserted_file_oids)
-        else:
+        elif structure == 'emb':
             try:
                 new_doc = Utils.doc_traverse(doc, inserted_file_oids, query,
                                              self.file_list_attachment)
             except Exception:
                 raise
+        else:
+            raise EdmanFormatError('構造はrefかembが必要です')
 
         # ドキュメント差し替え
         replace_result = self.db[collection].replace_one({'_id': oid}, new_doc)
+
         if replace_result.modified_count == 1:
-            result = True
+            return True
         else:  # 差し替えができなかった時は添付ファイルは削除
             self.fs_delete(inserted_file_oids)
-            result = False
-
-        return result
+            return False
 
     def grid_in(self, files: Tuple[Tuple[Any, bool]]) -> list[Any]:
         """
-        Gridfsへ複数のデータをアップロード
+        Gridfsへ複数のデータをアップロードし
+        compressに圧縮指定があればgzipで圧縮する
 
         :param tuple files:
         :return: inserted
         :rtype: list
         """
         inserted = []
         for file, compress in files:
             try:
                 with file.open('rb') as f:
                     fb = f.read()
-                    metadata = {'filename': os.path.basename(f.name)}
+                    if compress:
+                        fb = gzip.compress(fb, compresslevel=self.comp_level)
+                        compress = 'gzip'
+                    else:
+                        compress = None
+                    metadata = {'filename': os.path.basename(f.name),
+                                'compress': compress}
             except (IOError, OSError) as e:
                 raise EdmanDbProcessError(e)
             try:
                 inserted.append(self.fs.put(fb, **metadata))
             except GridFSError as e:
                 raise EdmanDbProcessError(e)
         return inserted
@@ -397,15 +415,20 @@
                     try:
                         content = self.fs.get(file_ref)
                     except NoFile:
                         raise EdmanDbProcessError('指定の関連ファイルが存在しません')
                     except GridFSError:
                         raise
                     else:
-                        filepath = os.path.join(dir_path, content.name)
+                        # 圧縮設定の場合はその拡張子を追加
+                        if content.compress is not None:
+                            filename = content.name + '.' + content.compress
+                        else:
+                            filename = content.name
+                        filepath = os.path.join(dir_path, filename)
                     try:
                         with open(filepath, 'wb') as f:
                             f.write(content.read())
                     except (FileNotFoundError, IOError):
                         EdmanInternalError('ファイルを保存することが出来ませんでした')
                     except GridFSError:
                         raise
@@ -422,58 +445,21 @@
                 with NamedTemporaryFile() as fp:
                     zip_filepath = shutil.make_archive(fp.name, zip_suffix[1:],
                                                        tmpdir)
             except Exception:
                 raise
         return zip_filepath
 
-    # def zipped_contents_path(self, downloads: dict, json_tree_file_name: str,
-    #                     encoded_json: bytes, p: Path) -> str:
-    #     """
-    #     jsonと添付ファイルを含むzipファイルを生成
-    #     zipファイル内部にjson_tree_file_name.jsonのjsonファイルを含む
-    #     添付ファイルがなく、jsonファイルだけ取得したい場合はzipped_jsonを利用
-    #
-    #     :param dict downloads:
-    #     :param str json_tree_file_name:
-    #     :param bytes encoded_json:
-    #     :param Path p:
-    #     :rtype: str
-    #     :return:
-    #     """
-    #
-    #     json_suffix = '.json'
-    #     dir_path_list = [p/str(doc_oid) for doc_oid in downloads]
-    #
-    #     for file_refs, dir_path in zip([i for i in downloads.values()],
-    #                                    dir_path_list):
-    #         os.mkdir(dir_path)
-    #         for file_ref in file_refs:
-    #             content = self.fs.get(file_ref)
-    #             filepath = dir_path / content.name
-    #             with open(filepath, 'wb') as f:
-    #                 f.write(content.read())
-    #
-    #         json_dir = dir_path / json_tree_file_name + json_suffix
-    #         # jsonファイルとして一時ディレクトリに保存
-    #         with json_dir.open('wb') as f:
-    #             f.write(encoded_json)
-    #
-    #     # 最終的にDLするzipファイルを作成
-    #     zip_filepath = shutil.make_archive('dl', 'zip', p)
-    #
-    #     return zip_filepath
-
-
     @staticmethod
     def zipped_json(encoded_json: bytes, json_tree_file_name: str) -> str:
         """
         jsonファイルとzipファイルを名前付きテンポラリとして生成し、パスを生成
         zipファイル内部にjson_tree_file_name.jsonのjsonファイルを含む
         添付ファイルがなく、jsonファイルだけ取得したい場合に使用する
+        # リファクタリング対象
 
         :param bytes encoded_json: json文字列としてダンプしたものを指定の文字コードでバイト列に変換したもの
         :param str json_tree_file_name: zipファイル内に配置するjsonファイルの名前
         :return:
         :rtype:str
         """
 
@@ -496,44 +482,14 @@
                     zip_filepath = fp.name
                     archive.write(filepath,
                                   arcname=json_tree_file_name + json_suffix)
         except Exception:
             raise
         return zip_filepath
 
-    @staticmethod
-    def zipped_json_path(encoded_json: bytes, json_tree_file_name: str,
-                     p: Path) -> Path:
-        """
-        zipファイル内部にjson_tree_file_name.jsonのjsonファイルを含む
-        添付ファイルがなく、jsonファイルだけ取得したい場合に使用する
-
-        :param bytes encoded_json: json文字列としてダンプしたものを指定の文字コードでバイト列に変換したもの
-        :param str json_tree_file_name: zipファイル内に配置するjsonファイルの名前
-        :param Path p: ファイルを保存するディレクトリのパス
-        :return:zip_filepath
-        :rtype:Path
-        """
-        zip_filename = json_tree_file_name + '.zip'
-        filename = json_tree_file_name + '.json'
-        jsonfile = p / filename
-        zip_filepath = p / zip_filename
-
-        try:
-            with jsonfile.open('wb') as f:
-                f.write(encoded_json)
-        except Exception:
-            raise
-        try:
-            with zipfile.ZipFile(zip_filepath, 'w', zipfile.ZIP_DEFLATED) as f:
-                f.write(jsonfile, arcname=filename)
-        except Exception:
-            raise
-        return zip_filepath
-
     def get_fileref_and_generate_dl_list(self, docs: dict,
                                          attach_key: str) -> tuple[dict, dict]:
         """
         json出力用の辞書内のファイルリファレンスをファイルパス文字列リストに置き換える
             例:
             {"_ed_file":[ObjectId('file_oid_1'),ObjectId('file_oid_2')]}
             ↓
```

### Comparing `edman-2023.5.15.1/edman/json_manager.py` & `edman-2023.5.8/edman/json_manager.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/edman/search.py` & `edman-2023.5.8/edman/search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/edman/utils.py` & `edman-2023.5.8/edman/utils.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/edman.egg-info/PKG-INFO` & `edman-2023.5.8/edman.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.5.15.1
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Author-email: Masaki Ohno <masakio@post.kek.jp>
+Home-page: https://github.com/ryde/edman
+Author: Masaki Ohno
+Author-email: masakio@post.kek.jp
 License: MIT License
-        
-        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: documentation, https://ryde.github.io/edman/
-Project-URL: repository, https://github.com/ryde/edman
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman
 =====
```

### Comparing `edman-2023.5.15.1/tests/test_convert.py` & `edman-2023.5.8/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/tests/test_db.py` & `edman-2023.5.8/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/tests/test_file.py` & `edman-2023.5.8/tests/test_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -454,42 +454,14 @@
             ps = list(p.glob('**/*.json'))[0]
             actual = ps.stem
 
         expected = filename
         self.assertEqual(expected, actual)
         os.unlink(ac_z_path)
 
-    def test_zipped_json2(self):
-
-        # # 正常系
-        s = {"document": [{"test1": "ABC"}, {"test2": 12345}]}
-        raw_json = dumps(s, ensure_ascii=False, indent=4)
-        encoded_json = raw_json.encode('utf-8')
-        filename = 'jsonfile'
-
-        with tempfile.TemporaryDirectory() as tmpdir:
-            p = Path(tmpdir)
-            ac_z_path = self.file.zipped_json_path(encoded_json, filename, p)
-
-            # 圧縮前のjsonファイルを削除する
-            first_file = filename + '.json'
-            first = p / first_file
-            first.unlink()
-
-            # ac_z_pathを解凍して中身のファイル名がzipped_filepathと同じか調べる
-            with zipfile.ZipFile(ac_z_path, 'r') as inputFile:
-                inputFile.extractall(tmpdir)
-
-            # 解凍されたディレクトリ名を取得する
-            ps = list(p.glob('**/*.json'))[0]
-            actual = ps.stem
-
-        expected = filename
-        self.assertEqual(expected, actual)
-
     def test_zipped_contents(self):
         if not self.db_server_connect:
             return
 
         with tempfile.TemporaryDirectory() as tmp_dl_dir:
             # 添付ファイル用テキストファイル作成
 
@@ -580,113 +552,14 @@
         self.assertDictEqual(res, actual_data['json_data'])
         self.assertEqual(test_var, actual_data['attached_data'])
 
         # テスト用zipファイル削除
         if os.path.exists(zip_filepath):
             os.remove(zip_filepath)
 
-    # def test_zipped_contents_path(self):
-    #     if not self.db_server_connect:
-    #         return
-    #
-    #     # TODO テストを書いている途中
-    #
-    #     with tempfile.TemporaryDirectory() as tmp_dl_dir:
-    #         # 添付ファイル用テキストファイル作成
-    #
-    #         test_var = 'test'
-    #         name = 'file_dl_list.txt'
-    #         input_filename = os.path.splitext(os.path.basename(name))[0]
-    #         file_dl_list = self.make_txt_files(tmp_dl_dir, name=input_filename,
-    #                                            text=test_var)
-    #
-    #         # ファイル読み込み、ファイルをgridfsに入れる
-    #         files_oid = []
-    #         self.fs = gridfs.GridFS(self.testdb)
-    #         for filename in file_dl_list:
-    #             metadata = {'filename': filename.name, 'compress': None}
-    #             with filename.open('rb') as f:
-    #                 files_oid.append(self.fs.put(f.read(), **metadata))
-    #
-    #         # docをDBに入れる
-    #         parent_id = ObjectId()
-    #         doc_id = ObjectId()
-    #         child_id = ObjectId()
-    #         parent_col = 'parent_col'
-    #         doc_col = 'doc_col'
-    #         child_col = 'child_col'
-    #         insert_docs = [
-    #             {
-    #                 'col': parent_col,
-    #                 'doc': {
-    #                     '_id': parent_id,
-    #                     'name': 'parent',
-    #                     Config.child: [DBRef(doc_col, doc_id)]
-    #                 },
-    #             },
-    #             {
-    #                 'col': doc_col,
-    #                 'doc': {
-    #                     '_id': doc_id,
-    #                     'name': 'doc',
-    #                     Config.file: files_oid,
-    #                     Config.parent: DBRef(parent_col, parent_id),
-    #                     Config.child: [DBRef(child_col, child_id)]
-    #                 }
-    #             },
-    #             {
-    #                 'col': child_col,
-    #                 'doc': {
-    #                     '_id': child_id,
-    #                     'name': 'child',
-    #                     Config.parent: DBRef(doc_col, doc_id),
-    #                 }
-    #             }]
-    #         result = {}
-    #         for i in insert_docs:
-    #             insert_result = self.testdb[i['col']].insert_one(i['doc'])
-    #             result.update({i['col']: insert_result.inserted_id})
-    #
-    #         # # ドキュメントを取得する
-    #         search = Search(self.db)
-    #         exclusion = ['_id', Config.file]
-    #         docs = search.find(doc_col, {'_id': result[doc_col]}, 1, 1,
-    #                            exclusion)
-    #         result_with_filepath, downloads = self.file.get_fileref_and_generate_dl_list(
-    #             docs, "_ed_attachment")
-    #         res = search.process_data_derived_from_mongodb(
-    #             result_with_filepath)
-    #
-    #     # 実行
-    #     raw_json = dumps(res, ensure_ascii=False, indent=4)
-    #     encoded_json = raw_json.encode('utf-8')
-    #     json_tree_file_name = 'json_tree'
-    #
-    #     with tempfile.TemporaryDirectory() as tmp:
-    #         p = Path(tmp)
-    #         zip_filepath = self.file.zipped_contents_path(downloads,
-    #                                                  json_tree_file_name,
-    #                                                  encoded_json, p)
-    #         # 解凍
-    #         shutil.unpack_archive(zip_filepath, tmp)
-    #         # 添付ファイルを読み込んでテキストの中身を抽出
-    #         path_lists = [tmp, str(list(downloads.keys())[0]), name]
-    #         with open(os.path.join(*path_lists)) as f:
-    #             attached_s = f.read()
-    #         path_lists = [tmp, json_tree_file_name + '.json']
-    #         json_file_path = os.path.join(*path_lists)
-    #         with open(json_file_path) as jf:
-    #             j_data = json.load(jf)
-    #         # 外に出すデータを組み立て(zip内部のjsonデータ、上記の添付ファイルデータ)
-    #         actual_data = {'json_data': j_data, 'attached_data': attached_s}
-    #     # テスト
-    #     self.assertDictEqual(res, actual_data['json_data'])
-    #     self.assertEqual(test_var, actual_data['attached_data'])
-
-
     def test_get_fileref_and_generate_dl_list(self):
 
         if not self.db_server_connect:
             return
 
         # DBにdocsと添付ファイルを挿入する
         with tempfile.TemporaryDirectory() as tmp_dl_dir:
@@ -764,20 +637,18 @@
             # ファイル読み込み、ファイルをgridfsに入れる
             files_oid = []
             self.fs = gridfs.GridFS(self.testdb)
             test_vars = {}
             for filename in files:
                 with filename.open('rb') as f:
                     content = f.read()
-                    # file_obj = gzip.compress(content, compresslevel=6)
-                    # files_oid.append(
-                    #     self.fs.put(file_obj, filename=filename.name,
-                    #                 compress='gzip'))
+                    file_obj = gzip.compress(content, compresslevel=6)
                     files_oid.append(
-                        self.fs.put(content, filename=filename.name))
+                        self.fs.put(file_obj, filename=filename.name,
+                                    compress='gzip'))
                     test_vars.update({filename.name: content.decode()})
 
         with tempfile.TemporaryDirectory() as tmp_dl_dir:
             path = Path(tmp_dl_dir)
 
             grid_out_result = self.file._grid_out(files_oid, tmp_dl_dir)
             # 実行結果
@@ -1014,31 +885,28 @@
         if not self.db_server_connect:
             return
 
         # 正常系
         with tempfile.TemporaryDirectory() as tmp_dir:
             sample_files = self.make_txt_files(tmp_dir, name='grid_in_test',
                                                qty=2)
-            compress_settings = [False, False]
+            compress_settings = [True, False]
             td = tuple(
                 [(p, b) for (p, b) in zip(sample_files, compress_settings)])
 
             self.fs = gridfs.GridFS(self.testdb)
             actual = []
             for oid in self.file.grid_in(td):
                 data = self.fs.get(oid)
-                # if data.compress == 'gzip':
-                #     f_data = gzip.decompress(data.read()).decode()
-                #     b_data = True
-                # else:
-                #     f_data = data.read().decode()
-                #     b_data = False
-
-                f_data = data.read().decode()
-                b_data = False
+                if data.compress == 'gzip':
+                    f_data = gzip.decompress(data.read()).decode()
+                    b_data = True
+                else:
+                    f_data = data.read().decode()
+                    b_data = False
                 actual.append([data.filename, f_data, b_data])
 
             expected = []
             for file_path, compress in zip(sample_files, compress_settings):
                 with file_path.open() as f:
                     expected.append([file_path.name, f.read(), compress])
```

### Comparing `edman-2023.5.15.1/tests/test_multiuser.py` & `edman-2023.5.8/tests/test_multiuser.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/tests/test_search.py` & `edman-2023.5.8/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.15.1/tests/test_utils.py` & `edman-2023.5.8/tests/test_utils.py`

 * *Files identical despite different names*

