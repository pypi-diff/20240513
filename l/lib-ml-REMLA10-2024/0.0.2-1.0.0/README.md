# Comparing `tmp/lib_ml_remla10_2024-0.0.2.tar.gz` & `tmp/lib_ml_remla10_2024-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_ml_remla10_2024-0.0.2.tar", max compression
+gzip compressed data, was "lib_ml_remla10_2024-1.0.0.tar", max compression
```

## Comparing `lib_ml_remla10_2024-0.0.2.tar` & `lib_ml_remla10_2024-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1103 2024-05-11 23:26:51.561388 lib_ml_remla10_2024-0.0.2/LICENSE
--rw-r--r--   0        0        0     2023 2024-05-11 23:26:51.561388 lib_ml_remla10_2024-0.0.2/README.md
--rw-r--r--   0        0        0     1952 2024-05-11 23:27:32.177438 lib_ml_remla10_2024-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       74 2024-05-11 23:27:32.177438 lib_ml_remla10_2024-0.0.2/src/lib_ml_remla/__init__.py
--rw-r--r--   0        0        0     2955 2024-05-11 23:26:51.561388 lib_ml_remla10_2024-0.0.2/src/lib_ml_remla/preprocess.py
--rw-r--r--   0        0        0     2874 1970-01-01 00:00:00.000000 lib_ml_remla10_2024-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1103 2024-05-13 20:38:54.023238 lib_ml_remla10_2024-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2025 2024-05-13 20:38:54.023238 lib_ml_remla10_2024-1.0.0/README.md
+-rw-r--r--   0        0        0     1952 2024-05-13 20:39:32.583391 lib_ml_remla10_2024-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-05-13 20:39:32.583391 lib_ml_remla10_2024-1.0.0/src/lib_ml_remla/__init__.py
+-rw-r--r--   0        0        0     3476 2024-05-13 20:38:54.023238 lib_ml_remla10_2024-1.0.0/src/lib_ml_remla/preprocess.py
+-rw-r--r--   0        0        0     2044 2024-05-13 20:38:54.023238 lib_ml_remla10_2024-1.0.0/src/lib_ml_remla/utils.py
+-rw-r--r--   0        0        0     2876 1970-01-01 00:00:00.000000 lib_ml_remla10_2024-1.0.0/PKG-INFO
```

### Comparing `lib_ml_remla10_2024-0.0.2/LICENSE` & `lib_ml_remla10_2024-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_ml_remla10_2024-0.0.2/README.md` & `lib_ml_remla10_2024-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 [![License](https://img.shields.io/github/license/test/package_template_tester)](https://github.com/test/package_template_tester/blob/master/LICENSE)
 ![Coverage Report](assets/images/coverage.svg) -->
 
 
 </div>
 
 ## Installation
-> Python 3.9 is needed for this library!
+> Python 3.11 is needed for this library!
 
-Inside your python 3.9 virtual environment run:
+Inside your python 3.11 virtual environment run:
 
 ```bash
 poetry add lib-ml-REMLA10-2024
 ```
 
 or install with `pip`
```

### Comparing `lib_ml_remla10_2024-0.0.2/pyproject.toml` & `lib_ml_remla10_2024-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-ml-REMLA10-2024"
-version = "0.0.2"
+version = "1.0.0"
 description = "Pre-processing logic for some ML work."
 authors = ["Jan <j2000.vdm@gmail.com>", "Shayan Ramezani <s.ramezani@student.tudelft.nl>", "Remi Lejeune <R.J.Lejeune@student.tudelft.nl>", "Michael Chan <J.M.Chan@student.tudelft.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "lib_ml_remla", from = "src" }
 ]
@@ -46,15 +46,15 @@
     )?                                # pre-release section is optional
 """
 serialize = [
     "{major}.{minor}.{patch}-beta.{pre_n}",
     "{major}.{minor}.{patch}",
 ]
 regex = true
-current_version = "0.0.2"
+current_version = "1.0.0"
 ignore_missing_version = false
 tag = false
 commit = true
 message = "Bump version: {current_version} → {new_version}"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
```

### Comparing `lib_ml_remla10_2024-0.0.2/src/lib_ml_remla/preprocess.py` & `lib_ml_remla10_2024-1.0.0/src/lib_ml_remla/preprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 """
 import numpy as np
 from sklearn.preprocessing import LabelEncoder
 from keras._tf_keras.keras.preprocessing.text import Tokenizer
 from keras._tf_keras.keras.preprocessing.sequence import pad_sequences
 
 
-def split_data(train: list[str], test: list[str], val: list[str]) -> tuple[list[str], list[str], list[str], list[str], list[str], list[str]]:
+def split_data(train: list[str], test: list[str], val: list[str]) -> tuple[list[str], list[str],list[str], list[str],
+                                                                           list[str], list[str]]:
     """
     Split the data into training, validation, and test sets.
 
     Args:
         train: List of strings containing the training data.
         test: List of strings containing the test data.
         val: List of strings containing the validation data.
@@ -32,15 +33,15 @@
     return raw_X_train, raw_y_train, raw_X_val, raw_y_val, raw_X_test, raw_y_test
 
 
 def preprocess_data(raw_X_train: list[str], raw_y_train: list[str],
                     raw_X_val: list[str], raw_y_val: list[str],
                     raw_X_test: list[str], raw_y_test: list[str], sequence_length: int = 200
                     ) -> tuple[np.ndarray, np.ndarray, np.ndarray,
-                               np.ndarray, np.ndarray, np.ndarray, dict[str, int]]:
+                               np.ndarray, np.ndarray, np.ndarray, dict[str, int], Tokenizer, LabelEncoder]:
     """
     Preprocess the data for training the model.
 
     Args:
         raw_X_train: List of strings containing the training data.
         raw_y_train: List of strings containing the training labels.
         raw_X_val: List of strings containing the validation data.
@@ -63,8 +64,22 @@
     X_test = pad_sequences(tokenizer.texts_to_sequences(raw_X_test), maxlen=sequence_length)
     encoder = LabelEncoder()
 
     y_train = encoder.fit_transform(raw_y_train)
     y_val = encoder.transform(raw_y_val)
     y_test = encoder.transform(raw_y_test)
 
-    return X_train, y_train, X_val, y_val, X_test, y_test, char_index
+    return X_train, y_train, X_val, y_val, X_test, y_test, char_index, tokenizer, encoder
+
+def prepare(raw_X_test: np.ndarray, tokenizer: Tokenizer, sequence_length: int=200):
+    """
+    Preprocesses X_test given a tokenizer
+
+    Args:
+        raw_x_test: Unprocessed test data.
+        tokenizer: Tokenizer used to process the data
+
+    Returns:
+        Processed X_test
+    """
+    X_test = pad_sequences(tokenizer.texts_to_sequences(raw_X_test), maxlen=sequence_length)
+    return X_test
```

### Comparing `lib_ml_remla10_2024-0.0.2/PKG-INFO` & `lib_ml_remla10_2024-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-ml-REMLA10-2024
-Version: 0.0.2
+Version: 1.0.0
 Summary: Pre-processing logic for some ML work.
 License: MIT
 Author: Jan
 Author-email: j2000.vdm@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,17 +33,17 @@
 [![License](https://img.shields.io/github/license/test/package_template_tester)](https://github.com/test/package_template_tester/blob/master/LICENSE)
 ![Coverage Report](assets/images/coverage.svg) -->
 
 
 </div>
 
 ## Installation
-> Python 3.9 is needed for this library!
+> Python 3.11 is needed for this library!
 
-Inside your python 3.9 virtual environment run:
+Inside your python 3.11 virtual environment run:
 
 ```bash
 poetry add lib-ml-REMLA10-2024
 ```
 
 or install with `pip`
```

