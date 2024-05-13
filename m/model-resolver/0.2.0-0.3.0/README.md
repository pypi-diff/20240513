# Comparing `tmp/model_resolver-0.2.0.tar.gz` & `tmp/model_resolver-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_resolver-0.2.0.tar", max compression
+gzip compressed data, was "model_resolver-0.3.0.tar", max compression
```

## Comparing `model_resolver-0.2.0.tar` & `model_resolver-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-05-12 15:08:20.291992 model_resolver-0.2.0/LICENSE
--rw-r--r--   0        0        0     1370 2024-05-12 15:08:20.291992 model_resolver-0.2.0/README.md
--rw-r--r--   0        0        0       36 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/__init__.py
--rw-r--r--   0        0        0       59 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/__main__.py
--rw-r--r--   0        0        0     1623 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/cli.py
--rw-r--r--   0        0        0     1474 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/my_glutinit.py
--rw-r--r--   0        0        0    14846 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/plugin.py
--rw-r--r--   0        0        0    18287 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/render.py
--rw-r--r--   0        0        0     1248 2024-05-12 15:08:20.291992 model_resolver-0.2.0/model_resolver/utils.py
--rw-r--r--   0        0        0      714 2024-05-12 15:08:40.623995 model_resolver-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 model_resolver-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-13 10:38:25.142918 model_resolver-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1752 2024-05-13 10:38:25.142918 model_resolver-0.3.0/README.md
+-rw-r--r--   0        0        0       36 2024-05-13 10:38:25.146918 model_resolver-0.3.0/model_resolver/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-13 10:38:25.146918 model_resolver-0.3.0/model_resolver/__main__.py
+-rw-r--r--   0        0        0     1623 2024-05-13 10:38:25.146918 model_resolver-0.3.0/model_resolver/cli.py
+-rw-r--r--   0        0        0     1474 2024-05-13 10:38:25.146918 model_resolver-0.3.0/model_resolver/my_glutinit.py
+-rw-r--r--   0        0        0    14846 2024-05-13 10:38:25.146918 model_resolver-0.3.0/model_resolver/plugin.py
+-rw-r--r--   0        0        0    18114 2024-05-13 10:38:25.146918 model_resolver-0.3.0/model_resolver/render.py
+-rw-r--r--   0        0        0     1248 2024-05-13 10:38:25.146918 model_resolver-0.3.0/model_resolver/utils.py
+-rw-r--r--   0        0        0      715 2024-05-13 10:38:40.502723 model_resolver-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.3.0/PKG-INFO
```

### Comparing `model_resolver-0.2.0/LICENSE` & `model_resolver-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `model_resolver-0.2.0/README.md` & `model_resolver-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,40 @@
 # Model Resolver
 
 A beet plugin that render all models in the beet project.
 
 
 ## Usage
 
+
+### Renders project
+
+Without any installlation, all vanilla models are rendered in this [repository](https://github.com/edayot/renders/tree/renders)
+
+### With the CLI
+
+This command will show all available options:
+
+```bash
+model_resolver --help
+```
+
+```bash
+# this will render the current resource pack models
+model_resolver 
+```
+
+```bash
+# this will render the current resource pack models and load vanilla models
+model_resolver --load-vanilla
+```
+
+
+
+### As a beet plugin
 Add the plugin to your pipeline:
 
 ```yaml
 # beet.yaml
 pipeline:
   (...)  # other plugins you may have
   - model_resolver
@@ -57,17 +83,16 @@
     x11-utils
 ```
 
 This is particularly useful in CI, see [the github action](./.github/workflows/artifact.yml) for an example.
 
 ### Common installation
 
-Using poetry, add this to your pyproject.toml file:
+Install the plugin by running:
 
-```toml
-[tool.poetry.dependencies]
-# (other dependencies ...)
-model-resolver = {git = "https://github.com/edayot/model_resolver.git", branch = "master"}
+```bash
+pip install model-resolver
 ```
 
+Pypi: https://pypi.org/project/model-resolver/
```

### Comparing `model_resolver-0.2.0/model_resolver/cli.py` & `model_resolver-0.3.0/model_resolver/cli.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.2.0/model_resolver/my_glutinit.py` & `model_resolver-0.3.0/model_resolver/my_glutinit.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.2.0/model_resolver/plugin.py` & `model_resolver-0.3.0/model_resolver/plugin.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.2.0/model_resolver/render.py` & `model_resolver-0.3.0/model_resolver/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,24 +126,21 @@
         glutInitWindowPosition(100, 100)
         glutCreateWindow(b"Isometric View")
         glutHideWindow()
         glutSetOption(GLUT_ACTION_ON_WINDOW_CLOSE, GLUT_ACTION_GLUTMAINLOOP_RETURNS)
         glClearColor(0.0, 0.0, 0.0, 0.0)
 
         # Enable lighting
+        MINECRAFT_LIGHT_POWER = 1.0
+        MINECRAFT_AMBIENT_LIGHT = 0.4
 
-        glLightfv(GL_LIGHT0, GL_POSITION, [-0.7, -1.0, 0.7, 0.0])
-        glLightfv(GL_LIGHT0, GL_DIFFUSE, [1.0, 1.0, 1.0, 1.0])
-        glLightfv(GL_LIGHT0, GL_SPECULAR, [0.0, 0.0, 0.0, 1.0])
-        glLightModelfv(GL_LIGHT_MODEL_AMBIENT, [0.5, 0.5, 0.5, 1.0])
-
-        glColorMaterial(GL_FRONT_AND_BACK, GL_AMBIENT_AND_DIFFUSE)
-        glMaterialfv(GL_FRONT_AND_BACK, GL_SPECULAR, [1.0, 1.0, 1.0, 1.0])
-        glMaterialf(GL_FRONT_AND_BACK, GL_SHININESS, 50.0)
-
+        glLightfv(GL_LIGHT0, GL_POSITION, [-0.5, -1.0, 0.35, 0.0])
+        glLightfv(GL_LIGHT0, GL_AMBIENT, [MINECRAFT_AMBIENT_LIGHT] * 4)
+        glLightfv(GL_LIGHT0, GL_DIFFUSE, [MINECRAFT_LIGHT_POWER] * 4)
+        
         self.reload()
 
         glutDisplayFunc(self.display)
         glutReshapeFunc(self.reshape)
         glutIdleFunc(self.display)
 
         glutMainLoop()
```

### Comparing `model_resolver-0.2.0/model_resolver/utils.py` & `model_resolver-0.3.0/model_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.2.0/PKG-INFO` & `model_resolver-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-resolver
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: edayot
 Author-email: pro.e.dayot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,40 @@
 # Model Resolver
 
 A beet plugin that render all models in the beet project.
 
 
 ## Usage
 
+
+### Renders project
+
+Without any installlation, all vanilla models are rendered in this [repository](https://github.com/edayot/renders/tree/renders)
+
+### With the CLI
+
+This command will show all available options:
+
+```bash
+model_resolver --help
+```
+
+```bash
+# this will render the current resource pack models
+model_resolver 
+```
+
+```bash
+# this will render the current resource pack models and load vanilla models
+model_resolver --load-vanilla
+```
+
+
+
+### As a beet plugin
 Add the plugin to your pipeline:
 
 ```yaml
 # beet.yaml
 pipeline:
   (...)  # other plugins you may have
   - model_resolver
@@ -79,18 +105,17 @@
     x11-utils
 ```
 
 This is particularly useful in CI, see [the github action](./.github/workflows/artifact.yml) for an example.
 
 ### Common installation
 
-Using poetry, add this to your pyproject.toml file:
+Install the plugin by running:
 
-```toml
-[tool.poetry.dependencies]
-# (other dependencies ...)
-model-resolver = {git = "https://github.com/edayot/model_resolver.git", branch = "master"}
+```bash
+pip install model-resolver
 ```
 
+Pypi: https://pypi.org/project/model-resolver/
```

