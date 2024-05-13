# Comparing `tmp/pypomes_db-0.7.5.tar.gz` & `tmp/pypomes_db-0.7.6.tar.gz`

## Comparing `pypomes_db-0.7.5.tar` & `pypomes_db-0.7.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    17001 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    17279 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.6/PKG-INFO
```

### Comparing `pypomes_db-0.7.5/src/pypomes_db/__init__.py` & `pypomes_db-0.7.6/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.5/src/pypomes_db/db_common.py` & `pypomes_db-0.7.6/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.5/src/pypomes_db/db_pomes.py` & `pypomes_db-0.7.6/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.5/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.7.6/src/pypomes_db/migration_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,21 +323,26 @@
                     case "mysql":
                         pass
                     case "oracle":
                         ora_lob.write(data=lob_data,
                                       offset=offset)
                     case "postgres":
                         from psycopg2 import Binary
-                        # string data may come from some LOBs (Oracle's NCLOB is a good example)
+                        # remove append indication on first update
+                        if offset == 1:
+                            update_pg: str = update_stmt.replace(f"{target_column} || ", "")
+                        else:
+                            update_pg: str = update_stmt
+                        # string data may come from LOB (Oracle's NCLOB is a good example)
                         col_data: str | Binary = Binary(lob_data) if isinstance(lob_data, bytes) else lob_data
-                        target_cursor.execute(query=update_stmt,
+                        target_cursor.execute(query=update_pg,
                                               vars=(col_data, *pk_vals))
                     case "sqlserver":
                         from pyodbc import Binary
-                        # string data may come from some LOBs (Oracle's NCLOB is a good example)
+                        # string data may come from LOB (Oracle's NCLOB is a good example)
                         col_data: str | Binary = Binary(lob_data) if isinstance(lob_data, bytes) else lob_data
                         target_cursor.execute(sql=update_stmt,
                                               params=(col_data, *pk_vals))
                 # read the next chunk
                 offset += size
                 lob_data = lob.read(offset=offset,
                                     amount=chunk_size)
```

### Comparing `pypomes_db-0.7.5/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.7.6/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.5/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.7.6/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.5/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.7.6/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.5/LICENSE` & `pypomes_db-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.5/pyproject.toml` & `pypomes_db-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.7.5"
+version = "0.7.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

