# Comparing `tmp/scriptman-0.0.0.8.tar.gz` & `tmp/scriptman-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptman-0.0.0.8.tar", last modified: Sun Sep 24 18:53:07 2023, max compression
+gzip compressed data, was "scriptman-0.0.0.9.tar", last modified: Sun Sep 24 18:59:59 2023, max compression
```

## Comparing `scriptman-0.0.0.8.tar` & `scriptman-0.0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-09-24 18:53:07.132855 scriptman-0.0.0.8/
--rw-rw-rw-   0        0        0       64 2023-09-24 16:27:01.000000 scriptman-0.0.0.8/.gitignore
-drwxrwxrwx   0        0        0        0 2023-09-24 18:53:07.076902 scriptman-0.0.0.8/.vscode/
--rw-rw-rw-   0        0        0      516 2023-09-24 12:28:16.000000 scriptman-0.0.0.8/.vscode/launch.json
--rw-rw-rw-   0        0        0      235 2023-09-24 15:22:35.000000 scriptman-0.0.0.8/.vscode/settings.json
--rw-rw-rw-   0        0        0      701 2023-09-24 18:53:07.130790 scriptman-0.0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4272 2023-09-24 18:18:48.000000 scriptman-0.0.0.8/publish.py
--rw-rw-rw-   0        0        0      102 2023-09-24 12:38:16.000000 scriptman-0.0.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-09-24 18:53:07.112493 scriptman-0.0.0.8/scriptman/
--rw-rw-rw-   0        0        0     1969 2023-09-24 16:16:26.000000 scriptman-0.0.0.8/scriptman/__init__.py
--rw-rw-rw-   0        0        0     9360 2023-09-24 16:10:48.000000 scriptman-0.0.0.8/scriptman/chrome.py
--rw-rw-rw-   0        0        0     5351 2023-09-24 16:07:06.000000 scriptman-0.0.0.8/scriptman/cleanup.py
--rw-rw-rw-   0        0        0     2967 2023-09-24 15:59:32.000000 scriptman-0.0.0.8/scriptman/cli.py
--rw-rw-rw-   0        0        0     3104 2023-09-24 16:06:20.000000 scriptman-0.0.0.8/scriptman/csv_handler.py
--rw-rw-rw-   0        0        0     9680 2023-09-24 14:07:50.000000 scriptman-0.0.0.8/scriptman/database.py
--rw-rw-rw-   0        0        0     7439 2023-09-24 16:17:35.000000 scriptman-0.0.0.8/scriptman/directories.py
--rw-rw-rw-   0        0        0    20515 2023-09-24 18:51:53.000000 scriptman-0.0.0.8/scriptman/etl.py
--rw-rw-rw-   0        0        0     4968 2023-09-24 16:15:06.000000 scriptman-0.0.0.8/scriptman/interactions.py
--rw-rw-rw-   0        0        0     5061 2023-09-24 16:12:40.000000 scriptman-0.0.0.8/scriptman/logs.py
--rw-rw-rw-   0        0        0     7944 2023-09-24 16:14:17.000000 scriptman-0.0.0.8/scriptman/scripts.py
--rw-rw-rw-   0        0        0     1266 2023-09-24 15:12:05.000000 scriptman-0.0.0.8/scriptman/selenium_handler.py
--rw-rw-rw-   0        0        0    16629 2023-09-24 15:53:28.000000 scriptman-0.0.0.8/scriptman/settings.py
-drwxrwxrwx   0        0        0        0 2023-09-24 18:53:07.127108 scriptman-0.0.0.8/scriptman.egg-info/
--rw-rw-rw-   0        0        0      701 2023-09-24 18:53:06.000000 scriptman-0.0.0.8/scriptman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-09-24 18:53:07.000000 scriptman-0.0.0.8/scriptman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-24 18:53:06.000000 scriptman-0.0.0.8/scriptman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-09-24 18:53:06.000000 scriptman-0.0.0.8/scriptman.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-09-24 18:53:06.000000 scriptman-0.0.0.8/scriptman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-24 18:53:07.133869 scriptman-0.0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      972 2023-09-24 18:52:35.000000 scriptman-0.0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-24 18:59:59.380650 scriptman-0.0.0.9/
+-rw-rw-rw-   0        0        0       64 2023-09-24 16:27:01.000000 scriptman-0.0.0.9/.gitignore
+drwxrwxrwx   0        0        0        0 2023-09-24 18:59:59.312491 scriptman-0.0.0.9/.vscode/
+-rw-rw-rw-   0        0        0      516 2023-09-24 12:28:16.000000 scriptman-0.0.0.9/.vscode/launch.json
+-rw-rw-rw-   0        0        0      235 2023-09-24 15:22:35.000000 scriptman-0.0.0.9/.vscode/settings.json
+-rw-rw-rw-   0        0        0      701 2023-09-24 18:59:59.377653 scriptman-0.0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4272 2023-09-24 18:18:48.000000 scriptman-0.0.0.9/publish.py
+-rw-rw-rw-   0        0        0      102 2023-09-24 12:38:16.000000 scriptman-0.0.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-09-24 18:59:59.357192 scriptman-0.0.0.9/scriptman/
+-rw-rw-rw-   0        0        0     1969 2023-09-24 16:16:26.000000 scriptman-0.0.0.9/scriptman/__init__.py
+-rw-rw-rw-   0        0        0     9360 2023-09-24 16:10:48.000000 scriptman-0.0.0.9/scriptman/chrome.py
+-rw-rw-rw-   0        0        0     5351 2023-09-24 16:07:06.000000 scriptman-0.0.0.9/scriptman/cleanup.py
+-rw-rw-rw-   0        0        0     2967 2023-09-24 15:59:32.000000 scriptman-0.0.0.9/scriptman/cli.py
+-rw-rw-rw-   0        0        0     3104 2023-09-24 16:06:20.000000 scriptman-0.0.0.9/scriptman/csv_handler.py
+-rw-rw-rw-   0        0        0     9680 2023-09-24 14:07:50.000000 scriptman-0.0.0.9/scriptman/database.py
+-rw-rw-rw-   0        0        0     7439 2023-09-24 16:17:35.000000 scriptman-0.0.0.9/scriptman/directories.py
+-rw-rw-rw-   0        0        0    20515 2023-09-24 18:51:53.000000 scriptman-0.0.0.9/scriptman/etl.py
+-rw-rw-rw-   0        0        0     4977 2023-09-24 18:58:19.000000 scriptman-0.0.0.9/scriptman/interactions.py
+-rw-rw-rw-   0        0        0     5061 2023-09-24 16:12:40.000000 scriptman-0.0.0.9/scriptman/logs.py
+-rw-rw-rw-   0        0        0     7944 2023-09-24 16:14:17.000000 scriptman-0.0.0.9/scriptman/scripts.py
+-rw-rw-rw-   0        0        0     1266 2023-09-24 15:12:05.000000 scriptman-0.0.0.9/scriptman/selenium_handler.py
+-rw-rw-rw-   0        0        0    16629 2023-09-24 15:53:28.000000 scriptman-0.0.0.9/scriptman/settings.py
+drwxrwxrwx   0        0        0        0 2023-09-24 18:59:59.372220 scriptman-0.0.0.9/scriptman.egg-info/
+-rw-rw-rw-   0        0        0      701 2023-09-24 18:59:59.000000 scriptman-0.0.0.9/scriptman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-09-24 18:59:59.000000 scriptman-0.0.0.9/scriptman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-24 18:59:59.000000 scriptman-0.0.0.9/scriptman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-09-24 18:59:59.000000 scriptman-0.0.0.9/scriptman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-09-24 18:59:59.000000 scriptman-0.0.0.9/scriptman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-09-24 18:59:59.380905 scriptman-0.0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      972 2023-09-24 18:59:31.000000 scriptman-0.0.0.9/setup.py
```

### Comparing `scriptman-0.0.0.8/.vscode/launch.json` & `scriptman-0.0.0.9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/PKG-INFO` & `scriptman-0.0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptman
-Version: 0.0.0.8
+Version: 0.0.0.9
 Summary: Script Manager assists with managing python scripts.
 Author: Nelson Ombuya
 Author-email: nelson.ombuya@zohomail.com
 Keywords: python,scripts,etl,selenium
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scriptman-0.0.0.8/publish.py` & `scriptman-0.0.0.9/publish.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/__init__.py` & `scriptman-0.0.0.9/scriptman/__init__.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/chrome.py` & `scriptman-0.0.0.9/scriptman/chrome.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/cleanup.py` & `scriptman-0.0.0.9/scriptman/cleanup.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/cli.py` & `scriptman-0.0.0.9/scriptman/cli.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/csv_handler.py` & `scriptman-0.0.0.9/scriptman/csv_handler.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/database.py` & `scriptman-0.0.0.9/scriptman/database.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/directories.py` & `scriptman-0.0.0.9/scriptman/directories.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/etl.py` & `scriptman-0.0.0.9/scriptman/etl.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/interactions.py` & `scriptman-0.0.0.9/scriptman/interactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,29 +90,29 @@
         Raises:
             ValueError: If an invalid interaction mode is provided.
         """
         wait = WebDriverWait(self._driver, timeout)
         if mode == Interaction.WAIT_TILL_INVISIBLE:
             wait.until(EC.invisibility_of_element_located((By.XPATH, xpath)))
             return
+        elif mode == Interaction.DENY_COOKIES:
+            return self.interact_with_element(
+                mode=Interaction.JS_CLICK,
+                xpath=xpath or '//*[@id="tarteaucitronAllDenied2"]',
+            )
 
         element = wait.until(EC.element_to_be_clickable((By.XPATH, xpath)))
         ActionChains(self._driver).move_to_element(element).perform()
 
         if mode == Interaction.CLICK:
             element.click()
         elif mode == Interaction.JS_CLICK:
             self._driver.execute_script("arguments[0].click();", element)
         elif mode == Interaction.SEND_KEYS:
             element.send_keys(keys)
-        elif mode == Interaction.DENY_COOKIES:
-            return self.interact_with_element(
-                mode=Interaction.JS_CLICK,
-                xpath='//*[@id="tarteaucitronAllDenied2"]',
-            )
         else:
             raise ValueError(f"Passed Invalid Mode: {mode}")
         time.sleep(2 if Settings.debug_mode else rest)
 
     def wait_for_downloads_to_finish(self) -> None:
         """
         Wait for all downloads to finish before continuing.
```

### Comparing `scriptman-0.0.0.8/scriptman/logs.py` & `scriptman-0.0.0.9/scriptman/logs.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/scripts.py` & `scriptman-0.0.0.9/scriptman/scripts.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/selenium_handler.py` & `scriptman-0.0.0.9/scriptman/selenium_handler.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman/settings.py` & `scriptman-0.0.0.9/scriptman/settings.py`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/scriptman.egg-info/PKG-INFO` & `scriptman-0.0.0.9/scriptman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptman
-Version: 0.0.0.8
+Version: 0.0.0.9
 Summary: Script Manager assists with managing python scripts.
 Author: Nelson Ombuya
 Author-email: nelson.ombuya@zohomail.com
 Keywords: python,scripts,etl,selenium
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scriptman-0.0.0.8/scriptman.egg-info/SOURCES.txt` & `scriptman-0.0.0.9/scriptman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scriptman-0.0.0.8/setup.py` & `scriptman-0.0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = "0.0.0.8"
+VERSION = "0.0.0.9"
 DESCRIPTION = "Script Manager assists with managing python scripts."
 
 setup(
     name="scriptman",
     version=VERSION,
     author="Nelson Ombuya",
     description=DESCRIPTION,
```

