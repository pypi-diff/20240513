# Comparing `tmp/sqlpage-0.0.4-py3-none-any.whl.zip` & `tmp/sqlpage-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3609 bytes, number of entries: 8
+Zip file size: 3614 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       69 b- defN 24-May-13 06:21 sqlpage/__init__.py
 -rw-r--r--  2.0 unx      325 b- defN 24-May-11 10:00 sqlpage/models.py
--rw-r--r--  2.0 unx     2348 b- defN 24-May-13 06:31 sqlpage/sqlpage.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-13 06:31 sqlpage-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      716 b- defN 24-May-13 06:31 sqlpage-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-13 06:31 sqlpage-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-13 06:31 sqlpage-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      606 b- defN 24-May-13 06:31 sqlpage-0.0.4.dist-info/RECORD
-8 files, 5232 bytes uncompressed, 2553 bytes compressed:  51.2%
+-rw-r--r--  2.0 unx     2348 b- defN 24-May-13 06:33 sqlpage/sqlpage.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      716 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      606 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/RECORD
+8 files, 5232 bytes uncompressed, 2558 bytes compressed:  51.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: sqlpage/models.py
 Comment: 
 
 Filename: sqlpage/sqlpage.py
 Comment: 
 
-Filename: sqlpage-0.0.4.dist-info/LICENSE
+Filename: sqlpage-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: sqlpage-0.0.4.dist-info/METADATA
+Filename: sqlpage-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: sqlpage-0.0.4.dist-info/WHEEL
+Filename: sqlpage-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: sqlpage-0.0.4.dist-info/top_level.txt
+Filename: sqlpage-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlpage-0.0.4.dist-info/RECORD
+Filename: sqlpage-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlpage/sqlpage.py

```diff
@@ -1,14 +1,14 @@
 import base64
 import json
 from typing import Sequence, Optional, Any
 
 import sqlalchemy
 from sqlalchemy import Row
-from sqlpage import PageData, PageToken
+from .models import PageData, PageToken
 
 
 def paginate(session, query: sqlalchemy.orm.query.Query, token: str = None, page_size: int = 10) -> PageData[Any]:
     """
     Method to get the result from query in a paginated way.
 
     :param session: The DB session
```

## Comparing `sqlpage-0.0.4.dist-info/LICENSE` & `sqlpage-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sqlpage-0.0.4.dist-info/METADATA` & `sqlpage-0.0.5.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlpage
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package to add pagination to a model and return bas64 encoded pagination token
 Author: Prabhu Pant
 Project-URL: Homepage, https://github.com/prabhupant/sqlpage
 Project-URL: Issues, https://github.com/prabhupant/sqlpage/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

