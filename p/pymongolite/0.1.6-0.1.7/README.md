# Comparing `tmp/pymongolite-0.1.6.tar.gz` & `tmp/pymongolite-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongolite-0.1.6.tar", max compression
+gzip compressed data, was "pymongolite-0.1.7.tar", max compression
```

## Comparing `pymongolite-0.1.6.tar` & `pymongolite-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     2476 2022-05-05 15:21:05.420637 pymongolite-0.1.6/README.md
--rw-r--r--   0        0        0       59 2022-04-16 17:22:59.839142 pymongolite-0.1.6/pymongolite/__init__.py
--rw-r--r--   0        0        0        0 2022-04-16 17:17:10.838693 pymongolite-0.1.6/pymongolite/backend/__init__.py
--rw-r--r--   0        0        0      788 2022-05-05 21:49:40.001587 pymongolite-0.1.6/pymongolite/backend/command.py
--rw-r--r--   0        0        0       30 2022-04-17 16:42:22.929645 pymongolite-0.1.6/pymongolite/backend/consts.py
--rw-r--r--   0        0        0      131 2022-05-04 14:52:15.464663 pymongolite-0.1.6/pymongolite/backend/document.py
--rw-r--r--   0        0        0     1331 2022-04-29 15:20:58.940073 pymongolite-0.1.6/pymongolite/backend/exceptions.py
--rw-r--r--   0        0        0        0 2022-04-29 14:04:59.674784 pymongolite-0.1.6/pymongolite/backend/execution_engine/__init__.py
--rw-r--r--   0        0        0     2598 2022-05-05 21:49:39.993587 pymongolite-0.1.6/pymongolite/backend/execution_engine/base_engine.py
--rw-r--r--   0        0        0    15835 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/execution_engine/chunked_engine.py
--rw-r--r--   0        0        0      533 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/execution_engine/cursor.py
--rw-r--r--   0        0        0      257 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/execution_engine/exceptions.py
--rw-r--r--   0        0        0     5247 2022-04-29 15:23:53.047568 pymongolite-0.1.6/pymongolite/backend/execution_engine/utils.py
--rw-r--r--   0        0        0        0 2022-05-04 14:52:15.464663 pymongolite-0.1.6/pymongolite/backend/indexing_engine/__init__.py
--rw-r--r--   0        0        0     5316 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/indexing_engine/base_engine.py
--rw-r--r--   0        0        0      454 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/indexing_engine/base_index.py
--rw-r--r--   0        0        0      155 2022-05-04 14:52:15.464663 pymongolite-0.1.6/pymongolite/backend/indexing_engine/index_metadata.py
--rw-r--r--   0        0        0        0 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/indexing_engine/index_types/__init__.py
--rw-r--r--   0        0        0     3045 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/indexing_engine/index_types/sorted_list_basic_index.py
--rw-r--r--   0        0        0     6413 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/indexing_engine/v1_engine.py
--rw-r--r--   0        0        0      979 2022-05-04 14:52:15.464663 pymongolite-0.1.6/pymongolite/backend/objectid.py
--rw-r--r--   0        0        0     3155 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/read_instructions.py
--rw-r--r--   0        0        0     1097 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/session.py
--rw-r--r--   0        0        0        0 2022-04-29 11:39:36.397540 pymongolite-0.1.6/pymongolite/backend/storage_engine/__init__.py
--rw-r--r--   0        0        0     1805 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/storage_engine/base_engine.py
--rw-r--r--   0        0        0     8367 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/storage_engine/files_engine.py
--rw-r--r--   0        0        0      193 2022-04-29 14:41:45.094400 pymongolite-0.1.6/pymongolite/backend/storage_engine/insert_instruction.py
--rw-r--r--   0        0        0      241 2022-04-29 15:19:01.037729 pymongolite-0.1.6/pymongolite/backend/storage_engine/update_instructions.py
--rw-r--r--   0        0        0     5457 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/backend/utils.py
--rw-r--r--   0        0        0     1877 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/client.py
--rw-r--r--   0        0        0     8905 2022-05-05 21:49:39.997587 pymongolite-0.1.6/pymongolite/collection.py
--rw-r--r--   0        0        0     7758 2022-05-05 21:49:40.001587 pymongolite-0.1.6/pymongolite/database.py
--rw-r--r--   0        0        0      384 2022-04-15 10:40:34.719684 pymongolite-0.1.6/pymongolite/exceptions.py
--rw-r--r--   0        0        0      584 2022-05-05 21:56:47.045953 pymongolite-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3413 2022-05-05 21:57:05.504572 pymongolite-0.1.6/setup.py
--rw-r--r--   0        0        0     3077 2022-05-05 21:57:05.504919 pymongolite-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2555 2024-05-13 16:00:25.601472 pymongolite-0.1.7/README.md
+-rw-r--r--   0        0        0       59 2024-05-13 16:00:25.601472 pymongolite-0.1.7/pymongolite/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:00:25.601472 pymongolite-0.1.7/pymongolite/backend/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-13 16:00:25.601472 pymongolite-0.1.7/pymongolite/backend/command.py
+-rw-r--r--   0        0        0      131 2024-05-13 16:00:25.601472 pymongolite-0.1.7/pymongolite/backend/document.py
+-rw-r--r--   0        0        0     1331 2024-05-13 16:00:25.601472 pymongolite-0.1.7/pymongolite/backend/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:00:25.601472 pymongolite-0.1.7/pymongolite/backend/execution_engine/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-13 16:00:25.601472 pymongolite-0.1.7/pymongolite/backend/execution_engine/base_engine.py
+-rw-r--r--   0        0        0    15835 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/execution_engine/chunked_engine.py
+-rw-r--r--   0        0        0      533 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/execution_engine/cursor.py
+-rw-r--r--   0        0        0      257 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/execution_engine/exceptions.py
+-rw-r--r--   0        0        0     5247 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/execution_engine/utils.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/indexing_engine/__init__.py
+-rw-r--r--   0        0        0     5316 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/indexing_engine/base_engine.py
+-rw-r--r--   0        0        0      454 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/indexing_engine/base_index.py
+-rw-r--r--   0        0        0      155 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/indexing_engine/index_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/indexing_engine/index_types/__init__.py
+-rw-r--r--   0        0        0     3073 2024-05-13 16:04:55.581445 pymongolite-0.1.7/pymongolite/backend/indexing_engine/index_types/sorted_list_basic_index.py
+-rw-r--r--   0        0        0     6413 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/indexing_engine/v1_engine.py
+-rw-r--r--   0        0        0      979 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/objectid.py
+-rw-r--r--   0        0        0     3155 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/read_instructions.py
+-rw-r--r--   0        0        0     1097 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/session.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/storage_engine/__init__.py
+-rw-r--r--   0        0        0     1805 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/storage_engine/base_engine.py
+-rw-r--r--   0        0        0     8118 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/storage_engine/files_engine.py
+-rw-r--r--   0        0        0      193 2024-05-13 16:00:25.605472 pymongolite-0.1.7/pymongolite/backend/storage_engine/insert_instruction.py
+-rw-r--r--   0        0        0      241 2024-05-13 16:00:25.609472 pymongolite-0.1.7/pymongolite/backend/storage_engine/update_instructions.py
+-rw-r--r--   0        0        0     5457 2024-05-13 16:00:25.609472 pymongolite-0.1.7/pymongolite/backend/utils.py
+-rw-r--r--   0        0        0     1877 2024-05-13 16:00:25.609472 pymongolite-0.1.7/pymongolite/client.py
+-rw-r--r--   0        0        0     8905 2024-05-13 16:00:25.609472 pymongolite-0.1.7/pymongolite/collection.py
+-rw-r--r--   0        0        0     7758 2024-05-13 16:00:25.609472 pymongolite-0.1.7/pymongolite/database.py
+-rw-r--r--   0        0        0      384 2024-05-13 16:00:25.609472 pymongolite-0.1.7/pymongolite/exceptions.py
+-rw-r--r--   0        0        0      595 2024-05-13 16:09:23.789405 pymongolite-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3504 2024-05-13 16:18:32.869692 pymongolite-0.1.7/setup.py
+-rw-r--r--   0        0        0     3167 2024-05-13 16:18:32.869975 pymongolite-0.1.7/PKG-INFO
```

### Comparing `pymongolite-0.1.6/README.md` & `pymongolite-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # mongolite 
 Lite mongodb engine in python  
 
-[![Run Tests](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml/badge.svg)](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml)  
+[![Run Tests](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml/badge.svg)](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml) 
+[![BringThemBack](https://badge.yehoyada.com/)](https://www.standwithus.com/)  
 
 ---
 
 ```shell
 pip install pymongolite
 ```
```

### Comparing `pymongolite-0.1.6/pymongolite/backend/command.py` & `pymongolite-0.1.7/pymongolite/backend/command.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/exceptions.py` & `pymongolite-0.1.7/pymongolite/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/execution_engine/base_engine.py` & `pymongolite-0.1.7/pymongolite/backend/execution_engine/base_engine.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/execution_engine/chunked_engine.py` & `pymongolite-0.1.7/pymongolite/backend/execution_engine/chunked_engine.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/execution_engine/cursor.py` & `pymongolite-0.1.7/pymongolite/backend/execution_engine/cursor.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/execution_engine/utils.py` & `pymongolite-0.1.7/pymongolite/backend/execution_engine/utils.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/indexing_engine/base_engine.py` & `pymongolite-0.1.7/pymongolite/backend/indexing_engine/base_engine.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/indexing_engine/index_types/sorted_list_basic_index.py` & `pymongolite-0.1.7/pymongolite/backend/indexing_engine/index_types/sorted_list_basic_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 from bisect import bisect_left, bisect_right
 from itertools import chain
 
-from blist import sortedlist
+from sortedcontainers import SortedKeyList as sortedlist
 
 from pymongolite.backend.indexing_engine.base_index import BaseIndex
 
 
 class SortedListBasicIndex(BaseIndex):
     def __init__(self):
         self.__sortedlist = sortedlist(key=lambda t: t[0])
```

### Comparing `pymongolite-0.1.6/pymongolite/backend/indexing_engine/v1_engine.py` & `pymongolite-0.1.7/pymongolite/backend/indexing_engine/v1_engine.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/objectid.py` & `pymongolite-0.1.7/pymongolite/backend/objectid.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/read_instructions.py` & `pymongolite-0.1.7/pymongolite/backend/read_instructions.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/session.py` & `pymongolite-0.1.7/pymongolite/backend/session.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/storage_engine/base_engine.py` & `pymongolite-0.1.7/pymongolite/backend/storage_engine/base_engine.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/backend/storage_engine/files_engine.py` & `pymongolite-0.1.7/pymongolite/backend/storage_engine/files_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,14 @@
     def _root_path(self):
         return Path(self._dirpath).absolute()
 
     def _ensure_root_dir(self):
         if not os.path.exists(self._root_path):
             os.mkdir(self._root_path)
 
-    def create_read_offset(self) -> str:
-        offset = str(uuid4())
-        self._offsets[offset] = 0
-        return offset
-
-    def delete_read_offset(self, offset_id: str) -> bool:
-        return self._offsets.pop(offset_id, None) is not None
-
     def _get_database_path(
         self, database_name: str, error_not_found: bool = False
     ) -> Path:
         if error_not_found and not self.is_database_exists(database_name):
             raise DatabaseNotFound(database_name)
 
         return self._root_path / database_name
```

### Comparing `pymongolite-0.1.6/pymongolite/backend/utils.py` & `pymongolite-0.1.7/pymongolite/backend/utils.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/client.py` & `pymongolite-0.1.7/pymongolite/client.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/collection.py` & `pymongolite-0.1.7/pymongolite/collection.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pymongolite/database.py` & `pymongolite-0.1.7/pymongolite/database.py`

 * *Files identical despite different names*

### Comparing `pymongolite-0.1.6/pyproject.toml` & `pymongolite-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pymongolite"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 readme = "README.md"
 authors = ["yehoyada <yehoyada.sht@gmail.com>"]
 homepage = "https://github.com/hvuhsg/mongolite"
 repository = "https://github.com/hvuhsg/mongolite"
 keywords = ["mongo", "python", "lite", "local", "simple", "pymongo", "NoSQL", "db", "database"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-blist = "^1.3.6"
+sortedcontainers = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 black = "^22.3.0"
 pytest-benchmark = "^3.4.1"
 
 [build-system]
```

### Comparing `pymongolite-0.1.6/setup.py` & `pymongolite-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,21 @@
  'pymongolite.backend.indexing_engine.index_types',
  'pymongolite.backend.storage_engine']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['blist>=1.3.6,<2.0.0']
+['sortedcontainers>=2.4.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'pymongolite',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': '',
-    'long_description': '# mongolite \nLite mongodb engine in python  \n\n[![Run Tests](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml/badge.svg)](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml)  \n\n---\n\n```shell\npip install pymongolite\n```\n\n## Examples\n\n#### simple \n```python\nfrom pymongolite import MongoClient\n\nwith MongoClient(dirpath="~/my_db_dir", database="my_db") as client:\n    db = client.get_default_database()\n    collection = db.get_collection("users")\n\n    collection.insert_one({"name": "yoyo"})\n    collection.update_one({"name": "yoyo"}, {"$set": {"age": 20}})\n    user = collection.find_one({"age": 20})\n    print(user) # -> {"_id": ObjectId(...), "name": "yoyo", "age": 20}\n```\n\n```python\nfrom pymongolite import MongoClient\n\nclient = MongoClient(dirpath="~/my_db_dir", database="my_db")\n\ndb = client.get_default_database()\ncollection = db.get_collection("users")\n\ncollection.insert_one({"name": "yoyo"})\ncollection.update_one({"name": "yoyo"}, {"$set": {"age": 20}})\nuser = collection.find_one({"age": 20})\nprint(user) # -> {"_id": ObjectId(...), "name": "yoyo", "age": 20}\n\nclient.close()\n```\n\n#### Indexes\n```python\nfrom pymongolite import MongoClient\n\nclient = MongoClient(dirpath="~/my_db_dir", database="my_db")\n\ndb = client.get_default_database()\ncollection = db.get_collection("users")\n\n# Make query with name faster\ncollection.create_index({"name": 1})\n\ncollection.insert_one({"name": "yoyo"})\ncollection.update_one({"name": "yoyo"}, {"$set": {"age": 20}})\nuser = collection.find_one({"age": 20})\nprint(user) # -> {"_id": ObjectId(...), "name": "yoyo", "age": 20}\n\nindexes = collection.get_indexes()\nprint(indexes)  # -> [{\'id\': UUID(\'8bb4cac8-ae52-4fff-9e69-9f36a99956cd\'), \'field\': \'age\', \'type\': 1, \'size\': 1}]\n\nclient.close()\n```\n\n## Support\nThe goal of this project is to create sqlite version for mongodb\n\n### For now the library is supporting:\n#### actions:\n- database\n  - create_database\n  - get_database\n  - drop_database\n- collection\n  - create_collection\n  - get_collection\n  - drop_collection\n  - get_collection_names\n- index\n  - create_index\n  - delete_index\n  - get_indexes\n- document\n  - insert_many / insert_one\n  - update_many / update_one\n  - find / find_one\n  - replace_many / replace_one\n#### filtering ops:\n- field matching\n- $eq / $ne\n- $gt / $gte\n- $lt / $lte\n- $not\n- $and / $or / $nor\n- $exists\n- $in / $nin\n#### mutation ops:\n- $set\n- $unset\n- $inc\n- $addToSet\n  - $each\n- $push\n  - $each\n  - $sort\n  - $slice\n- $pull\n',
+    'long_description': '# mongolite \nLite mongodb engine in python  \n\n[![Run Tests](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml/badge.svg)](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml) \n[![BringThemBack](https://badge.yehoyada.com/)](https://www.standwithus.com/)  \n\n---\n\n```shell\npip install pymongolite\n```\n\n## Examples\n\n#### simple \n```python\nfrom pymongolite import MongoClient\n\nwith MongoClient(dirpath="~/my_db_dir", database="my_db") as client:\n    db = client.get_default_database()\n    collection = db.get_collection("users")\n\n    collection.insert_one({"name": "yoyo"})\n    collection.update_one({"name": "yoyo"}, {"$set": {"age": 20}})\n    user = collection.find_one({"age": 20})\n    print(user) # -> {"_id": ObjectId(...), "name": "yoyo", "age": 20}\n```\n\n```python\nfrom pymongolite import MongoClient\n\nclient = MongoClient(dirpath="~/my_db_dir", database="my_db")\n\ndb = client.get_default_database()\ncollection = db.get_collection("users")\n\ncollection.insert_one({"name": "yoyo"})\ncollection.update_one({"name": "yoyo"}, {"$set": {"age": 20}})\nuser = collection.find_one({"age": 20})\nprint(user) # -> {"_id": ObjectId(...), "name": "yoyo", "age": 20}\n\nclient.close()\n```\n\n#### Indexes\n```python\nfrom pymongolite import MongoClient\n\nclient = MongoClient(dirpath="~/my_db_dir", database="my_db")\n\ndb = client.get_default_database()\ncollection = db.get_collection("users")\n\n# Make query with name faster\ncollection.create_index({"name": 1})\n\ncollection.insert_one({"name": "yoyo"})\ncollection.update_one({"name": "yoyo"}, {"$set": {"age": 20}})\nuser = collection.find_one({"age": 20})\nprint(user) # -> {"_id": ObjectId(...), "name": "yoyo", "age": 20}\n\nindexes = collection.get_indexes()\nprint(indexes)  # -> [{\'id\': UUID(\'8bb4cac8-ae52-4fff-9e69-9f36a99956cd\'), \'field\': \'age\', \'type\': 1, \'size\': 1}]\n\nclient.close()\n```\n\n## Support\nThe goal of this project is to create sqlite version for mongodb\n\n### For now the library is supporting:\n#### actions:\n- database\n  - create_database\n  - get_database\n  - drop_database\n- collection\n  - create_collection\n  - get_collection\n  - drop_collection\n  - get_collection_names\n- index\n  - create_index\n  - delete_index\n  - get_indexes\n- document\n  - insert_many / insert_one\n  - update_many / update_one\n  - find / find_one\n  - replace_many / replace_one\n#### filtering ops:\n- field matching\n- $eq / $ne\n- $gt / $gte\n- $lt / $lte\n- $not\n- $and / $or / $nor\n- $exists\n- $in / $nin\n#### mutation ops:\n- $set\n- $unset\n- $inc\n- $addToSet\n  - $each\n- $push\n  - $each\n  - $sort\n  - $slice\n- $pull\n',
     'author': 'yehoyada',
     'author_email': 'yehoyada.sht@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/hvuhsg/mongolite',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pymongolite-0.1.6/PKG-INFO` & `pymongolite-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: pymongolite
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/hvuhsg/mongolite
 Keywords: mongo,python,lite,local,simple,pymongo,NoSQL,db,database
 Author: yehoyada
 Author-email: yehoyada.sht@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: blist (>=1.3.6,<2.0.0)
+Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
 Project-URL: Repository, https://github.com/hvuhsg/mongolite
 Description-Content-Type: text/markdown
 
 # mongolite 
 Lite mongodb engine in python  
 
-[![Run Tests](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml/badge.svg)](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml)  
+[![Run Tests](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml/badge.svg)](https://github.com/hvuhsg/mongolite/actions/workflows/test.yml) 
+[![BringThemBack](https://badge.yehoyada.com/)](https://www.standwithus.com/)  
 
 ---
 
 ```shell
 pip install pymongolite
 ```
```

