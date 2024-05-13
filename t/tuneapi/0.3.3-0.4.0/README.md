# Comparing `tmp/tuneapi-0.3.3.tar.gz` & `tmp/tuneapi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.3.3.tar", max compression
+gzip compressed data, was "tuneapi-0.4.0.tar", max compression
```

## Comparing `tuneapi-0.3.3.tar` & `tuneapi-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.3.3/LICENSE
--rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.3.3/README.md
--rw-r--r--   0        0        0      712 2024-05-10 05:33:00.755395 tuneapi-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       78 2024-05-10 05:33:03.565847 tuneapi-0.3.3/tuneapi/__init__.py
--rw-r--r--   0        0        0      291 2024-04-23 00:52:16.205178 tuneapi-0.3.3/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     6965 2024-05-10 05:19:42.218444 tuneapi-0.3.3/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     3159 2024-04-25 05:37:07.370133 tuneapi-0.3.3/tuneapi/apis/model_groq.py
--rw-r--r--   0        0        0     3177 2024-04-18 21:08:27.197387 tuneapi-0.3.3/tuneapi/apis/model_mistral.py
--rw-r--r--   0        0        0     6328 2024-04-26 00:29:23.039606 tuneapi-0.3.3/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     5822 2024-04-22 20:41:11.558482 tuneapi-0.3.3/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0     3714 2024-04-23 01:23:26.207221 tuneapi-0.3.3/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      183 2024-04-25 04:12:26.606262 tuneapi-0.3.3/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    15414 2024-04-24 21:00:11.105695 tuneapi-0.3.3/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1076 2024-05-06 20:32:10.727462 tuneapi-0.3.3/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.3.3/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2942 2024-05-06 20:31:58.365454 tuneapi-0.3.3/tuneapi/utils/fs.py
--rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.3.3/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.3.3/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3712 2024-04-07 20:01:31.642080 tuneapi-0.3.3/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.3.3/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4846 2024-04-25 22:30:49.313201 tuneapi-0.3.3/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0     1154 2024-04-30 05:41:11.504281 tuneapi-0.3.3/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.3.3/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5772 2024-04-23 00:48:09.361152 tuneapi-0.3.3/tuneapi/utils/subway.py
--rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.3.3/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 tuneapi-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.4.0/LICENSE
+-rw-r--r--   0        0        0      184 2024-05-13 05:27:01.434096 tuneapi-0.4.0/README.md
+-rw-r--r--   0        0        0      769 2024-05-13 05:24:53.684666 tuneapi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-05-13 05:24:58.687284 tuneapi-0.4.0/tuneapi/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-12 11:13:29.482846 tuneapi-0.4.0/tuneapi/__main__.py
+-rw-r--r--   0        0        0     6012 2024-05-13 05:29:39.964606 tuneapi-0.4.0/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     6965 2024-05-10 05:19:42.218444 tuneapi-0.4.0/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     5009 2024-05-12 10:18:59.196318 tuneapi-0.4.0/tuneapi/apis/model_gemini.py
+-rw-r--r--   0        0        0     3159 2024-05-12 10:20:04.649037 tuneapi-0.4.0/tuneapi/apis/model_groq.py
+-rw-r--r--   0        0        0     3177 2024-04-18 21:08:27.197387 tuneapi-0.4.0/tuneapi/apis/model_mistral.py
+-rw-r--r--   0        0        0     6328 2024-04-26 00:29:23.039606 tuneapi-0.4.0/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     5822 2024-04-22 20:41:11.558482 tuneapi-0.4.0/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0     3714 2024-04-23 01:23:26.207221 tuneapi-0.4.0/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      183 2024-04-25 04:12:26.606262 tuneapi-0.4.0/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    15414 2024-04-24 21:00:11.105695 tuneapi-0.4.0/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1153 2024-05-13 05:29:07.982518 tuneapi-0.4.0/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0      345 2024-05-12 08:34:03.731467 tuneapi-0.4.0/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2987 2024-05-12 08:34:17.889266 tuneapi-0.4.0/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0     1024 2024-05-13 05:28:35.812363 tuneapi-0.4.0/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33527 2024-05-12 08:34:20.152416 tuneapi-0.4.0/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3778 2024-05-12 08:34:28.068601 tuneapi-0.4.0/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2131 2024-05-12 08:34:30.772098 tuneapi-0.4.0/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4883 2024-05-12 08:34:35.753162 tuneapi-0.4.0/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0     1220 2024-05-12 08:34:38.734730 tuneapi-0.4.0/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     2496 2024-05-12 08:34:41.922150 tuneapi-0.4.0/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5838 2024-05-12 08:34:44.657582 tuneapi-0.4.0/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0     1430 2024-05-13 05:28:59.510065 tuneapi-0.4.0/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 tuneapi-0.4.0/PKG-INFO
```

### Comparing `tuneapi-0.3.3/LICENSE` & `tuneapi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.3/pyproject.toml` & `tuneapi-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.3.3"
+version = "0.4.0"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
@@ -17,14 +17,17 @@
 tqdm = "^4.66.1"
 snowflake_id = "1.0.2"
 boto3 = { version = "1.29.6", optional = true }
 
 [tool.poetry.extras]
 boto3 = ["boto3"]
 
+[tool.poetry.scripts]
+tuneapi = "tuneapi.__main__:main"
+
 [tool.poetry.group.dev.dependencies]
 sphinx = "7.2.5"
 sphinx_rtd_theme = "1.3.0"
 poetry = "1.6.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `tuneapi-0.3.3/tuneapi/apis/model_anthropic.py` & `tuneapi-0.4.0/tuneapi/apis/model_anthropic.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.3/tuneapi/apis/model_groq.py` & `tuneapi-0.4.0/tuneapi/apis/model_groq.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.3/tuneapi/apis/model_mistral.py` & `tuneapi-0.4.0/tuneapi/apis/model_mistral.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.3/tuneapi/apis/model_openai.py` & `tuneapi-0.4.0/tuneapi/apis/model_openai.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.3/tuneapi/apis/model_tune.py` & `tuneapi-0.4.0/tuneapi/apis/model_tune.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.3/tuneapi/apis/threads.py` & `tuneapi-0.4.0/tuneapi/apis/threads.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.3/tuneapi/types/chats.py` & `tuneapi-0.4.0/tuneapi/types/chats.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.3.3/tuneapi/utils/__init__.py` & `tuneapi-0.4.0/tuneapi/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright © 2024- Frello Technology Private Limited
+# REMEMBER: nothing from outside tune should be imported in utils
 
 import os
 
 from tuneapi.utils.env import ENV
 from tuneapi.utils.logger import (
     get_logger,
     warning_with_fix,
@@ -35,14 +36,15 @@
     folder,
     joinp,
     load_module_from_path,
     fetch,
 )
 from tuneapi.utils.terminal import (
     hr,
+    color,
 )
 from tuneapi.utils.mime import (
     get_mime_type,
 )
 from tuneapi.utils.misc import (
     SimplerTimes,
     unsafe_exit,
```

### Comparing `tuneapi-0.3.3/tuneapi/utils/fs.py` & `tuneapi-0.4.0/tuneapi/utils/fs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-"""
-File System
-"""
-
 # Copyright © 2024- Frello Technology Private Limited
+# REMEMBER: nothing from outside tune should be imported in utils
 
 import os
 import re
 import sys
 import requests
 from typing import List
 from importlib.util import spec_from_file_location, module_from_spec
```

### Comparing `tuneapi-0.3.3/tuneapi/utils/mime.py` & `tuneapi-0.4.0/tuneapi/utils/mime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright © 2024- Frello Technology Private Limited
+# REMEMBER: nothing from outside tune should be imported in utils
 
 import os
 from functools import lru_cache
 
 MIMETYPES = {
     ".123": "application/vnd.lotus-1-2-3",
     ".3dml": "text/vnd.in3d.3dml",
```

### Comparing `tuneapi-0.3.3/tuneapi/utils/misc.py` & `tuneapi-0.4.0/tuneapi/utils/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright © 2024- Frello Technology Private Limited
+# REMEMBER: nothing from outside tune should be imported in utils
 
 import os
 import base64
 import hashlib
 from cryptography.fernet import Fernet
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
```

### Comparing `tuneapi-0.3.3/tuneapi/utils/networking.py` & `tuneapi-0.4.0/tuneapi/utils/networking.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright © 2024- Frello Technology Private Limited
+# REMEMBER: nothing from outside tune should be imported in utils
 
 import time
 from typing import Any, Dict
 
 from tuneapi.utils.logger import logger
```

### Comparing `tuneapi-0.3.3/tuneapi/utils/parallel.py` & `tuneapi-0.4.0/tuneapi/utils/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-"""
-Parallel processing
-"""
-
 # Copyright © 2024- Frello Technology Private Limited
+# REMEMBER: nothing from outside tune should be imported in utils
 
 import time
 from uuid import uuid4
 from tqdm import trange
 from typing import Any, Dict, List, Union, Tuple, Generator
 
 from concurrent.futures import ThreadPoolExecutor, as_completed, Future
```

### Comparing `tuneapi-0.3.3/tuneapi/utils/randomness.py` & `tuneapi-0.4.0/tuneapi/utils/randomness.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright © 2024- Frello Technology Private Limited
+# REMEMBER: nothing from outside tune should be imported in utils
 
 import random
 import string
 from threading import Lock
 from snowflake import SnowflakeGenerator
```

### Comparing `tuneapi-0.3.3/tuneapi/utils/serdeser.py` & `tuneapi-0.4.0/tuneapi/utils/serdeser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright © 2024- Frello Technology Private Limited
+# REMEMBER: nothing from outside tune should be imported in utils
 
 import os
 import json
 import cloudpickle
 from typing import Any, Dict
 from base64 import b64encode, b64decode
 from google.protobuf.struct_pb2 import Struct
```

### Comparing `tuneapi-0.3.3/tuneapi/utils/subway.py` & `tuneapi-0.4.0/tuneapi/utils/subway.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright © 2024- Frello Technology Private Limited
+# REMEMBER: nothing from outside tune should be imported in utils
 
 from requests import Session
 from pydantic import BaseModel
 from typing import Dict, Any, Optional, Tuple
 
 from tuneapi.utils.logger import logger
 from tuneapi.utils.misc import SimplerTimes
```

### Comparing `tuneapi-0.3.3/PKG-INFO` & `tuneapi-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.3.3
+Version: 0.4.0
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: MIT
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -22,8 +22,11 @@
 Requires-Dist: snowflake_id (==1.0.2)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/NimbleBoxAI/tuneapi
 Description-Content-Type: text/markdown
 
 # Tune API
 
-Package for using 
+Python package for building GenAI apps tightly integrated to Tune Studio.
+
+> The largest utils for any GenAI package ever! See [tuneapi.utils](./tuneapi/utils/__init__.py)
+
```

