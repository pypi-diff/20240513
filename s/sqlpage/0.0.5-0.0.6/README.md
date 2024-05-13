# Comparing `tmp/sqlpage-0.0.5-py3-none-any.whl.zip` & `tmp/sqlpage-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 3614 bytes, number of entries: 8
+Zip file size: 4648 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 24-May-13 06:47 __init__.py
 -rw-r--r--  2.0 unx       69 b- defN 24-May-13 06:21 sqlpage/__init__.py
 -rw-r--r--  2.0 unx      325 b- defN 24-May-11 10:00 sqlpage/models.py
--rw-r--r--  2.0 unx     2348 b- defN 24-May-13 06:33 sqlpage/sqlpage.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      716 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      606 b- defN 24-May-13 06:33 sqlpage-0.0.5.dist-info/RECORD
-8 files, 5232 bytes uncompressed, 2558 bytes compressed:  51.1%
+-rw-r--r--  2.0 unx     3115 b- defN 24-May-13 08:59 sqlpage/sqlpage.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-13 09:14 sqlpage-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-13 09:14 sqlpage-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 09:14 sqlpage-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-May-13 09:14 sqlpage-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      673 b- defN 24-May-13 09:14 sqlpage-0.0.6.dist-info/RECORD
+9 files, 7858 bytes uncompressed, 3494 bytes compressed:  55.5%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
+Filename: __init__.py
+Comment: 
+
 Filename: sqlpage/__init__.py
 Comment: 
 
 Filename: sqlpage/models.py
 Comment: 
 
 Filename: sqlpage/sqlpage.py
 Comment: 
 
-Filename: sqlpage-0.0.5.dist-info/LICENSE
+Filename: sqlpage-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: sqlpage-0.0.5.dist-info/METADATA
+Filename: sqlpage-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: sqlpage-0.0.5.dist-info/WHEEL
+Filename: sqlpage-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: sqlpage-0.0.5.dist-info/top_level.txt
+Filename: sqlpage-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlpage-0.0.5.dist-info/RECORD
+Filename: sqlpage-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlpage/sqlpage.py

```diff
@@ -1,12 +1,13 @@
 import base64
 import json
 from typing import Sequence, Optional, Any
 
 import sqlalchemy
+import sqlmodel
 from sqlalchemy import Row
 from .models import PageData, PageToken
 
 
 def paginate(session, query: sqlalchemy.orm.query.Query, token: str = None, page_size: int = 10) -> PageData[Any]:
     """
     Method to get the result from query in a paginated way.
@@ -20,17 +21,21 @@
     """
     if not token:
         page_token = decode_token(make_first_token(query=query, page_size=page_size))
         page_token.total_count = query.count()
     else:
         page_token = decode_token(token)
 
+        # Since this is the second time call, so check if the page_size if not the default value, and then update it here
+        if page_size != 10:
+            page_token.page_size = page_size
+
     statement = query.limit(page_token.page_size).offset(page_token.offset)
 
-    result: Sequence[Row] = session.exec(statement).all()
+    result: Sequence[Row] = get_result(session, statement)
 
     size = len(result)
 
     total_elements_fetched = page_token.elements_fetched + size
 
     next_page_token: Optional[str] = None
 
@@ -44,14 +49,30 @@
                 offset=page_token.offset + size,
                 elements_fetched=total_elements_fetched,
             )
         )
 
     return PageData(items=result, next_page_token=next_page_token)
 
+
+def get_result(session, statement) -> Sequence[Row]:
+    result: Sequence[Row]
+
+    if isinstance(session, sqlmodel.orm.session.Session):
+        return session.exec(statement).all()
+    elif isinstance(session, sqlalchemy.orm.session.Session):
+        return session.execute(statement).all()
+    else:
+        raise Exception(f"Unsupported session type {type(session)} passed. "
+                        f"Please use session for SQLAlchemy or SQLModel")
+
+def run_on_sqlalchemy(session):
+    isinstance(session, sqlalchemy.orm.session.Session)
+    pass
+
 def make_first_token(query: sqlalchemy.orm.query.Query, page_size: int = 10):
     total_count = query.count()
     page_token: PageToken = PageToken(
         total_count=total_count,
         page_size=page_size,
         remaining=total_count,
         page_num=0,
```

## Comparing `sqlpage-0.0.5.dist-info/LICENSE` & `sqlpage-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

