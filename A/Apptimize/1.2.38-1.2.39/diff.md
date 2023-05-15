# Comparing `tmp/Apptimize-1.2.38.tar.gz` & `tmp/Apptimize-1.2.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Apptimize-1.2.38.tar", last modified: Tue Mar 21 18:46:29 2023, max compression
+gzip compressed data, was "dist/Apptimize-1.2.39.tar", last modified: Fri May 12 14:57:17 2023, max compression
```

## Comparing `Apptimize-1.2.38.tar` & `Apptimize-1.2.39.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-21 18:46:29.000000 Apptimize-1.2.38/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-21 18:46:29.000000 Apptimize-1.2.38/Apptimize.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1825 2023-03-21 18:46:29.000000 Apptimize-1.2.38/Apptimize.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      256 2023-03-21 18:46:29.000000 Apptimize-1.2.38/Apptimize.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-03-21 18:46:29.000000 Apptimize-1.2.38/Apptimize.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2023-03-21 18:46:29.000000 Apptimize-1.2.38/Apptimize.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2023-03-21 18:46:29.000000 Apptimize-1.2.38/Apptimize.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     9665 2023-03-21 18:46:29.000000 Apptimize-1.2.38/CHANGELOG.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    13692 2023-03-21 18:46:29.000000 Apptimize-1.2.38/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-03-21 18:41:40.000000 Apptimize-1.2.38/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1825 2023-03-21 18:46:29.000000 Apptimize-1.2.38/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      971 2023-03-21 18:41:40.000000 Apptimize-1.2.38/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2023-03-21 18:46:29.000000 Apptimize-1.2.38/VERSION.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   687382 2023-03-21 18:46:29.000000 Apptimize-1.2.38/apptimize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2023-03-21 18:46:29.000000 Apptimize-1.2.38/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     7971 2023-03-21 18:41:40.000000 Apptimize-1.2.38/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-12 14:57:17.000000 Apptimize-1.2.39/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-12 14:57:17.000000 Apptimize-1.2.39/Apptimize.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1825 2023-05-12 14:57:17.000000 Apptimize-1.2.39/Apptimize.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      256 2023-05-12 14:57:17.000000 Apptimize-1.2.39/Apptimize.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-12 14:57:17.000000 Apptimize-1.2.39/Apptimize.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       17 2023-05-12 14:57:17.000000 Apptimize-1.2.39/Apptimize.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       10 2023-05-12 14:57:17.000000 Apptimize-1.2.39/Apptimize.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9793 2023-05-12 14:57:17.000000 Apptimize-1.2.39/CHANGELOG.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13692 2023-05-12 14:57:17.000000 Apptimize-1.2.39/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-05-12 14:52:22.000000 Apptimize-1.2.39/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1825 2023-05-12 14:57:17.000000 Apptimize-1.2.39/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      971 2023-05-12 14:52:22.000000 Apptimize-1.2.39/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2023-05-12 14:57:17.000000 Apptimize-1.2.39/VERSION.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   686576 2023-05-12 14:57:17.000000 Apptimize-1.2.39/apptimize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       92 2023-05-12 14:57:17.000000 Apptimize-1.2.39/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7971 2023-05-12 14:52:22.000000 Apptimize-1.2.39/setup.py
```

### Comparing `Apptimize-1.2.38/Apptimize.egg-info/PKG-INFO` & `Apptimize-1.2.39/Apptimize.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apptimize
-Version: 1.2.38
+Version: 1.2.39
 Summary: Apptimize Python Server SDK
 Home-page: https://apptimize.com/
 Author: Apptimize, Inc.
 Author-email: support@apptimize.com
 License: UNKNOWN
 Project-URL: Learn More, https://apptimize.com/
 Project-URL: Documentation, https://apptimize.com/docs/
```

### Comparing `Apptimize-1.2.38/CHANGELOG.txt` & `Apptimize-1.2.39/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 Cross-Platform SDK Change Log
 
+Apptimize Cross-Platform SDK Change Log 1.2.39 - 12 May 2023
+ * Handle missing userID parameter more gracefully in server SDKs
+
 Apptimize Cross-Platform SDK Change Log 1.2.38 - 21 March 2023
  * Fixed rare local storage overflow crash (Javascript)
 
 Apptimize Cross-Platform SDK Change Log 1.2.37 - 10 March 2023
  * Added Pilot Targeting ID (Roku)
  * Added userid, pilotid, and customattributes as fields on Apptimize node (Roku)
```

### Comparing `Apptimize-1.2.38/LICENSE.txt` & `Apptimize-1.2.39/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Apptimize-1.2.38/PKG-INFO` & `Apptimize-1.2.39/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apptimize
-Version: 1.2.38
+Version: 1.2.39
 Summary: Apptimize Python Server SDK
 Home-page: https://apptimize.com/
 Author: Apptimize, Inc.
 Author-email: support@apptimize.com
 License: UNKNOWN
 Project-URL: Learn More, https://apptimize.com/
 Project-URL: Documentation, https://apptimize.com/docs/
```

### Comparing `Apptimize-1.2.38/README.rst` & `Apptimize-1.2.39/README.rst`

 * *Files identical despite different names*

### Comparing `Apptimize-1.2.38/apptimize.py` & `Apptimize-1.2.39/apptimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         if apptimize_Apptimize._isInitialized():
             apptimize_ABTDataStore.sharedInstance().flushTracking()
         else:
             apptimize_ABTLogger.w("Tracking can only be flushed after setup().",_hx_AnonObject({'fileName': "src/apptimize/Apptimize.hx", 'lineNumber': 466, 'className': "apptimize.Apptimize", 'methodName': "flushTracking"}))
 
     @staticmethod
     def getApptimizeSDKVersion():
-        return "1.2.38"
+        return "1.2.39"
 
     @staticmethod
     def getApptimizeSDKPlatform():
         sdkPlatform = "N/A"
         sdkPlatform = "Python"
         return sdkPlatform
 
@@ -207,21 +207,22 @@
     def _getCodeBlockMethod(codeBlockVariableName,userID,customAttributes):
         apptimize_ABTDataStore._checkForUpdatedMetadataIfNecessary()
         envParams = apptimize_filter_ABTFilterEnvParams(userID,apptimize_Apptimize._getApptimizeAnonUserId(),customAttributes,apptimize_ABTDataStore.getAppKey(),apptimize_support_properties_ABTApplicationProperties.sharedInstance(),apptimize_support_properties_ABTInternalProperties.sharedInstance())
         return apptimize_ApptimizeInternal._getCodeBlockMethod(envParams,codeBlockVariableName)
 
     @staticmethod
     def runCodeBlock(codeBlockVariableName,callback,userID,customAttributes = None):
-        if ((not apptimize_util_ABTTypes.isNullOrString(userID)) or ((StringTools.ltrim(userID) == ""))):
-            apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 46, 'className': "apptimize.Apptimize", 'methodName': "runCodeBlock"}))
-            userID = None
-        if ((userID is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize.runCodeBlock"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 51, 'className': "apptimize.Apptimize", 'methodName': "runCodeBlock"}))
+        if (userID is not None):
+            if ((not apptimize_util_ABTTypes.isString(userID)) or ((StringTools.ltrim(userID) == ""))):
+                apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 47, 'className': "apptimize.Apptimize", 'methodName': "runCodeBlock"}))
+                userID = None
+        if (userID is None):
+            apptimize_ABTLogger.c((("The parameter " + "userID") + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 53, 'className': "apptimize.Apptimize", 'methodName': "runCodeBlock"}))
         if ((customAttributes is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize.runCodeBlock"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 57, 'className': "apptimize.Apptimize", 'methodName': "runCodeBlock"}))
+            apptimize_ABTLogger.c((("The parameter " + HxOverrides.stringOrNull(None)) + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 59, 'className': "apptimize.Apptimize", 'methodName': "runCodeBlock"}))
         attrs = apptimize_util_ABTUtilDictionary.nativeObjectToStringMap(customAttributes)
         methodName = apptimize_Apptimize._getCodeBlockMethod(codeBlockVariableName,userID,attrs)
         callbackMap = apptimize_util_ABTUtilDictionary.nativeObjectToStringMap(callback)
         if ((methodName is None) or ((methodName == ""))):
             apptimize_ABTLogger.w((("No Code Block with variable name " + ("null" if codeBlockVariableName is None else codeBlockVariableName)) + " found, skipping callback."),_hx_AnonObject({'fileName': "src/apptimize/Apptimize.hx", 'lineNumber': 615, 'className': "apptimize.Apptimize", 'methodName': "runCodeBlock"}))
             return
         elif ((callback is None) or ((callbackMap.h.get(methodName,None) is None))):
@@ -326,34 +327,36 @@
             return defaultValue
         return doubleDictionaryValue
 
     @staticmethod
     def _getValue(name,userID,_hx_type,nestedType,customAttributes):
         if (not apptimize_Apptimize._isInitialized()):
             return None
-        if ((not apptimize_util_ABTTypes.isNullOrString(userID)) or ((StringTools.ltrim(userID) == ""))):
-            apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 46, 'className': "apptimize.Apptimize", 'methodName': "_getValue"}))
-            userID = None
-        if ((userID is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize._getValue"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 51, 'className': "apptimize.Apptimize", 'methodName': "_getValue"}))
+        if (userID is not None):
+            if ((not apptimize_util_ABTTypes.isString(userID)) or ((StringTools.ltrim(userID) == ""))):
+                apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 47, 'className': "apptimize.Apptimize", 'methodName': "_getValue"}))
+                userID = None
+        if (userID is None):
+            apptimize_ABTLogger.c((("The parameter " + "userID") + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 53, 'className': "apptimize.Apptimize", 'methodName': "_getValue"}))
         if ((customAttributes is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize._getValue"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 57, 'className': "apptimize.Apptimize", 'methodName': "_getValue"}))
+            apptimize_ABTLogger.c((("The parameter " + HxOverrides.stringOrNull(None)) + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 59, 'className': "apptimize.Apptimize", 'methodName': "_getValue"}))
         attrMap = apptimize_util_ABTUtilDictionary.nativeObjectToStringMap(customAttributes)
         envParams = apptimize_filter_ABTFilterEnvParams(userID,apptimize_Apptimize._getApptimizeAnonUserId(),attrMap,apptimize_ABTDataStore.getAppKey(),apptimize_support_properties_ABTApplicationProperties.sharedInstance(),apptimize_support_properties_ABTInternalProperties.sharedInstance())
         return apptimize_ABTApptimizeVariable.getValue(envParams,name,_hx_type,nestedType)
 
     @staticmethod
     def getVariantInfo(userID,customAttributes = None):
-        if ((not apptimize_util_ABTTypes.isNullOrString(userID)) or ((StringTools.ltrim(userID) == ""))):
-            apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 46, 'className': "apptimize.Apptimize", 'methodName': "getVariantInfo"}))
-            userID = None
-        if ((userID is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize.getVariantInfo"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 51, 'className': "apptimize.Apptimize", 'methodName': "getVariantInfo"}))
+        if (userID is not None):
+            if ((not apptimize_util_ABTTypes.isString(userID)) or ((StringTools.ltrim(userID) == ""))):
+                apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 47, 'className': "apptimize.Apptimize", 'methodName': "getVariantInfo"}))
+                userID = None
+        if (userID is None):
+            apptimize_ABTLogger.c((("The parameter " + "userID") + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 53, 'className': "apptimize.Apptimize", 'methodName': "getVariantInfo"}))
         if ((customAttributes is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize.getVariantInfo"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 57, 'className': "apptimize.Apptimize", 'methodName': "getVariantInfo"}))
+            apptimize_ABTLogger.c((("The parameter " + HxOverrides.stringOrNull(None)) + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 59, 'className': "apptimize.Apptimize", 'methodName': "getVariantInfo"}))
         variantInfos = list()
         anonID = apptimize_Apptimize._getApptimizeAnonUserId()
         attrMap = apptimize_util_ABTUtilDictionary.nativeObjectToStringMap(customAttributes)
         envParams = apptimize_filter_ABTFilterEnvParams(userID,anonID,attrMap,apptimize_ABTDataStore.getAppKey(),apptimize_support_properties_ABTApplicationProperties.sharedInstance(),apptimize_support_properties_ABTInternalProperties.sharedInstance())
         _g = 0
         _g1 = apptimize_ApptimizeInternal._getVariants(envParams)
         while (_g < len(_g1)):
@@ -373,33 +376,35 @@
             _g = (_g + 1)
             if (alteration.getKey() == name):
                 return apptimize_VariantInfo.initWithVariant(alteration.getVariant(),userID,anonID)
         return None
 
     @staticmethod
     def _getVariantInfoForDynamicVariable(name,userID,customAttributes = None):
-        if ((not apptimize_util_ABTTypes.isNullOrString(userID)) or ((StringTools.ltrim(userID) == ""))):
-            apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 46, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForDynamicVariable"}))
-            userID = None
-        if ((userID is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize._getVariantInfoForDynamicVariable"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 51, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForDynamicVariable"}))
+        if (userID is not None):
+            if ((not apptimize_util_ABTTypes.isString(userID)) or ((StringTools.ltrim(userID) == ""))):
+                apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 47, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForDynamicVariable"}))
+                userID = None
+        if (userID is None):
+            apptimize_ABTLogger.c((("The parameter " + "userID") + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 53, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForDynamicVariable"}))
         if ((customAttributes is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize._getVariantInfoForDynamicVariable"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 57, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForDynamicVariable"}))
+            apptimize_ABTLogger.c((("The parameter " + HxOverrides.stringOrNull(None)) + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 59, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForDynamicVariable"}))
         attrMap = apptimize_util_ABTUtilDictionary.nativeObjectToStringMap(customAttributes)
         return apptimize_Apptimize._getVariantInfoForAlteration(name,userID,attrMap)
 
     @staticmethod
     def _getVariantInfoForExperiment(name,userID,customAttributes = None):
-        if ((not apptimize_util_ABTTypes.isNullOrString(userID)) or ((StringTools.ltrim(userID) == ""))):
-            apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 46, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForExperiment"}))
-            userID = None
-        if ((userID is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize._getVariantInfoForExperiment"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 51, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForExperiment"}))
+        if (userID is not None):
+            if ((not apptimize_util_ABTTypes.isString(userID)) or ((StringTools.ltrim(userID) == ""))):
+                apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 47, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForExperiment"}))
+                userID = None
+        if (userID is None):
+            apptimize_ABTLogger.c((("The parameter " + "userID") + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 53, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForExperiment"}))
         if ((customAttributes is None) and False):
-            apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize._getVariantInfoForExperiment"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 57, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForExperiment"}))
+            apptimize_ABTLogger.c((("The parameter " + HxOverrides.stringOrNull(None)) + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 59, 'className': "apptimize.Apptimize", 'methodName': "_getVariantInfoForExperiment"}))
         anonID = apptimize_Apptimize._getApptimizeAnonUserId()
         attrMap = apptimize_util_ABTUtilDictionary.nativeObjectToStringMap(customAttributes)
         envParams = apptimize_filter_ABTFilterEnvParams(userID,anonID,attrMap,apptimize_ABTDataStore.getAppKey(),apptimize_support_properties_ABTApplicationProperties.sharedInstance(),apptimize_support_properties_ABTInternalProperties.sharedInstance())
         _g = 0
         _g1 = apptimize_ApptimizeInternal._getVariants(envParams)
         while (_g < len(_g1)):
             variant = (_g1[_g] if _g >= 0 and _g < len(_g1) else None)
@@ -407,37 +412,39 @@
             if (variant.getExperimentName() == name):
                 return apptimize_VariantInfo.initWithVariant(variant,userID,anonID)
         return None
 
     @staticmethod
     def track(eventName,userID,customAttributes = None):
         if apptimize_Apptimize._isInitialized():
-            if ((not apptimize_util_ABTTypes.isNullOrString(userID)) or ((StringTools.ltrim(userID) == ""))):
-                apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 46, 'className': "apptimize.Apptimize", 'methodName': "track"}))
-                userID = None
-            if ((userID is None) and False):
-                apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize.track"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 51, 'className': "apptimize.Apptimize", 'methodName': "track"}))
+            if (userID is not None):
+                if ((not apptimize_util_ABTTypes.isString(userID)) or ((StringTools.ltrim(userID) == ""))):
+                    apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 47, 'className': "apptimize.Apptimize", 'methodName': "track"}))
+                    userID = None
+            if (userID is None):
+                apptimize_ABTLogger.c((("The parameter " + "userID") + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 53, 'className': "apptimize.Apptimize", 'methodName': "track"}))
             if ((customAttributes is None) and False):
-                apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize.track"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 57, 'className': "apptimize.Apptimize", 'methodName': "track"}))
+                apptimize_ABTLogger.c((("The parameter " + HxOverrides.stringOrNull(None)) + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 59, 'className': "apptimize.Apptimize", 'methodName': "track"}))
             attrMap = apptimize_util_ABTUtilDictionary.nativeObjectToStringMap(customAttributes)
             envParams = apptimize_filter_ABTFilterEnvParams(userID,apptimize_Apptimize._getApptimizeAnonUserId(),attrMap,apptimize_ABTDataStore.getAppKey(),apptimize_support_properties_ABTApplicationProperties.sharedInstance(),apptimize_support_properties_ABTInternalProperties.sharedInstance())
             apptimize_ApptimizeInternal.generateTrackEvent(envParams,eventName,None)
         else:
             apptimize_ABTLogger.w("Events can only be tracked after setup() has been called.",_hx_AnonObject({'fileName': "src/apptimize/Apptimize.hx", 'lineNumber': 1215, 'className': "apptimize.Apptimize", 'methodName': "track"}))
 
     @staticmethod
     def trackValue(eventName,value,userID,customAttributes = None):
         if apptimize_Apptimize._isInitialized():
-            if ((not apptimize_util_ABTTypes.isNullOrString(userID)) or ((StringTools.ltrim(userID) == ""))):
-                apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 46, 'className': "apptimize.Apptimize", 'methodName': "trackValue"}))
-                userID = None
-            if ((userID is None) and False):
-                apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize.trackValue"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 51, 'className': "apptimize.Apptimize", 'methodName': "trackValue"}))
+            if (userID is not None):
+                if ((not apptimize_util_ABTTypes.isString(userID)) or ((StringTools.ltrim(userID) == ""))):
+                    apptimize_ABTLogger.w("The `userID` argument cannot be set to a non-string value, be empty or be whitespace only, setting to null instead.",_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 47, 'className': "apptimize.Apptimize", 'methodName': "trackValue"}))
+                    userID = None
+            if (userID is None):
+                apptimize_ABTLogger.c((("The parameter " + "userID") + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 53, 'className': "apptimize.Apptimize", 'methodName': "trackValue"}))
             if ((customAttributes is None) and False):
-                apptimize_ABTLogger.c(((("The parameter " + HxOverrides.stringOrNull(None)) + " is required for ") + "apptimize.Apptimize.trackValue"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 57, 'className': "apptimize.Apptimize", 'methodName': "trackValue"}))
+                apptimize_ABTLogger.c((("The parameter " + HxOverrides.stringOrNull(None)) + " is required"),_hx_AnonObject({'fileName': "src/apptimize/macros/ABTClientMacro.hx", 'lineNumber': 59, 'className': "apptimize.Apptimize", 'methodName': "trackValue"}))
             if ((not Std.isOfType(value,Float)) and (not Std.isOfType(value,apptimize_util_ArrayType.Int))):
                 apptimize_ABTLogger.w("trackValue() called with a non-float value. Event not logged.",_hx_AnonObject({'fileName': "src/apptimize/Apptimize.hx", 'lineNumber': 1246, 'className': "apptimize.Apptimize", 'methodName': "trackValue"}))
                 return
             attrMap = apptimize_util_ABTUtilDictionary.nativeObjectToStringMap(customAttributes)
             envParams = apptimize_filter_ABTFilterEnvParams(userID,apptimize_Apptimize._getApptimizeAnonUserId(),attrMap,apptimize_ABTDataStore.getAppKey(),apptimize_support_properties_ABTApplicationProperties.sharedInstance(),apptimize_support_properties_ABTInternalProperties.sharedInstance())
             apptimize_ApptimizeInternal.generateTrackEvent(envParams,eventName,value)
         else:
@@ -7234,34 +7241,27 @@
 _hx_classes["apptimize.util.ABTTimer"] = apptimize_util_ABTTimer
 
 
 class apptimize_util_ABTTypes:
     _hx_class_name = "apptimize.util.ABTTypes"
     _hx_is_interface = "False"
     __slots__ = ()
-    _hx_statics = ["isString", "isNullOrString"]
+    _hx_statics = ["isString"]
 
     @staticmethod
     def isString(string):
         _g = Type.typeof(string)
         if (_g.index == 6):
             c = _g.params[0]
             if (Type.getClassName(c) == "String"):
                 return True
             else:
                 return False
         else:
             return False
-
-    @staticmethod
-    def isNullOrString(string):
-        if (string is not None):
-            return apptimize_util_ABTTypes.isString(string)
-        else:
-            return True
 apptimize_util_ABTTypes._hx_class = apptimize_util_ABTTypes
 _hx_classes["apptimize.util.ABTTypes"] = apptimize_util_ABTTypes
 
 class apptimize_util_ArrayType(Enum):
     __slots__ = ()
     _hx_class_name = "apptimize.util.ArrayType"
     _hx_constructs = ["Int", "Bool", "Double", "String", "VariantInfo"]
@@ -10860,30 +10860,27 @@
                 return (_gthis._threadPool.state == hx_concurrent_ServiceState.STOPPED)
             hx_concurrent_thread_Threads._hx_await(_hx_local_6,-1)
             _gthis.set_state(hx_concurrent_ServiceState.STOPPED)
         hx_concurrent_thread_Threads.spawn(_hx_local_7)
 
     def submit(self,task,schedule = None):
         _gthis = self
+        schedule1 = (hx_concurrent_executor_Executor.NOW_ONCE if ((schedule is None)) else schedule)
         def _hx_local_2():
             def _hx_local_1():
-                nonlocal schedule
                 if (_gthis.state != hx_concurrent_ServiceState.RUNNING):
                     raise haxe_Exception.thrown((("Cannot accept new tasks. Executor is not in state [RUNNING] but [" + Std.string(_gthis.state)) + "]."))
-                if (schedule is None):
-                    schedule = hx_concurrent_executor_Executor.NOW_ONCE
-                future = hx_concurrent_executor__ThreadPoolExecutor_TaskFutureImpl(_gthis,task,schedule)
-                if (schedule is not None):
-                    if (schedule.index == 0):
-                        _g = schedule.params[0]
-                        if future.isDue():
-                            def _hx_local_0(ctx):
-                                future.run()
-                            _gthis._threadPool.submit(_hx_local_0)
-                            return future
+                future = hx_concurrent_executor__ThreadPoolExecutor_TaskFutureImpl(_gthis,task,schedule1)
+                if (schedule1.index == 0):
+                    _g = schedule1.params[0]
+                    if future.isDue():
+                        def _hx_local_0(ctx):
+                            future.run()
+                        _gthis._threadPool.submit(_hx_local_0)
+                        return future
                 _gthis._newScheduledTasks.push(future)
                 return future
             return self._stateLock.execute(_hx_local_1)
         return _hx_local_2()
 
     @staticmethod
     def _hx_empty_init(_hx_o):
@@ -11018,14 +11015,15 @@
         self._scheduledTasks = []
         super().__init__()
         if autostart:
             self.start()
 
     def submit(self,task,schedule = None):
         _gthis = self
+        schedule1 = (hx_concurrent_executor_Executor.NOW_ONCE if ((schedule is None)) else schedule)
         def _hx_local_1():
             def _hx_local_0():
                 if (_gthis.state != hx_concurrent_ServiceState.RUNNING):
                     raise haxe_Exception.thrown((("Cannot accept new tasks. Executor is not in state [RUNNING] but [" + Std.string(_gthis.state)) + "]."))
                 i = len(_gthis._scheduledTasks)
                 while True:
                     tmp = i
@@ -11037,20 +11035,17 @@
                         pos = i
                         if (pos < 0):
                             pos = (len(_this) + pos)
                         if (pos < 0):
                             pos = 0
                         res = _this[pos:(pos + 1)]
                         del _this[pos:(pos + 1)]
-                future = hx_concurrent_executor__TimerExecutor_TaskFutureImpl(_gthis,task,(hx_concurrent_executor_Executor.NOW_ONCE if ((schedule is None)) else schedule))
-                if (schedule is None):
-                    _this = _gthis._scheduledTasks
-                    _this.append(future)
-                elif (schedule.index == 0):
-                    _g = schedule.params[0]
+                future = hx_concurrent_executor__TimerExecutor_TaskFutureImpl(_gthis,task,schedule1)
+                if (schedule1.index == 0):
+                    _g = schedule1.params[0]
                     if (_g is None):
                         _this = _gthis._scheduledTasks
                         _this.append(future)
                     elif (_g != 0):
                         _this = _gthis._scheduledTasks
                         _this.append(future)
                 else:
@@ -11287,26 +11282,27 @@
 hx_concurrent_lock_RLock._hx_class = hx_concurrent_lock_RLock
 _hx_classes["hx.concurrent.lock.RLock"] = hx_concurrent_lock_RLock
 
 
 class hx_concurrent_thread_ThreadPool(hx_concurrent_ServiceBase):
     _hx_class_name = "hx.concurrent.thread.ThreadPool"
     _hx_is_interface = "False"
-    __slots__ = ("_spawnedThreadCount", "_workingThreadCount", "_workQueue", "threadCount")
-    _hx_fields = ["_spawnedThreadCount", "_workingThreadCount", "_workQueue", "threadCount"]
+    __slots__ = ("_spawnedThreadCount", "_workingThreadCount", "_workQueue", "threadCount", "pollPeriod")
+    _hx_fields = ["_spawnedThreadCount", "_workingThreadCount", "_workQueue", "threadCount", "pollPeriod"]
     _hx_methods = ["onStart", "submit"]
-    _hx_statics = ["_threadIDs"]
+    _hx_statics = ["DEFAULT_POLL_PERIOD", "_threadIDs"]
     _hx_interfaces = []
     _hx_super = hx_concurrent_ServiceBase
 
 
     def __init__(self,numThreads,autostart = None):
         if (autostart is None):
             autostart = True
         self.threadCount = None
+        self.pollPeriod = hx_concurrent_thread_ThreadPool.DEFAULT_POLL_PERIOD
         self._workQueue = hx_concurrent_collection_Queue()
         val = 0
         if (val is None):
             val = 0
         this1 = hx_concurrent_atomic__AtomicInt_AtomicIntImpl(val)
         self._workingThreadCount = this1
         val = 0
@@ -11328,30 +11324,30 @@
         _g1 = self.threadCount
         while (_g < _g1):
             i = _g
             _g = (_g + 1)
             def _hx_local_1():
                 _gthis._spawnedThreadCount.getAndIncrement()
                 context = hx_concurrent_thread_ThreadContext(hx_concurrent_thread_ThreadPool._threadIDs.incrementAndGet())
-                haxe_Log.trace((((((((("[" + Std.string(_gthis)) + "] Spawned thread ") + HxOverrides.stringOrNull((("null" if ((_gthis._spawnedThreadCount is None)) else Std.string(_gthis._spawnedThreadCount.get_value()))))) + "/") + Std.string(_gthis.threadCount)) + " with ID ") + Std.string(context.id)) + "."),_hx_AnonObject({'fileName': "hx/concurrent/thread/ThreadPool.hx", 'lineNumber': 93, 'className': "hx.concurrent.thread.ThreadPool", 'methodName': "onStart"}))
+                haxe_Log.trace((((((((("[" + Std.string(_gthis)) + "] Spawned thread ") + HxOverrides.stringOrNull((("null" if ((_gthis._spawnedThreadCount is None)) else Std.string(_gthis._spawnedThreadCount.get_value()))))) + "/") + Std.string(_gthis.threadCount)) + " with ID ") + Std.string(context.id)) + "."),_hx_AnonObject({'fileName': "hx/concurrent/thread/ThreadPool.hx", 'lineNumber': 107, 'className': "hx.concurrent.thread.ThreadPool", 'methodName': "onStart"}))
                 while True:
                     task = _gthis._workQueue.pop()
                     if (task is None):
                         if (_gthis.state != hx_concurrent_ServiceState.RUNNING):
                             break
-                        Sys.sleep(0.001)
+                        Sys.sleep(_gthis.pollPeriod)
                     else:
                         try:
                             _gthis._workingThreadCount.getAndIncrement()
                             task(context)
                         except BaseException as _g:
                             ex = haxe_Exception.caught(_g)
-                            haxe_Log.trace(ex,_hx_AnonObject({'fileName': "hx/concurrent/thread/ThreadPool.hx", 'lineNumber': 106, 'className': "hx.concurrent.thread.ThreadPool", 'methodName': "onStart"}))
+                            haxe_Log.trace(ex,_hx_AnonObject({'fileName': "hx/concurrent/thread/ThreadPool.hx", 'lineNumber': 120, 'className': "hx.concurrent.thread.ThreadPool", 'methodName': "onStart"}))
                         _gthis._workingThreadCount.getAndIncrement(-1)
-                haxe_Log.trace((((("[" + Std.string(_gthis)) + "] Stopped thread with ID ") + Std.string(context.id)) + "."),_hx_AnonObject({'fileName': "hx/concurrent/thread/ThreadPool.hx", 'lineNumber': 112, 'className': "hx.concurrent.thread.ThreadPool", 'methodName': "onStart"}))
+                haxe_Log.trace((((("[" + Std.string(_gthis)) + "] Stopped thread with ID ") + Std.string(context.id)) + "."),_hx_AnonObject({'fileName': "hx/concurrent/thread/ThreadPool.hx", 'lineNumber': 126, 'className': "hx.concurrent.thread.ThreadPool", 'methodName': "onStart"}))
                 _gthis._spawnedThreadCount.getAndIncrement(-1)
                 if (_gthis._spawnedThreadCount.get_value() == 0):
                     def _hx_local_0():
                         return _gthis.set_state(hx_concurrent_ServiceState.STOPPED)
                     _gthis._stateLock.execute(_hx_local_0)
             hx_concurrent_thread_Threads.spawn(_hx_local_1)
 
@@ -11367,14 +11363,15 @@
 
     @staticmethod
     def _hx_empty_init(_hx_o):
         _hx_o._spawnedThreadCount = None
         _hx_o._workingThreadCount = None
         _hx_o._workQueue = None
         _hx_o.threadCount = None
+        _hx_o.pollPeriod = None
 hx_concurrent_thread_ThreadPool._hx_class = hx_concurrent_thread_ThreadPool
 _hx_classes["hx.concurrent.thread.ThreadPool"] = hx_concurrent_thread_ThreadPool
 
 
 class hx_concurrent_thread_ThreadContext:
     _hx_class_name = "hx.concurrent.thread.ThreadContext"
     _hx_is_interface = "False"
@@ -15368,14 +15365,15 @@
 def _hx_init_hx_concurrent_ServiceBase__ids():
     def _hx_local_0():
         this1 = hx_concurrent_atomic__AtomicInt_AtomicIntImpl(0)
         return this1
     return _hx_local_0()
 hx_concurrent_ServiceBase._ids = _hx_init_hx_concurrent_ServiceBase__ids()
 hx_concurrent_executor_Executor.NOW_ONCE = hx_concurrent_executor_Schedule.ONCE(0)
+hx_concurrent_thread_ThreadPool.DEFAULT_POLL_PERIOD = 0.001
 def _hx_init_hx_concurrent_thread_ThreadPool__threadIDs():
     def _hx_local_0():
         this1 = hx_concurrent_atomic__AtomicInt_AtomicIntImpl(0)
         return this1
     return _hx_local_0()
 hx_concurrent_thread_ThreadPool._threadIDs = _hx_init_hx_concurrent_thread_ThreadPool__threadIDs()
 pako_Inflate.DEFAULT_OPTIONS = _hx_AnonObject({'chunkSize': 16384, 'windowBits': 0, 'raw': False, 'dictionary': None})
```

### Comparing `Apptimize-1.2.38/setup.py` & `Apptimize-1.2.39/setup.py`

 * *Files identical despite different names*

