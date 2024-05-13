# Comparing `tmp/python_sponsorblock-0.1.tar.gz` & `tmp/python_sponsorblock-0.1.dev1.tar.gz`

## Comparing `python_sponsorblock-0.1.tar` & `python_sponsorblock-0.1.dev1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 python_sponsorblock-0.1/python_sponsorblock/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 python_sponsorblock-0.1/python_sponsorblock/_version.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 python_sponsorblock-0.1/python_sponsorblock/constants.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 python_sponsorblock-0.1/python_sponsorblock/exceptions.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 python_sponsorblock-0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 python_sponsorblock-0.1/LICENSE
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 python_sponsorblock-0.1/README.md
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 python_sponsorblock-0.1/pyproject.toml
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 python_sponsorblock-0.1/PKG-INFO
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 python_sponsorblock-0.1.dev1/python_sponsorblock/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 python_sponsorblock-0.1.dev1/python_sponsorblock/_version.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 python_sponsorblock-0.1.dev1/python_sponsorblock/constants.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 python_sponsorblock-0.1.dev1/python_sponsorblock/exceptions.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 python_sponsorblock-0.1.dev1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 python_sponsorblock-0.1.dev1/LICENSE
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 python_sponsorblock-0.1.dev1/README.md
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 python_sponsorblock-0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 python_sponsorblock-0.1.dev1/PKG-INFO
```

### Comparing `python_sponsorblock-0.1/python_sponsorblock/__init__.py` & `python_sponsorblock-0.1.dev1/python_sponsorblock/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from urllib.parse import urlparse, urlunparse, parse_qs, urlencode
 import re
 from typing import Optional, List, Dict, Union, Any, Callable, Set
 import json
 from functools import wraps
 
 from .exceptions import SponsorBlockError, SponsorBlockIdNotFoundError, ReturnDefault
-from .constants import Segment, Category
+from .constants import Segment
 
 
 def error_handling(default: Any) -> Callable:
     def _decorator(func: Callable) -> Callable:
         @wraps(func)
         def _wrapper(self, *args, **kwargs) -> Any:
             nonlocal default
@@ -95,29 +95,18 @@
             data = r.json()
         except json.JSONDecodeError:
             raise exceptions.SponsorBlockConnectionError(f"{r.text} is invalid json.")
         
         return data
         
     @error_handling(default=[])
-    def get_segments(self, video: str, categories: List[Category] = None) -> List[Segment]:
-        """
-        Retrieves the skip segments for a given video.
-
-        Args:
-            video (str): The video identifier.
-            categories (List[Category], optional): A list of categories to filter the skip segments. Defaults to all categories.
-
-        Returns:
-            List[Segment]: A list of skip segments for the given video.
-        """
+    def get_segments(self, video: str) -> List[Segment]:
         video_id = self._get_video_id(video)
-        categories = categories or [c for c in Category]
         
         # build query parameters
         query = {
-            "videoID": video_id,
-            "categories": json.dumps([c.value for c in categories])
+            "videoID": video_id
         }
 
+        print(query)
         r = self._request(method="GET", endpoint="/api/skipSegments?" + urlencode(query))
         return [constants.Segment(**d) for d in r]
```

### Comparing `python_sponsorblock-0.1/python_sponsorblock/constants.py` & `python_sponsorblock-0.1.dev1/python_sponsorblock/constants.py`

 * *Files identical despite different names*

### Comparing `python_sponsorblock-0.1/.gitignore` & `python_sponsorblock-0.1.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `python_sponsorblock-0.1/LICENSE` & `python_sponsorblock-0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_sponsorblock-0.1/README.md` & `python_sponsorblock-0.1.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # Python Sponsorblock
 
-[![status-badge](https://ci.elara.ws/api/badges/61/status.svg)](https://ci.elara.ws/repos/61)
-
 <img src="https://gitea.elara.ws/music-kraken/python-sponsorblock/raw/branch/main/assets/logo.svg" width=300  alt="python-sponsorblock logo"/>
 
 This is a wrapper for the sponsorblock api, enabling you to get the timestamps of sponsor segments from Youtube videos.
 
 ## Installation
 
 ```bash
 # using this gitea repository (recommended)
-pip install --index-url https://gitea.elara.ws/api/packages/music-kraken/pypi/simple/ python-sponsorblock
+pip install --index-url https://gitea.elara.ws/api/packages/music-kraken/pypi/simple/ music-kraken
 ```
 
 ```bash
 # using pip
 pip install python-sponsorblock
 ```
```

### Comparing `python_sponsorblock-0.1/pyproject.toml` & `python_sponsorblock-0.1.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_sponsorblock-0.1/PKG-INFO` & `python_sponsorblock-0.1.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-sponsorblock
-Version: 0.1
+Version: 0.1.dev1
 Summary: This is a wrapper for the sponsorblock api, enabling you to get the timestamps of sponsor segments from youtube videos.
 Author-email: Hazel <hazel_is_cute@proton.me>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,25 +12,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Requires-Dist: requests~=2.31.0
 Description-Content-Type: text/markdown
 
 # Python Sponsorblock
 
-[![status-badge](https://ci.elara.ws/api/badges/61/status.svg)](https://ci.elara.ws/repos/61)
-
 <img src="https://gitea.elara.ws/music-kraken/python-sponsorblock/raw/branch/main/assets/logo.svg" width=300  alt="python-sponsorblock logo"/>
 
 This is a wrapper for the sponsorblock api, enabling you to get the timestamps of sponsor segments from Youtube videos.
 
 ## Installation
 
 ```bash
 # using this gitea repository (recommended)
-pip install --index-url https://gitea.elara.ws/api/packages/music-kraken/pypi/simple/ python-sponsorblock
+pip install --index-url https://gitea.elara.ws/api/packages/music-kraken/pypi/simple/ music-kraken
 ```
 
 ```bash
 # using pip
 pip install python-sponsorblock
 ```
```

