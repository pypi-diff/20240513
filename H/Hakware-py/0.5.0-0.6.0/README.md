# Comparing `tmp/Hakware-py-0.5.0.tar.gz` & `tmp/Hakware-py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hakware-py-0.5.0.tar", last modified: Mon May 13 09:45:00 2024, max compression
+gzip compressed data, was "Hakware-py-0.6.0.tar", last modified: Mon May 13 13:24:59 2024, max compression
```

## Comparing `Hakware-py-0.5.0.tar` & `Hakware-py-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 09:45:00.703483 Hakware-py-0.5.0/
-drwxrwxrwx   0        0        0        0 2024-05-13 09:45:00.681983 Hakware-py-0.5.0/Hakware-py/
--rw-rw-rw-   0        0        0     9613 2024-05-13 09:34:51.000000 Hakware-py-0.5.0/Hakware-py/HakwareObserverpy.py
--rw-rw-rw-   0        0        0      255 2024-05-13 09:44:17.000000 Hakware-py-0.5.0/Hakware-py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:45:00.702483 Hakware-py-0.5.0/Hakware_py.egg-info/
--rw-rw-rw-   0        0        0      702 2024-05-13 09:45:00.000000 Hakware-py-0.5.0/Hakware_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-13 09:45:00.000000 Hakware-py-0.5.0/Hakware_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 09:45:00.000000 Hakware-py-0.5.0/Hakware_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-05-13 09:45:00.000000 Hakware-py-0.5.0/Hakware_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 09:45:00.000000 Hakware-py-0.5.0/Hakware_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      702 2024-05-13 09:45:00.703483 Hakware-py-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-13 09:19:09.000000 Hakware-py-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 09:45:00.704485 Hakware-py-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1161 2024-05-13 09:30:45.000000 Hakware-py-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:24:59.753779 Hakware-py-0.6.0/
+drwxrwxrwx   0        0        0        0 2024-05-13 13:24:59.733562 Hakware-py-0.6.0/Hakware-py/
+-rw-rw-rw-   0        0        0     9609 2024-05-13 13:24:29.000000 Hakware-py-0.6.0/Hakware-py/HakwareObserverpy.py
+-rw-rw-rw-   0        0        0      255 2024-05-13 13:24:21.000000 Hakware-py-0.6.0/Hakware-py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:24:59.752778 Hakware-py-0.6.0/Hakware_py.egg-info/
+-rw-rw-rw-   0        0        0      702 2024-05-13 13:24:59.000000 Hakware-py-0.6.0/Hakware_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-13 13:24:59.000000 Hakware-py-0.6.0/Hakware_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 13:24:59.000000 Hakware-py-0.6.0/Hakware_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-13 13:24:59.000000 Hakware-py-0.6.0/Hakware_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 13:24:59.000000 Hakware-py-0.6.0/Hakware_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      702 2024-05-13 13:24:59.752778 Hakware-py-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-13 09:19:09.000000 Hakware-py-0.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 13:24:59.753779 Hakware-py-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-05-13 13:24:13.000000 Hakware-py-0.6.0/setup.py
```

### Comparing `Hakware-py-0.5.0/Hakware-py/HakwareObserverpy.py` & `Hakware-py-0.6.0/Hakware-py/HakwareObserverpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,16 +150,14 @@
         #"disk_usage_percent": disk_usage,
         "total_memory": total_memory_gb,
         "total_cpus": total_cpus,
         "total_cores": total_cores
     }
 
 
-
-
 ###############################################################################################################################################################################
 
 def LinInitiateCollecection(HWDeviceID, ObserverVersion):  
    
 
     get_system_usage(HWDeviceID,ObserverVersion)
```

### Comparing `Hakware-py-0.5.0/Hakware_py.egg-info/PKG-INFO` & `Hakware-py-0.6.0/Hakware_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hakware-py
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package connect endpoints to the Hakware Application
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Hakware-py-0.5.0/PKG-INFO` & `Hakware-py-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hakware-py
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package connect endpoints to the Hakware Application
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Hakware-py-0.5.0/setup.py` & `Hakware-py-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Hakware-py',  # Your package name
-    version='0.5.0',  # Start with a version number
+    version='0.6.0',  # Start with a version number
     description='A package connect endpoints to the Hakware Application',  # Short description
     long_description=open('README.md').read(),  # Long description from README
     long_description_content_type='text/markdown',
     author='Jacob O\'Brien',  # Your name
     # author_email='your.email@example.com',  # Your email
     # url='https://github.com/your-username/XGRCPy',  # Your package's URL (if applicable)
     packages=find_packages(),  # Find all sub-packages
     install_requires=[  # Add your package dependencies here
         'requests',
         'psutil',
         'requests_html',
-        'subprocess',
         'winreg',
         'json',
         'platform',
         'traceback',
         'datetime'
 
     ],
```

