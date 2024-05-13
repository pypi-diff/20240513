# Comparing `tmp/image_input_handler-0.1.0.tar.gz` & `tmp/image_input_handler-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_input_handler-0.1.0.tar", last modified: Sun May 12 20:16:44 2024, max compression
+gzip compressed data, was "image_input_handler-0.2.4.tar", last modified: Sun May 12 20:35:20 2024, max compression
```

## Comparing `image_input_handler-0.1.0.tar` & `image_input_handler-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:16:44.552787 image_input_handler-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:16:44.548787 image_input_handler-0.1.0/ImageInputHandler/
--rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-05-12 20:16:40.000000 image_input_handler-0.1.0/ImageInputHandler/ImageInputHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:16:40.000000 image_input_handler-0.1.0/ImageInputHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-12 20:16:44.552787 image_input_handler-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-12 20:16:40.000000 image_input_handler-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:16:44.552787 image_input_handler-0.1.0/image_input_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-12 20:16:44.000000 image_input_handler-0.1.0/image_input_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-12 20:16:44.000000 image_input_handler-0.1.0/image_input_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:16:44.000000 image_input_handler-0.1.0/image_input_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-12 20:16:44.000000 image_input_handler-0.1.0/image_input_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 20:16:44.000000 image_input_handler-0.1.0/image_input_handler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:16:44.552787 image_input_handler-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-12 20:16:40.000000 image_input_handler-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:35:20.927633 image_input_handler-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:35:20.923633 image_input_handler-0.2.4/ImageInputHandler/
+-rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-05-12 20:35:16.000000 image_input_handler-0.2.4/ImageInputHandler/ImageInputHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:35:16.000000 image_input_handler-0.2.4/ImageInputHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-12 20:35:20.927633 image_input_handler-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-12 20:35:16.000000 image_input_handler-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:35:20.927633 image_input_handler-0.2.4/image_input_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-12 20:35:20.000000 image_input_handler-0.2.4/image_input_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-12 20:35:20.000000 image_input_handler-0.2.4/image_input_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:35:20.000000 image_input_handler-0.2.4/image_input_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 20:35:20.000000 image_input_handler-0.2.4/image_input_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 20:35:20.000000 image_input_handler-0.2.4/image_input_handler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:35:20.927633 image_input_handler-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-12 20:35:16.000000 image_input_handler-0.2.4/setup.py
```

### Comparing `image_input_handler-0.1.0/ImageInputHandler/ImageInputHandler.py` & `image_input_handler-0.2.4/ImageInputHandler/ImageInputHandler.py`

 * *Files identical despite different names*

### Comparing `image_input_handler-0.1.0/PKG-INFO` & `image_input_handler-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: image_input_handler
-Version: 0.1.0
+Version: 0.2.4
 Summary: A module to handle different formats of image input
-Home-page: https://github.com/karaposu/image-input-handler
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,16 +14,14 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: urllib3
-Requires-Dist: base64
-Requires-Dist: re
 
  Image Input Handler
 
 `image-input-handler` is a versatile Python package designed to simplify the handling of various image inputs. It supports images from multiple sources including file paths, URLs, and base64 encoded strings. It adjusts image channels according to user needs and includes functionality for checking compatibility and enabling debug mode, making it an essential tool for projects involving image processing.
 
 ## Features
```

### Comparing `image_input_handler-0.1.0/README.md` & `image_input_handler-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `image_input_handler-0.1.0/image_input_handler.egg-info/PKG-INFO` & `image_input_handler-0.2.4/image_input_handler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: image_input_handler
-Version: 0.1.0
+Version: 0.2.4
 Summary: A module to handle different formats of image input
-Home-page: https://github.com/karaposu/image-input-handler
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,16 +14,14 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: urllib3
-Requires-Dist: base64
-Requires-Dist: re
 
  Image Input Handler
 
 `image-input-handler` is a versatile Python package designed to simplify the handling of various image inputs. It supports images from multiple sources including file paths, URLs, and base64 encoded strings. It adjusts image channels according to user needs and includes functionality for checking compatibility and enabling debug mode, making it an essential tool for projects involving image processing.
 
 ## Features
```

### Comparing `image_input_handler-0.1.0/setup.py` & `image_input_handler-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 
 
 
 
 
 setup(
     name='image_input_handler',  # Package name
-    version='0.1.0',  # Version of your package
+    version='0.2.4',  # Version of your package
     author='Enes Kuzucu',  # Your name
 
     description='A module to handle different formats of image input',  # Short description
     long_description=open('README.md').read(),  # Long description from a README file
     long_description_content_type='text/markdown',  # Type of the long description
-    url='https://github.com/karaposu/image-input-handler',  # URL to the repository
+#     url='https://github.com/karaposu/image-input-handler',  # URL to the repository
     packages=find_packages(),  # Automatically find packages in the directory
     install_requires=[
-        'numpy', 'opencv-python', 'Pillow', 'urllib3', 'base64', 're'  # List of dependencies
+        'numpy', 'opencv-python', 'Pillow', 'urllib3'  # List of dependencies
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',  # Development status
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',  # License as you choose
         'Programming Language :: Python :: 3',  # Supported Python versions
         'Programming Language :: Python :: 3.7',
```

