# Comparing `tmp/virgo_modules-0.0.84.tar.gz` & `tmp/virgo_modules-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.84.tar", last modified: Thu May  2 07:45:51 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.85.tar", last modified: Mon May 13 19:18:57 2024, max compression
```

## Comparing `virgo_modules-0.0.84.tar` & `virgo_modules-0.0.85.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.564259 virgo_modules-0.0.84/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.84/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-05-02 07:45:51.555098 virgo_modules-0.0.84/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.84/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 07:45:51.565260 virgo_modules-0.0.84/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-05-02 07:45:11.000000 virgo_modules-0.0.84/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.460379 virgo_modules-0.0.84/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.496394 virgo_modules-0.0.84/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.550093 virgo_modules-0.0.84/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    71652 2024-04-27 12:41:59.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   143298 2024-05-02 07:44:54.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.521894 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.881178 virgo_modules-0.0.85/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.85/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-05-13 19:18:57.878178 virgo_modules-0.0.85/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.85/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 19:18:57.883186 virgo_modules-0.0.85/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-05-13 19:18:08.000000 virgo_modules-0.0.85/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.795129 virgo_modules-0.0.85/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.822816 virgo_modules-0.0.85/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.871010 virgo_modules-0.0.85/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    71603 2024-05-13 19:18:08.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   143298 2024-05-02 07:44:54.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.840006 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.84/LICENSE` & `virgo_modules-0.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.84/PKG-INFO` & `virgo_modules-0.0.85/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo_modules
-Version: 0.0.84
+Version: 0.0.85
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.84/setup.py` & `virgo_modules-0.0.85/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.84",
+    version="0.0.85",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.84/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.85/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.84/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.85/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.84/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.85/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.84/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.85/virgo_app/virgo_modules/src/re_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1153,16 +1153,16 @@
 
         
         fig.update_layout(height=height_plot, width=1600, title_text = f'State model analysis: {self.ticket_name}', coloraxis=dict(colorbar_len=0.50))
 
         date_execution = datetime.datetime.today().strftime('%Y-%m-%d')
         current_step = df.iloc[-1,:].hmm_chain_order
         current_state = df.iloc[-1,:].hmm_feature
-        message1 = 'current state: ' +  str(current_state)
-        message2 = 'current step in state: ' + str(current_step)
+        message1 = str(current_state)
+        message2 = str(current_step)
         message3 = str(date_execution)
 
         messages = {
             'current state':message1,
             'current step in state': message2,
             'execution date':message3,
         }
```

### Comparing `virgo_modules-0.0.84/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.85/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo-modules
-Version: 0.0.84
+Version: 0.0.85
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

