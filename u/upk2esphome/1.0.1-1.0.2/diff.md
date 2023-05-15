# Comparing `tmp/upk2esphome-1.0.1.tar.gz` & `tmp/upk2esphome-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upk2esphome-1.0.1.tar", max compression
+gzip compressed data, was "upk2esphome-1.0.2.tar", max compression
```

## Comparing `upk2esphome-1.0.1.tar` & `upk2esphome-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1076 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/LICENSE
--rw-r--r--   0        0        0      531 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/README.md
--rw-r--r--   0        0        0      455 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      256 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/__init__.py
--rw-r--r--   0        0        0     1650 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/generator.py
--rw-r--r--   0        0        0     1442 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/input.py
--rw-r--r--   0        0        0      400 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/opts.py
--rw-r--r--   0        0        0       48 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/parts/__init__.py
--rw-r--r--   0        0        0     8367 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/parts/bulb.py
--rw-r--r--   0        0        0     1403 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/parts/module.py
--rw-r--r--   0        0        0     3355 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/parts/monitor.py
--rw-r--r--   0        0        0      775 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/parts/netled.py
--rw-r--r--   0        0        0     1355 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/parts/static.py
--rw-r--r--   0        0        0     3009 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/parts/switch.py
--rw-r--r--   0        0        0     1834 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/result.py
--rw-r--r--   0        0        0      651 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/test.py
--rw-r--r--   0        0        0      444 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/bulb_cw_pwm.txt
--rw-r--r--   0        0        0      563 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/bulb_rgbc_2135_2.txt
--rw-r--r--   0        0        0      430 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/bulb_rgbcw_2135.txt
--rw-r--r--   0        0        0      543 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt
--rw-r--r--   0        0        0      599 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/bulb_rgbcw_2235.txt
--rw-r--r--   0        0        0      496 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/bulb_rgbcw_5758d.txt
--rw-r--r--   0        0        0        0 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/empty.txt
--rw-r--r--   0        0        0     2936 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/plug_monitor_bl0937.txt
--rw-r--r--   0        0        0      476 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/plug_monitor_bl0942.txt
--rw-r--r--   0        0        0      497 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/plug_monitor_hlw8032.txt
--rw-r--r--   0        0        0      914 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/plug_total.txt
--rw-r--r--   0        0        0      777 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/tests/switch_monitor.txt
--rw-r--r--   0        0        0      922 2023-05-13 17:10:01.414842 upk2esphome-1.0.1/upk2esphome/web.py
--rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 upk2esphome-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/LICENSE
+-rw-r--r--   0        0        0      531 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/README.md
+-rw-r--r--   0        0        0      455 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      256 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/__init__.py
+-rw-r--r--   0        0        0     1650 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/generator.py
+-rw-r--r--   0        0        0     1442 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/input.py
+-rw-r--r--   0        0        0      400 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/opts.py
+-rw-r--r--   0        0        0       48 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/__init__.py
+-rw-r--r--   0        0        0     8367 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/bulb.py
+-rw-r--r--   0        0        0     1406 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/module.py
+-rw-r--r--   0        0        0     3403 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/monitor.py
+-rw-r--r--   0        0        0      775 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/netled.py
+-rw-r--r--   0        0        0     1355 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/static.py
+-rw-r--r--   0        0        0     3009 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/parts/switch.py
+-rw-r--r--   0        0        0     1834 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/result.py
+-rw-r--r--   0        0        0      651 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/test.py
+-rw-r--r--   0        0        0      444 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_cw_pwm.txt
+-rw-r--r--   0        0        0      563 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbc_2135_2.txt
+-rw-r--r--   0        0        0      430 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2135.txt
+-rw-r--r--   0        0        0      543 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt
+-rw-r--r--   0        0        0      599 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2235.txt
+-rw-r--r--   0        0        0      496 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_5758d.txt
+-rw-r--r--   0        0        0        0 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/empty.txt
+-rw-r--r--   0        0        0     2936 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/plug_monitor_bl0937.txt
+-rw-r--r--   0        0        0      476 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/plug_monitor_bl0942.txt
+-rw-r--r--   0        0        0      497 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/plug_monitor_hlw8032.txt
+-rw-r--r--   0        0        0      914 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/plug_total.txt
+-rw-r--r--   0        0        0      777 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/tests/switch_monitor.txt
+-rw-r--r--   0        0        0      922 2023-05-15 18:24:44.766976 upk2esphome-1.0.2/upk2esphome/web.py
+-rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 upk2esphome-1.0.2/PKG-INFO
```

### Comparing `upk2esphome-1.0.1/LICENSE` & `upk2esphome-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/README.md` & `upk2esphome-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/generator.py` & `upk2esphome-1.0.2/upk2esphome/generator.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/input.py` & `upk2esphome-1.0.2/upk2esphome/input.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/parts/bulb.py` & `upk2esphome-1.0.2/upk2esphome/parts/bulb.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/parts/module.py` & `upk2esphome-1.0.2/upk2esphome/parts/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         if opts.esphome_block:
             yr.data["esphome"] = {
                 "name": "upk2esphome",
             }
             if opts.name_mac:
                 yr.data["esphome"]["name_add_mac_suffix"] = True
             yr.data["libretiny"] = {
-                "board": "FIX_ME",
+                "board": "REPLACEME",
                 "framework": {
                     "version": "dev",
                 },
             }
         return
 
     match module[0:2].upper():
```

### Comparing `upk2esphome-1.0.1/upk2esphome/parts/monitor.py` & `upk2esphome-1.0.2/upk2esphome/parts/monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,27 +33,28 @@
             ele_pin = config.get("ele_pin", None)
             vi_pin = config.get("vi_pin", None)
             sel_pin = config.get("sel_pin_pin", None)
             sel_inv = config.get("sel_pin_lv", None) == 1
             chip = "BL0937" if chip_type == 0 else "HLW8012"
             yr.log(
                 f"Power monitoring chip {chip}: "
-                f"CF=P{ele_pin}, CF1=P{vi_pin}, SEL={sel_pin}"
+                f"CF/ELE=P{ele_pin}, CF1/VI=P{vi_pin}, SEL={sel_pin}"
             )
             yr.found = True
             sensor = {
                 "platform": "hlw8012",
                 "model": chip,
                 "cf_pin": f"P{ele_pin}",
                 "cf1_pin": f"P{vi_pin}",
                 "sel_pin": f"P{sel_pin}",
                 "current": {"name": f"{chip} Current"},
                 "voltage": {"name": f"{chip} Voltage"},
                 "power": {"name": f"{chip} Power"},
                 "energy": {"name": f"{chip} Energy"},
+                "voltage_divider": 1600,
             }
             if resistor is not None:
                 yr.log(f" - shunt resistor: {resistor} mΩ")
                 sensor["current_resistor"] = f"{resistor/1000:.03f} ohm"
             invert(sensor, sel_inv, "sel_pin")
             invert(sensor, chip_type == 0, "cf_pin")
             invert(sensor, chip_type == 0, "cf1_pin")
```

### Comparing `upk2esphome-1.0.1/upk2esphome/parts/netled.py` & `upk2esphome-1.0.2/upk2esphome/parts/netled.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/parts/static.py` & `upk2esphome-1.0.2/upk2esphome/parts/static.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/parts/switch.py` & `upk2esphome-1.0.2/upk2esphome/parts/switch.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/result.py` & `upk2esphome-1.0.2/upk2esphome/result.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/test.py` & `upk2esphome-1.0.2/upk2esphome/test.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/tests/bulb_rgbc_2135_2.txt` & `upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbc_2135_2.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt` & `upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/tests/bulb_rgbcw_2235.txt` & `upk2esphome-1.0.2/upk2esphome/tests/bulb_rgbcw_2235.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/tests/plug_monitor_bl0937.txt` & `upk2esphome-1.0.2/upk2esphome/tests/plug_monitor_bl0937.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/tests/plug_total.txt` & `upk2esphome-1.0.2/upk2esphome/tests/plug_total.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/tests/switch_monitor.txt` & `upk2esphome-1.0.2/upk2esphome/tests/switch_monitor.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/upk2esphome/web.py` & `upk2esphome-1.0.2/upk2esphome/web.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.0.1/PKG-INFO` & `upk2esphome-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upk2esphome
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert Tuya device configuration to ESPHome YAML
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

