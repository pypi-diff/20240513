# Comparing `tmp/connectlife-0.0.3.tar.gz` & `tmp/connectlife-0.0.4.tar.gz`

## Comparing `connectlife-0.0.3.tar` & `connectlife-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 connectlife-0.0.3/.github/workflows/python-publish.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 connectlife-0.0.3/connectlife/__init__.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 connectlife-0.0.3/connectlife/api.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 connectlife-0.0.3/connectlife/appliance.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 connectlife-0.0.3/connectlife/dump.py
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_dishwasher.json
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_hood_1.json
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_hood_2.json
--rw-r--r--   0        0        0    14445 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_induction_hob_1.json
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_induction_hob_2.json
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_professional_tumble_dryer.json
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_professional_washing_machine.json
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Gorenje_dishwasher.json
--rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Gorenje_washing_machine.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Heat_pump.json
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Oven_type_1.json
--rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Oven_type_2.json
--rw-r--r--   0        0        0   587306 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/format.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 connectlife-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 connectlife-0.0.3/LICENSE
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 connectlife-0.0.3/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 connectlife-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 connectlife-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 connectlife-0.0.4/.github/workflows/python-publish.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 connectlife-0.0.4/connectlife/__init__.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 connectlife-0.0.4/connectlife/api.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 connectlife-0.0.4/connectlife/appliance.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 connectlife-0.0.4/connectlife/dump.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_dishwasher.json
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_hood_1.json
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_hood_2.json
+-rw-r--r--   0        0        0    14445 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_induction_hob_1.json
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_induction_hob_2.json
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_professional_tumble_dryer.json
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Asko_professional_washing_machine.json
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Gorenje_dishwasher.json
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Gorenje_washing_machine.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Heat_pump.json
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Oven_type_1.json
+-rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/Oven_type_2.json
+-rw-r--r--   0        0        0   587306 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 connectlife-0.0.4/dumps/format.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 connectlife-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 connectlife-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 connectlife-0.0.4/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 connectlife-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 connectlife-0.0.4/PKG-INFO
```

### Comparing `connectlife-0.0.3/.github/workflows/python-publish.yaml` & `connectlife-0.0.4/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/connectlife/api.py` & `connectlife-0.0.4/connectlife/api.py`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/connectlife/appliance.py` & `connectlife-0.0.4/connectlife/appliance.py`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Asko_dishwasher.json` & `connectlife-0.0.4/dumps/Asko_dishwasher.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Asko_hood_1.json` & `connectlife-0.0.4/dumps/Asko_hood_1.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Asko_hood_2.json` & `connectlife-0.0.4/dumps/Asko_hood_2.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Asko_induction_hob_1.json` & `connectlife-0.0.4/dumps/Asko_induction_hob_1.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Asko_induction_hob_2.json` & `connectlife-0.0.4/dumps/Asko_induction_hob_2.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Asko_professional_tumble_dryer.json` & `connectlife-0.0.4/dumps/Asko_professional_tumble_dryer.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Asko_professional_washing_machine.json` & `connectlife-0.0.4/dumps/Asko_professional_washing_machine.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Gorenje_dishwasher.json` & `connectlife-0.0.4/dumps/Gorenje_dishwasher.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Gorenje_washing_machine.json` & `connectlife-0.0.4/dumps/Gorenje_washing_machine.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Heat_pump.json` & `connectlife-0.0.4/dumps/Heat_pump.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Oven_type_1.json` & `connectlife-0.0.4/dumps/Oven_type_1.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/Oven_type_2.json` & `connectlife-0.0.4/dumps/Oven_type_2.json`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/README.md` & `connectlife-0.0.4/dumps/README.md`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/dumps/format.py` & `connectlife-0.0.4/dumps/format.py`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/LICENSE` & `connectlife-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/README.md` & `connectlife-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.3/pyproject.toml` & `connectlife-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "connectlife"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Øyvind Matheson Wergeland", email="oyvind@wergeland.org" },
 ]
 description = "A Python library for communicating with the ConnectLife API"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `connectlife-0.0.3/PKG-INFO` & `connectlife-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: connectlife
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library for communicating with the ConnectLife API
 Project-URL: Homepage, https://github.com/oyvindwe/connectlife
 Project-URL: Issues, https://github.com/oyvindwe/connectlife/issues
 Author-email: Øyvind Matheson Wergeland <oyvind@wergeland.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

