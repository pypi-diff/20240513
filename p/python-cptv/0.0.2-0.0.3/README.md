# Comparing `tmp/python_cptv-0.0.2.tar.gz` & `tmp/python_cptv-0.0.3.tar.gz`

## Comparing `python_cptv-0.0.2.tar` & `python_cptv-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-rw-r--   0     2000     2000      392 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/Cargo.toml
--rw-rw-r--   0     2000     2000     2011 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_field_type.rs
--rw-rw-r--   0     2000     2000    11698 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_frame.rs
--rw-rw-r--   0     2000     2000     8587 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_header.rs
--rw-rw-r--   0     2000     2000      131 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/common/mod.rs
--rw-rw-r--   0     2000     2000     9384 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/decode/mod.rs
--rw-rw-r--   0     2000     2000       69 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/encode/mod.rs
--rw-rw-r--   0     2000     2000      113 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/lib.rs
--rw-rw-r--   0     2000     2000     3649 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/tests/decode_cptv.rs
--rw-rw-r--   0     2000     2000  2124991 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20180603-090916.cptv
--rwxrwxr-x   0     2000     2000  2975020 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20201221-748923.cptv
--rw-rw-r--   0     2000     2000   341972 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20240507-074536.cptv
--rw-r--r--   0        0        0      373 1970-01-01 00:00:00.000000 python_cptv-0.0.2/python-bindings/Cargo.toml
--rw-rw-r--   0     2000     2000      232 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/.cargo/config.toml
--rw-rw-r--   0     2000     2000      317 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/README.md
--rwxrwxr-x   0     2000     2000      155 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/build.sh
--rw-rw-r--   0     2000     2000     1321 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/examples/python-cptv-decoder.py
--rw-rw-r--   0     2000     2000        5 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/requirements.txt
--rw-rw-r--   0     2000     2000     3920 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/src/lib.rs
--rw-rw-r--   0     2000     2000    39354 2024-05-13 04:13:18.000000 python_cptv-0.0.2/Cargo.lock
--rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 python_cptv-0.0.2/Cargo.toml
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 python_cptv-0.0.2/pyproject.toml
--rw-rw-r--   0     2000     2000      317 2024-05-13 04:13:18.000000 python_cptv-0.0.2/README.md
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 python_cptv-0.0.2/PKG-INFO
+-rw-rw-r--   0     2000     2000      392 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/Cargo.toml
+-rw-rw-r--   0     2000     2000     2011 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/src/common/cptv_field_type.rs
+-rw-rw-r--   0     2000     2000    11698 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/src/common/cptv_frame.rs
+-rw-rw-r--   0     2000     2000     8587 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/src/common/cptv_header.rs
+-rw-rw-r--   0     2000     2000      131 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/src/common/mod.rs
+-rw-rw-r--   0     2000     2000     9384 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/src/decode/mod.rs
+-rw-rw-r--   0     2000     2000       69 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/src/encode/mod.rs
+-rw-rw-r--   0     2000     2000      113 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/src/lib.rs
+-rw-rw-r--   0     2000     2000     3649 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/tests/decode_cptv.rs
+-rw-rw-r--   0     2000     2000  2124991 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/tests/fixtures/20180603-090916.cptv
+-rwxrwxr-x   0     2000     2000  2975020 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/tests/fixtures/20201221-748923.cptv
+-rw-rw-r--   0     2000     2000   341972 2024-05-13 04:29:14.000000 python_cptv-0.0.3/cptv-codec-rs/tests/fixtures/20240507-074536.cptv
+-rw-r--r--   0        0        0      373 1970-01-01 00:00:00.000000 python_cptv-0.0.3/python-bindings/Cargo.toml
+-rw-rw-r--   0     2000     2000      232 2024-05-13 04:29:14.000000 python_cptv-0.0.3/python-bindings/.cargo/config.toml
+-rw-rw-r--   0     2000     2000      485 2024-05-13 04:29:14.000000 python_cptv-0.0.3/python-bindings/README.md
+-rwxrwxr-x   0     2000     2000      155 2024-05-13 04:29:14.000000 python_cptv-0.0.3/python-bindings/build.sh
+-rw-rw-r--   0     2000     2000     1321 2024-05-13 04:29:14.000000 python_cptv-0.0.3/python-bindings/examples/python-cptv-decoder.py
+-rw-rw-r--   0     2000     2000        5 2024-05-13 04:29:14.000000 python_cptv-0.0.3/python-bindings/requirements.txt
+-rw-rw-r--   0     2000     2000     3920 2024-05-13 04:29:14.000000 python_cptv-0.0.3/python-bindings/src/lib.rs
+-rw-rw-r--   0     2000     2000    39354 2024-05-13 04:29:14.000000 python_cptv-0.0.3/Cargo.lock
+-rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 python_cptv-0.0.3/Cargo.toml
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 python_cptv-0.0.3/pyproject.toml
+-rw-rw-r--   0     2000     2000      485 2024-05-13 04:29:14.000000 python_cptv-0.0.3/README.md
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 python_cptv-0.0.3/PKG-INFO
```

### Comparing `python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_field_type.rs` & `python_cptv-0.0.3/cptv-codec-rs/src/common/cptv_field_type.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_frame.rs` & `python_cptv-0.0.3/cptv-codec-rs/src/common/cptv_frame.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_header.rs` & `python_cptv-0.0.3/cptv-codec-rs/src/common/cptv_header.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/cptv-codec-rs/src/decode/mod.rs` & `python_cptv-0.0.3/cptv-codec-rs/src/decode/mod.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/cptv-codec-rs/tests/decode_cptv.rs` & `python_cptv-0.0.3/cptv-codec-rs/tests/decode_cptv.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20180603-090916.cptv` & `python_cptv-0.0.3/cptv-codec-rs/tests/fixtures/20180603-090916.cptv`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20201221-748923.cptv` & `python_cptv-0.0.3/cptv-codec-rs/tests/fixtures/20201221-748923.cptv`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20240507-074536.cptv` & `python_cptv-0.0.3/cptv-codec-rs/tests/fixtures/20240507-074536.cptv`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/python-bindings/examples/python-cptv-decoder.py` & `python_cptv-0.0.3/python-bindings/examples/python-cptv-decoder.py`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/python-bindings/src/lib.rs` & `python_cptv-0.0.3/python-bindings/src/lib.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/Cargo.lock` & `python_cptv-0.0.3/Cargo.lock`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.2/pyproject.toml` & `python_cptv-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.maturin]
 # "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
 features = ["pyo3/extension-module"]
 manifest-path = "python-bindings/Cargo.toml"
 
 [project]
 name = "python-cptv"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jon Hardie", email="Jon@cacophony.org.nz" },
   { name = "Giampaolo Feraro", email = "Giampaolo@Cacophony.org.nz"}
 ]
 description = "This is Python package provides for quick parsing Cacophony Project Thermal Video (CPTV) files. "
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `python_cptv-0.0.2/PKG-INFO` & `python_cptv-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-cptv
-Version: 0.0.2
+Version: 0.0.3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: numpy
 Summary: This is Python package provides for quick parsing Cacophony Project Thermal Video (CPTV) files. 
 Author-email: Jon Hardie <Jon@cacophony.org.nz>, Giampaolo Feraro <Giampaolo@Cacophony.org.nz>
 Requires-Python: >=3.8
@@ -14,7 +14,12 @@
 
 ## Running the example
 
 To build the module run `./build.sh`, which will put a native module called `ctpv_rs_python_bindings.so` into
 the `./examples` folder.
 Then in a python virtual environment with `numpy` installed, you can run `python python-cptv-decoder.py` from inside
 the `examples` folder.
+
+## Release to pypi
+
+Update `pyproject.toml` version identifier then create a release on github this will upload a new version to https://pypi.org/project/python-cptv
+
```

