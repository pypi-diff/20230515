# Comparing `tmp/lightweight_charts-1.0.2.tar.gz` & `tmp/lightweight_charts-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweight_charts-1.0.2.tar", last modified: Fri May 12 12:23:58 2023, max compression
+gzip compressed data, was "lightweight_charts-1.0.3.tar", last modified: Mon May 15 11:27:10 2023, max compression
```

## Comparing `lightweight_charts-1.0.2.tar` & `lightweight_charts-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-12 12:23:58.692836 lightweight_charts-1.0.2/
--rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.2/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)     5248 2023-05-12 12:23:58.692422 lightweight_charts-1.0.2/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     4902 2023-05-10 19:28:46.000000 lightweight_charts-1.0.2/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-12 12:23:58.689163 lightweight_charts-1.0.2/lightweight_charts/
--rw-r--r--   0 louis      (501) staff       (20)      121 2023-05-09 21:54:08.000000 lightweight_charts-1.0.2/lightweight_charts/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     8733 2023-05-12 11:55:19.000000 lightweight_charts-1.0.2/lightweight_charts/chart.py
--rw-r--r--   0 louis      (501) staff       (20)    22951 2023-05-10 12:49:09.000000 lightweight_charts-1.0.2/lightweight_charts/js.py
--rw-r--r--   0 louis      (501) staff       (20)   141259 2023-05-09 19:50:25.000000 lightweight_charts-1.0.2/lightweight_charts/pkg.py
--rw-r--r--   0 louis      (501) staff       (20)     2364 2023-05-12 11:50:34.000000 lightweight_charts-1.0.2/lightweight_charts/pywebview.py
--rw-r--r--   0 louis      (501) staff       (20)     1422 2023-05-10 00:01:10.000000 lightweight_charts-1.0.2/lightweight_charts/util.py
--rw-r--r--   0 louis      (501) staff       (20)      796 2023-05-12 11:35:31.000000 lightweight_charts-1.0.2/lightweight_charts/widgets.py
--rw-r--r--   0 louis      (501) staff       (20)     1547 2023-05-12 11:45:19.000000 lightweight_charts-1.0.2/lightweight_charts/working.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-12 12:23:58.691786 lightweight_charts-1.0.2/lightweight_charts.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     5248 2023-05-12 12:23:58.000000 lightweight_charts-1.0.2/lightweight_charts.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      464 2023-05-12 12:23:58.000000 lightweight_charts-1.0.2/lightweight_charts.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-12 12:23:58.000000 lightweight_charts-1.0.2/lightweight_charts.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-12 12:23:58.000000 lightweight_charts-1.0.2/lightweight_charts.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-12 12:23:58.000000 lightweight_charts-1.0.2/lightweight_charts.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-12 12:23:58.693041 lightweight_charts-1.0.2/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-12 12:23:43.000000 lightweight_charts-1.0.2/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-15 11:27:10.537022 lightweight_charts-1.0.3/
+-rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.3/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)     5309 2023-05-15 11:27:10.536615 lightweight_charts-1.0.3/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     4963 2023-05-15 11:26:26.000000 lightweight_charts-1.0.3/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-15 11:27:10.532447 lightweight_charts-1.0.3/lightweight_charts/
+-rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.3/lightweight_charts/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     8834 2023-05-15 11:19:36.000000 lightweight_charts-1.0.3/lightweight_charts/chart.py
+-rw-r--r--   0 louis      (501) staff       (20)    22951 2023-05-14 16:01:34.000000 lightweight_charts-1.0.3/lightweight_charts/js.py
+-rw-r--r--   0 louis      (501) staff       (20)   141259 2023-05-09 19:50:25.000000 lightweight_charts-1.0.3/lightweight_charts/pkg.py
+-rw-r--r--   0 louis      (501) staff       (20)     2364 2023-05-12 11:50:34.000000 lightweight_charts-1.0.3/lightweight_charts/pywebview.py
+-rw-r--r--   0 louis      (501) staff       (20)      516 2023-05-15 00:43:19.000000 lightweight_charts-1.0.3/lightweight_charts/qttest.py
+-rw-r--r--   0 louis      (501) staff       (20)     1422 2023-05-10 00:01:10.000000 lightweight_charts-1.0.3/lightweight_charts/util.py
+-rw-r--r--   0 louis      (501) staff       (20)     1721 2023-05-15 11:19:36.000000 lightweight_charts-1.0.3/lightweight_charts/widgets.py
+-rw-r--r--   0 louis      (501) staff       (20)     1584 2023-05-14 13:53:44.000000 lightweight_charts-1.0.3/lightweight_charts/working.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-15 11:27:10.535941 lightweight_charts-1.0.3/lightweight_charts.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     5309 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      493 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-15 11:27:10.000000 lightweight_charts-1.0.3/lightweight_charts.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-15 11:27:10.537190 lightweight_charts-1.0.3/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-15 11:19:36.000000 lightweight_charts-1.0.3/setup.py
```

### Comparing `lightweight_charts-1.0.2/LICENSE` & `lightweight_charts-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.2/PKG-INFO` & `lightweight_charts-1.0.3/lightweight_charts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: lightweight_charts
-Version: 1.0.2
+Name: lightweight-charts
+Version: 1.0.3
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lightweight_charts_python
 
+
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
 ___
@@ -155,24 +156,27 @@
 
 if __name__ == '__main__':
     
     chart = Chart(debug=True)
 
     df = pd.read_csv('ohlcv.csv')
 
-    chart.layout(background_color='#090008', text_color='#FFFFFF', font_size=16, font_family='Helvetica')
+    chart.layout(background_color='#090008', text_color='#FFFFFF', font_size=16,
+                 font_family='Helvetica')
 
-    chart.candle_style(up_color='#00ff55', down_color='#ed4807', border_up_color='#FFFFFF', border_down_color='#FFFFFF',
+    chart.candle_style(up_color='#00ff55', down_color='#ed4807',
+                       border_up_color='#FFFFFF', border_down_color='#FFFFFF',
                        wick_up_color='#FFFFFF', wick_down_color='#FFFFFF')
 
     chart.volume_config(up_color='#00ff55', down_color='#ed4807')
 
     chart.watermark('1D', color='rgba(180, 180, 240, 0.7)')
 
-    chart.crosshair(mode='normal', vert_color='#FFFFFF', vert_style='dotted', horz_color='#FFFFFF', horz_style='dotted')
+    chart.crosshair(mode='normal', vert_color='#FFFFFF', vert_style='dotted',
+                    horz_color='#FFFFFF', horz_style='dotted')
 
     chart.legend(visible=True, font_size=14)
 
     chart.set(df)
 
     chart.show(block=True)
```

### Comparing `lightweight_charts-1.0.2/README.md` & `lightweight_charts-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # lightweight_charts_python
 
+
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
 ___
@@ -143,24 +144,27 @@
 
 if __name__ == '__main__':
     
     chart = Chart(debug=True)
 
     df = pd.read_csv('ohlcv.csv')
 
-    chart.layout(background_color='#090008', text_color='#FFFFFF', font_size=16, font_family='Helvetica')
+    chart.layout(background_color='#090008', text_color='#FFFFFF', font_size=16,
+                 font_family='Helvetica')
 
-    chart.candle_style(up_color='#00ff55', down_color='#ed4807', border_up_color='#FFFFFF', border_down_color='#FFFFFF',
+    chart.candle_style(up_color='#00ff55', down_color='#ed4807',
+                       border_up_color='#FFFFFF', border_down_color='#FFFFFF',
                        wick_up_color='#FFFFFF', wick_down_color='#FFFFFF')
 
     chart.volume_config(up_color='#00ff55', down_color='#ed4807')
 
     chart.watermark('1D', color='rgba(180, 180, 240, 0.7)')
 
-    chart.crosshair(mode='normal', vert_color='#FFFFFF', vert_style='dotted', horz_color='#FFFFFF', horz_style='dotted')
+    chart.crosshair(mode='normal', vert_color='#FFFFFF', vert_style='dotted',
+                    horz_color='#FFFFFF', horz_style='dotted')
 
     chart.legend(visible=True, font_size=14)
 
     chart.set(df)
 
     chart.show(block=True)
```

### Comparing `lightweight_charts-1.0.2/lightweight_charts/chart.py` & `lightweight_charts-1.0.3/lightweight_charts/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 from datetime import datetime
 from typing import Union
 
 from lightweight_charts.pywebview import _loop
 from lightweight_charts.util import LINE_TYPE, POSITION, SHAPE, CROSSHAIR_MODE, PRICE_SCALE_MODE
 
 
+# TODO Changelog
+#   Added support for PyQt.
+#   Refactored widgets to catch ModuleNotFoundErrors.
+
+
 class Line:
     def __init__(self, chart, line_id):
         self._chart = chart
         self.id = line_id
 
     def set(self, data: pd.DataFrame):
         """
```

### Comparing `lightweight_charts-1.0.2/lightweight_charts/js.py` & `lightweight_charts-1.0.3/lightweight_charts/js.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.2/lightweight_charts/pkg.py` & `lightweight_charts-1.0.3/lightweight_charts/pkg.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.2/lightweight_charts/pywebview.py` & `lightweight_charts-1.0.3/lightweight_charts/pywebview.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.2/lightweight_charts/util.py` & `lightweight_charts-1.0.3/lightweight_charts/util.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.2/lightweight_charts/working.py` & `lightweight_charts-1.0.3/lightweight_charts/working.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 
 import wx
 from time import sleep
 import pandas as pd
 
-from lightweight_charts import Chart, WxChart
+from lightweight_charts import Chart
+from lightweight_charts.widgets import WxChart
 
 
 def on_click(x):
     print('yeayea')
     print(x)
 
 
@@ -48,15 +49,14 @@
     df = pd.read_csv('../examples/1_setting_data/ohlcv.csv')
     frame.chart.set(df)
     app.MainLoop()
 
 
 if __name__ == '__main__':
 
-
     start_wx_app()
 
     chart = Chart(width=1000, debug=True)
 
     df = pd.read_csv('../examples/1_setting_data/ohlcv.csv')
 
     chart.set(df)
```

### Comparing `lightweight_charts-1.0.2/lightweight_charts.egg-info/PKG-INFO` & `lightweight_charts-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: lightweight-charts
-Version: 1.0.2
+Name: lightweight_charts
+Version: 1.0.3
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lightweight_charts_python
 
+
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
 ___
@@ -155,24 +156,27 @@
 
 if __name__ == '__main__':
     
     chart = Chart(debug=True)
 
     df = pd.read_csv('ohlcv.csv')
 
-    chart.layout(background_color='#090008', text_color='#FFFFFF', font_size=16, font_family='Helvetica')
+    chart.layout(background_color='#090008', text_color='#FFFFFF', font_size=16,
+                 font_family='Helvetica')
 
-    chart.candle_style(up_color='#00ff55', down_color='#ed4807', border_up_color='#FFFFFF', border_down_color='#FFFFFF',
+    chart.candle_style(up_color='#00ff55', down_color='#ed4807',
+                       border_up_color='#FFFFFF', border_down_color='#FFFFFF',
                        wick_up_color='#FFFFFF', wick_down_color='#FFFFFF')
 
     chart.volume_config(up_color='#00ff55', down_color='#ed4807')
 
     chart.watermark('1D', color='rgba(180, 180, 240, 0.7)')
 
-    chart.crosshair(mode='normal', vert_color='#FFFFFF', vert_style='dotted', horz_color='#FFFFFF', horz_style='dotted')
+    chart.crosshair(mode='normal', vert_color='#FFFFFF', vert_style='dotted',
+                    horz_color='#FFFFFF', horz_style='dotted')
 
     chart.legend(visible=True, font_size=14)
 
     chart.set(df)
 
     chart.show(block=True)
```

### Comparing `lightweight_charts-1.0.2/setup.py` & `lightweight_charts-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='lightweight_charts',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'pandas',
         'pywebview',
     ],
     author='louisnw',
```

