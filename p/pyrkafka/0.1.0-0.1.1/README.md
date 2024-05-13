# Comparing `tmp/pyrkafka-0.1.0.tar.gz` & `tmp/pyrkafka-0.1.1.tar.gz`

## Comparing `pyrkafka-0.1.0.tar` & `pyrkafka-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 pyrkafka-0.1.0/Cargo.toml
--rw-r--r--   0      501       20      701 2024-05-12 13:40:31.000000 pyrkafka-0.1.0/.gitignore
--rw-r--r--   0      501       20     1231 2024-05-12 13:37:21.000000 pyrkafka-0.1.0/README.md
--rw-r--r--   0      501       20     3059 2024-05-08 13:43:29.000000 pyrkafka-0.1.0/src/consumer.rs
--rw-r--r--   0      501       20      295 2024-05-08 17:55:26.000000 pyrkafka-0.1.0/src/lib.rs
--rw-r--r--   0      501       20     1635 2024-05-08 13:21:51.000000 pyrkafka-0.1.0/src/producer.rs
--rw-r--r--   0      501       20    16668 2024-05-12 11:52:35.000000 pyrkafka-0.1.0/Cargo.lock
--rw-r--r--   0      501       20      869 2024-05-12 13:38:38.000000 pyrkafka-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 pyrkafka-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 pyrkafka-0.1.1/Cargo.toml
+-rw-r--r--   0      501       20      701 2024-05-12 13:40:31.000000 pyrkafka-0.1.1/.gitignore
+-rw-r--r--   0      501       20     1232 2024-05-13 12:03:36.000000 pyrkafka-0.1.1/README.md
+-rw-r--r--   0      501       20     3059 2024-05-08 13:43:29.000000 pyrkafka-0.1.1/src/consumer.rs
+-rw-r--r--   0      501       20      295 2024-05-08 17:55:26.000000 pyrkafka-0.1.1/src/lib.rs
+-rw-r--r--   0      501       20     1635 2024-05-08 13:21:51.000000 pyrkafka-0.1.1/src/producer.rs
+-rw-r--r--   0      501       20    16668 2024-05-12 11:52:35.000000 pyrkafka-0.1.1/Cargo.lock
+-rw-r--r--   0      501       20      869 2024-05-13 12:01:17.000000 pyrkafka-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 pyrkafka-0.1.1/PKG-INFO
```

### Comparing `pyrkafka-0.1.0/.gitignore` & `pyrkafka-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrkafka-0.1.0/README.md` & `pyrkafka-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# rdfkafka
+# pyrkakfa
 
-[![PyPI version](https://badge.fury.io/py/rdfkafka.svg)](https://badge.fury.io/py/rdfkafka)
+[![PyPI version](https://badge.fury.io/py/pyrkafka.svg)](https://pypi.org/project/pyrkafka/)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 ## Description
 
 `rdfkafka` is a Rust library for working with Kafka in Python. It provides a high-level interface for producing and consuming RDF data using the Kafka messaging system.
 
 ## Features
```

### Comparing `pyrkafka-0.1.0/src/consumer.rs` & `pyrkafka-0.1.1/src/consumer.rs`

 * *Files identical despite different names*

### Comparing `pyrkafka-0.1.0/src/producer.rs` & `pyrkafka-0.1.1/src/producer.rs`

 * *Files identical despite different names*

### Comparing `pyrkafka-0.1.0/Cargo.lock` & `pyrkafka-0.1.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pyrkafka-0.1.0/pyproject.toml` & `pyrkafka-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.2,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "pyrkafka"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python bindings for rdfkafka Rust library"
 authors = [{ name = "Michael Rademaker", email = "michael@appbriek.com" }]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT License"}
 classifiers = [
     "Programming Language :: Rust",
```

### Comparing `pyrkafka-0.1.0/PKG-INFO` & `pyrkafka-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.3
 Name: pyrkafka
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python bindings for rdfkafka Rust library
 Author-email: Michael Rademaker <michael@appbriek.com>
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/Miggets7/pyrkafka
 Project-URL: Documentation, https://github.com/Miggets7/pyrkafka
 Project-URL: Repository, https://github.com/Miggets7/pyrkafka
 Project-URL: Issues, https://github.com/Miggets7/pyrkafka/issues
 Project-URL: Changelog, https://github.com/Miggets7/pyrkafka
 
-# rdfkafka
+# pyrkakfa
 
-[![PyPI version](https://badge.fury.io/py/rdfkafka.svg)](https://badge.fury.io/py/rdfkafka)
+[![PyPI version](https://badge.fury.io/py/pyrkafka.svg)](https://pypi.org/project/pyrkafka/)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 ## Description
 
 `rdfkafka` is a Rust library for working with Kafka in Python. It provides a high-level interface for producing and consuming RDF data using the Kafka messaging system.
 
 ## Features
```

