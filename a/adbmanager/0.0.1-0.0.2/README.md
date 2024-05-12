# Comparing `tmp/adbmanager-0.0.1.tar.gz` & `tmp/adbmanager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbmanager-0.0.1.tar", last modified: Sun May 12 21:55:02 2024, max compression
+gzip compressed data, was "adbmanager-0.0.2.tar", last modified: Sun May 12 22:39:22 2024, max compression
```

## Comparing `adbmanager-0.0.1.tar` & `adbmanager-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 21:55:02.384061 adbmanager-0.0.1/
--rw-rw-rw-   0        0        0     1090 2024-05-12 21:32:13.000000 adbmanager-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1036 2024-05-12 21:55:02.383062 adbmanager-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 21:26:23.000000 adbmanager-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 21:55:02.382063 adbmanager-0.0.1/adbmanager.egg-info/
--rw-rw-rw-   0        0        0     1036 2024-05-12 21:55:02.000000 adbmanager-0.0.1/adbmanager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-05-12 21:55:02.000000 adbmanager-0.0.1/adbmanager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 21:55:02.000000 adbmanager-0.0.1/adbmanager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 21:55:02.000000 adbmanager-0.0.1/adbmanager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      961 2024-05-12 21:52:24.000000 adbmanager-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 21:55:02.384061 adbmanager-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      384 2024-05-12 21:47:16.000000 adbmanager-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:39:22.640961 adbmanager-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-12 21:32:13.000000 adbmanager-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      975 2024-05-12 22:39:22.639963 adbmanager-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 22:18:39.000000 adbmanager-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 22:39:22.632961 adbmanager-0.0.2/adbmanager/
+-rw-rw-rw-   0        0        0        0 2024-05-12 22:28:07.000000 adbmanager-0.0.2/adbmanager/__init__.py
+-rw-rw-rw-   0        0        0     4508 2024-05-12 21:46:08.000000 adbmanager-0.0.2/adbmanager/adbmanager.py
+-rw-rw-rw-   0        0        0     1570 2024-05-12 20:31:25.000000 adbmanager-0.0.2/adbmanager/deviceInfo.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:39:22.638961 adbmanager-0.0.2/adbmanager/keyboardEvents/
+-rw-rw-rw-   0        0        0        0 2024-05-12 21:05:26.000000 adbmanager-0.0.2/adbmanager/keyboardEvents/__init__.py
+-rw-rw-rw-   0        0        0      406 2024-05-12 22:28:59.000000 adbmanager-0.0.2/adbmanager/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:39:22.638961 adbmanager-0.0.2/adbmanager.egg-info/
+-rw-rw-rw-   0        0        0      975 2024-05-12 22:39:22.000000 adbmanager-0.0.2/adbmanager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-12 22:39:22.000000 adbmanager-0.0.2/adbmanager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 22:39:22.000000 adbmanager-0.0.2/adbmanager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 22:39:22.000000 adbmanager-0.0.2/adbmanager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      961 2024-05-12 22:34:39.000000 adbmanager-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 22:39:22.640961 adbmanager-0.0.2/setup.cfg
```

### Comparing `adbmanager-0.0.1/LICENSE` & `adbmanager-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adbmanager-0.0.1/PKG-INFO` & `adbmanager-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: adbmanager
-Version: 0.0.1
+Version: 0.0.2
 Summary: adbmanager is a small library for managing and administrating Android devices through ADB, developed by Frankelly Franco and distributed by Francarium Platforms. This tool will assist you in controlling each Android device in an organized manner through ADB, assuming it is installed. With adbmanager, you can streamline management tasks such as installing applications, transferring files, executing commands in the shell, and more, on connected Android devices via ADB.
-Home-page: https://francarium.com
-Author: Frankelly Franco
 Author-email: Frankelly Franco <lic.frankellyfranco@gmail.com>
 Project-URL: Homepage, https://github.com/francarium/adbmanager
 Project-URL: Issues, https://github.com/francarium/adbmanager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `adbmanager-0.0.1/adbmanager.egg-info/PKG-INFO` & `adbmanager-0.0.2/adbmanager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: adbmanager
-Version: 0.0.1
+Version: 0.0.2
 Summary: adbmanager is a small library for managing and administrating Android devices through ADB, developed by Frankelly Franco and distributed by Francarium Platforms. This tool will assist you in controlling each Android device in an organized manner through ADB, assuming it is installed. With adbmanager, you can streamline management tasks such as installing applications, transferring files, executing commands in the shell, and more, on connected Android devices via ADB.
-Home-page: https://francarium.com
-Author: Frankelly Franco
 Author-email: Frankelly Franco <lic.frankellyfranco@gmail.com>
 Project-URL: Homepage, https://github.com/francarium/adbmanager
 Project-URL: Issues, https://github.com/francarium/adbmanager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `adbmanager-0.0.1/pyproject.toml` & `adbmanager-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "adbmanager"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Frankelly Franco", email="lic.frankellyfranco@gmail.com" },
 ]
 description = "adbmanager is a small library for managing and administrating Android devices through ADB, developed by Frankelly Franco and distributed by Francarium Platforms. This tool will assist you in controlling each Android device in an organized manner through ADB, assuming it is installed. With adbmanager, you can streamline management tasks such as installing applications, transferring files, executing commands in the shell, and more, on connected Android devices via ADB."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

