# Comparing `tmp/stack_graphs_python_bindings-0.0.6.tar.gz` & `tmp/stack_graphs_python_bindings-0.0.7.tar.gz`

## Comparing `stack_graphs_python_bindings-0.0.6.tar` & `stack_graphs_python_bindings-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.6/Cargo.toml
--rw-r--r--   0     1001      127      840 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/.github/workflows/ci.yaml
--rw-r--r--   0     1001      127     4176 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/.github/workflows/release.yaml
--rw-r--r--   0     1001      127      739 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/.gitignore
--rw-r--r--   0     1001      127     1077 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/LICENSE
--rw-r--r--   0     1001      127     1664 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/Makefile
--rw-r--r--   0     1001      127      909 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/README.md
--rw-r--r--   0     1001      127     2101 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/src/classes.rs
--rw-r--r--   0     1001      127     1159 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/src/lib.rs
--rw-r--r--   0     1001      127     3547 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/src/stack_graphs_wrapper/mod.rs
--rw-r--r--   0     1001      127      456 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/stack_graphs_python.pyi
--rw-r--r--   0     1001      127       66 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/tests/js_sample/index.js
--rw-r--r--   0     1001      127       25 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/tests/js_sample/module.js
--rw-r--r--   0     1001      127      934 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/tests/test.py
--rw-r--r--   0     1001      127    50375 2024-05-13 14:40:34.000000 stack_graphs_python_bindings-0.0.6/Cargo.lock
--rw-r--r--   0     1001      127      405 2024-05-13 14:40:29.000000 stack_graphs_python_bindings-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.7/Cargo.toml
+-rw-r--r--   0     1001      127      840 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/.github/workflows/ci.yaml
+-rw-r--r--   0     1001      127     4111 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/.github/workflows/release.yaml
+-rw-r--r--   0     1001      127      739 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/.gitignore
+-rw-r--r--   0     1001      127     1077 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/LICENSE
+-rw-r--r--   0     1001      127     1708 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/Makefile
+-rw-r--r--   0     1001      127      909 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/README.md
+-rw-r--r--   0     1001      127     2101 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/src/classes.rs
+-rw-r--r--   0     1001      127     1159 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/src/lib.rs
+-rw-r--r--   0     1001      127     3547 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/src/stack_graphs_wrapper/mod.rs
+-rw-r--r--   0     1001      127      456 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/stack_graphs_python.pyi
+-rw-r--r--   0     1001      127       66 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/tests/js_sample/index.js
+-rw-r--r--   0     1001      127       25 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/tests/js_sample/module.js
+-rw-r--r--   0     1001      127      934 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/tests/test.py
+-rw-r--r--   0     1001      127    50375 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/Cargo.lock
+-rw-r--r--   0     1001      127      405 2024-05-13 14:51:49.000000 stack_graphs_python_bindings-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.7/PKG-INFO
```

### Comparing `stack_graphs_python_bindings-0.0.6/Cargo.toml` & `stack_graphs_python_bindings-0.0.7/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "stack-graphs-python-bindings"
-version = "0.0.6"
+version = "0.0.7"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "stack_graphs_python"
 crate-type = ["cdylib"]
```

### Comparing `stack_graphs_python_bindings-0.0.6/.github/workflows/ci.yaml` & `stack_graphs_python_bindings-0.0.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.6/.github/workflows/release.yaml` & `stack_graphs_python_bindings-0.0.7/.github/workflows/release.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -139,14 +139,12 @@
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
           args: --non-interactive --skip-existing wheels-*/*
       - name: Create GitHub Release
-        uses: softprops/action-gh-release@v1
+        uses: softprops/action-gh-release@v2
         if: success()
         with:
           files: |
             wheels-*/*
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `stack_graphs_python_bindings-0.0.6/.gitignore` & `stack_graphs_python_bindings-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.6/LICENSE` & `stack_graphs_python_bindings-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.6/Makefile` & `stack_graphs_python_bindings-0.0.7/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -42,10 +42,11 @@
 		exit 1; \
 	fi
 	$(eval LATEST_TAG := $(shell git describe --tags --abbrev=0))
 	@if [ "$(LATEST_TAG)" = "$(VERSION_PY)" ]; then \
 		echo "No version bump detected. Current version $(VERSION_PY) matches the latest tag $(LATEST_TAG)."; \
 		exit 1; \
 	fi
-	git tag $(VERSION_PY)
-	git push origin $(VERSION_PY)
-	@echo "Released new version $(VERSION_PY)"
+	git commit -m 'Release $(TAG)' --allow-empty
+	git tag $(TAG) -m "$(TAG)"
+	git push origin --follow-tags
+	@echo "Released new version $(TAG)"
```

### Comparing `stack_graphs_python_bindings-0.0.6/README.md` & `stack_graphs_python_bindings-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.6/src/classes.rs` & `stack_graphs_python_bindings-0.0.7/src/classes.rs`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.6/src/lib.rs` & `stack_graphs_python_bindings-0.0.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.6/src/stack_graphs_wrapper/mod.rs` & `stack_graphs_python_bindings-0.0.7/src/stack_graphs_wrapper/mod.rs`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.6/tests/test.py` & `stack_graphs_python_bindings-0.0.7/tests/test.py`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.6/Cargo.lock` & `stack_graphs_python_bindings-0.0.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1229,15 +1229,15 @@
  "serde_with",
  "smallvec",
  "thiserror",
 ]
 
 [[package]]
 name = "stack-graphs-python-bindings"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "pyo3",
  "stack-graphs",
  "tree-sitter-stack-graphs",
  "tree-sitter-stack-graphs-java",
  "tree-sitter-stack-graphs-javascript",
  "tree-sitter-stack-graphs-python",
```

### Comparing `stack_graphs_python_bindings-0.0.6/PKG-INFO` & `stack_graphs_python_bindings-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stack-graphs-python-bindings
-Version: 0.0.6
+Version: 0.0.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

