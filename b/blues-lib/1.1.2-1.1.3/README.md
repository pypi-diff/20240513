# Comparing `tmp/blues_lib-1.1.2.tar.gz` & `tmp/blues_lib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\blues_lib-1.1.2.tar", last modified: Sun May 12 15:35:11 2024, max compression
+gzip compressed data, was "dist\blues_lib-1.1.3.tar", last modified: Mon May 13 17:03:23 2024, max compression
```

## Comparing `blues_lib-1.1.2.tar` & `blues_lib-1.1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 15:35:11.111984 blues_lib-1.1.2/
--rw-rw-rw-   0        0        0     1047 2024-05-12 15:35:11.111984 blues_lib-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      604 2024-05-12 14:30:47.000000 blues_lib-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 15:35:11.042870 blues_lib-1.1.2/blues_lib/
--rw-rw-rw-   0        0        0        0 2024-05-10 14:52:26.000000 blues_lib-1.1.2/blues_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:35:11.052642 blues_lib-1.1.2/blues_lib/sele/
--rw-rw-rw-   0        0        0      652 2024-05-12 04:42:19.000000 blues_lib-1.1.2/blues_lib/sele/BluesBrowser.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.2/blues_lib/sele/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:35:11.054609 blues_lib-1.1.2/blues_lib/sele/action/
--rw-rw-rw-   0        0        0     1240 2024-05-09 17:07:48.000000 blues_lib-1.1.2/blues_lib/sele/action/BluesDriverAction.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.2/blues_lib/sele/action/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:35:11.080878 blues_lib-1.1.2/blues_lib/sele/action/parts/
--rw-rw-rw-   0        0        0      847 2024-05-09 13:20:33.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesAlertAction.py
--rw-rw-rw-   0        0        0     1282 2024-05-08 12:42:33.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesCookieAction.py
--rw-rw-rw-   0        0        0     1042 2024-05-08 12:29:54.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesDocumentAction.py
--rw-rw-rw-   0        0        0     4408 2024-05-08 16:59:14.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesElementAction.py
--rw-rw-rw-   0        0        0     1546 2024-05-08 13:10:15.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesEventAction.py
--rw-rw-rw-   0        0        0     1633 2024-05-07 19:59:12.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesFormAction.py
--rw-rw-rw-   0        0        0      952 2024-05-08 14:33:15.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesFrameAction.py
--rw-rw-rw-   0        0        0     8315 2024-05-09 16:01:28.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesJavaScriptAction.py
--rw-rw-rw-   0        0        0     2852 2024-05-08 15:55:31.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesMoverAction.py
--rw-rw-rw-   0        0        0     1921 2024-05-09 12:42:45.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesSelectAction.py
--rw-rw-rw-   0        0        0     3398 2024-05-12 15:25:06.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/BluesWindowAction.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.2/blues_lib/sele/action/parts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:35:11.086594 blues_lib-1.1.2/blues_lib/sele/browser/
--rw-rw-rw-   0        0        0     3569 2024-05-12 15:25:06.000000 blues_lib-1.1.2/blues_lib/sele/browser/BluesChrome.py
--rw-rw-rw-   0        0        0     3027 2024-05-12 15:25:06.000000 blues_lib-1.1.2/blues_lib/sele/browser/BluesDebugChrome.py
--rw-rw-rw-   0        0        0     4120 2024-05-12 15:25:06.000000 blues_lib-1.1.2/blues_lib/sele/browser/BluesProxyChrome.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.2/blues_lib/sele/browser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:35:11.095772 blues_lib-1.1.2/blues_lib/sql/
--rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.1.2/blues_lib/sql/BluesMySQLExecutor.py
--rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.1.2/blues_lib/sql/BluesSQLConvertor.py
--rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.1.2/blues_lib/sql/BluesSQLExecutor.py
--rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.1.2/blues_lib/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:35:11.110978 blues_lib-1.1.2/blues_lib/util/
--rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.1.2/blues_lib/util/BluesConsole.py
--rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.1.2/blues_lib/util/BluesDateTime.py
--rw-rw-rw-   0        0        0     5213 2024-05-12 06:52:48.000000 blues_lib-1.1.2/blues_lib/util/BluesFiler.py
--rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.1.2/blues_lib/util/BluesImager.py
--rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.1.2/blues_lib/util/BluesLogger.py
--rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.1.2/blues_lib/util/BluesMailer.py
--rw-rw-rw-   0        0        0     1713 2024-05-07 09:54:17.000000 blues_lib-1.1.2/blues_lib/util/BluesPowerShell.py
--rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.1.2/blues_lib/util/BluesType.py
--rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.2/blues_lib/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:35:11.049229 blues_lib-1.1.2/blues_lib.egg-info/
--rw-rw-rw-   0        0        0     1047 2024-05-12 15:35:10.000000 blues_lib-1.1.2/blues_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2024-05-12 15:35:10.000000 blues_lib-1.1.2/blues_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 15:35:10.000000 blues_lib-1.1.2/blues_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 15:35:10.000000 blues_lib-1.1.2/blues_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-12 15:35:11.112982 blues_lib-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      575 2024-05-12 15:35:04.000000 blues_lib-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.705390 blues_lib-1.1.3/
+-rw-rw-rw-   0        0        0     1172 2024-05-13 17:03:23.705390 blues_lib-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2024-05-12 15:38:25.000000 blues_lib-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.635805 blues_lib-1.1.3/blues_lib/
+-rw-rw-rw-   0        0        0        0 2024-05-10 14:52:26.000000 blues_lib-1.1.3/blues_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.645758 blues_lib-1.1.3/blues_lib/sele/
+-rw-rw-rw-   0        0        0      652 2024-05-12 04:42:19.000000 blues_lib-1.1.3/blues_lib/sele/BluesBrowser.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/sele/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.648605 blues_lib-1.1.3/blues_lib/sele/action/
+-rw-rw-rw-   0        0        0     1240 2024-05-09 17:07:48.000000 blues_lib-1.1.3/blues_lib/sele/action/BluesDriverAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/sele/action/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.674516 blues_lib-1.1.3/blues_lib/sele/action/parts/
+-rw-rw-rw-   0        0        0      847 2024-05-09 13:20:33.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesAlertAction.py
+-rw-rw-rw-   0        0        0     1282 2024-05-08 12:42:33.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesCookieAction.py
+-rw-rw-rw-   0        0        0     1042 2024-05-08 12:29:54.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesDocumentAction.py
+-rw-rw-rw-   0        0        0     4408 2024-05-08 16:59:14.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesElementAction.py
+-rw-rw-rw-   0        0        0     1546 2024-05-08 13:10:15.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesEventAction.py
+-rw-rw-rw-   0        0        0     1633 2024-05-07 19:59:12.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesFormAction.py
+-rw-rw-rw-   0        0        0      952 2024-05-08 14:33:15.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesFrameAction.py
+-rw-rw-rw-   0        0        0     8315 2024-05-09 16:01:28.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesJavaScriptAction.py
+-rw-rw-rw-   0        0        0     2852 2024-05-08 15:55:31.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesMoverAction.py
+-rw-rw-rw-   0        0        0     1921 2024-05-09 12:42:45.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesSelectAction.py
+-rw-rw-rw-   0        0        0     3398 2024-05-12 15:25:06.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/BluesWindowAction.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/sele/action/parts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.680009 blues_lib-1.1.3/blues_lib/sele/browser/
+-rw-rw-rw-   0        0        0     3862 2024-05-13 13:14:08.000000 blues_lib-1.1.3/blues_lib/sele/browser/BluesChrome.py
+-rw-rw-rw-   0        0        0     3280 2024-05-13 13:12:42.000000 blues_lib-1.1.3/blues_lib/sele/browser/BluesDebugChrome.py
+-rw-rw-rw-   0        0        0     4120 2024-05-12 15:25:06.000000 blues_lib-1.1.3/blues_lib/sele/browser/BluesProxyChrome.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/sele/browser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.685930 blues_lib-1.1.3/blues_lib/sql/
+-rw-rw-rw-   0        0        0     2757 2024-04-28 16:34:34.000000 blues_lib-1.1.3/blues_lib/sql/BluesMySQLExecutor.py
+-rw-rw-rw-   0        0        0     5403 2024-04-27 20:02:59.000000 blues_lib-1.1.3/blues_lib/sql/BluesSQLConvertor.py
+-rw-rw-rw-   0        0        0     3992 2024-04-28 16:33:04.000000 blues_lib-1.1.3/blues_lib/sql/BluesSQLExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 16:53:02.000000 blues_lib-1.1.3/blues_lib/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.703388 blues_lib-1.1.3/blues_lib/util/
+-rw-rw-rw-   0        0        0     1506 2024-05-09 17:16:52.000000 blues_lib-1.1.3/blues_lib/util/BluesConsole.py
+-rw-rw-rw-   0        0        0      766 2024-04-26 16:50:11.000000 blues_lib-1.1.3/blues_lib/util/BluesDateTime.py
+-rw-rw-rw-   0        0        0     5231 2024-05-13 17:00:25.000000 blues_lib-1.1.3/blues_lib/util/BluesFiler.py
+-rw-rw-rw-   0        0        0     2716 2024-04-20 10:37:16.000000 blues_lib-1.1.3/blues_lib/util/BluesImager.py
+-rw-rw-rw-   0        0        0     2923 2024-04-28 16:53:18.000000 blues_lib-1.1.3/blues_lib/util/BluesLogger.py
+-rw-rw-rw-   0        0        0     2619 2024-04-25 16:33:16.000000 blues_lib-1.1.3/blues_lib/util/BluesMailer.py
+-rw-rw-rw-   0        0        0     1744 2024-05-13 12:40:57.000000 blues_lib-1.1.3/blues_lib/util/BluesPowerShell.py
+-rw-rw-rw-   0        0        0      387 2024-05-08 11:04:20.000000 blues_lib-1.1.3/blues_lib/util/BluesType.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:13:28.000000 blues_lib-1.1.3/blues_lib/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:03:23.642553 blues_lib-1.1.3/blues_lib.egg-info/
+-rw-rw-rw-   0        0        0     1172 2024-05-13 17:03:23.000000 blues_lib-1.1.3/blues_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1458 2024-05-13 17:03:23.000000 blues_lib-1.1.3/blues_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:03:23.000000 blues_lib-1.1.3/blues_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 17:03:23.000000 blues_lib-1.1.3/blues_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-13 17:03:23.707686 blues_lib-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      575 2024-05-13 17:00:41.000000 blues_lib-1.1.3/setup.py
```

### Comparing `blues_lib-1.1.2/PKG-INFO` & `blues_lib-1.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: blues_lib
-Version: 1.1.2
+Version: 1.1.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## Description
         Python library writed by Blues Liu.
         
         ### Install
         ```
+        // first installation 
         pip install blues-lib==1.1.1
+        
+        // upgrade to the newest version
+        pip install --upgrade blues-lib
         ```
         
         ### sele
         #### BluesDebugChrome
         
         ##### reliant env variables
         1. `$env:CHROME_EXE` : the chrome's .exe file path - * required
```

### Comparing `blues_lib-1.1.2/README.md` & `blues_lib-1.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ## Description
 Python library writed by Blues Liu.
 
 ### Install
 ```
+// first installation 
 pip install blues-lib==1.1.1
+
+// upgrade to the newest version
+pip install --upgrade blues-lib
 ```
 
 ### sele
 #### BluesDebugChrome
 
 ##### reliant env variables
 1. `$env:CHROME_EXE` : the chrome's .exe file path - * required
```

### Comparing `blues_lib-1.1.2/blues_lib/sele/BluesBrowser.py` & `blues_lib-1.1.3/blues_lib/sele/BluesBrowser.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/BluesDriverAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/BluesDriverAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesAlertAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesAlertAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesCookieAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesCookieAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesDocumentAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesDocumentAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesElementAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesElementAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesEventAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesEventAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesFormAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesFormAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesFrameAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesFrameAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesJavaScriptAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesJavaScriptAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesMoverAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesMoverAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesSelectAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesSelectAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/action/parts/BluesWindowAction.py` & `blues_lib-1.1.3/blues_lib/sele/action/parts/BluesWindowAction.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sele/browser/BluesChrome.py` & `blues_lib-1.1.3/blues_lib/sele/browser/BluesChrome.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     '--no-default-browser-check':'',
     '--disable-notifications':'',
     '--disable-web-security':'',
     '--ignore-certificate-errors':'',
     '--disable-infobars':'',
     '--hide-crash-restore-bubble':'',
     '--disable-popup-blocking':'',
+    '--disable-extensions-api':'',
+    '--disable-application-install-prompt':'',
+    '--no-first-run':'', # 关闭广告隐藏设置弹框 （首次执行设置）
   }
 
   EXPERIMENTAL_OPTIONS = {
     'detach':True,
     'prefs' : {
       # 0 - Default, 1 - Allow, 2 - Block
       "profile.default_content_setting_values.notification": 2,
@@ -43,30 +46,31 @@
   }
 
   def __init__(self,config={},arguments={},experimental_options={}):
     '''
     @description : Get a Chrome Driver instance
     @param {dict} config
     '''
+    self.before_created(config,arguments,experimental_options)
+    self.created()
+    self.after_created()
+
+  def before_created(self,config,arguments,experimental_options):
+    self.driver = None
+    self.action = None
     self.config = {**self.CONFIG,**config}
     self.arguments = {**self.ARGUMENTS,**arguments} 
-
     # connect to a exist chrome, can't set detach and prefs options
     if experimental_options.get('debuggerAddress'):
       self.experimental_options = experimental_options
     else:
       self.experimental_options = {**self.EXPERIMENTAL_OPTIONS,**experimental_options}
-
     self.chrome_driver_exe = BluesPowerShell.get_env_value('CHROME_DRIVER_EXE')
-    self.driver = None
-    self.action = None
-    self.__created()
-    self.after_created()
 
-  def __created(self):
+  def created(self):
     '''
     @description : create the driver and action instance
     '''
     chrome_service = self.__get_service()
     chrome_options = self.__get_options()
     web_driver = self.get_driver_creator()
     self.driver = web_driver.Chrome( service = chrome_service, options = chrome_options)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `blues_lib-1.1.2/blues_lib/sele/browser/BluesDebugChrome.py` & `blues_lib-1.1.3/blues_lib/sele/browser/BluesDebugChrome.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,37 @@
 
 sys.path.append(re.sub('blues_lib.*','blues_lib',os.path.realpath(__file__)))
 from util.BluesPowerShell import BluesPowerShell 
 from sele.browser.BluesChrome import BluesChrome  
 
 # debug模式下chrome被PS提前打开，不是由webdriver启动，wire无法实现代理
 class BluesDebugChrome(BluesChrome):
+  # cover the parent options.detach and prefs can't be set in debug mode
+  EXPERIMENTAL_OPTIONS = {}
 
   def __init__(self,config={},arguments={},experimental_options={}):
     '''
     @description : Get a Chrome Driver instance
     @param {dict} config
     @param {list} arguments
     @param {dict} experimental_options
     '''
     self.chrome_exe = BluesPowerShell.get_env_value('CHROME_EXE')
     self.process_args=''
     self.__validate(arguments)
-    self.__set_args_options(arguments,experimental_options)
-    self.__restart()
     super().__init__(config,arguments,experimental_options)
 
+  def before_created(self,config,arguments,experimental_options):
+    '''
+    @description cover the parent method
+    '''
+    super().before_created(config,arguments,experimental_options)
+    self.__set_args_options()
+    self.__restart()
+
   def __validate(self,arguments):
     error = self.__get_env_error()
     if error:
       raise Exception(error)
 
     error = self.__get_args_error(arguments)
     if error:
@@ -54,27 +62,27 @@
       return 'Parameter arguments.--user-data-dir missing'
       
     if not arguments.get('--remote-debugging-address'):
       return 'Parameter arguments.--remote-debugging-address missing'
 
     return ''
 
-  def __set_args_options(self,arguments,experimental_options):
+  def __set_args_options(self):
     args = ''
-    for key,value in arguments.items():
+    for key,value in self.arguments.items():
       arg_value = '%s=%s' % (key,value) if value else key
       args+=' %s ' % arg_value
       if key == '--remote-debugging-address':
         # must set port or the driver can't connect to the browser
         args+='--remote-debugging-port=%s' % value.split(':')[1]
     
     self.process_args = args
 
     # cover the all default options (these default options can't be used to connect to a existed debuug chrome)
-    experimental_options['debuggerAddress'] = arguments['--remote-debugging-address']
+    self.experimental_options['debuggerAddress'] = self.arguments['--remote-debugging-address']
 
   def __close_chrome(self):
     BluesPowerShell.stop_process('chrome')
 
   def __restart(self):
     '''
     @description : repopen the specific chrome (stop all chrome processes)
```

### Comparing `blues_lib-1.1.2/blues_lib/sele/browser/BluesProxyChrome.py` & `blues_lib-1.1.3/blues_lib/sele/browser/BluesProxyChrome.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sql/BluesMySQLExecutor.py` & `blues_lib-1.1.3/blues_lib/sql/BluesMySQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sql/BluesSQLConvertor.py` & `blues_lib-1.1.3/blues_lib/sql/BluesSQLConvertor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/sql/BluesSQLExecutor.py` & `blues_lib-1.1.3/blues_lib/sql/BluesSQLExecutor.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/util/BluesConsole.py` & `blues_lib-1.1.3/blues_lib/util/BluesConsole.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/util/BluesDateTime.py` & `blues_lib-1.1.3/blues_lib/util/BluesDateTime.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/util/BluesFiler.py` & `blues_lib-1.1.3/blues_lib/util/BluesFiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         return (200,local_file) 
 
     except Exception as e:
       return (500,str(e))
 
   @classmethod
   def read_json(cls,file_path):
-    with open(file_path, 'r') as file:
+    with open(file_path, 'r', encoding='utf-8') as file:
       data = json.load(file)
       return data
 
   @classmethod
   def __get_result(cls):
     return {
       'code':500,
```

### Comparing `blues_lib-1.1.2/blues_lib/util/BluesImager.py` & `blues_lib-1.1.3/blues_lib/util/BluesImager.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/util/BluesLogger.py` & `blues_lib-1.1.3/blues_lib/util/BluesLogger.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/util/BluesMailer.py` & `blues_lib-1.1.3/blues_lib/util/BluesMailer.py`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/blues_lib/util/BluesPowerShell.py` & `blues_lib-1.1.3/blues_lib/util/BluesPowerShell.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     @param {str}  args : the multi exe executor's arguments, split by space
      - '--arg1 --arg2 --arg3'
     '''
     args_list = ''
     if args:
       args_list = '-ArgumentList \'%s\''  % args
     ps_script = 'Start-Process -FilePath \'%s\' %s' % (file_path,args_list)
+    print('===>ps',ps_script)
     return cls.execute(ps_script )
 
   @classmethod
   def get_env_value(cls,name):
     '''
     @description : get env variable's value
     @param {str} name : varibale's name
```

### Comparing `blues_lib-1.1.2/blues_lib.egg-info/SOURCES.txt` & `blues_lib-1.1.3/blues_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blues_lib-1.1.2/setup.py` & `blues_lib-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
   name="blues_lib", # package name
-  version="1.1.2", # package version
+  version="1.1.3", # package version
   long_description=open('README.md').read(),
   long_description_content_type='text/markdown',
   packages=find_packages(), # package module
   # add from requirement.txt,本地测试注释所有包，不能从镜像立即安装
   install_requires=[
     #'Pillow>=10.3.0',
     #'Requests>=2.31.0',
```

