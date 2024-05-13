# Comparing `tmp/pypomes_db-0.7.4.tar.gz` & `tmp/pypomes_db-0.7.5.tar.gz`

## Comparing `pypomes_db-0.7.4.tar` & `pypomes_db-0.7.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    17228 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    17001 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15671 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.5/PKG-INFO
```

### Comparing `pypomes_db-0.7.4/src/pypomes_db/__init__.py` & `pypomes_db-0.7.5/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.4/src/pypomes_db/db_common.py` & `pypomes_db-0.7.5/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.4/src/pypomes_db/db_pomes.py` & `pypomes_db-0.7.5/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.4/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.7.5/src/pypomes_db/migration_pomes.py`

 * *Files 9% similar despite different names*

```diff
@@ -257,31 +257,31 @@
     pks: str = ", ".join(pk_columns)
     sel_stmt: str = f"SELECT {pks}, {source_column} FROM {source_table}"
     if where_clause:
         sel_stmt += f" WHERE {where_clause}"
     blob_index: int = len(pk_columns)
 
     # build the UPDATE query
-    blob_column: str = _db_bind_columns(engine=target_engine,
-                                        columns=[target_column],
-                                        concat=", ",
-                                        start_index=1)
     where_columns: str = _db_bind_columns(engine=target_engine,
                                           columns=pk_columns,
                                           concat=" AND ",
                                           start_index=2)
-    # insert the value
-    update_stmt_1: str = (f"UPDATE {target_table} "
-                          f"SET {blob_column} "
-                          f"WHERE {where_columns}")
-    # append the value
-    update_stmt_2: str = (f"UPDATE {target_table} "
-                          f"SET {blob_column[:len(target_column)+3]}"
-                          f"{target_column} || {blob_column[len(target_column)+3:]} "
-                          f"WHERE {where_columns}")
+    if target_engine == "oracle":
+        update_stmt: str = (f"UPDATE {target_table} "
+                            f"SET {target_column} = empty_blob() "
+                            f"WHERE {where_columns} "
+                            f"RETURNING {target_column} INTO :{len(where_columns)+2}")
+    else:
+        lob_bind: str = _db_bind_columns(engine=target_engine,
+                                         columns=[target_column],
+                                         concat=", ",
+                                         start_index=1)
+        update_stmt: str = (f"UPDATE {target_table} "
+                            f"SET {target_column} = {target_column} || {lob_bind[len(target_column)+3:]} "
+                            f"WHERE {where_columns}")
 
     # log the migration start
     _db_log(logger=logger,
             engine=source_engine,
             stmt=(f"Started migrating LOBs, "
                   f"from {source_engine}.{source_table}.{source_column} "
                   f"to {target_engine}.{target_table}.{target_column}"))
@@ -289,64 +289,60 @@
     # migrate the LOBs
     err_msg: str | None = None
     try:
         source_cursor: Any = curr_source_conn.cursor()
         target_cursor: Any = curr_target_conn.cursor()
 
         # execute the query
-        source_cursor.execute(statement=sel_stmt)
+        # (parameter is 'statement' for oracle, 'query' for postgres, 'sql' for sqlserver)
+        source_cursor.execute(sel_stmt)
 
         # fetch rows
         for row in source_cursor:
 
-            # retrieve the values of the primary key columns (leave blob column out)
+            # retrieve the values of the primary key columns (leave lob column out)
             pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
 
             ora_lob: Any = None
             if target_engine == "oracle":
+                # initialize the LOB column with an empty LOB
                 import oracledb
                 lob_var = target_cursor.var(oracledb.DB_TYPE_BLOB)
-                params: list[tuple] = list(pk_vals)
-                params.append(lob_var)
-                update_ora: str = (f"UPDATE {target_table} "
-                                   f"SET {blob_column} = empty_blob() "
-                                   f"WHERE {where_columns} "
-                                   f"RETURNING {blob_column} INTO :{len(where_columns)+2}")
-                target_cursor.execute(statement=update_ora,
-                                      parameters=params)
+                target_cursor.execute(statement=update_stmt,
+                                      parameters=(*pk_vals, lob_var))
                 ora_lob = lob_var.getValue()
 
+
             # access the blob in chunks and write it to file
             offset: int = 1
-            update_stmt: str = update_stmt_1
             lob: Any = row[blob_index]
             lob_data: bytes | str = lob.read(offset=offset,
                                              amount=chunk_size)
             while lob_data:
+                size: int = len(lob_data)
                 match target_engine:
                     case "mysql":
                         pass
                     case "oracle":
                         ora_lob.write(data=lob_data,
                                       offset=offset)
                     case "postgres":
-                        from psycopg2 import Binary as PgBinary
+                        from psycopg2 import Binary
                         # string data may come from some LOBs (Oracle's NCLOB is a good example)
-                        col_data: Any = PgBinary(lob_data) if isinstance(lob_data, bytes) else lob_data
+                        col_data: str | Binary = Binary(lob_data) if isinstance(lob_data, bytes) else lob_data
                         target_cursor.execute(query=update_stmt,
                                               vars=(col_data, *pk_vals))
                     case "sqlserver":
-                        from pyodbc import Binary as SqlsBinary
+                        from pyodbc import Binary
                         # string data may come from some LOBs (Oracle's NCLOB is a good example)
-                        col_data: Any = SqlsBinary(lob_data) if isinstance(lob_data, bytes) else lob_data
+                        col_data: str | Binary = Binary(lob_data) if isinstance(lob_data, bytes) else lob_data
                         target_cursor.execute(sql=update_stmt,
                                               params=(col_data, *pk_vals))
-                update_stmt = update_stmt_2
                 # read the next chunk
-                offset += len(lob_data)
+                offset += size
                 lob_data = lob.read(offset=offset,
                                     amount=chunk_size)
 
             # increment the LOB migration counter
             result += 1
 
         # close the cursors and commit the transactions
```

### Comparing `pypomes_db-0.7.4/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.7.5/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.4/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.7.5/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.4/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.7.5/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.4/LICENSE` & `pypomes_db-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.7.4/pyproject.toml` & `pypomes_db-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.7.4"
+version = "0.7.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.7.4/PKG-INFO` & `pypomes_db-0.7.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.7.4
+Version: 0.7.5
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

