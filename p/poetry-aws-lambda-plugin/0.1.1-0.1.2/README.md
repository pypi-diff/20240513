# Comparing `tmp/poetry_aws_lambda_plugin-0.1.1.tar.gz` & `tmp/poetry_aws_lambda_plugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_aws_lambda_plugin-0.1.1.tar", max compression
+gzip compressed data, was "poetry_aws_lambda_plugin-0.1.2.tar", max compression
```

## Comparing `poetry_aws_lambda_plugin-0.1.1.tar` & `poetry_aws_lambda_plugin-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1097 2024-05-12 11:39:30.627126 poetry_aws_lambda_plugin-0.1.1/LICENSE
--rw-r--r--   0        0        0      796 2024-05-12 18:24:20.209461 poetry_aws_lambda_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-12 11:39:30.627126 poetry_aws_lambda_plugin-0.1.1/README.md
--rw-r--r--   0        0        0      107 2024-05-12 11:39:30.629207 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 11:39:30.630313 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/builders/__init__.py
--rw-r--r--   0        0        0     1278 2024-05-12 11:39:30.630313 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/builders/builder.py
--rw-r--r--   0        0        0     3156 2024-05-12 17:38:50.543492 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/builders/zip.py
--rw-r--r--   0        0        0        0 2024-05-12 11:39:30.631410 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/commands/__init__.py
--rw-r--r--   0        0        0     4857 2024-05-12 11:39:30.631410 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/commands/build_aws_lambda.py
--rw-r--r--   0        0        0        0 2024-05-12 11:39:30.632483 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/packages_getters/__init__.py
--rw-r--r--   0        0        0     5292 2024-05-12 11:39:30.632483 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/packages_getters/dependencies.py
--rw-r--r--   0        0        0      793 2024-05-12 11:39:30.633514 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/packages_getters/package_getter.py
--rw-r--r--   0        0        0     1922 2024-05-12 11:39:30.633514 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/packages_getters/project.py
--rw-r--r--   0        0        0      482 2024-05-12 11:39:30.634562 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/plugin.py
--rw-r--r--   0        0        0        0 2024-05-12 11:39:30.634615 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/slimmers/__init__.py
--rw-r--r--   0        0        0     3531 2024-05-12 11:39:30.634615 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/slimmers/files_remover.py
--rw-r--r--   0        0        0      821 2024-05-12 11:39:30.636055 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/slimmers/slimmer.py
--rw-r--r--   0        0        0        0 2024-05-12 11:39:30.636055 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/steps/__init__.py
--rw-r--r--   0        0        0      849 2024-05-12 11:39:30.637132 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/steps/step.py
--rw-r--r--   0        0        0        0 2024-05-12 11:39:30.637132 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/utils/__init__.py
--rw-r--r--   0        0        0     4977 2024-05-12 17:52:55.149830 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/utils/config.py
--rw-r--r--   0        0        0     1534 2024-05-12 11:39:30.639240 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/utils/enums.py
--rw-r--r--   0        0        0      203 2024-05-12 11:39:30.639322 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/utils/exceptions.py
--rw-r--r--   0        0        0      632 2024-05-12 11:39:30.639322 poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/utils/logging.py
--rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 poetry_aws_lambda_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-12 11:39:30.627126 poetry_aws_lambda_plugin-0.1.2/LICENSE
+-rw-r--r--   0        0        0      796 2024-05-13 21:22:48.374409 poetry_aws_lambda_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-12 11:39:30.627126 poetry_aws_lambda_plugin-0.1.2/README.md
+-rw-r--r--   0        0        0      107 2024-05-12 11:39:30.629207 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:39:30.630313 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/builders/__init__.py
+-rw-r--r--   0        0        0     1278 2024-05-12 11:39:30.630313 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/builders/builder.py
+-rw-r--r--   0        0        0     3171 2024-05-13 21:00:21.241369 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/builders/zip.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:39:30.631410 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/commands/__init__.py
+-rw-r--r--   0        0        0     5432 2024-05-13 21:19:39.221160 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/commands/build_aws_lambda.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:39:30.632483 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/packages_getters/__init__.py
+-rw-r--r--   0        0        0     5292 2024-05-12 11:39:30.632483 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/packages_getters/dependencies.py
+-rw-r--r--   0        0        0      793 2024-05-12 11:39:30.633514 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/packages_getters/package_getter.py
+-rw-r--r--   0        0        0     1922 2024-05-12 11:39:30.633514 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/packages_getters/project.py
+-rw-r--r--   0        0        0      482 2024-05-12 11:39:30.634562 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:39:30.634615 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/slimmers/__init__.py
+-rw-r--r--   0        0        0     3531 2024-05-12 11:39:30.634615 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/slimmers/files_remover.py
+-rw-r--r--   0        0        0      821 2024-05-12 11:39:30.636055 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/slimmers/slimmer.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:39:30.636055 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/steps/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-12 11:39:30.637132 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/steps/step.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:39:30.637132 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/utils/__init__.py
+-rw-r--r--   0        0        0     5096 2024-05-13 21:13:44.761839 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/utils/config.py
+-rw-r--r--   0        0        0     1539 2024-05-13 20:57:43.204038 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/utils/enums.py
+-rw-r--r--   0        0        0      203 2024-05-12 11:39:30.639322 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/utils/exceptions.py
+-rw-r--r--   0        0        0      632 2024-05-12 11:39:30.639322 poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/utils/logging.py
+-rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 poetry_aws_lambda_plugin-0.1.2/PKG-INFO
```

### Comparing `poetry_aws_lambda_plugin-0.1.1/LICENSE` & `poetry_aws_lambda_plugin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_aws_lambda_plugin-0.1.1/pyproject.toml` & `poetry_aws_lambda_plugin-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-aws-lambda-plugin"
-version = "0.1.1"
+version = "0.1.2"
 description = "Poetry plugin for building and publishing AWS Lambda functions and layers"
 authors = ["Hector Basset <hector.basset.dev@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "poetry_aws_lambda_plugin", from = "src" }
 ]
```

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/builders/builder.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/builders/builder.py`

 * *Files identical despite different names*

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/builders/zip.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/builders/zip.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     def do(self) -> None:
         write_lines(self.io, f"Building {self.description()}")
         if is_verbosity(self.io, Verbosity.VERBOSE):
             write_lines(
                 self.io,
                 str(self.output_path.relative_to(self.config.all_artefacts_path)),
-                f"Compression type: {self.config.compression_type.name}",
+                f"Compression type: {self.config.compression_algorithm.name}",
                 f"Compression level: {self.config.compression_level}",
                 stack_level=2,
                 verbosity=Verbosity.VERBOSE
             )
 
         if not self.dry_run:
             with zipfile.ZipFile(
                     self.output_path,
                     mode="w",
-                    compression=self.config.compression_type.numeric_constant,
+                    compression=self.config.compression_algorithm.numeric_constant,
                     compresslevel=self.config.compression_level
             ) as archive:
                 for input_path in self.input_paths:
                     for root, _, files in os.walk(input_path):
                         for file in files:
                             file_path = Path(root).joinpath(file)
                             arc_file_path = self.get_arc_file_path(file_path, input_path)
@@ -48,15 +48,15 @@
                                     f"Adding {file_path.relative_to(self.config.lambda_artefacts_path)} as {arc_file_path}.",
                                     verbosity=Verbosity.VERBOSE
                                 )
 
                             archive.write(
                                 file_path,
                                 arcname=arc_file_path,
-                                compress_type=self.config.compression_type.numeric_constant,
+                                compress_type=self.config.compression_algorithm.numeric_constant,
                                 compresslevel=self.config.compression_level
                             )
 
         write_lines(self.io, f"Built <c1>{self.output_path.name}</c1>")
 
 
 class FunctionBuilder(ZipBuilder):
```

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/commands/build_aws_lambda.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/commands/build_aws_lambda.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 from poetry_aws_lambda_plugin.builders.zip import FunctionBuilder, LayerBuilder
 from poetry_aws_lambda_plugin.packages_getters.dependencies import DependenciesPackagesGetter
 from poetry_aws_lambda_plugin.packages_getters.project import ProjectPackageGetter
 from poetry_aws_lambda_plugin.slimmers.files_remover import BinDirectoryRemoverSlimmer, DistInfoDirectoriesRemoverSlimmer, \
     TestsDirectoriesRemoverSlimmer, PycacheDirectoriesRemoverSlimmer, PyTypedFilesRemoverSlimmer
 from poetry_aws_lambda_plugin.utils.config import Config
-from poetry_aws_lambda_plugin.utils.enums import LambdaResource, describe_enum_config, LambdaArchitecture
+from poetry_aws_lambda_plugin.utils.enums import LambdaResource, describe_enum_config, LambdaArchitecture, \
+    CompressionAlgorithm
 from poetry_aws_lambda_plugin.utils.exceptions import PoetryAwsLambdaPluginException
 
 if TYPE_CHECKING:
     from typing import List
 
     from poetry_aws_lambda_plugin.steps.step import Step
 
@@ -38,26 +39,40 @@
         ),
         option(
             "only-root",
             None,
             "Exclude all dependencies and only install the root package (the current project)."
         ),
         option(
-            "resource",
+            "lambda-resource",
             "r",
             f"Lambda resource to build ({describe_enum_config(LambdaResource)})",
             flag=False,
             default=LambdaResource.FUNCTION.name.lower()
         ),
         option(
-            "architecture",
+            "lambda-architecture",
             "a",
             f"Lambda architecture ({describe_enum_config(LambdaArchitecture)})",
             flag=False,
             default=LambdaArchitecture.X86_64.name.lower()
+        ),
+        option(
+            "compression-algorithm",
+            "c",
+            f"ZIP compression algorithm ({describe_enum_config(CompressionAlgorithm)})",
+            flag=False,
+            default=CompressionAlgorithm.DEFLATED.name.lower()
+        ),
+        option(
+            "compression-level",
+            "l",
+            f"ZIP compression level, valid values depend on the compression algorithm "
+            f"(default to the minimum level of the selected algorithm)",
+            flag=False
         )
     ]
 
     @cached_property
     def config(self) -> Config:
         return Config(self)
```

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/packages_getters/dependencies.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/packages_getters/dependencies.py`

 * *Files identical despite different names*

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/packages_getters/package_getter.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/packages_getters/package_getter.py`

 * *Files identical despite different names*

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/packages_getters/project.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/packages_getters/project.py`

 * *Files identical despite different names*

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/slimmers/files_remover.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/slimmers/files_remover.py`

 * *Files identical despite different names*

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/slimmers/slimmer.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/slimmers/slimmer.py`

 * *Files identical despite different names*

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/steps/step.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/steps/step.py`

 * *Files identical despite different names*

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/utils/config.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/utils/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from functools import cached_property, lru_cache
 from typing import TYPE_CHECKING
 
 from poetry.core.constraints.version import Version, VersionRange
-from poetry_aws_lambda_plugin.utils.enums import LambdaResource, LambdaArchitecture, CompressionType
+from poetry_aws_lambda_plugin.utils.enums import LambdaResource, LambdaArchitecture, CompressionAlgorithm
 from poetry_aws_lambda_plugin.utils.exceptions import PoetryAwsLambdaPluginException
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Set, Optional
 
     from poetry.console.commands.group_command import GroupCommand
@@ -59,65 +59,65 @@
                 f"from package Python constraint {python_constraint}"
             )
 
         return Version.parse(f"{python_version.major}.{python_version.minor}")
 
     @cached_property
     def lambda_resource(self) -> LambdaResource:
-        resource_option = self._command.option("resource").upper()
+        resource_option = self._command.option("lambda-resource").upper()
         if resource_option not in LambdaResource.__members__:
             raise PoetryAwsLambdaPluginException(
                 f"Invalid Lambda Resource ({resource_option}), "
                 f"must be one of {', '.join(LambdaResource.__members__)}."
             )
         return LambdaResource[resource_option]
 
     @cached_property
     def lambda_architecture(self) -> LambdaArchitecture:
-        architecture_option = self._command.option("architecture").upper()
+        architecture_option = self._command.option("lambda-architecture").upper()
         if architecture_option not in LambdaArchitecture.__members__:
             raise PoetryAwsLambdaPluginException(
                 f"Invalid Lambda Architecture ({architecture_option}), "
                 f"must be one of {', '.join(LambdaArchitecture.__members__)}."
             )
         return LambdaArchitecture[architecture_option]
 
     @cached_property
-    def compression_type(self) -> CompressionType:
-        ct_config = (self._command.poetry.pyproject.data
-                     .get("aws-lambda", {})
-                     .get("compression-type", CompressionType.BZIP2.name)).upper()
-        if ct_config not in CompressionType.__members__:
+    def compression_algorithm(self) -> CompressionAlgorithm:
+        algorithm_option = self._command.option("compression-algorithm").upper()
+        if algorithm_option not in CompressionAlgorithm.__members__:
             raise PoetryAwsLambdaPluginException(
-                f"Invalid Compression Type ({ct_config}), "
-                f"must be one of {', '.join(CompressionType.__members__)}."
+                f"Invalid Compression Algorithm ({algorithm_option}), "
+                f"must be one of {', '.join(CompressionAlgorithm.__members__)}."
             )
-        return CompressionType[ct_config]
+        return CompressionAlgorithm[algorithm_option]
 
     @cached_property
     def compression_level(self) -> int:
-        ct = self.compression_type
-        cl_conf = (self._command.poetry.pyproject.data
-                   .get("aws-lambda", {})
-                   .get("compression-level", ct.min_compression_level))
+        algorithm = self.compression_algorithm
+        level_option = self._command.option("compression-level")
+        if level_option is None:
+            level_option = algorithm.min_compression_level
+        else:
+            level_option = int(level_option)
 
-        if ct.adjustable:
-            if (cl_conf < ct.min_compression_level) or (cl_conf > ct.max_compression_level):
+        if algorithm.adjustable:
+            if (level_option < algorithm.min_compression_level) or (level_option > algorithm.max_compression_level):
                 raise PoetryAwsLambdaPluginException(
-                    f"Invalid Compression Level ({cl_conf}), "
-                    f"must be between {ct.min_compression_level} and {ct.max_compression_level} "
-                    f"for {ct.name}."
+                    f"Invalid Compression Level ({level_option}), "
+                    f"must be between {algorithm.min_compression_level} and {algorithm.max_compression_level} "
+                    f"for {algorithm.name}."
                 )
-        elif cl_conf != ct.min_compression_level:
+        elif level_option != algorithm.min_compression_level:
             raise PoetryAwsLambdaPluginException(
-                f"Invalid Compression Level ({cl_conf}), "
-                f"must be {ct.min_compression_level} for {ct.name} (not adjustable)."
+                f"Invalid Compression Level ({level_option}), "
+                f"must be {algorithm.min_compression_level} for {algorithm.name} (not adjustable)."
             )
 
-        return cl_conf
+        return level_option
 
     @cached_property
     def slimmers(self) -> Optional[Set[str]]:
         return (self._command.poetry.pyproject.data
                 .get("aws-lambda", {})
                 .get("slimmers", None))
```

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/utils/enums.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/utils/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
     if default is not None:
         desc = f"{desc}, default to {default.name.lower()}"
 
     return desc
 
 
-class CompressionType(Enum):
+class CompressionAlgorithm(Enum):
     BZIP2 = (zipfile.ZIP_BZIP2, True, 1, 9)
-    DEFLATED = (zipfile.ZIP_DEFLATED, True, 0, 9)
+    DEFLATED = (zipfile.ZIP_DEFLATED, True, 1, 9)
     LZMA = (zipfile.ZIP_LZMA, False, -1, -1)
     STORED = (zipfile.ZIP_STORED, False, -1, -1)
 
     @property
     def numeric_constant(self) -> int:
         return self.value[0]
```

### Comparing `poetry_aws_lambda_plugin-0.1.1/src/poetry_aws_lambda_plugin/utils/logging.py` & `poetry_aws_lambda_plugin-0.1.2/src/poetry_aws_lambda_plugin/utils/logging.py`

 * *Files identical despite different names*

### Comparing `poetry_aws_lambda_plugin-0.1.1/PKG-INFO` & `poetry_aws_lambda_plugin-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-aws-lambda-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Poetry plugin for building and publishing AWS Lambda functions and layers
 Home-page: https://github.com/HectorBst/poetry-aws-lambda-plugin
 License: MIT
 Author: Hector Basset
 Author-email: hector.basset.dev@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

