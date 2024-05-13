# Comparing `tmp/pyproject_fmt_rust-1.0.5.tar.gz` & `tmp/pyproject_fmt_rust-1.0.6.tar.gz`

## Comparing `pyproject_fmt_rust-1.0.5.tar` & `pyproject_fmt_rust-1.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.5/Cargo.toml
--rw-r--r--   0     1001      127       36 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/FUNDING.yml
--rw-r--r--   0     1001      127      365 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/SECURITY.md
--rw-r--r--   0     1001      127      117 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/dependabot.yml
--rw-r--r--   0     1001      127       76 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/release.yml
--rw-r--r--   0     1001      127     2248 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/workflows/check.yml
--rw-r--r--   0     1001      127     3709 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.github/workflows/release.yml
--rw-r--r--   0     1001      127      158 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.gitignore
--rw-r--r--   0     1001      127      973 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      240 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127       16 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/.rustfmt.toml
--rw-r--r--   0     1001      127     3256 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1023 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/LICENSE.txt
--rw-r--r--   0     1001      127      861 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/README.md
--rw-r--r--   0     1001      127     3370 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/build_system.rs
--rw-r--r--   0     1001      127     3755 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/global.rs
--rw-r--r--   0     1001      127     8964 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/array.rs
--rw-r--r--   0     1001      127     4529 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/create.rs
--rw-r--r--   0     1001      127       78 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/mod.rs
--rw-r--r--   0     1001      127     4056 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/pep508.rs
--rw-r--r--   0     1001      127     1605 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/string.rs
--rw-r--r--   0     1001      127     9369 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/helpers/table.rs
--rw-r--r--   0     1001      127     5748 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/main.rs
--rw-r--r--   0     1001      127    30490 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust/src/project.rs
--rw-r--r--   0     1001      127       29 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/rust-toolchain.toml
--rw-r--r--   0     1001      127      161 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/src/pyproject_fmt_rust/__init__.py
--rw-r--r--   0     1001      127      638 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/src/pyproject_fmt_rust/_lib.pyi
--rw-r--r--   0     1001      127        0 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/src/pyproject_fmt_rust/py.typed
--rw-r--r--   0     1001      127      991 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/tests/test_main.py
--rw-r--r--   0     1001      127     2081 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/tox.ini
--rw-r--r--   0     1001      127    26464 2024-05-13 15:34:52.000000 pyproject_fmt_rust-1.0.5/Cargo.lock
--rw-r--r--   0     1001      127     3312 2024-05-13 15:34:38.000000 pyproject_fmt_rust-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.6/Cargo.toml
+-rw-r--r--   0     1001      127       36 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      365 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/SECURITY.md
+-rw-r--r--   0     1001      127      117 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/dependabot.yml
+-rw-r--r--   0     1001      127       76 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/release.yml
+-rw-r--r--   0     1001      127     2248 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/workflows/check.yml
+-rw-r--r--   0     1001      127     3714 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      158 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.gitignore
+-rw-r--r--   0     1001      127      973 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      240 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127       16 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/.rustfmt.toml
+-rw-r--r--   0     1001      127     3256 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1023 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/LICENSE.txt
+-rw-r--r--   0     1001      127      861 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/README.md
+-rw-r--r--   0     1001      127     3370 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/build_system.rs
+-rw-r--r--   0     1001      127     3755 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/global.rs
+-rw-r--r--   0     1001      127     8964 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/array.rs
+-rw-r--r--   0     1001      127     4529 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/create.rs
+-rw-r--r--   0     1001      127       78 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/mod.rs
+-rw-r--r--   0     1001      127     4595 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/pep508.rs
+-rw-r--r--   0     1001      127     1605 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/string.rs
+-rw-r--r--   0     1001      127     9369 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/helpers/table.rs
+-rw-r--r--   0     1001      127     5748 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/main.rs
+-rw-r--r--   0     1001      127    30490 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust/src/project.rs
+-rw-r--r--   0     1001      127       29 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/rust-toolchain.toml
+-rw-r--r--   0     1001      127      161 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/src/pyproject_fmt_rust/__init__.py
+-rw-r--r--   0     1001      127      638 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/src/pyproject_fmt_rust/_lib.pyi
+-rw-r--r--   0     1001      127        0 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/src/pyproject_fmt_rust/py.typed
+-rw-r--r--   0     1001      127      991 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/tests/test_main.py
+-rw-r--r--   0     1001      127     2081 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/tox.ini
+-rw-r--r--   0     1001      127    26478 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/Cargo.lock
+-rw-r--r--   0     1001      127     3312 2024-05-13 16:34:10.000000 pyproject_fmt_rust-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.6/PKG-INFO
```

### Comparing `pyproject_fmt_rust-1.0.5/Cargo.toml` & `pyproject_fmt_rust-1.0.6/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [package]
 name = "pyproject-fmt-rust"
-version = "1.0.5"
+version = "1.0.6"
 description = "Format pyproject.toml files"
 repository = "https://github.com/tox-dev/pyproject-fmt"
 readme = "README.md"
 license = "MIT"
 edition = "2021"
 
 [lib]
 name = "_lib"
 path = "rust/src/main.rs"
 crate-type = ["cdylib"]
 
 [dependencies]
 taplo = { version = "0.13.0" }                          # formatter
 pyo3 = { version = "0.21.2", features = ["abi3-py38"] } # integration with Python
-pep508_rs = { version = "0.5.0" }
+pep440_rs = { version = "0.6.0" }
+pep508_rs = { version = "0.6.0" }
 lexical-sort = { version = "0.3.1" }
 regex = { version = "1.10.4" }
 
 [features]
 extension-module = ["pyo3/extension-module"]
 default = ["extension-module"]
```

### Comparing `pyproject_fmt_rust-1.0.5/.github/workflows/check.yml` & `pyproject_fmt_rust-1.0.6/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/.github/workflows/release.yml` & `pyproject_fmt_rust-1.0.6/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     environment:
       name: release
-      url: https://pypi.org/p/pyproject-fmt
+      url: https://pypi.org/p/pyproject-fmt/rust
     permissions:
       id-token: write
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [ linux, windows, macos, sdist ]
     steps:
       - uses: actions/download-artifact@v4
       - name: Publish to PyPI
```

### Comparing `pyproject_fmt_rust-1.0.5/.pre-commit-config.yaml` & `pyproject_fmt_rust-1.0.6/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         args: [ "--write-changes" ]
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: "1.3.1"
     hooks:
       - id: tox-ini-fmt
         args: [ "-p", "fix" ]
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: "2.0.1"
+    rev: "2.0.3"
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/astral-sh/ruff-pre-commit
     rev: "v0.4.4"
     hooks:
       - id: ruff-format
       - id: ruff
```

### Comparing `pyproject_fmt_rust-1.0.5/CODE_OF_CONDUCT.md` & `pyproject_fmt_rust-1.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/LICENSE.txt` & `pyproject_fmt_rust-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/README.md` & `pyproject_fmt_rust-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/rust/src/build_system.rs` & `pyproject_fmt_rust-1.0.6/rust/src/build_system.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/rust/src/global.rs` & `pyproject_fmt_rust-1.0.6/rust/src/global.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/rust/src/helpers/array.rs` & `pyproject_fmt_rust-1.0.6/rust/src/helpers/array.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/rust/src/helpers/create.rs` & `pyproject_fmt_rust-1.0.6/rust/src/helpers/create.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/rust/src/helpers/pep508.rs` & `pyproject_fmt_rust-1.0.6/rust/src/helpers/pep508.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use std::fmt::Write;
 use std::str::FromStr;
 
+use pep440_rs::Operator;
 use pep508_rs::{MarkerTree, Requirement, VersionOrUrl};
 
 pub fn format_requirement(value: &str, keep_full_version: bool) -> String {
     let req = Requirement::from_str(value).unwrap();
     let mut result = req.name.to_string();
     if !req.extras.is_empty() {
         write!(&mut result, "[").unwrap();
@@ -19,15 +20,15 @@
     }
     if let Some(version_or_url) = req.version_or_url {
         match version_or_url {
             VersionOrUrl::VersionSpecifier(v) => {
                 let extra_count = v.len() - 1;
                 for (at, spec) in v.iter().enumerate() {
                     let mut spec_repr = format!("{spec}");
-                    if !keep_full_version {
+                    if !keep_full_version && spec.operator() != &Operator::TildeEqual {
                         loop {
                             let propose = spec_repr.strip_suffix(".0");
                             if propose.is_none() {
                                 break;
                             }
                             spec_repr = propose.unwrap().to_string();
                         }
@@ -35,15 +36,15 @@
                     write!(&mut result, "{spec_repr}").unwrap();
                     if extra_count != at {
                         write!(&mut result, ",").unwrap();
                     }
                 }
             }
             VersionOrUrl::Url(u) => {
-                write!(&mut result, "{u}").unwrap();
+                write!(&mut result, " @ {u}").unwrap();
             }
         }
     }
     if let Some(marker) = req.marker {
         write!(&mut result, "; ").unwrap();
         handle_marker(&marker, &mut result, false);
     }
@@ -105,11 +106,20 @@
         false
     )]
     #[case::keep_version(
     r#"requests [security , tests] >= 2.0.0, == 2.8.* ; (os_name=="a" or os_name=='b') and os_name=='c' and python_version > "3.8""#,
     "requests[security,tests]>=2.0.0,==2.8.*; (os_name=='a' or os_name=='b') and os_name=='c' and python_version>'3.8'",
     true
     )]
+    #[case::do_not_strip_tilda("a~=3.0.0", "a~=3.0.0", false)]
+    #[case::url(
+        " pip   @   https://github.com/pypa/pip/archive/1.3.1.zip#sha1=da9234ee9982d4bbb3c72346a6de940a148ea686 ",
+        "pip @ https://github.com/pypa/pip/archive/1.3.1.zip#sha1=da9234ee9982d4bbb3c72346a6de940a148ea686",
+        true
+    )]
     fn test_format_requirement(#[case] start: &str, #[case] expected: &str, #[case] keep_full_version: bool) {
-        assert_eq!(format_requirement(start, keep_full_version), expected);
+        let got = format_requirement(start, keep_full_version);
+        assert_eq!(got, expected);
+        // formatting remains stable
+        assert_eq!(format_requirement(got.as_str(), keep_full_version), expected);
     }
 }
```

### Comparing `pyproject_fmt_rust-1.0.5/rust/src/helpers/string.rs` & `pyproject_fmt_rust-1.0.6/rust/src/helpers/string.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/rust/src/helpers/table.rs` & `pyproject_fmt_rust-1.0.6/rust/src/helpers/table.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/rust/src/main.rs` & `pyproject_fmt_rust-1.0.6/rust/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/rust/src/project.rs` & `pyproject_fmt_rust-1.0.6/rust/src/project.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/src/pyproject_fmt_rust/_lib.pyi` & `pyproject_fmt_rust-1.0.6/src/pyproject_fmt_rust/_lib.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/tests/test_main.py` & `pyproject_fmt_rust-1.0.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/tox.ini` & `pyproject_fmt_rust-1.0.6/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/Cargo.lock` & `pyproject_fmt_rust-1.0.6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -398,17 +398,17 @@
  "once_cell",
  "unicode-width",
  "unscanny",
 ]
 
 [[package]]
 name = "pep508_rs"
-version = "0.5.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa3d4bcbc98074b50cdfd37e7ca597aec4d816252af135a7e3ad2e67d1ad6f66"
+checksum = "581c27e97a3f38c5d691962af7da93c2672b5227d59cf165b87a9b1fd53dd724"
 dependencies = [
  "derivative",
  "once_cell",
  "pep440_rs",
  "regex",
  "thiserror",
  "unicode-width",
@@ -516,18 +516,19 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyproject-fmt-rust"
-version = "1.0.5"
+version = "1.0.6"
 dependencies = [
  "indoc",
  "lexical-sort",
+ "pep440_rs",
  "pep508_rs",
  "pyo3",
  "regex",
  "rstest",
  "taplo",
 ]
```

### Comparing `pyproject_fmt_rust-1.0.5/pyproject.toml` & `pyproject_fmt_rust-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.5/PKG-INFO` & `pyproject_fmt_rust-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt-rust
-Version: 1.0.5
+Version: 1.0.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

