# Comparing `tmp/graphemy-1.0.0rc4.tar.gz` & `tmp/graphemy-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphemy-1.0.0rc4.tar", max compression
+gzip compressed data, was "graphemy-1.0.0rc5.tar", max compression
```

## Comparing `graphemy-1.0.0rc4.tar` & `graphemy-1.0.0rc5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1313 2024-05-04 06:58:42.123037 graphemy-1.0.0rc4/graphemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc4/graphemy/database/__init__.py
--rw-r--r--   0        0        0     5638 2024-05-04 06:58:42.139371 graphemy-1.0.0rc4/graphemy/database/operations.py
--rw-r--r--   0        0        0     1639 2024-05-04 06:58:42.140383 graphemy-1.0.0rc4/graphemy/database/utils.py
--rw-r--r--   0        0        0     4319 2024-05-04 06:58:42.142373 graphemy-1.0.0rc4/graphemy/dl.py
--rw-r--r--   0        0        0     3986 2024-05-04 06:58:42.143376 graphemy-1.0.0rc4/graphemy/models.py
--rw-r--r--   0        0        0     8165 2024-05-04 06:58:42.145372 graphemy-1.0.0rc4/graphemy/router.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc4/graphemy/schemas/__init__.py
--rw-r--r--   0        0        0     7785 2024-05-04 06:58:42.146375 graphemy-1.0.0rc4/graphemy/schemas/generators.py
--rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0rc4/graphemy/schemas/models.py
--rw-r--r--   0        0        0     4808 2024-05-04 06:58:42.147374 graphemy-1.0.0rc4/graphemy/setup.py
--rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0rc4/LICENSE
--rw-r--r--   0        0        0     2180 2024-05-04 06:58:42.149376 graphemy-1.0.0rc4/pyproject.toml
--rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0rc4/README.md
--rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 graphemy-1.0.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1313 2024-05-04 06:58:42.123037 graphemy-1.0.0rc5/graphemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc5/graphemy/database/__init__.py
+-rw-r--r--   0        0        0     5638 2024-05-04 06:58:42.139371 graphemy-1.0.0rc5/graphemy/database/operations.py
+-rw-r--r--   0        0        0     1672 2024-05-13 03:58:55.132609 graphemy-1.0.0rc5/graphemy/database/utils.py
+-rw-r--r--   0        0        0     4319 2024-05-04 06:58:42.142373 graphemy-1.0.0rc5/graphemy/dl.py
+-rw-r--r--   0        0        0     3986 2024-05-04 06:58:42.143376 graphemy-1.0.0rc5/graphemy/models.py
+-rw-r--r--   0        0        0     8165 2024-05-04 06:58:42.145372 graphemy-1.0.0rc5/graphemy/router.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc5/graphemy/schemas/__init__.py
+-rw-r--r--   0        0        0     7816 2024-05-13 03:57:43.288280 graphemy-1.0.0rc5/graphemy/schemas/generators.py
+-rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0rc5/graphemy/schemas/models.py
+-rw-r--r--   0        0        0     4808 2024-05-04 06:58:42.147374 graphemy-1.0.0rc5/graphemy/setup.py
+-rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0rc5/LICENSE
+-rw-r--r--   0        0        0     2180 2024-05-13 04:03:19.041963 graphemy-1.0.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0rc5/README.md
+-rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 graphemy-1.0.0rc5/PKG-INFO
```

### Comparing `graphemy-1.0.0rc4/graphemy/__init__.py` & `graphemy-1.0.0rc5/graphemy/__init__.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc4/graphemy/database/operations.py` & `graphemy-1.0.0rc5/graphemy/database/operations.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc4/graphemy/database/utils.py` & `graphemy-1.0.0rc5/graphemy/database/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     if isinstance(id, list):
         filter = []
         for j, key in enumerate(keys):
             f = []
             if None not in key:
                 for k in range(len(id)):
                     f.append(
-                        id[k][1:] if id[k].startswith('_') else  getattr(model, id[k])
+                        id[k] if type(id[k]) == int else id[k][1:] if id[k].startswith('_') else  getattr(model, id[k])
                         == bindparam(
                             f'p{i}_{j}_{k}',
                             literal_execute=not isinstance(key[k], date),
                         )
                     )
                     params[f'p{i}_{j}_{k}'] = key[k]
                 filter.append(and_(*f))
```

### Comparing `graphemy-1.0.0rc4/graphemy/dl.py` & `graphemy-1.0.0rc5/graphemy/dl.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc4/graphemy/models.py` & `graphemy-1.0.0rc5/graphemy/models.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc4/graphemy/router.py` & `graphemy-1.0.0rc5/graphemy/router.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc4/graphemy/schemas/generators.py` & `graphemy-1.0.0rc5/graphemy/schemas/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             strawberry.lazy('graphemy.router'),
         ]
         | None = None,
     ) -> return_type:
         """The dynamically generated DataLoader function."""
         filter_args = vars(filters) if filters else None
         source_value = (
-            [ attr[1:] if attr.startswith('_') else  getattr(self, attr) for attr in field_value.source]
+            [ attr if type(attr) == int else attr[1:] if attr.startswith('_') else  getattr(self, attr) for attr in field_value.source]
             if isinstance(field_value.source, list)
             else getattr(self, field_value.source)
         )
         return await info.context[dl_name].load(
             source_value, {'filters': filter_args}
         )
```

### Comparing `graphemy-1.0.0rc4/graphemy/setup.py` & `graphemy-1.0.0rc5/graphemy/setup.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc4/LICENSE` & `graphemy-1.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc4/pyproject.toml` & `graphemy-1.0.0rc5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphemy"
-version = "1.0.0-rc.4"
+version = "1.0.0-rc.5"
 description = "A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions."
 authors = ["Matheus Doreto <matheusdoreto.md@gmail.com>"]
 readme = "README.md"
 packages = [{include = "graphemy"}]
 homepage = "https://github.com/MDoreto/graphemy"
 documentation = "https://graphemy.readthedocs.io/en/latest/"
 repository = "https://github.com/MDoreto/graphemy"
```

### Comparing `graphemy-1.0.0rc4/README.md` & `graphemy-1.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc4/PKG-INFO` & `graphemy-1.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphemy
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions.
 Home-page: https://github.com/MDoreto/graphemy
 License: MIT
 Author: Matheus Doreto
 Author-email: matheusdoreto.md@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 4 - Beta
```

