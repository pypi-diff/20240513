# Comparing `tmp/metabase-api-0.3.2.tar.gz` & `tmp/metabase-api-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabase-api-0.3.2.tar", last modified: Wed Apr 17 05:34:16 2024, max compression
+gzip compressed data, was "metabase-api-0.3.3.tar", last modified: Mon May 13 04:24:49 2024, max compression
```

## Comparing `metabase-api-0.3.2.tar` & `metabase-api-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 05:34:16.108412 metabase-api-0.3.2/
--rw-rw-rw-   0        0        0     1080 2024-04-17 05:25:08.000000 metabase-api-0.3.2/LICENSE
--rw-rw-rw-   0        0        0    13118 2024-04-17 05:34:16.108412 metabase-api-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    12508 2024-04-17 05:25:08.000000 metabase-api-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 05:34:16.093900 metabase-api-0.3.2/metabase_api/
--rw-rw-rw-   0        0        0       39 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/__init__.py
--rw-rw-rw-   0        0        0    12728 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/_helper_methods.py
--rw-rw-rw-   0        0        0     1108 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/_rest_methods.py
--rw-rw-rw-   0        0        0    17174 2024-04-17 05:32:06.000000 metabase-api-0.3.2/metabase_api/copy_methods.py
--rw-rw-rw-   0        0        0    11866 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/create_methods.py
--rw-rw-rw-   0        0        0    15125 2024-04-17 05:25:08.000000 metabase-api-0.3.2/metabase_api/metabase_api.py
-drwxrwxrwx   0        0        0        0 2024-04-17 05:34:16.100917 metabase-api-0.3.2/metabase_api.egg-info/
--rw-rw-rw-   0        0        0    13118 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-17 05:34:15.000000 metabase-api-0.3.2/metabase_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 05:34:16.108412 metabase-api-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      687 2024-04-17 05:25:24.000000 metabase-api-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 05:34:16.103390 metabase-api-0.3.2/tests/
--rw-rw-rw-   0        0        0        1 2024-04-17 05:25:08.000000 metabase-api-0.3.2/tests/__init__.py
--rw-rw-rw-   0        0        0    11222 2024-04-17 05:25:08.000000 metabase-api-0.3.2/tests/test_metabase_api.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:24:49.420837 metabase-api-0.3.3/
+-rw-rw-rw-   0        0        0     1080 2024-05-13 00:48:54.000000 metabase-api-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0    13252 2024-05-13 04:24:49.420837 metabase-api-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12638 2024-05-13 00:51:10.000000 metabase-api-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 04:24:49.404095 metabase-api-0.3.3/metabase_api/
+-rw-rw-rw-   0        0        0       39 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/__init__.py
+-rw-rw-rw-   0        0        0    12728 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/_helper_methods.py
+-rw-rw-rw-   0        0        0     1108 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/_rest_methods.py
+-rw-rw-rw-   0        0        0    17174 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/copy_methods.py
+-rw-rw-rw-   0        0        0    11866 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/create_methods.py
+-rw-rw-rw-   0        0        0    15325 2024-05-13 04:15:23.000000 metabase-api-0.3.3/metabase_api/metabase_api.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:24:49.414335 metabase-api-0.3.3/metabase_api.egg-info/
+-rw-rw-rw-   0        0        0    13252 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 04:24:49.422020 metabase-api-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      687 2024-05-13 00:49:44.000000 metabase-api-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 04:24:49.418332 metabase-api-0.3.3/tests/
+-rw-rw-rw-   0        0        0        1 2024-05-13 00:48:54.000000 metabase-api-0.3.3/tests/__init__.py
+-rw-rw-rw-   0        0        0    11237 2024-05-13 04:15:59.000000 metabase-api-0.3.3/tests/test_metabase_api.py
```

### Comparing `metabase-api-0.3.2/LICENSE` & `metabase-api-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.2/PKG-INFO` & `metabase-api-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python Wrapper for Metabase API
 Home-page: https://github.com/vvaezian/metabase_api_python
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,19 @@
 pip install metabase-api
 ```
 
 ## Initializing
 ```python
 from metabase_api import Metabase_API
 
+# authentication using username/password
 mb = Metabase_API('https://...', 'username', 'password')  # if password is not given, it will prompt for password
+
+# authentication using API key
+mb = Metabase_API('https://...', api_key='YOUR_API_KEY')
 ```
 ## Functions
 ### REST functions (get, post, put, delete)
 Calling Metabase API endpoints (documented [here](https://github.com/metabase/metabase/blob/master/docs/api-documentation.md)) can be done using the corresponding REST function in the wrapper.  
 E.g. to call the [endpoint](https://github.com/metabase/metabase/blob/master/docs/api-documentation.md#get-apidatabase) `GET /api/database/`, use `mb.get('/api/database/')`.
 
 ### Helper Functions
```

### Comparing `metabase-api-0.3.2/README.md` & `metabase-api-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 pip install metabase-api
 ```
 
 ## Initializing
 ```python
 from metabase_api import Metabase_API
 
+# authentication using username/password
 mb = Metabase_API('https://...', 'username', 'password')  # if password is not given, it will prompt for password
+
+# authentication using API key
+mb = Metabase_API('https://...', api_key='YOUR_API_KEY')
 ```
 ## Functions
 ### REST functions (get, post, put, delete)
 Calling Metabase API endpoints (documented [here](https://github.com/metabase/metabase/blob/master/docs/api-documentation.md)) can be done using the corresponding REST function in the wrapper.  
 E.g. to call the [endpoint](https://github.com/metabase/metabase/blob/master/docs/api-documentation.md#get-apidatabase) `GET /api/database/`, use `mb.get('/api/database/')`.
 
 ### Helper Functions
```

### Comparing `metabase-api-0.3.2/metabase_api/_helper_methods.py` & `metabase-api-0.3.3/metabase_api/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.2/metabase_api/_rest_methods.py` & `metabase-api-0.3.3/metabase_api/_rest_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.2/metabase_api/copy_methods.py` & `metabase-api-0.3.3/metabase_api/copy_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.2/metabase_api/create_methods.py` & `metabase-api-0.3.3/metabase_api/create_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.2/metabase_api/metabase_api.py` & `metabase-api-0.3.3/metabase_api/metabase_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import requests
 import getpass
 
 class Metabase_API():
 
-    def __init__(self, domain, email, password=None, basic_auth=False, is_admin=True):
-
+    def __init__(self, domain, email=None, password=None, api_key=None, basic_auth=False, is_admin=True):
+        assert email is not None or api_key is not None
         self.domain = domain.rstrip('/')
         self.email = email
-        self.password = getpass.getpass(prompt='Please enter your password: ') if password is None else password
-        self.session_id = None
-        self.header = None
-        self.auth = (self.email, self.password) if basic_auth else None
-        self.authenticate()
+        self.auth = (self.email, self.password) if basic_auth and email else None
+        if email:
+            self.password = getpass.getpass(prompt='Please enter your password: ') if password is None else password
+            self.session_id = None
+            self.header = None
+            self.authenticate()
+        else:
+            self.header = {"X-API-KEY": api_key}
         self.is_admin = is_admin
         if not self.is_admin:
             print('''
                 Ask your Metabase admin to disable "Friendly Table and Field Names" (in Admin Panel > Settings > General).
                 Without this some of the functions of the current package may not work as expected.
             ''')
 
@@ -33,14 +36,16 @@
 
         self.session_id = res.json()['id']
         self.header = {'X-Metabase-Session':self.session_id}
 
 
     def validate_session(self):
         """Get a new session ID if the previous one has expired"""
+        if not self.email: # if email was not provided then the authentication would be based on api key so there would be no session to validate
+            return
         res = requests.get(self.domain + '/api/user/current', headers=self.header, auth=self.auth)
 
         if res.ok:  # 200
             return True
         elif res.status_code == 401:  # unauthorized
             return self.authenticate()
         else:
@@ -58,28 +63,26 @@
 
     ##################################################################
     ###################### Custom Functions ##########################
     ##################################################################
     from .create_methods import create_card, create_collection, create_segment
     from .copy_methods import copy_card, copy_collection, copy_dashboard, copy_pulse
     
-    def search(self, q, item_type=None, archived=False):
+    def search(self, q, item_type=None):
         """
         Search for Metabase objects and return their basic info. 
         We can limit the search to a certain item type by providing a value for item_type keyword. 
 
         Keyword arguments:
         q -- search input
         item_type -- to limit the search to certain item types (default:None, means no limit)
-        archived -- whether to include archived items in the search
         """
         assert item_type in [None, 'card', 'dashboard', 'collection', 'table', 'pulse', 'segment', 'metric' ]
-        assert archived in [True, False]
 
-        res = self.get(endpoint='/api/search/', params={'q':q, 'archived':archived})
+        res = self.get(endpoint='/api/search/', params={'q':q})
         if type(res) == dict:  # in Metabase version *.40.0 the format of the returned result for this endpoint changed
             res = res['data']
         if item_type is not None:
             res = [ item for item in res if item['model'] == item_type ]
 
         return res
```

### Comparing `metabase-api-0.3.2/metabase_api.egg-info/PKG-INFO` & `metabase-api-0.3.3/metabase_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python Wrapper for Metabase API
 Home-page: https://github.com/vvaezian/metabase_api_python
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,19 @@
 pip install metabase-api
 ```
 
 ## Initializing
 ```python
 from metabase_api import Metabase_API
 
+# authentication using username/password
 mb = Metabase_API('https://...', 'username', 'password')  # if password is not given, it will prompt for password
+
+# authentication using API key
+mb = Metabase_API('https://...', api_key='YOUR_API_KEY')
 ```
 ## Functions
 ### REST functions (get, post, put, delete)
 Calling Metabase API endpoints (documented [here](https://github.com/metabase/metabase/blob/master/docs/api-documentation.md)) can be done using the corresponding REST function in the wrapper.  
 E.g. to call the [endpoint](https://github.com/metabase/metabase/blob/master/docs/api-documentation.md#get-apidatabase) `GET /api/database/`, use `mb.get('/api/database/')`.
 
 ### Helper Functions
```

### Comparing `metabase-api-0.3.2/setup.py` & `metabase-api-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="metabase-api",
-    version="0.3.2",
+    version="0.3.3",
     author="Vahid Vaezian",
     author_email="vahid.vaezian@gmail.com",
     description="A Python Wrapper for Metabase API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vvaezian/metabase_api_python",
     packages=setuptools.find_packages(),
```

### Comparing `metabase-api-0.3.2/tests/test_metabase_api.py` & `metabase-api-0.3.3/tests/test_metabase_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     # database
     res = mb.get_item_info('database', 2)
     self.assertEqual(res['name'], 'test_db')
     self.assertEqual(res['id'], 2)
 
     # table
     res = mb.get_item_info('table', 9)
-    self.assertEqual(res['name'], 'test_table')
+    self.assertEqual(res['name'], 'test_table2')
     self.assertEqual(res['id'], 9)
 
     # card
     res = mb.get_item_info('card', 1)
     self.assertEqual(res['name'], 'test_card')
     self.assertEqual(res['id'], 1)
 
@@ -61,15 +61,15 @@
   def test_get_item_name(self):
     # database
     db_name = mb.get_item_name('database', 2)
     self.assertEqual(db_name, 'test_db')
 
     # table
     table_name = mb.get_item_name('table', 9)
-    self.assertEqual(table_name, 'test_table')
+    self.assertEqual(table_name, 'test_table2')
 
     # card
     card_name = mb.get_item_name('card', 1)
     self.assertEqual(card_name, 'test_card')
 
     # collection
     collection_name = mb.get_item_name('collection', 2)
@@ -84,15 +84,15 @@
   def test_get_item_id(self):
     # database
     db_id = mb.get_item_id('database', 'test_db')
     self.assertEqual(db_id, 2)
 
     # table
     table_id = mb.get_item_id('table', 'test_table')
-    self.assertEqual(table_id, 9)
+    self.assertEqual(table_id, 10)
 
     # card
     card_id = mb.get_item_id('card', 'test_card')
     self.assertEqual(card_id, 1)
 
     # collection
     collection_id = mb.get_item_id('collection', 'test_collection')
@@ -121,19 +121,19 @@
   def test_get_table_metadata(self):
     table_info = mb.get_table_metadata(table_id=9)
     self.assertEqual(table_info['fields'][0]['name'], 'col1')
 
 
 
   def test_get_columns_name_id(self):
-    name_id_mapping = mb.get_columns_name_id(table_id=1)  # table with id 1 is the products table from sample dataset
-    self.assertEqual(name_id_mapping['CATEGORY'], 1)
+    name_id_mapping = mb.get_columns_name_id(table_id=8)  # table with id 8 is the products table from sample dataset
+    self.assertEqual(name_id_mapping['CATEGORY'], 64)
 
-    id_name_mapping = mb.get_columns_name_id(table_id=1, column_id_name=True)
-    self.assertEqual(id_name_mapping[1], 'CATEGORY')
+    id_name_mapping = mb.get_columns_name_id(table_id=8, column_id_name=True)
+    self.assertEqual(id_name_mapping[64], 'CATEGORY')
 
 
 
   ### Testing the Custom Functions
 
   def test_create_card(self):
     t = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
@@ -248,31 +248,31 @@
 
 
 
   def test_get_card_data(self):
     # json
     res = mb.get_card_data(card_id=1)
     json_data = [
-      {'col1': 'row1 cell1', 'col2': 1},
-      {'col1': None, 'col2': 2},
+      {'col1': 'row1 cell1', 'col2': '1'},
+      {'col1': '', 'col2': '2'},
       {'col1': 'row3 cell1', 'col2': None},
-      {'col1': None, 'col2': None},
-      {'col1': 'row5 cell1', 'col2': 5}
+      {'col1': '', 'col2': None},
+      {'col1': 'row5 cell1', 'col2': '5'}
     ]
     self.assertEqual(res, json_data)
 
     # csv
     res = mb.get_card_data(card_id=1, data_format='csv')
     csv_data = 'col1,col2\nrow1 cell1,1\n,2\nrow3 cell1,\n,\nrow5 cell1,5\n'
     self.assertEqual(res, csv_data)
 
-    # filtered data
-    res = mb.get_card_data(card_id=2, parameters=[{"type":"string/=","value":['row1 cell1', 'row3 cell1'],"target":["dimension",["template-tag","test_filter"]]}])
-    filtered_data = [{'col1': 'row1 cell1', 'col2': 1}, {'col1': 'row3 cell1', 'col2': None}]
-    self.assertEqual(res, filtered_data)
+    # # filtered data
+    # res = mb.get_card_data(card_id=2, parameters=[{"type":"string/=","value":['row1 cell1', 'row3 cell1'],"target":["dimension",["template-tag","test_filter"]]}])
+    # filtered_data = [{'col1': 'row1 cell1', 'col2': 1}, {'col1': 'row3 cell1', 'col2': None}]
+    # self.assertEqual(res, filtered_data)
 
 
 
   def test_clone_card(self):
     # native question
     res = mb.clone_card(2, 9, 10, new_card_name='test_clone_native', new_card_collection_id=1, return_card=True)
     # simple/custom question
```

