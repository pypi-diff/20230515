# Comparing `tmp/ttaken-0.2.0-py3-none-any.whl.zip` & `tmp/ttaken-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1634 bytes, number of entries: 5
--rw-r--r--  2.0 unx      902 b- defN 23-May-15 02:13 ttaken.py
--rw-r--r--  2.0 unx      319 b- defN 23-May-15 02:15 ttaken-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 02:15 ttaken-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-15 02:15 ttaken-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      357 b- defN 23-May-15 02:15 ttaken-0.2.0.dist-info/RECORD
-5 files, 1677 bytes uncompressed, 966 bytes compressed:  42.4%
+Zip file size: 1485 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      532 b- defN 23-May-15 02:31 ttaken.py
+-rw-r--r--  2.0 unx      319 b- defN 23-May-15 02:43 ttaken-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 02:43 ttaken-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-15 02:43 ttaken-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      357 b- defN 23-May-15 02:43 ttaken-0.3.0.dist-info/RECORD
+5 files, 1307 bytes uncompressed, 817 bytes compressed:  37.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: ttaken.py
 Comment: 
 
-Filename: ttaken-0.2.0.dist-info/METADATA
+Filename: ttaken-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: ttaken-0.2.0.dist-info/WHEEL
+Filename: ttaken-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: ttaken-0.2.0.dist-info/top_level.txt
+Filename: ttaken-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ttaken-0.2.0.dist-info/RECORD
+Filename: ttaken-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ttaken.py

```diff
@@ -1,27 +1,20 @@
 #!/usr/local/bin/python3
 
 import logging
 import time
-import socket
 
 """
 This module prints the time taken by a function where it is decorated
 """
 
 def ttaken(logger):
     def decorator(func):
         def wrapper(*args, **kwargs):
             start_time = time.time()
             result = func(*args, **kwargs)
             end_time = time.time()
             elapsed_time = end_time - start_time
-            FORMAT = '%(asctime)s %(clientip)-15s %(hostname)-8s %(message)s'
-            logging.basicConfig(format=FORMAT)
-            ## getting the hostname by socket.gethostname() method
-            hostname = socket.gethostname() 
-            ip_address = socket.gethostbyname(hostname) 
-            d = {'clientip': ip_adress, 'hostname': hostname}
             logger.info(f"func.__name__ took {elapsed_time} seconds to execute!")
             return result
         return wrapper
     return decorator
```

