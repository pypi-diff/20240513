# Comparing `tmp/binpolar-0.3.tar.gz` & `tmp/binpolar-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binpolar-0.3.tar", last modified: Mon May 13 06:30:13 2024, max compression
+gzip compressed data, was "binpolar-0.5.tar", last modified: Mon May 13 06:37:19 2024, max compression
```

## Comparing `binpolar-0.3.tar` & `binpolar-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:30:13.367291 binpolar-0.3/
--rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 06:30:13.367093 binpolar-0.3/PKG-INFO
--rw-r--r--   0 joycelee   (501) staff       (20)        3 2024-05-13 03:33:09.000000 binpolar-0.3/README.md
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:30:13.366094 binpolar-0.3/binpolar/
--rw-r--r--   0 joycelee   (501) staff       (20)       54 2024-05-13 06:21:47.000000 binpolar-0.3/binpolar/__init__.py
--rw-r--r--   0 joycelee   (501) staff       (20)     1178 2024-05-13 06:26:35.000000 binpolar-0.3/binpolar/polarity_detector.py
-drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:30:13.366891 binpolar-0.3/binpolar.egg-info/
--rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/PKG-INFO
--rw-r--r--   0 joycelee   (501) staff       (20)      228 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/SOURCES.txt
--rw-r--r--   0 joycelee   (501) staff       (20)        1 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/dependency_links.txt
--rw-r--r--   0 joycelee   (501) staff       (20)       13 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/requires.txt
--rw-r--r--   0 joycelee   (501) staff       (20)        9 2024-05-13 06:30:13.000000 binpolar-0.3/binpolar.egg-info/top_level.txt
--rw-r--r--   0 joycelee   (501) staff       (20)       38 2024-05-13 06:30:13.367343 binpolar-0.3/setup.cfg
--rw-r--r--   0 joycelee   (501) staff       (20)      853 2024-05-13 06:30:00.000000 binpolar-0.3/setup.py
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:37:19.920149 binpolar-0.5/
+-rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 06:37:19.919954 binpolar-0.5/PKG-INFO
+-rw-r--r--   0 joycelee   (501) staff       (20)        3 2024-05-13 03:33:09.000000 binpolar-0.5/README.md
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:37:19.919062 binpolar-0.5/binpolar/
+-rw-r--r--   0 joycelee   (501) staff       (20)       54 2024-05-13 06:21:47.000000 binpolar-0.5/binpolar/__init__.py
+-rw-r--r--   0 joycelee   (501) staff       (20)     1168 2024-05-13 06:37:09.000000 binpolar-0.5/binpolar/polarity_detector.py
+drwxr-xr-x   0 joycelee   (501) staff       (20)        0 2024-05-13 06:37:19.919774 binpolar-0.5/binpolar.egg-info/
+-rw-r--r--   0 joycelee   (501) staff       (20)      587 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/PKG-INFO
+-rw-r--r--   0 joycelee   (501) staff       (20)      228 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/SOURCES.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)        1 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/dependency_links.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)       13 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/requires.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)        9 2024-05-13 06:37:19.000000 binpolar-0.5/binpolar.egg-info/top_level.txt
+-rw-r--r--   0 joycelee   (501) staff       (20)       38 2024-05-13 06:37:19.920200 binpolar-0.5/setup.cfg
+-rw-r--r--   0 joycelee   (501) staff       (20)      853 2024-05-13 06:37:13.000000 binpolar-0.5/setup.py
```

### Comparing `binpolar-0.3/PKG-INFO` & `binpolar-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binpolar
-Version: 0.3
+Version: 0.5
 Summary: Binary polarity detection
 Author: Joyce Lee
 Author-email: <leejoy1610@gmail.com>
 Keywords: python,text,polarity
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binpolar-0.3/binpolar/polarity_detector.py` & `binpolar-0.5/binpolar/polarity_detector.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 _model = None
 _tokenizer = None
 
 # Lazily loads and returns the model and tokenizer
 def get_model():
     global _model
     if _model is None:
-        _model = tf.keras.models.load_model('distilbert_ocean')
+        _model = tf.keras.models.load_model('ocean_isPos')
     return _model
 
 def get_tokenizer():
     global _tokenizer
     if _tokenizer is None:
-        _tokenizer = DistilBertTokenizer.from_pretrained('distilbert_ocean/tokenizer')
+        _tokenizer = DistilBertTokenizer.from_pretrained('ocean_isPos/tokenizer')
     return _tokenizer
 
 def preprocess_text(text):
     text = re.sub(r'[^\w\s]', '', text).lower()
     return text
 
 def detect_polarity(input):
```

### Comparing `binpolar-0.3/binpolar.egg-info/PKG-INFO` & `binpolar-0.5/binpolar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binpolar
-Version: 0.3
+Version: 0.5
 Summary: Binary polarity detection
 Author: Joyce Lee
 Author-email: <leejoy1610@gmail.com>
 Keywords: python,text,polarity
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binpolar-0.3/setup.py` & `binpolar-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3'
+VERSION = '0.5'
 DESCRIPTION = 'Binary polarity detection'
 LONG_DESCRIPTION = 'A fine-tuned DistilBERT model for binary polarity detection in text.'
 
 # Setting up
 setup(
     name="binpolar",
     version=VERSION,
```

