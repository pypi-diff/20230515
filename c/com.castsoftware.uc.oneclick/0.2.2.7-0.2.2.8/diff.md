# Comparing `tmp/com.castsoftware.uc.oneclick-0.2.2.7.tar.gz` & `tmp/com.castsoftware.uc.oneclick-0.2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.7.tar", last modified: Fri May 12 16:07:21 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.8.tar", last modified: Mon May 15 20:37:26 2023, max compression
```

## Comparing `com.castsoftware.uc.oneclick-0.2.2.7.tar` & `com.castsoftware.uc.oneclick-0.2.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 16:07:21.492621 com.castsoftware.uc.oneclick-0.2.2.7/
--rw-rw-rw-   0        0        0      517 2023-05-12 16:07:21.479867 com.castsoftware.uc.oneclick-0.2.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-12 16:07:21.187239 com.castsoftware.uc.oneclick-0.2.2.7/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      517 2023-05-12 16:07:21.000000 com.castsoftware.uc.oneclick-0.2.2.7/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2023-05-12 16:07:21.000000 com.castsoftware.uc.oneclick-0.2.2.7/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 16:07:21.000000 com.castsoftware.uc.oneclick-0.2.2.7/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      170 2023-05-12 16:07:21.000000 com.castsoftware.uc.oneclick-0.2.2.7/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 16:07:21.000000 com.castsoftware.uc.oneclick-0.2.2.7/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 16:07:21.316044 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/
--rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:07:21.371066 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     3454 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    19841 2023-05-12 13:25:09.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:07:21.467810 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4429 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0     7040 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     9049 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     3472 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0      491 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     6835 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     2251 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    11247 2023-05-11 12:19:40.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/main.py
--rw-rw-rw-   0        0        0     2152 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0     6039 2023-05-12 13:56:42.000000 com.castsoftware.uc.oneclick-0.2.2.7/oneclick/setup.py
--rw-rw-rw-   0        0        0      753 2023-05-12 16:07:05.000000 com.castsoftware.uc.oneclick-0.2.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 16:07:21.493623 com.castsoftware.uc.oneclick-0.2.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 20:37:26.067985 com.castsoftware.uc.oneclick-0.2.2.8/
+-rw-rw-rw-   0        0        0      517 2023-05-15 20:37:26.056528 com.castsoftware.uc.oneclick-0.2.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-15 20:37:25.745651 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 20:37:25.000000 com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 20:37:25.890416 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/
+-rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:37:25.947856 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     3914 2023-05-13 12:48:37.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    19803 2023-05-15 16:57:12.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:37:26.047175 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4432 2023-05-13 21:26:47.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0     7052 2023-05-13 21:24:21.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     8411 2023-05-15 20:34:04.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     3472 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0      491 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     6835 2023-05-13 12:48:23.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     2251 2023-05-12 17:11:00.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    10978 2023-05-13 14:37:06.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/main.py
+-rw-rw-rw-   0        0        0     2152 2023-05-15 16:56:38.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0     6003 2023-05-15 13:33:19.000000 com.castsoftware.uc.oneclick-0.2.2.8/oneclick/setup.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 20:36:44.000000 com.castsoftware.uc.oneclick-0.2.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 20:37:26.068987 com.castsoftware.uc.oneclick-0.2.2.8/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.7
+Version: 0.2.2.8
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.7
+Version: 0.2.2.8
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com.castsoftware.uc.oneclick-0.2.2.8/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/aip_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/aip_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/highlight_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/highlight_analysis.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,16 +24,21 @@
             for appl in config.application:
                 hl_status = config.application[appl]['hl']
                 if hl_status == '' or hl_status.startswith('Error'):
 
                     cls._log.info(f'Running Highlight analysis for {config.project_name}\{appl}')
                     app_id = rest.get_app_id(appl)
                     if app_id is None:
-                        cls._log.error(f'Application {appl} not found in Highlight')
-                        continue
+                        cls._log.info(f'Application {appl} not found in Highlight, Creating Application {appl}...')
+                        resp_code = rest.create_an_app(config.hl_url, config.hl_instance, appl)
+                        if resp_code == 200:
+                            cls._log.info(f'Application {appl} created inside Highlight.')
+                            app_id = rest.get_app_id(appl)
+                        else:
+                            cls._log.info(f'Not able to Application {appl} inside Highlight due to some error!')                       
 
                     hl_sourceDir = f'{config.base}\\STAGED\\HL\\{config.project_name}\\{appl}'
                     hl_workingDir = f'{config.oneclick_work}\\{config.project_name}\\HL_ANALYSIS_RESULT\\{appl}'
                     create_folder(f'{config.oneclick_work}\\{config.project_name}\\HL_ANALYSIS_RESULT')
                     create_folder(hl_workingDir)
                     java_home = config.java_home
                     if len(java_home) > 0:
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/analysis/trackAnalysis.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/config.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         if not exists(abspath(args.baseFolder)):
             raise InvalidConfigNoBase(f'Base folder must exist: {args.baseFolder}')
 
         base_config=abspath(f'{args.baseFolder}/.oneclick/config.json')
         if not exists(base_config) and args.command == 'run':
             raise NoConfigFound('Base configuration file found, please run with the "config" option')
 
+
         if args.command == 'config':
             if not exists(base_config):
                 self._config={}
                 self._config_file=base_config
                 self.base = args.baseFolder
             else: 
                 if args.projectName is None:
@@ -94,22 +95,22 @@
             except AttributeError as e:
                 self.log.debug(str(e))
             return
 
         #do all required fields contain data
         if args.command == 'run':
             try:
+                self._config={}
                 self._config_file = abspath(f'{args.baseFolder}/.oneclick/{args.projectName}.json')
                 if exists(self._config_file):
                     with open(abspath(self._config_file), 'rb') as config_file:
                         self._config = load(config_file)
                 else:
                     with open(base_config) as config_file:
                         self._config = load(config_file)
-                    self._save()
 
                 self.base=args.baseFolder
                 self.project = args.projectName
                 self.company_name = args.companyName
 
                 self.start=args.start
                 self.start=args.end
@@ -125,15 +126,15 @@
                 msg = str(e)
                 self.log.error(msg)
                 exit()
 
     def validate_for_run(self):
         if self.cloc_version == '':
             raise InvalidConfiguration('Missing CLOC executable name')
-        exec = f'{getcwd()}\\scripts\\{self.cloc_version}'
+        exec = abspath(f'{self.base}\\scripts\\{self.cloc_version}')
         if not exists(exec):
             raise InvalidConfiguration(f'CLOC executable not found: {exec}')
         if not self.is_console_active and not self.is_hl_active:
             raise InvalidConfiguration('Both Hightlight and AIP configureations are incomplete, at least one must be')
 
 
     def check_default(self,arg_value,cfg_value,default_value) -> bool:
@@ -533,25 +534,23 @@
     @property
     def email_subject(self):
         return self.email['subject'] 
 
     """ **************** Setting related entries ************************ """
     @property 
     def setting(self):
-        if 'setting' not in self._config:
-            self._config['setting']={}
-        return self._config['setting']
+        return self._get(self._config,'setting',{})        
 
     @property
     def arg_template(self):
         return self._get(self.setting,'arg-template')
 
     @property
     def base(self):
-        return self.setting['base']
+        return self._get(self.setting,'base','')
     @base.setter
     def base(self,value):
         if value is not None:
             self.setting['base']=value
             self._save()
 
     @property
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/cleanup.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/cleanup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def run(cls,config:Config):
         cls._log.debug('Source Code cleanup is in progress')
         
         output_path = f'{config.oneclick_work}/{config.project_name}/LOGS'    
         #create_folder(output_path)
 
-        dir = getcwd()
+        dir = config.base
         dateTimeObj=datetime.now()
         file_suffix=dateTimeObj.strftime("%d-%b-%Y(%H.%M.%S.%f)")
         
         exclusionFileList= f'{dir}\\scripts\\{cls.cleanup_file_prefix}deleteFileList.txt'
         with open(exclusionFileList) as f:
             files_list = f.read().splitlines()
             f.close()
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/cloc.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/cloc.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,31 +39,30 @@
         return f'{cls.cloc_base}\\{cls.config.project_name}'
 
     @property
     def cloc_results(cls):
         return cls._df
 
     def _run_cloc(cls,work_folder:str,cloc_output:str,cloc_output_ignored:str):
-        cloc_path=abspath(f'{getcwd()}\\scripts\\{cls.config.cloc_version}')
-        args = [cloc_path,work_folder,"--report-file",cloc_output,"--ignored",cloc_output_ignored,"--quiet"]
+        args = [cls.cloc_path,work_folder,"--report-file",cloc_output,"--ignored",cloc_output_ignored,"--quiet"]
         proc = run_process(args,False)
 
         sleep(10)
         if proc.poll() is not None and exists(cloc_output):
             return 'DONE'
         else:
             return proc
 
     def open_excel_writer(cls,config:Config):
         ClocPreCleanup.writer = ExcelWriter(abspath(f'{config.report}/{config.project_name}/{config.project_name}-cloc.xlsx'), engine='xlsxwriter')
 
     def run(cls,config:Config):
         cls.open_excel_writer(config)
-
-        list_of_tech_file=abspath(f'{getcwd()}\\scripts\\ListOfTechnologies.csv')
+        cls.cloc_path=abspath(f'{config.base}\\scripts\\{cls.config.cloc_version}')
+        list_of_tech_file=abspath(f'{config.base}\\scripts\\ListOfTechnologies.csv')
         with open(list_of_tech_file) as f:
             tech_list = f.read().splitlines()
             f.close()
 
         process = {}
         cloc_run=False
         for appl in config.application:
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/discoveryReport.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/discoveryReport.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pandas
 from oneclick.discovery.sourceValidation import SourceValidation 
 from pandas import DataFrame,read_excel
 from os.path import abspath
 import docx
 from oneclick.config import Config
 from cast_common.util import convert_LOC
-from docx.enum.table import WD_TABLE_ALIGNMENT
 
 #todo: add totals to the cloc report (d1)
 #todo: if SQL problems, add bullet under SQL Delivery to describe (d1)
 
 class DiscoveryReport(SourceValidation):
 
     def __init__(cls, config:Config, log_level:int):
@@ -54,43 +53,43 @@
             before_df = cls.cloc_report(cloc_report,f'Before({appl})')
             #print(before_df)
 
             filt=(before_df['APPLICABLE']==False)
             l=before_df.loc[filt,['LANGUAGE','CODE']].sort_values(by=['CODE'], ascending=False) 
             non_code=''
             if len(l) == 1:
-                non_code= str(l.iloc[0]['CODE']//1000) +' KLoc of '+ l.iloc[0]['LANGUAGE']
+                non_code= str(l.iloc[0]['CODE']//1000) +' KLOC of '+ l.iloc[0]['LANGUAGE']
             elif len(l) > 1:
-                non_code= str(l.iloc[0]['CODE']//1000) +' KLoc of '+ l.iloc[0]['LANGUAGE'] +' non code files and ~'+ str(l.iloc[1]['CODE']//1000) +' KLOC of '+ l.iloc[1]['LANGUAGE']
+                non_code= str(l.iloc[0]['CODE']//1000) +' KLOC of '+ l.iloc[0]['LANGUAGE'] +' non code files and ~'+ str(l.iloc[1]['CODE']//1000) +' KLOC of '+ l.iloc[1]['LANGUAGE']
 
             # read by 'Stats After Code CleanUP' sheet of an Cloc_Output excel file
             after_df = cls.cloc_report(cloc_report,f'After({appl})')
             #print(after_df)
 
             # read by 'Summary' sheet of an SQL_Output excel file
             sql_df = read_excel(sql_report,sheet_name='Summary')
             #sql_df = sql_df[sql_df['Total']>0]
 
             doc.add_heading(f'Application {appl} :', 2)
 
             # out of scope code base
             total = int(before_df['CODE'].sum())
             total, unit = convert_LOC(total)
-            doc.add_paragraph(f"This delivery contains a total of {len(before_df)-1} technologies/extensions discovered with a total of {total} {unit}.",style='List Bullet')
+            doc.add_paragraph(f"This delivery contains a total of {len(after_df)-1} technologies/extensions discovered with a total of {total} {unit}.",style='List Bullet')
 
-            bsuport = before_df[before_df['APPLICABLE']==True]
+            bsuport = after_df[after_df['APPLICABLE']==True]
             total = int(bsuport['CODE'].sum())
             total, unit = convert_LOC(total)
 
             lang_list = list(bsuport['LANGUAGE'])
             lang_list[-1]=f'and {lang_list[-1]}'
             bsup_lang = ', '.join(lang_list)
             doc.add_paragraph(f"{len(bsuport)} technologies/extensions are relevant for the CAST analysis, which include {bsup_lang}.",style='List Bullet')
 
-            nsuport = before_df[before_df['APPLICABLE']==False]
+            nsuport = after_df[after_df['APPLICABLE']==False]
             total = int(bsuport['CODE'].sum())
             total, unit = convert_LOC(total)
 
             lang_list = list(nsuport['LANGUAGE'])
             lang_list[-1]=f'and {lang_list[-1]}'
             bsup_lang = ', '.join(lang_list)
             doc.add_paragraph(f"The remaining {len(nsuport)} technologies/extensions are not relevant and will not be analyzed. These include {bsup_lang}.",style='List Bullet')
@@ -126,48 +125,39 @@
 
             # line = []
             # for index, row in sql_df.iterrows():
             #     line.append(f"{row['Unique']} {row['Catagory']}")
             #     if row['Catagory'] == 'SQL files':
             #         line[-1]=f'in {line[-1]}'
             #doc.add_paragraph(f"The delivery also inclues, {', '.join(line)}.",style='List Bullet')
-            removed_code=(before_df['CODE'].sum()-after_df['CODE'].sum())//1000
-            doc.add_paragraph(f'We removed {removed_code} KLoc of sample, test and other non-production code from the source code.',style='List Bullet')
+            removed_code=before_df['CODE'].sum()-after_df['CODE'].sum()
+            doc.add_paragraph(f'We removed {removed_code} KLOC of sample, test and other non-production code from the source code.',style='List Bullet')
             after_df=after_df.drop(after_df[after_df['APPLICABLE']==0.0].index)
             total = after_df['CODE'].sum()//1000
-            doc.add_paragraph(f"Here is a high-level summary of the source code that will be analyzed by CAST, totaling {total} KLoc.",style='List Bullet')
+            doc.add_paragraph(f"Here is a high-level summary of the source code that will be analyzed by CAST, totaling {total} KLOC.",style='List Bullet')
 
             after_df = after_df[['LANGUAGE','FILES','CODE']]
             after_df = after_df[:-1]
             files_count=after_df['FILES'].sum()
             code_count=after_df['CODE'].sum()
             new_row = pandas.DataFrame({'LANGUAGE':'Totals', 'FILES':[files_count], 'CODE':[code_count]})
             after_df = pandas.concat([after_df,new_row])
-
+            
             t = doc.add_table(after_df.shape[0]+1, after_df.shape[1])
             # add the header rows.
             for j in range(after_df.shape[-1]):
                 t.cell(0,j).text = after_df.columns[j]
-                if j==0:
-                    t.cell(0,j).paragraphs[0].paragraph_format.alignment = WD_TABLE_ALIGNMENT.LEFT
-                else:
-                    t.cell(0,j).paragraphs[0].paragraph_format.alignment = WD_TABLE_ALIGNMENT.RIGHT
 
             # add the rest of the data frame
             for i in range(after_df.shape[0]):
                 for j in range(after_df.shape[-1]):
                     number = after_df.values[i,j]
                     if type(number) is int:
-                        number = "{:,}".format(number)
-                    if j==0:
-                        t.cell(i+1,j).text = str(number)
-                        t.cell(i+1,j).paragraphs[0].paragraph_format.alignment = WD_TABLE_ALIGNMENT.LEFT
-                    else:
-                        t.cell(i+1,j).text = str(number)
-                        t.cell(i+1,j).paragraphs[0].paragraph_format.alignment = WD_TABLE_ALIGNMENT.RIGHT
+                        number = "{}".format(number)
+                    t.cell(i+1,j).text = number
             
             # Adding style to a table
             t.style = 'Medium Shading 1 Accent 1'
 
         # now save the document to a location
         doc.save(discovery_report)
         cls._log.info(f'Source Code Discovery report has been written to {discovery_report}')
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/prep.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/prep.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/sqlDiscovery.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/sqlDiscovery.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/discovery/unzip.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/discovery/unzip.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/main.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,27 +36,15 @@
 def get_argparse_defaults(parser):
     defaults = {}
     for action in parser._actions:
         if not action.required and action.dest != "help":
             defaults[action.dest] = action.default
     return defaults
 
-
-#TODO: d2-Ability to install onclick with all its components via PIP (d2)
-#TODO: d1-send emails (d1-SHP)
-if __name__ == '__main__':
-
-    #printing some inital messages to the user
-    log_level = INFO
-    log = Logger("main")
-
-    print('\nCAST One Click')
-    print('Copyright (c) 2023 CAST Software Inc.\n')
-    print('If you need assistance, please contact Technical Due Diligence @team.ddassessment@castsoftware.com\n')
-
+def command_line() -> ArgumentParser:
     parser = ArgumentParser(prog='OneClick',  formatter_class=lambda prog: FlexiFormatter(prog, width=99999, max_help_position=60))
     subparsers = parser.add_subparsers(title='command',dest='command')
 
     """
         configure default json to be used with all projects going forward
     """
     config_parser = subparsers.add_parser('config')
@@ -119,17 +107,39 @@
     run_parser.add_argument('-p','--projectName', help='Name of the project')
 
     run_parser.add_argument('--start',choices=['Analysis','Report'],default='Discovery',help='Start from catagory')
     run_parser.add_argument('--end',choices=['Discovery','Analysis','Report'],default='Report',help='End after catagory')
 
     run_parser.add_argument('-d','--debug',  default=False,type=bool)
 
+    return parser,config_parser
+
+#TODO: d2-Ability to install onclick with all its components via PIP (d2)
+#TODO: d1-send emails (d1-SHP)
+if __name__ == '__main__':
+
+
+    print('\nCAST One Click')
+    print('Copyright (c) 2023 CAST Software Inc.\n')
+    print('If you need assistance, please contact Technical Due Diligence @team.ddassessment@castsoftware.com\n')
+
+
+    parser,config_parser = command_line()
     default_args = get_argparse_defaults(config_parser)
     args = parser.parse_args()
 
+    #printing some inital messages to the user
+    file_name=abspath(f'{args.baseFolder}/ONECLICK_WORK')
+    create_folder(file_name)
+    file_name=abspath(f'{file_name}/LOGS')
+    create_folder(file_name)
+    file_name=abspath(f'{file_name}/general.log')
+    
+    log_level = INFO
+    log = Logger("main",file_name=file_name)
     log.info(f'Running {args.command}')
 
     config = NotImplemented
     try:
         config=Config(parser,default_args)
         if args.command == 'config':
             file = ''
@@ -161,26 +171,14 @@
 
         log.info('To update the default configuraiton file use')
         log.info(f'     OneClick config {cfg}')
         log.info('To update the application configuraiton file use:')
         log.info(f'     OneClick config -p {config.project_name} {cfg}')
         exit()
 
-
-    # parser.add_argument('-c','--companyName',  default='Company Name', help='Name of the project')
-    # parser.add_argument('--JavaHome',  help='Location of the JRE')
-    # parser.add_argument('--from-email',  help='Email sending from')
-    # parser.add_argument('--from-to',  help='Email sending from')
-    # parser.add_argument('--from-email',  help='Email sending from')
-    # parser.add_argument('--from-email',  help='Email sending from')
-
-    # TODO: add args for aip and console rest setup (d2)
-    # TODO: add arg to reset analysis status for specific application (d2)
-
-    #args = parser.parse_args()
     if args.debug:
         log_level=DEBUG
 
     create_folder(abspath(f'{config.base}/STAGED'))
     create_folder(abspath(config.work))
     #create_folder(abspath(config.logs))
     #create_folder(abspath(f'{config.logs}/{config.project_name}'))
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/runArg.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/runArg.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/sendEmail.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/oneclick/setup.py` & `com.castsoftware.uc.oneclick-0.2.2.8/oneclick/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,19 +112,20 @@
         if yes_no_input('Are both "AIP Console Enterprise Edition" and the matching "AIP Console automation tools" installed?'):
             print ('\nConfiguring for AIP Console')
             config.console_url = url_input('\t"AIP Console Enterprise Edition" URL',config.console_url)
             config.console_cli = folder_input('\t"AIP Console automation tools" location',dirname(config.console_cli),"aip-console-tools-cli.jar",True)
             config.console_key = string_input('\t"AIP Console Enterprise Edition" Key',config.console_key)
             config.enable_security_assessment = yes_no_input('\tEnable security analysis',config.enable_security_assessment)
             config.blueprint = yes_no_input('\tEnable Blueprint analysis',config.blueprint)
-            if config.is_console_active:
-                print ('AIP Console configuration complete')
-            else:
-                print ('Error updating AIP Console configuration!')
-            print ('\n')
+
+        if config.is_console_active:
+            print ('AIP Console configuration complete')
+        else:
+            print ('Error updating AIP Console configuration!')
+        print ('\n')
     
     if yes_no_input('Configure Highlight automatic scans'):
         if yes_no_input('Are both the Highlight Agent and Command Line Interface installed?'):
             print ('\nConfiguring for Highlight')
             if len(config.hl_url)==0:
                 config.hl_url = "https://rpa.casthighlight.com/"
             config.hl_url = url_input('\tHighlight URL',config.hl_url)
@@ -134,16 +135,16 @@
             config.hl_cli = folder_input('\tHighlight command line interface installation location',config.hl_cli,'HighlightAutomation.jar',True)
             
             agent_folder = f'{config.perl_install_dir}'.replace('\\strawberry\\perl','')
             agent_folder = folder_input('\tHighlight agent installation location',agent_folder,'strawberry',False)
             config.perl_install_dir=abspath(f'{agent_folder}/strawberry/perl')
             config.analyzer_dir=abspath(f'{agent_folder}/perl')
 
-            if config.is_console_active:
-                print ('Highlight configuration complete')
-            else:
-                print ('Error updating Highlight configuration!')
-            print ('\n')
+        if config.is_highlight_active:
+            print ('Highlight configuration complete')
+        else:
+            print ('Error updating Highlight configuration!')
+        print ('\n')
 
 
         pass
     pass
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.7/pyproject.toml` & `com.castsoftware.uc.oneclick-0.2.2.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='0.2.2.7' #prod version
+version='0.2.2.8' #prod version
 dependencies = [
     'pandas==1.4.0','python-pptx==0.6.18','python-docx','argparse_formatter',
     'django',
-    'com.castsoftware.uc.python.common>=0.1.11',
+    'com.castsoftware.uc.python.common==1.0.1',
     'com.castsoftware.uc.action-plan',
     'com.castsoftware.uc.arg'
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

