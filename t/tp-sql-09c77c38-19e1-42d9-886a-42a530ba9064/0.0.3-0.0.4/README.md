# Comparing `tmp/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3.tar.gz` & `tmp/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3.tar", last modified: Fri May 10 18:19:53 2024, max compression
+gzip compressed data, was "tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4.tar", last modified: Mon May 13 13:40:59 2024, max compression
```

## Comparing `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3.tar` & `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 18:19:53.679694 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/
--rw-r--r--   0 test      (1000) test      (1000)      126 2024-05-10 18:19:53.679694 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)      211 2024-05-10 18:19:44.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/pyproject.toml
--rw-rw-r--   0 test      (1000) test      (1000)       38 2024-05-10 18:19:53.679694 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/setup.cfg
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 18:19:53.679694 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 18:19:53.679694 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/tp_sql/
--rw-rw-r--   0 test      (1000) test      (1000)     2860 2024-05-10 16:12:45.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/tp_sql/main.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 18:19:53.679694 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/
--rw-r--r--   0 test      (1000) test      (1000)      126 2024-05-10 18:19:53.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)      404 2024-05-10 18:19:53.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1000) test      (1000)        1 2024-05-10 18:19:53.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1000) test      (1000)       24 2024-05-10 18:19:53.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/requires.txt
--rw-rw-r--   0 test      (1000) test      (1000)        7 2024-05-10 18:19:53.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/top_level.txt
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-10 18:19:53.679694 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/test/
--rw-rw-r--   0 test      (1000) test      (1000)     1655 2024-05-10 18:02:47.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/test/test_sql.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 13:40:59.133195 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/
+-rw-r--r--   0 test      (1000) test      (1000)      155 2024-05-13 13:40:59.133195 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/PKG-INFO
+-rw-rw-r--   0 test      (1000) test      (1000)      232 2024-05-13 13:35:31.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/pyproject.toml
+-rw-rw-r--   0 test      (1000) test      (1000)       38 2024-05-13 13:40:59.133195 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/setup.cfg
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 13:40:59.129195 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 13:40:59.129195 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/tp_sql/
+-rw-rw-r--   0 test      (1000) test      (1000)     2755 2024-05-13 13:34:42.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/tp_sql/main.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 13:40:59.133195 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/
+-rw-r--r--   0 test      (1000) test      (1000)      155 2024-05-13 13:40:59.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1000) test      (1000)      404 2024-05-13 13:40:59.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1000) test      (1000)        1 2024-05-13 13:40:59.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1000) test      (1000)       38 2024-05-13 13:40:59.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/requires.txt
+-rw-rw-r--   0 test      (1000) test      (1000)        7 2024-05-13 13:40:59.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/top_level.txt
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 13:40:59.133195 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/test/
+-rw-rw-r--   0 test      (1000) test      (1000)     1655 2024-05-10 18:02:47.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/test/test_sql.py
```

### Comparing `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/src/tp_sql/main.py` & `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/src/tp_sql/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import psycopg
-from psycopg.errors import SerializationFailure, Error
-from psycopg.rows import namedtuple_row
+from psycopg_pool import ConnectionPool
+
 
 class sql():
     CONFIG_PASSWORD = 'password'
     CONFIG_USER = 'user'
     CONFIG_HOST = 'host'
     CONFIG_PORT = 'port'
     CONFIG_DBNAME = 'db_name'
@@ -57,12 +56,12 @@
         postgresql://localhost:5433
         postgresql://localhost/mydb
         postgresql://user@localhost
         postgresql://user:secret@localhost
         postgresql://other@localhost/otherdb?connect_timeout=10&application_name=myapp
         postgresql://host1:123,host2:456/somedb?target_session_attrs=any&application_name=myapp
         '''
-        self.logger.info(f"SQL: Creasting connection for: {application_name}")
-        conn = psycopg.connect(uri, application_name=application_name, row_factory=namedtuple_row)
-        return conn
+        self.logger.info(f"SQL: Creating connection pool for: {application_name}")
+        pool = ConnectionPool(uri, min_size=2, max_size=5)
+        return pool
```

### Comparing `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.3/test/test_sql.py` & `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.4/test/test_sql.py`

 * *Files identical despite different names*

