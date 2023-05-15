# Comparing `tmp/phenospy-0.17.tar.gz` & `tmp/phenospy-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenospy-0.17.tar", last modified: Fri Apr 21 08:01:34 2023, max compression
+gzip compressed data, was "phenospy-0.18.tar", last modified: Mon May 15 19:26:28 2023, max compression
```

## Comparing `phenospy-0.17.tar` & `phenospy-0.18.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-21 08:01:34.568066 phenospy-0.17/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1080 2023-03-13 19:55:04.000000 phenospy-0.17/LICENSE.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       31 2023-03-13 20:40:28.000000 phenospy-0.17/MANIFEST.in
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-04-21 08:01:34.567899 phenospy-0.17/PKG-INFO
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2539 2023-04-18 19:03:17.000000 phenospy-0.17/README.md
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-21 08:01:34.564796 phenospy-0.17/phenospy/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      370 2023-04-03 16:35:02.000000 phenospy-0.17/phenospy/__init__.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18969 2023-04-17 16:25:07.000000 phenospy-0.17/phenospy/nl_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1109 2023-04-03 16:31:49.000000 phenospy-0.17/phenospy/nl_owlToMd.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2258 2023-04-03 16:50:14.000000 phenospy-0.17/phenospy/nl_owlToMd_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2403 2023-03-28 14:23:07.000000 phenospy-0.17/phenospy/owl_make_phsOntology.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      631 2023-03-28 17:14:38.000000 phenospy-0.17/phenospy/owl_owlready_config.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     4013 2023-03-28 18:24:24.000000 phenospy-0.17/phenospy/owl_xml2owl_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    16941 2023-04-21 08:00:08.000000 phenospy-0.17/phenospy/owl_xmlToOwl.py
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-21 08:01:34.567674 phenospy-0.17/phenospy/package-data/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6148 2023-03-28 19:11:16.000000 phenospy-0.17/phenospy/package-data/.DS_Store
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      591 2023-03-27 19:35:46.000000 phenospy-0.17/phenospy/package-data/phenoscript.obda
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18495 2023-03-27 19:35:46.000000 phenospy-0.17/phenospy/package-data/phenoscript.owl
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      127 2023-03-27 19:35:46.000000 phenospy-0.17/phenospy/package-data/phenoscript.properties
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3224 2023-04-19 08:58:27.000000 phenospy-0.17/phenospy/package-data/phs-config.yaml
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7502 2023-03-27 17:52:38.000000 phenospy-0.17/phenospy/package-data/snippets-default.json
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1065 2023-03-15 14:43:16.000000 phenospy-0.17/phenospy/phs_addXmlMeta.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5390 2023-03-28 18:02:16.000000 phenospy-0.17/phenospy/phs_grammar.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2232 2023-03-28 18:15:48.000000 phenospy-0.17/phenospy/phs_mainConvert.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3898 2023-03-28 18:28:37.000000 phenospy-0.17/phenospy/phs_parser_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3153 2023-03-28 18:28:31.000000 phenospy-0.17/phenospy/phs_various_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    14872 2023-03-28 18:12:47.000000 phenospy-0.17/phenospy/phs_xml.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6508 2023-03-28 18:13:03.000000 phenospy-0.17/phenospy/phs_xmlTranslateTerms.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7009 2023-03-28 17:14:38.000000 phenospy-0.17/phenospy/snips_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    10953 2023-04-19 14:00:48.000000 phenospy-0.17/phenospy/snips_makeFromYaml.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5312 2023-04-19 15:37:02.000000 phenospy-0.17/phenospy/snips_readFromJSON.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2366 2023-04-17 06:49:33.000000 phenospy-0.17/phenospy/xml_recodeThis.py
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-21 08:01:34.566097 phenospy-0.17/phenospy.egg-info/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-04-21 08:01:34.000000 phenospy-0.17/phenospy.egg-info/PKG-INFO
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      944 2023-04-21 08:01:34.000000 phenospy-0.17/phenospy.egg-info/SOURCES.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        1 2023-04-21 08:01:34.000000 phenospy-0.17/phenospy.egg-info/dependency_links.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       43 2023-04-21 08:01:34.000000 phenospy-0.17/phenospy.egg-info/requires.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        9 2023-04-21 08:01:34.000000 phenospy-0.17/phenospy.egg-info/top_level.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       38 2023-04-21 08:01:34.568118 phenospy-0.17/setup.cfg
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1238 2023-04-21 08:00:56.000000 phenospy-0.17/setup.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-05-15 19:26:28.436832 phenospy-0.18/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1080 2023-03-13 19:55:04.000000 phenospy-0.18/LICENSE.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       31 2023-03-13 20:40:28.000000 phenospy-0.18/MANIFEST.in
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-05-15 19:26:28.436655 phenospy-0.18/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2539 2023-04-18 19:03:17.000000 phenospy-0.18/README.md
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-05-15 19:26:28.432045 phenospy-0.18/phenospy/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      370 2023-04-03 16:35:02.000000 phenospy-0.18/phenospy/__init__.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    19013 2023-05-15 19:21:52.000000 phenospy-0.18/phenospy/nl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1109 2023-04-03 16:31:49.000000 phenospy-0.18/phenospy/nl_owlToMd.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2258 2023-04-03 16:50:14.000000 phenospy-0.18/phenospy/nl_owlToMd_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2403 2023-03-28 14:23:07.000000 phenospy-0.18/phenospy/owl_make_phsOntology.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      631 2023-03-28 17:14:38.000000 phenospy-0.18/phenospy/owl_owlready_config.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     4013 2023-03-28 18:24:24.000000 phenospy-0.18/phenospy/owl_xml2owl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    16941 2023-04-21 08:00:08.000000 phenospy-0.18/phenospy/owl_xmlToOwl.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-05-15 19:26:28.436270 phenospy-0.18/phenospy/package-data/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6148 2023-03-28 19:11:16.000000 phenospy-0.18/phenospy/package-data/.DS_Store
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      591 2023-03-27 19:35:46.000000 phenospy-0.18/phenospy/package-data/phenoscript.obda
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18495 2023-03-27 19:35:46.000000 phenospy-0.18/phenospy/package-data/phenoscript.owl
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      127 2023-03-27 19:35:46.000000 phenospy-0.18/phenospy/package-data/phenoscript.properties
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3224 2023-04-19 08:58:27.000000 phenospy-0.18/phenospy/package-data/phs-config.yaml
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7502 2023-03-27 17:52:38.000000 phenospy-0.18/phenospy/package-data/snippets-default.json
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1065 2023-03-15 14:43:16.000000 phenospy-0.18/phenospy/phs_addXmlMeta.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5390 2023-03-28 18:02:16.000000 phenospy-0.18/phenospy/phs_grammar.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2232 2023-03-28 18:15:48.000000 phenospy-0.18/phenospy/phs_mainConvert.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3898 2023-03-28 18:28:37.000000 phenospy-0.18/phenospy/phs_parser_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3153 2023-03-28 18:28:31.000000 phenospy-0.18/phenospy/phs_various_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    14872 2023-03-28 18:12:47.000000 phenospy-0.18/phenospy/phs_xml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6508 2023-03-28 18:13:03.000000 phenospy-0.18/phenospy/phs_xmlTranslateTerms.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7009 2023-03-28 17:14:38.000000 phenospy-0.18/phenospy/snips_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    10953 2023-04-19 14:00:48.000000 phenospy-0.18/phenospy/snips_makeFromYaml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5312 2023-04-19 15:37:02.000000 phenospy-0.18/phenospy/snips_readFromJSON.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2366 2023-04-17 06:49:33.000000 phenospy-0.18/phenospy/xml_recodeThis.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-05-15 19:26:28.433766 phenospy-0.18/phenospy.egg-info/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-05-15 19:26:28.000000 phenospy-0.18/phenospy.egg-info/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      944 2023-05-15 19:26:28.000000 phenospy-0.18/phenospy.egg-info/SOURCES.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        1 2023-05-15 19:26:28.000000 phenospy-0.18/phenospy.egg-info/dependency_links.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       43 2023-05-15 19:26:28.000000 phenospy-0.18/phenospy.egg-info/requires.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        9 2023-05-15 19:26:28.000000 phenospy-0.18/phenospy.egg-info/top_level.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       38 2023-05-15 19:26:28.436885 phenospy-0.18/setup.cfg
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1238 2023-05-15 19:23:55.000000 phenospy-0.18/setup.py
```

### Comparing `phenospy-0.17/LICENSE.txt` & `phenospy-0.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/PKG-INFO` & `phenospy-0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.17
+Version: 0.18
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `phenospy-0.17/README.md` & `phenospy-0.18/README.md`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/nl_fun.py` & `phenospy-0.18/phenospy/nl_fun.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,16 @@
         item['E0'].phs_NL.append(txt)
         # print("NL:", item['E0'].phs_NL)
         # return(dic_mesuare)
     #
     # DELETE
     # dic_mesuare
     for item in dic_mesuare:
-        destroy_ListEntities([item['Q'], item['Unit']])
+        # destroy_ListEntities([item['Q'], item['Unit']])
+        destroy_ListEntities([item['Q']])
         if item['x'] is not None:
             # print(item['x'])
             destroy_entity(item['x'])
 
 # destroy list entitities from sparql query
 def destroy_ListEntities(list):
     for entity in list:
```

### Comparing `phenospy-0.17/phenospy/nl_owlToMd.py` & `phenospy-0.18/phenospy/nl_owlToMd.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/nl_owlToMd_fun.py` & `phenospy-0.18/phenospy/nl_owlToMd_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/owl_make_phsOntology.py` & `phenospy-0.18/phenospy/owl_make_phsOntology.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/owl_owlready_config.py` & `phenospy-0.18/phenospy/owl_owlready_config.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/owl_xml2owl_fun.py` & `phenospy-0.18/phenospy/owl_xml2owl_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/owl_xmlToOwl.py` & `phenospy-0.18/phenospy/owl_xmlToOwl.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/package-data/.DS_Store` & `phenospy-0.18/phenospy/package-data/.DS_Store`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/package-data/phenoscript.obda` & `phenospy-0.18/phenospy/package-data/phenoscript.obda`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/package-data/phenoscript.owl` & `phenospy-0.18/phenospy/package-data/phenoscript.owl`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/package-data/phs-config.yaml` & `phenospy-0.18/phenospy/package-data/phs-config.yaml`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/package-data/snippets-default.json` & `phenospy-0.18/phenospy/package-data/snippets-default.json`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/phs_addXmlMeta.py` & `phenospy-0.18/phenospy/phs_addXmlMeta.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/phs_grammar.py` & `phenospy-0.18/phenospy/phs_grammar.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/phs_mainConvert.py` & `phenospy-0.18/phenospy/phs_mainConvert.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/phs_parser_fun.py` & `phenospy-0.18/phenospy/phs_parser_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/phs_various_fun.py` & `phenospy-0.18/phenospy/phs_various_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/phs_xml.py` & `phenospy-0.18/phenospy/phs_xml.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/phs_xmlTranslateTerms.py` & `phenospy-0.18/phenospy/phs_xmlTranslateTerms.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/snips_fun.py` & `phenospy-0.18/phenospy/snips_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/snips_makeFromYaml.py` & `phenospy-0.18/phenospy/snips_makeFromYaml.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/snips_readFromJSON.py` & `phenospy-0.18/phenospy/snips_readFromJSON.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy/xml_recodeThis.py` & `phenospy-0.18/phenospy/xml_recodeThis.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/phenospy.egg-info/PKG-INFO` & `phenospy-0.18/phenospy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.17
+Version: 0.18
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `phenospy-0.17/phenospy.egg-info/SOURCES.txt` & `phenospy-0.18/phenospy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.17/setup.py` & `phenospy-0.18/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phenospy',
-    version='0.17',
+    version='0.18',
     packages=find_packages(exclude=['tests*', 'devel*', 'build*']),
     license='MIT',
     description='Tools for making and processing computable phenotype descriptions',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     install_requires=['Owlready2',
                       'PyYAML',
```

