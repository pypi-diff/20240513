# Comparing `tmp/koza-0.5.4.tar.gz` & `tmp/koza-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koza-0.5.4.tar", max compression
+gzip compressed data, was "koza-0.6.0.tar", max compression
```

## Comparing `koza-0.5.4.tar` & `koza-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1526 2024-04-02 19:34:36.940962 koza-0.5.4/LICENSE
--rw-r--r--   0        0        0     2809 2024-04-02 19:34:36.940962 koza-0.5.4/README.md
--rw-r--r--   0        0        0     1159 2024-04-02 19:34:36.944963 koza-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       71 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/__init__.py
--rw-r--r--   0        0        0     8702 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/app.py
--rw-r--r--   0        0        0     6073 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/cli_runner.py
--rw-r--r--   0        0        0        0 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/converter/__init__.py
--rw-r--r--   0        0        0      883 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/converter/biolink_converter.py
--rw-r--r--   0        0        0     1730 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/converter/kgx_converter.py
--rw-r--r--   0        0        0      250 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/__init__.py
--rw-r--r--   0        0        0       62 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/reader/__init__.py
--rw-r--r--   0        0        0    10168 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/reader/csv_reader.py
--rw-r--r--   0        0        0     2964 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/reader/json_reader.py
--rw-r--r--   0        0        0     2118 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/reader/jsonl_reader.py
--rw-r--r--   0        0        0     7966 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/utils.py
--rw-r--r--   0        0        0        0 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/writer/__init__.py
--rw-r--r--   0        0        0     1553 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/writer/jsonl_writer.py
--rw-r--r--   0        0        0     4841 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/writer/tsv_writer.py
--rw-r--r--   0        0        0      370 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/writer/writer.py
--rw-r--r--   0        0        0     1572 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/yaml_loader.py
--rwxr-xr-x   0        0        0     2325 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/main.py
--rw-r--r--   0        0        0       28 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/config/__init__.py
--rw-r--r--   0        0        0      218 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/config/pydantic_config.py
--rw-r--r--   0        0        0    11357 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/config/source_config.py
--rw-r--r--   0        0        0     6206 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/config/sssom_config.py
--rw-r--r--   0        0        0      396 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/curie_cleaner.py
--rw-r--r--   0        0        0      356 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/map_dict.py
--rw-r--r--   0        0        0     3652 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/source.py
--rw-r--r--   0        0        0     2914 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/translation_table.py
--rw-r--r--   0        0        0        0 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/utils/__init__
--rw-r--r--   0        0        0      294 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/utils/exceptions.py
--rw-r--r--   0        0        0      763 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/utils/log_utils.py
--rw-r--r--   0        0        0     1849 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/utils/row_filter.py
--rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 koza-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1526 2024-05-13 20:38:24.748773 koza-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2809 2024-05-13 20:38:24.748773 koza-0.6.0/README.md
+-rw-r--r--   0        0        0     1189 2024-05-13 20:38:49.720295 koza-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/__init__.py
+-rw-r--r--   0        0        0     8649 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/app.py
+-rw-r--r--   0        0        0     7636 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/cli_utils.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/converter/__init__.py
+-rw-r--r--   0        0        0      898 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/converter/biolink_converter.py
+-rw-r--r--   0        0        0     1730 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/converter/kgx_converter.py
+-rw-r--r--   0        0        0      250 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/reader/__init__.py
+-rw-r--r--   0        0        0     9815 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/reader/csv_reader.py
+-rw-r--r--   0        0        0     2970 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/reader/json_reader.py
+-rw-r--r--   0        0        0     2118 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/reader/jsonl_reader.py
+-rw-r--r--   0        0        0     7969 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/utils.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/writer/__init__.py
+-rw-r--r--   0        0        0     1553 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/writer/jsonl_writer.py
+-rw-r--r--   0        0        0     4867 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/writer/tsv_writer.py
+-rw-r--r--   0        0        0      370 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/writer/writer.py
+-rw-r--r--   0        0        0     1572 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/io/yaml_loader.py
+-rwxr-xr-x   0        0        0     2367 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/main.py
+-rw-r--r--   0        0        0       28 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/model/config/__init__.py
+-rw-r--r--   0        0        0      213 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/model/config/pydantic_config.py
+-rw-r--r--   0        0        0    12276 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/model/config/source_config.py
+-rw-r--r--   0        0        0     6155 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/model/config/sssom_config.py
+-rw-r--r--   0        0        0      328 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/model/curie_cleaner.py
+-rw-r--r--   0        0        0      356 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/model/map_dict.py
+-rw-r--r--   0        0        0     3621 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/model/source.py
+-rw-r--r--   0        0        0     2914 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/model/translation_table.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/utils/__init__
+-rw-r--r--   0        0        0      294 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/utils/exceptions.py
+-rw-r--r--   0        0        0      763 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/utils/log_utils.py
+-rw-r--r--   0        0        0     1849 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/utils/row_filter.py
+-rw-r--r--   0        0        0     2237 2024-05-13 20:38:24.752773 koza-0.6.0/src/koza/utils/testing_utils.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 koza-0.6.0/PKG-INFO
```

### Comparing `koza-0.5.4/LICENSE` & `koza-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `koza-0.5.4/README.md` & `koza-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Koza - a data transformation framework  
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/koza.svg)](https://pypi.python.org/pypi/koza)
 [![PyPi](https://img.shields.io/pypi/v/koza.svg)](https://pypi.python.org/pypi/koza)
-![Github Action](https://github.com/monarch-initiative/koza/actions/workflows/build.yml/badge.svg)
+![Github Action](https://github.com/monarch-initiative/koza/actions/workflows/test.yaml/badge.svg)
 
 ![pupa](docs/img/pupa.png)  
 
 [**Documentation**](https://koza.monarchinitiative.org/  )
 
 _Disclaimer_: Koza is in beta - we are looking for testers!
```

### Comparing `koza-0.5.4/pyproject.toml` & `koza-0.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koza"
-version = "0.5.4"
+version = "v0.6.0"
 description = "Data transformation framework for LinkML data models"
 authors = [
     "The Monarch Initiative <info@monarchinitiative.org>",
     "Kevin Schaper <kevinschaper@gmail.com>",
     "Glass Elsarboukh <g.elsarboukh@gmail.com>",
     "Kent Shefchek <kent@tislab.org>",
     ]
@@ -12,43 +12,43 @@
 license = "BSD License"
 packages = [
     { include = "koza", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-linkml = ">=1.6.3"
+duckdb = "*"
+linkml = ">=1.7.8"
+loguru = "*"
+ordered-set = ">=4.1.0"
 pydantic = "^2.4"
 pyyaml = ">=5.0.0"
 requests = "^2.24.0"
-ordered-set = ">=4.1.0"
-typer = "^0.7.0"
-typer-cli = "^0.0.13"
-loguru = "*"
 sssom = ">=0.4"
+typer = ">=0.12.3"
 
 [tool.poetry.dev-dependencies]
-black = "^23.10.0"
+black = "^24.4"
 ruff = "*"
 pytest = ">=6.0.0"
-biolink-model = ">=3.6"
+biolink-model = ">=4.2"
 dask = ">=2022.5.2"
-mkdocs = ">=1.4.2"
-mkdocs-material = ">=9.1.16"
+mkdocs = ">=1.4"
+mkdocs-material = ">=9.5"
 mkdocstrings = {extras = ["python"], version = ">=0.22.0"}
 
 [tool.poetry.scripts]
 koza = "koza.main:typer_app"
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
-line_length = 120
+line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
 line-length = 120
-ignore = [
+lint.ignore = [
     "F541", # f-strings with no placeholders
 ]
```

### Comparing `koza-0.5.4/src/koza/app.py` & `koza-0.6.0/src/koza/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,19 @@
         self.output_dir = output_dir
         self.output_format = output_format
         self._map_registry: Dict[str, Source] = {}
         self._map_cache: Dict[str, Dict] = {}
         self.curie_cleaner: CurieCleaner = CurieCleaner()
         self.writer: KozaWriter = self._get_writer()
         self.logger = logger
+        self.outfiles = []
+        if hasattr(self.writer, 'nodes_file_name'):
+            self.node_file = self.writer.nodes_file_name
+        if hasattr(self.writer, 'edges_file_name'):
+            self.edge_file = self.writer.edges_file_name
 
         if schema:
             # self.validate = True
             # self.schema = schema
             # self.node_type = node_type
             # self.edge_type = edge_type
             self.converter = KGXConverter()
@@ -77,15 +82,15 @@
     def process_sources(self):
         """
         Transform an entire file using ingest logic in a functionless python file
         where the path to this file is stored in source.transform_code
         or inferred by taking the name and path of the config file and looking for
         a .py file along side it (see constructor)
 
-        Intended for decoupling ingest logic into a configuration like file
+        Intended for decoupling ingest logic into a configuration-like file
         """
         import sys
 
         parent_path = Path(self.source.config.transform_code).parent
         transform_code = Path(self.source.config.transform_code).stem
         sys.path.append(str(parent_path))
         is_first = True
@@ -102,18 +107,18 @@
                     else:
                         importlib.reload(transform_module)
                 except MapItemException as mie:
                     if self.logger:
                         self.logger.debug(f"{str(mie)} not found in map")
                 except NextRowException:
                     continue
-                except ValidationError as ve:
+                except ValidationError:
                     if self.logger:
                         self.logger.error(f"Validation error while processing: {self.source.last_row}")
-                    raise ve
+                    raise ValidationError
                 except StopIteration:
                     break
         elif self.source.config.transform_mode == 'loop':
             if transform_code not in sys.modules.keys():
                 importlib.import_module(transform_code)
             else:
                 importlib.reload(importlib.import_module(transform_code))
@@ -210,17 +215,10 @@
             value_columns = map_file.config.values
             for row in map_file:
                 map[row[key_column]] = {key: value for key, value in row.items() if key in value_columns}
 
     @staticmethod
     def _map_sniffer(depends_on: str):
         """
-        TODO a utility function to determine if a depends_on string
-        is a path to a map config file, a yaml file that should be
-        interpreted as a dictionary, or a json file that should be
-        interpreted as a dictionary
-
-        See https://github.com/monarch-initiative/koza/issues/39
-
         :param depends_on:
         """
         pass
```

### Comparing `koza-0.5.4/src/koza/cli_runner.py` & `koza-0.6.0/src/koza/cli_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Module for managing koza runs through the CLI
 """
 
 from pathlib import Path
-from typing import Dict, Optional, Union
+from typing import Dict, Literal, Optional, Union
 import yaml
 
+import duckdb
+
 from koza.app import KozaApp
 from koza.io.reader.csv_reader import CSVReader
 from koza.io.reader.json_reader import JSONReader
 from koza.io.reader.jsonl_reader import JSONLReader
 from koza.io.utils import open_resource
 from koza.io.yaml_loader import UniqueIncludeLoader
 from koza.model.config.source_config import FormatType, OutputFormat, PrimaryFileConfig
@@ -25,22 +27,22 @@
     """Return a KozaApp object for a given source
 
     Args:
         source_name (str): Name of source
     """
     try:
         return koza_apps[source_name]
-    except:
+    except KeyError:
         raise KeyError(f"{source_name} was not found in KozaApp dictionary")
 
 
 def transform_source(
     source: str,
     output_dir: str,
-    output_format: OutputFormat = OutputFormat('tsv'),
+    output_format: OutputFormat = OutputFormat("tsv"),
     global_table: str = None,
     local_table: str = None,
     schema: str = None,
     node_type: str = None,
     edge_type: str = None,
     row_limit: int = None,
     verbose: bool = None,
@@ -57,23 +59,28 @@
         schema (str, optional): Path to schema file. Defaults to None.
         row_limit (int, optional): Number of rows to process. Defaults to None.
         verbose (bool, optional): Verbose logging. Defaults to None.
         log (bool, optional): Log to file. Defaults to False.
     """
     logger = get_logger(name=Path(source).name if log else None, verbose=verbose)
 
-    with open(source, 'r') as source_fh:
+    with open(source, "r") as source_fh:
         source_config = PrimaryFileConfig(**yaml.load(source_fh, Loader=UniqueIncludeLoader))
 
+    # Set name and transform code if not provided
     if not source_config.name:
         source_config.name = Path(source).stem
 
     if not source_config.transform_code:
-        # look for it alongside the source conf as a .py file
-        source_config.transform_code = str(Path(source).parent / Path(source).stem) + '.py'
+        filename = f"{Path(source).parent / Path(source).stem}.py"
+        if not Path(filename).exists():
+            filename = Path(source).parent / "transform.py"
+        if not Path(filename).exists():
+            raise FileNotFoundError(f"Could not find transform file for {source}")
+        source_config.transform_code = filename
 
     koza_source = Source(source_config, row_limit)
     logger.debug(f"Source created: {koza_source.config.name}")
     translation_table = get_translation_table(
         global_table if global_table else source_config.global_table,
         local_table if local_table else source_config.local_table,
         logger,
@@ -81,19 +88,52 @@
 
     koza_app = _set_koza_app(
         koza_source, translation_table, output_dir, output_format, schema, node_type, edge_type, logger
     )
     koza_app.process_maps()
     koza_app.process_sources()
 
+    ### QC checks
+
+    def _check_row_count(type: Literal["node", "edge"]):
+        """Check row count for nodes or edges."""
+
+        if type == "node":
+            outfile = koza_app.node_file
+            min_count = source_config.min_node_count
+        elif type == "edge":
+            outfile = koza_app.edge_file
+            min_count = source_config.min_edge_count
+
+        count = duckdb.sql(f"SELECT count(*) from '{outfile}' as count").fetchone()[0]
+
+        if row_limit and row_limit < min_count:
+            logger.warning(f"Row limit '{row_limit}' is less than expected count of {min_count} {type}s")
+        elif row_limit and row_limit < count:
+            logger.error(f"Actual {type} count {count} exceeds row limit {row_limit}")
+        else:
+            if count < min_count * 0.7:
+                raise ValueError(f"Actual {type} count {count} is less than 70% of expected {min_count} {type}s")
+            if min_count * 0.7 <= count < min_count:
+                logger.warning(
+                    f"Actual {type} count {count} is less than expected {min_count}, but more than 70% of expected"
+                )
+
+    # Confirm min number of rows in output
+    if hasattr(koza_app, "node_file") and source_config.min_node_count is not None:
+        _check_row_count("node")
+
+    if hasattr(koza_app, "edge_file") and source_config.min_edge_count is not None:
+        _check_row_count("edge")
+
 
 def validate_file(
     file: str,
     format: FormatType = FormatType.csv,
-    delimiter: str = ',',
+    delimiter: str = ",",
     header_delimiter: str = None,
     skip_blank_lines: bool = True,
 ):
     """
     Runs a file through one of the Koza readers
     For csv files will return header and row length
 
@@ -140,48 +180,42 @@
     if not global_table:
         if local_table:
             raise ValueError("Local table without a global table not allowed")
         else:
             logger.debug("No global table used for transform")
     else:
         if isinstance(global_table, str):
-            with open(global_table, 'r') as global_tt_fh:
+            with open(global_table, "r") as global_tt_fh:
                 global_tt = yaml.safe_load(global_tt_fh)
         elif isinstance(global_table, Dict):
             global_tt = global_table
 
         if local_table:
             if isinstance(local_table, str):
-                with open(local_table, 'r') as local_tt_fh:
+                with open(local_table, "r") as local_tt_fh:
                     local_tt = yaml.safe_load(local_tt_fh)
             elif isinstance(local_table, Dict):
                 local_tt = local_table
 
         else:
             logger.debug("No local table used for transform")
 
     return TranslationTable(global_tt, local_tt)
 
 
 def _set_koza_app(
     source: Source,
     translation_table: TranslationTable = None,
-    output_dir: str = './output',
-    output_format: OutputFormat = OutputFormat('tsv'),
+    output_dir: str = "./output",
+    output_format: OutputFormat = OutputFormat("tsv"),
     schema: str = None,
     node_type: str = None,
     edge_type: str = None,
     logger=None,
 ) -> KozaApp:
     """Create a KozaApp object for a given source"""
 
     koza_apps[source.config.name] = KozaApp(
         source, translation_table, output_dir, output_format, schema, node_type, edge_type, logger
     )
     logger.debug(f"koza_apps entry created for {source.config.name}: {koza_apps[source.config.name]}")
     return koza_apps[source.config.name]
-
-
-def test_koza(koza: KozaApp):
-    """Manually sets KozaApp (for testing)"""
-    global koza_app
-    koza_app = koza
```

### Comparing `koza-0.5.4/src/koza/converter/biolink_converter.py` & `koza-0.6.0/src/koza/converter/biolink_converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from biolink.pydanticmodel_v2 import Gene
+from biolink_model.datamodel.pydanticmodel_v2 import Gene
 
-from koza.cli_runner import koza_app
+from koza.cli_utils import koza_app
 
 
 def gpi2gene(row: dict) -> Gene:
     """
     Convert from Gene Product Information format to biolink:Gene instance
 
     http://geneontology.org/docs/gene-product-information-gpi-format/
```

### Comparing `koza-0.5.4/src/koza/converter/kgx_converter.py` & `koza-0.6.0/src/koza/converter/kgx_converter.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.4/src/koza/io/reader/csv_reader.py` & `koza-0.6.0/src/koza/io/reader/csv_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,16 +34,14 @@
       - Support a type map dictionary, in which fieldnames
         can be mapped to types, and the CSVReader will attempt
         to coerce them from their str representation, eg int('42')
 
       - Potentially will add support a multivalued field DSL, eg
         List[str][';'] would convert a semicolon delimited multivalued
         field to a list of strings
-
-    TODO handle cases when delimiter is >1 character
     """
 
     def __init__(
         self,
         io_str: IO[str],
         field_type_map: Dict[str, FieldType] = None,
         delimiter: str = ",",
@@ -133,34 +131,28 @@
 
         # skip commented lines (this is for footers)
         if self.comment_char is not None:
             while row[0].startswith(self.comment_char):
                 row = next(self.reader)
 
         # Check row length discrepancies for each row
-        # TODO currently varying line lengths will raise an exception
-        # and hard fail, we should probably make these warnings and report
-        # out which lines vary
-        # Could also create a custom exception and allow the client code
-        # to determine what to do here
         fields_len = len(self._header)
         row_len = len(row)
         stripped_row = [val.strip() for val in row]
 
         # if we've made it here we can convert a row to a dict
         field_map = dict(zip(self._header, stripped_row))
 
         if fields_len > row_len:
             raise ValueError(f"CSV file {self.name} has {fields_len - row_len} fewer columns at {self.reader.line_num}")
 
         elif fields_len < row_len:
             logger.warning(f"CSV file {self.name} has {row_len - fields_len} extra columns at {self.reader.line_num}")
-            # Not sure if this would serve a purpose
-            #
-            # if not 'extra_cols' in self.field_type_map:
+            # # Not sure if this would serve a purpose:
+            # if 'extra_cols' not in self.field_type_map:
             #     # Create a type map for extra columns
             #     self.field_type_map['extra_cols'] = FieldType.str
             # field_map['extra_cols'] = row[fields_len:]
 
         typed_field_map = {}
 
         for field, field_value in field_map.items():
```

### Comparing `koza-0.5.4/src/koza/io/reader/json_reader.py` & `koza-0.6.0/src/koza/io/reader/json_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import json, yaml
+import json
+import yaml
 from typing import IO, Any, Dict, Iterator, List, Union
 
 # from xmlrpc.client import Boolean
 
 from koza.io.utils import check_data
 
 # from koza.utils.log_utils import get_logger
```

### Comparing `koza-0.5.4/src/koza/io/reader/jsonl_reader.py` & `koza-0.6.0/src/koza/io/reader/jsonl_reader.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.4/src/koza/io/utils.py` & `koza-0.6.0/src/koza/io/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         raise ValueError(
             f"Cannot open local or remote file: {resource}. Check the URL/path, and that the file exists, and try again."
         )
 
     # If resource is local, check for compression
     if is_zipfile(resource):
         with ZipFile(resource, 'r') as zip_file:
-            file = TextIOWrapper(zip_file.open(zip_file.namelist()[0], 'r'))#, encoding='utf-8')
+            file = TextIOWrapper(zip_file.open(zip_file.namelist()[0], 'r'))  # , encoding='utf-8')
             # file = zip_file.read(zip_file.namelist()[0], 'r').decode('utf-8')
     elif str(resource).endswith('gz'):
         file = gzip.open(resource, 'rt')
         file.read(1)
         file.seek(0)
 
     # If resource is local and not compressed, open as text
```

### Comparing `koza-0.5.4/src/koza/io/writer/jsonl_writer.py` & `koza-0.6.0/src/koza/io/writer/jsonl_writer.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.4/src/koza/io/writer/tsv_writer.py` & `koza-0.6.0/src/koza/io/writer/tsv_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #### TSV Writer ####
 # NOTE - May want to rename to KGXWriter at some point, if we develop writers for other models non biolink/kgx specific
 
 from pathlib import Path
-import typing as t
+from typing import Dict, Iterable, List, Literal, Set, Union
 
 from ordered_set import OrderedSet
 
 from koza.converter.kgx_converter import KGXConverter
 from koza.io.utils import build_export_row
 from koza.io.writer.writer import KozaWriter
 from koza.model.config.sssom_config import SSSOMConfig
 
 
 class TSVWriter(KozaWriter):
     def __init__(
         self,
-        output_dir: t.Union[str, Path],
+        output_dir: Union[str, Path],
         source_name: str,
-        node_properties: t.List[str] = None,
-        edge_properties: t.List[str] = None,
+        node_properties: List[str] = None,
+        edge_properties: List[str] = None,
         sssom_config: SSSOMConfig = None,
     ):
         self.basename = source_name
         self.dirname = output_dir
         self.delimiter = "\t"
         self.list_delimiter = "|"
         self.converter = KGXConverter()
@@ -40,30 +40,30 @@
             if sssom_config:
                 edge_properties = self.add_sssom_columns(edge_properties)
             self.edge_columns = TSVWriter._order_columns(edge_properties, "edge")
             self.edges_file_name = Path(self.dirname if self.dirname else "", f"{self.basename}_edges.tsv")
             self.edgeFH = open(self.edges_file_name, "w")
             self.edgeFH.write(self.delimiter.join(self.edge_columns) + "\n")
 
-    def write(self, entities: t.Iterable) -> None:
+    def write(self, entities: Iterable) -> None:
         """Write an entities object to separate node and edge .tsv files"""
 
         nodes, edges = self.converter.convert(entities)
 
         if nodes:
             for node in nodes:
                 self.write_row(node, record_type="node")
 
         if edges:
             for edge in edges:
                 if self.sssom_config:
                     edge = self.sssom_config.apply_mapping(edge)
                 self.write_row(edge, record_type="edge")
 
-    def write_row(self, record: t.Dict, record_type: t.Literal["node", "edge"]) -> None:
+    def write_row(self, record: Dict, record_type: Literal["node", "edge"]) -> None:
         """Write a row to the underlying store.
 
         Args:
             record: Dict - A node or edge record
             record_type: Literal["node", "edge"] - The record_type of record
         """
         fh = self.nodeFH if record_type == "node" else self.edgeFH
@@ -84,15 +84,15 @@
 
         if hasattr(self, "nodeFH"):
             self.nodeFH.close()
         if hasattr(self, "edgeFH"):
             self.edgeFH.close()
 
     @staticmethod
-    def _order_columns(cols: t.Set, record_type: t.Literal["node", "edge"]) -> OrderedSet:
+    def _order_columns(cols: Set, record_type: Literal["node", "edge"]) -> OrderedSet:
         """Arrange node or edge columns in a defined order.
 
         Args:
             cols: Set - A set with elements in any order
 
         Returns:
             OrderedSet - A set with elements in a defined order
```

### Comparing `koza-0.5.4/src/koza/io/yaml_loader.py` & `koza-0.6.0/src/koza/io/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.4/src/koza/main.py` & `koza-0.6.0/src/koza/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """CLI for Koza - wraps the koza library to provide a command line interface"""
 
 from pathlib import Path
 from typing import Optional
 
-from koza.cli_runner import transform_source, validate_file
+from koza.cli_utils import transform_source, validate_file
 from koza.model.config.source_config import FormatType, OutputFormat
 
 import typer
 
 typer_app = typer.Typer()
 
 
@@ -20,49 +20,51 @@
         typer.echo(f"Koza version: {__version__}")
         raise typer.Exit()
 
 
 @typer_app.command()
 def transform(
     source: str = typer.Option(..., help="Source metadata file"),
-    output_dir: str = typer.Option('./output', help="Path to output directory"),
+    output_dir: str = typer.Option("./output", help="Path to output directory"),
     output_format: OutputFormat = typer.Option("tsv", help="Output format"),
     global_table: str = typer.Option(None, help="Path to global translation table"),
     local_table: str = typer.Option(None, help="Path to local translation table"),
-    schema: str = typer.Option(None, help='Path to schema YAML for validation in writer'),
+    schema: str = typer.Option(None, help="Path to schema YAML for validation in writer"),
     row_limit: int = typer.Option(None, help="Number of rows to process (if skipped, processes entire source file)"),
     verbose: Optional[bool] = typer.Option(None, "--debug/--quiet"),
-    log: bool = typer.Option(False, help='Optional log mode - set true to save output to ./logs'),
+    log: bool = typer.Option(False, help="Optional log mode - set true to save output to ./logs"),
 ) -> None:
     """Transform a source file"""
-
     output_path = Path(output_dir)
-
     if output_path.exists() and not output_path.is_dir():
         raise NotADirectoryError(f"{output_dir} is not a directory")
     elif not output_path.exists():
         output_path.mkdir(parents=True)
-
-    transform_source(source, output_dir, output_format, global_table, local_table, schema, row_limit, verbose, log)
+    transform_source(
+        source,
+        output_dir,
+        output_format,
+        global_table,
+        local_table,
+        schema,
+        node_type=None,
+        edge_type=None,
+        row_limit=row_limit,
+        verbose=verbose,
+        log=log,
+    )
 
 
 @typer_app.command()
 def validate(
     file: str = typer.Option(..., help="Path or url to the source file"),
     format: FormatType = FormatType.csv,
-    delimiter: str = ',',
+    delimiter: str = ",",
     header_delimiter: str = None,
     skip_blank_lines: bool = True,
 ) -> None:
     """Validate a source file"""
     validate_file(file, format, delimiter, header_delimiter, skip_blank_lines)
 
 
-# @typer_app.command()
-# def create():
-#    """
-#    TODO
-#    Create a new koza project
-#    """
-
-# if __name__ == "__main__":
-#     typer_app()
+if __name__ == "__main__":
+    typer_app()
```

### Comparing `koza-0.5.4/src/koza/model/config/source_config.py` & `koza-0.6.0/src/koza/model/config/source_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import zipfile
 from dataclasses import field
 from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Union, Optional
 import yaml
 
-from loguru import logger
 from pydantic import StrictFloat, StrictInt, StrictStr
 from pydantic.dataclasses import dataclass
 
 from koza.model.config.pydantic_config import PYDANTIC_CONFIG
 from koza.model.config.sssom_config import SSSOMConfig
 
 
@@ -53,15 +52,15 @@
 class FormatType(str, Enum):
     """Enum for supported file types"""
 
     csv = "csv"
     jsonl = "jsonl"
     json = "json"
     yaml = "yaml"
-    xml = "xml"  # TODO
+    # xml = "xml" # Not yet supported
 
 
 class HeaderMode(str, Enum):
     """Enum for supported header modes in addition to an index based lookup"""
 
     infer = "infer"
     none = "none"
@@ -112,74 +111,74 @@
 
 @dataclass(frozen=True)
 class DatasetDescription:
     """
     These options should be treated as being in alpha, as we need
     to align with various efforts (hcls, translator infores)
 
-    These currently do not serve a purpose in koza other
-    than documentation
+    These currently do not serve a purpose in koza other than documentation
     """
 
-    id: Optional[str] = None  # TODO constrain to a curie?
+    # id: Optional[str] = None          # Can uncomment when we have a standard
     name: Optional[str] = None  # If empty use source name
-    ingest_title: Optional[str] = None  # Map to biolink name
-    ingest_url: Optional[str] = None  # Maps to biolink iri
-    description: Optional[str] = None
-    source: Optional[str] = None
-    provided_by: Optional[str] = None
-    license: Optional[str] = None
-    rights: Optional[str] = None
+    ingest_title: Optional[str] = None  # Title of source of data, map to biolink name
+    ingest_url: Optional[str] = None  # URL to source of data, maps to biolink iri
+    description: Optional[str] = None  # Description of the data/ingest
+    # source: Optional[str] = None      # Possibly replaced with provided_by
+    provided_by: Optional[str] = None  # <data source>_<type_of_ingest>, ex. hpoa_gene_to_disease
+    # license: Optional[str] = None     # Possibly redundant, same as rights
+    rights: Optional[str] = None  # License information for the data source
 
 
 @dataclass(config=PYDANTIC_CONFIG)
 class SourceConfig:
     """
     Source config data class
 
     Parameters
     ----------
     name: str (required) - name of the source
     files: List[str] (required) - list of files to process
     file_archive: str (optional) - path to a file archive containing files to process
     format: FormatType (optional) - format of the data file(s)
     sssom_config: SSSOMConfig (optional) - SSSOM config options
-    metadata: DatasetDescription (optional) - metadata for the source
     columns: List[str] (optional) - list of columns to include
+    field_type_map: dict (optional) - dict of field names and their type (using the FieldType enum)
+    filters: List[ColumnFilter] (optional) - list of filters to apply
     required_properties: List[str] (optional) - list of properties which must be in json data files
+    metadata: DatasetDescription (optional) - metadata for the source
     delimiter: str (optional) - delimiter for csv files
-    header: int (optional) - header row index
+    header: int (optional) - header row index (required if format is csv and header is not none)
     header_delimiter: str (optional) - delimiter for header in csv files
     header_prefix: str (optional) - prefix for header in csv files
     comment_char: str (optional) - comment character for csv files
     skip_blank_lines: bool (optional) - skip blank lines in csv files
-    filters: List[ColumnFilter] (optional) - list of filters to apply
     json_path: List[str] (optional) - path within JSON object containing data to process
     transform_code: str (optional) - path to a python file to transform the data
     transform_mode: TransformMode (optional) - how to process the transform file
     global_table: str (optional) - path to a global table file
     local_table: str (optional) - path to a local table file
     """
 
     name: str
     files: List[Union[str, Path]]
     file_archive: Optional[Union[str, Path]] = None
     format: FormatType = FormatType.csv
     sssom_config: Optional[SSSOMConfig] = None
     columns: Optional[List[Union[str, Dict[str, FieldType]]]] = None
     field_type_map: Optional[dict] = None
+    filters: List[ColumnFilter] = field(default_factory=list)
     required_properties: Optional[List[str]] = None
     metadata: Optional[Union[DatasetDescription, str]] = None
     delimiter: Optional[str] = None
     header: Union[int, HeaderMode] = HeaderMode.infer
     header_delimiter: Optional[str] = None
     header_prefix: Optional[str] = None
     comment_char: str = "#"
     skip_blank_lines: bool = True
-    filters: List[ColumnFilter] = field(default_factory=list)
     json_path: Optional[List[Union[StrictStr, StrictInt]]] = None
     transform_code: Optional[str] = None
     transform_mode: TransformMode = TransformMode.flat
     global_table: Optional[Union[str, Dict]] = None
     local_table: Optional[Union[str, Dict]] = None
 
     def extract_archive(self):
@@ -188,51 +187,48 @@
             with tarfile.open(self.file_archive) as archive:
                 archive.extractall(archive_path)
         elif self.file_archive.endswith(".zip"):
             with zipfile.ZipFile(self.file_archive, "r") as archive:
                 archive.extractall(archive_path)
         else:
             raise ValueError("Error extracting archive. Supported archive types: .tar.gz, .zip")
-        files = [os.path.join(archive_path, file) for file in self.files]
+        if self.files:
+            files = [os.path.join(archive_path, file) for file in self.files]
+        else:
+            files = [os.path.join(archive_path, file) for file in os.listdir(archive_path)]
         return files
 
     def __post_init__(self):
-        """
-        TO DO figure out why we're using object.__setattr__(self, ...)
-            here and document it.
-            Is this a workaround for a pydantic bug?
-        """
+        # Get files as paths, or extract them from an archive
         if self.file_archive:
             files = self.extract_archive()
         else:
             files = self.files
 
         files_as_paths: List[Path] = []
         for file in files:
             if isinstance(file, str):
                 files_as_paths.append(Path(file))
             else:
                 files_as_paths.append(file)
         object.__setattr__(self, "files", files_as_paths)
-        # self.files = files_as_paths <---- is this equivalent to the above?
 
+        # If metadata looks like a file path attempt to load it from the yaml
         if self.metadata and isinstance(self.metadata, str):
-            # If this looks like a file path attempt to load it from the yaml
-            # TODO enforce that this is imported via an include?
-            # See https://github.com/monarch-initiative/koza/issues/46
             try:
                 with open(self.metadata, "r") as meta:
                     object.__setattr__(self, "metadata", DatasetDescription(**yaml.safe_load(meta)))
             except Exception as e:
-                # TODO check for more explicit exceptions
                 raise ValueError(f"Unable to load metadata from {self.metadata}: {e}")
 
+        # Format tab as delimiter
         if self.delimiter in ["tab", "\\t"]:
             object.__setattr__(self, "delimiter", "\t")
 
+        # Filter columns
         filtered_columns = [column_filter.column for column_filter in self.filters]
 
         all_columns = []
         if self.columns:
             all_columns = [next(iter(column)) if isinstance(column, Dict) else column for column in self.columns]
 
         if self.header == HeaderMode.none and not self.columns:
@@ -245,70 +241,79 @@
 
         for column in filtered_columns:
             if column not in all_columns:
                 raise (ValueError(f"Filter column {column} not in column list"))
 
         for column_filter in self.filters:
             if column_filter.filter_code in ["lt", "gt", "lte", "gte"]:
-                # TODO determine if this should raise an exception
-                # or instead try to type coerce the string to a float
-                # type coercion is probably the best thing to do here
                 if not isinstance(column_filter.value, (int, float)):
                     raise ValueError(f"Filter value must be int or float for operator {column_filter.filter_code}")
             elif column_filter.filter_code == "eq":
                 if not isinstance(column_filter.value, (str, int, float)):
                     raise ValueError(
                         f"Filter value must be string, int or float for operator {column_filter.filter_code}"
                     )
             elif column_filter.filter_code == "in":
                 if not isinstance(column_filter.value, List):
                     raise ValueError(f"Filter value must be List for operator {column_filter.filter_code}")
 
+        # Check for conflicting configurations
         if self.format == FormatType.csv and self.required_properties:
             raise ValueError(
                 "CSV specified but required properties have been configured\n"
-                "either set format to jsonl or change properties to columns in the config"
+                "Either set format to jsonl or change properties to columns in the config"
             )
-
         if self.columns and self.format != FormatType.csv:
             raise ValueError(
-                "columns have been configured but format is not csv\n"
-                "either set format to csv or change columns to properties in the config"
+                "Columns have been configured but format is not csv\n"
+                "Either set format to csv or change columns to properties in the config"
             )
-
         if self.json_path and self.format != FormatType.json:
             raise ValueError(
                 "iterate_over has been configured but format is not json\n"
-                "either set format to json or remove iterate_over in the configuration"
+                "Either set format to json or remove iterate_over in the configuration"
             )
 
+        # Create a field_type_map if columns are supplied
         if self.columns:
             field_type_map = {}
             for field in self.columns:
                 if isinstance(field, str):
                     field_type_map[field] = FieldType.str
                 else:
                     if len(field) != 1:
-                        # TODO expand this exception msg
                         raise ValueError("Field type map contains more than one key")
                     for key, val in field.items():
                         field_type_map[key] = val
-            # print(f"FIELD TYPE MAP: {field_type_map}")    
-            self.field_type_map = field_type_map
+            object.__setattr__(self, "field_type_map", field_type_map)
 
 
 @dataclass(config=PYDANTIC_CONFIG)
 class PrimaryFileConfig(SourceConfig):
     """
-    node_properties and edge_properties are used for configuring
-    the KGX writer
+    Primary configuration for transforming a source file
+
+    Parameters
+    ----------
+    node_properties: List[str] (optional) - list of node properties/columns to include
+    edge_properties: List[str] (optional) - list of edge properties/columns to include
+    min_node_count: int (optional) - minimum number of nodes required in output
+    min_edge_count: int (optional) - minimum number of edges required in output
+    node_report_columns: List[str] (optional) - list of node properties to include in the report
+    edge_report_columns: List[str] (optional) - list of edge properties to include in the report
+    depends_on: List[str] (optional) - Optional lookup dictionary for basic mapping
+    on_map_failure: MapErrorEnum (optional) - How to handle key errors in map files
     """
 
     node_properties: Optional[List[str]] = None
     edge_properties: Optional[List[str]] = None
+    min_node_count: Optional[int] = None
+    min_edge_count: Optional[int] = None
+    # node_report_columns: Optional[List[str]] = None
+    # edge_report_columns: Optional[List[str]] = None
     depends_on: List[str] = field(default_factory=list)
     on_map_failure: MapErrorEnum = MapErrorEnum.warning
 
 
 @dataclass(config=PYDANTIC_CONFIG)
 class MapFileConfig(SourceConfig):
     key: Optional[str] = None
```

### Comparing `koza-0.5.4/src/koza/model/config/sssom_config.py` & `koza-0.6.0/src/koza/model/config/sssom_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
             df=new_msdf.df, filter_prefixes=filters, require_all_prefixes=False, features=new_msdf.df.columns  # type: ignore
         )
 
         return new_msdf
 
     def _build_sssom_lut(self) -> Dict:
         """Build a lookup table from SSSOM mapping dataframe."""
-        # TODO add narrow and broad match mappings
         sssom_lut = {}
         for _, row in self.df.iterrows():
             subject_id = row["subject_id"]
             object_id = row["object_id"]
             predicate = row["predicate_id"]
             if Match.exact in self.use_match:
                 # Add exact match mappings in both directions
```

### Comparing `koza-0.5.4/src/koza/model/source.py` & `koza-0.6.0/src/koza/model/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,59 +15,59 @@
     """
     Source class for files and maps
 
     Source is an iterator that provides a layer of abstraction over file types
     and adds filter support to the readers in io.reader
 
     config: Source config
-    reader: An iterator that takes in an IO[str] as its first argument
-    and yields a dictionary
+    row_limit: Number of rows to process
+    reader: An iterator that takes in an IO[str] and yields a dictionary
     """
 
     def __init__(self, config: Union[PrimaryFileConfig, MapFileConfig], row_limit: Optional[int] = None):
         self.config = config
         self.row_limit = row_limit
         self._filter = RowFilter(config.filters)
         self._reader = None
         self._readers: List = []
         self.last_row: Optional[Dict] = None
 
         for file in config.files:
             resource_io = open_resource(file)
-            if self.config.format == 'csv':
+            if self.config.format == "csv":
                 self._readers.append(
                     CSVReader(
                         resource_io,
                         name=config.name,
                         field_type_map=config.field_type_map,
                         delimiter=config.delimiter,
                         header=config.header,
                         header_delimiter=config.header_delimiter,
                         header_prefix=config.header_prefix,
                         comment_char=self.config.comment_char,
                         row_limit=self.row_limit,
                     )
                 )
-            elif self.config.format == 'jsonl':
+            elif self.config.format == "jsonl":
                 self._readers.append(
                     JSONLReader(
                         resource_io,
                         name=config.name,
                         required_properties=config.required_properties,
                         row_limit=self.row_limit,
                     )
                 )
-            elif self.config.format == 'json' or self.config.format == 'yaml':
+            elif self.config.format == "json" or self.config.format == "yaml":
                 self._readers.append(
                     JSONReader(
                         resource_io,
                         name=config.name,
                         json_path=config.json_path,
                         required_properties=config.required_properties,
-                        is_yaml=(self.config.format == 'yaml'),
+                        is_yaml=(self.config.format == "yaml"),
                         row_limit=self.row_limit,
                     )
                 )
             else:
                 raise ValueError(f"File type {format} not supported")
 
     def __iter__(self) -> Iterator:
@@ -86,14 +86,13 @@
                 row = self._get_row()
         return row
 
     def _get_row(self):
         if self._filter:
             row = next(self._reader)
             while not self._filter.include_row(row):
-                # TODO log filtered out lines
                 row = next(self._reader)
         else:
             row = next(self._reader)
         # Retain the most recent row so that it can be logged alongside validation errors
         self.last_row = row
         return row
```

### Comparing `koza-0.5.4/src/koza/model/translation_table.py` & `koza-0.6.0/src/koza/model/translation_table.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.4/src/koza/utils/log_utils.py` & `koza-0.6.0/src/koza/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.4/src/koza/utils/row_filter.py` & `koza-0.6.0/src/koza/utils/row_filter.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.4/PKG-INFO` & `koza-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: koza
-Version: 0.5.4
+Version: 0.6.0
 Summary: Data transformation framework for LinkML data models
 License: BSD License
 Author: The Monarch Initiative
 Author-email: info@monarchinitiative.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: linkml (>=1.6.3)
+Requires-Dist: duckdb
+Requires-Dist: linkml (>=1.7.8)
 Requires-Dist: loguru
 Requires-Dist: ordered-set (>=4.1.0)
 Requires-Dist: pydantic (>=2.4,<3.0)
 Requires-Dist: pyyaml (>=5.0.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: sssom (>=0.4)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
-Requires-Dist: typer-cli (>=0.0.13,<0.0.14)
+Requires-Dist: typer (>=0.12.3)
 Description-Content-Type: text/markdown
 
 # Koza - a data transformation framework  
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/koza.svg)](https://pypi.python.org/pypi/koza)
 [![PyPi](https://img.shields.io/pypi/v/koza.svg)](https://pypi.python.org/pypi/koza)
-![Github Action](https://github.com/monarch-initiative/koza/actions/workflows/build.yml/badge.svg)
+![Github Action](https://github.com/monarch-initiative/koza/actions/workflows/test.yaml/badge.svg)
 
 ![pupa](docs/img/pupa.png)  
 
 [**Documentation**](https://koza.monarchinitiative.org/  )
 
 _Disclaimer_: Koza is in beta - we are looking for testers!
```

