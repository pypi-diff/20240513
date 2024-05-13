# Comparing `tmp/boosty-0.0.8.tar.gz` & `tmp/boosty-0.0.9.tar.gz`

## Comparing `boosty-0.0.8.tar` & `boosty-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    24409 2020-02-02 00:00:00.000000 boosty-0.0.8/logo.png
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/api/__init__.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/api/api.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/api/auth.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/base.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/comment.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/content.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/donator.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/media_types.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/poll.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/post.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/reactions.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/reply.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/teaser.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/types/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/__init__.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/client.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/json.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/logging.py
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/post.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 boosty-0.0.8/boosty/utils/video.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 boosty-0.0.8/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 boosty-0.0.8/LICENSE
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 boosty-0.0.8/README.md
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 boosty-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 boosty-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    24409 2020-02-02 00:00:00.000000 boosty-0.0.9/logo.png
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/api/__init__.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/api/api.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/api/auth.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/base.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/comment.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/content.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/donator.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/media_types.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/poll.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/post.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/reactions.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/reply.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/teaser.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/types/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/utils/__init__.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/utils/client.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/utils/json.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/utils/logging.py
+-rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/utils/post.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 boosty-0.0.9/boosty/utils/video.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boosty-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 boosty-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 boosty-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 boosty-0.0.9/README.md
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 boosty-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 boosty-0.0.9/PKG-INFO
```

### Comparing `boosty-0.0.8/logo.png` & `boosty-0.0.9/logo.png`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/api/api.py` & `boosty-0.0.9/boosty/api/api.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/api/auth.py` & `boosty-0.0.9/boosty/api/auth.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/types/comment.py` & `boosty-0.0.9/boosty/types/comment.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/types/media_types.py` & `boosty-0.0.9/boosty/types/media_types.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/types/poll.py` & `boosty-0.0.9/boosty/types/poll.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/types/post.py` & `boosty-0.0.9/boosty/types/post.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/types/reply.py` & `boosty-0.0.9/boosty/types/reply.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/types/users.py` & `boosty-0.0.9/boosty/types/users.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/utils/client.py` & `boosty-0.0.9/boosty/utils/client.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/boosty/utils/post.py` & `boosty-0.0.9/boosty/utils/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 from struct import unpack
 from typing import TYPE_CHECKING
 
 from boosty.types.base import schema_strict
-from boosty.types.comment import Comment
 from boosty.types.media_types import Text, Link
 from boosty.utils.json import json
 from pydantic import BaseModel, HttpUrl
 
 if TYPE_CHECKING:
     from boosty.types import Post, Content
+    from boosty.types.comment import Comment
 
 
 # pyrogram/parser/utils.py:19@626a1bd
 # SMP = Supplementary Multilingual Plane: https://en.wikipedia.org/wiki/Plane_(Unicode)#Overview
 SMP_RE = re.compile(r"[\U00010000-\U0010FFFF]")
```

### Comparing `boosty-0.0.8/boosty/utils/video.py` & `boosty-0.0.9/boosty/utils/video.py`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/.gitignore` & `boosty-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/LICENSE` & `boosty-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/README.md` & `boosty-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 from boosty.api import API
 
 api = API()
 response = await api.get_post("boosty", post_id="c9fb8a19-c45e-4602-9942-087c3af28c1b")
 print(response.title)
 # 'Добро пожаловать на борт!'
 ```
-More examples in [examples/](examples/) folder
+More examples in [examples/](https://github.com/barsikus007/boosty/blob/master/examples/) folder
 
 ### TODO for stable release
 - api schema
   - add access levels logic for requests
 - minimal docs
 - useful properties for models
 - merge reply comment with comment model
```

#### html2text {}

```diff
@@ -14,12 +14,12 @@
 "ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff",
 "device_id": "ffffffff-ffff-ffff-ffff-ffffffffffff", "expires_at": 12345678900,
 "refresh_token":
 "ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff" } ```
 Example: ```python from boosty.api import API api = API() response = await
 api.get_post("boosty", post_id="c9fb8a19-c45e-4602-9942-087c3af28c1b") print
 (response.title) # 'ÐÐ¾Ð±ÑÐ¾ Ð¿Ð¾Ð¶Ð°Ð»Ð¾Ð²Ð°ÑÑ Ð½Ð° Ð±Ð¾ÑÑ!' ``` More
-examples in [examples/](examples/) folder ### TODO for stable release - api
-schema - add access levels logic for requests - minimal docs - useful
-properties for models - merge reply comment with comment model - add examples -
-render text - get video url - get comment url - add tests - boosty profile -
-comments - replies
+examples in [examples/](https://github.com/barsikus007/boosty/blob/master/
+examples/) folder ### TODO for stable release - api schema - add access levels
+logic for requests - minimal docs - useful properties for models - merge reply
+comment with comment model - add examples - render text - get video url - get
+comment url - add tests - boosty profile - comments - replies
```

### Comparing `boosty-0.0.8/pyproject.toml` & `boosty-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boosty-0.0.8/PKG-INFO` & `boosty-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boosty
-Version: 0.0.8
+Version: 0.0.9
 Summary: Asynchronous boosty wrapper with some utils
 Project-URL: Documentation, https://github.com/barsikus007/boosty#readme
 Project-URL: Issues, https://github.com/barsikus007/boosty/issues
 Project-URL: Source, https://github.com/barsikus007/boosty
 Author: barsikus007
 License-Expression: MIT
 License-File: LICENSE
@@ -82,15 +82,15 @@
 from boosty.api import API
 
 api = API()
 response = await api.get_post("boosty", post_id="c9fb8a19-c45e-4602-9942-087c3af28c1b")
 print(response.title)
 # 'Добро пожаловать на борт!'
 ```
-More examples in [examples/](examples/) folder
+More examples in [examples/](https://github.com/barsikus007/boosty/blob/master/examples/) folder
 
 ### TODO for stable release
 - api schema
   - add access levels logic for requests
 - minimal docs
 - useful properties for models
 - merge reply comment with comment model
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boosty Version: 0.0.8 Summary: Asynchronous boosty
+Metadata-Version: 2.1 Name: boosty Version: 0.0.9 Summary: Asynchronous boosty
 wrapper with some utils Project-URL: Documentation, https://github.com/
 barsikus007/boosty#readme Project-URL: Issues, https://github.com/barsikus007/
 boosty/issues Project-URL: Source, https://github.com/barsikus007/boosty
 Author: barsikus007 License-Expression: MIT License-File: LICENSE Keywords:
 asyncio,boosty,wrapper Classifier: Development Status :: 4 - Beta Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -30,12 +30,12 @@
 "ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff",
 "device_id": "ffffffff-ffff-ffff-ffff-ffffffffffff", "expires_at": 12345678900,
 "refresh_token":
 "ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff" } ```
 Example: ```python from boosty.api import API api = API() response = await
 api.get_post("boosty", post_id="c9fb8a19-c45e-4602-9942-087c3af28c1b") print
 (response.title) # 'ÐÐ¾Ð±ÑÐ¾ Ð¿Ð¾Ð¶Ð°Ð»Ð¾Ð²Ð°ÑÑ Ð½Ð° Ð±Ð¾ÑÑ!' ``` More
-examples in [examples/](examples/) folder ### TODO for stable release - api
-schema - add access levels logic for requests - minimal docs - useful
-properties for models - merge reply comment with comment model - add examples -
-render text - get video url - get comment url - add tests - boosty profile -
-comments - replies
+examples in [examples/](https://github.com/barsikus007/boosty/blob/master/
+examples/) folder ### TODO for stable release - api schema - add access levels
+logic for requests - minimal docs - useful properties for models - merge reply
+comment with comment model - add examples - render text - get video url - get
+comment url - add tests - boosty profile - comments - replies
```

