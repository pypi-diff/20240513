# Comparing `tmp/cookieplone-0.5.1.tar.gz` & `tmp/cookieplone-0.5.2.tar.gz`

## Comparing `cookieplone-0.5.1.tar` & `cookieplone-0.5.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cookieplone-0.5.1/CHANGES.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.1/Makefile
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tox.ini
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.1/.github/workflows/changelog.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.1/.github/workflows/main.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/__main__.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/cli.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/data.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/exceptions.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/generator.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/repository.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/settings.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/console.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/files.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/git.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/internal.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.1/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.1/news/.changelog_template.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/test_filters.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/utils/test_commands.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/utils/test_console.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/utils/test_containers.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/utils/test_files.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/utils/test_git.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/utils/test_internal.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/utils/test_sanity.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/utils/test_validators.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.1/tests/utils/test_versions.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.1/LICENSE
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.1/README.md
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 cookieplone-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 cookieplone-0.5.2/CHANGES.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 cookieplone-0.5.2/Makefile
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tox.ini
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cookieplone-0.5.2/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 cookieplone-0.5.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/cli.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/data.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/generator.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/repository.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/settings.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/git.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/internal.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cookieplone-0.5.2/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cookieplone-0.5.2/news/.changelog_template.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/test_filters.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_console.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_containers.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_internal.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_sanity.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_validators.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cookieplone-0.5.2/tests/utils/test_versions.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cookieplone-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 cookieplone-0.5.2/LICENSE
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 cookieplone-0.5.2/README.md
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 cookieplone-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 cookieplone-0.5.2/PKG-INFO
```

### Comparing `cookieplone-0.5.1/.pre-commit-config.yaml` & `cookieplone-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/CHANGES.md` & `cookieplone-0.5.2/CHANGES.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 0.5.2 (2024-05-13)
+
+
+### Bug fixes:
+
+- Set default `tag` value to **main** instead of the empty string [@ericof] [#15](https://github.com/plone/cookieplone/issues/15)
+
 ## 0.5.1 (2024-05-07)
 
 
 ### Internal:
 
 - Use `gh:plone/cookieplone-templates` as the default repository [@ericof] [#13](https://github.com/plone/cookieplone/issues/13)
```

### Comparing `cookieplone-0.5.1/Makefile` & `cookieplone-0.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/.github/workflows/changelog.yml` & `cookieplone-0.5.2/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/.github/workflows/main.yml` & `cookieplone-0.5.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/cli.py` & `cookieplone-0.5.2/cookieplone/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         data.OptionalListStr,
         typer.Argument(callback=validate_extra_context, help="Extra context."),
     ] = None,
     output_dir: Annotated[
         data.OptionalPath,
         typer.Option("--output-dir", "-o", help="Where to generate the code."),
     ] = None,
-    tag: Annotated[str, typer.Option(help="Tag.")] = "",
+    tag: Annotated[str, typer.Option(help="Tag.")] = "main",
     version: Annotated[
         bool, typer.Option("--version", help="Display the version of cookieplone.")
     ] = False,
     no_input: Annotated[
         bool,
         typer.Option(
             "--no_input",
```

### Comparing `cookieplone-0.5.1/cookieplone/data.py` & `cookieplone-0.5.2/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/exceptions.py` & `cookieplone-0.5.2/cookieplone/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/generator.py` & `cookieplone-0.5.2/cookieplone/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
     except exc.UndefinedVariableInTemplate as undefined_err:
         context_str = json.dumps(undefined_err.context, indent=2, sort_keys=True)
         msg = f"""{undefined_err.message}
         Error message: {undefined_err.error.message}
         Context: {context_str}
         """
         raise GeneratorException(message=msg, original=undefined_err)  # noQA:B904
+    except Exception as e:
+        raise GeneratorException(message=str(e), original=e)  # noQA:B904
     else:
         return Path(result)
 
 
 def generate_subtemplate(
     template: str,
     output_dir: Path,
```

### Comparing `cookieplone-0.5.1/cookieplone/repository.py` & `cookieplone-0.5.2/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/settings.py` & `cookieplone-0.5.2/cookieplone/settings.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/filters/__init__.py` & `cookieplone-0.5.2/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/utils/console.py` & `cookieplone-0.5.2/cookieplone/utils/console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/utils/files.py` & `cookieplone-0.5.2/cookieplone/utils/files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/utils/git.py` & `cookieplone-0.5.2/cookieplone/utils/git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/utils/internal.py` & `cookieplone-0.5.2/cookieplone/utils/internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/utils/sanity.py` & `cookieplone-0.5.2/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/utils/validators.py` & `cookieplone-0.5.2/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/utils/versions.py` & `cookieplone-0.5.2/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/cookieplone/utils/commands/__init__.py` & `cookieplone-0.5.2/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/tests/test_filters.py` & `cookieplone-0.5.2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/tests/utils/test_commands.py` & `cookieplone-0.5.2/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/tests/utils/test_console.py` & `cookieplone-0.5.2/tests/utils/test_console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/tests/utils/test_files.py` & `cookieplone-0.5.2/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/tests/utils/test_git.py` & `cookieplone-0.5.2/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/tests/utils/test_internal.py` & `cookieplone-0.5.2/tests/utils/test_internal.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/tests/utils/test_sanity.py` & `cookieplone-0.5.2/tests/utils/test_sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/tests/utils/test_validators.py` & `cookieplone-0.5.2/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/tests/utils/test_versions.py` & `cookieplone-0.5.2/tests/utils/test_versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/.gitignore` & `cookieplone-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/LICENSE` & `cookieplone-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/README.md` & `cookieplone-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/pyproject.toml` & `cookieplone-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.5.1/PKG-INFO` & `cookieplone-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cookieplone
-Version: 0.5.1
+Version: 0.5.2
 Summary: Create Plone projects, addons, documentation with ease!
 Project-URL: Documentation, https://github.com/plone/cookieplone#readme
 Project-URL: Issues, https://github.com/plone/cookieplone/issues
 Project-URL: Source, https://github.com/plone/cookieplone
 Author-email: Plone Community <dev@plone.org>
 License-Expression: MIT
 License-File: LICENSE
```

