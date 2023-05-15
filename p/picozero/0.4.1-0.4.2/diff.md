# Comparing `tmp/picozero-0.4.1.tar.gz` & `tmp/picozero-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picozero-0.4.1.tar", last modified: Thu Dec 22 08:34:55 2022, max compression
+gzip compressed data, was "picozero-0.4.2.tar", last modified: Mon May 15 08:54:26 2023, max compression
```

## Comparing `picozero-0.4.1.tar` & `picozero-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-12-22 08:34:55.768132 picozero-0.4.1/
--rw-rw-rw-   0        0        0     1068 2022-10-12 15:09:13.000000 picozero-0.4.1/LICENSE.md
--rw-rw-rw-   0        0        0      984 2022-12-22 08:34:55.767098 picozero-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1888 2022-12-16 16:01:08.000000 picozero-0.4.1/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-22 08:34:55.749744 picozero-0.4.1/picozero/
--rw-rw-rw-   0        0        0      645 2022-12-22 08:34:18.000000 picozero-0.4.1/picozero/__init__.py
--rw-rw-rw-   0        0        0    69859 2022-12-20 18:05:42.000000 picozero-0.4.1/picozero/picozero.py
-drwxrwxrwx   0        0        0        0 2022-12-22 08:34:55.766647 picozero-0.4.1/picozero.egg-info/
--rw-rw-rw-   0        0        0      984 2022-12-22 08:34:55.000000 picozero-0.4.1/picozero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2022-12-22 08:34:55.000000 picozero-0.4.1/picozero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-22 08:34:55.000000 picozero-0.4.1/picozero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-12-22 08:34:55.000000 picozero-0.4.1/picozero.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-22 08:34:55.768775 picozero-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1470 2022-12-22 08:34:00.000000 picozero-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:54:26.819448 picozero-0.4.2/
+-rw-rw-rw-   0        0        0     1068 2023-05-15 08:53:17.000000 picozero-0.4.2/LICENSE.md
+-rw-rw-rw-   0        0        0      984 2023-05-15 08:54:26.819448 picozero-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1985 2023-05-15 08:53:17.000000 picozero-0.4.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-15 08:54:26.786107 picozero-0.4.2/picozero/
+-rw-rw-rw-   0        0        0      645 2023-05-15 08:53:37.000000 picozero-0.4.2/picozero/__init__.py
+-rw-rw-rw-   0        0        0    69868 2023-05-15 08:53:37.000000 picozero-0.4.2/picozero/picozero.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:54:26.819448 picozero-0.4.2/picozero.egg-info/
+-rw-rw-rw-   0        0        0      984 2023-05-15 08:54:26.000000 picozero-0.4.2/picozero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-15 08:54:26.000000 picozero-0.4.2/picozero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 08:54:26.000000 picozero-0.4.2/picozero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 08:54:26.000000 picozero-0.4.2/picozero.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 08:54:26.819448 picozero-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1470 2023-05-15 08:53:37.000000 picozero-0.4.2/setup.py
```

### Comparing `picozero-0.4.1/LICENSE.md` & `picozero-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `picozero-0.4.1/PKG-INFO` & `picozero-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picozero
-Version: 0.4.1
+Version: 0.4.2
 Summary: A beginner-friendly library for using common electronics components with the Raspberry Pi Pico. 
 Home-page: https://github.com/RaspberryPiFoundation/picozero
 Author: Raspberry Pi Foundation
 Author-email: learning@raspberrypi.org
 License: MIT
 Keywords: raspberry,pi,pico,electronics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `picozero-0.4.1/README.rst` & `picozero-0.4.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 -------------
 
 Documentation is available at `picozero.readthedocs.io <https://picozero.readthedocs.io>`_:
 
 - `Installation and getting started guide <https://picozero.readthedocs.io/en/latest/gettingstarted.html>`_
 - `Recipes and how-to's <https://picozero.readthedocs.io/en/latest/recipes.html>`_
 - `API <https://picozero.readthedocs.io/en/latest/api.html>`_
+- `Example code <https://github.com/RaspberryPiFoundation/picozero/tree/master/docs/examples>`_
 
 Code
 ----
 
 The code and project is at `github.com/RaspberryPiFoundation/picozero <https://github.com/RaspberryPiFoundation/picozero>`_. 
 
 Issues can be raised at `github.com/RaspberryPiFoundation/picozero/issues <https://github.com/RaspberryPiFoundation/picozero/issues>`_ (see `Contributing <https://picozero.readthedocs.io/en/latest/contributing.html>`_).
```

### Comparing `picozero-0.4.1/picozero/__init__.py` & `picozero-0.4.2/picozero/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __name__ = "picozero"
 __package__ = "picozero"
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 __author__ = "Raspberry Pi Foundation"
 
 from .picozero import (
     PWMChannelAlreadyInUse,
     EventFailedScheduleQueueFull,
 
     pinout,
```

### Comparing `picozero-0.4.1/picozero/picozero.py` & `picozero-0.4.2/picozero/picozero.py`

 * *Files 0% similar despite different names*

```diff
@@ -1539,16 +1539,16 @@
     Represents a generic input device with digital functionality e.g. buttons 
     that can be either active or inactive.
 
     :param int pin:
         The pin that the device is connected to.
 
     :param bool pull_up:
-        If :data:`True` (the default), the device will be pulled up to
-        HIGH. If :data:`False`, the device will be pulled down to LOW.
+        If :data:`True`, the device will be pulled up to HIGH. If
+        :data:`False` (the default), the device will be pulled down to LOW.
 
     :param bool active_state:
         If :data:`True` (the default), the device will return :data:`True`
         if the pin is HIGH. If :data:`False`, the device will return
         :data:`False` if the pin is LOW.
 
     :param float bounce_time:
@@ -1594,15 +1594,15 @@
         
         if self._bounce_time is not None:
             # wait for stability
             stop = ticks_ms() + (self._bounce_time * 1000)
             while ticks_ms() < stop:
                 # keep checking, reset the stop if the value changes
                 if p.value() != last_state:
-                    stop = ticks_ms() + self._bounce_time
+                    stop = ticks_ms() + (self._bounce_time * 1000)
                     last_state = p.value()
         
         # re-enable the interupt
         p.irq(self._pin_change, Pin.IRQ_RISING | Pin.IRQ_FALLING)
         
         # did the value actually change? 
         if self._state != last_state:
```

### Comparing `picozero-0.4.1/picozero.egg-info/PKG-INFO` & `picozero-0.4.2/picozero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picozero
-Version: 0.4.1
+Version: 0.4.2
 Summary: A beginner-friendly library for using common electronics components with the Raspberry Pi Pico. 
 Home-page: https://github.com/RaspberryPiFoundation/picozero
 Author: Raspberry Pi Foundation
 Author-email: learning@raspberrypi.org
 License: MIT
 Keywords: raspberry,pi,pico,electronics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `picozero-0.4.1/setup.py` & `picozero-0.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 __project__ = 'picozero'
 __packages__ = ['picozero']
 __desc__ = 'A beginner-friendly library for using common electronics components with the Raspberry Pi Pico. '
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 __author__ = "Raspberry Pi Foundation"
 __author_email__ = 'learning@raspberrypi.org'
 __license__ = 'MIT'
 __url__ = 'https://github.com/RaspberryPiFoundation/picozero'
 __keywords__ = [
     'raspberry',
     'pi',
```

