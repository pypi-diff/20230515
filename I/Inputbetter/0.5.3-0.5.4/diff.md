# Comparing `tmp/Inputbetter-0.5.3-py3-none-any.whl.zip` & `tmp/Inputbetter-0.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1623 bytes, number of entries: 6
+Zip file size: 1703 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       30 b- defN 23-May-14 09:06 Inputbetter/__init__.py
--rw-rw-rw-  2.0 fat      616 b- defN 23-May-15 03:37 Inputbetter/functions.py
--rw-rw-rw-  2.0 fat      151 b- defN 23-May-15 03:37 Inputbetter-0.5.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 03:37 Inputbetter-0.5.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-15 03:37 Inputbetter-0.5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      471 b- defN 23-May-15 03:37 Inputbetter-0.5.3.dist-info/RECORD
-6 files, 1372 bytes uncompressed, 763 bytes compressed:  44.4%
+-rw-rw-rw-  2.0 fat      831 b- defN 23-May-15 04:00 Inputbetter/functions.py
+-rw-rw-rw-  2.0 fat      151 b- defN 23-May-15 04:01 Inputbetter-0.5.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 04:01 Inputbetter-0.5.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-15 04:01 Inputbetter-0.5.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      471 b- defN 23-May-15 04:01 Inputbetter-0.5.4.dist-info/RECORD
+6 files, 1587 bytes uncompressed, 843 bytes compressed:  46.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: Inputbetter/__init__.py
 Comment: 
 
 Filename: Inputbetter/functions.py
 Comment: 
 
-Filename: Inputbetter-0.5.3.dist-info/METADATA
+Filename: Inputbetter-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: Inputbetter-0.5.3.dist-info/WHEEL
+Filename: Inputbetter-0.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: Inputbetter-0.5.3.dist-info/top_level.txt
+Filename: Inputbetter-0.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: Inputbetter-0.5.3.dist-info/RECORD
+Filename: Inputbetter-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Inputbetter/functions.py

```diff
@@ -1,25 +1,28 @@
-def btrinpt(type,k,n):
+def btrinpt(type,user_inpt_display,numberofelements):
+    k=str(user_inpt_display)
+    n=int(numberofelements)
     global mylist
-    mylist=[]
-    if type=="str":
-        for i in range(0,n):
-            ic=str(i)
-            kf=str(k+ic+":")
+    mylist=[]   
+    for i in range(0,n):
+        ic=str(i)
+        kf=str(k+ic+":")
+        if type=="str":
             xu=str(input(kf))
             mylist.append(xu)
-            return mylist    
-    elif type=="int":
-        for j in range(0,n):
-         jc=str(j)
-         kf=str(k+jc+":")
-         xu=int(input(kf))
-         mylist.append(xu)
-         return mylist
-    elif type=="mixed":
-        for l in range(0,n):
-         lc=str(l)
-         kf=str(k+lc+":")
-         xu=input(kf)
-         mylist.append(xu)
-         return mylist
-    
+        elif type == "int":
+            xu=int(input(kf))
+            mylist.append(xu)
+        elif type=="mixed":
+            subtypetext=str(kf+"is this str or int, reply s/i:")
+            subtype=str(input(subtypetext))
+            if subtype=="s":
+                xu=str((input(kf)))
+                mylist.append(xu)
+            if subtype=="i":
+             xu=int(input(kf))
+             mylist.append(xu)
+        else:
+            xu=(input(kf))
+            mylist.append(xu)
+    return mylist
+
```

