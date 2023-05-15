# Comparing `tmp/wiretap-4.2.0-py3-none-any.whl.zip` & `tmp/wiretap-4.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4748 bytes, number of entries: 7
+Zip file size: 4814 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      131 b- defN 23-May-13 15:30 wiretap/__init__.py
 -rw-rw-rw-  2.0 fat      620 b- defN 23-Feb-08 09:16 wiretap/layers.py
--rw-rw-rw-  2.0 fat    12190 b- defN 23-May-13 15:37 wiretap/wiretap.py
--rw-rw-rw-  2.0 fat      244 b- defN 23-May-13 15:49 wiretap-4.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-13 15:49 wiretap-4.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-13 15:49 wiretap-4.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      520 b- defN 23-May-13 15:49 wiretap-4.2.0.dist-info/RECORD
-7 files, 13805 bytes uncompressed, 3830 bytes compressed:  72.3%
+-rw-rw-rw-  2.0 fat    12350 b- defN 23-May-15 08:44 wiretap/wiretap.py
+-rw-rw-rw-  2.0 fat      244 b- defN 23-May-15 08:45 wiretap-4.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 08:45 wiretap-4.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-15 08:45 wiretap-4.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      520 b- defN 23-May-15 08:45 wiretap-4.2.1.dist-info/RECORD
+7 files, 13965 bytes uncompressed, 3896 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: wiretap/layers.py
 Comment: 
 
 Filename: wiretap/wiretap.py
 Comment: 
 
-Filename: wiretap-4.2.0.dist-info/METADATA
+Filename: wiretap-4.2.1.dist-info/METADATA
 Comment: 
 
-Filename: wiretap-4.2.0.dist-info/WHEEL
+Filename: wiretap-4.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: wiretap-4.2.0.dist-info/top_level.txt
+Filename: wiretap-4.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: wiretap-4.2.0.dist-info/RECORD
+Filename: wiretap-4.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wiretap/wiretap.py

```diff
@@ -93,15 +93,15 @@
     return {"args": {key: multi_format(args.get(key, None), args_format) for key in args}}
 
 
 def create_result_details(result: Any | None, result_format: FormatOptions | dict[str, FormatOptions]) -> dict[str, Any]:
     if result_format == NO_DETAILS:
         return {}
 
-    if not result:
+    if result is None:
         return {"result": None}
 
     if isinstance(result_format, dict):
         return {"result": {key: multi_format(result, result_format[key]) for key in result_format}}
 
     return {"result": multi_format(result, result_format)}
 
@@ -264,14 +264,16 @@
                     d[n] = logger
 
         def params(*decoratee_args, **decoratee_kwargs) -> Dict[str, Any]:
             # Zip arg names and their indexes up to the number of args of the decoratee_args.
             arg_pairs = zip(inspect.getfullargspec(decoratee).args, range(len(decoratee_args)))
             # Turn arg_pairs into a dictionary and combine it with decoratee_kwargs.
             return {t[0]: decoratee_args[t[1]] for t in arg_pairs} | decoratee_kwargs
+            # No need to filter args as the logger is injected later.
+            # return {k: v for k, v in result.items() if not isinstance(v, Logger)}
 
         if asyncio.iscoroutinefunction(decoratee):
             @functools.wraps(decoratee)
             async def decorator(*decoratee_args, **decoratee_kwargs):
                 details = create_args_details(params(*decoratee_args, **decoratee_kwargs), args_format)
                 with telemetry_scope(module_name, scope_name, details=details) as scope:
                     inject_logger(scope, decoratee_kwargs)
```

