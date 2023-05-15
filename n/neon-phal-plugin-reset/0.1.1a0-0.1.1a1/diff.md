# Comparing `tmp/neon-phal-plugin-reset-0.1.1a0.tar.gz` & `tmp/neon-phal-plugin-reset-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-reset-0.1.1a0.tar", last modified: Fri May 12 19:14:05 2023, max compression
+gzip compressed data, was "neon-phal-plugin-reset-0.1.1a1.tar", last modified: Mon May 15 20:22:13 2023, max compression
```

## Comparing `neon-phal-plugin-reset-0.1.1a0.tar` & `neon-phal-plugin-reset-0.1.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/create_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-12 19:14:04.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 19:14:05.000000 neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:14:05.542487 neon-phal-plugin-reset-0.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-12 19:14:01.000000 neon-phal-plugin-reset-0.1.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:13.750777 neon-phal-plugin-reset-0.1.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-15 20:22:08.000000 neon-phal-plugin-reset-0.1.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 20:22:08.000000 neon-phal-plugin-reset-0.1.1a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-15 20:22:13.750777 neon-phal-plugin-reset-0.1.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-15 20:22:08.000000 neon-phal-plugin-reset-0.1.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:13.746777 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-05-15 20:22:08.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-15 20:22:08.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-15 20:22:08.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset/create_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-15 20:22:11.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:13.750777 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-15 20:22:13.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-15 20:22:13.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:22:13.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 20:22:13.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-15 20:22:13.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 20:22:13.000000 neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:22:13.750777 neon-phal-plugin-reset-0.1.1a1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-15 20:22:08.000000 neon-phal-plugin-reset-0.1.1a1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:22:13.750777 neon-phal-plugin-reset-0.1.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-15 20:22:08.000000 neon-phal-plugin-reset-0.1.1a1/setup.py
```

### Comparing `neon-phal-plugin-reset-0.1.1a0/LICENSE.md` & `neon-phal-plugin-reset-0.1.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.1.1a0/PKG-INFO` & `neon-phal-plugin-reset-0.1.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description: # Neon Reset Plugin
         Plugin to handle factory reset requests. Note that this plugin will install system
```

### Comparing `neon-phal-plugin-reset-0.1.1a0/README.md` & `neon-phal-plugin-reset-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/__init__.py` & `neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,16 +108,16 @@
 
         # Contents are now at /tmp/neon/neon-image-recipe
         try:
             if message.data.get('skill_config'):
                 LOG.debug("Updating skill config from default")
                 Popen(["/usr/bin/cp", "-r",
                        "/tmp/neon/neon-image-recipe/05_neon_core"
-                       "/overlay/home/neon/.config/neon",
-                       "/home/neon/.config/"])
+                       "/overlay/home/neon/.config/neon/skills",
+                       "/home/neon/.config/neon/"])
                 Popen("chown -R neon:neon /home/neon", shell=True)
             if message.data.get('core_config'):
                 LOG.debug("Updating system config from default")
                 move("/tmp/neon/neon-image-recipe/05_neon_core/overlay"
                      "/etc/neon/neon.yaml", "/etc/neon/neon.yaml")
             LOG.info(f"Restored default configuration")
             rmtree("/tmp/neon/neon-image-recipe")
```

### Comparing `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/config.py` & `neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset/config.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/create_media.py` & `neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset/create_media.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset/version.py` & `neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a0"
+__version__ = "0.1.1a1"
```

### Comparing `neon-phal-plugin-reset-0.1.1a0/neon_phal_plugin_reset.egg-info/PKG-INFO` & `neon-phal-plugin-reset-0.1.1a1/neon_phal_plugin_reset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description: # Neon Reset Plugin
         Plugin to handle factory reset requests. Note that this plugin will install system
```

### Comparing `neon-phal-plugin-reset-0.1.1a0/setup.py` & `neon-phal-plugin-reset-0.1.1a1/setup.py`

 * *Files identical despite different names*

