# Comparing `tmp/pastperfect-0.1.2.tar.gz` & `tmp/pastperfect-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastperfect-0.1.2.tar", max compression
+gzip compressed data, was "pastperfect-0.2.0.tar", max compression
```

## Comparing `pastperfect-0.1.2.tar` & `pastperfect-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-05-02 19:59:02.121990 pastperfect-0.1.2/LICENSE
--rw-r--r--   0        0        0      915 2024-05-09 15:38:32.222021 pastperfect-0.1.2/README.md
--rw-r--r--   0        0        0     1061 2024-05-10 08:37:39.650394 pastperfect-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       42 2024-05-02 19:59:02.125536 pastperfect-0.1.2/src/pastperfect/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-07 21:04:43.334099 pastperfect-0.1.2/src/pastperfect/events.py
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 pastperfect-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-02 19:59:02.121990 pastperfect-0.2.0/LICENSE
+-rw-r--r--   0        0        0      915 2024-05-09 15:38:32.222021 pastperfect-0.2.0/README.md
+-rw-r--r--   0        0        0     1061 2024-05-13 19:31:15.379331 pastperfect-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-05-02 19:59:02.125536 pastperfect-0.2.0/src/pastperfect/__init__.py
+-rw-r--r--   0        0        0     3034 2024-05-13 19:29:46.512105 pastperfect-0.2.0/src/pastperfect/events.py
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 pastperfect-0.2.0/PKG-INFO
```

### Comparing `pastperfect-0.1.2/LICENSE` & `pastperfect-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pastperfect-0.1.2/README.md` & `pastperfect-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pastperfect-0.1.2/pyproject.toml` & `pastperfect-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "pastperfect"
-version = "0.1.2"
+version = "0.2.0"
 description = "An experience on storing events."
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicense"
 readme = "README.md"
 packages = [{ include = "pastperfect", from = "src" }]
 exclude = ["**/*_test.py"]
```

### Comparing `pastperfect-0.1.2/src/pastperfect/events.py` & `pastperfect-0.2.0/src/pastperfect/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     data: dict
     id: Optional[int] = None
     created_at: Optional[datetime] = field(default_factory=datetime.utcnow)
 
 
 class Events:
     """
-    Events it's a list of events.
+    A list of events.
     """
 
     def __init__(self, db_session: Any):
         super().__init__()
         self._session = db_session
 
     def __len__(self) -> int:
@@ -42,21 +42,35 @@
             data=json.dumps(event.data),
             created_at=event.created_at,
         )
         self._session.execute(prepared_statement)
 
         return self
 
-    def replay(self, handlers):
-        sql_stmt = """SELECT id, name, data, created_at FROM event ORDER BY id ASC"""
-        prepared_statement = text(sql_stmt)
+    def replay(self, handlers, name: Optional[str] = None):
+        """
+        Replays events with the option of filtering by the event name.
+        """
+        if not name:
+            sql_stmt = (
+                """SELECT id, name, data, created_at FROM event ORDER BY id ASC"""
+            )
+            prepared_statement = text(sql_stmt)
+        else:
+            sql_stmt = """SELECT id, name, data, created_at FROM event WHERE name=:name ORDER BY id ASC"""
+            prepared_statement = text(sql_stmt)
+            prepared_statement = prepared_statement.bindparams(name=name)
+
         results = self._session.execute(prepared_statement)
         for row in results:
             e = Event(
-                id=row[0], name=row[1], data=json.loads(row[2]), created_at=row[3]
+                id=row[0],
+                name=row[1],
+                data=json.loads(row[2]),
+                created_at=row[3],
             )
             for handler in handlers:
                 handler(e)
 
     def __getitem__(self, event_id: int) -> Event:
         sql_stmt = """SELECT id, name, data, created_at FROM event WHERE id = :item"""
         prepared_statement = text(sql_stmt)
```

### Comparing `pastperfect-0.1.2/PKG-INFO` & `pastperfect-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastperfect
-Version: 0.1.2
+Version: 0.2.0
 Summary: An experience on storing events.
 License: Unlicense
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

