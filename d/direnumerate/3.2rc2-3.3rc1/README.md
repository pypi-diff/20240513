# Comparing `tmp/direnumerate-3.2rc2.tar.gz` & `tmp/direnumerate-3.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-3.2rc2.tar", last modified: Sat Apr  6 12:18:52 2024, max compression
+gzip compressed data, was "direnumerate-3.3rc1.tar", last modified: Mon May 13 14:33:40 2024, max compression
```

## Comparing `direnumerate-3.2rc2.tar` & `direnumerate-3.3rc1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-06 12:18:52.008754 direnumerate-3.2rc2/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3710 2024-04-06 12:18:52.008754 direnumerate-3.2rc2/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2284 2024-04-06 12:08:44.000000 direnumerate-3.2rc2/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-06 12:18:52.004754 direnumerate-3.2rc2/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    16620 2024-04-06 12:08:38.000000 direnumerate-3.2rc2/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3403 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/getinfo.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/ipcalculator.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/list_urls_accounts.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-06 11:58:06.000000 direnumerate-3.2rc2/direnumerate/version.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-06 12:18:52.008754 direnumerate-3.2rc2/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3710 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-06 11:58:00.000000 direnumerate-3.2rc2/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-06 12:18:52.008754 direnumerate-3.2rc2/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 14:33:40.543056 direnumerate-3.3rc1/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3708 2024-05-13 14:33:40.543056 direnumerate-3.3rc1/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2282 2024-05-13 13:44:29.000000 direnumerate-3.3rc1/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 14:33:40.539056 direnumerate-3.3rc1/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    16991 2024-05-13 14:27:59.000000 direnumerate-3.3rc1/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3401 2024-05-13 14:31:54.000000 direnumerate-3.3rc1/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      229 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/exceptions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/getinfo.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      981 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/help.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/ipcalculator.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       78 2024-05-13 14:25:50.000000 direnumerate-3.3rc1/direnumerate/list_urls_accounts.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-05-13 13:45:37.000000 direnumerate-3.3rc1/direnumerate/version.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      334 2024-05-13 14:28:03.000000 direnumerate-3.3rc1/direnumerate/warning.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 14:33:40.543056 direnumerate-3.3rc1/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3708 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      577 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-05-13 14:32:04.000000 direnumerate-3.3rc1/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-13 14:33:40.543056 direnumerate-3.3rc1/setup.cfg
```

### Comparing `direnumerate-3.2rc2/LICENSE` & `direnumerate-3.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-3.2rc2/PKG-INFO` & `direnumerate-3.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.2rc2
+Version: 3.3rc1
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -29,24 +29,22 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Direnumerate
 
-
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/direnumerate)
 ![PyPI - License](https://img.shields.io/pypi/l/direnumerate)
 [![Documentation Status](https://readthedocs.org/projects/direnumerate/badge/?version=latest)](https://direnumerate.readthedocs.io/en/latest/?badge=latest)
 ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/direnumerate?include_prereleases&link=https%3A%2F%2Fgithub.com%2FJuanBindez%2Fdirenumerate%2Ftags)
 <a href="https://pypi.org/project/direnumerate/"><img src="https://img.shields.io/pypi/v/direnumerate" /></a>
 
 [PDF documentation](https://direnumerate.readthedocs.io/_/downloads/en/latest/pdf/)
 
-
 ## Description
 
 Direnumerate is an open source tool written in Python designed to automate directory and file enumeration on web servers. It is useful for security professionals and system administrators who want to identify hidden resources and assess the security of web applications.
 
 ## Key Features
 
 - Enumeration of directories and files on web servers.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.2rc2 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.3rc1 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.2rc2/README.md` & `direnumerate-3.3rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Direnumerate
 
-
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/direnumerate)
 ![PyPI - License](https://img.shields.io/pypi/l/direnumerate)
 [![Documentation Status](https://readthedocs.org/projects/direnumerate/badge/?version=latest)](https://direnumerate.readthedocs.io/en/latest/?badge=latest)
 ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/direnumerate?include_prereleases&link=https%3A%2F%2Fgithub.com%2FJuanBindez%2Fdirenumerate%2Ftags)
 <a href="https://pypi.org/project/direnumerate/"><img src="https://img.shields.io/pypi/v/direnumerate" /></a>
 
 [PDF documentation](https://direnumerate.readthedocs.io/_/downloads/en/latest/pdf/)
 
-
 ## Description
 
 Direnumerate is an open source tool written in Python designed to automate directory and file enumeration on web servers. It is useful for security professionals and system administrators who want to identify hidden resources and assess the security of web applications.
 
 ## Key Features
 
 - Enumeration of directories and files on web servers.
```

### Comparing `direnumerate-3.2rc2/direnumerate/__init__.py` & `direnumerate-3.3rc1/direnumerate/__init__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.2rc2/direnumerate/__main__.py` & `direnumerate-3.3rc1/direnumerate/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 from direnumerate.createlist import create_wordlist
 from direnumerate.colors import Color
 from direnumerate.banner import *
 from direnumerate.getinfo import get_info_ip
 from direnumerate.ipcalculator import *
 from direnumerate.list_urls_accounts import *
+from direnumerate.help import help_direnumerate
+import direnumerate.exceptions as exception
+from direnumerate.warning import deprecated
 
 
 class DirScan:
     """
     A class for directory scanning.
 
     Attributes:
@@ -44,25 +47,31 @@
         Initializes a DirScan instance.
 
         Args:
             url (str): The URL to scan.
             wordlist_file (str): The path to the wordlist file.
         """
 
-        url_verify = url[4]
+        self.url = url
 
-        if url_verify == ":":
-            url = url.replace("http://", "https://")
-            self.url = url
+        try:
+            url_verify = url[4]
+        
+            if url_verify == ":":
+                url = url.replace("http://", "https://")
+                self.url = url
 
-        elif url_verify == "s":
-            self.url = url
+            elif url_verify == "s":
+                self.url = url
 
-        else:
-            self.url = "https://" + url
+            else:
+                self.url = "https://" + url
+                
+        except IndexError:
+            raise exception.DirenumerateError("[error] expected an argument")
 
     def dir_enum(self, wordlist_file, verbose: bool = False):
         """
         Perform directory enumeration.
 
         This method reads paths from a wordlist file, appends them to the URL, and sends HTTP requests to
         check for the existence of the resources. It prints the results based on the response status code.
@@ -395,18 +404,20 @@
         print(Color.GREEN + "Regional Internet Registry (RIR):" + Color.RESET, informations.get("region"))
         print(Color.GREEN + "IP Block:" + Color.RESET, informations.get("ip_block"))
         
         ic = InfoIp(self.ip)
         ic.ip_calculator(all=True)
 
 
+@deprecated
 class UserScan:
     def __init__(self, user_name):
         self.user_name = user_name
-
+        
+    @deprecated
     def found_users(self):
         for user in list_accounts:
 
             full_url = user + self.user_name
             response = requests.get(full_url)
                         
             if response.status_code == 200:
```

### Comparing `direnumerate-3.2rc2/direnumerate/cli.py` & `direnumerate-3.3rc1/direnumerate/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     fp = FindPattern(file_name_log)
     fp.find_in_log(keyword=key)
 
 
 def show_info_ip(args):
     show_banner()
-    ip_address = args.target
+    ip_address = args.info
 
     ipinfo = InfoIp(ip_address)
     ipinfo.show_info()
 
 
 def main():
     """
```

### Comparing `direnumerate-3.2rc2/direnumerate/createlist.py` & `direnumerate-3.3rc1/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.2rc2/direnumerate/ipcalculator.py` & `direnumerate-3.3rc1/direnumerate/ipcalculator.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.2rc2/direnumerate.egg-info/PKG-INFO` & `direnumerate-3.3rc1/direnumerate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.2rc2
+Version: 3.3rc1
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -29,24 +29,22 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Direnumerate
 
-
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/direnumerate)
 ![PyPI - License](https://img.shields.io/pypi/l/direnumerate)
 [![Documentation Status](https://readthedocs.org/projects/direnumerate/badge/?version=latest)](https://direnumerate.readthedocs.io/en/latest/?badge=latest)
 ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/direnumerate?include_prereleases&link=https%3A%2F%2Fgithub.com%2FJuanBindez%2Fdirenumerate%2Ftags)
 <a href="https://pypi.org/project/direnumerate/"><img src="https://img.shields.io/pypi/v/direnumerate" /></a>
 
 [PDF documentation](https://direnumerate.readthedocs.io/_/downloads/en/latest/pdf/)
 
-
 ## Description
 
 Direnumerate is an open source tool written in Python designed to automate directory and file enumeration on web servers. It is useful for security professionals and system administrators who want to identify hidden resources and assess the security of web applications.
 
 ## Key Features
 
 - Enumeration of directories and files on web servers.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.2rc2 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.3rc1 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.2rc2/pyproject.toml` & `direnumerate-3.3rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "3.2-rc2"
+version = "3.3-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

