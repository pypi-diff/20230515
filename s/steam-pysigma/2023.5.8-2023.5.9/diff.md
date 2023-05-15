# Comparing `tmp/steam-pysigma-2023.5.8.tar.gz` & `tmp/steam-pysigma-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.5.8.tar", last modified: Mon May 15 09:29:21 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.5.9.tar", last modified: Mon May 15 09:46:05 2023, max compression
```

## Comparing `steam-pysigma-2023.5.8.tar` & `steam-pysigma-2023.5.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.364102 steam-pysigma-2023.5.8/
--rw-rw-rw-   0        0        0     1030 2023-05-15 09:29:21.363102 steam-pysigma-2023.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.5.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 09:29:21.364102 steam-pysigma-2023.5.8/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-05-15 09:29:00.000000 steam-pysigma-2023.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.317224 steam-pysigma-2023.5.8/steam_pysigma/
--rw-rw-rw-   0        0        0     2252 2023-05-09 08:07:19.000000 steam-pysigma-2023.5.8/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.5.8/steam_pysigma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.336101 steam-pysigma-2023.5.8/steam_pysigma/comsol/
--rw-rw-rw-   0        0        0    14576 2023-05-15 09:25:31.000000 steam-pysigma-2023.5.8/steam_pysigma/comsol/BuildComsolModel.py
--rw-rw-rw-   0        0        0    14785 2023-05-09 13:02:54.000000 steam-pysigma-2023.5.8/steam_pysigma/comsol/BuildGlobalVariables.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.8/steam_pysigma/comsol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.341101 steam-pysigma-2023.5.8/steam_pysigma/data/
--rw-rw-rw-   0        0        0     7899 2023-03-21 08:33:21.000000 steam-pysigma-2023.5.8/steam_pysigma/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     7220 2023-05-09 12:57:42.000000 steam-pysigma-2023.5.8/steam_pysigma/data/DataSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.8/steam_pysigma/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.344100 steam-pysigma-2023.5.8/steam_pysigma/domain_generator/
--rw-rw-rw-   0        0        0    17382 2023-05-04 09:30:11.000000 steam-pysigma-2023.5.8/steam_pysigma/domain_generator/GeometryMultipole.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.8/steam_pysigma/domain_generator/__init__.py
--rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.5.8/steam_pysigma/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.348101 steam-pysigma-2023.5.8/steam_pysigma/parsers/
--rw-rw-rw-   0        0        0     1673 2023-05-02 10:05:01.000000 steam-pysigma-2023.5.8/steam_pysigma/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.8/steam_pysigma/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.353101 steam-pysigma-2023.5.8/steam_pysigma/plotters/
--rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.5.8/steam_pysigma/plotters/PlotterPysigma.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.8/steam_pysigma/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.357187 steam-pysigma-2023.5.8/steam_pysigma/postprocessing/
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.8/steam_pysigma/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.5.8/steam_pysigma/postprocessing/postprocessing.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.5.8/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.361099 steam-pysigma-2023.5.8/steam_pysigma/utils/
--rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.5.8/steam_pysigma/utils/Util.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.8/steam_pysigma/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.5.8/steam_pysigma/utils/make_folder_if_not_existing.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:29:21.327264 steam-pysigma-2023.5.8/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-05-15 09:29:17.000000 steam-pysigma-2023.5.8/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      966 2023-05-15 09:29:17.000000 steam-pysigma-2023.5.8/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:29:17.000000 steam-pysigma-2023.5.8/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-05-15 09:29:17.000000 steam-pysigma-2023.5.8/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 09:29:17.000000 steam-pysigma-2023.5.8/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:05.008297 steam-pysigma-2023.5.9/
+-rw-rw-rw-   0        0        0     1030 2023-05-15 09:46:05.007296 steam-pysigma-2023.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.5.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 09:46:05.008297 steam-pysigma-2023.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-05-15 09:38:17.000000 steam-pysigma-2023.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.965543 steam-pysigma-2023.5.9/steam_pysigma/
+-rw-rw-rw-   0        0        0     2302 2023-05-15 09:37:50.000000 steam-pysigma-2023.5.9/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.5.9/steam_pysigma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.980862 steam-pysigma-2023.5.9/steam_pysigma/comsol/
+-rw-rw-rw-   0        0        0    14494 2023-05-15 09:35:20.000000 steam-pysigma-2023.5.9/steam_pysigma/comsol/BuildComsolModel.py
+-rw-rw-rw-   0        0        0    14785 2023-05-09 13:02:54.000000 steam-pysigma-2023.5.9/steam_pysigma/comsol/BuildGlobalVariables.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/comsol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.987007 steam-pysigma-2023.5.9/steam_pysigma/data/
+-rw-rw-rw-   0        0        0     7899 2023-03-21 08:33:21.000000 steam-pysigma-2023.5.9/steam_pysigma/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     7220 2023-05-09 12:57:42.000000 steam-pysigma-2023.5.9/steam_pysigma/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.990007 steam-pysigma-2023.5.9/steam_pysigma/domain_generator/
+-rw-rw-rw-   0        0        0    17382 2023-05-04 09:30:11.000000 steam-pysigma-2023.5.9/steam_pysigma/domain_generator/GeometryMultipole.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/domain_generator/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.5.9/steam_pysigma/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.993007 steam-pysigma-2023.5.9/steam_pysigma/parsers/
+-rw-rw-rw-   0        0        0     1673 2023-05-02 10:05:01.000000 steam-pysigma-2023.5.9/steam_pysigma/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.995007 steam-pysigma-2023.5.9/steam_pysigma/plotters/
+-rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.5.9/steam_pysigma/plotters/PlotterPysigma.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.998139 steam-pysigma-2023.5.9/steam_pysigma/postprocessing/
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.5.9/steam_pysigma/postprocessing/postprocessing.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.5.9/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:05.005139 steam-pysigma-2023.5.9/steam_pysigma/utils/
+-rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.5.9/steam_pysigma/utils/Util.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.5.9/steam_pysigma/utils/make_folder_if_not_existing.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.975652 steam-pysigma-2023.5.9/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      966 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.5.8/PKG-INFO` & `steam-pysigma-2023.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.5.8
+Version: 2023.5.9
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: SIGMA,STEAM,CERN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.5.8/README.md` & `steam-pysigma-2023.5.9/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/setup.py` & `steam-pysigma-2023.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.5.8",
+    version="2023.5.9",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/MainSIGMA.py` & `steam-pysigma-2023.5.9/steam_pysigma/MainSIGMA.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class MainSIGMA:
     """
         Class to generate SIGMA models
     """
 
     def __init__(self, input_file_path: str = None, model_folder: str = None, dm=None,
-                 system_settings: dict = None, verbose: bool = False):
+                 system_settings: dict = None, bh_curve_database: str = None, verbose: bool = False):
         """
               Main class for working with FiQuS simulations
               :param input_file_path: input file full path
               :param verbose: if True, more info is printed in the console
               """
         self.start_folder = os.getcwd()
         self.wrk_folder = model_folder
@@ -35,15 +35,15 @@
             self.dm = Util.FilesAndFolders.read_data_from_yaml(input_file_path, dS.DataSIGMA)
         else:
             self.dm = dm
         base_file_name = os.path.splitext(input_file_path)[0]
         self.sdm = Util.FilesAndFolders.read_data_from_yaml(f'{base_file_name}.set', dS.MultipoleSettings)
         self.roxie_data = Util.FilesAndFolders.read_data_from_yaml(f'{base_file_name}.geom', dS.SIGMAGeometry)
 
-        BuildComsolModel(self.dm, self.sdm, self.settings, self.wrk_folder, self.roxie_data)
+        BuildComsolModel(self.dm, self.sdm, self.settings, self.wrk_folder, self.roxie_data, bh_curve_database)
 
 
 if __name__ == "__main__":
     # if len(sys.argv) < 4:
     #     mp = MainFiQuS(sys.argv[1], sys.argv[2])
 
     magnet = 'MQXA_SIGMA'
```

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/comsol/BuildComsolModel.py` & `steam-pysigma-2023.5.9/steam_pysigma/comsol/BuildComsolModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,30 @@
 
 
 class BuildComsolModel:
     """
     Class take in domains and a configuration and builds a functioning comsol model saved as java.
     """
 
-    def __init__(self, model_data, input_conductor_params, settings, output_path, roxie_data):
+    def __init__(self, model_data, input_conductor_params, settings, output_path, roxie_data, bh_curve_database):
         self.g = ps.GatewaySIGMA()
         self.a = ps.ArraysSIGMA
         self.model_data = model_data
         self.output_path = output_path
         self.roxie_data = roxie_data.Roxie_Data
         self.settings_dict = dict(settings)
         self.input_conductor_params = input_conductor_params
         self.funlib_map = ps.FunLibCSVReader().read_csv_funclib_create_hashmap(self.g)
         self.COMSOL_exe_path = Path(self.settings_dict['comsolexe_path']).parent
         self.java_jdk_path = self.settings_dict['JAVA_jdk_path']
         self.COMSOL_compile_path = os.path.join(self.COMSOL_exe_path, 'comsolcompile.exe')  # Change os.join()
         self.COMSOL_batch_path = os.path.join(self.COMSOL_exe_path, 'comsolbatch.exe')
         self.COMSOL_version = os.path.basename(os.path.dirname(self.COMSOL_exe_path.parent.parent)).replace("COMSOL",
                                                                                                             "")
-        self.bh_curve_database = os.path.join(Path(self.output_path).parent, 'sources',
-                                               'roxie.bhdata')
+        self.bh_curve_database = bh_curve_database
         if self.COMSOL_version != "60" and self.COMSOL_version != "53a":
             raise Exception("Not supporting any other versions than 6.0 and 5.3a")
 
         self.model_name = f"{self.model_data.general_parameters.magnet_name}_Model"
 
         self.model_java_file_path = f"{os.path.join(self.output_path, self.model_name)}.java"
         self.compile_batch_file_path = f"{os.path.join(self.output_path, self.model_name)}_Compile_and_Open.bat"
```

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/comsol/BuildGlobalVariables.py` & `steam-pysigma-2023.5.9/steam_pysigma/comsol/BuildGlobalVariables.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/data/DataRoxieParser.py` & `steam-pysigma-2023.5.9/steam_pysigma/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/data/DataSIGMA.py` & `steam-pysigma-2023.5.9/steam_pysigma/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/domain_generator/GeometryMultipole.py` & `steam-pysigma-2023.5.9/steam_pysigma/domain_generator/GeometryMultipole.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/helpers.py` & `steam-pysigma-2023.5.9/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/parsers/ParserRoxie.py` & `steam-pysigma-2023.5.9/steam_pysigma/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/plotters/PlotterPysigma.py` & `steam-pysigma-2023.5.9/steam_pysigma/plotters/PlotterPysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/postprocessing/postprocessing.py` & `steam-pysigma-2023.5.9/steam_pysigma/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/pysigma.py` & `steam-pysigma-2023.5.9/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma/utils/Util.py` & `steam-pysigma-2023.5.9/steam_pysigma/utils/Util.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.8/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.5.9/steam_pysigma.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.5.8
+Version: 2023.5.9
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: SIGMA,STEAM,CERN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.5.8/steam_pysigma.egg-info/SOURCES.txt` & `steam-pysigma-2023.5.9/steam_pysigma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

