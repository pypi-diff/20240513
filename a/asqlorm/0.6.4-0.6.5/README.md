# Comparing `tmp/asqlorm-0.6.4.tar.gz` & `tmp/asqlorm-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asqlorm-0.6.4.tar", max compression
+gzip compressed data, was "asqlorm-0.6.5.tar", max compression
```

## Comparing `asqlorm-0.6.4.tar` & `asqlorm-0.6.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.4/README.md
--rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.4/asqlorm/__init__.py
--rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.4/asqlorm/generator/main.py
--rw-r--r--   0        0        0    44542 2024-04-25 00:06:52.855343 asqlorm-0.6.4/asqlorm/models.py
--rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.4/asqlorm/sql/sql_alchemy.py
--rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.4/asqlorm/utils.py
--rw-r--r--   0        0        0      655 2024-05-08 17:40:19.668975 asqlorm-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 asqlorm-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.5/README.md
+-rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.5/asqlorm/__init__.py
+-rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.5/asqlorm/generator/main.py
+-rw-r--r--   0        0        0    44542 2024-04-25 00:06:52.855343 asqlorm-0.6.5/asqlorm/models.py
+-rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.5/asqlorm/sql/sql_alchemy.py
+-rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.5/asqlorm/utils.py
+-rw-r--r--   0        0        0      652 2024-05-13 21:32:47.423151 asqlorm-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 asqlorm-0.6.5/PKG-INFO
```

### Comparing `asqlorm-0.6.4/asqlorm/generator/main.py` & `asqlorm-0.6.5/asqlorm/generator/main.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.4/asqlorm/models.py` & `asqlorm-0.6.5/asqlorm/models.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.4/asqlorm/sql/sql_alchemy.py` & `asqlorm-0.6.5/asqlorm/sql/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.4/asqlorm/utils.py` & `asqlorm-0.6.5/asqlorm/utils.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.4/pyproject.toml` & `asqlorm-0.6.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asqlorm"
-version = "0.6.4"
+version = "0.6.5"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = 'asqlorm' }]
 exclude = ["tests/**/*"]
 
 
@@ -13,15 +13,15 @@
 pydantic = "^2.7"
 fastgql = "*"
 devtools = "*"
 sqlparse = "*"
 black = "*"
 psycopg = {extras = ["binary"], version = "*"}
 sqlalchemy = "^2.0.29"
-sentry-sdk = {extras = ["sqlalchemy"], version = "^1.45.0"}
+sentry-sdk = {extras = ["sqlalchemy"], version = "^2.1"}
 greenlet = "^3.0.3"
 asyncpg = "^0.29.0"
 
 [tool.poetry.dev-dependencies]
 mypy = '^1.8'
 ruff = '*'
 doppler-env = '^0.3.1'
```

### Comparing `asqlorm-0.6.4/PKG-INFO` & `asqlorm-0.6.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asqlorm
-Version: 0.6.4
+Version: 0.6.5
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: black
 Requires-Dist: devtools
 Requires-Dist: fastgql
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: psycopg[binary]
 Requires-Dist: pydantic (>=2.7,<3.0)
-Requires-Dist: sentry-sdk[sqlalchemy] (>=1.45.0,<2.0.0)
+Requires-Dist: sentry-sdk[sqlalchemy] (>=2.1,<3.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: sqlparse
 Description-Content-Type: text/markdown
 
 sqlorm!
```

