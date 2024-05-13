# Comparing `tmp/pyproject_fmt_rust-1.0.4.tar.gz` & `tmp/pyproject_fmt_rust-1.0.5.tar.gz`

## Comparing `pyproject_fmt_rust-1.0.4.tar` & `pyproject_fmt_rust-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.4/Cargo.toml
--rw-r--r--   0     1001      127       36 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.github/FUNDING.yml
--rw-r--r--   0     1001      127      365 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.github/SECURITY.md
--rw-r--r--   0     1001      127      117 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.github/dependabot.yml
--rw-r--r--   0     1001      127       76 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.github/release.yml
--rw-r--r--   0     1001      127     2248 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.github/workflows/check.yml
--rw-r--r--   0     1001      127     3709 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.github/workflows/release.yml
--rw-r--r--   0     1001      127      158 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.gitignore
--rw-r--r--   0     1001      127      973 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      240 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127       16 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/.rustfmt.toml
--rw-r--r--   0     1001      127     3256 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1023 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/LICENSE.txt
--rw-r--r--   0     1001      127      861 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/README.md
--rw-r--r--   0     1001      127     3370 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/build_system.rs
--rw-r--r--   0     1001      127     3454 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/global.rs
--rw-r--r--   0     1001      127     8964 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/helpers/array.rs
--rw-r--r--   0     1001      127     4529 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/helpers/create.rs
--rw-r--r--   0     1001      127       78 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/helpers/mod.rs
--rw-r--r--   0     1001      127     4056 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/helpers/pep508.rs
--rw-r--r--   0     1001      127     1605 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/helpers/string.rs
--rw-r--r--   0     1001      127     9237 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/helpers/table.rs
--rw-r--r--   0     1001      127     5188 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/main.rs
--rw-r--r--   0     1001      127    30490 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust/src/project.rs
--rw-r--r--   0     1001      127       29 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/rust-toolchain.toml
--rw-r--r--   0     1001      127      161 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/src/pyproject_fmt_rust/__init__.py
--rw-r--r--   0     1001      127      638 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/src/pyproject_fmt_rust/_lib.pyi
--rw-r--r--   0     1001      127        0 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/src/pyproject_fmt_rust/py.typed
--rw-r--r--   0     1001      127      991 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/tests/test_main.py
--rw-r--r--   0     1001      127     2081 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/tox.ini
--rw-r--r--   0     1001      127    26464 2024-05-11 17:55:46.000000 pyproject_fmt_rust-1.0.4/Cargo.lock
--rw-r--r--   0     1001      127     3312 2024-05-11 17:55:34.000000 pyproject_fmt_rust-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.5/Cargo.toml
+-rw-r--r--   0     1001      127       36 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      365 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/SECURITY.md
+-rw-r--r--   0     1001      127      117 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/dependabot.yml
+-rw-r--r--   0     1001      127       76 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/release.yml
+-rw-r--r--   0     1001      127     2248 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/workflows/check.yml
+-rw-r--r--   0     1001      127     3709 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      158 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.gitignore
+-rw-r--r--   0     1001      127      973 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      240 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127       16 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.rustfmt.toml
+-rw-r--r--   0     1001      127     3256 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1023 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/LICENSE.txt
+-rw-r--r--   0     1001      127      861 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/README.md
+-rw-r--r--   0     1001      127     3370 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/build_system.rs
+-rw-r--r--   0     1001      127     3755 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/global.rs
+-rw-r--r--   0     1001      127     8964 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/array.rs
+-rw-r--r--   0     1001      127     4529 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/create.rs
+-rw-r--r--   0     1001      127       78 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/mod.rs
+-rw-r--r--   0     1001      127     4056 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/pep508.rs
+-rw-r--r--   0     1001      127     1605 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/string.rs
+-rw-r--r--   0     1001      127     9369 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/table.rs
+-rw-r--r--   0     1001      127     5748 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/main.rs
+-rw-r--r--   0     1001      127    30490 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/project.rs
+-rw-r--r--   0     1001      127       29 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust-toolchain.toml
+-rw-r--r--   0     1001      127      161 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/src/pyproject_fmt_rust/__init__.py
+-rw-r--r--   0     1001      127      638 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/src/pyproject_fmt_rust/_lib.pyi
+-rw-r--r--   0     1001      127        0 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/src/pyproject_fmt_rust/py.typed
+-rw-r--r--   0     1001      127      991 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/tests/test_main.py
+-rw-r--r--   0     1001      127     2081 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/tox.ini
+-rw-r--r--   0     1001      127    26464 2024-05-13 15:34:52.000000 pyproject_fmt_rust-1.0.5/Cargo.lock
+-rw-r--r--   0     1001      127     3312 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.5/PKG-INFO
```

### Comparing `pyproject_fmt_rust-1.0.4/Cargo.toml` & `pyproject_fmt_rust-1.0.5/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyproject-fmt-rust"
-version = "1.0.4"
+version = "1.0.5"
 description = "Format pyproject.toml files"
 repository = "https://github.com/tox-dev/pyproject-fmt"
 readme = "README.md"
 license = "MIT"
 edition = "2021"
 
 [lib]
```

### Comparing `pyproject_fmt_rust-1.0.4/.github/workflows/check.yml` & `pyproject_fmt_rust-1.0.5/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/.github/workflows/release.yml` & `pyproject_fmt_rust-1.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/.pre-commit-config.yaml` & `pyproject_fmt_rust-1.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/CODE_OF_CONDUCT.md` & `pyproject_fmt_rust-1.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/LICENSE.txt` & `pyproject_fmt_rust-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/README.md` & `pyproject_fmt_rust-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/rust/src/build_system.rs` & `pyproject_fmt_rust-1.0.5/rust/src/build_system.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/rust/src/global.rs` & `pyproject_fmt_rust-1.0.5/rust/src/global.rs`

 * *Files 8% similar despite different names*

```diff
@@ -97,14 +97,22 @@
     ek = "ev"
     [tool.undefined]
     mu="mu"
     [tool.ruff]
     mr="vr"
     [demo]
     ed = "ed"
+    [tool.coverage.report]
+    cd="de"
+    [tool.coverage]
+    aa = "bb"
+    [tool.coverage.paths]
+    ab="bc"
+    [tool.coverage.run]
+    ef="fg"
     [tool.pytest]
     mk="mv"
     "#},
         indoc ! {r#"
     # comment
     a = "b"
 
@@ -125,14 +133,23 @@
     mr = "vr"
     [tool.ruff.test]
     mrt = "vrt"
 
     [tool.pytest]
     mk = "mv"
 
+    [tool.coverage]
+    aa = "bb"
+    [tool.coverage.report]
+    cd = "de"
+    [tool.coverage.paths]
+    ab = "bc"
+    [tool.coverage.run]
+    ef = "fg"
+
     [tool.mypy]
     mk = "mv"
 
     [extra]
     ek = "ev"
 
     [tool.undefined]
```

### Comparing `pyproject_fmt_rust-1.0.4/rust/src/helpers/array.rs` & `pyproject_fmt_rust-1.0.5/rust/src/helpers/array.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/rust/src/helpers/create.rs` & `pyproject_fmt_rust-1.0.5/rust/src/helpers/create.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/rust/src/helpers/pep508.rs` & `pyproject_fmt_rust-1.0.5/rust/src/helpers/pep508.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/rust/src/helpers/string.rs` & `pyproject_fmt_rust-1.0.5/rust/src/helpers/string.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/rust/src/helpers/table.rs` & `pyproject_fmt_rust-1.0.5/rust/src/helpers/table.rs`

 * *Files 2% similar despite different names*

```diff
@@ -83,26 +83,31 @@
     let max_ordering = ordering.len() * 2;
     let key_to_pos = ordering
         .iter()
         .enumerate()
         .map(|(k, v)| (v, k * 2))
         .collect::<HashMap<&&str, usize>>();
 
-    let mut order: Vec<String> = header_to_pos.clone().into_keys().collect();
-    order.sort_by_cached_key(|k| -> usize {
+    let mut header_pos: Vec<(String, usize)> = header_to_pos.clone().into_iter().collect();
+
+    header_pos.sort_by_cached_key(|(k, file_pos)| -> (usize, usize) {
         let key = get_key(k);
         let pos = key_to_pos.get(&key.as_str());
-        if pos.is_some() {
-            let offset = usize::from(key != *k);
-            pos.unwrap() + offset
-        } else {
-            max_ordering + header_to_pos[k]
-        }
+
+        (
+            if let Some(&pos) = pos {
+                let offset = usize::from(key != *k);
+                pos + offset
+            } else {
+                max_ordering
+            },
+            *file_pos,
+        )
     });
-    order
+    header_pos.into_iter().map(|(k, _)| k).collect()
 }
 
 fn get_key(k: &str) -> String {
     let parts: Vec<&str> = k.splitn(3, '.').collect();
     if !parts.is_empty() {
         return if parts[0] == "tool" && parts.len() >= 2 {
             parts[0..2].join(".")
```

### Comparing `pyproject_fmt_rust-1.0.4/rust/src/main.rs` & `pyproject_fmt_rust-1.0.5/rust/src/main.rs`

 * *Files 7% similar despite different names*

```diff
@@ -173,14 +173,45 @@
     scripts.a = "b"
     scripts.c = "d"
     "#},
         2,
         true,
         (3, 8)
     )]
+    #[case::subsubtable(
+        indoc ! {r#"
+    [project]
+    [tool.coverage.report]
+    a = 2
+    [tool.coverage]
+    a = 0
+    [tool.coverage.paths]
+    a = 1
+    [tool.coverage.run]
+    a = 3
+    "#},
+        indoc ! {r#"
+    [project]
+    classifiers = [
+      "Programming Language :: Python :: 3 :: Only",
+      "Programming Language :: Python :: 3.8",
+    ]
+    [tool.coverage]
+    a = 0
+    [tool.coverage.report]
+    a = 2
+    [tool.coverage.paths]
+    a = 1
+    [tool.coverage.run]
+    a = 3
+    "#},
+        2,
+        true,
+        (3, 8)
+    )]
     fn test_format_toml(
         #[case] start: &str,
         #[case] expected: &str,
         #[case] indent: usize,
         #[case] keep_full_version: bool,
         #[case] max_supported_python: (u8, u8),
     ) {
```

### Comparing `pyproject_fmt_rust-1.0.4/rust/src/project.rs` & `pyproject_fmt_rust-1.0.5/rust/src/project.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/src/pyproject_fmt_rust/_lib.pyi` & `pyproject_fmt_rust-1.0.5/src/pyproject_fmt_rust/_lib.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/tests/test_main.py` & `pyproject_fmt_rust-1.0.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/tox.ini` & `pyproject_fmt_rust-1.0.5/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/Cargo.lock` & `pyproject_fmt_rust-1.0.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyproject-fmt-rust"
-version = "1.0.4"
+version = "1.0.5"
 dependencies = [
  "indoc",
  "lexical-sort",
  "pep508_rs",
  "pyo3",
  "regex",
  "rstest",
```

### Comparing `pyproject_fmt_rust-1.0.4/pyproject.toml` & `pyproject_fmt_rust-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.4/PKG-INFO` & `pyproject_fmt_rust-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt-rust
-Version: 1.0.4
+Version: 1.0.5
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

