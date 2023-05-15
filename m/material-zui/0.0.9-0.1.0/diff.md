# Comparing `tmp/material_zui-0.0.9.tar.gz` & `tmp/material_zui-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.0.9.tar", max compression
+gzip compressed data, was "material_zui-0.1.0.tar", max compression
```

## Comparing `material_zui-0.0.9.tar` & `material_zui-0.1.0.tar`

### file list

```diff
@@ -1,46 +1,53 @@
--rw-r--r--   0        0        0      778 2023-05-13 12:22:55.970961 material_zui-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.0.9/src/material_zui/.pypirc
--rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.0.9/src/material_zui/ResizeImage.py
--rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.0.9/src/material_zui/compress/__init__.py
--rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.0.9/src/material_zui/compress/index.py
--rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.0.9/src/material_zui/compress/text.py
--rw-r--r--   0        0        0       36 2023-05-02 13:44:44.126257 material_zui-0.0.9/src/material_zui/crawl/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:44:44.126257 material_zui-0.0.9/src/material_zui/crawl/index.py
--rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.0.9/src/material_zui/crontab/__init__.py
--rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.0.9/src/material_zui/crontab/index.py
--rw-r--r--   0        0        0       43 2023-05-07 14:15:59.556081 material_zui-0.0.9/src/material_zui/date_time/__init__.py
--rw-r--r--   0        0        0       60 2023-05-07 14:15:59.604081 material_zui-0.0.9/src/material_zui/date_time/date_time.py
--rw-r--r--   0        0        0       49 2023-05-07 14:16:28.308295 material_zui-0.0.9/src/material_zui/date_time/index.py
--rw-r--r--   0        0        0      692 2023-05-07 14:16:10.888166 material_zui-0.0.9/src/material_zui/date_time/time.py
--rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.0.9/src/material_zui/image/__init__.py
--rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.0.9/src/material_zui/image/colorization.py
--rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.0.9/src/material_zui/image/combine.py
--rw-r--r--   0        0        0     5490 2023-05-11 10:24:19.669145 material_zui-0.0.9/src/material_zui/image/common.py
--rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.0.9/src/material_zui/image/convert.py
--rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.0.9/src/material_zui/image/data.py
--rw-r--r--   0        0        0      461 2023-05-11 10:14:50.303432 material_zui-0.0.9/src/material_zui/image/index.py
--rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.0.9/src/material_zui/image/model/colorization_deploy_v2.prototxt
--rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.0.9/src/material_zui/image/model/pts_in_hull.npy
--rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.0.9/src/material_zui/image/remove_background.py
--rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.0.9/src/material_zui/image/to_svg.py
--rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.0.9/src/material_zui/image/transparent_background.py
--rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.0.9/src/material_zui/image/type.py
--rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.0.9/src/material_zui/image/upscale.py
--rw-r--r--   0        0        0       48 2023-05-02 05:21:47.818631 material_zui-0.0.9/src/material_zui/language_model/__init__.py
--rw-r--r--   0        0        0      987 2023-05-02 05:36:54.809448 material_zui-0.0.9/src/material_zui/language_model/index.py
--rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.0.9/src/material_zui/log/__init__.py
--rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.0.9/src/material_zui/log/index.py
--rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.0.9/src/material_zui/log/log.py
--rw-r--r--   0        0        0      911 2023-05-12 10:39:11.524186 material_zui-0.0.9/src/material_zui/readme.md
--rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.0.9/src/material_zui/regex/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.0.9/src/material_zui/regex/index.py
--rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.0.9/src/material_zui/replicate/__init__.py
--rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.0.9/src/material_zui/replicate/index.py
--rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.0.9/src/material_zui/setup.py
--rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.0.9/src/material_zui/telegram_bot/__init__.py
--rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.0.9/src/material_zui/telegram_bot/index.py
--rw-r--r--   0        0        0       36 2023-04-30 11:48:06.223146 material_zui-0.0.9/src/material_zui/tmp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 03:39:00.036364 material_zui-0.0.9/src/material_zui/tmp/index.py
--rw-r--r--   0        0        0       36 2023-05-01 14:11:23.375942 material_zui-0.0.9/src/material_zui/validate/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 14:11:23.379941 material_zui-0.0.9/src/material_zui/validate/index.py
--rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 material_zui-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      822 2023-05-15 09:25:51.263824 material_zui-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.0/src/material_zui/.pypirc
+-rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.0/src/material_zui/ResizeImage.py
+-rw-r--r--   0        0        0       38 2023-05-15 08:52:40.288888 material_zui-0.1.0/src/material_zui/bard/__init__.py
+-rw-r--r--   0        0        0      543 2023-05-15 09:14:12.082997 material_zui-0.1.0/src/material_zui/bard/google_bard.py
+-rw-r--r--   0        0        0       77 2023-05-15 09:15:57.588848 material_zui-0.1.0/src/material_zui/bard/index.py
+-rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.0/src/material_zui/compress/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.0/src/material_zui/compress/index.py
+-rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.0/src/material_zui/compress/text.py
+-rw-r--r--   0        0        0       36 2023-05-02 13:44:44.126257 material_zui-0.1.0/src/material_zui/crawl/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:44:44.126257 material_zui-0.1.0/src/material_zui/crawl/index.py
+-rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.0/src/material_zui/crontab/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.0/src/material_zui/crontab/index.py
+-rw-r--r--   0        0        0       43 2023-05-07 14:15:59.556081 material_zui-0.1.0/src/material_zui/date_time/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-07 14:15:59.604081 material_zui-0.1.0/src/material_zui/date_time/date_time.py
+-rw-r--r--   0        0        0       49 2023-05-07 14:16:28.308295 material_zui-0.1.0/src/material_zui/date_time/index.py
+-rw-r--r--   0        0        0      692 2023-05-07 14:16:10.888166 material_zui-0.1.0/src/material_zui/date_time/time.py
+-rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.0/src/material_zui/env/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.0/src/material_zui/env/env.py
+-rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.0/src/material_zui/env/index.py
+-rw-r--r--   0        0        0       37 2023-05-15 08:50:53.425688 material_zui-0.1.0/src/material_zui/gpt/__init__.py
+-rw-r--r--   0        0        0     1057 2023-05-15 05:15:31.650338 material_zui-0.1.0/src/material_zui/gpt/gpt_vietnam.py
+-rw-r--r--   0        0        0       62 2023-05-15 08:50:53.385689 material_zui-0.1.0/src/material_zui/gpt/index.py
+-rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.0/src/material_zui/image/__init__.py
+-rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.0/src/material_zui/image/colorization.py
+-rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.0/src/material_zui/image/combine.py
+-rw-r--r--   0        0        0     5490 2023-05-11 10:24:19.669145 material_zui-0.1.0/src/material_zui/image/common.py
+-rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.0/src/material_zui/image/convert.py
+-rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.0/src/material_zui/image/data.py
+-rw-r--r--   0        0        0      461 2023-05-11 10:14:50.303432 material_zui-0.1.0/src/material_zui/image/index.py
+-rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.0/src/material_zui/image/model/colorization_deploy_v2.prototxt
+-rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.0/src/material_zui/image/model/pts_in_hull.npy
+-rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.0/src/material_zui/image/remove_background.py
+-rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.0/src/material_zui/image/to_svg.py
+-rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.0/src/material_zui/image/transparent_background.py
+-rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.0/src/material_zui/image/type.py
+-rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.0/src/material_zui/image/upscale.py
+-rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.0/src/material_zui/log/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.0/src/material_zui/log/index.py
+-rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.0/src/material_zui/log/log.py
+-rw-r--r--   0        0        0     1011 2023-05-15 09:24:15.658964 material_zui-0.1.0/src/material_zui/readme.md
+-rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.0/src/material_zui/regex/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.0/src/material_zui/regex/index.py
+-rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.0/src/material_zui/replicate/__init__.py
+-rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.0/src/material_zui/replicate/index.py
+-rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.0/src/material_zui/setup.py
+-rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.0/src/material_zui/telegram_bot/__init__.py
+-rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.0/src/material_zui/telegram_bot/index.py
+-rw-r--r--   0        0        0       36 2023-04-30 11:48:06.223146 material_zui-0.1.0/src/material_zui/tmp/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 03:39:00.036364 material_zui-0.1.0/src/material_zui/tmp/index.py
+-rw-r--r--   0        0        0       36 2023-05-01 14:11:23.375942 material_zui-0.1.0/src/material_zui/validate/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 14:11:23.379941 material_zui-0.1.0/src/material_zui/validate/index.py
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 material_zui-0.1.0/PKG-INFO
```

### Comparing `material_zui-0.0.9/pyproject.toml` & `material_zui-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "material_zui"
-version = "0.0.9"
+version = "0.1.0"
 description = "Material Zui"
 authors = ["chauhmnguyen <chauhoangminhnguyen@gmail.com>"]
 readme = "src/material_zui/readme.md"
 keywords = [
 	"material",
 	"zui",
 	"material zui",
@@ -24,11 +24,13 @@
 replicate = "^0.8.1"
 multipledispatch = "^0.6.0"
 pandas = "^2.0.1"
 pythonlangutil = "^0.1"
 python-crontab = "^2.7.1"
 rembg = "^2.0.36"
 pytelegrambotapi = "^4.11.0"
+bardapi = "^0.1.2"
+python-dotenv = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `material_zui-0.0.9/src/material_zui/ResizeImage.py` & `material_zui-0.1.0/src/material_zui/ResizeImage.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/compress/text.py` & `material_zui-0.1.0/src/material_zui/compress/text.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/crontab/index.py` & `material_zui-0.1.0/src/material_zui/crontab/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/date_time/time.py` & `material_zui-0.1.0/src/material_zui/date_time/time.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/colorization.py` & `material_zui-0.1.0/src/material_zui/image/colorization.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/combine.py` & `material_zui-0.1.0/src/material_zui/image/combine.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/common.py` & `material_zui-0.1.0/src/material_zui/image/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/convert.py` & `material_zui-0.1.0/src/material_zui/image/convert.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/model/colorization_deploy_v2.prototxt` & `material_zui-0.1.0/src/material_zui/image/model/colorization_deploy_v2.prototxt`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/model/pts_in_hull.npy` & `material_zui-0.1.0/src/material_zui/image/model/pts_in_hull.npy`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/remove_background.py` & `material_zui-0.1.0/src/material_zui/image/remove_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/to_svg.py` & `material_zui-0.1.0/src/material_zui/image/to_svg.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/transparent_background.py` & `material_zui-0.1.0/src/material_zui/image/transparent_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/image/upscale.py` & `material_zui-0.1.0/src/material_zui/image/upscale.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/language_model/index.py` & `material_zui-0.1.0/src/material_zui/gpt/gpt_vietnam.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         "temperature": 0.8,
         "top_p": 1
     })
     response = requests.post(url, headers=headers, data=payload)
     return response.text
 
 
-def gpt_last_result(prompt: str):
+def gpt_last_result(prompt: str) -> dict[{'text': str}] | None:
     data = gpt_call(prompt)
     last_value = value(data, '.+"finish_reason":"stop".+')
-    return json.loads(last_value)
+    return json.loads(last_value) if last_value else None
 
 
 def gpt_last_text_result(prompt: str) -> str:
     data = gpt_last_result(prompt)
-    return data['text']
+    return data['text'] if data else ''
```

### Comparing `material_zui-0.0.9/src/material_zui/log/log.py` & `material_zui-0.1.0/src/material_zui/log/log.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/regex/index.py` & `material_zui-0.1.0/src/material_zui/regex/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/replicate/index.py` & `material_zui-0.1.0/src/material_zui/replicate/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/src/material_zui/setup.py` & `material_zui-0.1.0/src/material_zui/setup.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.0.9/PKG-INFO` & `material_zui-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d61 7465  : 2.1.Name: mate
 00000020: 7269 616c 2d7a 7569 0a56 6572 7369 6f6e  rial-zui.Version
-00000030: 3a20 302e 302e 390a 5375 6d6d 6172 793a  : 0.0.9.Summary:
+00000030: 3a20 302e 312e 300a 5375 6d6d 6172 793a  : 0.1.0.Summary:
 00000040: 204d 6174 6572 6961 6c20 5a75 690a 4b65   Material Zui.Ke
 00000050: 7977 6f72 6473 3a20 6d61 7465 7269 616c  ywords: material
 00000060: 2c7a 7569 2c6d 6174 6572 6961 6c20 7a75  ,zui,material zu
 00000070: 692c 7a75 6920 6d61 7465 7269 616c 0a41  i,zui material.A
 00000080: 7574 686f 723a 2063 6861 7568 6d6e 6775  uthor: chauhmngu
 00000090: 7965 6e0a 4175 7468 6f72 2d65 6d61 696c  yen.Author-email
 000000a0: 3a20 6368 6175 686f 616e 676d 696e 686e  : chauhoangminhn
@@ -15,101 +15,113 @@
 000000e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
 000000f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 00000100: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
 00000110: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
 00000120: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 00000130: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
 00000140: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000150: 666c 6173 6b20 283e 3d32 2e33 2e32 2c3c  flask (>=2.3.2,<
-00000160: 332e 302e 3029 0a52 6571 7569 7265 732d  3.0.0).Requires-
-00000170: 4469 7374 3a20 6d61 7470 6c6f 746c 6962  Dist: matplotlib
-00000180: 2028 3e3d 332e 372e 312c 3c34 2e30 2e30   (>=3.7.1,<4.0.0
-00000190: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-000001a0: 206d 756c 7469 706c 6564 6973 7061 7463   multipledispatc
-000001b0: 6820 283e 3d30 2e36 2e30 2c3c 302e 372e  h (>=0.6.0,<0.7.
-000001c0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-000001d0: 3a20 6e75 6d70 7920 283e 3d31 2e32 342e  : numpy (>=1.24.
-000001e0: 332c 3c32 2e30 2e30 290a 5265 7175 6972  3,<2.0.0).Requir
-000001f0: 6573 2d44 6973 743a 206f 7065 6e63 762d  es-Dist: opencv-
-00000200: 7079 7468 6f6e 2028 3e3d 342e 372e 302e  python (>=4.7.0.
-00000210: 3732 2c3c 352e 302e 302e 3029 0a52 6571  72,<5.0.0.0).Req
-00000220: 7569 7265 732d 4469 7374 3a20 7061 6e64  uires-Dist: pand
-00000230: 6173 2028 3e3d 322e 302e 312c 3c33 2e30  as (>=2.0.1,<3.0
-00000240: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000250: 743a 2070 696c 6c6f 7720 283e 3d39 2e35  t: pillow (>=9.5
-00000260: 2e30 2c3c 3130 2e30 2e30 290a 5265 7175  .0,<10.0.0).Requ
-00000270: 6972 6573 2d44 6973 743a 2070 7974 656c  ires-Dist: pytel
-00000280: 6567 7261 6d62 6f74 6170 6920 283e 3d34  egrambotapi (>=4
-00000290: 2e31 312e 302c 3c35 2e30 2e30 290a 5265  .11.0,<5.0.0).Re
-000002a0: 7175 6972 6573 2d44 6973 743a 2070 7974  quires-Dist: pyt
-000002b0: 686f 6e2d 6372 6f6e 7461 6220 283e 3d32  hon-crontab (>=2
-000002c0: 2e37 2e31 2c3c 332e 302e 3029 0a52 6571  .7.1,<3.0.0).Req
-000002d0: 7569 7265 732d 4469 7374 3a20 7079 7468  uires-Dist: pyth
-000002e0: 6f6e 6c61 6e67 7574 696c 2028 3e3d 302e  onlangutil (>=0.
-000002f0: 312c 3c30 2e32 290a 5265 7175 6972 6573  1,<0.2).Requires
-00000300: 2d44 6973 743a 2072 656d 6267 2028 3e3d  -Dist: rembg (>=
-00000310: 322e 302e 3336 2c3c 332e 302e 3029 0a52  2.0.36,<3.0.0).R
-00000320: 6571 7569 7265 732d 4469 7374 3a20 7265  equires-Dist: re
-00000330: 706c 6963 6174 6520 283e 3d30 2e38 2e31  plicate (>=0.8.1
-00000340: 2c3c 302e 392e 3029 0a52 6571 7569 7265  ,<0.9.0).Require
-00000350: 732d 4469 7374 3a20 7265 7175 6573 7473  s-Dist: requests
-00000360: 2028 3e3d 322e 3330 2e30 2c3c 332e 302e   (>=2.30.0,<3.0.
-00000370: 3029 0a44 6573 6372 6970 7469 6f6e 2d43  0).Description-C
-00000380: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000390: 742f 6d61 726b 646f 776e 0a0a 2320 4d6f  t/markdown..# Mo
-000003a0: 6475 6c65 730a 0a3c 6f6c 3e0a 2020 3c6c  dules..<ol>.  <l
-000003b0: 693e 4372 6177 6c3c 2f6c 693e 0a20 203c  i>Crawl</li>.  <
-000003c0: 6c69 3e0a 2020 2020 496d 6167 650a 2020  li>.    Image.  
-000003d0: 2020 3c75 6c3e 0a20 2020 2020 203c 6c69    <ul>.      <li
-000003e0: 3e67 7261 7973 6361 6c65 3c2f 6c69 3e0a  >grayscale</li>.
-000003f0: 2020 2020 2020 3c6c 693e 636f 6c6f 7269        <li>colori
-00000400: 7a61 7469 6f6e 3c2f 6c69 3e0a 2020 2020  zation</li>.    
-00000410: 2020 3c6c 693e 736b 6574 6368 3c2f 6c69    <li>sketch</li
-00000420: 3e0a 2020 2020 2020 3c6c 693e 7472 616e  >.      <li>tran
-00000430: 7370 6172 656e 7420 6261 636b 6772 6f75  sparent backgrou
-00000440: 6e64 3c2f 6c69 3e0a 2020 2020 2020 3c6c  nd</li>.      <l
-00000450: 693e 7570 7363 616c 653c 2f6c 693e 0a20  i>upscale</li>. 
-00000460: 2020 2020 203c 6c69 3e63 6f6e 7665 7274       <li>convert
-00000470: 2074 6f20 6a70 672f 706e 673c 2f6c 693e   to jpg/png</li>
-00000480: 0a20 2020 203c 2f75 6c3e 0a20 203c 2f6c  .    </ul>.  </l
-00000490: 693e 0a20 203c 6c69 3e4c 616e 6775 6167  i>.  <li>Languag
-000004a0: 6520 4d6f 6465 6c3c 2f6c 693e 0a20 203c  e Model</li>.  <
-000004b0: 6c69 3e52 6567 6578 3c2f 6c69 3e0a 2020  li>Regex</li>.  
-000004c0: 3c6c 693e 4c6f 673c 2f6c 693e 0a20 203c  <li>Log</li>.  <
-000004d0: 6c69 3e52 6570 6c69 6361 7465 3a20 4149  li>Replicate: AI
-000004e0: 2050 6c61 7466 6f72 6d20 4150 493c 2f6c   Platform API</l
-000004f0: 693e 0a20 203c 6c69 3e54 656c 6567 7261  i>.  <li>Telegra
-00000500: 6d20 426f 743c 2f6c 693e 0a20 203c 6c69  m Bot</li>.  <li
-00000510: 3e56 616c 6964 6174 653c 2f6c 693e 0a3c  >Validate</li>.<
-00000520: 2f6f 6c3e 0a0a 2320 4c6f 670a 0a2d 2045  /ol>..# Log..- E
-00000530: 7861 6d70 6c65 3a0a 0a60 6060 7079 0a66  xample:..```py.f
-00000540: 726f 6d20 6d61 7465 7269 616c 5f7a 7569  rom material_zui
-00000550: 2e6c 6f67 2069 6d70 6f72 7420 6465 6275  .log import debu
-00000560: 672c 2069 6e66 6f2c 2077 6172 6e69 6e67  g, info, warning
-00000570: 2c20 6572 726f 722c 2063 7269 7469 6361  , error, critica
-00000580: 6c2c 2070 7269 6e74 5461 626c 650a 0a64  l, printTable..d
-00000590: 6562 7567 2827 5468 6973 2069 7320 6120  ebug('This is a 
-000005a0: 6465 6275 6720 6d65 7373 6167 6527 290a  debug message').
-000005b0: 696e 666f 2827 5468 6973 2069 7320 616e  info('This is an
-000005c0: 2069 6e66 6f20 6d65 7373 6167 6527 290a   info message').
-000005d0: 7761 726e 696e 6728 2754 6869 7320 6973  warning('This is
-000005e0: 2061 2077 6172 6e69 6e67 206d 6573 7361   a warning messa
-000005f0: 6765 2729 0a65 7272 6f72 2827 5468 6973  ge').error('This
-00000600: 2069 7320 616e 2065 7272 6f72 206d 6573   is an error mes
-00000610: 7361 6765 2729 0a63 7269 7469 6361 6c28  sage').critical(
-00000620: 2754 6869 7320 6973 2061 2063 7269 7469  'This is a criti
-00000630: 6361 6c20 6d65 7373 6167 6527 290a 0a70  cal message')..p
-00000640: 7269 6e74 5461 626c 6528 7b0a 2020 2020  rintTable({.    
-00000650: 274e 616d 6527 3a20 5b27 416c 6963 6527  'Name': ['Alice'
-00000660: 2c20 2742 6f62 272c 2027 4368 6172 6c69  , 'Bob', 'Charli
-00000670: 6527 2c20 2744 6176 6527 5d2c 0a20 2020  e', 'Dave'],.   
-00000680: 2027 4167 6527 3a20 5b32 352c 2033 312c   'Age': [25, 31,
-00000690: 2033 352c 2031 395d 2c0a 2020 2020 2753   35, 19],.    'S
-000006a0: 636f 7265 273a 205b 3835 2c20 3934 2c20  core': [85, 94, 
-000006b0: 3736 2c20 3935 5d0a 7d29 0a60 6060 0a0a  76, 95].}).```..
-000006c0: 2d20 5265 7375 6c74 3a0a 2020 215b 416c  - Result:.  ![Al
-000006d0: 7420 7465 7874 5d28 2e2e 2f2e 2e2f 7374  t text](../../st
-000006e0: 6174 6963 2f69 6d67 2f64 6f63 2f6c 6f67  atic/img/doc/log
-000006f0: 312e 706e 6729 0a0a 2320 5061 636b 6167  1.png)..# Packag
-00000700: 650a 0a2d 2068 7474 7073 3a2f 2f70 7970  e..- https://pyp
-00000710: 692e 6f72 672f 7072 6f6a 6563 742f 6d61  i.org/project/ma
-00000720: 7465 7269 616c 2d7a 7569 0a0a            terial-zui..
+00000150: 6261 7264 6170 6920 283e 3d30 2e31 2e32  bardapi (>=0.1.2
+00000160: 2c3c 302e 322e 3029 0a52 6571 7569 7265  ,<0.2.0).Require
+00000170: 732d 4469 7374 3a20 666c 6173 6b20 283e  s-Dist: flask (>
+00000180: 3d32 2e33 2e32 2c3c 332e 302e 3029 0a52  =2.3.2,<3.0.0).R
+00000190: 6571 7569 7265 732d 4469 7374 3a20 6d61  equires-Dist: ma
+000001a0: 7470 6c6f 746c 6962 2028 3e3d 332e 372e  tplotlib (>=3.7.
+000001b0: 312c 3c34 2e30 2e30 290a 5265 7175 6972  1,<4.0.0).Requir
+000001c0: 6573 2d44 6973 743a 206d 756c 7469 706c  es-Dist: multipl
+000001d0: 6564 6973 7061 7463 6820 283e 3d30 2e36  edispatch (>=0.6
+000001e0: 2e30 2c3c 302e 372e 3029 0a52 6571 7569  .0,<0.7.0).Requi
+000001f0: 7265 732d 4469 7374 3a20 6e75 6d70 7920  res-Dist: numpy 
+00000200: 283e 3d31 2e32 342e 332c 3c32 2e30 2e30  (>=1.24.3,<2.0.0
+00000210: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+00000220: 206f 7065 6e63 762d 7079 7468 6f6e 2028   opencv-python (
+00000230: 3e3d 342e 372e 302e 3732 2c3c 352e 302e  >=4.7.0.72,<5.0.
+00000240: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
+00000250: 7374 3a20 7061 6e64 6173 2028 3e3d 322e  st: pandas (>=2.
+00000260: 302e 312c 3c33 2e30 2e30 290a 5265 7175  0.1,<3.0.0).Requ
+00000270: 6972 6573 2d44 6973 743a 2070 696c 6c6f  ires-Dist: pillo
+00000280: 7720 283e 3d39 2e35 2e30 2c3c 3130 2e30  w (>=9.5.0,<10.0
+00000290: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
+000002a0: 743a 2070 7974 656c 6567 7261 6d62 6f74  t: pytelegrambot
+000002b0: 6170 6920 283e 3d34 2e31 312e 302c 3c35  api (>=4.11.0,<5
+000002c0: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+000002d0: 6973 743a 2070 7974 686f 6e2d 6372 6f6e  ist: python-cron
+000002e0: 7461 6220 283e 3d32 2e37 2e31 2c3c 332e  tab (>=2.7.1,<3.
+000002f0: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
+00000300: 7374 3a20 7079 7468 6f6e 2d64 6f74 656e  st: python-doten
+00000310: 7620 283e 3d31 2e30 2e30 2c3c 322e 302e  v (>=1.0.0,<2.0.
+00000320: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000330: 3a20 7079 7468 6f6e 6c61 6e67 7574 696c  : pythonlangutil
+00000340: 2028 3e3d 302e 312c 3c30 2e32 290a 5265   (>=0.1,<0.2).Re
+00000350: 7175 6972 6573 2d44 6973 743a 2072 656d  quires-Dist: rem
+00000360: 6267 2028 3e3d 322e 302e 3336 2c3c 332e  bg (>=2.0.36,<3.
+00000370: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
+00000380: 7374 3a20 7265 706c 6963 6174 6520 283e  st: replicate (>
+00000390: 3d30 2e38 2e31 2c3c 302e 392e 3029 0a52  =0.8.1,<0.9.0).R
+000003a0: 6571 7569 7265 732d 4469 7374 3a20 7265  equires-Dist: re
+000003b0: 7175 6573 7473 2028 3e3d 322e 3330 2e30  quests (>=2.30.0
+000003c0: 2c3c 332e 302e 3029 0a44 6573 6372 6970  ,<3.0.0).Descrip
+000003d0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+000003e0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+000003f0: 0a0a 2320 4d6f 6475 6c65 730a 0a3c 6f6c  ..# Modules..<ol
+00000400: 3e0a 2020 3c6c 693e 6261 7264 3c2f 6c69  >.  <li>bard</li
+00000410: 3e0a 2020 3c6c 693e 636f 6d70 7265 7373  >.  <li>compress
+00000420: 3c2f 6c69 3e0a 2020 3c6c 693e 6372 6177  </li>.  <li>craw
+00000430: 6c3c 2f6c 693e 0a20 203c 6c69 3e63 726f  l</li>.  <li>cro
+00000440: 6e74 6162 3c2f 6c69 3e0a 2020 3c6c 693e  ntab</li>.  <li>
+00000450: 6461 7465 5f74 696d 653c 2f6c 693e 0a20  date_time</li>. 
+00000460: 203c 6c69 3e65 6e76 3c2f 6c69 3e0a 2020   <li>env</li>.  
+00000470: 3c6c 693e 6770 743c 2f6c 693e 0a20 203c  <li>gpt</li>.  <
+00000480: 6c69 3e0a 2020 2020 696d 6167 650a 2020  li>.    image.  
+00000490: 2020 3c75 6c3e 0a20 2020 2020 203c 6c69    <ul>.      <li
+000004a0: 3e67 7261 7973 6361 6c65 3c2f 6c69 3e0a  >grayscale</li>.
+000004b0: 2020 2020 2020 3c6c 693e 636f 6c6f 7269        <li>colori
+000004c0: 7a61 7469 6f6e 3c2f 6c69 3e0a 2020 2020  zation</li>.    
+000004d0: 2020 3c6c 693e 736b 6574 6368 3c2f 6c69    <li>sketch</li
+000004e0: 3e0a 2020 2020 2020 3c6c 693e 7472 616e  >.      <li>tran
+000004f0: 7370 6172 656e 7420 6261 636b 6772 6f75  sparent backgrou
+00000500: 6e64 3c2f 6c69 3e0a 2020 2020 2020 3c6c  nd</li>.      <l
+00000510: 693e 7570 7363 616c 653c 2f6c 693e 0a20  i>upscale</li>. 
+00000520: 2020 2020 203c 6c69 3e63 6f6e 7665 7274       <li>convert
+00000530: 2074 6f20 6a70 672f 706e 673c 2f6c 693e   to jpg/png</li>
+00000540: 0a20 2020 203c 2f75 6c3e 0a20 203c 2f6c  .    </ul>.  </l
+00000550: 693e 0a20 203c 6c69 3e3c 6120 6872 6566  i>.  <li><a href
+00000560: 3d22 236c 6f67 223e 4c6f 673c 2f61 3e3c  ="#log">Log</a><
+00000570: 2f6c 693e 0a20 203c 6c69 3e72 6567 6578  /li>.  <li>regex
+00000580: 3c2f 6c69 3e0a 2020 3c6c 693e 7265 706c  </li>.  <li>repl
+00000590: 6963 6174 653a 2041 4920 506c 6174 666f  icate: AI Platfo
+000005a0: 726d 2041 5049 3c2f 6c69 3e0a 2020 3c6c  rm API</li>.  <l
+000005b0: 693e 7465 6c65 6772 616d 5f62 6f74 3c2f  i>telegram_bot</
+000005c0: 6c69 3e0a 2020 3c6c 693e 7661 6c69 6461  li>.  <li>valida
+000005d0: 7465 3c2f 6c69 3e0a 3c2f 6f6c 3e0a 0a23  te</li>.</ol>..#
+000005e0: 204c 6f67 0a0a 2d20 4578 616d 706c 653a   Log..- Example:
+000005f0: 0a0a 6060 6070 790a 6672 6f6d 206d 6174  ..```py.from mat
+00000600: 6572 6961 6c5f 7a75 692e 6c6f 6720 696d  erial_zui.log im
+00000610: 706f 7274 2064 6562 7567 2c20 696e 666f  port debug, info
+00000620: 2c20 7761 726e 696e 672c 2065 7272 6f72  , warning, error
+00000630: 2c20 6372 6974 6963 616c 2c20 7072 696e  , critical, prin
+00000640: 7454 6162 6c65 0a0a 6465 6275 6728 2754  tTable..debug('T
+00000650: 6869 7320 6973 2061 2064 6562 7567 206d  his is a debug m
+00000660: 6573 7361 6765 2729 0a69 6e66 6f28 2754  essage').info('T
+00000670: 6869 7320 6973 2061 6e20 696e 666f 206d  his is an info m
+00000680: 6573 7361 6765 2729 0a77 6172 6e69 6e67  essage').warning
+00000690: 2827 5468 6973 2069 7320 6120 7761 726e  ('This is a warn
+000006a0: 696e 6720 6d65 7373 6167 6527 290a 6572  ing message').er
+000006b0: 726f 7228 2754 6869 7320 6973 2061 6e20  ror('This is an 
+000006c0: 6572 726f 7220 6d65 7373 6167 6527 290a  error message').
+000006d0: 6372 6974 6963 616c 2827 5468 6973 2069  critical('This i
+000006e0: 7320 6120 6372 6974 6963 616c 206d 6573  s a critical mes
+000006f0: 7361 6765 2729 0a0a 7072 696e 7454 6162  sage')..printTab
+00000700: 6c65 287b 0a20 2020 2027 4e61 6d65 273a  le({.    'Name':
+00000710: 205b 2741 6c69 6365 272c 2027 426f 6227   ['Alice', 'Bob'
+00000720: 2c20 2743 6861 726c 6965 272c 2027 4461  , 'Charlie', 'Da
+00000730: 7665 275d 2c0a 2020 2020 2741 6765 273a  ve'],.    'Age':
+00000740: 205b 3235 2c20 3331 2c20 3335 2c20 3139   [25, 31, 35, 19
+00000750: 5d2c 0a20 2020 2027 5363 6f72 6527 3a20  ],.    'Score': 
+00000760: 5b38 352c 2039 342c 2037 362c 2039 355d  [85, 94, 76, 95]
+00000770: 0a7d 290a 6060 600a 0a3c 212d 2d20 2d20  .}).```..<!-- - 
+00000780: 5265 7375 6c74 3a0a 2020 215b 5d28 2e2e  Result:.  ![](..
+00000790: 2f2e 2e2f 7374 6174 6963 2f69 6d67 2f64  /../static/img/d
+000007a0: 6f63 2f6c 6f67 312e 706e 6729 202d 2d3e  oc/log1.png) -->
+000007b0: 0a0a 2320 5061 636b 6167 650a 0a2d 2068  ..# Package..- h
+000007c0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000007d0: 7072 6f6a 6563 742f 6d61 7465 7269 616c  project/material
+000007e0: 2d7a 7569 0a0a                           -zui..
```

