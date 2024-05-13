# Comparing `tmp/solar_registry-0.2.1.tar.gz` & `tmp/solar_registry-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.2.1.tar", last modified: Mon May 13 06:24:35 2024, max compression
+gzip compressed data, was "solar_registry-0.2.2.tar", last modified: Mon May 13 11:46:44 2024, max compression
```

## Comparing `solar_registry-0.2.1.tar` & `solar_registry-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-05-13 06:24:10.323039 solar_registry-0.2.1/LICENSE
--rw-r--r--   0        0        0      682 2024-05-13 06:24:10.323039 solar_registry-0.2.1/README.md
--rw-r--r--   0        0        0     1182 2024-05-13 06:24:35.175118 solar_registry-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     1418 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     4789 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0     2051 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     2517 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2628 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      505 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/test_merger.py
--rw-r--r--   0        0        0      495 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/test_pr_generator.py
--rw-r--r--   0        0        0      928 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/test_testtool.py
--rw-r--r--   0        0        0      731 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/testdata/error_meta_file/pytest/testtool.yaml
--rw-r--r--   0        0        0      736 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/testdata/error_version_file/pytest/testtool.yaml
--rw-r--r--   0        0        0     2820 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 solar_registry-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 11:46:22.059521 solar_registry-0.2.2/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-13 11:46:22.059521 solar_registry-0.2.2/README.md
+-rw-r--r--   0        0        0     1182 2024-05-13 11:46:44.535754 solar_registry-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     1880 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     4906 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0     2051 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     2517 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2628 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      505 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     1625 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-13 11:46:22.059521 solar_registry-0.2.2/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:46:22.059521 solar_registry-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-13 11:46:22.059521 solar_registry-0.2.2/tests/test_merger.py
+-rw-r--r--   0        0        0      495 2024-05-13 11:46:22.059521 solar_registry-0.2.2/tests/test_pr_generator.py
+-rw-r--r--   0        0        0      928 2024-05-13 11:46:22.059521 solar_registry-0.2.2/tests/test_testtool.py
+-rw-r--r--   0        0        0      291 2024-05-13 11:46:22.059521 solar_registry-0.2.2/tests/test_validator.py
+-rw-r--r--   0        0        0      731 2024-05-13 11:46:22.059521 solar_registry-0.2.2/tests/testdata/error_meta_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0      736 2024-05-13 11:46:22.059521 solar_registry-0.2.2/tests/testdata/error_version_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0     2820 2024-05-13 11:46:22.059521 solar_registry-0.2.2/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-13 11:46:22.063521 solar_registry-0.2.2/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     2942 2024-05-13 11:46:22.063521 solar_registry-0.2.2/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 solar_registry-0.2.2/PKG-INFO
```

### Comparing `solar_registry-0.2.1/LICENSE` & `solar_registry-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/README.md` & `solar_registry-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/pyproject.toml` & `solar_registry-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.2.1"
+version = "0.2.2"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.2.1/src/solar_registry/cli.py` & `solar_registry-0.2.2/src/solar_registry/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import typer
 from loguru import logger
 from typing_extensions import Annotated
 
 from .commands.meta_merger import MetaMerger
 from .service.pr_generator import PullRequestGenerator
 from .service.testtool import get_testtool
+from .service.validator import ToolValidator
 
 app = typer.Typer()
 
 
 @app.command()
 def merge(tool_name: str, output: str, working_dir: Optional[str] = None) -> None:
     """
@@ -37,17 +38,34 @@
     testtool = get_testtool(tool_name, working_dir)
     pr_gen = PullRequestGenerator(testtool)
     pr_gen.merge_and_create_pull_request()
 
 
 @app.command()
 def validate(tool_name: str, working_dir: Optional[str] = None) -> None:
+    """
+    校验测试工具的testtools.yaml是否符合要求
+
+    :param tool_name: 工具名称
+    :param working_dir: 可选工作目录
+    """
     testtool = get_testtool(tool_name, working_dir)
     logger.info(f"测试工具 {testtool.name} 有效性校验通过")
 
 
+@app.command()
+def validate_json(working_dir: Optional[str] = None) -> None:
+    """
+    校验当前目录下的json文件是否符合要求
+
+    :param working_dir: 可选工作目录
+    """
+    validator = ToolValidator(working_dir)
+    validator.validate()
+
+
 def cli_entry() -> None:
     app()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `solar_registry-0.2.1/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.2.2/src/solar_registry/commands/meta_merger.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,30 +28,34 @@
         """
         new_index = self._download_and_merge_stable_index()
         new_history = self._download_and_merge_meta_history()
 
         index_file = Path(output_dir) / "testtools" / "stable.index.json"
         index_file.parent.mkdir(exist_ok=True, parents=True)
         with open(index_file, "w", encoding="utf-8") as f:
-            f.write(new_index.model_dump_json(by_alias=True, indent=2))
+            f.write(
+                new_index.model_dump_json(by_alias=True, indent=2, exclude_none=True)
+            )
 
         meta_file = (
             Path(output_dir)
             / "testtools"
             / self.testtool.lang
             / self.testtool.name
             / "metadata.json"
         )
         meta_file.parent.mkdir(exist_ok=True, parents=True)
         with open(
             meta_file,
             "w",
             encoding="utf-8",
         ) as f:
-            f.write(new_history.model_dump_json(by_alias=True, indent=2))
+            f.write(
+                new_history.model_dump_json(by_alias=True, indent=2, exclude_none=True)
+            )
 
     def _download_and_merge_stable_index(self) -> StableIndexMetaData:
         """
         合并稳定索引文件内容
 
         一般用于新版本发布后索引文件的更新
         """
@@ -120,15 +124,15 @@
         for index, version in enumerate(history.versions):
             if version.meta.version == self.metadata.meta.version:
                 history.versions[index] = self.metadata
         else:
             history.versions.append(self.metadata)
 
         logger.info(
-            f"Merge meta history result: {history.model_dump_json(by_alias=True, indent=2)}"
+            f"Merge meta history result: {history.model_dump_json(by_alias=True, indent=2, exclude_none=True)}"
         )
 
         return history
 
     def _create_new_metadata_history(self) -> MetaDataHistory:
         # 读取本地生成好的metadata文件
         logger.info("Creating meta history...")
```

### Comparing `solar_registry-0.2.1/src/solar_registry/model/test_tool.py` & `solar_registry-0.2.2/src/solar_registry/model/test_tool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/src/solar_registry/service/generator.py` & `solar_registry-0.2.2/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/src/solar_registry/service/pr_generator.py` & `solar_registry-0.2.2/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/src/solar_registry/util/file.py` & `solar_registry-0.2.2/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/tests/test_merger.py` & `solar_registry-0.2.2/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/tests/test_testtool.py` & `solar_registry-0.2.2/tests/test_testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/tests/testdata/error_meta_file/pytest/testtool.yaml` & `solar_registry-0.2.2/tests/testdata/error_meta_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/tests/testdata/error_version_file/pytest/testtool.yaml` & `solar_registry-0.2.2/tests/testdata/error_version_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.2.2/tests/testdata/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.1/PKG-INFO` & `solar_registry-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

