# Comparing `tmp/kaizen_cloudcode-0.1.1.tar.gz` & `tmp/kaizen_cloudcode-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaizen_cloudcode-0.1.1.tar", max compression
+gzip compressed data, was "kaizen_cloudcode-0.1.2.tar", max compression
```

## Comparing `kaizen_cloudcode-0.1.1.tar` & `kaizen_cloudcode-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-05-11 23:53:49.165611 kaizen_cloudcode-0.1.1/LICENSE
--rw-r--r--   0        0        0     4135 2024-05-11 23:53:49.165611 kaizen_cloudcode-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/actors/__init__.py
--rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/generator/__init__.py
--rw-r--r--   0        0        0     3075 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/generator/ui.py
--rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/chunker.py
--rw-r--r--   0        0        0     1467 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/general.py
--rw-r--r--   0        0        0     3611 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/output.py
--rw-r--r--   0        0        0     1038 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/parser.py
--rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/integrations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/llms/__init__.py
--rw-r--r--   0        0        0     7183 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/llms/prompts.py
--rw-r--r--   0        0        0     1900 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/llms/provider.py
--rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/reviewer/__init__.py
--rw-r--r--   0        0        0     2969 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/reviewer/code_review.py
--rw-r--r--   0        0        0     1386 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/reviewer/work_summarizer.py
--rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/utils/__init__.py
--rw-r--r--   0        0        0     1103 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/utils/config.py
--rw-r--r--   0        0        0      753 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-13 11:50:49.061935 kaizen_cloudcode-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4135 2024-05-13 11:50:49.061935 kaizen_cloudcode-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/actors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/generator/__init__.py
+-rw-r--r--   0        0        0     3075 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/generator/ui.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/chunker.py
+-rw-r--r--   0        0        0     1467 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/general.py
+-rw-r--r--   0        0        0     3631 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/output.py
+-rw-r--r--   0        0        0     1038 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/helpers/parser.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/llms/__init__.py
+-rw-r--r--   0        0        0     7183 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/llms/prompts.py
+-rw-r--r--   0        0        0     1900 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/llms/provider.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/reviewer/__init__.py
+-rw-r--r--   0        0        0     2969 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/reviewer/code_review.py
+-rw-r--r--   0        0        0     1386 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/reviewer/work_summarizer.py
+-rw-r--r--   0        0        0        0 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/utils/__init__.py
+-rw-r--r--   0        0        0     1677 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/kaizen/utils/config.py
+-rw-r--r--   0        0        0      776 2024-05-13 11:50:49.065935 kaizen_cloudcode-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.2/PKG-INFO
```

### Comparing `kaizen_cloudcode-0.1.1/LICENSE` & `kaizen_cloudcode-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.1/README.md` & `kaizen_cloudcode-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.1/kaizen/generator/ui.py` & `kaizen_cloudcode-0.1.2/kaizen/generator/ui.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.1/kaizen/helpers/general.py` & `kaizen_cloudcode-0.1.2/kaizen/helpers/general.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.1/kaizen/helpers/output.py` & `kaizen_cloudcode-0.1.2/kaizen/helpers/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from playwright.async_api import async_playwright
 from bs4 import BeautifulSoup, Comment
 import asyncio
 import nest_asyncio
 import subprocess
 import os
 import json
-import general
+from kaizen.helpers import general
 
 logger = logging.getLogger(__name__)
 
 
 PR_COLLAPSIBLE_TEMPLATE = """
 <details>
 <summary>{comment}</summary>
```

### Comparing `kaizen_cloudcode-0.1.1/kaizen/helpers/parser.py` & `kaizen_cloudcode-0.1.2/kaizen/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.1/kaizen/llms/prompts.py` & `kaizen_cloudcode-0.1.2/kaizen/llms/prompts.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.1/kaizen/llms/provider.py` & `kaizen_cloudcode-0.1.2/kaizen/llms/provider.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.1/kaizen/reviewer/code_review.py` & `kaizen_cloudcode-0.1.2/kaizen/reviewer/code_review.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.1/kaizen/reviewer/work_summarizer.py` & `kaizen_cloudcode-0.1.2/kaizen/reviewer/work_summarizer.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.1/kaizen/utils/config.py` & `kaizen_cloudcode-0.1.2/kaizen/utils/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 import json
 import os
+from pathlib import Path
 
 
 def get_config():
-    with open("config.json", "r") as f:
-        config_data = json.loads(f.read())
+    # Get the directory of the calling function
+    caller_dir = Path(os.path.dirname(os.path.abspath(__file__)))
+    config_file = f"{caller_dir}/config.json"
+    if Path(config_file).is_file():
+        with open(config_file, "r") as f:
+            config_data = json.loads(f.read())
+    else:
+        config_data = {
+            "language_model": {
+                "provider": "litellm",
+                "enable_observability_logging": False
+            },
+            "github_app": {
+                "check_signature": False,
+                "auto_pr_review": False,
+                "edit_pr_desc": False
+            }
+        }
     return config_data
 
 
 def validate_config_settings(config):
     "Make sure relvant enviorment variables are set"
     if config.get("github_app", {}).get("check_signature", False):
         if not os.environ.get("GITHUB_APP_WEBHOOK_SECRET"):
```

### Comparing `kaizen_cloudcode-0.1.1/pyproject.toml` & `kaizen_cloudcode-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaizen-cloudcode"
-version = "0.1.1"
+version = "0.1.2"
 description = "An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly."
 authors = ["Saurav Panda <saurav.panda@cloudcode.ai>"]
 license = "Apache2.0"
 readme = "README.md"
 packages = [
     { include = "kaizen" }
 ]
@@ -19,12 +19,13 @@
 flake8 = "^7.0.0"
 black = "^24.3.0"
 cryptography = "^42.0.5"
 bs4 = "^0.0.2"
 nest-asyncio = "^1.6.0"
 pytest-playwright = "^0.4.4"
 pip = "^24.0"
+fuzzywuzzy = "^0.18.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kaizen_cloudcode-0.1.1/PKG-INFO` & `kaizen_cloudcode-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaizen-cloudcode
-Version: 0.1.1
+Version: 0.1.2
 Summary: An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly.
 License: Apache2.0
 Author: Saurav Panda
 Author-email: saurav.panda@cloudcode.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=24.3.0,<25.0.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: flake8 (>=7.0.0,<8.0.0)
+Requires-Dist: fuzzywuzzy (>=0.18.0,<0.19.0)
 Requires-Dist: litellm (>=1.34.42,<2.0.0)
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: pip (>=24.0,<25.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: pytest-playwright (>=0.4.4,<0.5.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.1 Summary: An
+Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.2 Summary: An
 intelligent coding companion that accelerates your development workflow by
 providing efficient assistance, enabling you to craft high-quality code more
 rapidly. License: Apache2.0 Author: Saurav Panda Author-email:
 saurav.panda@cloudcode.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: black
 (>=24.3.0,<25.0.0) Requires-Dist: bs4 (>=0.0.2,<0.0.3) Requires-Dist:
 cryptography (>=42.0.5,<43.0.0) Requires-Dist: fastapi (>=0.110.0,<0.111.0)
-Requires-Dist: flake8 (>=7.0.0,<8.0.0) Requires-Dist: litellm
-(>=1.34.42,<2.0.0) Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0) Requires-Dist:
-pip (>=24.0,<25.0) Requires-Dist: pyjwt (>=2.8.0,<3.0.0) Requires-Dist: pytest-
-playwright (>=0.4.4,<0.5.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
-Dist: uvicorn (>=0.29.0,<0.30.0) Description-Content-Type: text/markdown
+Requires-Dist: flake8 (>=7.0.0,<8.0.0) Requires-Dist: fuzzywuzzy
+(>=0.18.0,<0.19.0) Requires-Dist: litellm (>=1.34.42,<2.0.0) Requires-Dist:
+nest-asyncio (>=1.6.0,<2.0.0) Requires-Dist: pip (>=24.0,<25.0) Requires-Dist:
+pyjwt (>=2.8.0,<3.0.0) Requires-Dist: pytest-playwright (>=0.4.4,<0.5.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: uvicorn
+(>=0.29.0,<0.30.0) Description-Content-Type: text/markdown
               _[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_L_i_c_e_n_s_e_:_ _A_G_P_L_-_3_._0_]
 # Kaizen Kaizen is an open-source project that helps teams ensure quality in
 their software delivery by providing a suite of tools for code review, test
 generation, and end-to-end testing. It integrates with your existing code
 repositories and workflows, allowing you to streamline your software
 development process. ## Features ### End-to-End Testing Kaizen generates
 comprehensive end-to-end tests based on your application's code and
```

