# Comparing `tmp/flux_local-5.2.0.tar.gz` & `tmp/flux_local-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux_local-5.2.0.tar", last modified: Fri May 10 20:10:03 2024, max compression
+gzip compressed data, was "flux_local-5.3.0.tar", last modified: Sun May 12 22:34:29 2024, max compression
```

## Comparing `flux_local-5.2.0.tar` & `flux_local-5.3.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.689629 flux_local-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 20:09:56.000000 flux_local-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-10 20:10:03.689629 flux_local-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-10 20:09:56.000000 flux_local-5.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.681629 flux_local-5.2.0/flux_local/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27576 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22676 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.685629 flux_local-5.2.0/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16948 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/tool/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-10 20:09:56.000000 flux_local-5.2.0/flux_local/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.689629 flux_local-5.2.0/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 20:10:03.000000 flux_local-5.2.0/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-10 20:10:03.689629 flux_local-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-10 20:09:56.000000 flux_local-5.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.685629 flux_local-5.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16462 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/test_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:10:03.689629 flux_local-5.2.0/tests/tool/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_diff_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_diff_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_get_hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_get_ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-10 20:09:56.000000 flux_local-5.2.0/tests/tool/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.645139 flux_local-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 22:34:25.000000 flux_local-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-12 22:34:29.645139 flux_local-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-12 22:34:25.000000 flux_local-5.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.637139 flux_local-5.3.0/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27695 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22706 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.641139 flux_local-5.3.0/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16948 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/tool/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-12 22:34:25.000000 flux_local-5.3.0/flux_local/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.645139 flux_local-5.3.0/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 22:34:29.000000 flux_local-5.3.0/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-12 22:34:25.000000 flux_local-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-12 22:34:29.645139 flux_local-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 22:34:25.000000 flux_local-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.641139 flux_local-5.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16462 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:34:29.645139 flux_local-5.3.0/tests/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_diff_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_diff_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_get_hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_get_ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-12 22:34:25.000000 flux_local-5.3.0/tests/tool/test_test.py
```

### Comparing `flux_local-5.2.0/LICENSE` & `flux_local-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/PKG-INFO` & `flux_local-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 5.2.0
+Version: 5.3.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux_local-5.2.0/README.md` & `flux_local-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/command.py` & `flux_local-5.3.0/flux_local/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,17 @@
     """Run a set of commands, piped together, returning stdout of last."""
     stdin = None
     out = None
     for cmd in cmds:
         try:
             out = await asyncio.wait_for(cmd.run(stdin), _TIMEOUT)
         except asyncio.exceptions.TimeoutError as err:
-            raise cmd.exc(f"Command '{cmd}' timed out") from err
+            if isinstance(cmd, Command):
+                raise cmd.exc(f"Command '{cmd}' timed out") from err
+            raise err
         stdin = out
     return out.decode("utf-8") if out else ""
 
 
 async def run_piped(cmds: Sequence[Task]) -> str:
     """Run a set of commands, piped together, returning stdout of last."""
     async with _SEM:
```

### Comparing `flux_local-5.2.0/flux_local/context.py` & `flux_local-5.3.0/flux_local/context.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/exceptions.py` & `flux_local-5.3.0/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/git_repo.py` & `flux_local-5.3.0/flux_local/git_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,15 +629,17 @@
             if doc.get("kind") == CONFIG_MAP_KIND
         ]
         kustomization.secrets = [
             Secret.parse_doc(doc) for doc in docs if doc.get("kind") == SECRET_KIND
         ]
 
 
-def _ready_kustomizations(kustomizations: list[Kustomization], visited: set[str]) -> tuple[Kustomization, Kustomization]:
+def _ready_kustomizations(
+    kustomizations: list[Kustomization], visited: set[str]
+) -> tuple[list[Kustomization], list[Kustomization]]:
     """Split the kustomizations into those that are ready vs pending."""
     ready = []
     pending = []
     for kustomization in kustomizations:
         if not_ready := (set(kustomization.depends_on or {}) - visited):
             _LOGGER.debug(
                 "Kustomization %s waiting for %s",
@@ -686,15 +688,19 @@
         async def update_kustomization(cluster: Cluster) -> None:
             queue = [*cluster.kustomizations]
             visited: set[str] = set()
             while queue:
                 build_tasks = []
                 (ready, pending) = _ready_kustomizations(queue, visited)
                 for kustomization in ready:
-                    _LOGGER.debug("Processing kustomization '%s': %s", kustomization.name, kustomization.path)
+                    _LOGGER.debug(
+                        "Processing kustomization '%s': %s",
+                        kustomization.name,
+                        kustomization.path,
+                    )
 
                     if kustomization.postbuild_substitute_from:
                         values.expand_postbuild_substitute_reference(
                             kustomization,
                             values.ks_cluster_config(cluster.kustomizations),
                         )
                         # Clear the cache to remove any previous builds that are
@@ -768,15 +774,17 @@
                             None,
                         )
 
         return Manifest(clusters=clusters)
 
 
 @contextlib.contextmanager
-def create_worktree(repo: git.repo.Repo, existing_branch: str | None = None) -> Generator[Path, None, None]:
+def create_worktree(
+    repo: git.repo.Repo, existing_branch: str | None = None
+) -> Generator[Path, None, None]:
     """Create a ContextManager for a new git worktree in the current repo.
 
     This is used to get a fork of the current repo without any local changes
     in order to produce a diff.
     Specifying existing_branch allows  to compare the current state with the existing branch.
     """
     orig = os.getcwd()
```

### Comparing `flux_local-5.2.0/flux_local/helm.py` & `flux_local-5.3.0/flux_local/helm.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from .manifest import (
     HelmRelease,
     HelmRepository,
     CRD_KIND,
     SECRET_KIND,
     REPO_TYPE_OCI,
     HELM_REPOSITORY,
-    GIT_REPOSITORY
+    GIT_REPOSITORY,
 )
 from .exceptions import HelmException
 
 __all__ = [
     "Helm",
     "Options",
 ]
@@ -64,26 +64,25 @@
 
 HELM_BIN = "helm"
 
 
 def _chart_name(release: HelmRelease, repo: HelmRepository | None) -> str:
     """Return the helm chart name used for the helm template command."""
     if release.chart.repo_kind == HELM_REPOSITORY:
-        if repo.repo_type == REPO_TYPE_OCI:
+        if repo and repo.repo_type == REPO_TYPE_OCI:
             return f"{repo.url}/{release.chart.name}"
         return release.chart.chart_name
     elif release.chart.repo_kind == GIT_REPOSITORY:
         return release.chart.name
     raise HelmException(
         f"Unable to find chart source for chart {release.chart.chart_name} "
         f"kind {release.chart.repo_kind} for HelmRelease {release.name}"
     )
 
 
-
 class RepositoryConfig:
     """Generates a helm repository configuration from flux HelmRepository objects."""
 
     def __init__(self, repos: list[HelmRepository]) -> None:
         """Initialize RepositoryConfig."""
         self._repos = repos
```

### Comparing `flux_local-5.2.0/flux_local/image.py` & `flux_local-5.3.0/flux_local/image.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/kustomize.py` & `flux_local-5.3.0/flux_local/kustomize.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 You can apply kyverno policies to the objects with the `validate` method.
 """
 
 from aiofiles.ospath import isdir
 import asyncio
 from contextlib import asynccontextmanager
+from collections.abc import AsyncIterator
 import logging
 from pathlib import Path
 import tempfile
 from typing import Any, AsyncGenerator
 
 import yaml
 
@@ -66,14 +67,15 @@
 KYVERNO_BIN = "kyverno"
 FLUX_BIN = "flux"
 HELM_RELEASE_KIND = "HelmRelease"
 
 # Used to limit access to specific resources
 _LOCK_MAP: dict[str, asyncio.Lock] = {}
 
+
 class Kustomize:
     """Library for issuing a kustomize command."""
 
     def __init__(self, cmds: list[Task]) -> None:
         """Initialize Kustomize, used internally for copying object."""
         self._cmds = cmds
 
@@ -190,17 +192,17 @@
 
     async def run(self, stdin: bytes | None = None) -> bytes:
         """Run the task."""
         return self._out
 
 
 @asynccontextmanager
-async def _resource_lock(key: str):
+async def _resource_lock(key: str) -> AsyncIterator[None]:
     """Run while holding a lock for the specified resource.
-    
+
     This is not threadsafe and expected to be run in the asyncio loop.
     """
     if not (lock := _LOCK_MAP.get(key)):
         lock = asyncio.Lock()
         _LOCK_MAP[key] = lock
     async with lock:
         yield
```

### Comparing `flux_local-5.2.0/flux_local/manifest.py` & `flux_local-5.3.0/flux_local/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     @classmethod
     def parse_yaml(cls, content: str) -> "BaseManifest":
         """Parse a serialized manifest."""
         return yaml_decode(content, cls)
 
     def yaml(self, exclude: dict[str, Any] | None = None) -> str:
         """Return a YAML string representation of compact_dict."""
-        return yaml_encode(self, self.__class__)
+        return yaml_encode(self, self.__class__)  # type: ignore[return-value]
 
     class Config(BaseConfig):
         omit_none = True
 
 
 @dataclass
 class HelmChart(BaseManifest):
```

### Comparing `flux_local-5.2.0/flux_local/tool/build.py` & `flux_local-5.3.0/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/tool/diagnostics.py` & `flux_local-5.3.0/flux_local/tool/diagnostics.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/tool/diff.py` & `flux_local-5.3.0/flux_local/tool/diff.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/tool/flux_local.py` & `flux_local-5.3.0/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/tool/format.py` & `flux_local-5.3.0/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/tool/get.py` & `flux_local-5.3.0/flux_local/tool/get.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/tool/selector.py` & `flux_local-5.3.0/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/tool/test.py` & `flux_local-5.3.0/flux_local/tool/test.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/tool/visitor.py` & `flux_local-5.3.0/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local/values.py` & `flux_local-5.3.0/flux_local/values.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/flux_local.egg-info/PKG-INFO` & `flux_local-5.3.0/flux_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 5.2.0
+Version: 5.3.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux_local-5.2.0/flux_local.egg-info/SOURCES.txt` & `flux_local-5.3.0/flux_local.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 flux_local/__init__.py
 flux_local/command.py
 flux_local/context.py
 flux_local/exceptions.py
 flux_local/git_repo.py
```

### Comparing `flux_local-5.2.0/setup.cfg` & `flux_local-5.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 5.2.0
+version = 5.3.0
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux_local-5.2.0/tests/test_command.py` & `flux_local-5.3.0/tests/test_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for command library."""
 
 import pytest
 
-from flux_local.command import Command, CommandException, run, run_piped
+from flux_local.command import Command, run, run_piped
+from flux_local.exceptions import CommandException
 
 
 async def test_command() -> None:
     """Test stdout parsing of a command."""
     result = await run(Command(["echo", "Hello"]))
     assert result == "Hello\n"
```

### Comparing `flux_local-5.2.0/tests/test_git_repo.py` & `flux_local-5.3.0/tests/test_git_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 async def test_kustomization_visitor(snapshot: SnapshotAssertion) -> None:
     """Tests for visiting Kustomizations."""
 
     query = ResourceSelector()
     query.path.path = TESTDATA
 
     stream = io.StringIO()
-    visits: list[tuple[str, str, str, str]] = []
+    visits: list[tuple[str, str, str]] = []
 
     async def write(x: Path, y: Any, cmd: Kustomize | None) -> None:
         visits.append((str(x), y.namespace, y.name))
         if cmd:
             stream.write(await cmd.run())
 
     query.kustomization.visitor = ResourceVisitor(func=write)
@@ -108,15 +108,15 @@
 
 async def test_helm_repo_visitor(snapshot: SnapshotAssertion) -> None:
     """Tests for visiting a HelmRepository objects."""
 
     query = ResourceSelector()
     query.path.path = TESTDATA
 
-    visits: list[tuple[str, str, str, str]] = []
+    visits: list[tuple[str, str, str]] = []
 
     async def append(x: Path, y: Any, z: Any) -> None:
         visits.append((str(x), y.namespace, y.name))
 
     query.helm_repo.visitor = ResourceVisitor(func=append)
 
     manifest = await build_manifest(selector=query)
@@ -128,15 +128,15 @@
 
 async def test_helm_release_visitor(snapshot: SnapshotAssertion) -> None:
     """Tests for visiting a HelmRelease objects."""
 
     query = ResourceSelector()
     query.path.path = TESTDATA
 
-    visits: list[tuple[str, str, str, str]] = []
+    visits: list[tuple[str, str, str]] = []
 
     async def append(x: Path, y: Any, z: Any) -> None:
         visits.append((str(x), y.namespace, y.name))
 
     query.helm_release.visitor = ResourceVisitor(
         func=append,
     )
```

### Comparing `flux_local-5.2.0/tests/test_helm.py` & `flux_local-5.3.0/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/test_image.py` & `flux_local-5.3.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/test_kustomize.py` & `flux_local-5.3.0/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/test_manifest.py` & `flux_local-5.3.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/test_values.py` & `flux_local-5.3.0/tests/test_values.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_build.py` & `flux_local-5.3.0/tests/tool/test_build.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_diagnostics.py` & `flux_local-5.3.0/tests/tool/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_diff.py` & `flux_local-5.3.0/tests/tool/test_diff.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_diff_hr.py` & `flux_local-5.3.0/tests/tool/test_diff_hr.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_diff_ks.py` & `flux_local-5.3.0/tests/tool/test_diff_ks.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_format.py` & `flux_local-5.3.0/tests/tool/test_format.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_get_cluster.py` & `flux_local-5.3.0/tests/tool/test_get_cluster.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_get_hr.py` & `flux_local-5.3.0/tests/tool/test_get_hr.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_get_ks.py` & `flux_local-5.3.0/tests/tool/test_get_ks.py`

 * *Files identical despite different names*

### Comparing `flux_local-5.2.0/tests/tool/test_test.py` & `flux_local-5.3.0/tests/tool/test_test.py`

 * *Files identical despite different names*

