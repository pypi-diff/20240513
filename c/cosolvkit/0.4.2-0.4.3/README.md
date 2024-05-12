# Comparing `tmp/cosolvkit-0.4.2.tar.gz` & `tmp/cosolvkit-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosolvkit-0.4.2.tar", last modified: Tue May  7 01:17:24 2024, max compression
+gzip compressed data, was "cosolvkit-0.4.3.tar", last modified: Sun May 12 22:36:56 2024, max compression
```

## Comparing `cosolvkit-0.4.2.tar` & `cosolvkit-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.145645 cosolvkit-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/cosolvkit/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    58843 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/cosolvent_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/cosolvkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/aromatic.json
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/cosolvents.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/forcefields.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/h_bonding.json
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/lipophilic.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/negative.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/data/positive.json
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/cosolvkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/cosolvkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 01:17:24.000000 cosolvkit-0.4.2/cosolvkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:17:24.141646 cosolvkit-0.4.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/scripts/create_cosolvent_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/scripts/post_simulation_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:17:24.145645 cosolvkit-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-07 01:17:16.000000 cosolvkit-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:36:56.162469 cosolvkit-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-12 22:36:56.158470 cosolvkit-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:36:56.158470 cosolvkit-0.4.3/cosolvkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25858 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58843 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/cosolvent_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:36:56.158470 cosolvkit-0.4.3/cosolvkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/aromatic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/cosolvents.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/forcefields.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/h_bonding.json
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/lipophilic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/negative.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/data/positive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/cosolvkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:36:56.158470 cosolvkit-0.4.3/cosolvkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 22:36:56.000000 cosolvkit-0.4.3/cosolvkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 22:36:56.162469 cosolvkit-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-12 22:36:48.000000 cosolvkit-0.4.3/setup.py
```

### Comparing `cosolvkit-0.4.2/LICENSE` & `cosolvkit-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.2/PKG-INFO` & `cosolvkit-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosolvkit
-Version: 0.4.2
+Version: 0.4.3
 Summary: CosolvKit
 Home-page: https://github.com/forlilab/cosolvkit
 Author: Niccolo Bruciaferri, Jerome Eberhardt
 Author-email: forli@scripps.edu
 License: LGPL-2.1
 Keywords: molecular modeling,drug design,cosolvent,MD simulations
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `cosolvkit-0.4.2/README.md` & `cosolvkit-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) [![PyPI - Version](https://img.shields.io/pypi/v/cosolvkit)](https://pypi.org/project/cosolvkit/0.4.1/) [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![License: LGPL v2.1](https://img.shields.io/badge/License-LGPL_v2.1-green.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html) [![PyPI - Version](https://img.shields.io/pypi/v/cosolvkit)](https://pypi.org/project/cosolvkit/0.4.3/) [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
 [![Documentation Status](https://readthedocs.org/projects/cosolvkit/badge/?version=latest)](https://cosolvkit.readthedocs.io/en/latest/?badge=latest)
       
     
 
 # CosolvKit
 The python package for creating cosolvent system.
```

### Comparing `cosolvkit-0.4.2/cosolvkit/analysis.py` & `cosolvkit-0.4.3/cosolvkit/analysis.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.2/cosolvkit/config.py` & `cosolvkit-0.4.3/cosolvkit/config.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.2/cosolvkit/cosolvent_system.py` & `cosolvkit-0.4.3/cosolvkit/cosolvent_system.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.2/cosolvkit/data/config.json` & `cosolvkit-0.4.3/cosolvkit/data/config.json`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.2/cosolvkit/data/cosolvents.json` & `cosolvkit-0.4.3/cosolvkit/data/cosolvents.json`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.2/cosolvkit/simulation.py` & `cosolvkit-0.4.3/cosolvkit/simulation.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.2/cosolvkit/utils.py` & `cosolvkit-0.4.3/cosolvkit/utils.py`

 * *Files identical despite different names*

### Comparing `cosolvkit-0.4.2/cosolvkit.egg-info/PKG-INFO` & `cosolvkit-0.4.3/cosolvkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosolvkit
-Version: 0.4.2
+Version: 0.4.3
 Summary: CosolvKit
 Home-page: https://github.com/forlilab/cosolvkit
 Author: Niccolo Bruciaferri, Jerome Eberhardt
 Author-email: forli@scripps.edu
 License: LGPL-2.1
 Keywords: molecular modeling,drug design,cosolvent,MD simulations
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `cosolvkit-0.4.2/cosolvkit.egg-info/SOURCES.txt` & `cosolvkit-0.4.3/cosolvkit.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 cosolvkit/config.py
 cosolvkit/cosolvent_system.py
 cosolvkit/simulation.py
 cosolvkit/utils.py
 cosolvkit.egg-info/PKG-INFO
 cosolvkit.egg-info/SOURCES.txt
 cosolvkit.egg-info/dependency_links.txt
+cosolvkit.egg-info/entry_points.txt
 cosolvkit.egg-info/not-zip-safe
 cosolvkit.egg-info/top_level.txt
 cosolvkit/data/aromatic.json
 cosolvkit/data/config.json
 cosolvkit/data/cosolvents.json
 cosolvkit/data/forcefields.json
 cosolvkit/data/h_bonding.json
 cosolvkit/data/lipophilic.json
 cosolvkit/data/negative.json
-cosolvkit/data/positive.json
-scripts/create_cosolvent_system.py
-scripts/post_simulation_processing.py
+cosolvkit/data/positive.json
```

### Comparing `cosolvkit-0.4.2/setup.py` & `cosolvkit-0.4.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,31 +14,37 @@
         for filename in fnmatch.filter(filenames, '*'):
             matches.append(os.path.join(root, filename))
 
     return matches
 
 
 setup(name="cosolvkit",
-      version='0.4.2',
+      version='0.4.3',
       description="CosolvKit",
       author="Niccolo Bruciaferri, Jerome Eberhardt",
       author_email="forli@scripps.edu",
       url="https://github.com/forlilab/cosolvkit",
-      packages=find_packages(),
-      scripts=["scripts/create_cosolvent_system.py",
-               "scripts/post_simulation_processing.py"],
+      packages=find_packages(exclude=['docs']),
+    #   scripts=["scripts/create_cosolvent_system.py",
+    #            "scripts/post_simulation_processing.py"],
       package_data={"cosolvkit" : ["data/*"]},
-      data_files=[("", ["README.md", "LICENSE"]),
-                  ("scripts", find_files("scripts"))],
+      data_files=[("", ["README.md", "LICENSE"])],
       include_package_data=True,
       zip_safe=False,
       python_requires=">=3.9, <3.12",
       license="LGPL-2.1",
       keywords=["molecular modeling", "drug design",
                 "cosolvent", "MD simulations"],
       classifiers=["Programming Language :: Python :: 3.9",
                    "Programming Language :: Python :: 3.10",
                    "Programming Language :: Python :: 3.11",
                    "Operating System :: Unix",
                    "Operating System :: MacOS",
-                   "Topic :: Scientific/Engineering"]
+                   "Topic :: Scientific/Engineering"],
+      entry_points={
+          'console_scripts': [
+              'create_cosolvent_system=scripts.create_cosolvent_system:main',
+              'post_simulation_processing=scripts.post_simulation_processing:main'
+          ]
+      }
+      
 )
```

