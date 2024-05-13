# Comparing `tmp/binpolar-0.5.tar.gz` & `tmp/binpolar-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binpolar-0.5.tar", last modified: Mon May 13 06:37:19 2024, max compression
+gzip compressed data, was "binpolar-0.6.tar", last modified: Mon May 13 07:32:28 2024, max compression
```

## Comparing `binpolar-0.5.tar` & `binpolar-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:37:19.920149 binpolar-0.5/
--rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 06:37:19.919954 binpolar-0.5/PKG-INFO
--rw-r--r--   0 joycelee   (501) staff       (20)        3 2024-05-13 03:33:09.000000 binpolar-0.5/README.md
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:37:19.919062 binpolar-0.5/binpolar/
--rw-r--r--   0 joycelee   (501) staff       (20)       54 2024-05-13 06:21:47.000000 binpolar-0.5/binpolar/__init__.py
--rw-r--r--   0 joycelee   (501) staff       (20)     1168 2024-05-13 06:37:09.000000 binpolar-0.5/binpolar/polarity_detector.py
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:37:19.919774 binpolar-0.5/binpolar.egg-info/
--rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/PKG-INFO
--rw-r--r--   0 joycelee   (501) staff       (20)      228 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/SOURCES.txt
--rw-r--r--   0 joycelee   (501) staff       (20)        1 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/dependency_links.txt
--rw-r--r--   0 joycelee   (501) staff       (20)       13 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/requires.txt
--rw-r--r--   0 joycelee   (501) staff       (20)        9 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/top_level.txt
--rw-r--r--   0 joycelee   (501) staff       (20)       38 2024-05-13 06:37:19.920200 binpolar-0.5/setup.cfg
--rw-r--r--   0 joycelee   (501) staff       (20)      853 2024-05-13 06:37:13.000000 binpolar-0.5/setup.py
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 07:32:28.182608 binpolar-0.6/
+-rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 07:32:28.182433 binpolar-0.6/PKG-INFO
+-rw-r--r--   0 joycelee   (501) staff       (20)        3 2024-05-13 03:33:09.000000 binpolar-0.6/README.md
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 07:32:28.181543 binpolar-0.6/binpolar/
+-rw-r--r--   0 joycelee   (501) staff       (20)       54 2024-05-13 06:21:47.000000 binpolar-0.6/binpolar/__init__.py
+-rw-r--r--   0 joycelee   (501) staff       (20)     1436 2024-05-13 07:32:06.000000 binpolar-0.6/binpolar/polarity_detector.py
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 07:32:28.182258 binpolar-0.6/binpolar.egg-info/
+-rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 07:32:28.000000 binpolar-0.6/binpolar.egg-info/PKG-INFO
+-rw-r--r--   0 joycelee   (501) staff       (20)      228 2024-05-13 07:32:28.000000 binpolar-0.6/binpolar.egg-info/SOURCES.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)        1 2024-05-13 07:32:28.000000 binpolar-0.6/binpolar.egg-info/dependency_links.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)       13 2024-05-13 07:32:28.000000 binpolar-0.6/binpolar.egg-info/requires.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)        9 2024-05-13 07:32:28.000000 binpolar-0.6/binpolar.egg-info/top_level.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)       38 2024-05-13 07:32:28.182672 binpolar-0.6/setup.cfg
+-rw-r--r--   0 joycelee   (501) staff       (20)      853 2024-05-13 07:32:16.000000 binpolar-0.6/setup.py
```

### Comparing `binpolar-0.5/PKG-INFO` & `binpolar-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binpolar
-Version: 0.5
+Version: 0.6
 Summary: Binary polarity detection
 Author: Joyce Lee
 Author-email: <leejoy1610@gmail.com>
 Keywords: python,text,polarity
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binpolar-0.5/binpolar/polarity_detector.py` & `binpolar-0.6/binpolar/polarity_detector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import re
+import os
 import tensorflow as tf
 from transformers import DistilBertTokenizer
 
-# Define global variables for the model and tokenizer
+ocean_isPos_path = os.path.abspath(os.path.join(os.path.dirname(__file__), 'ocean_isPos'))
+
+# model = tf.keras.models.load_model(os.path.join(ocean_isPos_path, 'model'))
+# tokenizer = DistilBertTokenizer.from_pretrained(os.path.join(ocean_isPos_path, 'tokenizer'))
+
 _model = None
 _tokenizer = None
 
 # Lazily loads and returns the model and tokenizer
 def get_model():
     global _model
     if _model is None:
-        _model = tf.keras.models.load_model('ocean_isPos')
+        _model = tf.keras.models.load_model(os.path.join(ocean_isPos_path, 'model'))
     return _model
 
 def get_tokenizer():
     global _tokenizer
     if _tokenizer is None:
-        _tokenizer = DistilBertTokenizer.from_pretrained('ocean_isPos/tokenizer')
+        _tokenizer = DistilBertTokenizer.from_pretrained(os.path.join(ocean_isPos_path, 'tokenizer'))
     return _tokenizer
 
 def preprocess_text(text):
     text = re.sub(r'[^\w\s]', '', text).lower()
     return text
 
 def detect_polarity(input):
```

### Comparing `binpolar-0.5/binpolar.egg-info/PKG-INFO` & `binpolar-0.6/binpolar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binpolar
-Version: 0.5
+Version: 0.6
 Summary: Binary polarity detection
 Author: Joyce Lee
 Author-email: <leejoy1610@gmail.com>
 Keywords: python,text,polarity
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binpolar-0.5/setup.py` & `binpolar-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5'
+VERSION = '0.6'
 DESCRIPTION = 'Binary polarity detection'
 LONG_DESCRIPTION = 'A fine-tuned DistilBERT model for binary polarity detection in text.'
 
 # Setting up
 setup(
     name="binpolar",
     version=VERSION,
```

