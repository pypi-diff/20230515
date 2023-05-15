# Comparing `tmp/gandai-1.1.7.tar.gz` & `tmp/gandai-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.1.7.tar", last modified: Sun May 14 18:15:28 2023, max compression
+gzip compressed data, was "gandai-1.1.8.tar", last modified: Mon May 15 00:34:47 2023, max compression
```

## Comparing `gandai-1.1.7.tar` & `gandai-1.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.373960 gandai-1.1.7/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.7/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-14 18:15:28.373853 gandai-1.1.7/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.371071 gandai-1.1.7/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-13 19:24:50.000000 gandai-1.1.7/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.372893 gandai-1.1.7/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-13 19:25:52.000000 gandai-1.1.7/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.7/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.7/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4064 2023-05-14 00:47:34.000000 gandai-1.1.7/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2075 2023-05-13 19:36:23.000000 gandai-1.1.7/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.7/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5068 2023-05-12 19:30:40.000000 gandai-1.1.7/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6137 2023-05-14 03:30:02.000000 gandai-1.1.7/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16436 2023-05-14 01:24:41.000000 gandai-1.1.7/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.7/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7849 2023-05-12 19:25:42.000000 gandai-1.1.7/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1699 2023-05-13 19:58:43.000000 gandai-1.1.7/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1583 2023-05-14 00:47:07.000000 gandai-1.1.7/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)     2451 2023-05-13 19:35:44.000000 gandai-1.1.7/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     3295 2023-05-14 18:08:29.000000 gandai-1.1.7/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.373338 gandai-1.1.7/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.7/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.373572 gandai-1.1.7/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.1.7/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6424 2023-05-14 03:30:02.000000 gandai-1.1.7/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-13 19:26:13.000000 gandai-1.1.7/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1626 2023-05-14 03:24:47.000000 gandai-1.1.7/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3257 2023-05-14 17:36:57.000000 gandai-1.1.7/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.373704 gandai-1.1.7/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)     2843 2023-05-14 17:45:11.000000 gandai-1.1.7/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2642 2023-05-14 03:28:36.000000 gandai-1.1.7/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)     8697 2023-05-14 01:24:23.000000 gandai-1.1.7/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     5442 2023-05-14 02:14:15.000000 gandai-1.1.7/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-14 18:15:28.371575 gandai-1.1.7/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-14 18:15:28.000000 gandai-1.1.7/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1015 2023-05-14 18:15:28.000000 gandai-1.1.7/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-14 18:15:28.000000 gandai-1.1.7/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-14 18:15:28.000000 gandai-1.1.7/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2023-05-14 18:09:10.000000 gandai-1.1.7/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-14 18:15:28.373990 gandai-1.1.7/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.7/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.389003 gandai-1.1.8/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.8/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-15 00:34:47.388872 gandai-1.1.8/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.384188 gandai-1.1.8/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-13 19:24:50.000000 gandai-1.1.8/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.386850 gandai-1.1.8/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-13 19:25:52.000000 gandai-1.1.8/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.8/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-15 00:21:53.000000 gandai-1.1.8/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4064 2023-05-14 00:47:34.000000 gandai-1.1.8/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2075 2023-05-13 19:36:23.000000 gandai-1.1.8/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.8/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5474 2023-05-15 00:13:44.000000 gandai-1.1.8/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6137 2023-05-14 03:30:02.000000 gandai-1.1.8/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17744 2023-05-15 00:13:44.000000 gandai-1.1.8/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.8/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8074 2023-05-15 00:13:44.000000 gandai-1.1.8/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1703 2023-05-15 00:33:20.000000 gandai-1.1.8/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1583 2023-05-15 00:33:21.000000 gandai-1.1.8/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     2451 2023-05-13 19:35:44.000000 gandai-1.1.8/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     3443 2023-05-15 00:05:22.000000 gandai-1.1.8/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.387754 gandai-1.1.8/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.8/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.388321 gandai-1.1.8/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.1.8/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-14 19:49:36.000000 gandai-1.1.8/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-13 19:26:13.000000 gandai-1.1.8/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1655 2023-05-14 20:47:34.000000 gandai-1.1.8/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3257 2023-05-14 17:36:57.000000 gandai-1.1.8/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.388606 gandai-1.1.8/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)     2920 2023-05-15 00:05:33.000000 gandai-1.1.8/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2642 2023-05-14 03:28:36.000000 gandai-1.1.8/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)     9337 2023-05-15 00:00:59.000000 gandai-1.1.8/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     5497 2023-05-14 21:00:02.000000 gandai-1.1.8/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.384717 gandai-1.1.8/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-15 00:34:47.000000 gandai-1.1.8/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1015 2023-05-15 00:34:47.000000 gandai-1.1.8/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-15 00:34:47.000000 gandai-1.1.8/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-15 00:34:47.000000 gandai-1.1.8/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2023-05-15 00:34:23.000000 gandai-1.1.8/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-15 00:34:47.389036 gandai-1.1.8/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.8/setup.py
```

### Comparing `gandai-1.1.7/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xcfb22564 (Thu Mar 30 16:03:27 2023 UTC)
-files sz: 1704
+moddate:  0x207b6164 (Mon May 15 00:21:52 2023 UTC)
+files sz: 1703
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a01640064016c025a02640064026c036d045a046d
@@ -63,28 +63,28 @@
      7          70 LOAD_CONST               0 (0)
                 72 LOAD_CONST               5 (('Client',))
                 74 IMPORT_NAME             11 (twilio.rest)
                 76 IMPORT_FROM             12 (Client)
                 78 STORE_NAME              12 (Client)
                 80 POP_TOP
    
-     9          82 LOAD_CONST               0 (0)
+    11          82 LOAD_CONST               0 (0)
                 84 LOAD_CONST               6 (('Cloudstore',))
                 86 IMPORT_NAME             13 (gandai.datastore)
                 88 IMPORT_FROM             14 (Cloudstore)
                 90 STORE_NAME              14 (Cloudstore)
                 92 POP_TOP
    
-    13          94 PUSH_NULL
+    14          94 PUSH_NULL
                 96 LOAD_NAME               14 (Cloudstore)
                 98 PRECALL                  0
                102 CALL                     0
                112 STORE_NAME              15 (ds)
    
-    14         114 PUSH_NULL
+    15         114 PUSH_NULL
                116 LOAD_NAME               12 (Client)
                118 PUSH_NULL
                120 LOAD_NAME               10 (os)
                122 LOAD_ATTR               16 (getenv)
                132 LOAD_CONST               7 ('TWILIO_APP')
                134 PRECALL                  1
                138 CALL                     1
@@ -94,62 +94,62 @@
                162 LOAD_CONST               8 ('TWILIO_TOKEN')
                164 PRECALL                  1
                168 CALL                     1
                178 PRECALL                  2
                182 CALL                     2
                192 STORE_NAME              17 (twilio_client)
    
-    17         194 LOAD_NAME                5 (dataclass)
+    18         194 LOAD_NAME                5 (dataclass)
    
-    18         196 PUSH_NULL
+    19         196 PUSH_NULL
                198 LOAD_BUILD_CLASS
-               200 LOAD_CONST               9 (<code object Auth, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 17>)
+               200 LOAD_CONST               9 (<code object Auth, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 18>)
                202 MAKE_FUNCTION            0
                204 LOAD_CONST              10 ('Auth')
                206 PRECALL                  2
                210 CALL                     2
    
-    17         220 PRECALL                  0
+    18         220 PRECALL                  0
                224 CALL                     0
    
-    18         234 STORE_NAME              18 (Auth)
+    19         234 STORE_NAME              18 (Auth)
    
-    34         236 LOAD_CONST              11 ('auth')
+    35         236 LOAD_CONST              11 ('auth')
                238 LOAD_NAME               18 (Auth)
                240 LOAD_CONST              12 ('return')
                242 LOAD_CONST               1 (None)
                244 BUILD_TUPLE              4
-               246 LOAD_CONST              13 (<code object _send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 34>)
+               246 LOAD_CONST              13 (<code object _send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 35>)
                248 MAKE_FUNCTION            4 (annotations)
                250 STORE_NAME              19 (_send_code)
    
-    43         252 LOAD_CONST              14 ('phone')
+    44         252 LOAD_CONST              14 ('phone')
                254 LOAD_NAME               20 (str)
                256 LOAD_CONST              12 ('return')
                258 LOAD_CONST               1 (None)
                260 BUILD_TUPLE              4
-               262 LOAD_CONST              15 (<code object send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 43>)
+               262 LOAD_CONST              15 (<code object send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 44>)
                264 MAKE_FUNCTION            4 (annotations)
                266 STORE_NAME              21 (send_code)
    
-    51         268 LOAD_CONST              16 ('code')
+    52         268 LOAD_CONST              16 ('code')
                270 LOAD_NAME               20 (str)
                272 LOAD_CONST              12 ('return')
                274 LOAD_NAME               18 (Auth)
                276 BUILD_TUPLE              4
-               278 LOAD_CONST              17 (<code object authenticate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 51>)
+               278 LOAD_CONST              17 (<code object authenticate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 52>)
                280 MAKE_FUNCTION            4 (annotations)
                282 STORE_NAME              22 (authenticate)
    
-    63         284 LOAD_CONST              18 ('token')
+    64         284 LOAD_CONST              18 ('token')
                286 LOAD_NAME               20 (str)
                288 LOAD_CONST              12 ('return')
                290 LOAD_NAME               23 (bool)
                292 BUILD_TUPLE              4
-               294 LOAD_CONST              19 (<code object validate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 63>)
+               294 LOAD_CONST              19 (<code object validate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 64>)
                296 MAKE_FUNCTION            4 (annotations)
                298 STORE_NAME              24 (validate)
                300 LOAD_CONST               1 (None)
                302 RETURN_VALUE
    consts
       0
       None
@@ -167,68 +167,68 @@
          flags     : 0
          code
             0x970065005a0164005a025500020065036401ac02a6010000ab01000000
             00000000005a046505650664033c0000006505650664043c000000650565
             0664053c000000020065036401ac02a6010000ab0100000000000000005a
             076508650664063c000000020065036401ac02a6010000ab010000000000
             0000005a096505650664073c000000640884005a0a64095300
-          17           0 RESUME                   0
+          18           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Auth')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          19          12 PUSH_NULL
+          20          12 PUSH_NULL
                       14 LOAD_NAME                3 (field)
                       16 LOAD_CONST               1 (False)
                       18 KW_NAMES                 2
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_NAME               4 (key)
                       36 LOAD_NAME                5 (str)
                       38 LOAD_NAME                6 (__annotations__)
                       40 LOAD_CONST               3 ('key')
                       42 STORE_SUBSCR
          
-          20          46 LOAD_NAME                5 (str)
+          21          46 LOAD_NAME                5 (str)
                       48 LOAD_NAME                6 (__annotations__)
                       50 LOAD_CONST               4 ('phone')
                       52 STORE_SUBSCR
          
-          21          56 LOAD_NAME                5 (str)
+          22          56 LOAD_NAME                5 (str)
                       58 LOAD_NAME                6 (__annotations__)
                       60 LOAD_CONST               5 ('code')
                       62 STORE_SUBSCR
          
-          22          66 PUSH_NULL
+          23          66 PUSH_NULL
                       68 LOAD_NAME                3 (field)
                       70 LOAD_CONST               1 (False)
                       72 KW_NAMES                 2
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_NAME               7 (expires)
                       90 LOAD_NAME                8 (int)
                       92 LOAD_NAME                6 (__annotations__)
                       94 LOAD_CONST               6 ('expires')
                       96 STORE_SUBSCR
          
-          23         100 PUSH_NULL
+          24         100 PUSH_NULL
                      102 LOAD_NAME                3 (field)
                      104 LOAD_CONST               1 (False)
                      106 KW_NAMES                 2
                      108 PRECALL                  1
                      112 CALL                     1
                      122 STORE_NAME               9 (token)
                      124 LOAD_NAME                5 (str)
                      126 LOAD_NAME                6 (__annotations__)
                      128 LOAD_CONST               7 ('token')
                      130 STORE_SUBSCR
          
-          25         134 LOAD_CONST               8 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 25>)
+          26         134 LOAD_CONST               8 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 26>)
                      136 MAKE_FUNCTION            0
                      138 STORE_NAME              10 (__post_init__)
                      140 LOAD_CONST               9 (None)
                      142 RETURN_VALUE
          consts
             'Auth'
             False
@@ -254,71 +254,71 @@
                   00000000007c017a0000007c005f06000000000000000064047c006a0300
                   000000000000009b0064057c006a0600000000000000009b009d047c005f
                   0700000000000000007411000000000000000000007c006a070000000000
                   000000a0090000000000000000000000000000000000000000a6000000ab
                   000000000000000000a6010000ab010000000000000000a00a0000000000
                   000000000000000000000000000000a6000000ab0000000000000000007c
                   005f0b000000000000000064005300
-                25           0 RESUME                   0
+                26           0 RESUME                   0
                
-                26           2 LOAD_GLOBAL              1 (NULL + len)
+                27           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_GLOBAL              3 (NULL + str)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (code)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 PRECALL                  1
                             56 CALL                     1
                             66 LOAD_CONST               1 (6)
                             68 COMPARE_OP               2 (==)
                             74 POP_JUMP_FORWARD_IF_TRUE     2 (to 80)
                             76 LOAD_ASSERTION_ERROR
                             78 RAISE_VARARGS            1
                
-                27     >>   80 LOAD_GLOBAL              1 (NULL + len)
+                28     >>   80 LOAD_GLOBAL              1 (NULL + len)
                             92 LOAD_GLOBAL              3 (NULL + str)
                            104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                3 (phone)
                            116 PRECALL                  1
                            120 CALL                     1
                            130 PRECALL                  1
                            134 CALL                     1
                            144 LOAD_CONST               2 (10)
                            146 COMPARE_OP               2 (==)
                            152 POP_JUMP_FORWARD_IF_TRUE     2 (to 158)
                            154 LOAD_ASSERTION_ERROR
                            156 RAISE_VARARGS            1
                
-                28     >>  158 LOAD_CONST               3 (604800)
+                29     >>  158 LOAD_CONST               3 (604800)
                            160 STORE_FAST               1 (SEVEN_DAYS)
                
-                29         162 LOAD_GLOBAL              9 (NULL + int)
+                30         162 LOAD_GLOBAL              9 (NULL + int)
                            174 LOAD_GLOBAL             11 (NULL + time)
                            186 PRECALL                  0
                            190 CALL                     0
                            200 PRECALL                  1
                            204 CALL                     1
                            214 LOAD_FAST                1 (SEVEN_DAYS)
                            216 BINARY_OP                0 (+)
                            220 LOAD_FAST                0 (self)
                            222 STORE_ATTR               6 (expires)
                
-                30         232 LOAD_CONST               4 ('auth/')
+                31         232 LOAD_CONST               4 ('auth/')
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                3 (phone)
                            246 FORMAT_VALUE             0
                            248 LOAD_CONST               5 ('/')
                            250 LOAD_FAST                0 (self)
                            252 LOAD_ATTR                6 (expires)
                            262 FORMAT_VALUE             0
                            264 BUILD_STRING             4
                            266 LOAD_FAST                0 (self)
                            268 STORE_ATTR               7 (key)
                
-                31         278 LOAD_GLOBAL             17 (NULL + md5)
+                32         278 LOAD_GLOBAL             17 (NULL + md5)
                            290 LOAD_FAST                0 (self)
                            292 LOAD_ATTR                7 (key)
                            302 LOAD_METHOD              9 (encode)
                            324 PRECALL                  0
                            328 CALL                     0
                            338 PRECALL                  1
                            342 CALL                     1
@@ -338,24 +338,24 @@
                   '/'
                names      ('len', 'str', 'code', 'phone', 'int', 'time', 'expires', 'key', 'md5', 'encode', 'hexdigest', 'token')
                varnames   ('self', 'SEVEN_DAYS')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
                name       '__post_init__'
-               firstlineno 25
+               firstlineno 26
                lnotab 0x02014e014e01040146012e01
             None
          names      ('__name__', '__module__', '__qualname__', 'field', 'key', 'str', '__annotations__', 'expires', 'int', 'token', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'Auth'
-         firstlineno 17
+         firstlineno 18
          lnotab 0x0c0222010a010a0122012202
       'Auth'
       'auth'
       'return'
       code
          argcount  : 1
          nlocals   : 2
@@ -365,64 +365,64 @@
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007c006a03000000000000000074
             09000000000000000000006a0500000000000000006401a6010000ab0100
             000000000000007c006a0600000000000000009b0064029d02ac03a60300
             00ab0300000000000000007d01740f0000000000000000000064047c006a
             0300000000000000009b009d02a6010000ab010000000000000000010064
             005300
-          34           0 RESUME                   0
+          35           0 RESUME                   0
          
-          35           2 LOAD_GLOBAL              0 (twilio_client)
+          36           2 LOAD_GLOBAL              0 (twilio_client)
                       14 LOAD_ATTR                1 (messages)
                       24 LOAD_METHOD              2 (create)
          
-          36          46 LOAD_FAST                0 (auth)
+          37          46 LOAD_FAST                0 (auth)
                       48 LOAD_ATTR                3 (phone)
          
-          37          58 LOAD_GLOBAL              9 (NULL + os)
+          38          58 LOAD_GLOBAL              9 (NULL + os)
                       70 LOAD_ATTR                5 (getenv)
                       80 LOAD_CONST               1 ('TWILIO_NUMBER')
                       82 PRECALL                  1
                       86 CALL                     1
          
-          38          96 LOAD_FAST                0 (auth)
+          39          96 LOAD_FAST                0 (auth)
                       98 LOAD_ATTR                6 (code)
                      108 FORMAT_VALUE             0
-                     110 LOAD_CONST               2 (' is your G&AI Research authentication code.')
+                     110 LOAD_CONST               2 (' is your GA Research authentication code.')
                      112 BUILD_STRING             2
          
-          35         114 KW_NAMES                 3
+          36         114 KW_NAMES                 3
                      116 PRECALL                  3
                      120 CALL                     3
                      130 STORE_FAST               1 (message)
          
-          40         132 LOAD_GLOBAL             15 (NULL + print)
+          41         132 LOAD_GLOBAL             15 (NULL + print)
                      144 LOAD_CONST               4 ('Login Sent to ')
                      146 LOAD_FAST                0 (auth)
                      148 LOAD_ATTR                3 (phone)
                      158 FORMAT_VALUE             0
                      160 BUILD_STRING             2
                      162 PRECALL                  1
                      166 CALL                     1
                      176 POP_TOP
                      178 LOAD_CONST               0 (None)
                      180 RETURN_VALUE
          consts
             None
             'TWILIO_NUMBER'
-            ' is your G&AI Research authentication code.'
+            ' is your GA Research authentication code.'
             ('to', 'from_', 'body')
             'Login Sent to '
          names      ('twilio_client', 'messages', 'create', 'phone', 'os', 'getenv', 'code', 'print')
          varnames   ('auth', 'message')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       '_send_code'
-         firstlineno 34
+         firstlineno 35
          lnotab 0x02012c010c01260112fd1205
       'phone'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -430,45 +430,45 @@
             0x97007401000000000000000000007403000000000000000000006a0200
             0000000000000064016402a6020000ab020000000000000000a6010000ab
             0100000000000000007d017407000000000000000000007c007c01ac03a6
             020000ab0200000000000000007d027409000000000000000000007c02a6
             010000ab010000000000000000740a000000000000000000007c026a0600
             000000000000003c000000740f000000000000000000007c02a6010000ab
             010000000000000000010064005300
-          43           0 RESUME                   0
+          44           0 RESUME                   0
          
-          45           2 LOAD_GLOBAL              1 (NULL + str)
+          46           2 LOAD_GLOBAL              1 (NULL + str)
                       14 LOAD_GLOBAL              3 (NULL + random)
                       26 LOAD_ATTR                2 (randint)
                       36 LOAD_CONST               1 (100000)
                       38 LOAD_CONST               2 (999999)
                       40 PRECALL                  2
                       44 CALL                     2
                       54 PRECALL                  1
                       58 CALL                     1
                       68 STORE_FAST               1 (auth_code)
          
-          46          70 LOAD_GLOBAL              7 (NULL + Auth)
+          47          70 LOAD_GLOBAL              7 (NULL + Auth)
                       82 LOAD_FAST                0 (phone)
                       84 LOAD_FAST                1 (auth_code)
                       86 KW_NAMES                 3
                       88 PRECALL                  2
                       92 CALL                     2
                      102 STORE_FAST               2 (auth)
          
-          47         104 LOAD_GLOBAL              9 (NULL + asdict)
+          48         104 LOAD_GLOBAL              9 (NULL + asdict)
                      116 LOAD_FAST                2 (auth)
                      118 PRECALL                  1
                      122 CALL                     1
                      132 LOAD_GLOBAL             10 (ds)
                      144 LOAD_FAST                2 (auth)
                      146 LOAD_ATTR                6 (key)
                      156 STORE_SUBSCR
          
-          48         160 LOAD_GLOBAL             15 (NULL + _send_code)
+          49         160 LOAD_GLOBAL             15 (NULL + _send_code)
                      172 LOAD_FAST                2 (auth)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 POP_TOP
                      190 LOAD_CONST               0 (None)
                      192 RETURN_VALUE
          consts
@@ -478,15 +478,15 @@
             ('phone', 'code')
          names      ('str', 'random', 'randint', 'Auth', 'asdict', 'ds', 'key', '_send_code')
          varnames   ('phone', 'auth_code', 'auth')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'send_code'
-         firstlineno 43
+         firstlineno 44
          lnotab 0x0202440122013801
       'code'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -500,80 +500,80 @@
             00000000000000740d00000000000000000000a6000000ab000000000000
             000000a6010000ab0100000000000000006b040000000019000000000000
             0000007d027c027c026404190000000000000000007c006b020000000019
             0000000000000000007d02740f000000000000000000007c02a6010000ab
             01000000000000000064056b0400000000721c7c02a00800000000000000
             000000000000000000000000006406ac07a6010000ab0100000000000000
             00640519000000000000000000530064005300
-          51           0 RESUME                   0
+          52           0 RESUME                   0
          
-          52           2 LOAD_GLOBAL              0 (ds)
+          53           2 LOAD_GLOBAL              0 (ds)
                       14 LOAD_METHOD              1 (keys)
                       36 LOAD_CONST               1 ('auth/')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 LOAD_CONST               2 (1)
                       54 LOAD_CONST               0 (None)
                       56 BUILD_SLICE              2
                       58 BINARY_SUBSCR
                       68 STORE_FAST               1 (keys)
          
-          53          70 LOAD_GLOBAL              5 (NULL + pd)
+          54          70 LOAD_GLOBAL              5 (NULL + pd)
                       82 LOAD_ATTR                3 (DataFrame)
                       92 LOAD_GLOBAL              0 (ds)
                      104 LOAD_METHOD              4 (load_async)
                      126 LOAD_FAST                1 (keys)
                      128 PRECALL                  1
                      132 CALL                     1
                      142 PRECALL                  1
                      146 CALL                     1
                      156 STORE_FAST               2 (df)
          
-          54         158 LOAD_FAST                2 (df)
+          55         158 LOAD_FAST                2 (df)
                      160 LOAD_FAST                2 (df)
                      162 LOAD_CONST               3 ('expires')
                      164 BINARY_SUBSCR
                      174 LOAD_GLOBAL             11 (NULL + int)
                      186 LOAD_GLOBAL             13 (NULL + time)
                      198 PRECALL                  0
                      202 CALL                     0
                      212 PRECALL                  1
                      216 CALL                     1
                      226 COMPARE_OP               4 (>)
                      232 BINARY_SUBSCR
                      242 STORE_FAST               2 (df)
          
-          55         244 LOAD_FAST                2 (df)
+          56         244 LOAD_FAST                2 (df)
                      246 LOAD_FAST                2 (df)
                      248 LOAD_CONST               4 ('code')
                      250 BINARY_SUBSCR
                      260 LOAD_FAST                0 (code)
                      262 COMPARE_OP               2 (==)
                      268 BINARY_SUBSCR
                      278 STORE_FAST               2 (df)
          
-          56         280 LOAD_GLOBAL             15 (NULL + len)
+          57         280 LOAD_GLOBAL             15 (NULL + len)
                      292 LOAD_FAST                2 (df)
                      294 PRECALL                  1
                      298 CALL                     1
                      308 LOAD_CONST               5 (0)
                      310 COMPARE_OP               4 (>)
                      316 POP_JUMP_FORWARD_IF_FALSE    28 (to 374)
          
-          58         318 LOAD_FAST                2 (df)
+          59         318 LOAD_FAST                2 (df)
                      320 LOAD_METHOD              8 (to_dict)
                      342 LOAD_CONST               6 ('records')
                      344 KW_NAMES                 7
                      346 PRECALL                  1
                      350 CALL                     1
                      360 LOAD_CONST               5 (0)
                      362 BINARY_SUBSCR
                      372 RETURN_VALUE
          
-          60     >>  374 LOAD_CONST               0 (None)
+          61     >>  374 LOAD_CONST               0 (None)
                      376 RETURN_VALUE
          consts
             None
             'auth/'
             1
             'expires'
             'code'
@@ -582,40 +582,40 @@
             ('orient',)
          names      ('ds', 'keys', 'pd', 'DataFrame', 'load_async', 'int', 'time', 'len', 'to_dict')
          varnames   ('code', 'keys', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'authenticate'
-         firstlineno 51
+         firstlineno 52
          lnotab 0x0201440158015601240126023802
       'token'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 1
          flags     : 3
          code 0x970064005300
-          63           0 RESUME                   0
+          64           0 RESUME                   0
          
-          64           2 LOAD_CONST               0 (None)
+          65           2 LOAD_CONST               0 (None)
                        4 RETURN_VALUE
          consts
             None
          names      ()
          varnames   ('token',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'validate'
-         firstlineno 63
+         firstlineno 64
          lnotab 0x0201
    names      ('pandas', 'pd', 'random', 'dataclasses', 'asdict', 'dataclass', 'field', 'hashlib', 'md5', 'time', 'os', 'twilio.rest', 'Client', 'gandai.datastore', 'Cloudstore', 'ds', 'getenv', 'twilio_client', 'Auth', '_send_code', 'str', 'send_code', 'authenticate', 'bool', 'validate')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080114010c010c0108010c020c0414015003020118ff0e
+      0x00ff02010801080114010c010c0108010c040c0314015003020118ff0e
       01021010091008100c
```

### Comparing `gandai-1.1.7/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0xdd935e64 (Fri May 12 19:30:37 2023 UTC)
-files sz: 3286
+moddate:  0x42776164 (Mon May 15 00:05:22 2023 UTC)
+files sz: 3443
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a030100640064036c046d
-      055a056d065a060100640064046c076d085a086d095a096d0a5a0a010064
-      0064056c0b6d0c5a0c0100640064066c0d6d0e5a0f010064076508640864
-      016604640984045a10640a6511640865116604640b84045a1264015300
+      055a056d065a060100640064046c076d085a080100640064056c096d0a5a
+      0a6d0b5a0b6d0c5a0c0100640064066c0d6d0e5a0e0100640064076c0f6d
+      105a11010064086512640964016604640a84045a13640b65126409651266
+      04640c84045a1464015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (pandas)
                  8 STORE_NAME               1 (pd)
    
@@ -30,371 +31,391 @@
                 26 IMPORT_NAME              4 (dataclasses)
                 28 IMPORT_FROM              5 (dataclass)
                 30 STORE_NAME               5 (dataclass)
                 32 IMPORT_FROM              6 (field)
                 34 STORE_NAME               6 (field)
                 36 POP_TOP
    
-     6          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               4 (('Event', 'Company', 'Checkpoint'))
-                42 IMPORT_NAME              7 (gandai.models)
-                44 IMPORT_FROM              8 (Event)
-                46 STORE_NAME               8 (Event)
-                48 IMPORT_FROM              9 (Company)
-                50 STORE_NAME               9 (Company)
-                52 IMPORT_FROM             10 (Checkpoint)
-                54 STORE_NAME              10 (Checkpoint)
-                56 POP_TOP
+     4          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               4 (('ThreadPoolExecutor',))
+                42 IMPORT_NAME              7 (concurrent.futures)
+                44 IMPORT_FROM              8 (ThreadPoolExecutor)
+                46 STORE_NAME               8 (ThreadPoolExecutor)
+                48 POP_TOP
    
-     7          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               5 (('query',))
-                62 IMPORT_NAME             11 (gandai)
-                64 IMPORT_FROM             12 (query)
-                66 STORE_NAME              12 (query)
+     6          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               5 (('Event', 'Company', 'Checkpoint'))
+                54 IMPORT_NAME              9 (gandai.models)
+                56 IMPORT_FROM             10 (Event)
+                58 STORE_NAME              10 (Event)
+                60 IMPORT_FROM             11 (Company)
+                62 STORE_NAME              11 (Company)
+                64 IMPORT_FROM             12 (Checkpoint)
+                66 STORE_NAME              12 (Checkpoint)
                 68 POP_TOP
    
-     9          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               6 (('GrataWrapper',))
-                74 IMPORT_NAME             13 (gandai.sources)
-                76 IMPORT_FROM             14 (GrataWrapper)
-                78 STORE_NAME              15 (grata)
+     7          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               6 (('query',))
+                74 IMPORT_NAME             13 (gandai)
+                76 IMPORT_FROM             14 (query)
+                78 STORE_NAME              14 (query)
                 80 POP_TOP
    
-    12          82 LOAD_CONST               7 ('e')
-                84 LOAD_NAME                8 (Event)
-                86 LOAD_CONST               8 ('return')
-                88 LOAD_CONST               1 (None)
-                90 BUILD_TUPLE              4
-                92 LOAD_CONST               9 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 12>)
-                94 MAKE_FUNCTION            4 (annotations)
-                96 STORE_NAME              16 (process_event)
+     9          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               7 (('GrataWrapper',))
+                86 IMPORT_NAME             15 (gandai.sources)
+                88 IMPORT_FROM             16 (GrataWrapper)
+                90 STORE_NAME              17 (grata)
+                92 POP_TOP
    
-    85          98 LOAD_CONST              10 ('search_uid')
-               100 LOAD_NAME               17 (int)
-               102 LOAD_CONST               8 ('return')
-               104 LOAD_NAME               17 (int)
-               106 BUILD_TUPLE              4
-               108 LOAD_CONST              11 (<code object process_events, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 85>)
-               110 MAKE_FUNCTION            4 (annotations)
-               112 STORE_NAME              18 (process_events)
-               114 LOAD_CONST               1 (None)
-               116 RETURN_VALUE
+    12          94 LOAD_CONST               8 ('event_id')
+                96 LOAD_NAME               18 (int)
+                98 LOAD_CONST               9 ('return')
+               100 LOAD_CONST               1 (None)
+               102 BUILD_TUPLE              4
+               104 LOAD_CONST              10 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 12>)
+               106 MAKE_FUNCTION            4 (annotations)
+               108 STORE_NAME              19 (process_event)
+   
+    91         110 LOAD_CONST              11 ('search_uid')
+               112 LOAD_NAME               18 (int)
+               114 LOAD_CONST               9 ('return')
+               116 LOAD_NAME               18 (int)
+               118 BUILD_TUPLE              4
+               120 LOAD_CONST              12 (<code object process_events, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 91>)
+               122 MAKE_FUNCTION            4 (annotations)
+               124 STORE_NAME              20 (process_events)
+               126 LOAD_CONST               1 (None)
+               128 RETURN_VALUE
    consts
       0
       None
       ('from_dict',)
       ('dataclass', 'field')
+      ('ThreadPoolExecutor',)
       ('Event', 'Company', 'Checkpoint')
       ('query',)
       ('GrataWrapper',)
-      'e'
+      'event_id'
       'return'
       code
          argcount  : 1
-         nlocals   : 5
+         nlocals   : 6
          stacksize : 6
          flags     : 3
          code
-            0x8705970064017400000000000000000000006402740000000000000000
-            000000640364006606880566016404840c7d017c006a0100000000000000
-            008a057c006a02000000000000000064056b0200000000720290016eeb7c
-            006a02000000000000000064066b020000000072c7740700000000000000
-            0000006a0400000000000000007c006a050000000000000000a6010000ab
-            0100000000000000007d02740d000000000000000000006a070000000000
-            0000007c026a050000000000000000a6010000ab0100000000000000007d
-            037c03a00800000000000000000000000000000000000000006407a60100
-            00ab01000000000000000064086b02000000007214741300000000000000
-            0000007c029b0064099d02a6010000ab010000000000000000010090016e
-            817413000000000000000000007c03a6010000ab01000000000000000001
-            007c03a0080000000000000000000000000000000000000000640aa60100
-            00ab0100000000000000007c025f0a00000000000000007c03a008000000
-            0000000000000000000000000000000000640ba6010000ab010000000000
-            0000007c025f0b00000000000000007c026a0c00000000000000007c037a
-            0700007c025f0c00000000000000007407000000000000000000006a0d00
-            000000000000007c02a6010000ab010000000000000000010090016e197c
-            006a020000000000000000640c6b02000000007266740700000000000000
-            0000006a0e00000000000000008905a6010000ab0100000000000000007d
-            0402007c01740d000000000000000000006a0f00000000000000007c006a
-            0500000000000000007c04ac0da6020000ab020000000000000000740700
-            0000000000000000006a1000000000000000008905ac0ea6010000ab0100
-            00000000000000640f19000000000000000000a011000000000000000000
-            0000000000000000000000a6000000ab000000000000000000ac10a60200
-            00ab02000000000000000001006ea87c006a02000000000000000064116b
-            020000000072016e9c7c006a02000000000000000064126b020000000072
-            016e907c006a02000000000000000064136b020000000072016e847c006a
-            02000000000000000064146b020000000072016e787c006a020000000000
-            00000064156b0200000000726d7413000000000000000000006416a60100
-            00ab01000000000000000001007407000000000000000000006a0e000000
-            00000000008905a6010000ab0100000000000000007d0402007c01740d00
-            0000000000000000006a1200000000000000007c04a6010000ab01000000
-            00000000007407000000000000000000006a1000000000000000008905ac
-            0ea6010000ab010000000000000000640f19000000000000000000a01100
-            00000000000000000000000000000000000000a6000000ab000000000000
-            000000ac10a6020000ab0200000000000000000100740700000000000000
-            0000006a1300000000000000007429000000000000000000007c006a1500
-            00000000000000ac17a6010000ab010000000000000000a6010000ab0100
-            00000000000000010074130000000000000000000064187c009b009d02a6
-            010000ab010000000000000000010064005300
-                       0 MAKE_CELL                5 (search_uid)
+            0x8706970064017400000000000000000000006402740000000000000000
+            000000640364046606880666016405840c7d017403000000000000000000
+            006a0200000000000000007c00a6010000ab0100000000000000007d027c
+            026a0300000000000000008a067c026a04000000000000000064066b0200
+            000000720290016eec7c026a04000000000000000064076b020000000072
+            c87403000000000000000000006a0500000000000000007c026a06000000
+            0000000000a6010000ab0100000000000000007d03740f00000000000000
+            0000006a0800000000000000007c036a060000000000000000a6010000ab
+            0100000000000000007d047c04a009000000000000000000000000000000
+            00000000006408a6010000ab01000000000000000064096b020000000072
+            147415000000000000000000007c039b00640a9d02a6010000ab01000000
+            0000000000010090016e827415000000000000000000007c04a6010000ab
+            01000000000000000001007c04a009000000000000000000000000000000
+            0000000000640ba6010000ab0100000000000000007c035f0b0000000000
+            0000007c04a0090000000000000000000000000000000000000000640ca6
+            010000ab0100000000000000007c035f0c000000000000000069007c036a
+            0d0000000000000000a5017c04a5017c035f0d0000000000000000740300
+            0000000000000000006a0e00000000000000007c03a6010000ab01000000
+            0000000000010090016e197c026a040000000000000000640d6b02000000
+            0072667403000000000000000000006a0f00000000000000008906a60100
+            00ab0100000000000000007d0502007c01740f000000000000000000006a
+            1000000000000000007c026a0600000000000000007c05ac0ea6020000ab
+            0200000000000000007403000000000000000000006a1100000000000000
+            008906ac0fa6010000ab0100000000000000006410190000000000000000
+            00a0120000000000000000000000000000000000000000a6000000ab0000
+            00000000000000ac11a6020000ab02000000000000000001006ea87c026a
+            04000000000000000064126b020000000072016e9c7c026a040000000000
+            00000064136b020000000072016e907c026a04000000000000000064146b
+            020000000072016e847c026a04000000000000000064156b020000000072
+            016e787c026a04000000000000000064166b0200000000726d7415000000
+            000000000000006417a6010000ab01000000000000000001007403000000
+            000000000000006a0f00000000000000008906a6010000ab010000000000
+            0000007d0502007c01740f000000000000000000006a1300000000000000
+            007c05a6010000ab0100000000000000007403000000000000000000006a
+            1100000000000000008906ac0fa6010000ab010000000000000000641019
+            000000000000000000a01200000000000000000000000000000000000000
+            00a6000000ab000000000000000000ac11a6020000ab0200000000000000
+            0001007403000000000000000000006a140000000000000000742b000000
+            000000000000007c026a160000000000000000ac18a6010000ab01000000
+            0000000000a6010000ab0100000000000000000100741500000000000000
+            00000064197c029b009d02a6010000ab0100000000000000000100640453
+            00
+                       0 MAKE_CELL                6 (search_uid)
          
           12           2 RESUME                   0
          
-          14           4 LOAD_CONST               1 ('companies')
+          18           4 LOAD_CONST               1 ('companies')
                        6 LOAD_GLOBAL              0 (list)
                       18 LOAD_CONST               2 ('existing_domains')
                       20 LOAD_GLOBAL              0 (list)
                       32 LOAD_CONST               3 ('return')
-                      34 LOAD_CONST               0 (None)
+                      34 LOAD_CONST               4 (None)
                       36 BUILD_TUPLE              6
-                      38 LOAD_CLOSURE             5 (search_uid)
+                      38 LOAD_CLOSURE             6 (search_uid)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               4 (<code object _insert_companies, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 14>)
+                      42 LOAD_CONST               5 (<code object _insert_companies, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 18>)
                       44 MAKE_FUNCTION           12 (annotations, closure)
                       46 STORE_FAST               1 (_insert_companies)
          
-          41          48 LOAD_FAST                0 (e)
-                      50 LOAD_ATTR                1 (search_uid)
-                      60 STORE_DEREF              5 (search_uid)
-         
-          42          62 LOAD_FAST                0 (e)
-                      64 LOAD_ATTR                2 (type)
-                      74 LOAD_CONST               5 ('create')
-                      76 COMPARE_OP               2 (==)
-                      82 POP_JUMP_FORWARD_IF_FALSE     2 (to 88)
-         
-          43          84 EXTENDED_ARG             1
-                      86 JUMP_FORWARD           491 (to 1070)
-         
-          44     >>   88 LOAD_FAST                0 (e)
-                      90 LOAD_ATTR                2 (type)
-                     100 LOAD_CONST               6 ('advance')
-                     102 COMPARE_OP               2 (==)
-                     108 POP_JUMP_FORWARD_IF_FALSE   199 (to 508)
-         
-          46         110 LOAD_GLOBAL              7 (NULL + query)
-                     122 LOAD_ATTR                4 (find_company_by_domain)
-                     132 LOAD_FAST                0 (e)
-                     134 LOAD_ATTR                5 (domain)
-                     144 PRECALL                  1
-                     148 CALL                     1
-                     158 STORE_FAST               2 (company)
-         
-          48         160 LOAD_GLOBAL             13 (NULL + grata)
-                     172 LOAD_ATTR                7 (enrich)
-                     182 LOAD_FAST                2 (company)
-                     184 LOAD_ATTR                5 (domain)
-                     194 PRECALL                  1
-                     198 CALL                     1
-                     208 STORE_FAST               3 (resp)
-         
-          49         210 LOAD_FAST                3 (resp)
-                     212 LOAD_METHOD              8 (get)
-                     234 LOAD_CONST               7 ('status')
-                     236 PRECALL                  1
-                     240 CALL                     1
-                     250 LOAD_CONST               8 (404)
-                     252 COMPARE_OP               2 (==)
-                     258 POP_JUMP_FORWARD_IF_FALSE    20 (to 300)
-         
-          50         260 LOAD_GLOBAL             19 (NULL + print)
-                     272 LOAD_FAST                2 (company)
-                     274 FORMAT_VALUE             0
-                     276 LOAD_CONST               9 (' not found')
-                     278 BUILD_STRING             2
-                     280 PRECALL                  1
-                     284 CALL                     1
-                     294 POP_TOP
-                     296 EXTENDED_ARG             1
-                     298 JUMP_FORWARD           385 (to 1070)
-         
-          52     >>  300 LOAD_GLOBAL             19 (NULL + print)
-                     312 LOAD_FAST                3 (resp)
-                     314 PRECALL                  1
-                     318 CALL                     1
-                     328 POP_TOP
-         
-          53         330 LOAD_FAST                3 (resp)
-                     332 LOAD_METHOD              8 (get)
-                     354 LOAD_CONST              10 ('name')
-                     356 PRECALL                  1
-                     360 CALL                     1
-                     370 LOAD_FAST                2 (company)
-                     372 STORE_ATTR              10 (name)
-         
-          54         382 LOAD_FAST                3 (resp)
-                     384 LOAD_METHOD              8 (get)
-                     406 LOAD_CONST              11 ('description')
-                     408 PRECALL                  1
-                     412 CALL                     1
-                     422 LOAD_FAST                2 (company)
-                     424 STORE_ATTR              11 (description)
-         
-          55         434 LOAD_FAST                2 (company)
-                     436 LOAD_ATTR               12 (meta)
-                     446 LOAD_FAST                3 (resp)
-                     448 BINARY_OP                7 (|)
-                     452 LOAD_FAST                2 (company)
-                     454 STORE_ATTR              12 (meta)
-         
-          56         464 LOAD_GLOBAL              7 (NULL + query)
-                     476 LOAD_ATTR               13 (update_company)
-                     486 LOAD_FAST                2 (company)
-                     488 PRECALL                  1
-                     492 CALL                     1
-                     502 POP_TOP
-                     504 EXTENDED_ARG             1
-                     506 JUMP_FORWARD           281 (to 1070)
-         
-          58     >>  508 LOAD_FAST                0 (e)
-                     510 LOAD_ATTR                2 (type)
-                     520 LOAD_CONST              12 ('validate')
-                     522 COMPARE_OP               2 (==)
-                     528 POP_JUMP_FORWARD_IF_FALSE   102 (to 734)
-         
-          59         530 LOAD_GLOBAL              7 (NULL + query)
-                     542 LOAD_ATTR               14 (find_search_by_uid)
-                     552 LOAD_DEREF               5 (search_uid)
-                     554 PRECALL                  1
-                     558 CALL                     1
-                     568 STORE_FAST               4 (search)
-         
-          60         570 PUSH_NULL
-                     572 LOAD_FAST                1 (_insert_companies)
-         
-          61         574 LOAD_GLOBAL             13 (NULL + grata)
-                     586 LOAD_ATTR               15 (find_similar)
-                     596 LOAD_FAST                0 (e)
-                     598 LOAD_ATTR                5 (domain)
-                     608 LOAD_FAST                4 (search)
-                     610 KW_NAMES                13
-                     612 PRECALL                  2
-                     616 CALL                     2
-         
-          62         626 LOAD_GLOBAL              7 (NULL + query)
-                     638 LOAD_ATTR               16 (target)
-                     648 LOAD_DEREF               5 (search_uid)
-                     650 KW_NAMES                14
-                     652 PRECALL                  1
-                     656 CALL                     1
-                     666 LOAD_CONST              15 ('domain')
-                     668 BINARY_SUBSCR
-                     678 LOAD_METHOD             17 (tolist)
-                     700 PRECALL                  0
-                     704 CALL                     0
-         
-          60         714 KW_NAMES                16
-                     716 PRECALL                  2
-                     720 CALL                     2
-                     730 POP_TOP
-                     732 JUMP_FORWARD           168 (to 1070)
-         
-          64     >>  734 LOAD_FAST                0 (e)
-                     736 LOAD_ATTR                2 (type)
-                     746 LOAD_CONST              17 ('send')
-                     748 COMPARE_OP               2 (==)
-                     754 POP_JUMP_FORWARD_IF_FALSE     1 (to 758)
-         
-          65         756 JUMP_FORWARD           156 (to 1070)
-         
-          66     >>  758 LOAD_FAST                0 (e)
-                     760 LOAD_ATTR                2 (type)
-                     770 LOAD_CONST              18 ('accept')
-                     772 COMPARE_OP               2 (==)
-                     778 POP_JUMP_FORWARD_IF_FALSE     1 (to 782)
-         
-          67         780 JUMP_FORWARD           144 (to 1070)
-         
-          68     >>  782 LOAD_FAST                0 (e)
-                     784 LOAD_ATTR                2 (type)
-                     794 LOAD_CONST              19 ('reject')
-                     796 COMPARE_OP               2 (==)
-                     802 POP_JUMP_FORWARD_IF_FALSE     1 (to 806)
-         
-          69         804 JUMP_FORWARD           132 (to 1070)
-         
-          70     >>  806 LOAD_FAST                0 (e)
-                     808 LOAD_ATTR                2 (type)
-                     818 LOAD_CONST              20 ('conflict')
-                     820 COMPARE_OP               2 (==)
-                     826 POP_JUMP_FORWARD_IF_FALSE     1 (to 830)
-         
-          71         828 JUMP_FORWARD           120 (to 1070)
-         
-          72     >>  830 LOAD_FAST                0 (e)
-                     832 LOAD_ATTR                2 (type)
-                     842 LOAD_CONST              21 ('criteria')
-                     844 COMPARE_OP               2 (==)
-                     850 POP_JUMP_FORWARD_IF_FALSE   109 (to 1070)
-         
-          73         852 LOAD_GLOBAL             19 (NULL + print)
-                     864 LOAD_CONST              22 ('criteria search here we gooo')
-                     866 PRECALL                  1
-                     870 CALL                     1
-                     880 POP_TOP
-         
-          74         882 LOAD_GLOBAL              7 (NULL + query)
-                     894 LOAD_ATTR               14 (find_search_by_uid)
-                     904 LOAD_DEREF               5 (search_uid)
-                     906 PRECALL                  1
-                     910 CALL                     1
-                     920 STORE_FAST               4 (search)
-         
-          75         922 PUSH_NULL
-                     924 LOAD_FAST                1 (_insert_companies)
-         
-          76         926 LOAD_GLOBAL             13 (NULL + grata)
-                     938 LOAD_ATTR               18 (find_by_criteria)
-                     948 LOAD_FAST                4 (search)
-                     950 PRECALL                  1
-                     954 CALL                     1
-         
-          77         964 LOAD_GLOBAL              7 (NULL + query)
-                     976 LOAD_ATTR               16 (target)
-                     986 LOAD_DEREF               5 (search_uid)
-                     988 KW_NAMES                14
-                     990 PRECALL                  1
-                     994 CALL                     1
-                    1004 LOAD_CONST              15 ('domain')
-                    1006 BINARY_SUBSCR
-                    1016 LOAD_METHOD             17 (tolist)
-                    1038 PRECALL                  0
-                    1042 CALL                     0
-         
-          75        1052 KW_NAMES                16
-                    1054 PRECALL                  2
-                    1058 CALL                     2
-                    1068 POP_TOP
-         
-          81     >> 1070 LOAD_GLOBAL              7 (NULL + query)
-                    1082 LOAD_ATTR               19 (insert_checkpoint)
-                    1092 LOAD_GLOBAL             41 (NULL + Checkpoint)
-                    1104 LOAD_FAST                0 (e)
-                    1106 LOAD_ATTR               21 (id)
-                    1116 KW_NAMES                23
-                    1118 PRECALL                  1
-                    1122 CALL                     1
-                    1132 PRECALL                  1
-                    1136 CALL                     1
-                    1146 POP_TOP
-         
-          82        1148 LOAD_GLOBAL             19 (NULL + print)
-                    1160 LOAD_CONST              24 ('processed: ')
-                    1162 LOAD_FAST                0 (e)
-                    1164 FORMAT_VALUE             0
-                    1166 BUILD_STRING             2
-                    1168 PRECALL                  1
-                    1172 CALL                     1
-                    1182 POP_TOP
-                    1184 LOAD_CONST               0 (None)
-                    1186 RETURN_VALUE
+          46          48 LOAD_GLOBAL              3 (NULL + query)
+                      60 LOAD_ATTR                2 (find_event_by_id)
+                      70 LOAD_FAST                0 (event_id)
+                      72 PRECALL                  1
+                      76 CALL                     1
+                      86 STORE_FAST               2 (e)
+         
+          47          88 LOAD_FAST                2 (e)
+                      90 LOAD_ATTR                3 (search_uid)
+                     100 STORE_DEREF              6 (search_uid)
+         
+          48         102 LOAD_FAST                2 (e)
+                     104 LOAD_ATTR                4 (type)
+                     114 LOAD_CONST               6 ('create')
+                     116 COMPARE_OP               2 (==)
+                     122 POP_JUMP_FORWARD_IF_FALSE     2 (to 128)
+         
+          49         124 EXTENDED_ARG             1
+                     126 JUMP_FORWARD           492 (to 1112)
+         
+          50     >>  128 LOAD_FAST                2 (e)
+                     130 LOAD_ATTR                4 (type)
+                     140 LOAD_CONST               7 ('advance')
+                     142 COMPARE_OP               2 (==)
+                     148 POP_JUMP_FORWARD_IF_FALSE   200 (to 550)
+         
+          52         150 LOAD_GLOBAL              3 (NULL + query)
+                     162 LOAD_ATTR                5 (find_company_by_domain)
+                     172 LOAD_FAST                2 (e)
+                     174 LOAD_ATTR                6 (domain)
+                     184 PRECALL                  1
+                     188 CALL                     1
+                     198 STORE_FAST               3 (company)
+         
+          54         200 LOAD_GLOBAL             15 (NULL + grata)
+                     212 LOAD_ATTR                8 (enrich)
+                     222 LOAD_FAST                3 (company)
+                     224 LOAD_ATTR                6 (domain)
+                     234 PRECALL                  1
+                     238 CALL                     1
+                     248 STORE_FAST               4 (resp)
+         
+          55         250 LOAD_FAST                4 (resp)
+                     252 LOAD_METHOD              9 (get)
+                     274 LOAD_CONST               8 ('status')
+                     276 PRECALL                  1
+                     280 CALL                     1
+                     290 LOAD_CONST               9 (404)
+                     292 COMPARE_OP               2 (==)
+                     298 POP_JUMP_FORWARD_IF_FALSE    20 (to 340)
+         
+          56         300 LOAD_GLOBAL             21 (NULL + print)
+                     312 LOAD_FAST                3 (company)
+                     314 FORMAT_VALUE             0
+                     316 LOAD_CONST              10 (' not found')
+                     318 BUILD_STRING             2
+                     320 PRECALL                  1
+                     324 CALL                     1
+                     334 POP_TOP
+                     336 EXTENDED_ARG             1
+                     338 JUMP_FORWARD           386 (to 1112)
+         
+          58     >>  340 LOAD_GLOBAL             21 (NULL + print)
+                     352 LOAD_FAST                4 (resp)
+                     354 PRECALL                  1
+                     358 CALL                     1
+                     368 POP_TOP
+         
+          59         370 LOAD_FAST                4 (resp)
+                     372 LOAD_METHOD              9 (get)
+                     394 LOAD_CONST              11 ('name')
+                     396 PRECALL                  1
+                     400 CALL                     1
+                     410 LOAD_FAST                3 (company)
+                     412 STORE_ATTR              11 (name)
+         
+          60         422 LOAD_FAST                4 (resp)
+                     424 LOAD_METHOD              9 (get)
+                     446 LOAD_CONST              12 ('description')
+                     448 PRECALL                  1
+                     452 CALL                     1
+                     462 LOAD_FAST                3 (company)
+                     464 STORE_ATTR              12 (description)
+         
+          61         474 BUILD_MAP                0
+                     476 LOAD_FAST                3 (company)
+                     478 LOAD_ATTR               13 (meta)
+                     488 DICT_UPDATE              1
+                     490 LOAD_FAST                4 (resp)
+                     492 DICT_UPDATE              1
+                     494 LOAD_FAST                3 (company)
+                     496 STORE_ATTR              13 (meta)
+         
+          62         506 LOAD_GLOBAL              3 (NULL + query)
+                     518 LOAD_ATTR               14 (update_company)
+                     528 LOAD_FAST                3 (company)
+                     530 PRECALL                  1
+                     534 CALL                     1
+                     544 POP_TOP
+                     546 EXTENDED_ARG             1
+                     548 JUMP_FORWARD           281 (to 1112)
+         
+          64     >>  550 LOAD_FAST                2 (e)
+                     552 LOAD_ATTR                4 (type)
+                     562 LOAD_CONST              13 ('validate')
+                     564 COMPARE_OP               2 (==)
+                     570 POP_JUMP_FORWARD_IF_FALSE   102 (to 776)
+         
+          65         572 LOAD_GLOBAL              3 (NULL + query)
+                     584 LOAD_ATTR               15 (find_search_by_uid)
+                     594 LOAD_DEREF               6 (search_uid)
+                     596 PRECALL                  1
+                     600 CALL                     1
+                     610 STORE_FAST               5 (search)
+         
+          66         612 PUSH_NULL
+                     614 LOAD_FAST                1 (_insert_companies)
+         
+          67         616 LOAD_GLOBAL             15 (NULL + grata)
+                     628 LOAD_ATTR               16 (find_similar)
+                     638 LOAD_FAST                2 (e)
+                     640 LOAD_ATTR                6 (domain)
+                     650 LOAD_FAST                5 (search)
+                     652 KW_NAMES                14
+                     654 PRECALL                  2
+                     658 CALL                     2
+         
+          68         668 LOAD_GLOBAL              3 (NULL + query)
+                     680 LOAD_ATTR               17 (target)
+                     690 LOAD_DEREF               6 (search_uid)
+                     692 KW_NAMES                15
+                     694 PRECALL                  1
+                     698 CALL                     1
+                     708 LOAD_CONST              16 ('domain')
+                     710 BINARY_SUBSCR
+                     720 LOAD_METHOD             18 (tolist)
+                     742 PRECALL                  0
+                     746 CALL                     0
+         
+          66         756 KW_NAMES                17
+                     758 PRECALL                  2
+                     762 CALL                     2
+                     772 POP_TOP
+                     774 JUMP_FORWARD           168 (to 1112)
+         
+          70     >>  776 LOAD_FAST                2 (e)
+                     778 LOAD_ATTR                4 (type)
+                     788 LOAD_CONST              18 ('send')
+                     790 COMPARE_OP               2 (==)
+                     796 POP_JUMP_FORWARD_IF_FALSE     1 (to 800)
+         
+          71         798 JUMP_FORWARD           156 (to 1112)
+         
+          72     >>  800 LOAD_FAST                2 (e)
+                     802 LOAD_ATTR                4 (type)
+                     812 LOAD_CONST              19 ('accept')
+                     814 COMPARE_OP               2 (==)
+                     820 POP_JUMP_FORWARD_IF_FALSE     1 (to 824)
+         
+          73         822 JUMP_FORWARD           144 (to 1112)
+         
+          74     >>  824 LOAD_FAST                2 (e)
+                     826 LOAD_ATTR                4 (type)
+                     836 LOAD_CONST              20 ('reject')
+                     838 COMPARE_OP               2 (==)
+                     844 POP_JUMP_FORWARD_IF_FALSE     1 (to 848)
+         
+          75         846 JUMP_FORWARD           132 (to 1112)
+         
+          76     >>  848 LOAD_FAST                2 (e)
+                     850 LOAD_ATTR                4 (type)
+                     860 LOAD_CONST              21 ('conflict')
+                     862 COMPARE_OP               2 (==)
+                     868 POP_JUMP_FORWARD_IF_FALSE     1 (to 872)
+         
+          77         870 JUMP_FORWARD           120 (to 1112)
+         
+          78     >>  872 LOAD_FAST                2 (e)
+                     874 LOAD_ATTR                4 (type)
+                     884 LOAD_CONST              22 ('criteria')
+                     886 COMPARE_OP               2 (==)
+                     892 POP_JUMP_FORWARD_IF_FALSE   109 (to 1112)
+         
+          79         894 LOAD_GLOBAL             21 (NULL + print)
+                     906 LOAD_CONST              23 ('criteria search here we gooo')
+                     908 PRECALL                  1
+                     912 CALL                     1
+                     922 POP_TOP
+         
+          80         924 LOAD_GLOBAL              3 (NULL + query)
+                     936 LOAD_ATTR               15 (find_search_by_uid)
+                     946 LOAD_DEREF               6 (search_uid)
+                     948 PRECALL                  1
+                     952 CALL                     1
+                     962 STORE_FAST               5 (search)
+         
+          81         964 PUSH_NULL
+                     966 LOAD_FAST                1 (_insert_companies)
+         
+          82         968 LOAD_GLOBAL             15 (NULL + grata)
+                     980 LOAD_ATTR               19 (find_by_criteria)
+                     990 LOAD_FAST                5 (search)
+                     992 PRECALL                  1
+                     996 CALL                     1
+         
+          83        1006 LOAD_GLOBAL              3 (NULL + query)
+                    1018 LOAD_ATTR               17 (target)
+                    1028 LOAD_DEREF               6 (search_uid)
+                    1030 KW_NAMES                15
+                    1032 PRECALL                  1
+                    1036 CALL                     1
+                    1046 LOAD_CONST              16 ('domain')
+                    1048 BINARY_SUBSCR
+                    1058 LOAD_METHOD             18 (tolist)
+                    1080 PRECALL                  0
+                    1084 CALL                     0
+         
+          81        1094 KW_NAMES                17
+                    1096 PRECALL                  2
+                    1100 CALL                     2
+                    1110 POP_TOP
+         
+          87     >> 1112 LOAD_GLOBAL              3 (NULL + query)
+                    1124 LOAD_ATTR               20 (insert_checkpoint)
+                    1134 LOAD_GLOBAL             43 (NULL + Checkpoint)
+                    1146 LOAD_FAST                2 (e)
+                    1148 LOAD_ATTR               22 (id)
+                    1158 KW_NAMES                24
+                    1160 PRECALL                  1
+                    1164 CALL                     1
+                    1174 PRECALL                  1
+                    1178 CALL                     1
+                    1188 POP_TOP
+         
+          88        1190 LOAD_GLOBAL             21 (NULL + print)
+                    1202 LOAD_CONST              25 ('processed: ')
+                    1204 LOAD_FAST                2 (e)
+                    1206 FORMAT_VALUE             0
+                    1208 BUILD_STRING             2
+                    1210 PRECALL                  1
+                    1214 CALL                     1
+                    1224 POP_TOP
+                    1226 LOAD_CONST               4 (None)
+                    1228 RETURN_VALUE
          consts
-            None
+            '\n    May trigger additional targets adding to inbox, or something else\n    (e.g. a notification)\n    '
             'companies'
             'existing_domains'
             'return'
+            None
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 10
                flags     : 19
                code
                   0x950197007c0044005df07d027c02a00000000000000000000000000000
@@ -412,129 +433,129 @@
                   00a6010000ab01000000000000000001007405000000000000000000006a
                   050000000000000000740d0000000000000000000089037c02a000000000
                   00000000000000000000000000000000006401a6010000ab010000000000
                   000000640b640cac0da6040000ab040000000000000000a6010000ab0100
                   0000000000000001008cf164005300
                              0 COPY_FREE_VARS           1
                
-                14           2 RESUME                   0
+                18           2 RESUME                   0
                
-                16           4 LOAD_FAST                0 (companies)
+                20           4 LOAD_FAST                0 (companies)
                              6 GET_ITER
                        >>    8 FOR_ITER               240 (to 490)
                             10 STORE_FAST               2 (company)
                
-                17          12 LOAD_FAST                2 (company)
+                21          12 LOAD_FAST                2 (company)
                             14 LOAD_METHOD              0 (get)
                             36 LOAD_CONST               1 ('domain')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_JUMP_FORWARD_IF_NOT_NONE    20 (to 94)
                
-                18          54 LOAD_GLOBAL              3 (NULL + print)
+                22          54 LOAD_GLOBAL              3 (NULL + print)
                             66 LOAD_CONST               2 ('Missing domain: ')
                             68 LOAD_FAST                2 (company)
                             70 FORMAT_VALUE             0
                             72 LOAD_CONST               3 ('. Skipping')
                             74 BUILD_STRING             3
                             76 PRECALL                  1
                             80 CALL                     1
                             90 POP_TOP
                
-                19          92 JUMP_BACKWARD           43 (to 8)
+                23          92 JUMP_BACKWARD           43 (to 8)
                
-                21     >>   94 LOAD_FAST                2 (company)
+                25     >>   94 LOAD_FAST                2 (company)
                             96 LOAD_CONST               1 ('domain')
                             98 BINARY_SUBSCR
                            108 LOAD_FAST                1 (existing_domains)
                            110 CONTAINS_OP              0
                            112 POP_JUMP_FORWARD_IF_FALSE    26 (to 166)
                
-                22         114 LOAD_GLOBAL              3 (NULL + print)
+                26         114 LOAD_GLOBAL              3 (NULL + print)
                            126 LOAD_CONST               4 ('Skipping ')
                            128 LOAD_FAST                2 (company)
                            130 LOAD_CONST               1 ('domain')
                            132 BINARY_SUBSCR
                            142 FORMAT_VALUE             0
                            144 LOAD_CONST               5 (' as already a target')
                            146 BUILD_STRING             3
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                
-                23         164 JUMP_BACKWARD           79 (to 8)
+                27         164 JUMP_BACKWARD           79 (to 8)
                
-                24     >>  166 LOAD_GLOBAL              3 (NULL + print)
+                28     >>  166 LOAD_GLOBAL              3 (NULL + print)
                            178 LOAD_CONST               6 ('Adding ')
                            180 LOAD_FAST                2 (company)
                            182 LOAD_CONST               1 ('domain')
                            184 BINARY_SUBSCR
                            194 FORMAT_VALUE             0
                            196 LOAD_CONST               7 (' as target')
                            198 BUILD_STRING             3
                            200 PRECALL                  1
                            204 CALL                     1
                            214 POP_TOP
                
-                25         216 LOAD_GLOBAL              5 (NULL + query)
+                29         216 LOAD_GLOBAL              5 (NULL + query)
                            228 LOAD_ATTR                3 (insert_company)
                
-                26         238 LOAD_GLOBAL              9 (NULL + Company)
+                30         238 LOAD_GLOBAL              9 (NULL + Company)
                
-                27         250 LOAD_FAST                2 (company)
+                31         250 LOAD_FAST                2 (company)
                            252 LOAD_CONST               1 ('domain')
                            254 BINARY_SUBSCR
                
-                28         264 LOAD_FAST                2 (company)
+                32         264 LOAD_FAST                2 (company)
                            266 LOAD_METHOD              0 (get)
                            288 LOAD_CONST               8 ('name')
                            290 PRECALL                  1
                            294 CALL                     1
                
-                29         304 LOAD_FAST                2 (company)
+                33         304 LOAD_FAST                2 (company)
                            306 LOAD_METHOD              0 (get)
                            328 LOAD_CONST               9 ('description')
                            330 PRECALL                  1
                            334 CALL                     1
                
-                26         344 KW_NAMES                10
+                30         344 KW_NAMES                10
                            346 PRECALL                  3
                            350 CALL                     3
                
-                25         360 PRECALL                  1
+                29         360 PRECALL                  1
                            364 CALL                     1
                            374 POP_TOP
                
-                32         376 LOAD_GLOBAL              5 (NULL + query)
+                36         376 LOAD_GLOBAL              5 (NULL + query)
                            388 LOAD_ATTR                5 (insert_event)
                
-                33         398 LOAD_GLOBAL             13 (NULL + Event)
+                37         398 LOAD_GLOBAL             13 (NULL + Event)
                
-                34         410 LOAD_DEREF               3 (search_uid)
+                38         410 LOAD_DEREF               3 (search_uid)
                
-                35         412 LOAD_FAST                2 (company)
+                39         412 LOAD_FAST                2 (company)
                            414 LOAD_METHOD              0 (get)
                            436 LOAD_CONST               1 ('domain')
                            438 PRECALL                  1
                            442 CALL                     1
                
-                36         452 LOAD_CONST              11 ('grata')
+                40         452 LOAD_CONST              11 ('grata')
                
-                37         454 LOAD_CONST              12 ('create')
+                41         454 LOAD_CONST              12 ('create')
                
-                33         456 KW_NAMES                13
+                37         456 KW_NAMES                13
                            458 PRECALL                  4
                            462 CALL                     4
                
-                32         472 PRECALL                  1
+                36         472 PRECALL                  1
                            476 CALL                     1
                            486 POP_TOP
                            488 JUMP_BACKWARD          241 (to 8)
                
-                16     >>  490 LOAD_CONST               0 (None)
+                20     >>  490 LOAD_CONST               0 (None)
                            492 RETURN_VALUE
                consts
                   None
                   'domain'
                   'Missing domain: '
                   '. Skipping'
                   'Skipping '
@@ -549,15 +570,15 @@
                   ('search_uid', 'domain', 'actor_key', 'type')
                names      ('get', 'print', 'query', 'insert_company', 'Company', 'insert_event', 'Event')
                varnames   ('companies', 'existing_domains', 'company')
                freevars   ('search_uid',)
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
                name       '_insert_companies'
-               firstlineno 14
+               firstlineno 18
                lnotab
                   0x040208012a0126010202140132010201320116010c010e01280128fd10
                   ff100716010c0102012801020102fc10ff12f0
             'create'
             'advance'
             'status'
             404
@@ -573,136 +594,150 @@
             'accept'
             'reject'
             'conflict'
             'criteria'
             'criteria search here we gooo'
             ('event_id',)
             'processed: '
-         names      ('list', 'search_uid', 'type', 'query', 'find_company_by_domain', 'domain', 'grata', 'enrich', 'get', 'print', 'name', 'description', 'meta', 'update_company', 'find_search_by_uid', 'find_similar', 'target', 'tolist', 'find_by_criteria', 'insert_checkpoint', 'Checkpoint', 'id')
-         varnames   ('e', '_insert_companies', 'company', 'resp', 'search')
+         names      ('list', 'query', 'find_event_by_id', 'search_uid', 'type', 'find_company_by_domain', 'domain', 'grata', 'enrich', 'get', 'print', 'name', 'description', 'meta', 'update_company', 'find_search_by_uid', 'find_similar', 'target', 'tolist', 'find_by_criteria', 'insert_checkpoint', 'Checkpoint', 'id')
+         varnames   ('event_id', '_insert_companies', 'e', 'company', 'resp', 'search')
          freevars   ()
          cellvars   ('search_uid',)
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
          firstlineno 12
          lnotab
-            0x04022c1b0e0116010401160232023201320128021e01340134011e012c
-            02160128010401340158fe14041601020116010201160102011601020116
-            011e0128010401260158fe12064e01
+            0x04062c1c28010e0116010401160232023201320128021e013401340120
+            012c02160128010401340158fe1404160102011601020116010201160102
+            0116011e0128010401260158fe12064e01
       'search_uid'
       code
          argcount  : 1
-         nlocals   : 6
-         stacksize : 5
+         nlocals   : 5
+         stacksize : 7
          flags     : 3
          code
-            0x970067007d017401000000000000000000006a0100000000000000007c
-            00a6010000ab010000000000000000a00200000000000000000000000000
-            000000000000006401ac02a6010000ab01000000000000000044005d2c7d
-            027407000000000000000000007408000000000000000000007c02a60200
-            00ab0200000000000000007d027c01a00500000000000000000000000000
-            000000000000007c02a6010000ab01000000000000000001008c2d740100
-            0000000000000000006a060000000000000000a6000000ab000000000000
-            0000007d03740f000000000000000000007c03a6010000ab010000000000
-            000000010064037d047c0144005d257d057c056a0800000000000000007c
-            03640419000000000000000000760172147413000000000000000000007c
-            05a6010000ab01000000000000000001007c0464057a0d00007d048c267c
-            045300
-          85           0 RESUME                   0
-         
-          90           2 BUILD_LIST               0
-                       4 STORE_FAST               1 (events)
-         
-          92           6 LOAD_GLOBAL              1 (NULL + query)
-                      18 LOAD_ATTR                1 (event)
-                      28 LOAD_FAST                0 (search_uid)
-                      30 PRECALL                  1
-                      34 CALL                     1
-                      44 LOAD_METHOD              2 (to_dict)
-                      66 LOAD_CONST               1 ('records')
-                      68 KW_NAMES                 2
+            0x97007401000000000000000000006a0100000000000000007c00ac01a6
+            010000ab0100000000000000007d017401000000000000000000006a0200
+            000000000000007c00ac01a6010000ab0100000000000000007d02740700
+            0000000000000000007409000000000000000000007c0164021900000000
+            0000000000a0050000000000000000000000000000000000000000a60000
+            00ab000000000000000000a6010000ab0100000000000000007409000000
+            000000000000007c02640319000000000000000000a00500000000000000
+            00000000000000000000000000a6000000ab000000000000000000a60100
+            00ab0100000000000000007a0a0000a6010000ab0100000000000000007d
+            03740d000000000000000000006404ac05a6010000ab0100000000000000
+            0035007d047c04a007000000000000000000000000000000000000000074
+            10000000000000000000007c03a6020000ab020000000000000000010064
+            0664066406a6020000ab02000000000000000001006e0b23003100730477
+            0278035900770101005900010001007413000000000000000000007c03a6
+            010000ab0100000000000000005300
+          91           0 RESUME                   0
+         
+          96           2 LOAD_GLOBAL              1 (NULL + query)
+                      14 LOAD_ATTR                1 (event)
+                      24 LOAD_FAST                0 (search_uid)
+                      26 KW_NAMES                 1
+                      28 PRECALL                  1
+                      32 CALL                     1
+                      42 STORE_FAST               1 (events)
+         
+          97          44 LOAD_GLOBAL              1 (NULL + query)
+                      56 LOAD_ATTR                2 (checkpoint)
+                      66 LOAD_FAST                0 (search_uid)
+                      68 KW_NAMES                 1
                       70 PRECALL                  1
                       74 CALL                     1
-                      84 GET_ITER
-                 >>   86 FOR_ITER                44 (to 176)
-                      88 STORE_FAST               2 (event)
-         
-          93          90 LOAD_GLOBAL              7 (NULL + from_dict)
-                     102 LOAD_GLOBAL              8 (Event)
-                     114 LOAD_FAST                2 (event)
-                     116 PRECALL                  2
-                     120 CALL                     2
-                     130 STORE_FAST               2 (event)
-         
-          94         132 LOAD_FAST                1 (events)
-                     134 LOAD_METHOD              5 (append)
-                     156 LOAD_FAST                2 (event)
-                     158 PRECALL                  1
-                     162 CALL                     1
-                     172 POP_TOP
-                     174 JUMP_BACKWARD           45 (to 86)
-         
-          96     >>  176 LOAD_GLOBAL              1 (NULL + query)
-                     188 LOAD_ATTR                6 (checkpoint)
-                     198 PRECALL                  0
-                     202 CALL                     0
-                     212 STORE_FAST               3 (checkpoints)
-         
-          97         214 LOAD_GLOBAL             15 (NULL + print)
-                     226 LOAD_FAST                3 (checkpoints)
-                     228 PRECALL                  1
-                     232 CALL                     1
-                     242 POP_TOP
-         
-          98         244 LOAD_CONST               3 (0)
-                     246 STORE_FAST               4 (processed_count)
-         
-          99         248 LOAD_FAST                1 (events)
-                     250 GET_ITER
-                 >>  252 FOR_ITER                37 (to 328)
-                     254 STORE_FAST               5 (e)
-         
-         100         256 LOAD_FAST                5 (e)
-                     258 LOAD_ATTR                8 (id)
-                     268 LOAD_FAST                3 (checkpoints)
-                     270 LOAD_CONST               4 ('event_id')
-                     272 BINARY_SUBSCR
-                     282 CONTAINS_OP              1
-                     284 POP_JUMP_FORWARD_IF_FALSE    20 (to 326)
-         
-         101         286 LOAD_GLOBAL             19 (NULL + process_event)
-                     298 LOAD_FAST                5 (e)
-                     300 PRECALL                  1
-                     304 CALL                     1
-                     314 POP_TOP
-         
-         102         316 LOAD_FAST                4 (processed_count)
-                     318 LOAD_CONST               5 (1)
-                     320 BINARY_OP               13 (+=)
-                     324 STORE_FAST               4 (processed_count)
-                 >>  326 JUMP_BACKWARD           38 (to 252)
+                      84 STORE_FAST               2 (checkpoints)
          
-         104     >>  328 LOAD_FAST                4 (processed_count)
-                     330 RETURN_VALUE
+          99          86 LOAD_GLOBAL              7 (NULL + list)
+                      98 LOAD_GLOBAL              9 (NULL + set)
+                     110 LOAD_FAST                1 (events)
+                     112 LOAD_CONST               2 ('id')
+                     114 BINARY_SUBSCR
+                     124 LOAD_METHOD              5 (tolist)
+                     146 PRECALL                  0
+                     150 CALL                     0
+                     160 PRECALL                  1
+                     164 CALL                     1
+                     174 LOAD_GLOBAL              9 (NULL + set)
+                     186 LOAD_FAST                2 (checkpoints)
+                     188 LOAD_CONST               3 ('event_id')
+                     190 BINARY_SUBSCR
+                     200 LOAD_METHOD              5 (tolist)
+                     222 PRECALL                  0
+                     226 CALL                     0
+                     236 PRECALL                  1
+                     240 CALL                     1
+                     250 BINARY_OP               10 (-)
+                     254 PRECALL                  1
+                     258 CALL                     1
+                     268 STORE_FAST               3 (q)
+         
+         101         270 LOAD_GLOBAL             13 (NULL + ThreadPoolExecutor)
+                     282 LOAD_CONST               4 (4)
+                     284 KW_NAMES                 5
+                     286 PRECALL                  1
+                     290 CALL                     1
+                     300 BEFORE_WITH
+                     302 STORE_FAST               4 (executor)
+         
+         102         304 LOAD_FAST                4 (executor)
+                     306 LOAD_METHOD              7 (map)
+                     328 LOAD_GLOBAL             16 (process_event)
+                     340 LOAD_FAST                3 (q)
+                     342 PRECALL                  2
+                     346 CALL                     2
+                     356 POP_TOP
+         
+         101         358 LOAD_CONST               6 (None)
+                     360 LOAD_CONST               6 (None)
+                     362 LOAD_CONST               6 (None)
+                     364 PRECALL                  2
+                     368 CALL                     2
+                     378 POP_TOP
+                     380 JUMP_FORWARD            11 (to 404)
+                 >>  382 PUSH_EXC_INFO
+                     384 WITH_EXCEPT_START
+                     386 POP_JUMP_FORWARD_IF_TRUE     4 (to 396)
+                     388 RERAISE                  2
+                 >>  390 COPY                     3
+                     392 POP_EXCEPT
+                     394 RERAISE                  1
+                 >>  396 POP_TOP
+                     398 POP_EXCEPT
+                     400 POP_TOP
+                     402 POP_TOP
+         
+         104     >>  404 LOAD_GLOBAL             19 (NULL + len)
+                     416 LOAD_FAST                3 (q)
+                     418 PRECALL                  1
+                     422 CALL                     1
+                     432 RETURN_VALUE
+         ExceptionTable:
+           302 to 356 -> 382 [1] lasti
+           382 to 388 -> 390 [3] lasti
+           396 to 396 -> 390 [3] lasti
          consts
-            '\n    Process all events for a given search\n    Could tidy\n    '
-            'records'
-            ('orient',)
-            0
+            '\n    Process all events for a given search\n    '
+            ('search_uid',)
+            'id'
             'event_id'
-            1
-         names      ('query', 'event', 'to_dict', 'from_dict', 'Event', 'append', 'checkpoint', 'print', 'id', 'process_event')
-         varnames   ('search_uid', 'events', 'event', 'checkpoints', 'processed_count', 'e')
+            4
+            ('max_workers',)
+            None
+         names      ('query', 'event', 'checkpoint', 'list', 'set', 'tolist', 'ThreadPoolExecutor', 'map', 'process_event', 'len')
+         varnames   ('search_uid', 'events', 'checkpoints', 'q', 'executor')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_events'
-         firstlineno 85
-         lnotab 0x0205040254012a012c0226011e01040108011e011e010c02
-   names      ('pandas', 'pd', 'dacite', 'from_dict', 'dataclasses', 'dataclass', 'field', 'gandai.models', 'Event', 'Company', 'Checkpoint', 'gandai', 'query', 'gandai.sources', 'GrataWrapper', 'grata', 'process_event', 'int', 'process_events')
+         firstlineno 91
+         lnotab 0x02052a012a02b802220136ff2e03
+   names      ('pandas', 'pd', 'dacite', 'from_dict', 'dataclasses', 'dataclass', 'field', 'concurrent.futures', 'ThreadPoolExecutor', 'gandai.models', 'Event', 'Company', 'Checkpoint', 'gandai', 'query', 'gandai.sources', 'GrataWrapper', 'grata', 'int', 'process_event', 'process_events')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010c01100314010c020c031049
+   lnotab 0x00ff020108010c0110010c0214010c020c03104f
```

### Comparing `gandai-1.1.7/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,31 +1,32 @@
 magic:    0xa70d0d0a
-moddate:  0x47386064 (Sun May 14 01:24:23 2023 UTC)
-files sz: 8697
+moddate:  0x3b766164 (Mon May 15 00:00:59 2023 UTC)
+files sz: 9337
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a02640064026c036d045a0401
       00640064036c056d065a060100640064046c076d085a086d095a096d0a5a
       0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064016c0e5a0e640064056c0f6d
       105a100100640064066c116d125a12010002006512a6000000ab00000000
       00000000000100640064076c136d145a14010002006514a6000000ab0000
       000000000000005a15640865096602640984045a16640a6508640b650866
       04640c84045a17640d650b640b650b6604640e84045a18640f650c640b65
       0c6604641084045a196411650d640b650d6604641284045a1a641384005a
-      1b64216414651c6415651d6604641684055a1e6414651c640b65026a1f00
+      1b64236414651c6415651d6604641684055a1e6414651c640b65026a1f00
       000000000000006604641784045a206414651c640b65026a1f0000000000
       0000006604641884045a21640b65026a1f00000000000000006602641984
-      045a22640b65026a1f00000000000000006602641a84045a236414651c64
-      0b65026a1f00000000000000006604641b84045a246414651c640b650c66
-      04641c84045a25641d651d640b65096604641e84045a2664086509640b64
-      016604641f84045a27640f650c640b64016604642084045a2864015300
+      045a226414651c640b65026a1f00000000000000006604641a84045a2364
+      14651c640b65026a1f00000000000000006604641b84045a246414651c64
+      0b650c6604641c84045a25641d651d640b65096604641e84045a26641f65
+      1c640b65086604642084045a2764086509640b64016604642184045a2864
+      0f650c640b64016604642284045a2964015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (json)
                  8 STORE_NAME               0 (json)
    
@@ -80,173 +81,184 @@
     18          94 LOAD_CONST               0 (0)
                 96 LOAD_CONST               6 (('load_dotenv',))
                 98 IMPORT_NAME             17 (dotenv)
                100 IMPORT_FROM             18 (load_dotenv)
                102 STORE_NAME              18 (load_dotenv)
                104 POP_TOP
    
-    19         106 PUSH_NULL
+    20         106 PUSH_NULL
                108 LOAD_NAME               18 (load_dotenv)
                110 PRECALL                  0
                114 CALL                     0
                124 POP_TOP
    
-    21         126 LOAD_CONST               0 (0)
+    22         126 LOAD_CONST               0 (0)
                128 LOAD_CONST               7 (('connect_with_connector',))
                130 IMPORT_NAME             19 (gandai.db)
                132 IMPORT_FROM             20 (connect_with_connector)
                134 STORE_NAME              20 (connect_with_connector)
                136 POP_TOP
    
-    23         138 PUSH_NULL
+    24         138 PUSH_NULL
                140 LOAD_NAME               20 (connect_with_connector)
                142 PRECALL                  0
                146 CALL                     0
                156 STORE_NAME              21 (db)
    
-    29         158 LOAD_CONST               8 ('company')
+    30         158 LOAD_CONST               8 ('company')
                160 LOAD_NAME                9 (Company)
                162 BUILD_TUPLE              2
-               164 LOAD_CONST               9 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 29>)
+               164 LOAD_CONST               9 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 30>)
                166 MAKE_FUNCTION            4 (annotations)
                168 STORE_NAME              22 (insert_company)
    
-    43         170 LOAD_CONST              10 ('event')
+    44         170 LOAD_CONST              10 ('event')
                172 LOAD_NAME                8 (Event)
                174 LOAD_CONST              11 ('return')
                176 LOAD_NAME                8 (Event)
                178 BUILD_TUPLE              4
-               180 LOAD_CONST              12 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 43>)
+               180 LOAD_CONST              12 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 44>)
                182 MAKE_FUNCTION            4 (annotations)
                184 STORE_NAME              23 (insert_event)
    
-    64         186 LOAD_CONST              13 ('actor')
+    65         186 LOAD_CONST              13 ('actor')
                188 LOAD_NAME               11 (Actor)
                190 LOAD_CONST              11 ('return')
                192 LOAD_NAME               11 (Actor)
                194 BUILD_TUPLE              4
-               196 LOAD_CONST              14 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 64>)
+               196 LOAD_CONST              14 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 65>)
                198 MAKE_FUNCTION            4 (annotations)
                200 STORE_NAME              24 (insert_actor)
    
-    79         202 LOAD_CONST              15 ('search')
+    80         202 LOAD_CONST              15 ('search')
                204 LOAD_NAME               12 (Search)
                206 LOAD_CONST              11 ('return')
                208 LOAD_NAME               12 (Search)
                210 BUILD_TUPLE              4
-               212 LOAD_CONST              16 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 79>)
+               212 LOAD_CONST              16 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 80>)
                214 MAKE_FUNCTION            4 (annotations)
                216 STORE_NAME              25 (insert_search)
    
-    98         218 LOAD_CONST              17 ('checkpoint')
+    99         218 LOAD_CONST              17 ('checkpoint')
                220 LOAD_NAME               13 (Checkpoint)
                222 LOAD_CONST              11 ('return')
                224 LOAD_NAME               13 (Checkpoint)
                226 BUILD_TUPLE              4
-               228 LOAD_CONST              18 (<code object insert_checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 98>)
+               228 LOAD_CONST              18 (<code object insert_checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 99>)
                230 MAKE_FUNCTION            4 (annotations)
                232 STORE_NAME              26 (insert_checkpoint)
    
-   114         234 LOAD_CONST              19 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 114>)
+   115         234 LOAD_CONST              19 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 115>)
                236 MAKE_FUNCTION            0
                238 STORE_NAME              27 (search)
    
-   121         240 LOAD_CONST              33 ((None,))
+   124         240 LOAD_CONST              35 ((None,))
                242 LOAD_CONST              20 ('search_uid')
                244 LOAD_NAME               28 (int)
                246 LOAD_CONST              21 ('last_event_type')
                248 LOAD_NAME               29 (str)
                250 BUILD_TUPLE              4
-               252 LOAD_CONST              22 (<code object target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 121>)
+               252 LOAD_CONST              22 (<code object target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 124>)
                254 MAKE_FUNCTION            5 (defaults, annotations)
                256 STORE_NAME              30 (target)
    
-   153         258 LOAD_CONST              20 ('search_uid')
+   155         258 LOAD_CONST              20 ('search_uid')
                260 LOAD_NAME               28 (int)
                262 LOAD_CONST              11 ('return')
                264 LOAD_NAME                2 (pd)
                266 LOAD_ATTR               31 (DataFrame)
                276 BUILD_TUPLE              4
-               278 LOAD_CONST              23 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 153>)
+               278 LOAD_CONST              23 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 155>)
                280 MAKE_FUNCTION            4 (annotations)
                282 STORE_NAME              32 (target_count)
    
-   169         284 LOAD_CONST              20 ('search_uid')
+   171         284 LOAD_CONST              20 ('search_uid')
                286 LOAD_NAME               28 (int)
                288 LOAD_CONST              11 ('return')
                290 LOAD_NAME                2 (pd)
                292 LOAD_ATTR               31 (DataFrame)
                302 BUILD_TUPLE              4
-               304 LOAD_CONST              24 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 169>)
+               304 LOAD_CONST              24 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 171>)
                306 MAKE_FUNCTION            4 (annotations)
                308 STORE_NAME              33 (event)
    
-   180         310 LOAD_CONST              11 ('return')
+   183         310 LOAD_CONST              11 ('return')
                312 LOAD_NAME                2 (pd)
                314 LOAD_ATTR               31 (DataFrame)
                324 BUILD_TUPLE              2
-               326 LOAD_CONST              25 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 180>)
+               326 LOAD_CONST              25 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 183>)
                328 MAKE_FUNCTION            4 (annotations)
                330 STORE_NAME              34 (company)
    
-   190         332 LOAD_CONST              11 ('return')
-               334 LOAD_NAME                2 (pd)
-               336 LOAD_ATTR               31 (DataFrame)
-               346 BUILD_TUPLE              2
-               348 LOAD_CONST              26 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 190>)
-               350 MAKE_FUNCTION            4 (annotations)
-               352 STORE_NAME              35 (checkpoint)
-   
-   201         354 LOAD_CONST              20 ('search_uid')
-               356 LOAD_NAME               28 (int)
-               358 LOAD_CONST              11 ('return')
-               360 LOAD_NAME                2 (pd)
-               362 LOAD_ATTR               31 (DataFrame)
-               372 BUILD_TUPLE              4
-               374 LOAD_CONST              27 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 201>)
-               376 MAKE_FUNCTION            4 (annotations)
-               378 STORE_NAME              36 (comment_by_domain)
-   
-   222         380 LOAD_CONST              20 ('search_uid')
-               382 LOAD_NAME               28 (int)
-               384 LOAD_CONST              11 ('return')
-               386 LOAD_NAME               12 (Search)
-               388 BUILD_TUPLE              4
-               390 LOAD_CONST              28 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 222>)
-               392 MAKE_FUNCTION            4 (annotations)
-               394 STORE_NAME              37 (find_search_by_uid)
-   
-   238         396 LOAD_CONST              29 ('domain')
-               398 LOAD_NAME               29 (str)
-               400 LOAD_CONST              11 ('return')
-               402 LOAD_NAME                9 (Company)
-               404 BUILD_TUPLE              4
-               406 LOAD_CONST              30 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 238>)
-               408 MAKE_FUNCTION            4 (annotations)
-               410 STORE_NAME              38 (find_company_by_domain)
-   
-   257         412 LOAD_CONST               8 ('company')
-               414 LOAD_NAME                9 (Company)
-               416 LOAD_CONST              11 ('return')
-               418 LOAD_CONST               1 (None)
-               420 BUILD_TUPLE              4
-               422 LOAD_CONST              31 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 257>)
-               424 MAKE_FUNCTION            4 (annotations)
-               426 STORE_NAME              39 (update_company)
-   
-   281         428 LOAD_CONST              15 ('search')
-               430 LOAD_NAME               12 (Search)
-               432 LOAD_CONST              11 ('return')
-               434 LOAD_CONST               1 (None)
-               436 BUILD_TUPLE              4
-               438 LOAD_CONST              32 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 281>)
-               440 MAKE_FUNCTION            4 (annotations)
-               442 STORE_NAME              40 (update_search)
-               444 LOAD_CONST               1 (None)
-               446 RETURN_VALUE
+   194         332 LOAD_CONST              20 ('search_uid')
+               334 LOAD_NAME               28 (int)
+               336 LOAD_CONST              11 ('return')
+               338 LOAD_NAME                2 (pd)
+               340 LOAD_ATTR               31 (DataFrame)
+               350 BUILD_TUPLE              4
+               352 LOAD_CONST              26 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 194>)
+               354 MAKE_FUNCTION            4 (annotations)
+               356 STORE_NAME              35 (checkpoint)
+   
+   207         358 LOAD_CONST              20 ('search_uid')
+               360 LOAD_NAME               28 (int)
+               362 LOAD_CONST              11 ('return')
+               364 LOAD_NAME                2 (pd)
+               366 LOAD_ATTR               31 (DataFrame)
+               376 BUILD_TUPLE              4
+               378 LOAD_CONST              27 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 207>)
+               380 MAKE_FUNCTION            4 (annotations)
+               382 STORE_NAME              36 (comment_by_domain)
+   
+   228         384 LOAD_CONST              20 ('search_uid')
+               386 LOAD_NAME               28 (int)
+               388 LOAD_CONST              11 ('return')
+               390 LOAD_NAME               12 (Search)
+               392 BUILD_TUPLE              4
+               394 LOAD_CONST              28 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 228>)
+               396 MAKE_FUNCTION            4 (annotations)
+               398 STORE_NAME              37 (find_search_by_uid)
+   
+   244         400 LOAD_CONST              29 ('domain')
+               402 LOAD_NAME               29 (str)
+               404 LOAD_CONST              11 ('return')
+               406 LOAD_NAME                9 (Company)
+               408 BUILD_TUPLE              4
+               410 LOAD_CONST              30 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 244>)
+               412 MAKE_FUNCTION            4 (annotations)
+               414 STORE_NAME              38 (find_company_by_domain)
+   
+   260         416 LOAD_CONST              31 ('event_id')
+               418 LOAD_NAME               28 (int)
+               420 LOAD_CONST              11 ('return')
+               422 LOAD_NAME                8 (Event)
+               424 BUILD_TUPLE              4
+               426 LOAD_CONST              32 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 260>)
+               428 MAKE_FUNCTION            4 (annotations)
+               430 STORE_NAME              39 (find_event_by_id)
+   
+   278         432 LOAD_CONST               8 ('company')
+               434 LOAD_NAME                9 (Company)
+               436 LOAD_CONST              11 ('return')
+               438 LOAD_CONST               1 (None)
+               440 BUILD_TUPLE              4
+               442 LOAD_CONST              33 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 278>)
+               444 MAKE_FUNCTION            4 (annotations)
+               446 STORE_NAME              40 (update_company)
+   
+   302         448 LOAD_CONST              15 ('search')
+               450 LOAD_NAME               12 (Search)
+               452 LOAD_CONST              11 ('return')
+               454 LOAD_CONST               1 (None)
+               456 BUILD_TUPLE              4
+               458 LOAD_CONST              34 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 302>)
+               460 MAKE_FUNCTION            4 (annotations)
+               462 STORE_NAME              41 (update_search)
+               464 LOAD_CONST               1 (None)
+               466 RETURN_VALUE
    consts
       0
       None
       ('asdict',)
       ('from_dict',)
       ('Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint')
       ('Connector',)
@@ -264,50 +276,50 @@
             000000000000006a0300000000000000006401a6010000ab010000000000
             0000007d027c01a00400000000000000000000000000000000000000007c
             02740b000000000000000000007c00a6010000ab010000000000000000a6
             020000ab02000000000000000001007c01a0060000000000000000000000
             000000000000000000a6000000ab00000000000000000001006400640064
             00a6020000ab02000000000000000001006e0b2300310073047702780359
             00770101005900010001007c005300
-          29           0 RESUME                   0
+          30           0 RESUME                   0
          
-          30           2 LOAD_GLOBAL              0 (db)
+          31           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          31          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+          32          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-          32          76 LOAD_CONST               1 ('\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            ')
+          33          76 LOAD_CONST               1 ('\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            ')
          
-          31          78 PRECALL                  1
+          32          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-          38          94 LOAD_FAST                1 (con)
+          39          94 LOAD_FAST                1 (con)
                       96 LOAD_METHOD              4 (execute)
                      118 LOAD_FAST                2 (statement)
                      120 LOAD_GLOBAL             11 (NULL + asdict)
                      132 LOAD_FAST                0 (company)
                      134 PRECALL                  1
                      138 CALL                     1
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
          
-          39         164 LOAD_FAST                1 (con)
+          40         164 LOAD_FAST                1 (con)
                      166 LOAD_METHOD              6 (commit)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 POP_TOP
          
-          30         204 LOAD_CONST               0 (None)
+          31         204 LOAD_CONST               0 (None)
                      206 LOAD_CONST               0 (None)
                      208 LOAD_CONST               0 (None)
                      210 PRECALL                  2
                      214 CALL                     2
                      224 POP_TOP
                      226 JUMP_FORWARD            11 (to 250)
                  >>  228 PUSH_EXC_INFO
@@ -318,30 +330,30 @@
                      238 POP_EXCEPT
                      240 RERAISE                  1
                  >>  242 POP_TOP
                      244 POP_EXCEPT
                      246 POP_TOP
                      248 POP_TOP
          
-          40     >>  250 LOAD_FAST                0 (company)
+          41     >>  250 LOAD_FAST                0 (company)
                      252 RETURN_VALUE
          ExceptionTable:
            52 to 202 -> 228 [1] lasti
            228 to 234 -> 236 [3] lasti
            242 to 242 -> 236 [3] lasti
          consts
             None
             '\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            '
          names      ('db', 'connect', 'sqlalchemy', 'text', 'execute', 'asdict', 'commit')
          varnames   ('company', 'con', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_company'
-         firstlineno 29
+         firstlineno 30
          lnotab 0x02013401160102ff1007460128f72e0a
       'event'
       'return'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 6
@@ -359,91 +371,91 @@
             087c056403190000000000000000006e0164007c005f0900000000000000
             007c01a00700000000000000000000000000000000000000007405000000
             000000000000006a0300000000000000006404a6010000ab010000000000
             000000a6010000ab01000000000000000001007c01a00a00000000000000
             00000000000000000000000000a6000000ab000000000000000000010064
             0064006400a6020000ab02000000000000000001006e0b23003100730477
             0278035900770101005900010001007c005300
-          43           0 RESUME                   0
+          44           0 RESUME                   0
          
-          44           2 LOAD_GLOBAL              0 (db)
+          45           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          45          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+          46          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-          46          76 LOAD_CONST               1 ('\n                INSERT INTO event (search_uid, domain, actor_key, type, data) \n                VALUES(:search_uid, :domain, :actor_key, :type, :data)\n                ON CONFLICT DO NOTHING\n                RETURNING id\n            ')
+          47          76 LOAD_CONST               1 ('\n                INSERT INTO event (search_uid, domain, actor_key, type, data) \n                VALUES(:search_uid, :domain, :actor_key, :type, :data)\n                ON CONFLICT DO NOTHING\n                RETURNING id\n            ')
          
-          45          78 PRECALL                  1
+          46          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-          53          94 LOAD_GLOBAL              9 (NULL + asdict)
+          54          94 LOAD_GLOBAL              9 (NULL + asdict)
                      106 LOAD_FAST                0 (event)
                      108 PRECALL                  1
                      112 CALL                     1
                      122 STORE_FAST               3 (obj)
          
-          54         124 LOAD_GLOBAL             11 (NULL + json)
+          55         124 LOAD_GLOBAL             11 (NULL + json)
                      136 LOAD_ATTR                6 (dumps)
                      146 LOAD_FAST                3 (obj)
                      148 LOAD_CONST               2 ('data')
                      150 BINARY_SUBSCR
                      160 PRECALL                  1
                      164 CALL                     1
                      174 LOAD_FAST                3 (obj)
                      176 LOAD_CONST               2 ('data')
                      178 STORE_SUBSCR
          
-          55         182 LOAD_FAST                1 (con)
+          56         182 LOAD_FAST                1 (con)
                      184 LOAD_METHOD              7 (execute)
                      206 LOAD_FAST                2 (statement)
                      208 LOAD_FAST                3 (obj)
                      210 PRECALL                  2
                      214 CALL                     2
                      224 STORE_FAST               4 (result)
          
-          57         226 LOAD_FAST                4 (result)
+          58         226 LOAD_FAST                4 (result)
                      228 LOAD_METHOD              8 (first)
                      250 PRECALL                  0
                      254 CALL                     0
                      264 STORE_FAST               5 (_id)
          
-          58         266 LOAD_FAST                5 (_id)
+          59         266 LOAD_FAST                5 (_id)
                      268 POP_JUMP_FORWARD_IF_FALSE     8 (to 286)
                      270 LOAD_FAST                5 (_id)
                      272 LOAD_CONST               3 (0)
                      274 BINARY_SUBSCR
                      284 JUMP_FORWARD             1 (to 288)
                  >>  286 LOAD_CONST               0 (None)
                  >>  288 LOAD_FAST                0 (event)
                      290 STORE_ATTR               9 (id)
          
-          59         300 LOAD_FAST                1 (con)
+          60         300 LOAD_FAST                1 (con)
                      302 LOAD_METHOD              7 (execute)
                      324 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                      336 LOAD_ATTR                3 (text)
                      346 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW target')
                      348 PRECALL                  1
                      352 CALL                     1
                      362 PRECALL                  1
                      366 CALL                     1
                      376 POP_TOP
          
-          60         378 LOAD_FAST                1 (con)
+          61         378 LOAD_FAST                1 (con)
                      380 LOAD_METHOD             10 (commit)
                      402 PRECALL                  0
                      406 CALL                     0
                      416 POP_TOP
          
-          44         418 LOAD_CONST               0 (None)
+          45         418 LOAD_CONST               0 (None)
                      420 LOAD_CONST               0 (None)
                      422 LOAD_CONST               0 (None)
                      424 PRECALL                  2
                      428 CALL                     2
                      438 POP_TOP
                      440 JUMP_FORWARD            11 (to 464)
                  >>  442 PUSH_EXC_INFO
@@ -454,15 +466,15 @@
                      452 POP_EXCEPT
                      454 RERAISE                  1
                  >>  456 POP_TOP
                      458 POP_EXCEPT
                      460 POP_TOP
                      462 POP_TOP
          
-          61     >>  464 LOAD_FAST                0 (event)
+          62     >>  464 LOAD_FAST                0 (event)
                      466 RETURN_VALUE
          ExceptionTable:
            52 to 416 -> 442 [1] lasti
            442 to 448 -> 450 [3] lasti
            456 to 456 -> 450 [3] lasti
          consts
             None
@@ -472,15 +484,15 @@
             'REFRESH MATERIALIZED VIEW target'
          names      ('db', 'connect', 'sqlalchemy', 'text', 'asdict', 'json', 'dumps', 'execute', 'first', 'id', 'commit')
          varnames   ('event', 'con', 'statement', 'obj', 'result', '_id')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_event'
-         firstlineno 43
+         firstlineno 44
          lnotab 0x02013401160102ff10081e013a012c02280122014e0128f02e11
       'actor'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
@@ -490,53 +502,53 @@
             000000000000006a0300000000000000006401a6010000ab010000000000
             0000007d027409000000000000000000007c00a6010000ab010000000000
             0000007d037c01a00500000000000000000000000000000000000000007c
             027c03a6020000ab02000000000000000001007c01a00600000000000000
             00000000000000000000000000a6000000ab000000000000000000010064
             0064006400a6020000ab02000000000000000001006e0b23003100730477
             0278035900770101005900010001007c005300
-          64           0 RESUME                   0
+          65           0 RESUME                   0
          
-          65           2 LOAD_GLOBAL              0 (db)
+          66           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          66          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+          67          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-          67          76 LOAD_CONST               1 ('\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            ')
+          68          76 LOAD_CONST               1 ('\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            ')
          
-          66          78 PRECALL                  1
+          67          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-          73          94 LOAD_GLOBAL              9 (NULL + asdict)
+          74          94 LOAD_GLOBAL              9 (NULL + asdict)
                      106 LOAD_FAST                0 (actor)
                      108 PRECALL                  1
                      112 CALL                     1
                      122 STORE_FAST               3 (obj)
          
-          74         124 LOAD_FAST                1 (con)
+          75         124 LOAD_FAST                1 (con)
                      126 LOAD_METHOD              5 (execute)
                      148 LOAD_FAST                2 (statement)
                      150 LOAD_FAST                3 (obj)
                      152 PRECALL                  2
                      156 CALL                     2
                      166 POP_TOP
          
-          75         168 LOAD_FAST                1 (con)
+          76         168 LOAD_FAST                1 (con)
                      170 LOAD_METHOD              6 (commit)
                      192 PRECALL                  0
                      196 CALL                     0
                      206 POP_TOP
          
-          65         208 LOAD_CONST               0 (None)
+          66         208 LOAD_CONST               0 (None)
                      210 LOAD_CONST               0 (None)
                      212 LOAD_CONST               0 (None)
                      214 PRECALL                  2
                      218 CALL                     2
                      228 POP_TOP
                      230 JUMP_FORWARD            11 (to 254)
                  >>  232 PUSH_EXC_INFO
@@ -547,30 +559,30 @@
                      242 POP_EXCEPT
                      244 RERAISE                  1
                  >>  246 POP_TOP
                      248 POP_EXCEPT
                      250 POP_TOP
                      252 POP_TOP
          
-          76     >>  254 LOAD_FAST                0 (actor)
+          77     >>  254 LOAD_FAST                0 (actor)
                      256 RETURN_VALUE
          ExceptionTable:
            52 to 206 -> 232 [1] lasti
            232 to 238 -> 240 [3] lasti
            246 to 246 -> 240 [3] lasti
          consts
             None
             '\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            '
          names      ('db', 'connect', 'sqlalchemy', 'text', 'asdict', 'execute', 'commit')
          varnames   ('actor', 'con', 'statement', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_actor'
-         firstlineno 64
+         firstlineno 65
          lnotab 0x02013401160102ff10071e012c0128f62e0b
       'search'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
@@ -588,97 +600,97 @@
             0b000000000000000000006a0600000000000000007c0364051900000000
             0000000000a6010000ab0100000000000000007c0364053c0000007c01a0
             0700000000000000000000000000000000000000007c027c03a6020000ab
             02000000000000000001007c01a008000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006e0b230031007304770278035900770101
             005900010001007c005300
-          79           0 RESUME                   0
+          80           0 RESUME                   0
          
-          80           2 LOAD_GLOBAL              0 (db)
+          81           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          81          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+          82          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-          82          76 LOAD_CONST               1 ('\n                INSERT INTO search (uid, client_domain, label, meta, inclusion, exclusion, sort) \n                VALUES(:uid, :client_domain, :label, :meta, :inclusion, :exclusion, :sort)\n                ON CONFLICT DO NOTHING\n            ')
+          83          76 LOAD_CONST               1 ('\n                INSERT INTO search (uid, client_domain, label, meta, inclusion, exclusion, sort) \n                VALUES(:uid, :client_domain, :label, :meta, :inclusion, :exclusion, :sort)\n                ON CONFLICT DO NOTHING\n            ')
          
-          81          78 PRECALL                  1
+          82          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-          88          94 LOAD_GLOBAL              9 (NULL + asdict)
+          89          94 LOAD_GLOBAL              9 (NULL + asdict)
                      106 LOAD_FAST                0 (search)
                      108 PRECALL                  1
                      112 CALL                     1
                      122 STORE_FAST               3 (obj)
          
-          89         124 LOAD_GLOBAL             11 (NULL + json)
+          90         124 LOAD_GLOBAL             11 (NULL + json)
                      136 LOAD_ATTR                6 (dumps)
                      146 LOAD_FAST                3 (obj)
                      148 LOAD_CONST               2 ('meta')
                      150 BINARY_SUBSCR
                      160 PRECALL                  1
                      164 CALL                     1
                      174 LOAD_FAST                3 (obj)
                      176 LOAD_CONST               2 ('meta')
                      178 STORE_SUBSCR
          
-          90         182 LOAD_GLOBAL             11 (NULL + json)
+          91         182 LOAD_GLOBAL             11 (NULL + json)
                      194 LOAD_ATTR                6 (dumps)
                      204 LOAD_FAST                3 (obj)
                      206 LOAD_CONST               3 ('inclusion')
                      208 BINARY_SUBSCR
                      218 PRECALL                  1
                      222 CALL                     1
                      232 LOAD_FAST                3 (obj)
                      234 LOAD_CONST               3 ('inclusion')
                      236 STORE_SUBSCR
          
-          91         240 LOAD_GLOBAL             11 (NULL + json)
+          92         240 LOAD_GLOBAL             11 (NULL + json)
                      252 LOAD_ATTR                6 (dumps)
                      262 LOAD_FAST                3 (obj)
                      264 LOAD_CONST               4 ('exclusion')
                      266 BINARY_SUBSCR
                      276 PRECALL                  1
                      280 CALL                     1
                      290 LOAD_FAST                3 (obj)
                      292 LOAD_CONST               4 ('exclusion')
                      294 STORE_SUBSCR
          
-          92         298 LOAD_GLOBAL             11 (NULL + json)
+          93         298 LOAD_GLOBAL             11 (NULL + json)
                      310 LOAD_ATTR                6 (dumps)
                      320 LOAD_FAST                3 (obj)
                      322 LOAD_CONST               5 ('sort')
                      324 BINARY_SUBSCR
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_FAST                3 (obj)
                      350 LOAD_CONST               5 ('sort')
                      352 STORE_SUBSCR
          
-          93         356 LOAD_FAST                1 (con)
+          94         356 LOAD_FAST                1 (con)
                      358 LOAD_METHOD              7 (execute)
                      380 LOAD_FAST                2 (statement)
                      382 LOAD_FAST                3 (obj)
                      384 PRECALL                  2
                      388 CALL                     2
                      398 POP_TOP
          
-          94         400 LOAD_FAST                1 (con)
+          95         400 LOAD_FAST                1 (con)
                      402 LOAD_METHOD              8 (commit)
                      424 PRECALL                  0
                      428 CALL                     0
                      438 POP_TOP
          
-          80         440 LOAD_CONST               0 (None)
+          81         440 LOAD_CONST               0 (None)
                      442 LOAD_CONST               0 (None)
                      444 LOAD_CONST               0 (None)
                      446 PRECALL                  2
                      450 CALL                     2
                      460 POP_TOP
                      462 JUMP_FORWARD            11 (to 486)
                  >>  464 PUSH_EXC_INFO
@@ -689,15 +701,15 @@
                      474 POP_EXCEPT
                      476 RERAISE                  1
                  >>  478 POP_TOP
                      480 POP_EXCEPT
                      482 POP_TOP
                      484 POP_TOP
          
-          95     >>  486 LOAD_FAST                0 (search)
+          96     >>  486 LOAD_FAST                0 (search)
                      488 RETURN_VALUE
          ExceptionTable:
            52 to 438 -> 464 [1] lasti
            464 to 470 -> 472 [3] lasti
            478 to 478 -> 472 [3] lasti
          consts
             None
@@ -708,15 +720,15 @@
             'sort'
          names      ('db', 'connect', 'sqlalchemy', 'text', 'asdict', 'json', 'dumps', 'execute', 'commit')
          varnames   ('search', 'con', 'statement', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_search'
-         firstlineno 79
+         firstlineno 80
          lnotab 0x02013401160102ff10071e013a013a013a013a012c0128f22e0f
       'checkpoint'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
@@ -726,50 +738,50 @@
             000000000000006a0300000000000000006401a6010000ab010000000000
             0000007d027c01a00400000000000000000000000000000000000000007c
             02740b000000000000000000007c00a6010000ab010000000000000000a6
             020000ab02000000000000000001007c01a0060000000000000000000000
             000000000000000000a6000000ab00000000000000000001006400640064
             00a6020000ab02000000000000000001006e0b2300310073047702780359
             00770101005900010001007c005300
-          98           0 RESUME                   0
+          99           0 RESUME                   0
          
-          99           2 LOAD_GLOBAL              0 (db)
+         100           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-         100          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+         101          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
                       66 LOAD_ATTR                3 (text)
          
-         101          76 LOAD_CONST               1 ('\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            ')
+         102          76 LOAD_CONST               1 ('\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            ')
          
-         100          78 PRECALL                  1
+         101          78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               2 (statement)
          
-         106          94 LOAD_FAST                1 (con)
+         107          94 LOAD_FAST                1 (con)
                       96 LOAD_METHOD              4 (execute)
                      118 LOAD_FAST                2 (statement)
                      120 LOAD_GLOBAL             11 (NULL + asdict)
                      132 LOAD_FAST                0 (checkpoint)
                      134 PRECALL                  1
                      138 CALL                     1
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
          
-         107         164 LOAD_FAST                1 (con)
+         108         164 LOAD_FAST                1 (con)
                      166 LOAD_METHOD              6 (commit)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 POP_TOP
          
-          99         204 LOAD_CONST               0 (None)
+         100         204 LOAD_CONST               0 (None)
                      206 LOAD_CONST               0 (None)
                      208 LOAD_CONST               0 (None)
                      210 PRECALL                  2
                      214 CALL                     2
                      224 POP_TOP
                      226 JUMP_FORWARD            11 (to 250)
                  >>  228 PUSH_EXC_INFO
@@ -780,30 +792,30 @@
                      238 POP_EXCEPT
                      240 RERAISE                  1
                  >>  242 POP_TOP
                      244 POP_EXCEPT
                      246 POP_TOP
                      248 POP_TOP
          
-         108     >>  250 LOAD_FAST                0 (checkpoint)
+         109     >>  250 LOAD_FAST                0 (checkpoint)
                      252 RETURN_VALUE
          ExceptionTable:
            52 to 202 -> 228 [1] lasti
            228 to 234 -> 236 [3] lasti
            242 to 242 -> 236 [3] lasti
          consts
             None
             '\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            '
          names      ('db', 'connect', 'sqlalchemy', 'text', 'execute', 'asdict', 'commit')
          varnames   ('checkpoint', 'con', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_checkpoint'
-         firstlineno 98
+         firstlineno 99
          lnotab 0x02013401160102ff1006460128f82e09
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -813,50 +825,52 @@
             006a0400000000000000006401a6010000ab010000000000000000a60100
             00ab0100000000000000007d01740b000000000000000000006a06000000
             00000000007c01a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d02640064006400a6020000ab02000000000000000001
             006e0b230031007304770278035900770101005900010001007c025300
-         114           0 RESUME                   0
+         115           0 RESUME                   0
          
-         115           2 LOAD_GLOBAL              0 (db)
+         116           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         116          54 LOAD_FAST                0 (conn)
+         117          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
-                      78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         
+         118          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
                      100 LOAD_CONST               1 ("SELECT *, meta->>'group' as group FROM search")
                      102 PRECALL                  1
                      106 CALL                     1
-                     116 PRECALL                  1
+         
+         117         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         117         132 LOAD_GLOBAL             11 (NULL + pd)
+         120         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         115         248 LOAD_CONST               0 (None)
+         116         248 LOAD_CONST               0 (None)
                      250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 PRECALL                  2
                      258 CALL                     2
                      268 POP_TOP
                      270 JUMP_FORWARD            11 (to 294)
                  >>  272 PUSH_EXC_INFO
@@ -867,15 +881,15 @@
                      282 POP_EXCEPT
                      284 RERAISE                  1
                  >>  286 POP_TOP
                      288 POP_EXCEPT
                      290 POP_TOP
                      292 POP_TOP
          
-         118     >>  294 LOAD_FAST                2 (df)
+         121     >>  294 LOAD_FAST                2 (df)
                      296 RETURN_VALUE
          ExceptionTable:
            52 to 246 -> 272 [1] lasti
            272 to 278 -> 280 [3] lasti
            286 to 286 -> 280 [3] lasti
          consts
             None
@@ -883,16 +897,16 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search'
-         firstlineno 114
-         lnotab 0x020134014e0174fe2e03
+         firstlineno 115
+         lnotab 0x02013401180126ff100374fc2e05
       'search_uid'
       'last_event_type'
       code
          argcount  : 2
          nlocals   : 8
          stacksize : 7
          flags     : 3
@@ -916,84 +930,84 @@
             17000000000000000000007c00a6010000ab0100000000000000007d077c
             05a00c00000000000000000000000000000000000000007c076a0d000000
             0000000000a00e0000000000000000000000000000000000000000640964
             06a6020000ab0200000000000000007c076a0d0000000000000000a00e00
             00000000000000000000000000000000000000640aa6010000ab01000000
             0000000000640b6b0200000000ac0ca6020000ab0200000000000000007d
             057c055300
-         121           0 RESUME                   0
+         124           0 RESUME                   0
          
-         122           2 LOAD_GLOBAL              0 (db)
+         125           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               2 (conn)
          
-         123          54 LOAD_FAST                1 (last_event_type)
+         126          54 LOAD_FAST                1 (last_event_type)
                       56 POP_JUMP_FORWARD_IF_NONE    46 (to 150)
          
-         124          58 LOAD_CONST               1 ('SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type')
+         127          58 LOAD_CONST               1 ('SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type')
                       60 STORE_FAST               3 (statement)
          
-         125          62 LOAD_FAST                2 (conn)
+         128          62 LOAD_FAST                2 (conn)
                       64 LOAD_METHOD              2 (execute)
          
-         126          86 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         129          86 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       98 LOAD_ATTR                4 (text)
                      108 LOAD_FAST                3 (statement)
                      110 PRECALL                  1
                      114 CALL                     1
          
-         127         124 LOAD_FAST                0 (search_uid)
+         130         124 LOAD_FAST                0 (search_uid)
                      126 LOAD_FAST                1 (last_event_type)
                      128 LOAD_CONST               2 (('search_uid', 'last_event_type'))
                      130 BUILD_CONST_KEY_MAP      2
          
-         125         132 PRECALL                  2
+         128         132 PRECALL                  2
                      136 CALL                     2
                      146 STORE_FAST               4 (result)
                      148 JUMP_FORWARD            44 (to 238)
          
-         131     >>  150 LOAD_CONST               3 ('SELECT * FROM target WHERE search_uid = :search_uid')
+         134     >>  150 LOAD_CONST               3 ('SELECT * FROM target WHERE search_uid = :search_uid')
                      152 STORE_FAST               3 (statement)
          
-         132         154 LOAD_FAST                2 (conn)
+         135         154 LOAD_FAST                2 (conn)
                      156 LOAD_METHOD              2 (execute)
          
-         133         178 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         136         178 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      190 LOAD_ATTR                4 (text)
                      200 LOAD_FAST                3 (statement)
                      202 PRECALL                  1
                      206 CALL                     1
          
-         134         216 LOAD_CONST               4 ('search_uid')
+         137         216 LOAD_CONST               4 ('search_uid')
                      218 LOAD_FAST                0 (search_uid)
                      220 BUILD_MAP                1
          
-         132         222 PRECALL                  2
+         135         222 PRECALL                  2
                      226 CALL                     2
                      236 STORE_FAST               4 (result)
          
-         137     >>  238 LOAD_GLOBAL             11 (NULL + pd)
+         140     >>  238 LOAD_GLOBAL             11 (NULL + pd)
                      250 LOAD_ATTR                6 (DataFrame)
                      260 LOAD_FAST                4 (result)
                      262 LOAD_METHOD              7 (fetchall)
                      284 PRECALL                  0
                      288 CALL                     0
                      298 LOAD_FAST                4 (result)
                      300 LOAD_METHOD              8 (keys)
                      322 PRECALL                  0
                      326 CALL                     0
                      336 KW_NAMES                 5
                      338 PRECALL                  2
                      342 CALL                     2
                      352 STORE_FAST               5 (targets)
          
-         122         354 LOAD_CONST               0 (None)
+         125         354 LOAD_CONST               0 (None)
                      356 LOAD_CONST               0 (None)
                      358 LOAD_CONST               0 (None)
                      360 PRECALL                  2
                      364 CALL                     2
                      374 POP_TOP
                      376 JUMP_FORWARD            11 (to 400)
                  >>  378 PUSH_EXC_INFO
@@ -1004,62 +1018,62 @@
                      388 POP_EXCEPT
                      390 RERAISE                  1
                  >>  392 POP_TOP
                      394 POP_EXCEPT
                      396 POP_TOP
                      398 POP_TOP
          
-         139     >>  400 LOAD_GLOBAL             19 (NULL + comment_by_domain)
+         142     >>  400 LOAD_GLOBAL             19 (NULL + comment_by_domain)
                      412 LOAD_FAST                0 (search_uid)
                      414 PRECALL                  1
                      418 CALL                     1
                      428 STORE_FAST               6 (comments)
          
-         140         430 LOAD_FAST                5 (targets)
+         143         430 LOAD_FAST                5 (targets)
                      432 LOAD_METHOD             10 (merge)
                      454 LOAD_FAST                6 (comments)
                      456 LOAD_CONST               6 ('domain')
                      458 LOAD_CONST               7 ('left')
                      460 KW_NAMES                 8
                      462 PRECALL                  3
                      466 CALL                     3
                      476 STORE_FAST               5 (targets)
          
-         143         478 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
+         146         478 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
                      490 LOAD_FAST                0 (search_uid)
                      492 PRECALL                  1
                      496 CALL                     1
                      506 STORE_FAST               7 (search)
          
-         144         508 LOAD_FAST                5 (targets)
+         147         508 LOAD_FAST                5 (targets)
                      510 LOAD_METHOD             12 (sort_values)
          
-         145         532 LOAD_FAST                7 (search)
+         148         532 LOAD_FAST                7 (search)
                      534 LOAD_ATTR               13 (sort)
                      544 LOAD_METHOD             14 (get)
                      566 LOAD_CONST               9 ('field')
                      568 LOAD_CONST               6 ('domain')
                      570 PRECALL                  2
                      574 CALL                     2
          
-         146         584 LOAD_FAST                7 (search)
+         149         584 LOAD_FAST                7 (search)
                      586 LOAD_ATTR               13 (sort)
                      596 LOAD_METHOD             14 (get)
                      618 LOAD_CONST              10 ('order')
                      620 PRECALL                  1
                      624 CALL                     1
                      634 LOAD_CONST              11 ('asc')
                      636 COMPARE_OP               2 (==)
          
-         144         642 KW_NAMES                12
+         147         642 KW_NAMES                12
                      644 PRECALL                  2
                      648 CALL                     2
                      658 STORE_FAST               5 (targets)
          
-         150         660 LOAD_FAST                5 (targets)
+         152         660 LOAD_FAST                5 (targets)
                      662 RETURN_VALUE
          ExceptionTable:
            52 to 352 -> 378 [1] lasti
            378 to 384 -> 386 [3] lasti
            392 to 392 -> 386 [3] lasti
          consts
             None
@@ -1077,18 +1091,18 @@
             ('by', 'ascending')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get')
          varnames   ('search_uid', 'last_event_type', 'conn', 'statement', 'result', 'targets', 'comments', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target'
-         firstlineno 121
+         firstlineno 124
          lnotab
             0x02013401040104011801260108fe120604011801260106fe100574f12e
-            111e0130031e01180134013afe1206
+            111e0130031e01180134013afe1205
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
@@ -1098,59 +1112,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         153           0 RESUME                   0
+         155           0 RESUME                   0
          
-         154           2 LOAD_GLOBAL              0 (db)
+         156           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         155          54 LOAD_CONST               1 ('\n                SELECT last_event_type, count(*)\n                FROM target\n                WHERE search_uid = :search_uid\n                GROUP BY last_event_type\n            ')
+         157          54 LOAD_CONST               1 ('\n                SELECT last_event_type, count(*)\n                FROM target\n                WHERE search_uid = :search_uid\n                GROUP BY last_event_type\n            ')
                       56 STORE_FAST               2 (statement)
          
-         161          58 LOAD_FAST                1 (conn)
+         163          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         162          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         164          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         163         120 LOAD_CONST               2 ('search_uid')
+         165         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         161         126 PRECALL                  2
+         163         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         165         142 LOAD_GLOBAL             11 (NULL + pd)
+         167         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         154         258 LOAD_CONST               0 (None)
+         156         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -1161,15 +1175,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         166     >>  304 LOAD_FAST                4 (df)
+         168     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -1178,15 +1192,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target_count'
-         firstlineno 153
+         firstlineno 155
          lnotab 0x0201340104061801260106fe100474f52e0c
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -1197,56 +1211,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         169           0 RESUME                   0
+         171           0 RESUME                   0
          
-         170           2 LOAD_GLOBAL              0 (db)
+         172           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         171          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         173          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         176          58 LOAD_FAST                1 (conn)
+         178          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         177         142 LOAD_GLOBAL             11 (NULL + pd)
+         179         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         170         258 LOAD_CONST               0 (None)
+         172         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -1257,15 +1271,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         178     >>  304 LOAD_FAST                4 (df)
+         180     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -1274,15 +1288,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 169
+         firstlineno 171
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -1293,53 +1307,53 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d03640064006400a6020000ab020000000000
             00000001006e0b230031007304770278035900770101005900010001007c
             035300
-         180           0 RESUME                   0
+         183           0 RESUME                   0
          
-         181           2 LOAD_GLOBAL              0 (db)
+         184           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         182          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
+         185          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
                       56 STORE_FAST               1 (statement)
          
-         186          58 LOAD_FAST                0 (conn)
+         189          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         187         136 LOAD_GLOBAL             11 (NULL + pd)
+         190         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         181         252 LOAD_CONST               0 (None)
+         184         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -1350,15 +1364,15 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         188     >>  298 LOAD_FAST                3 (df)
+         191     >>  298 LOAD_FAST                3 (df)
                      300 RETURN_VALUE
          ExceptionTable:
            52 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -1366,108 +1380,112 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'company'
-         firstlineno 180
+         firstlineno 183
          lnotab 0x0201340104044e0174fa2e07
       code
-         argcount  : 0
-         nlocals   : 4
+         argcount  : 1
+         nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
-            00000000000000a6000000ab00000000000000000035007d0064017d017c
-            00a002000000000000000000000000000000000000000074070000000000
-            00000000006a0400000000000000007c01a6010000ab0100000000000000
-            00a6010000ab0100000000000000007d02740b000000000000000000006a
-            0600000000000000007c02a0070000000000000000000000000000000000
-            000000a6000000ab0000000000000000007c02a008000000000000000000
-            0000000000000000000000a6000000ab000000000000000000ac02a60200
-            00ab0200000000000000007d03640064006400a6020000ab020000000000
-            00000001006e0b230031007304770278035900770101005900010001007c
-            035300
-         190           0 RESUME                   0
+            00000000000000a6000000ab00000000000000000035007d0164017d027c
+            01a002000000000000000000000000000000000000000074070000000000
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03740b0000000000
+            00000000006a0600000000000000007c03a0070000000000000000000000
+            000000000000000000a6000000ab0000000000000000007c03a008000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
+            02000000000000000001006e0b2300310073047702780359007701010059
+            00010001007c045300
+         194           0 RESUME                   0
          
-         191           2 LOAD_GLOBAL              0 (db)
+         195           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
-                      52 STORE_FAST               0 (conn)
+                      52 STORE_FAST               1 (conn)
          
-         192          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n            ')
-                      56 STORE_FAST               1 (statement)
+         196          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            ')
+                      56 STORE_FAST               2 (statement)
          
-         196          58 LOAD_FAST                0 (conn)
+         202          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
-                     104 LOAD_FAST                1 (statement)
+                     104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
-                     120 PRECALL                  1
-                     124 CALL                     1
-                     134 STORE_FAST               2 (result)
+                     120 LOAD_CONST               2 ('search_uid')
+                     122 LOAD_FAST                0 (search_uid)
+                     124 BUILD_MAP                1
+                     126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
          
-         197         136 LOAD_GLOBAL             11 (NULL + pd)
-                     148 LOAD_ATTR                6 (DataFrame)
-                     158 LOAD_FAST                2 (result)
-                     160 LOAD_METHOD              7 (fetchall)
-                     182 PRECALL                  0
-                     186 CALL                     0
-                     196 LOAD_FAST                2 (result)
-                     198 LOAD_METHOD              8 (keys)
-                     220 PRECALL                  0
-                     224 CALL                     0
-                     234 KW_NAMES                 2
-                     236 PRECALL                  2
-                     240 CALL                     2
-                     250 STORE_FAST               3 (df)
+         203         142 LOAD_GLOBAL             11 (NULL + pd)
+                     154 LOAD_ATTR                6 (DataFrame)
+                     164 LOAD_FAST                3 (result)
+                     166 LOAD_METHOD              7 (fetchall)
+                     188 PRECALL                  0
+                     192 CALL                     0
+                     202 LOAD_FAST                3 (result)
+                     204 LOAD_METHOD              8 (keys)
+                     226 PRECALL                  0
+                     230 CALL                     0
+                     240 KW_NAMES                 3
+                     242 PRECALL                  2
+                     246 CALL                     2
+                     256 STORE_FAST               4 (df)
          
-         191         252 LOAD_CONST               0 (None)
-                     254 LOAD_CONST               0 (None)
-                     256 LOAD_CONST               0 (None)
-                     258 PRECALL                  2
-                     262 CALL                     2
-                     272 POP_TOP
-                     274 JUMP_FORWARD            11 (to 298)
-                 >>  276 PUSH_EXC_INFO
-                     278 WITH_EXCEPT_START
-                     280 POP_JUMP_FORWARD_IF_TRUE     4 (to 290)
-                     282 RERAISE                  2
-                 >>  284 COPY                     3
-                     286 POP_EXCEPT
-                     288 RERAISE                  1
-                 >>  290 POP_TOP
+         195         258 LOAD_CONST               0 (None)
+                     260 LOAD_CONST               0 (None)
+                     262 LOAD_CONST               0 (None)
+                     264 PRECALL                  2
+                     268 CALL                     2
+                     278 POP_TOP
+                     280 JUMP_FORWARD            11 (to 304)
+                 >>  282 PUSH_EXC_INFO
+                     284 WITH_EXCEPT_START
+                     286 POP_JUMP_FORWARD_IF_TRUE     4 (to 296)
+                     288 RERAISE                  2
+                 >>  290 COPY                     3
                      292 POP_EXCEPT
-                     294 POP_TOP
-                     296 POP_TOP
+                     294 RERAISE                  1
+                 >>  296 POP_TOP
+                     298 POP_EXCEPT
+                     300 POP_TOP
+                     302 POP_TOP
          
-         198     >>  298 LOAD_FAST                3 (df)
-                     300 RETURN_VALUE
+         204     >>  304 LOAD_FAST                4 (df)
+                     306 RETURN_VALUE
          ExceptionTable:
-           52 to 250 -> 276 [1] lasti
-           276 to 282 -> 284 [3] lasti
-           290 to 290 -> 284 [3] lasti
+           52 to 256 -> 282 [1] lasti
+           282 to 288 -> 290 [3] lasti
+           296 to 296 -> 290 [3] lasti
          consts
             None
-            '\n                SELECT *\n                FROM checkpoint\n            '
+            '\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            '
+            'search_uid'
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
-         varnames   ('conn', 'statement', 'result', 'df')
+         varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'checkpoint'
-         firstlineno 190
-         lnotab 0x0201340104044e0174fa2e07
+         firstlineno 194
+         lnotab 0x020134010406540174f82e09
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
@@ -1481,59 +1499,59 @@
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c04a009000000000000000000000000000000000000000064
             04a6010000ab010000000000000000a00a00000000000000000000000000
             000000000000006405640684006901a6010000ab010000000000000000a0
             0b0000000000000000000000000000000000000000a6000000ab00000000
             00000000005300
-         201           0 RESUME                   0
+         207           0 RESUME                   0
          
-         202           2 LOAD_GLOBAL              0 (db)
+         208           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         203          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
+         209          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
                       56 STORE_FAST               2 (statement)
          
-         210          58 LOAD_FAST                1 (conn)
+         216          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         211          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         217          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         212         120 LOAD_CONST               2 ('search_uid')
+         218         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         210         126 PRECALL                  2
+         216         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         214         142 LOAD_GLOBAL             11 (NULL + pd)
+         220         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         202         258 LOAD_CONST               0 (None)
+         208         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -1544,22 +1562,22 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         216     >>  304 LOAD_FAST                4 (df)
+         222     >>  304 LOAD_FAST                4 (df)
                      306 LOAD_METHOD              9 (groupby)
                      328 LOAD_CONST               4 ('domain')
                      330 PRECALL                  1
                      334 CALL                     1
                      344 LOAD_METHOD             10 (agg)
                      366 LOAD_CONST               5 ('comment')
-                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 216>)
+                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 222>)
                      370 MAKE_FUNCTION            0
                      372 BUILD_MAP                1
                      374 PRECALL                  1
                      378 CALL                     1
                      388 LOAD_METHOD             11 (reset_index)
                      410 PRECALL                  0
                      414 CALL                     0
@@ -1579,37 +1597,37 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-               216           0 RESUME                   0
+               222           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('list',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 216
+               firstlineno 222
                lnotab 0x
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'groupby', 'agg', 'reset_index')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'comment_by_domain'
-         firstlineno 201
+         firstlineno 207
          lnotab 0x0201340104071801260106fe100474f42e0e
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
@@ -1622,41 +1640,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         222           0 RESUME                   0
+         228           0 RESUME                   0
          
-         223           2 LOAD_GLOBAL              0 (db)
+         229           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         224          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
+         230          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         229          58 LOAD_FAST                1 (conn)
+         235          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         223         142 LOAD_CONST               0 (None)
+         229         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -1667,24 +1685,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         231     >>  188 LOAD_FAST                3 (result)
+         237     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         232         210 LOAD_CONST               0 (None)
+         238         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         234     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         240     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -1692,15 +1710,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         235         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         241         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Search)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -1713,15 +1731,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Search')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_uid'
-         firstlineno 222
+         firstlineno 228
          lnotab 0x02013401040554fa2e08160104028201
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -1735,41 +1753,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         238           0 RESUME                   0
+         244           0 RESUME                   0
          
-         239           2 LOAD_GLOBAL              0 (db)
+         245           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         240          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         246          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         245          58 LOAD_FAST                1 (conn)
+         251          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('domain')
                      122 LOAD_FAST                0 (domain)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         239         142 LOAD_CONST               0 (None)
+         245         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -1780,24 +1798,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         247     >>  188 LOAD_FAST                3 (result)
+         253     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         248         210 LOAD_CONST               0 (None)
+         254         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         250     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         256     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -1805,15 +1823,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         251         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         257         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -1826,15 +1844,128 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 238
+         firstlineno 244
+         lnotab 0x02013401040554fa2e08160104028201
+      'event_id'
+      code
+         argcount  : 1
+         nlocals   : 5
+         stacksize : 7
+         flags     : 3
+         code
+            0x9700740000000000000000000000a00100000000000000000000000000
+            00000000000000a6000000ab00000000000000000035007d0164017d027c
+            01a002000000000000000000000000000000000000000074070000000000
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03640064006400a6
+            020000ab02000000000000000001006e0b23003100730477027803590077
+            0101005900010001007c036a05000000000000000064036b020000000072
+            0264005300740d00000000000000000000740f000000000000000000007c
+            03a0080000000000000000000000000000000000000000a6000000ab0000
+            000000000000007c03a00900000000000000000000000000000000000000
+            00a6000000ab000000000000000000a6020000ab020000000000000000a6
+            010000ab0100000000000000007d04741500000000000000000000741600
+            0000000000000000007c04a6020000ab0200000000000000005300
+         260           0 RESUME                   0
+         
+         261           2 LOAD_GLOBAL              0 (db)
+                      14 LOAD_METHOD              1 (connect)
+                      36 PRECALL                  0
+                      40 CALL                     0
+                      50 BEFORE_WITH
+                      52 STORE_FAST               1 (conn)
+         
+         262          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+                      56 STORE_FAST               2 (statement)
+         
+         267          58 LOAD_FAST                1 (conn)
+                      60 LOAD_METHOD              2 (execute)
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                2 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 LOAD_CONST               2 ('event_id')
+                     122 LOAD_FAST                0 (event_id)
+                     124 BUILD_MAP                1
+                     126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         261         142 LOAD_CONST               0 (None)
+                     144 LOAD_CONST               0 (None)
+                     146 LOAD_CONST               0 (None)
+                     148 PRECALL                  2
+                     152 CALL                     2
+                     162 POP_TOP
+                     164 JUMP_FORWARD            11 (to 188)
+                 >>  166 PUSH_EXC_INFO
+                     168 WITH_EXCEPT_START
+                     170 POP_JUMP_FORWARD_IF_TRUE     4 (to 180)
+                     172 RERAISE                  2
+                 >>  174 COPY                     3
+                     176 POP_EXCEPT
+                     178 RERAISE                  1
+                 >>  180 POP_TOP
+                     182 POP_EXCEPT
+                     184 POP_TOP
+                     186 POP_TOP
+         
+         269     >>  188 LOAD_FAST                3 (result)
+                     190 LOAD_ATTR                5 (rowcount)
+                     200 LOAD_CONST               3 (0)
+                     202 COMPARE_OP               2 (==)
+                     208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
+         
+         270         210 LOAD_CONST               0 (None)
+                     212 RETURN_VALUE
+         
+         272     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+                     226 LOAD_GLOBAL             15 (NULL + zip)
+                     238 LOAD_FAST                3 (result)
+                     240 LOAD_METHOD              8 (keys)
+                     262 PRECALL                  0
+                     266 CALL                     0
+                     276 LOAD_FAST                3 (result)
+                     278 LOAD_METHOD              9 (fetchone)
+                     300 PRECALL                  0
+                     304 CALL                     0
+                     314 PRECALL                  2
+                     318 CALL                     2
+                     328 PRECALL                  1
+                     332 CALL                     1
+                     342 STORE_FAST               4 (obj)
+         
+         273         344 LOAD_GLOBAL             21 (NULL + from_dict)
+                     356 LOAD_GLOBAL             22 (Event)
+                     368 LOAD_FAST                4 (obj)
+                     370 PRECALL                  2
+                     374 CALL                     2
+                     384 RETURN_VALUE
+         ExceptionTable:
+           52 to 140 -> 166 [1] lasti
+           166 to 172 -> 174 [3] lasti
+           180 to 180 -> 174 [3] lasti
+         consts
+            None
+            '\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            '
+            'event_id'
+            0
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
+         varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'find_event_by_id'
+         firstlineno 260
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 10
          flags     : 3
          code
@@ -1848,76 +1979,76 @@
             020000ab02000000000000000001007c01a0020000000000000000000000
             0000000000000000007407000000000000000000006a0400000000000000
             006403a6010000ab010000000000000000a6010000ab0100000000000000
             0001007c01a00b0000000000000000000000000000000000000000a60000
             00ab0000000000000000000100640064006400a6020000ab020000000000
             000000010064005300230031007304770278035900770101005900010001
             0064005300
-         257           0 RESUME                   0
+         278           0 RESUME                   0
          
-         258           2 LOAD_GLOBAL              0 (db)
+         279           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         259          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
+         280          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         268          58 LOAD_FAST                1 (conn)
+         289          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         269          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         290          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         271         120 LOAD_FAST                0 (company)
+         292         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (name)
          
-         272         132 LOAD_FAST                0 (company)
+         293         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (description)
          
-         273         144 LOAD_FAST                0 (company)
+         294         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (domain)
          
-         274         156 LOAD_GLOBAL             17 (NULL + json)
+         295         156 LOAD_GLOBAL             17 (NULL + json)
                      168 LOAD_ATTR                9 (dumps)
                      178 LOAD_FAST                0 (company)
                      180 LOAD_ATTR               10 (meta)
                      190 PRECALL                  1
                      194 CALL                     1
          
-         270         204 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
+         291         204 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
                      206 BUILD_CONST_KEY_MAP      4
          
-         268         208 PRECALL                  2
+         289         208 PRECALL                  2
                      212 CALL                     2
                      222 POP_TOP
          
-         277         224 LOAD_FAST                1 (conn)
+         298         224 LOAD_FAST                1 (conn)
                      226 LOAD_METHOD              2 (execute)
                      248 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      260 LOAD_ATTR                4 (text)
                      270 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW target')
                      272 PRECALL                  1
                      276 CALL                     1
                      286 PRECALL                  1
                      290 CALL                     1
                      300 POP_TOP
          
-         278         302 LOAD_FAST                1 (conn)
+         299         302 LOAD_FAST                1 (conn)
                      304 LOAD_METHOD             11 (commit)
                      326 PRECALL                  0
                      330 CALL                     0
                      340 POP_TOP
          
-         258         342 LOAD_CONST               0 (None)
+         279         342 LOAD_CONST               0 (None)
                      344 LOAD_CONST               0 (None)
                      346 LOAD_CONST               0 (None)
                      348 PRECALL                  2
                      352 CALL                     2
                      362 POP_TOP
                      364 LOAD_CONST               0 (None)
                      366 RETURN_VALUE
@@ -1945,15 +2076,15 @@
             'REFRESH MATERIALIZED VIEW target'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'name', 'description', 'domain', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 257
+         firstlineno 278
          lnotab 0x020134010409180126020c010c010c0130fc04fe10094e0128ec
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 9
          flags     : 3
          code
@@ -1966,72 +2097,72 @@
             000000000000007c006a080000000000000000a6010000ab010000000000
             000000740b000000000000000000006a0600000000000000007c006a0900
             00000000000000a6010000ab0100000000000000007c006a0a0000000000
             00000064029c04a6020000ab02000000000000000001007c01a00b000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             000100640064006400a6020000ab02000000000000000001006400530023
             00310073047702780359007701010059000100010064005300
-         281           0 RESUME                   0
+         302           0 RESUME                   0
          
-         282           2 LOAD_GLOBAL              0 (db)
+         303           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         283          54 LOAD_FAST                1 (conn)
+         304          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         284          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         305          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         285         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
+         306         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
          
-         284         102 PRECALL                  1
+         305         102 PRECALL                  1
                      106 CALL                     1
          
-         295         116 LOAD_GLOBAL             11 (NULL + json)
+         316         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (sort)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         296         164 LOAD_GLOBAL             11 (NULL + json)
+         317         164 LOAD_GLOBAL             11 (NULL + json)
                      176 LOAD_ATTR                6 (dumps)
                      186 LOAD_FAST                0 (search)
                      188 LOAD_ATTR                8 (inclusion)
                      198 PRECALL                  1
                      202 CALL                     1
          
-         297         212 LOAD_GLOBAL             11 (NULL + json)
+         318         212 LOAD_GLOBAL             11 (NULL + json)
                      224 LOAD_ATTR                6 (dumps)
                      234 LOAD_FAST                0 (search)
                      236 LOAD_ATTR                9 (exclusion)
                      246 PRECALL                  1
                      250 CALL                     1
          
-         298         260 LOAD_FAST                0 (search)
+         319         260 LOAD_FAST                0 (search)
                      262 LOAD_ATTR               10 (uid)
          
-         294         272 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
+         315         272 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
                      274 BUILD_CONST_KEY_MAP      4
          
-         283         276 PRECALL                  2
+         304         276 PRECALL                  2
                      280 CALL                     2
                      290 POP_TOP
          
-         301         292 LOAD_FAST                1 (conn)
+         322         292 LOAD_FAST                1 (conn)
                      294 LOAD_METHOD             11 (commit)
                      316 PRECALL                  0
                      320 CALL                     0
                      330 POP_TOP
          
-         282         332 LOAD_CONST               0 (None)
+         303         332 LOAD_CONST               0 (None)
                      334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 PRECALL                  2
                      342 CALL                     2
                      352 POP_TOP
                      354 LOAD_CONST               0 (None)
                      356 RETURN_VALUE
@@ -2058,20 +2189,20 @@
             ('sort', 'inclusion', 'exclusion', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'sort', 'inclusion', 'exclusion', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 281
+         firstlineno 302
          lnotab 0x020134011801160102ff0e0b3001300130010cfc04f5101228ed
       (None,)
-   names      ('json', 'pandas', 'pd', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai.models', 'Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint', 'sqlalchemy', 'google.cloud.sql.connector', 'Connector', 'dotenv', 'load_dotenv', 'gandai.db', 'connect_with_connector', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'search', 'int', 'str', 'target', 'DataFrame', 'target_count', 'event', 'company', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'update_company', 'update_search')
+   names      ('json', 'pandas', 'pd', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai.models', 'Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint', 'sqlalchemy', 'google.cloud.sql.connector', 'Connector', 'dotenv', 'load_dotenv', 'gandai.db', 'connect_with_connector', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'search', 'int', 'str', 'target', 'DataFrame', 'target_count', 'event', 'company', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'find_event_by_id', 'update_company', 'update_search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010c010c01200a08020c010c0114020c0214060c0e10
-      15100f10131010060712201a101a0b160a160b1a15101010131018
+      0x00ff0201080108010c010c01200a08020c010c0214020c0214060c0e10
+      15100f101310100609121f1a101a0c160b1a0d1a151010101010121018
```

### Comparing `gandai-1.1.7/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.1.8/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xb5925e64 (Fri May 12 19:25:41 2023 UTC)
-files sz: 5418
+moddate:  0xd24b6164 (Sun May 14 21:00:02 2023 UTC)
+files sz: 5497
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -56,17 +56,17 @@
                 78 LOAD_CONST               5 (<code object GrataWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 10>)
                 80 MAKE_FUNCTION            0
                 82 LOAD_CONST               6 ('GrataWrapper')
                 84 PRECALL                  2
                 88 CALL                     2
                 98 STORE_NAME               8 (GrataWrapper)
    
-   165         100 PUSH_NULL
+   166         100 PUSH_NULL
                102 LOAD_BUILD_CLASS
-               104 LOAD_CONST               7 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 165>)
+               104 LOAD_CONST               7 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 166>)
                106 MAKE_FUNCTION            0
                108 LOAD_CONST               8 ('SourceScrubWrapper')
                110 PRECALL                  2
                114 CALL                     2
                124 STORE_NAME               9 (SourceScrubWrapper)
                126 LOAD_CONST               3 (None)
                128 RETURN_VALUE
@@ -135,20 +135,20 @@
                       94 LOAD_CONST               7 ('return')
                       96 LOAD_NAME               10 (dict)
                       98 BUILD_TUPLE              4
                      100 LOAD_CONST              10 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 54>)
                      102 MAKE_FUNCTION            4 (annotations)
                      104 STORE_NAME              12 (enrich)
          
-          63         106 LOAD_CONST               6 ('search')
+          64         106 LOAD_CONST               6 ('search')
                      108 LOAD_NAME                7 (Search)
                      110 LOAD_CONST               7 ('return')
                      112 LOAD_NAME               10 (dict)
                      114 BUILD_TUPLE              4
-                     116 LOAD_CONST              11 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 63>)
+                     116 LOAD_CONST              11 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 64>)
                      118 MAKE_FUNCTION            4 (annotations)
                      120 STORE_NAME              13 (_get_api_filter)
                      122 LOAD_CONST              12 (None)
                      124 RETURN_VALUE
          consts
             'GrataWrapper'
             'GRATA_API_TOKEN'
@@ -384,15 +384,17 @@
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000006401740400
                   0000000000000000006a03000000000000000064027c006901ac03a60300
                   00ab0300000000000000007d017c01a00400000000000000000000000000
-                  00000000000000a6000000ab0000000000000000007d027c025300
+                  00000000000000a6000000ab0000000000000000007d027c02a005000000
+                  00000000000000000000000000000000006404a6010000ab010000000000
+                  0000007c0264053c0000007c025300
                 54           0 RESUME                   0
                
                 55           2 LOAD_GLOBAL              1 (NULL + requests)
                             14 LOAD_ATTR                1 (post)
                
                 56          24 LOAD_CONST               1 ('https://search.grata.com/api/v1/enrich/')
                
@@ -411,28 +413,39 @@
                 60          72 LOAD_FAST                1 (response)
                             74 LOAD_METHOD              4 (json)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 STORE_FAST               2 (data)
                
                 61         112 LOAD_FAST                2 (data)
-                           114 RETURN_VALUE
+                           114 LOAD_METHOD              5 (get)
+                           136 LOAD_CONST               4 ('social_linkedin')
+                           138 PRECALL                  1
+                           142 CALL                     1
+                           152 LOAD_FAST                2 (data)
+                           154 LOAD_CONST               5 ('linkedin')
+                           156 STORE_SUBSCR
+               
+                62         160 LOAD_FAST                2 (data)
+                           162 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1/enrich/'
                   'domain'
                   ('headers', 'json')
-               names      ('requests', 'post', 'GrataWrapper', 'HEADERS', 'json')
+                  'social_linkedin'
+                  'linkedin'
+               names      ('requests', 'post', 'GrataWrapper', 'HEADERS', 'json', 'get')
                varnames   ('domain', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
                firstlineno 54
-               lnotab 0x020116010201160106fd12052801
+               lnotab 0x020116010201160106fd120528013001
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 8
                flags     : 3
                code
                   0x8700870487059700690064016402930164036404930164056406930164
@@ -445,361 +458,373 @@
                   01644364449301a50169006445644693016447644893016449644a930164
                   4b644c9301644d644e9301644f6450930164516452930164536454930164
                   55645693016457645893016459645a9301645b645c9301645d645e930164
                   5f64609301646164629301646364649301a5018a05646564666467646864
                   699c048a04646a740000000000000000000000660288006601646b840c7d
                   01646a74020000000000000000000066028804880588006603646c840c7d
                   02646a740200000000000000000000660288006601646d840c7d03646e89
-                  006a020000000000000000646f1900000000000000000089006a03000000
-                  0000000000646f1900000000000000000089006a02000000000000000064
-                  701900000000000000000002007c01a6000000ab00000000000000000002
-                  007c02a6000000ab00000000000000000002007c03a6000000ab00000000
-                  000000000064719c0264729c065300
+                  006a020000000000000000a0030000000000000000000000000000000000
+                  000000646f6700a6020000ab02000000000000000089006a040000000000
+                  000000a0030000000000000000000000000000000000000000646f6700a6
+                  020000ab02000000000000000089006a020000000000000000a003000000
+                  000000000000000000000000000000000064706700a6020000ab02000000
+                  000000000002007c01a6000000ab00000000000000000002007c02a60000
+                  00ab00000000000000000002007c03a6000000ab00000000000000000064
+                  719c0264729c065300
                              0 MAKE_CELL                0 (search)
                              2 MAKE_CELL                4 (COUNTRIES)
                              4 MAKE_CELL                5 (STATES)
                
-                63           6 RESUME                   0
+                64           6 RESUME                   0
                
-                64           8 BUILD_MAP                0
+                65           8 BUILD_MAP                0
                
-                65          10 LOAD_CONST               1 ('AL')
+                66          10 LOAD_CONST               1 ('AL')
                             12 LOAD_CONST               2 ('Alabama')
                
-                64          14 MAP_ADD                  1
+                65          14 MAP_ADD                  1
                
-                66          16 LOAD_CONST               3 ('AK')
+                67          16 LOAD_CONST               3 ('AK')
                             18 LOAD_CONST               4 ('Alaska')
                
-                64          20 MAP_ADD                  1
+                65          20 MAP_ADD                  1
                
-                67          22 LOAD_CONST               5 ('AZ')
+                68          22 LOAD_CONST               5 ('AZ')
                             24 LOAD_CONST               6 ('Arizona')
                
-                64          26 MAP_ADD                  1
+                65          26 MAP_ADD                  1
                
-                68          28 LOAD_CONST               7 ('AR')
+                69          28 LOAD_CONST               7 ('AR')
                             30 LOAD_CONST               8 ('Arkansas')
                
-                64          32 MAP_ADD                  1
+                65          32 MAP_ADD                  1
                
-                69          34 LOAD_CONST               9 ('CA')
+                70          34 LOAD_CONST               9 ('CA')
                             36 LOAD_CONST              10 ('California')
                
-                64          38 MAP_ADD                  1
+                65          38 MAP_ADD                  1
                
-                70          40 LOAD_CONST              11 ('CO')
+                71          40 LOAD_CONST              11 ('CO')
                             42 LOAD_CONST              12 ('Colorado')
                
-                64          44 MAP_ADD                  1
+                65          44 MAP_ADD                  1
                
-                71          46 LOAD_CONST              13 ('CT')
+                72          46 LOAD_CONST              13 ('CT')
                             48 LOAD_CONST              14 ('Connecticut')
                
-                64          50 MAP_ADD                  1
+                65          50 MAP_ADD                  1
                
-                72          52 LOAD_CONST              15 ('DE')
+                73          52 LOAD_CONST              15 ('DE')
                             54 LOAD_CONST              16 ('Delaware')
                
-                64          56 MAP_ADD                  1
+                65          56 MAP_ADD                  1
                
-                73          58 LOAD_CONST              17 ('FL')
+                74          58 LOAD_CONST              17 ('FL')
                             60 LOAD_CONST              18 ('Florida')
                
-                64          62 MAP_ADD                  1
+                65          62 MAP_ADD                  1
                
-                74          64 LOAD_CONST              19 ('GA')
+                75          64 LOAD_CONST              19 ('GA')
                             66 LOAD_CONST              20 ('Georgia')
                
-                64          68 MAP_ADD                  1
+                65          68 MAP_ADD                  1
                
-                75          70 LOAD_CONST              21 ('HI')
+                76          70 LOAD_CONST              21 ('HI')
                             72 LOAD_CONST              22 ('Hawaii')
                
-                64          74 MAP_ADD                  1
+                65          74 MAP_ADD                  1
                
-                76          76 LOAD_CONST              23 ('ID')
+                77          76 LOAD_CONST              23 ('ID')
                             78 LOAD_CONST              24 ('Idaho')
                
-                64          80 MAP_ADD                  1
+                65          80 MAP_ADD                  1
                
-                77          82 LOAD_CONST              25 ('IL')
+                78          82 LOAD_CONST              25 ('IL')
                             84 LOAD_CONST              26 ('Illinois')
                
-                64          86 MAP_ADD                  1
+                65          86 MAP_ADD                  1
                
-                78          88 LOAD_CONST              27 ('IN')
+                79          88 LOAD_CONST              27 ('IN')
                             90 LOAD_CONST              28 ('Indiana')
                
-                64          92 MAP_ADD                  1
+                65          92 MAP_ADD                  1
                
-                79          94 LOAD_CONST              29 ('IA')
+                80          94 LOAD_CONST              29 ('IA')
                             96 LOAD_CONST              30 ('Iowa')
                
-                64          98 MAP_ADD                  1
+                65          98 MAP_ADD                  1
                
-                80         100 LOAD_CONST              31 ('KS')
+                81         100 LOAD_CONST              31 ('KS')
                            102 LOAD_CONST              32 ('Kansas')
                
-                64         104 MAP_ADD                  1
+                65         104 MAP_ADD                  1
                
-                81         106 LOAD_CONST              33 ('KY')
+                82         106 LOAD_CONST              33 ('KY')
                            108 LOAD_CONST              34 ('Kentucky')
                
-                64         110 MAP_ADD                  1
+                65         110 MAP_ADD                  1
                            112 BUILD_MAP                0
                
-                82         114 LOAD_CONST              35 ('LA')
+                83         114 LOAD_CONST              35 ('LA')
                            116 LOAD_CONST              36 ('Louisiana')
                
-                64         118 MAP_ADD                  1
+                65         118 MAP_ADD                  1
                
-                83         120 LOAD_CONST              37 ('ME')
+                84         120 LOAD_CONST              37 ('ME')
                            122 LOAD_CONST              38 ('Maine')
                
-                64         124 MAP_ADD                  1
+                65         124 MAP_ADD                  1
                
-                84         126 LOAD_CONST              39 ('MD')
+                85         126 LOAD_CONST              39 ('MD')
                            128 LOAD_CONST              40 ('Maryland')
                
-                64         130 MAP_ADD                  1
+                65         130 MAP_ADD                  1
                
-                85         132 LOAD_CONST              41 ('MA')
+                86         132 LOAD_CONST              41 ('MA')
                            134 LOAD_CONST              42 ('Massachusetts')
                
-                64         136 MAP_ADD                  1
+                65         136 MAP_ADD                  1
                
-                86         138 LOAD_CONST              43 ('MI')
+                87         138 LOAD_CONST              43 ('MI')
                            140 LOAD_CONST              44 ('Michigan')
                
-                64         142 MAP_ADD                  1
+                65         142 MAP_ADD                  1
                
-                87         144 LOAD_CONST              45 ('MN')
+                88         144 LOAD_CONST              45 ('MN')
                            146 LOAD_CONST              46 ('Minnesota')
                
-                64         148 MAP_ADD                  1
+                65         148 MAP_ADD                  1
                
-                88         150 LOAD_CONST              47 ('MS')
+                89         150 LOAD_CONST              47 ('MS')
                            152 LOAD_CONST              48 ('Mississippi')
                
-                64         154 MAP_ADD                  1
+                65         154 MAP_ADD                  1
                
-                89         156 LOAD_CONST              49 ('MO')
+                90         156 LOAD_CONST              49 ('MO')
                            158 LOAD_CONST              50 ('Missouri')
                
-                64         160 MAP_ADD                  1
+                65         160 MAP_ADD                  1
                
-                90         162 LOAD_CONST              51 ('MT')
+                91         162 LOAD_CONST              51 ('MT')
                            164 LOAD_CONST              52 ('Montana')
                
-                64         166 MAP_ADD                  1
+                65         166 MAP_ADD                  1
                
-                91         168 LOAD_CONST              53 ('NE')
+                92         168 LOAD_CONST              53 ('NE')
                            170 LOAD_CONST              54 ('Nebraska')
                
-                64         172 MAP_ADD                  1
+                65         172 MAP_ADD                  1
                
-                92         174 LOAD_CONST              55 ('NV')
+                93         174 LOAD_CONST              55 ('NV')
                            176 LOAD_CONST              56 ('Nevada')
                
-                64         178 MAP_ADD                  1
+                65         178 MAP_ADD                  1
                
-                93         180 LOAD_CONST              57 ('NH')
+                94         180 LOAD_CONST              57 ('NH')
                            182 LOAD_CONST              58 ('New Hampshire')
                
-                64         184 MAP_ADD                  1
+                65         184 MAP_ADD                  1
                
-                94         186 LOAD_CONST              59 ('NJ')
+                95         186 LOAD_CONST              59 ('NJ')
                            188 LOAD_CONST              60 ('New Jersey')
                
-                64         190 MAP_ADD                  1
+                65         190 MAP_ADD                  1
                
-                95         192 LOAD_CONST              61 ('NM')
+                96         192 LOAD_CONST              61 ('NM')
                            194 LOAD_CONST              62 ('New Mexico')
                
-                64         196 MAP_ADD                  1
+                65         196 MAP_ADD                  1
                
-                96         198 LOAD_CONST              63 ('NY')
+                97         198 LOAD_CONST              63 ('NY')
                            200 LOAD_CONST              64 ('New York')
                
-                64         202 MAP_ADD                  1
+                65         202 MAP_ADD                  1
                
-                97         204 LOAD_CONST              65 ('NC')
+                98         204 LOAD_CONST              65 ('NC')
                            206 LOAD_CONST              66 ('North Carolina')
                
-                64         208 MAP_ADD                  1
+                65         208 MAP_ADD                  1
                
-                98         210 LOAD_CONST              67 ('ND')
+                99         210 LOAD_CONST              67 ('ND')
                            212 LOAD_CONST              68 ('North Dakota')
                
-                64         214 MAP_ADD                  1
+                65         214 MAP_ADD                  1
                            216 DICT_UPDATE              1
                            218 BUILD_MAP                0
                
-                99         220 LOAD_CONST              69 ('OH')
+               100         220 LOAD_CONST              69 ('OH')
                            222 LOAD_CONST              70 ('Ohio')
                
-                64         224 MAP_ADD                  1
+                65         224 MAP_ADD                  1
                
-               100         226 LOAD_CONST              71 ('OK')
+               101         226 LOAD_CONST              71 ('OK')
                            228 LOAD_CONST              72 ('Oklahoma')
                
-                64         230 MAP_ADD                  1
+                65         230 MAP_ADD                  1
                
-               101         232 LOAD_CONST              73 ('OR')
+               102         232 LOAD_CONST              73 ('OR')
                            234 LOAD_CONST              74 ('Oregon')
                
-                64         236 MAP_ADD                  1
+                65         236 MAP_ADD                  1
                
-               102         238 LOAD_CONST              75 ('PA')
+               103         238 LOAD_CONST              75 ('PA')
                            240 LOAD_CONST              76 ('Pennsylvania')
                
-                64         242 MAP_ADD                  1
+                65         242 MAP_ADD                  1
                
-               103         244 LOAD_CONST              77 ('RI')
+               104         244 LOAD_CONST              77 ('RI')
                            246 LOAD_CONST              78 ('Rhode Island')
                
-                64         248 MAP_ADD                  1
+                65         248 MAP_ADD                  1
                
-               104         250 LOAD_CONST              79 ('SC')
+               105         250 LOAD_CONST              79 ('SC')
                            252 LOAD_CONST              80 ('South Carolina')
                
-                64         254 MAP_ADD                  1
+                65         254 MAP_ADD                  1
                
-               105         256 LOAD_CONST              81 ('SD')
+               106         256 LOAD_CONST              81 ('SD')
                            258 LOAD_CONST              82 ('South Dakota')
                
-                64         260 MAP_ADD                  1
+                65         260 MAP_ADD                  1
                
-               106         262 LOAD_CONST              83 ('TN')
+               107         262 LOAD_CONST              83 ('TN')
                            264 LOAD_CONST              84 ('Tennessee')
                
-                64         266 MAP_ADD                  1
+                65         266 MAP_ADD                  1
                
-               107         268 LOAD_CONST              85 ('TX')
+               108         268 LOAD_CONST              85 ('TX')
                            270 LOAD_CONST              86 ('Texas')
                
-                64         272 MAP_ADD                  1
+                65         272 MAP_ADD                  1
                
-               108         274 LOAD_CONST              87 ('UT')
+               109         274 LOAD_CONST              87 ('UT')
                            276 LOAD_CONST              88 ('Utah')
                
-                64         278 MAP_ADD                  1
+                65         278 MAP_ADD                  1
                
-               109         280 LOAD_CONST              89 ('VT')
+               110         280 LOAD_CONST              89 ('VT')
                            282 LOAD_CONST              90 ('Vermont')
                
-                64         284 MAP_ADD                  1
+                65         284 MAP_ADD                  1
                
-               110         286 LOAD_CONST              91 ('VA')
+               111         286 LOAD_CONST              91 ('VA')
                            288 LOAD_CONST              92 ('Virginia')
                
-                64         290 MAP_ADD                  1
+                65         290 MAP_ADD                  1
                
-               111         292 LOAD_CONST              93 ('WA')
+               112         292 LOAD_CONST              93 ('WA')
                            294 LOAD_CONST              94 ('Washington')
                
-                64         296 MAP_ADD                  1
+                65         296 MAP_ADD                  1
                
-               112         298 LOAD_CONST              95 ('WV')
+               113         298 LOAD_CONST              95 ('WV')
                            300 LOAD_CONST              96 ('West Virginia')
                
-                64         302 MAP_ADD                  1
+                65         302 MAP_ADD                  1
                
-               113         304 LOAD_CONST              97 ('WI')
+               114         304 LOAD_CONST              97 ('WI')
                            306 LOAD_CONST              98 ('Wisconsin')
                
-                64         308 MAP_ADD                  1
+                65         308 MAP_ADD                  1
                
-               114         310 LOAD_CONST              99 ('WY')
+               115         310 LOAD_CONST              99 ('WY')
                            312 LOAD_CONST             100 ('Wyoming')
                
-                64         314 MAP_ADD                  1
+                65         314 MAP_ADD                  1
                            316 DICT_UPDATE              1
                            318 STORE_DEREF              5 (STATES)
                
-               118         320 LOAD_CONST             101 ('United States')
+               119         320 LOAD_CONST             101 ('United States')
                
-               119         322 LOAD_CONST             102 ('Canada')
+               120         322 LOAD_CONST             102 ('Canada')
                
-               120         324 LOAD_CONST             103 ('Mexico')
+               121         324 LOAD_CONST             103 ('Mexico')
                
-               121         326 LOAD_CONST             104 ('United Kingdom')
+               122         326 LOAD_CONST             104 ('United Kingdom')
                
-               117         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
+               118         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
                            330 BUILD_CONST_KEY_MAP      4
                            332 STORE_DEREF              4 (COUNTRIES)
                
-               124         334 LOAD_CONST             106 ('return')
+               125         334 LOAD_CONST             106 ('return')
                            336 LOAD_GLOBAL              0 (dict)
                            348 BUILD_TUPLE              2
                            350 LOAD_CLOSURE             0 (search)
                            352 BUILD_TUPLE              1
-                           354 LOAD_CONST             107 (<code object _ownership_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 124>)
+                           354 LOAD_CONST             107 (<code object _ownership_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 125>)
                            356 MAKE_FUNCTION           12 (annotations, closure)
                            358 STORE_FAST               1 (_ownership_filter)
                
-               137         360 LOAD_CONST             106 ('return')
+               138         360 LOAD_CONST             106 ('return')
                            362 LOAD_GLOBAL              2 (list)
                            374 BUILD_TUPLE              2
                            376 LOAD_CLOSURE             4 (COUNTRIES)
                            378 LOAD_CLOSURE             5 (STATES)
                            380 LOAD_CLOSURE             0 (search)
                            382 BUILD_TUPLE              3
-                           384 LOAD_CONST             108 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 137>)
+                           384 LOAD_CONST             108 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 138>)
                            386 MAKE_FUNCTION           12 (annotations, closure)
                            388 STORE_FAST               2 (_hq_include)
                
-               146         390 LOAD_CONST             106 ('return')
+               147         390 LOAD_CONST             106 ('return')
                            392 LOAD_GLOBAL              2 (list)
                            404 BUILD_TUPLE              2
                            406 LOAD_CLOSURE             0 (search)
                            408 BUILD_TUPLE              1
-                           410 LOAD_CONST             109 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 146>)
+                           410 LOAD_CONST             109 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 147>)
                            412 MAKE_FUNCTION           12 (annotations, closure)
                            414 STORE_FAST               3 (_hq_exclude)
                
-               153         416 LOAD_CONST             110 ('any')
+               154         416 LOAD_CONST             110 ('any')
                
-               154         418 LOAD_DEREF               0 (search)
+               155         418 LOAD_DEREF               0 (search)
                            420 LOAD_ATTR                2 (inclusion)
-                           430 LOAD_CONST             111 ('keywords')
-                           432 BINARY_SUBSCR
-               
-               155         442 LOAD_DEREF               0 (search)
-                           444 LOAD_ATTR                3 (exclusion)
-                           454 LOAD_CONST             111 ('keywords')
-                           456 BINARY_SUBSCR
-               
-               156         466 LOAD_DEREF               0 (search)
-                           468 LOAD_ATTR                2 (inclusion)
-                           478 LOAD_CONST             112 ('employees_range')
-                           480 BINARY_SUBSCR
-               
-               157         490 PUSH_NULL
-                           492 LOAD_FAST                1 (_ownership_filter)
-                           494 PRECALL                  0
-                           498 CALL                     0
-               
-               159         508 PUSH_NULL
-                           510 LOAD_FAST                2 (_hq_include)
-                           512 PRECALL                  0
-                           516 CALL                     0
-               
-               160         526 PUSH_NULL
-                           528 LOAD_FAST                3 (_hq_exclude)
-                           530 PRECALL                  0
-                           534 CALL                     0
-               
-               158         544 LOAD_CONST             113 (('include', 'exclude'))
-                           546 BUILD_CONST_KEY_MAP      2
-               
-               152         548 LOAD_CONST             114 (('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters'))
-                           550 BUILD_CONST_KEY_MAP      6
-                           552 RETURN_VALUE
+                           430 LOAD_METHOD              3 (get)
+                           452 LOAD_CONST             111 ('keywords')
+                           454 BUILD_LIST               0
+                           456 PRECALL                  2
+                           460 CALL                     2
+               
+               156         470 LOAD_DEREF               0 (search)
+                           472 LOAD_ATTR                4 (exclusion)
+                           482 LOAD_METHOD              3 (get)
+                           504 LOAD_CONST             111 ('keywords')
+                           506 BUILD_LIST               0
+                           508 PRECALL                  2
+                           512 CALL                     2
+               
+               157         522 LOAD_DEREF               0 (search)
+                           524 LOAD_ATTR                2 (inclusion)
+                           534 LOAD_METHOD              3 (get)
+                           556 LOAD_CONST             112 ('employees_range')
+                           558 BUILD_LIST               0
+                           560 PRECALL                  2
+                           564 CALL                     2
+               
+               158         574 PUSH_NULL
+                           576 LOAD_FAST                1 (_ownership_filter)
+                           578 PRECALL                  0
+                           582 CALL                     0
+               
+               160         592 PUSH_NULL
+                           594 LOAD_FAST                2 (_hq_include)
+                           596 PRECALL                  0
+                           600 CALL                     0
+               
+               161         610 PUSH_NULL
+                           612 LOAD_FAST                3 (_hq_exclude)
+                           614 PRECALL                  0
+                           618 CALL                     0
+               
+               159         628 LOAD_CONST             113 (('include', 'exclude'))
+                           630 BUILD_CONST_KEY_MAP      2
+               
+               153         632 LOAD_CONST             114 (('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters'))
+                           634 BUILD_CONST_KEY_MAP      6
+                           636 RETURN_VALUE
                consts
                   None
                   'AL'
                   'Alabama'
                   'AK'
                   'Alaska'
                   'AZ'
@@ -914,22 +939,22 @@
                         000000000000007c00a6010000ab01000000000000000074030000000000
                         000000000089016a020000000000000000a0030000000000000000000000
                         00000000000000000064026700a6020000ab020000000000000000a60100
                         00ab0100000000000000007a0a0000a6010000ab01000000000000000053
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     124           2 RESUME                   0
+                     125           2 RESUME                   0
                      
-                     126           4 BUILD_LIST               0
+                     127           4 BUILD_LIST               0
                                    6 LOAD_CONST               1 (('bootstrapped', 'investor_backed', 'public', 'public_subsidiary', 'private_subsidiary', 'private_equity', 'private_equity_add_on'))
                                    8 LIST_EXTEND              1
                                   10 STORE_FAST               0 (OWNERSHIP)
                      
-                     135          12 LOAD_GLOBAL              1 (NULL + list)
+                     136          12 LOAD_GLOBAL              1 (NULL + list)
                                   24 LOAD_GLOBAL              3 (NULL + set)
                                   36 LOAD_FAST                0 (OWNERSHIP)
                                   38 PRECALL                  1
                                   42 CALL                     1
                                   52 LOAD_GLOBAL              3 (NULL + set)
                                   64 LOAD_DEREF               1 (search)
                                   66 LOAD_ATTR                2 (exclusion)
@@ -950,15 +975,15 @@
                         'ownership'
                      names      ('list', 'set', 'exclusion', 'get')
                      varnames   ('OWNERSHIP',)
                      freevars   ('search',)
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_ownership_filter'
-                     firstlineno 124
+                     firstlineno 125
                      lnotab 0x04020809
                   code
                      argcount  : 0
                      nlocals   : 3
                      stacksize : 6
                      flags     : 19
                      code
@@ -969,202 +994,202 @@
                         00000001008c2089056a000000000000000000a001000000000000000000
                         000000000000000000000064026700a6020000ab02000000000000000044
                         005d1f7d027c00a002000000000000000000000000000000000000000064
                         0289037c02190000000000000000006901a6010000ab0100000000000000
                         0001008c207c005300
                                    0 COPY_FREE_VARS           3
                      
-                     137           2 RESUME                   0
+                     138           2 RESUME                   0
                      
-                     138           4 BUILD_LIST               0
+                     139           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (include)
                      
-                     139           8 LOAD_DEREF               5 (search)
+                     140           8 LOAD_DEREF               5 (search)
                                   10 LOAD_ATTR                0 (inclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('state')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 GET_ITER
                              >>   62 FOR_ITER                31 (to 126)
                                   64 STORE_FAST               1 (state)
                      
-                     141          66 LOAD_FAST                0 (include)
+                     142          66 LOAD_FAST                0 (include)
                                   68 LOAD_METHOD              2 (append)
                                   90 LOAD_CONST               1 ('state')
                                   92 LOAD_DEREF               4 (STATES)
                                   94 LOAD_FAST                1 (state)
                                   96 BINARY_SUBSCR
                                  106 BUILD_MAP                1
                                  108 PRECALL                  1
                                  112 CALL                     1
                                  122 POP_TOP
                                  124 JUMP_BACKWARD           32 (to 62)
                      
-                     142     >>  126 LOAD_DEREF               5 (search)
+                     143     >>  126 LOAD_DEREF               5 (search)
                                  128 LOAD_ATTR                0 (inclusion)
                                  138 LOAD_METHOD              1 (get)
                                  160 LOAD_CONST               2 ('country')
                                  162 BUILD_LIST               0
                                  164 PRECALL                  2
                                  168 CALL                     2
                                  178 GET_ITER
                              >>  180 FOR_ITER                31 (to 244)
                                  182 STORE_FAST               2 (country)
                      
-                     143         184 LOAD_FAST                0 (include)
+                     144         184 LOAD_FAST                0 (include)
                                  186 LOAD_METHOD              2 (append)
                                  208 LOAD_CONST               2 ('country')
                                  210 LOAD_DEREF               3 (COUNTRIES)
                                  212 LOAD_FAST                2 (country)
                                  214 BINARY_SUBSCR
                                  224 BUILD_MAP                1
                                  226 PRECALL                  1
                                  230 CALL                     1
                                  240 POP_TOP
                                  242 JUMP_BACKWARD           32 (to 180)
                      
-                     144     >>  244 LOAD_FAST                0 (include)
+                     145     >>  244 LOAD_FAST                0 (include)
                                  246 RETURN_VALUE
                      consts
                         None
                         'state'
                         'country'
                      names      ('inclusion', 'get', 'append')
                      varnames   ('include', 'state', 'country')
                      freevars   ('COUNTRIES', 'STATES', 'search')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_include'
-                     firstlineno 137
+                     firstlineno 138
                      lnotab 0x040104013a023c013a013c01
                   code
                      argcount  : 0
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007d0089026a000000000000000000a00100000000000000
                         0000000000000000000000000064016700a6020000ab0200000000000000
                         0044005d197d017c00a00200000000000000000000000000000000000000
                         0064017c016901a6010000ab01000000000000000001008c1a7c005300
                                    0 COPY_FREE_VARS           1
                      
-                     146           2 RESUME                   0
+                     147           2 RESUME                   0
                      
-                     147           4 BUILD_LIST               0
+                     148           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (exclude)
                      
-                     148           8 LOAD_DEREF               2 (search)
+                     149           8 LOAD_DEREF               2 (search)
                                   10 LOAD_ATTR                0 (exclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('state')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 GET_ITER
                              >>   62 FOR_ITER                25 (to 114)
                                   64 STORE_FAST               1 (state)
                      
-                     149          66 LOAD_FAST                0 (exclude)
+                     150          66 LOAD_FAST                0 (exclude)
                                   68 LOAD_METHOD              2 (append)
                                   90 LOAD_CONST               1 ('state')
                                   92 LOAD_FAST                1 (state)
                                   94 BUILD_MAP                1
                                   96 PRECALL                  1
                                  100 CALL                     1
                                  110 POP_TOP
                                  112 JUMP_BACKWARD           26 (to 62)
                      
-                     150     >>  114 LOAD_FAST                0 (exclude)
+                     151     >>  114 LOAD_FAST                0 (exclude)
                                  116 RETURN_VALUE
                      consts
                         None
                         'state'
                      names      ('exclusion', 'get', 'append')
                      varnames   ('exclude', 'state')
                      freevars   ('search',)
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_exclude'
-                     firstlineno 146
+                     firstlineno 147
                      lnotab 0x040104013a013001
                   'any'
                   'keywords'
                   'employees_range'
                   ('include', 'exclude')
                   ('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters')
-               names      ('dict', 'list', 'inclusion', 'exclusion')
+               names      ('dict', 'list', 'inclusion', 'get', 'exclusion')
                varnames   ('search', '_ownership_filter', '_hq_include', '_hq_exclude')
                freevars   ()
                cellvars   ('search', 'COUNTRIES', 'STATES')
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       '_get_api_filter'
-               firstlineno 63
+               firstlineno 64
                lnotab
                   0x0801020104ff020204fe020304fd020404fc020504fb020604fa020704
                   f9020804f8020904f7020a04f6020b04f5020c04f4020d04f3020e04f202
                   0f04f1021004f0021104ef041204ee021304ed021404ec021504eb021604
                   ea021704e9021804e8021904e7021a04e6021b04e5021c04e4021d04e302
                   1e04e2021f04e1022004e0022104df022204de062304dd022404dc022504
                   db022604da022704d9022804d8022904d7022a04d6022b04d5022c04d402
                   2d04d3022e04d2022f04d1023004d0023104cf023204ce06360201020102
-                  0102fc06071a0d1e091a0702011801180118011202120112fe04fa
+                  0102fc06071a0d1e091a0702013401340134011202120112fe04fa
             None
          names      ('__name__', '__module__', '__qualname__', 'os', 'getenv', 'HEADERS', 'str', 'Search', 'list', 'find_similar', 'dict', 'find_by_criteria', 'enrich', '_get_api_filter')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'GrataWrapper'
          firstlineno 10
-         lnotab 0x0a021e0102fe06050603141110121009
+         lnotab 0x0a021e0102fe0605060314111012100a
       'GrataWrapper'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a026401650364026504640365056606640484045a
             0664026504640365056604640584045a0764016503640365056604640684
             045a0864075300
-         165           0 RESUME                   0
+         166           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SourceScrubWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-         166          10 LOAD_CONST               1 ('domain')
+         167          10 LOAD_CONST               1 ('domain')
                       12 LOAD_NAME                3 (str)
                       14 LOAD_CONST               2 ('search')
                       16 LOAD_NAME                4 (Search)
                       18 LOAD_CONST               3 ('return')
                       20 LOAD_NAME                5 (dict)
                       22 BUILD_TUPLE              6
-                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 166>)
+                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 167>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               6 (find_similar)
          
-         169          30 LOAD_CONST               2 ('search')
+         170          30 LOAD_CONST               2 ('search')
                       32 LOAD_NAME                4 (Search)
                       34 LOAD_CONST               3 ('return')
                       36 LOAD_NAME                5 (dict)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 169>)
+                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 170>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               7 (find_by_criteria)
          
-         172          46 LOAD_CONST               1 ('domain')
+         173          46 LOAD_CONST               1 ('domain')
                       48 LOAD_NAME                3 (str)
                       50 LOAD_CONST               3 ('return')
                       52 LOAD_NAME                5 (dict)
                       54 BUILD_TUPLE              4
-                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 172>)
+                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 173>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               8 (enrich)
                       62 LOAD_CONST               7 (None)
                       64 RETURN_VALUE
          consts
             'SourceScrubWrapper'
             'domain'
@@ -1172,79 +1197,79 @@
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               166           0 RESUME                   0
+               167           0 RESUME                   0
                
-               167           2 LOAD_CONST               0 (None)
+               168           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain', 'search')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
-               firstlineno 166
+               firstlineno 167
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               169           0 RESUME                   0
+               170           0 RESUME                   0
                
-               170           2 LOAD_CONST               0 (None)
+               171           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('search',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
-               firstlineno 169
+               firstlineno 170
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               172           0 RESUME                   0
+               173           0 RESUME                   0
                
-               173           2 LOAD_CONST               0 (None)
+               174           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 172
+               firstlineno 173
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'str', 'Search', 'dict', 'find_similar', 'find_by_criteria', 'enrich')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'SourceScrubWrapper'
-         firstlineno 165
+         firstlineno 166
          lnotab 0x0a0114031003
       'SourceScrubWrapper'
    names      ('gandai', 'query', 'gandai.models', 'Search', 'requests', 'os', 'dotenv', 'load_dotenv', 'GrataWrapper', 'SourceScrubWrapper')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c01080108010c0214031a7f001c
+   lnotab 0x00ff02010c010c01080108010c0214031a7f001d
```

### Comparing `gandai-1.1.7/gandai/auth.py` & `gandai-1.1.8/gandai/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from hashlib import md5
 from time import time
 import os
 from twilio.rest import Client
 
 # from gandai.models.User import user_exists # create_user
 
-# ds = Cloudstore()
+from gandai.datastore import Cloudstore
+
+
+ds = Cloudstore()
 twilio_client = Client(os.getenv("TWILIO_APP"), os.getenv("TWILIO_TOKEN"))
 
 
 @dataclass
 class Auth:
     key: str = field(init=False)
     phone: str
@@ -38,26 +41,25 @@
     print(f"Login Sent to {auth.phone}")
 
 
 def send_code(phone: str) -> None:
     # Event.create(actor_key=phone)
     auth_code = str(random.randint(100000, 999999))
     auth = Auth(phone=phone, code=auth_code)
-    # ds[auth.key] = asdict(auth)
+    ds[auth.key] = asdict(auth)
     _send_code(auth)
 
 
 def authenticate(code: str) -> Auth:
-    return None
-    # keys = ds.keys("auth/")[1::]
-    # df = pd.DataFrame(ds.load_async(keys))
-    # df = df[df["expires"] > int(time())]
-    # df = df[df["code"] == code]
-    # if len(df) > 0:
-    #     # could parse to Auth and back to dict
-    #     return df.to_dict(orient="records")[0]
-    # else:
-    #     return None
+    keys = ds.keys("auth/")[1::]
+    df = pd.DataFrame(ds.load_async(keys))
+    df = df[df["expires"] > int(time())]
+    df = df[df["code"] == code]
+    if len(df) > 0:
+        # could parse to Auth and back to dict
+        return df.to_dict(orient="records")[0]
+    else:
+        return None
 
 
 def validate(token: str) -> bool:
     pass
```

### Comparing `gandai-1.1.7/gandai/datastore.py` & `gandai-1.1.8/gandai/datastore.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/db.py` & `gandai-1.1.8/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/main.py` & `gandai-1.1.8/gandai/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import pandas as pd
 from dacite import from_dict
 from dataclasses import dataclass, field
-
+from concurrent.futures import ThreadPoolExecutor
 
 from gandai.models import Event, Company, Checkpoint
 from gandai import query
 
 from gandai.sources import GrataWrapper as grata
 
 
-def process_event(e: Event) -> None:
+def process_event(event_id: int) -> None:
+    """
+    May trigger additional targets adding to inbox, or something else
+    (e.g. a notification)
+    """
 
     def _insert_companies(companies: list, existing_domains: list) -> None:
         # rewrite this in less db txns
         for company in companies:
             if company.get("domain") is None:
                 print(f"Missing domain: {company}. Skipping")
                 continue
@@ -34,71 +38,67 @@
                     search_uid=search_uid,
                     domain=company.get("domain"),
                     actor_key="grata",
                     type="create",
                 )
             )
 
+    # sets up better to do this threaded
+    e = query.find_event_by_id(event_id)
     search_uid = e.search_uid
     if e.type == "create":
         pass
     elif e.type == "advance":
         # enrich the company
         company = query.find_company_by_domain(e.domain)
         # might consider a check here to see if the company is already enriched
         resp = grata.enrich(company.domain)
         if resp.get("status") == 404:
             print(f"{company} not found")
         else:
             print(resp)
             company.name = resp.get("name")
             company.description = resp.get("description")
-            company.meta = {**company.meta, **resp} # merge 3.5+
+            company.meta = {**company.meta, **resp}  # merge 3.5+
             query.update_company(company)
 
     elif e.type == "validate":
         search = query.find_search_by_uid(search_uid)
         _insert_companies(
-            companies=grata.find_similar(domain=e.domain, search=search), 
-            existing_domains=query.target(search_uid=search_uid)["domain"].tolist()
+            companies=grata.find_similar(domain=e.domain, search=search),
+            existing_domains=query.target(search_uid=search_uid)["domain"].tolist(),
         )
     elif e.type == "send":
         pass
     elif e.type == "accept":
         pass
     elif e.type == "reject":
         pass
     elif e.type == "conflict":
         pass
     elif e.type == "criteria":
         print("criteria search here we gooo")
         search = query.find_search_by_uid(search_uid)
         _insert_companies(
-            companies=grata.find_by_criteria(search), 
-            existing_domains=query.target(search_uid=search_uid)["domain"].tolist()
+            companies=grata.find_by_criteria(search),
+            existing_domains=query.target(search_uid=search_uid)["domain"].tolist(),
         )
 
     # finally, record we processed the event
     query.insert_checkpoint(Checkpoint(event_id=e.id))
     print(f"processed: {e}")
 
 
 def process_events(search_uid: int) -> int:
     """
     Process all events for a given search
-    Could tidy
     """
-    events = []
 
-    for event in query.event(search_uid).to_dict(orient="records"):
-        event = from_dict(Event, event)
-        events.append(event)
-
-    checkpoints = query.checkpoint()
-    print(checkpoints)
-    processed_count = 0
-    for e in events:
-        if e.id not in checkpoints["event_id"]:
-            process_event(e)
-            processed_count += 1
+    events = query.event(search_uid=search_uid)
+    checkpoints = query.checkpoint(search_uid=search_uid)
 
-    return processed_count
+    q = list(set(events["id"].tolist()) - set(checkpoints["event_id"].tolist()))
+    
+    with ThreadPoolExecutor(max_workers=4) as executor:
+        executor.map(process_event, q)
+    
+    return len(q)
```

### Comparing `gandai-1.1.7/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.1.8/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x8a546064 (Sun May 14 03:24:58 2023 UTC)
-files sz: 3252
+moddate:  0x391c6164 (Sun May 14 17:36:57 2023 UTC)
+files sz: 3257
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -47,41 +47,41 @@
                 50 LOAD_ATTR                7 (DataFrame)
    
      8          60 BUILD_TUPLE              2
                 62 LOAD_CONST               6 (<code object dealcloud_company_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 8>)
                 64 MAKE_FUNCTION            5 (defaults, annotations)
                 66 STORE_NAME               8 (dealcloud_company_query)
    
-    33          68 LOAD_CONST              13 (('data/Engagement_05132023.xlsx',))
-                70 LOAD_CONST               8 (<code object dealcloud_engagements, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 33>)
+    35          68 LOAD_CONST              13 (('data/Engagement_05132023.xlsx',))
+                70 LOAD_CONST               8 (<code object dealcloud_engagements, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 35>)
                 72 MAKE_FUNCTION            1 (defaults)
                 74 STORE_NAME               9 (dealcloud_engagements)
    
-    54          76 LOAD_CONST               9 (<code object migrate_engagements, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 54>)
+    56          76 LOAD_CONST               9 (<code object migrate_engagements, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 56>)
                 78 MAKE_FUNCTION            0
                 80 STORE_NAME              10 (migrate_engagements)
    
-    88          82 LOAD_CONST              10 (<code object main, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 88>)
+    89          82 LOAD_CONST              10 (<code object main, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 89>)
                 84 MAKE_FUNCTION            0
                 86 STORE_NAME              11 (main)
    
-    92          88 LOAD_NAME               12 (__name__)
+    93          88 LOAD_NAME               12 (__name__)
                 90 LOAD_CONST              11 ('__main__')
                 92 COMPARE_OP               2 (==)
                 98 POP_JUMP_FORWARD_IF_FALSE    12 (to 124)
    
-    93         100 PUSH_NULL
+    94         100 PUSH_NULL
                102 LOAD_NAME               11 (main)
                104 PRECALL                  0
                108 CALL                     0
                118 POP_TOP
                120 LOAD_CONST               3 (None)
                122 RETURN_VALUE
    
-    92     >>  124 LOAD_CONST               3 (None)
+    93     >>  124 LOAD_CONST               3 (None)
                126 RETURN_VALUE
    consts
       0
       ('query',)
       ('Search',)
       None
       '/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx'
@@ -174,24 +174,26 @@
          
           21         346 LOAD_FAST                2 (df)
                      348 LOAD_CONST               8 ('days_since_contact')
                      350 STORE_SUBSCR
          
           24         354 LOAD_FAST                2 (df)
                      356 LOAD_METHOD              7 (rename)
-                     378 LOAD_CONST              10 ('name')
+         
+          25         378 LOAD_CONST              10 ('name')
                      380 LOAD_CONST              11 ('description')
                      382 LOAD_CONST              12 (('company_name', 'business_description'))
                      384 BUILD_CONST_KEY_MAP      2
-                     386 KW_NAMES                13
+         
+          24         386 KW_NAMES                13
                      388 PRECALL                  1
                      392 CALL                     1
                      402 STORE_FAST               2 (df)
          
-          30         404 LOAD_FAST                2 (df)
+          32         404 LOAD_FAST                2 (df)
                      406 RETURN_VALUE
          consts
             None
             'dealcloud_company_query'
             'return'
             code
                argcount  : 1
@@ -341,15 +343,15 @@
          names      ('print', 'str', 'pd', 'read_excel', 'columns', 'dropna', 'apply', 'rename')
          varnames   ('fp', '_get_domain', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
          name       'dealcloud_company_query'
          firstlineno 8
-         lnotab 0x02031e02160428012c01160160025aff08033206
+         lnotab 0x02031e02160428012c01160160025aff0803180108ff1208
       'data/Engagement_05132023.xlsx'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -373,174 +375,174 @@
             00000000000000a00b000000000000000000000000000000000000000067
             00640da201a6010000ab0100000000000000000f00190000000000000000
             00a00c0000000000000000000000000000000000000000640eac0fa60100
             00ab0100000000000000007d017c017c0164051900000000000000000064
             106b000000000019000000000000000000a00c0000000000000000000000
             000000000000000000640eac0fa6010000ab0100000000000000007d017c
             015300
-          33           0 RESUME                   0
+          35           0 RESUME                   0
          
-          34           2 LOAD_GLOBAL              1 (NULL + pd)
+          36           2 LOAD_GLOBAL              1 (NULL + pd)
                       14 LOAD_ATTR                1 (read_excel)
                       24 LOAD_FAST                0 (fp)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               1 (df)
          
-          35          42 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 35>)
+          37          42 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 37>)
                       44 MAKE_FUNCTION            0
                       46 LOAD_FAST                1 (df)
                       48 LOAD_ATTR                2 (columns)
                       58 GET_ITER
                       60 PRECALL                  0
                       64 CALL                     0
                       74 LOAD_FAST                1 (df)
                       76 STORE_ATTR               2 (columns)
          
-          36          86 LOAD_FAST                1 (df)
+          38          86 LOAD_FAST                1 (df)
                       88 LOAD_CONST               2 ('dealcloud_id')
                       90 BINARY_SUBSCR
                      100 LOAD_METHOD              3 (astype)
                      122 LOAD_GLOBAL              8 (str)
                      134 PRECALL                  1
                      138 CALL                     1
                      148 LOAD_FAST                1 (df)
                      150 LOAD_CONST               2 ('dealcloud_id')
                      152 STORE_SUBSCR
          
-          37         156 LOAD_CONST               2 ('dealcloud_id')
+          39         156 LOAD_CONST               2 ('dealcloud_id')
                      158 LOAD_FAST                1 (df)
                      160 LOAD_ATTR                2 (columns)
                      170 CONTAINS_OP              0
                      172 POP_JUMP_FORWARD_IF_TRUE     2 (to 178)
                      174 LOAD_ASSERTION_ERROR
                      176 RAISE_VARARGS            1
          
-          38     >>  178 LOAD_GLOBAL              1 (NULL + pd)
+          40     >>  178 LOAD_GLOBAL              1 (NULL + pd)
                      190 LOAD_ATTR                5 (to_datetime)
                      200 LOAD_CONST               3 ('today')
                      202 PRECALL                  1
                      206 CALL                     1
                      216 STORE_FAST               2 (today)
          
-          39         218 LOAD_FAST                2 (today)
+          41         218 LOAD_FAST                2 (today)
                      220 LOAD_GLOBAL              1 (NULL + pd)
                      232 LOAD_ATTR                5 (to_datetime)
                      242 LOAD_FAST                1 (df)
                      244 LOAD_CONST               4 ('modified_date')
                      246 BINARY_SUBSCR
                      256 PRECALL                  1
                      260 CALL                     1
                      270 BINARY_OP               10 (-)
                      274 LOAD_ATTR                6 (dt)
                      284 LOAD_ATTR                7 (days)
                      294 LOAD_FAST                1 (df)
                      296 LOAD_CONST               5 ('modified_days_ago')
                      298 STORE_SUBSCR
          
-          40         302 LOAD_CONST               6 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 40>)
+          42         302 LOAD_CONST               6 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 42>)
                      304 MAKE_FUNCTION            0
                      306 LOAD_FAST                1 (df)
                      308 LOAD_ATTR                2 (columns)
                      318 GET_ITER
                      320 PRECALL                  0
                      324 CALL                     0
                      334 STORE_FAST               3 (date_cols)
          
-          41         336 LOAD_FAST                3 (date_cols)
+          43         336 LOAD_FAST                3 (date_cols)
                      338 GET_ITER
                  >>  340 FOR_ITER                33 (to 408)
                      342 STORE_FAST               4 (col)
          
-          42         344 LOAD_FAST                1 (df)
+          44         344 LOAD_FAST                1 (df)
                      346 LOAD_FAST                4 (col)
                      348 BINARY_SUBSCR
                      358 LOAD_METHOD              8 (apply)
-                     380 LOAD_CONST               7 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 42>)
+                     380 LOAD_CONST               7 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py", line 44>)
                      382 MAKE_FUNCTION            0
                      384 PRECALL                  1
                      388 CALL                     1
                      398 LOAD_FAST                1 (df)
                      400 LOAD_FAST                4 (col)
                      402 STORE_SUBSCR
                      406 JUMP_BACKWARD           34 (to 340)
          
-          43     >>  408 LOAD_FAST                1 (df)
+          45     >>  408 LOAD_FAST                1 (df)
                      410 LOAD_METHOD              9 (dropna)
                      432 LOAD_CONST               8 ('engagement_name')
                      434 BUILD_LIST               1
                      436 KW_NAMES                 9
                      438 PRECALL                  1
                      442 CALL                     1
                      452 STORE_FAST               1 (df)
          
-          44         454 LOAD_FAST                1 (df)
+          46         454 LOAD_FAST                1 (df)
                      456 LOAD_METHOD             10 (sort_values)
                      478 LOAD_CONST               4 ('modified_date')
                      480 LOAD_CONST              10 (False)
                      482 KW_NAMES                11
                      484 PRECALL                  2
                      488 CALL                     2
                      498 STORE_FAST               1 (df)
          
-          45         500 LOAD_FAST                1 (df)
+          47         500 LOAD_FAST                1 (df)
          
-          46         502 LOAD_FAST                1 (df)
+          48         502 LOAD_FAST                1 (df)
                      504 LOAD_CONST              12 ('status')
                      506 BINARY_SUBSCR
                      516 LOAD_METHOD             11 (isin)
          
-          47         538 BUILD_LIST               0
+          49         538 BUILD_LIST               0
                      540 LOAD_CONST              13 (('Lost Pre-Mandate', 'Completed Engagement', 'Dead Post-Mandate'))
                      542 LIST_EXTEND              1
          
-          46         544 PRECALL                  1
+          48         544 PRECALL                  1
                      548 CALL                     1
                      558 UNARY_INVERT
          
-          45         560 BINARY_SUBSCR
+          47         560 BINARY_SUBSCR
          
-          49         570 LOAD_METHOD             12 (reset_index)
+          51         570 LOAD_METHOD             12 (reset_index)
                      592 LOAD_CONST              14 (True)
                      594 KW_NAMES                15
                      596 PRECALL                  1
                      600 CALL                     1
          
-          45         610 STORE_FAST               1 (df)
+          47         610 STORE_FAST               1 (df)
          
-          50         612 LOAD_FAST                1 (df)
+          52         612 LOAD_FAST                1 (df)
                      614 LOAD_FAST                1 (df)
                      616 LOAD_CONST               5 ('modified_days_ago')
                      618 BINARY_SUBSCR
                      628 LOAD_CONST              16 (365)
                      630 COMPARE_OP               0 (<)
                      636 BINARY_SUBSCR
                      646 LOAD_METHOD             12 (reset_index)
                      668 LOAD_CONST              14 (True)
                      670 KW_NAMES                15
                      672 PRECALL                  1
                      676 CALL                     1
                      686 STORE_FAST               1 (df)
          
-          51         688 LOAD_FAST                1 (df)
+          53         688 LOAD_FAST                1 (df)
                      690 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 19
                code
                   0x970067007c005d3e7d017c01a000000000000000000000000000000000
                   0000000000a6000000ab000000000000000000a001000000000000000000
                   000000000000000000000064006401a6020000ab020000000000000000a0
                   01000000000000000000000000000000000000000064026403a6020000ab
                   02000000000000000091028c3f5300
-                35           0 RESUME                   0
+                37           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                62 (to 132)
                              8 STORE_FAST               1 (col)
                             10 LOAD_FAST                1 (col)
                             12 LOAD_METHOD              0 (lower)
                             34 PRECALL                  0
@@ -565,30 +567,30 @@
                   ''
                names      ('lower', 'replace')
                varnames   ('.0', 'col')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
                name       '<listcomp>'
-               firstlineno 35
+               firstlineno 37
                lnotab 0x
             'dealcloud_id'
             'today'
             'modified_date'
             'modified_days_ago'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
                   0x970067007c005d197d017c01a000000000000000000000000000000000
                   00000000006400a6010000ab010000000000000000af177c0191028c1a53
                   00
-                40           0 RESUME                   0
+                42           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                25 (to 58)
                              8 STORE_FAST               1 (col)
                             10 LOAD_FAST                1 (col)
                             12 LOAD_METHOD              0 (endswith)
                             34 LOAD_CONST               0 ('_date')
@@ -603,25 +605,25 @@
                   '_date'
                names      ('endswith',)
                varnames   ('.0', 'col')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
                name       '<listcomp>'
-               firstlineno 40
+               firstlineno 42
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   00640164028502190000000000000000005300
-                42           0 RESUME                   0
+                44           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + str)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_CONST               1 (0)
                             32 LOAD_CONST               2 (10)
                             34 BUILD_SLICE              2
@@ -633,15 +635,15 @@
                   10
                names      ('str',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
                name       '<lambda>'
-               firstlineno 42
+               firstlineno 44
                lnotab 0x
             'engagement_name'
             ('subset',)
             False
             ('ascending',)
             'status'
             ('Lost Pre-Mandate', 'Completed Engagement', 'Dead Post-Mandate')
@@ -650,15 +652,15 @@
             365
          names      ('pd', 'read_excel', 'columns', 'astype', 'str', 'to_datetime', 'dt', 'days', 'apply', 'dropna', 'sort_values', 'isin', 'reset_index')
          varnames   ('fp', 'df', 'today', 'date_cols', 'col')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
          name       'dealcloud_engagements'
-         firstlineno 33
+         firstlineno 35
          lnotab
             0x020128012c0146011601280154012201080140012e012e010201240106
             ff10ff0a0428fc02054c01
       code
          argcount  : 0
          nlocals   : 5
          stacksize : 11
@@ -678,142 +680,142 @@
             000000000044005d627d03740f0000000000000000000074110000000000
             00000000007c03640d19000000000000000000a6010000ab010000000000
             0000007c036406190000000000000000007c03640e190000000000000000
             007c03640f670164106411670264129c026405641364149c02ac15a60600
             00ab0600000000000000007d047413000000000000000000007c04a60100
             00ab01000000000000000001007415000000000000000000006a0b000000
             00000000007c04a6010000ab01000000000000000001008c6364005300
-          54           0 RESUME                   0
+          56           0 RESUME                   0
          
-          55           2 LOAD_GLOBAL              1 (NULL + dealcloud_engagements)
+          57           2 LOAD_GLOBAL              1 (NULL + dealcloud_engagements)
          
-          56          14 LOAD_CONST               1 ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Engagement_05132023.xlsx')
+          58          14 LOAD_CONST               1 ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Engagement_05132023.xlsx')
          
-          55          16 PRECALL                  1
+          57          16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               0 (engagements)
          
-          58          32 LOAD_GLOBAL              3 (NULL + dealcloud_company_query)
+          60          32 LOAD_GLOBAL              3 (NULL + dealcloud_company_query)
          
-          59          44 LOAD_CONST               2 ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx')
+          61          44 LOAD_CONST               2 ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx')
          
-          58          46 PRECALL                  1
+          60          46 PRECALL                  1
                       50 CALL                     1
                       60 STORE_FAST               1 (companies)
          
-          62          62 LOAD_FAST                1 (companies)
+          64          62 LOAD_FAST                1 (companies)
                       64 LOAD_FAST                1 (companies)
                       66 LOAD_CONST               3 ('name')
                       68 BINARY_SUBSCR
                       78 LOAD_METHOD              2 (isin)
                      100 LOAD_FAST                0 (engagements)
                      102 LOAD_CONST               4 ('client')
                      104 BINARY_SUBSCR
                      114 PRECALL                  1
                      118 CALL                     1
                      128 BINARY_SUBSCR
                      138 STORE_FAST               2 (clients)
          
-          63         140 LOAD_FAST                2 (clients)
+          65         140 LOAD_FAST                2 (clients)
                      142 LOAD_METHOD              3 (rename)
                      164 LOAD_CONST               5 ('domain')
                      166 LOAD_CONST               6 ('client_domain')
                      168 BUILD_MAP                1
                      170 KW_NAMES                 7
                      172 PRECALL                  1
                      176 CALL                     1
          
-          64         186 LOAD_CONST               3 ('name')
+          66         186 LOAD_CONST               3 ('name')
                      188 LOAD_CONST               6 ('client_domain')
                      190 BUILD_LIST               2
          
-          63         192 BINARY_SUBSCR
+          65         192 BINARY_SUBSCR
                      202 STORE_FAST               2 (clients)
          
-          67         204 LOAD_FAST                0 (engagements)
+          69         204 LOAD_FAST                0 (engagements)
                      206 LOAD_METHOD              4 (merge)
          
-          68         228 LOAD_FAST                2 (clients)
+          70         228 LOAD_FAST                2 (clients)
                      230 LOAD_CONST               4 ('client')
                      232 LOAD_CONST               3 ('name')
                      234 LOAD_CONST               8 ('left')
          
-          67         236 KW_NAMES                 9
+          69         236 KW_NAMES                 9
                      238 PRECALL                  4
                      242 CALL                     4
                      252 STORE_FAST               0 (engagements)
          
-          71         254 LOAD_FAST                0 (engagements)
+          73         254 LOAD_FAST                0 (engagements)
                      256 LOAD_METHOD              5 (fillna)
                      278 LOAD_CONST              10 ('')
                      280 PRECALL                  1
                      284 CALL                     1
                      294 LOAD_METHOD              6 (to_dict)
                      316 LOAD_CONST              11 ('records')
                      318 KW_NAMES                12
                      320 PRECALL                  1
                      324 CALL                     1
                      334 GET_ITER
                  >>  336 FOR_ITER                98 (to 534)
                      338 STORE_FAST               3 (engagement)
          
-          72         340 LOAD_GLOBAL             15 (NULL + Search)
+          74         340 LOAD_GLOBAL             15 (NULL + Search)
          
-          73         352 LOAD_GLOBAL             17 (NULL + int)
+          75         352 LOAD_GLOBAL             17 (NULL + int)
                      364 LOAD_FAST                3 (engagement)
                      366 LOAD_CONST              13 ('dealcloud_id')
                      368 BINARY_SUBSCR
                      378 PRECALL                  1
                      382 CALL                     1
          
-          74         392 LOAD_FAST                3 (engagement)
+          76         392 LOAD_FAST                3 (engagement)
                      394 LOAD_CONST               6 ('client_domain')
                      396 BINARY_SUBSCR
          
-          75         406 LOAD_FAST                3 (engagement)
+          77         406 LOAD_FAST                3 (engagement)
                      408 LOAD_CONST              14 ('engagement_name')
                      410 BINARY_SUBSCR
          
-          76         420 LOAD_FAST                3 (engagement)
+          78         420 LOAD_FAST                3 (engagement)
          
-          78         422 LOAD_CONST              15 ('USA')
+          80         422 LOAD_CONST              15 ('USA')
                      424 BUILD_LIST               1
          
-          79         426 LOAD_CONST              16 (10)
+          81         426 LOAD_CONST              16 (10)
                      428 LOAD_CONST              17 (100)
                      430 BUILD_LIST               2
          
-          77         432 LOAD_CONST              18 (('country', 'employees_range'))
+          79         432 LOAD_CONST              18 (('country', 'employees_range'))
                      434 BUILD_CONST_KEY_MAP      2
          
-          81         436 LOAD_CONST               5 ('domain')
+          83         436 LOAD_CONST               5 ('domain')
                      438 LOAD_CONST              19 ('desc')
                      440 LOAD_CONST              20 (('field', 'order'))
                      442 BUILD_CONST_KEY_MAP      2
          
-          72         444 KW_NAMES                21
+          74         444 KW_NAMES                21
                      446 PRECALL                  6
                      450 CALL                     6
                      460 STORE_FAST               4 (search)
          
-          83         462 LOAD_GLOBAL             19 (NULL + print)
+          85         462 LOAD_GLOBAL             19 (NULL + print)
                      474 LOAD_FAST                4 (search)
                      476 PRECALL                  1
                      480 CALL                     1
                      490 POP_TOP
          
-          84         492 LOAD_GLOBAL             21 (NULL + query)
+          86         492 LOAD_GLOBAL             21 (NULL + query)
                      504 LOAD_ATTR               11 (insert_search)
                      514 LOAD_FAST                4 (search)
                      516 PRECALL                  1
                      520 CALL                     1
                      530 POP_TOP
                      532 JUMP_BACKWARD           99 (to 336)
          
-          71     >>  534 LOAD_CONST               0 (None)
+          73     >>  534 LOAD_CONST               0 (None)
                      536 RETURN_VALUE
          consts
             None
             '/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Engagement_05132023.xlsx'
             '/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx'
             'name'
             'client'
@@ -836,50 +838,50 @@
             ('uid', 'client_domain', 'label', 'meta', 'inclusion', 'sort')
          names      ('dealcloud_engagements', 'dealcloud_company_query', 'isin', 'rename', 'merge', 'fillna', 'to_dict', 'Search', 'int', 'print', 'query', 'insert_search')
          varnames   ('engagements', 'companies', 'clients', 'engagement', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
          name       'migrate_engagements'
-         firstlineno 54
+         firstlineno 56
          lnotab
             0x02010c0102ff10030c0102ff10044e012e0106ff0c04180108ff120456
             010c0128010e010e010202040106fe040408f7120b1e012af3
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab00000000000000000001
             0064005300
-          88           0 RESUME                   0
+          89           0 RESUME                   0
          
-          89           2 LOAD_GLOBAL              1 (NULL + migrate_engagements)
+          90           2 LOAD_GLOBAL              1 (NULL + migrate_engagements)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 POP_TOP
                       30 LOAD_CONST               0 (None)
                       32 RETURN_VALUE
          consts
             None
          names      ('migrate_engagements',)
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
          name       'main'
-         firstlineno 88
+         firstlineno 89
          lnotab 0x0201
       '__main__'
       ('/Users/parker/Development/gandai-workspace/notebooks/2023-05-13/data/Company_05132023.xlsx',)
       ('data/Engagement_05132023.xlsx',)
    names      ('gandai', 'query', 'gandai.models', 'Search', 're', 'pandas', 'pd', 'DataFrame', 'dealcloud_company_query', 'dealcloud_engagements', 'migrate_engagements', 'main', '__name__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/migrations/dealcloud.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c020801080402ff04020cfe08190815062206040c0118
+      0x00ff02010c010c020801080402ff04020cfe081b0815062106040c0118
       ff
```

### Comparing `gandai-1.1.7/gandai/migrations/db_seed.py` & `gandai-1.1.8/gandai/migrations/db_seed.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     actors = {
         "7138248581": "Parker",
         "6508620943": "Gabe",
         "9413500954": "Skye",
         "3102835279": "Chris",
         "5126571681": "Brandon",
         "5125659474": "Jack",
+        "3125740050": "Jim",
         "4805706789": "Eli",
         "grata": "Grata Bot",
         "dealcloud": "DealCloud Bot",
         "chatgpt": "ChatGPT",
     }
 
     for key, name in actors.items():
```

### Comparing `gandai-1.1.7/gandai/migrations/dealcloud.py` & `gandai-1.1.8/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/migrations/sql/schema.sql` & `gandai-1.1.8/gandai/migrations/sql/schema.sql`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     domain VARCHAR(255) REFERENCES company(domain),
     actor_key VARCHAR(255) NOT NULL REFERENCES actor(key),
     type VARCHAR(255) NOT NULL,
     data JSONB DEFAULT '{}'::jsonb,
     created BIGINT NOT NULL DEFAULT FLOOR(EXTRACT(EPOCH FROM NOW()))
 );
 
---ALTER TABLE event ADD CONSTRAINT unique_event_type_domain_search_uid UNIQUE (type, domain, search_uid);
+CREATE INDEX idx_event_search_uid ON event(search_uid);
+ALTER TABLE event ADD CONSTRAINT unique_event_type_domain_search_uid_created UNIQUE (type, domain, search_uid, created);
 
 
 CREATE TABLE IF NOT EXISTS checkpoint (
     id SERIAL PRIMARY KEY,
     event_id INTEGER NOT NULL REFERENCES event(id),
     created BIGINT NOT NULL DEFAULT FLOOR(EXTRACT(EPOCH FROM NOW()))
 );
@@ -57,20 +58,21 @@
     e.id, 
     e.search_uid, 
     e.domain, 
     e.data, 
     e.type AS last_event_type, 
     e.created AS last_event_dt,
     c.name as name,
+    c.uid as dealcloud_id,
     c.description as description,
     c.meta as meta,
-    (c.meta->>'employees')::INTEGER AS employees,
+    (c.meta->>'employees') AS employees,
     (c.meta->>'ownership_status') AS ownership_status,
-    (c.meta->>'social_linkedin') AS linkedin,    
-    (r.data->>'rating')::int AS rating
+    (c.meta->>'linkedin') AS linkedin,    
+    (r.data->>'rating') AS rating
 FROM (
     SELECT 
         domain, 
         MAX(created) AS max_created
     FROM 
         event
     WHERE
```

### Comparing `gandai-1.1.7/gandai/models.py` & `gandai-1.1.8/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.7/gandai/query.py` & `gandai-1.1.8/gandai/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 
 
 import sqlalchemy
 
 from google.cloud.sql.connector import Connector
 from dotenv import load_dotenv
+
 load_dotenv()
 
 from gandai.db import connect_with_connector
 
 db = connect_with_connector()
 
 
@@ -109,48 +110,49 @@
 
 
 ### READS ###
 
 
 def search():
     with db.connect() as conn:
-        result = conn.execute(sqlalchemy.text("SELECT *, meta->>'group' as group FROM search"))
+        result = conn.execute(
+            sqlalchemy.text("SELECT *, meta->>'group' as group FROM search")
+        )
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
     return df
 
 
 def target(search_uid: int, last_event_type: str = None):
     with db.connect() as conn:
         if last_event_type is not None:
             statement = "SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type"
             result = conn.execute(
                 sqlalchemy.text(statement),
                 {"search_uid": search_uid, "last_event_type": last_event_type},
             )
-            
+
         else:
             statement = "SELECT * FROM target WHERE search_uid = :search_uid"
             result = conn.execute(
                 sqlalchemy.text(statement),
                 {"search_uid": search_uid},
             )
-            
+
         targets = pd.DataFrame(result.fetchall(), columns=result.keys())
 
     comments = comment_by_domain(search_uid)
     targets = targets.merge(comments, on="domain", how="left")
-    
+
     # handle sorting
     search = find_search_by_uid(search_uid)
     targets = targets.sort_values(
-        by=search.sort.get("field", "domain"), 
-        ascending=search.sort.get("order") == "asc"
+        by=search.sort.get("field", "domain"),
+        ascending=search.sort.get("order") == "asc",
     )
-    
-    
+
     return targets
 
 
 def target_count(search_uid: int) -> pd.DataFrame:
     with db.connect() as conn:
         statement = """
                 SELECT last_event_type, count(*)
@@ -173,31 +175,35 @@
                 FROM event
                 WHERE search_uid = :search_uid
             """
         result = conn.execute(sqlalchemy.text(statement), {"search_uid": search_uid})
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
     return df
 
+
 def company() -> pd.DataFrame:
     with db.connect() as conn:
         statement = """
                 SELECT *
                 FROM company
             """
         result = conn.execute(sqlalchemy.text(statement))
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
     return df
 
-def checkpoint() -> pd.DataFrame:
+
+def checkpoint(search_uid: int) -> pd.DataFrame:
     with db.connect() as conn:
         statement = """
                 SELECT *
                 FROM checkpoint
+                JOIN event ON checkpoint.event_id = event.id
+                WHERE search_uid = :search_uid
             """
-        result = conn.execute(sqlalchemy.text(statement))
+        result = conn.execute(sqlalchemy.text(statement), {"search_uid": search_uid})
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
     return df
 
 
 def comment_by_domain(search_uid: int) -> pd.DataFrame:
     with db.connect() as conn:
         statement = """
@@ -247,14 +253,29 @@
     if result.rowcount == 0:
         return None
     else:
         obj = dict(zip(result.keys(), result.fetchone()))
         return from_dict(Company, obj)
 
 
+def find_event_by_id(event_id: int) -> Event:
+    with db.connect() as conn:
+        statement = """
+                SELECT *
+                FROM event
+                WHERE id = :event_id
+            """
+        result = conn.execute(sqlalchemy.text(statement), {"event_id": event_id})
+        # obj = dict(zip(result.keys(), result.fetchone()))
+    if result.rowcount == 0:
+        return None
+    else:
+        obj = dict(zip(result.keys(), result.fetchone()))
+        return from_dict(Event, obj)
+
 ### UPDATE ###
 
 
 def update_company(company: Company) -> None:
     with db.connect() as conn:
         statement = """
             UPDATE company
@@ -295,9 +316,7 @@
                 "sort": json.dumps(search.sort),
                 "inclusion": json.dumps(search.inclusion),
                 "exclusion": json.dumps(search.exclusion),
                 "uid": search.uid,
             },
         )
         conn.commit()
-
-
```

### Comparing `gandai-1.1.7/gandai/sources.py` & `gandai-1.1.8/gandai/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     def enrich(domain: str) -> dict:
         response = requests.post(
             "https://search.grata.com/api/v1/enrich/",
             headers=GrataWrapper.HEADERS,
             json={"domain": domain},
         )
         data = response.json()
+        data['linkedin'] = data.get('social_linkedin')
         return data
 
     def _get_api_filter(search: Search) -> dict:
         STATES = {
             "AL": "Alabama",
             "AK": "Alaska",
             "AZ": "Arizona",
```

### Comparing `gandai-1.1.7/gandai.egg-info/SOURCES.txt` & `gandai-1.1.8/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

