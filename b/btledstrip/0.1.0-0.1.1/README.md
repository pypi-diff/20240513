# Comparing `tmp/btledstrip-0.1.0.tar.gz` & `tmp/btledstrip-0.1.1.tar.gz`

## Comparing `btledstrip-0.1.0.tar` & `btledstrip-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 btledstrip-0.1.0/.editorconfig
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 btledstrip-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 btledstrip-0.1.0/.tool-versions
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 btledstrip-0.1.0/Makefile
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 btledstrip-0.1.0/Pipfile
--rw-r--r--   0        0        0    31069 2020-02-02 00:00:00.000000 btledstrip-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 btledstrip-0.1.0/requirements.txt
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 btledstrip-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 btledstrip-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 btledstrip-0.1.0/btledstrip/__init__.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 btledstrip-0.1.0/btledstrip/controllers.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 btledstrip-0.1.0/btledstrip/dev.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 btledstrip-0.1.0/btledstrip/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 btledstrip-0.1.0/btledstrip/demonstrations/__init__.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 btledstrip-0.1.0/btledstrip/demonstrations/melk.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 btledstrip-0.1.0/docs/conf.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 btledstrip-0.1.0/docs/index.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 btledstrip-0.1.0/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 btledstrip-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 btledstrip-0.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 btledstrip-0.1.0/LICENSE
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 btledstrip-0.1.0/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 btledstrip-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 btledstrip-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.tool-versions
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 btledstrip-0.1.1/Makefile
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 btledstrip-0.1.1/Pipfile
+-rw-r--r--   0        0        0    31069 2020-02-02 00:00:00.000000 btledstrip-0.1.1/Pipfile.lock
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 btledstrip-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/__init__.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/controllers.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/dev.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/demonstrations/__init__.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 btledstrip-0.1.1/btledstrip/demonstrations/melk.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 btledstrip-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 btledstrip-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 btledstrip-0.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 btledstrip-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 btledstrip-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 btledstrip-0.1.1/LICENSE
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 btledstrip-0.1.1/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 btledstrip-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 btledstrip-0.1.1/PKG-INFO
```

### Comparing `btledstrip-0.1.0/Makefile` & `btledstrip-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.0/Pipfile.lock` & `btledstrip-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.0/.github/workflows/python-publish.yml` & `btledstrip-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.0/btledstrip/__init__.py` & `btledstrip-0.1.1/btledstrip/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,8 +119,8 @@
 __all__ = [
     "BTLedStrip",
     "Controller",
     "MELKController",
     "Command",
 ]
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
```

### Comparing `btledstrip-0.1.0/btledstrip/controllers.py` & `btledstrip-0.1.1/btledstrip/controllers.py`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.0/btledstrip/dev.py` & `btledstrip-0.1.1/btledstrip/dev.py`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.0/btledstrip/demonstrations/melk.py` & `btledstrip-0.1.1/btledstrip/demonstrations/melk.py`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.0/docs/index.rst` & `btledstrip-0.1.1/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 Python LED Strip Bluetooth Controller API was created by `Douglas Paz <https://www.douglaspaz.com/>`_ implemented with `bleak <https://github.com/hbldh/bleak>`_.
 
 Supported controllers/devices
 =============================
 
 - MELK: :class:`MELKController<btledstrip.MELKController>`
 
+Install
+=======
+
+Install from Pypi repository.
+
+.. code-block:: console
+
+   pip install btledstrip
+
 Usage
 =====
 
 .. code-block:: python
 
    from btledstrip import (
        BTLedStrip,
```

### Comparing `btledstrip-0.1.0/.gitignore` & `btledstrip-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.0/LICENSE` & `btledstrip-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `btledstrip-0.1.0/pyproject.toml` & `btledstrip-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [project]
 name = "btledstrip"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name="Douglas Paz", email="eu@douglaspaz.com" },
 ]
 description = "Python LED Strip Bluetooth Controller API"
 readme = "README.md"
 requires-python = ">=3.12"
+dependencies = [
+    "bleak==0.22.1",
+    "dbus-fast==2.21.2",
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/dougppaz/python-bt-led-strip"
+Documentation = "https://python-bt-led-strip.readthedocs.io/en/latest/"
 Issues = "https://github.com/dougppaz/python-bt-led-strip/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `btledstrip-0.1.0/PKG-INFO` & `btledstrip-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.3
 Name: btledstrip
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python LED Strip Bluetooth Controller API
 Project-URL: Homepage, https://github.com/dougppaz/python-bt-led-strip
+Project-URL: Documentation, https://python-bt-led-strip.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/dougppaz/python-bt-led-strip/issues
 Author-email: Douglas Paz <eu@douglaspaz.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
+Requires-Dist: bleak==0.22.1
+Requires-Dist: dbus-fast==2.21.2
 Description-Content-Type: text/markdown
 
 # Python LED Strip Bluetooth Controller API
 
 Compatible with MELK devices.
 
 - [Read the Docs](https://python-bt-led-strip.readthedocs.io/)
```

