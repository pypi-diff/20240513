# Comparing `tmp/creyPY-1.2.2.tar.gz` & `tmp/creyPY-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creyPY-1.2.2.tar", last modified: Thu Apr 25 17:47:36 2024, max compression
+gzip compressed data, was "creyPY-1.2.3.tar", last modified: Mon May 13 09:23:08 2024, max compression
```

## Comparing `creyPY-1.2.2.tar` & `creyPY-1.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:47:36.069415 creyPY-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 17:47:21.000000 creyPY-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-25 17:47:36.069415 creyPY-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-25 17:47:21.000000 creyPY-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:47:36.065415 creyPY-1.2.2/creyPY/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:47:36.065415 creyPY-1.2.2/creyPY/const/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/const/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/const/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/const/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:47:36.069415 creyPY-1.2.2/creyPY/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/crud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:47:36.069415 creyPY-1.2.2/creyPY/fastapi/db/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/db/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:47:36.069415 creyPY-1.2.2/creyPY/fastapi/models/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:47:36.069415 creyPY-1.2.2/creyPY/fastapi/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-25 17:47:21.000000 creyPY-1.2.2/creyPY/fastapi/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:47:36.069415 creyPY-1.2.2/creyPY.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-25 17:47:36.000000 creyPY-1.2.2/creyPY.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-25 17:47:36.000000 creyPY-1.2.2/creyPY.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:47:36.000000 creyPY-1.2.2/creyPY.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-25 17:47:36.000000 creyPY-1.2.2/creyPY.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 17:47:36.000000 creyPY-1.2.2/creyPY.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:47:36.069415 creyPY-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-25 17:47:21.000000 creyPY-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:23:08.630702 creyPY-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 09:22:54.000000 creyPY-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-13 09:23:08.630702 creyPY-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-13 09:22:54.000000 creyPY-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:23:08.626702 creyPY-1.2.3/creyPY/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:23:08.630702 creyPY-1.2.3/creyPY/const/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/const/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/const/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/const/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:23:08.630702 creyPY-1.2.3/creyPY/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:23:08.630702 creyPY-1.2.3/creyPY/fastapi/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/db/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:23:08.630702 creyPY-1.2.3/creyPY/fastapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:23:08.630702 creyPY-1.2.3/creyPY/fastapi/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-13 09:22:54.000000 creyPY-1.2.3/creyPY/fastapi/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:23:08.630702 creyPY-1.2.3/creyPY.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-13 09:23:08.000000 creyPY-1.2.3/creyPY.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-13 09:23:08.000000 creyPY-1.2.3/creyPY.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:23:08.000000 creyPY-1.2.3/creyPY.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 09:23:08.000000 creyPY-1.2.3/creyPY.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 09:23:08.000000 creyPY-1.2.3/creyPY.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:23:08.630702 creyPY-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-13 09:22:54.000000 creyPY-1.2.3/setup.py
```

### Comparing `creyPY-1.2.2/LICENSE` & `creyPY-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/PKG-INFO` & `creyPY-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creyPY
-Version: 1.2.2
+Version: 1.2.3
 Summary: Collection of my Python and FastAPI shortcuts, snippets etc.
 Home-page: https://github.com/creyD/creyPY
 Author: Conrad Großer
 Author-email: conrad@noah.tech
 License: MIT
 Keywords: creyPY,Python,FastAPI,shortcuts,snippets,utils,personal library
 Platform: any
```

### Comparing `creyPY-1.2.2/README.md` & `creyPY-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/creyPY/const/i18n.py` & `creyPY-1.2.3/creyPY/const/i18n.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/creyPY/const/stripe.py` & `creyPY-1.2.3/creyPY/const/stripe.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/creyPY/fastapi/app.py` & `creyPY-1.2.3/creyPY/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/creyPY/fastapi/crud.py` & `creyPY-1.2.3/creyPY/fastapi/crud.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 from sqlalchemy.orm import Session
 
 from .models.base import Base
 
 T = TypeVar("T", bound=Base)
 
 
-def get_object_or_404(db_class: Type[T], id: UUID | str, db: Session, expunge: bool = False) -> T:
-    obj = db.query(db_class).filter(db_class.id == id).one_or_none()
+def get_object_or_404(
+    db_class: Type[T], id: UUID | str, db: Session, expunge: bool = False, lookup_column: str = "id"
+) -> T:
+    obj = db.query(db_class).filter(getattr(db_class, lookup_column) == id).one_or_none()
     if obj is None:
         raise HTTPException(status_code=404, detail="The object does not exist.")
     if expunge:
         db.expunge(obj)
     return obj
```

### Comparing `creyPY-1.2.2/creyPY/fastapi/db/session.py` & `creyPY-1.2.3/creyPY/fastapi/db/session.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/creyPY/fastapi/models/base.py` & `creyPY-1.2.3/creyPY/fastapi/models/base.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/creyPY/fastapi/order_by.py` & `creyPY-1.2.3/creyPY/fastapi/order_by.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/creyPY/fastapi/pagination.py` & `creyPY-1.2.3/creyPY/fastapi/pagination.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/creyPY/fastapi/testing.py` & `creyPY-1.2.3/creyPY/fastapi/testing.py`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/creyPY.egg-info/PKG-INFO` & `creyPY-1.2.3/creyPY.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creyPY
-Version: 1.2.2
+Version: 1.2.3
 Summary: Collection of my Python and FastAPI shortcuts, snippets etc.
 Home-page: https://github.com/creyD/creyPY
 Author: Conrad Großer
 Author-email: conrad@noah.tech
 License: MIT
 Keywords: creyPY,Python,FastAPI,shortcuts,snippets,utils,personal library
 Platform: any
```

### Comparing `creyPY-1.2.2/creyPY.egg-info/SOURCES.txt` & `creyPY-1.2.3/creyPY.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `creyPY-1.2.2/setup.py` & `creyPY-1.2.3/setup.py`

 * *Files identical despite different names*

