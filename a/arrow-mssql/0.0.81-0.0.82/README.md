# Comparing `tmp/arrow_mssql-0.0.81.tar.gz` & `tmp/arrow_mssql-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrow_mssql-0.0.81.tar", max compression
+gzip compressed data, was "arrow_mssql-0.0.82.tar", max compression
```

## Comparing `arrow_mssql-0.0.81.tar` & `arrow_mssql-0.0.82.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      188 2024-04-10 19:19:46.678750 arrow_mssql-0.0.81/arrow_mssql/__init__.py
--rw-r--r--   0        0        0     1355 2024-04-02 19:24:19.265370 arrow_mssql-0.0.81/arrow_mssql/connector.py
--rw-r--r--   0        0        0     3609 2024-04-02 19:13:05.501619 arrow_mssql-0.0.81/arrow_mssql/export.py
--rw-r--r--   0        0        0        0 2024-04-02 17:17:13.445964 arrow_mssql-0.0.81/arrow_mssql/input/__init__.py
--rw-r--r--   0        0        0     3608 2024-04-10 18:24:20.692624 arrow_mssql-0.0.81/arrow_mssql/input/datatypes.py
--rw-r--r--   0        0        0     1568 2024-04-10 19:18:55.641653 arrow_mssql-0.0.81/arrow_mssql/input/schema.py
--rw-r--r--   0        0        0     1288 2024-04-10 18:36:45.564350 arrow_mssql-0.0.81/arrow_mssql/iport.py
--rw-r--r--   0        0        0        0 2024-04-02 17:15:34.399775 arrow_mssql-0.0.81/arrow_mssql/output/__init__.py
--rw-r--r--   0        0        0     2553 2024-04-02 19:07:18.402978 arrow_mssql-0.0.81/arrow_mssql/output/datatypes.py
--rw-r--r--   0        0        0     3435 2024-04-02 17:14:32.689965 arrow_mssql-0.0.81/arrow_mssql/output/schemas.py
--rw-r--r--   0        0        0      718 2024-03-18 12:53:20.396252 arrow_mssql-0.0.81/arrow_mssql/utils.py
--rw-r--r--   0        0        0      753 2024-04-10 19:19:38.301593 arrow_mssql-0.0.81/pyproject.toml
--rw-r--r--   0        0        0     1594 2024-04-10 18:46:28.079048 arrow_mssql-0.0.81/README.md
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 arrow_mssql-0.0.81/PKG-INFO
+-rw-r--r--   0        0        0      188 2024-04-10 19:20:44.547505 arrow_mssql-0.0.82/arrow_mssql/__init__.py
+-rw-r--r--   0        0        0     1355 2024-05-13 19:47:30.898739 arrow_mssql-0.0.82/arrow_mssql/connector.py
+-rw-r--r--   0        0        0     3609 2024-04-02 19:13:05.501619 arrow_mssql-0.0.82/arrow_mssql/export.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:17:13.445964 arrow_mssql-0.0.82/arrow_mssql/input/__init__.py
+-rw-r--r--   0        0        0     3608 2024-04-10 18:24:20.692624 arrow_mssql-0.0.82/arrow_mssql/input/datatypes.py
+-rw-r--r--   0        0        0     1568 2024-04-10 19:18:55.641653 arrow_mssql-0.0.82/arrow_mssql/input/schema.py
+-rw-r--r--   0        0        0     1288 2024-04-10 18:36:45.564350 arrow_mssql-0.0.82/arrow_mssql/iport.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:15:34.399775 arrow_mssql-0.0.82/arrow_mssql/output/__init__.py
+-rw-r--r--   0        0        0     2553 2024-04-02 19:07:18.402978 arrow_mssql-0.0.82/arrow_mssql/output/datatypes.py
+-rw-r--r--   0        0        0     3435 2024-04-02 17:14:32.689965 arrow_mssql-0.0.82/arrow_mssql/output/schemas.py
+-rw-r--r--   0        0        0      718 2024-03-18 12:53:20.396252 arrow_mssql-0.0.82/arrow_mssql/utils.py
+-rw-r--r--   0        0        0      755 2024-05-13 19:42:58.634364 arrow_mssql-0.0.82/pyproject.toml
+-rw-r--r--   0        0        0     1691 2024-05-13 19:45:26.619629 arrow_mssql-0.0.82/README.md
+-rw-r--r--   0        0        0     2427 1970-01-01 00:00:00.000000 arrow_mssql-0.0.82/PKG-INFO
```

### Comparing `arrow_mssql-0.0.81/arrow_mssql/connector.py` & `arrow_mssql-0.0.82/arrow_mssql/connector.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.81/arrow_mssql/export.py` & `arrow_mssql-0.0.82/arrow_mssql/export.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.81/arrow_mssql/input/datatypes.py` & `arrow_mssql-0.0.82/arrow_mssql/input/datatypes.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.81/arrow_mssql/input/schema.py` & `arrow_mssql-0.0.82/arrow_mssql/input/schema.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.81/arrow_mssql/iport.py` & `arrow_mssql-0.0.82/arrow_mssql/iport.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.81/arrow_mssql/output/datatypes.py` & `arrow_mssql-0.0.82/arrow_mssql/output/datatypes.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.81/arrow_mssql/output/schemas.py` & `arrow_mssql-0.0.82/arrow_mssql/output/schemas.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.81/arrow_mssql/utils.py` & `arrow_mssql-0.0.82/arrow_mssql/utils.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.81/pyproject.toml` & `arrow_mssql-0.0.82/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arrow-mssql"
-version = "0.0.81"
+version = "0.0.82"
 description = "Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet para tabela do sql server"
 authors = ["Marcus Holanda <mvsh777@hotmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Natural Language :: Portuguese (Brazilian)",
     "Programming Language :: PL/SQL",
@@ -13,14 +13,14 @@
 
 [tool.poetry.urls]
 "Codigo" = "https://github.com/Marcus-Holanda777/arrow-mssql"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pyodbc = "^5.1.0"
-pyarrow = "15.0.0"
-sqlglot = "20.11.0"
+pyarrow = "^16.0.0"
+sqlglot = "^23.15.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `arrow_mssql-0.0.81/README.md` & `arrow_mssql-0.0.82/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Arrow-mssql
+[![PyPI](https://img.shields.io/pypi/v/arrow-mssql.svg)](https://pypi.org/project/arrow-mssql/)
 
 ## O que é o Arrow-mssql ?
 
 é um projeto que recebe uma tabela ou consulta do `SQL SERVER`
 e faz a exportação para um arquivo *.parquet* ou *.csv*,
 utilizando a solução [arrow](https://arrow.apache.org/docs/index.html) que é uma tecnologia com
 foco em análise e desempenho na memória.
```

### Comparing `arrow_mssql-0.0.81/PKG-INFO` & `arrow_mssql-0.0.82/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: arrow-mssql
-Version: 0.0.81
+Version: 0.0.82
 Summary: Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet para tabela do sql server
 Author: Marcus Holanda
 Author-email: mvsh777@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Programming Language :: PL/SQL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pyarrow (==15.0.0)
+Requires-Dist: pyarrow (>=16.0.0,<17.0.0)
 Requires-Dist: pyodbc (>=5.1.0,<6.0.0)
-Requires-Dist: sqlglot (==20.11.0)
+Requires-Dist: sqlglot (>=23.15.0,<24.0.0)
 Project-URL: Codigo, https://github.com/Marcus-Holanda777/arrow-mssql
 Description-Content-Type: text/markdown
 
 # Arrow-mssql
+[![PyPI](https://img.shields.io/pypi/v/arrow-mssql.svg)](https://pypi.org/project/arrow-mssql/)
 
 ## O que é o Arrow-mssql ?
 
 é um projeto que recebe uma tabela ou consulta do `SQL SERVER`
 e faz a exportação para um arquivo *.parquet* ou *.csv*,
 utilizando a solução [arrow](https://arrow.apache.org/docs/index.html) que é uma tecnologia com
 foco em análise e desempenho na memória.
```

