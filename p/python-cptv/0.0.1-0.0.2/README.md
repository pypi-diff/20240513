# Comparing `tmp/python_cptv-0.0.1.tar.gz` & `tmp/python_cptv-0.0.2.tar.gz`

## Comparing `python_cptv-0.0.1.tar` & `python_cptv-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-rw-r--   0     1000     1000      392 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/Cargo.toml
--rw-rw-r--   0     1000     1000     2011 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/src/common/cptv_field_type.rs
--rw-rw-r--   0     1000     1000    11698 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/src/common/cptv_frame.rs
--rw-rw-r--   0     1000     1000     8587 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/src/common/cptv_header.rs
--rw-rw-r--   0     1000     1000      131 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/src/common/mod.rs
--rw-rw-r--   0     1000     1000     9384 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/src/decode/mod.rs
--rw-rw-r--   0     1000     1000       69 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/src/encode/mod.rs
--rw-rw-r--   0     1000     1000      113 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/src/lib.rs
--rw-rw-r--   0     1000     1000     3649 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/tests/decode_cptv.rs
--rw-rw-r--   0     1000     1000  2124991 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/tests/fixtures/20180603-090916.cptv
--rwxrwxr-x   0     1000     1000  2975020 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/tests/fixtures/20201221-748923.cptv
--rw-rw-r--   0     1000     1000   341972 2024-05-13 01:19:44.000000 python_cptv-0.0.1/cptv-codec-rs/tests/fixtures/20240507-074536.cptv
--rw-r--r--   0        0        0      373 1970-01-01 00:00:00.000000 python_cptv-0.0.1/python-bindings/Cargo.toml
--rw-rw-r--   0     1000     1000      232 2024-05-13 01:19:44.000000 python_cptv-0.0.1/python-bindings/.cargo/config.toml
--rw-rw-r--   0     1000     1000      317 2024-05-13 01:19:44.000000 python_cptv-0.0.1/python-bindings/README.md
--rwxrwxr-x   0     1000     1000      155 2024-05-13 01:59:45.000000 python_cptv-0.0.1/python-bindings/build.sh
--rw-rw-r--   0     1000     1000     1321 2024-05-13 01:38:50.000000 python_cptv-0.0.1/python-bindings/examples/python-cptv-decoder.py
--rw-rw-r--   0     1000     1000        5 2024-05-13 01:41:33.000000 python_cptv-0.0.1/python-bindings/requirements.txt
--rw-rw-r--   0     1000     1000     3896 2024-05-13 01:19:44.000000 python_cptv-0.0.1/python-bindings/src/lib.rs
--rw-rw-r--   0     1000     1000    39354 2024-05-13 01:19:44.000000 python_cptv-0.0.1/Cargo.lock
--rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 python_cptv-0.0.1/Cargo.toml
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 python_cptv-0.0.1/pyproject.toml
--rw-rw-r--   0     1000     1000      317 2024-05-13 01:19:44.000000 python_cptv-0.0.1/README.md
--rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 python_cptv-0.0.1/PKG-INFO
+-rw-rw-r--   0     2000     2000      392 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/Cargo.toml
+-rw-rw-r--   0     2000     2000     2011 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_field_type.rs
+-rw-rw-r--   0     2000     2000    11698 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_frame.rs
+-rw-rw-r--   0     2000     2000     8587 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_header.rs
+-rw-rw-r--   0     2000     2000      131 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/common/mod.rs
+-rw-rw-r--   0     2000     2000     9384 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/decode/mod.rs
+-rw-rw-r--   0     2000     2000       69 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/encode/mod.rs
+-rw-rw-r--   0     2000     2000      113 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/src/lib.rs
+-rw-rw-r--   0     2000     2000     3649 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/tests/decode_cptv.rs
+-rw-rw-r--   0     2000     2000  2124991 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20180603-090916.cptv
+-rwxrwxr-x   0     2000     2000  2975020 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20201221-748923.cptv
+-rw-rw-r--   0     2000     2000   341972 2024-05-13 04:13:18.000000 python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20240507-074536.cptv
+-rw-r--r--   0        0        0      373 1970-01-01 00:00:00.000000 python_cptv-0.0.2/python-bindings/Cargo.toml
+-rw-rw-r--   0     2000     2000      232 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/.cargo/config.toml
+-rw-rw-r--   0     2000     2000      317 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/README.md
+-rwxrwxr-x   0     2000     2000      155 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/build.sh
+-rw-rw-r--   0     2000     2000     1321 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/examples/python-cptv-decoder.py
+-rw-rw-r--   0     2000     2000        5 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/requirements.txt
+-rw-rw-r--   0     2000     2000     3920 2024-05-13 04:13:18.000000 python_cptv-0.0.2/python-bindings/src/lib.rs
+-rw-rw-r--   0     2000     2000    39354 2024-05-13 04:13:18.000000 python_cptv-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 python_cptv-0.0.2/Cargo.toml
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 python_cptv-0.0.2/pyproject.toml
+-rw-rw-r--   0     2000     2000      317 2024-05-13 04:13:18.000000 python_cptv-0.0.2/README.md
+-rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 python_cptv-0.0.2/PKG-INFO
```

### Comparing `python_cptv-0.0.1/cptv-codec-rs/src/common/cptv_field_type.rs` & `python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_field_type.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/cptv-codec-rs/src/common/cptv_frame.rs` & `python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_frame.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/cptv-codec-rs/src/common/cptv_header.rs` & `python_cptv-0.0.2/cptv-codec-rs/src/common/cptv_header.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/cptv-codec-rs/src/decode/mod.rs` & `python_cptv-0.0.2/cptv-codec-rs/src/decode/mod.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/cptv-codec-rs/tests/decode_cptv.rs` & `python_cptv-0.0.2/cptv-codec-rs/tests/decode_cptv.rs`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/cptv-codec-rs/tests/fixtures/20180603-090916.cptv` & `python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20180603-090916.cptv`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/cptv-codec-rs/tests/fixtures/20201221-748923.cptv` & `python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20201221-748923.cptv`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/cptv-codec-rs/tests/fixtures/20240507-074536.cptv` & `python_cptv-0.0.2/cptv-codec-rs/tests/fixtures/20240507-074536.cptv`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/python-bindings/examples/python-cptv-decoder.py` & `python_cptv-0.0.2/python-bindings/examples/python-cptv-decoder.py`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/python-bindings/src/lib.rs` & `python_cptv-0.0.2/python-bindings/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -115,21 +115,21 @@
             None
         }
     }
 
     pub fn next_frame<'py>(&mut self, py: Python<'py>) -> Option<CptvFrame> {
         if let Ok(frame_ref) = self.inner.next_frame() {
             let chunk =
-                Array::from_shape_vec((160, 120), frame_ref.image_data.data().to_vec()).unwrap();
+                Array::from_shape_vec((120, 160), frame_ref.image_data.data().to_vec()).unwrap();
             Some(CptvFrame {
                 time_on: frame_ref.time_on,
                 last_ffc_time: frame_ref.last_ffc_time,
                 temp_c: frame_ref.frame_temp_c,
                 last_ffc_temp_c: frame_ref.last_ffc_temp_c,
-                background_frame: false,
+                background_frame: frame_ref.is_background_frame,
                 pix: Bound::unbind(chunk.into_pyarray_bound(py)),
             })
         } else {
             None
         }
     }
 }
```

### Comparing `python_cptv-0.0.1/Cargo.lock` & `python_cptv-0.0.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `python_cptv-0.0.1/pyproject.toml` & `python_cptv-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 [tool.maturin]
 # "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
 features = ["pyo3/extension-module"]
 manifest-path = "python-bindings/Cargo.toml"
 
 [project]
 name = "python-cptv"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jon Hardie", email="Jon@cacophony.org.nz" },
   { name = "Giampaolo Feraro", email = "Giampaolo@Cacophony.org.nz"}
 ]
 description = "This is Python package provides for quick parsing Cacophony Project Thermal Video (CPTV) files. "
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "numpy"
+]
```

### Comparing `python_cptv-0.0.1/PKG-INFO` & `python_cptv-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.3
 Name: python-cptv
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Dist: numpy
 Summary: This is Python package provides for quick parsing Cacophony Project Thermal Video (CPTV) files. 
 Author-email: Jon Hardie <Jon@cacophony.org.nz>, Giampaolo Feraro <Giampaolo@Cacophony.org.nz>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Python bindings
```

