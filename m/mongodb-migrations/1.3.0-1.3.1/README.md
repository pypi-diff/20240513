# Comparing `tmp/mongodb-migrations-1.3.0.tar.gz` & `tmp/mongodb-migrations-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb-migrations-1.3.0.tar", last modified: Sun Aug 13 20:29:57 2023, max compression
+gzip compressed data, was "mongodb-migrations-1.3.1.tar", last modified: Mon May 13 21:44:42 2024, max compression
```

## Comparing `mongodb-migrations-1.3.0.tar` & `mongodb-migrations-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 darthjoker   (501) staff       (20)        0 2023-08-13 20:29:57.811687 mongodb-migrations-1.3.0/
--rw-r--r--   0 darthjoker   (501) staff       (20)    35134 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.0/LICENSE
--rw-r--r--   0 darthjoker   (501) staff       (20)     4394 2023-08-13 20:29:57.811540 mongodb-migrations-1.3.0/PKG-INFO
--rw-r--r--   0 darthjoker   (501) staff       (20)     3319 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.0/README.md
-drwxr-xr-x   0 darthjoker   (501) staff       (20)        0 2023-08-13 20:29:57.810327 mongodb-migrations-1.3.0/mongodb_migrations/
--rw-r--r--   0 darthjoker   (501) staff       (20)        0 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.0/mongodb_migrations/__init__.py
--rw-r--r--   0 darthjoker   (501) staff       (20)      967 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.0/mongodb_migrations/base.py
--rw-r--r--   0 darthjoker   (501) staff       (20)     7350 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.0/mongodb_migrations/cli.py
--rw-r--r--   0 darthjoker   (501) staff       (20)     6125 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.0/mongodb_migrations/config.py
-drwxr-xr-x   0 darthjoker   (501) staff       (20)        0 2023-08-13 20:29:57.811308 mongodb-migrations-1.3.0/mongodb_migrations.egg-info/
--rw-r--r--   0 darthjoker   (501) staff       (20)     4394 2023-08-13 20:29:57.000000 mongodb-migrations-1.3.0/mongodb_migrations.egg-info/PKG-INFO
--rw-r--r--   0 darthjoker   (501) staff       (20)      434 2023-08-13 20:29:57.000000 mongodb-migrations-1.3.0/mongodb_migrations.egg-info/SOURCES.txt
--rw-r--r--   0 darthjoker   (501) staff       (20)        1 2023-08-13 20:29:57.000000 mongodb-migrations-1.3.0/mongodb_migrations.egg-info/dependency_links.txt
--rw-r--r--   0 darthjoker   (501) staff       (20)      129 2023-08-13 20:29:57.000000 mongodb-migrations-1.3.0/mongodb_migrations.egg-info/entry_points.txt
--rw-r--r--   0 darthjoker   (501) staff       (20)        1 2023-08-13 20:29:57.000000 mongodb-migrations-1.3.0/mongodb_migrations.egg-info/not-zip-safe
--rw-r--r--   0 darthjoker   (501) staff       (20)       35 2023-08-13 20:29:57.000000 mongodb-migrations-1.3.0/mongodb_migrations.egg-info/requires.txt
--rw-r--r--   0 darthjoker   (501) staff       (20)       19 2023-08-13 20:29:57.000000 mongodb-migrations-1.3.0/mongodb_migrations.egg-info/top_level.txt
--rw-r--r--   0 darthjoker   (501) staff       (20)       38 2023-08-13 20:29:57.811733 mongodb-migrations-1.3.0/setup.cfg
--rw-r--r--   0 darthjoker   (501) staff       (20)     2098 2023-08-13 20:20:24.000000 mongodb-migrations-1.3.0/setup.py
+drwxr-xr-x   0 darthjoker   (501) staff       (20)        0 2024-05-13 21:44:42.651192 mongodb-migrations-1.3.1/
+-rw-r--r--   0 darthjoker   (501) staff       (20)    35134 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.1/LICENSE
+-rw-r--r--   0 darthjoker   (501) staff       (20)     4459 2024-05-13 21:44:42.651020 mongodb-migrations-1.3.1/PKG-INFO
+-rw-r--r--   0 darthjoker   (501) staff       (20)     3319 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.1/README.md
+drwxr-xr-x   0 darthjoker   (501) staff       (20)        0 2024-05-13 21:44:42.649987 mongodb-migrations-1.3.1/mongodb_migrations/
+-rw-r--r--   0 darthjoker   (501) staff       (20)        0 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.1/mongodb_migrations/__init__.py
+-rw-r--r--   0 darthjoker   (501) staff       (20)      967 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.1/mongodb_migrations/base.py
+-rw-r--r--   0 darthjoker   (501) staff       (20)     7350 2023-08-13 20:18:33.000000 mongodb-migrations-1.3.1/mongodb_migrations/cli.py
+-rw-r--r--   0 darthjoker   (501) staff       (20)     6128 2024-05-13 21:34:38.000000 mongodb-migrations-1.3.1/mongodb_migrations/config.py
+drwxr-xr-x   0 darthjoker   (501) staff       (20)        0 2024-05-13 21:44:42.650793 mongodb-migrations-1.3.1/mongodb_migrations.egg-info/
+-rw-r--r--   0 darthjoker   (501) staff       (20)     4459 2024-05-13 21:44:42.000000 mongodb-migrations-1.3.1/mongodb_migrations.egg-info/PKG-INFO
+-rw-r--r--   0 darthjoker   (501) staff       (20)      434 2024-05-13 21:44:42.000000 mongodb-migrations-1.3.1/mongodb_migrations.egg-info/SOURCES.txt
+-rw-r--r--   0 darthjoker   (501) staff       (20)        1 2024-05-13 21:44:42.000000 mongodb-migrations-1.3.1/mongodb_migrations.egg-info/dependency_links.txt
+-rw-r--r--   0 darthjoker   (501) staff       (20)      129 2024-05-13 21:44:42.000000 mongodb-migrations-1.3.1/mongodb_migrations.egg-info/entry_points.txt
+-rw-r--r--   0 darthjoker   (501) staff       (20)        1 2023-08-13 20:29:57.000000 mongodb-migrations-1.3.1/mongodb_migrations.egg-info/not-zip-safe
+-rw-r--r--   0 darthjoker   (501) staff       (20)       35 2024-05-13 21:44:42.000000 mongodb-migrations-1.3.1/mongodb_migrations.egg-info/requires.txt
+-rw-r--r--   0 darthjoker   (501) staff       (20)       19 2024-05-13 21:44:42.000000 mongodb-migrations-1.3.1/mongodb_migrations.egg-info/top_level.txt
+-rw-r--r--   0 darthjoker   (501) staff       (20)       38 2024-05-13 21:44:42.651229 mongodb-migrations-1.3.1/setup.cfg
+-rw-r--r--   0 darthjoker   (501) staff       (20)     2098 2024-05-13 21:35:44.000000 mongodb-migrations-1.3.1/setup.py
```

### Comparing `mongodb-migrations-1.3.0/LICENSE` & `mongodb-migrations-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodb-migrations-1.3.0/PKG-INFO` & `mongodb-migrations-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodb-migrations
-Version: 1.3.0
+Version: 1.3.1
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/DoubleCiti/mongodb-migrations
 Author: David Xie
 Author-email: david30xie@gmail.com
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymongo>=3.2.1
+Requires-Dist: configparser>=3.5.0
 
 mongodb-migrations
 ------------------
 
 MongoDB is a great NoSQL and schema-less database, but if already have data in database and you changed data schema, you need a migration tool to update your existing data.
 
 ## How to install
```

### Comparing `mongodb-migrations-1.3.0/README.md` & `mongodb-migrations-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mongodb-migrations-1.3.0/mongodb_migrations/base.py` & `mongodb-migrations-1.3.1/mongodb_migrations/base.py`

 * *Files identical despite different names*

### Comparing `mongodb-migrations-1.3.0/mongodb_migrations/cli.py` & `mongodb-migrations-1.3.1/mongodb_migrations/cli.py`

 * *Files identical despite different names*

### Comparing `mongodb-migrations-1.3.0/mongodb_migrations/config.py` & `mongodb-migrations-1.3.1/mongodb_migrations/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
         try:
             fp = open(self.config_file)
         except Exception:
             pass
         else:
             with fp:
-                self.ini_parser.readfp(fp)
+                self.ini_parser.read_file(fp)
                 if not self.ini_parser.sections():
                     raise Exception("Cannot find %s or it doesn't have sections." % self.config_file)
 
                 self.mongo_url = self.ini_parser.get('mongo', 'url')
                 self.mongo_host = self.ini_parser.get('mongo', 'host')
                 self.mongo_port = self.ini_parser.getint('mongo', 'port')
                 self.mongo_database = self.ini_parser.get('mongo', 'database')
```

### Comparing `mongodb-migrations-1.3.0/mongodb_migrations.egg-info/PKG-INFO` & `mongodb-migrations-1.3.1/mongodb_migrations.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodb-migrations
-Version: 1.3.0
+Version: 1.3.1
 Summary: A database migration tool for MongoDB
 Home-page: https://github.com/DoubleCiti/mongodb-migrations
 Author: David Xie
 Author-email: david30xie@gmail.com
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymongo>=3.2.1
+Requires-Dist: configparser>=3.5.0
 
 mongodb-migrations
 ------------------
 
 MongoDB is a great NoSQL and schema-less database, but if already have data in database and you changed data schema, you need a migration tool to update your existing data.
 
 ## How to install
```

### Comparing `mongodb-migrations-1.3.0/setup.py` & `mongodb-migrations-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         with open('README.md') as f:
             return f.read()
     except IOError:
         return DESCRIPTION
 
 setup(
     name='mongodb-migrations',
-    version='1.3.0',
+    version='1.3.1',
     description=DESCRIPTION,
     long_description=get_read_me(),
     long_description_content_type="text/markdown",
     url='https://github.com/DoubleCiti/mongodb-migrations',
     author='David Xie',
     author_email='david30xie@gmail.com',
     license='GPLv3',
```

