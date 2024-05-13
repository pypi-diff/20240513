# Comparing `tmp/revhubinterface-1.3.3.dev2.tar.gz` & `tmp/revhubinterface-1.3.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.3.dev2.tar", last modified: Sun May 12 02:34:19 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.3.dev3.tar", last modified: Mon May 13 18:17:50 2024, max compression
```

## Comparing `revhubinterface-1.3.3.dev2.tar` & `revhubinterface-1.3.3.dev3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:34:19.391183 revhubinterface-1.3.3.dev2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:34:19.383183 revhubinterface-1.3.3.dev2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:34:19.387183 revhubinterface-1.3.3.dev2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-12 02:34:19.391183 revhubinterface-1.3.3.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:34:19.387183 revhubinterface-1.3.3.dev2/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:34:19.391183 revhubinterface-1.3.3.dev2/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-12 02:34:19.000000 revhubinterface-1.3.3.dev2/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-12 02:34:19.000000 revhubinterface-1.3.3.dev2/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 02:34:19.000000 revhubinterface-1.3.3.dev2/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-12 02:34:19.000000 revhubinterface-1.3.3.dev2/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-12 02:34:19.000000 revhubinterface-1.3.3.dev2/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 02:34:19.000000 revhubinterface-1.3.3.dev2/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:34:19.391183 revhubinterface-1.3.3.dev2/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/flatpak/flatpak-pip-generator
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/flatpak/org.unofficialrevport.REVHubInterface.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/org.unofficialrevport.REVHubInterface.Devel.svg
--rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/org.unofficialrevport.REVHubInterface.Source.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/org.unofficialrevport.REVHubInterface.svg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 02:34:14.000000 revhubinterface-1.3.3.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 02:34:19.391183 revhubinterface-1.3.3.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.438745 revhubinterface-1.3.3.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.438745 revhubinterface-1.3.3.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/flatpak/flatpak-pip-generator
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/flatpak/org.unofficialrevport.REVHubInterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:17:50.446745 revhubinterface-1.3.3.dev3/setup.cfg
```

### Comparing `revhubinterface-1.3.3.dev2/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.3.dev3/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/.github/workflows/python-publish.yml` & `revhubinterface-1.3.3.dev3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/LICENSE.txt` & `revhubinterface-1.3.3.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/PKG-INFO` & `revhubinterface-1.3.3.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev2
+Version: 1.3.3.dev3
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev2/README.md` & `revhubinterface-1.3.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVADC.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVModule.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVServo.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface/__main__.py` & `revhubinterface-1.3.3.dev3/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev2
+Version: 1.3.3.dev3
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 LICENSE.txt
 README.md
 REVHubInterface.sh
 REVHubInterface.spec
 org.unofficialrevport.REVHubInterface.Devel.svg
 org.unofficialrevport.REVHubInterface.Source.svg
+org.unofficialrevport.REVHubInterface.metainfo.xml
 org.unofficialrevport.REVHubInterface.svg
 pyproject.toml
 requirements.txt
 .github/workflows/pyinstaller.yml
 .github/workflows/python-publish.yml
 REVHubInterface/REV2mSensor.py
 REVHubInterface/REVADC.py
```

### Comparing `revhubinterface-1.3.3.dev2/REVHubInterface.spec` & `revhubinterface-1.3.3.dev3/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.3.dev3/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.3.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/flatpak/python3-requirements.json` & `revhubinterface-1.3.3.dev3/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/org.unofficialrevport.REVHubInterface.Devel.svg` & `revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.Devel.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/org.unofficialrevport.REVHubInterface.Source.svg` & `revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.Source.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/org.unofficialrevport.REVHubInterface.svg` & `revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev2/pyproject.toml` & `revhubinterface-1.3.3.dev3/pyproject.toml`

 * *Files identical despite different names*

