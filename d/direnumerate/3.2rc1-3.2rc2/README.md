# Comparing `tmp/direnumerate-3.2rc1.tar.gz` & `tmp/direnumerate-3.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-3.2rc1.tar", last modified: Fri Apr  5 18:31:32 2024, max compression
+gzip compressed data, was "direnumerate-3.2rc2.tar", last modified: Sat Apr  6 12:18:52 2024, max compression
```

## Comparing `direnumerate-3.2rc1.tar` & `direnumerate-3.2rc2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-05 18:31:32.019710 direnumerate-3.2rc1/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3858 2024-04-05 18:31:32.019710 direnumerate-3.2rc1/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2432 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-05 18:31:32.015710 direnumerate-3.2rc1/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    16566 2024-04-05 18:29:56.000000 direnumerate-3.2rc1/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3403 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/direnumerate/getinfo.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/direnumerate/ipcalculator.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-05 17:20:17.000000 direnumerate-3.2rc1/direnumerate/list_urls_accounts.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-05 18:30:40.000000 direnumerate-3.2rc1/direnumerate/version.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-05 18:31:32.019710 direnumerate-3.2rc1/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3858 2024-04-05 18:31:31.000000 direnumerate-3.2rc1/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-05 18:31:31.000000 direnumerate-3.2rc1/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-05 18:31:31.000000 direnumerate-3.2rc1/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-05 18:31:31.000000 direnumerate-3.2rc1/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-05 18:31:31.000000 direnumerate-3.2rc1/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-05 18:31:31.000000 direnumerate-3.2rc1/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-05 17:35:20.000000 direnumerate-3.2rc1/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-05 18:31:32.019710 direnumerate-3.2rc1/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-06 12:18:52.008754 direnumerate-3.2rc2/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3710 2024-04-06 12:18:52.008754 direnumerate-3.2rc2/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2284 2024-04-06 12:08:44.000000 direnumerate-3.2rc2/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-06 12:18:52.004754 direnumerate-3.2rc2/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    16620 2024-04-06 12:08:38.000000 direnumerate-3.2rc2/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3403 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/getinfo.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/ipcalculator.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-06 11:55:32.000000 direnumerate-3.2rc2/direnumerate/list_urls_accounts.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-06 11:58:06.000000 direnumerate-3.2rc2/direnumerate/version.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-06 12:18:52.008754 direnumerate-3.2rc2/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3710 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-06 12:18:51.000000 direnumerate-3.2rc2/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-06 11:58:00.000000 direnumerate-3.2rc2/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-06 12:18:52.008754 direnumerate-3.2rc2/setup.cfg
```

### Comparing `direnumerate-3.2rc1/LICENSE` & `direnumerate-3.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-3.2rc1/PKG-INFO` & `direnumerate-3.2rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.2rc1
+Version: 3.2rc2
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -98,28 +98,14 @@
 wordlist = "wordlist.txt"
 
 enum = DirScan(url)
 enum.dir_enum(wordlist)
 ```
 ----------
 
-### User Accont Scan:
-
-```python
-
-from direnumerate import UserScan
-
-user = "username"
-
-found = UserScan(user)
-found.found_users()
-
-```
-----------
-
 ### Port Scan:
 
 ```python
 
 from direnumerate import PortScan
 
 ip = "44.228.249.3"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.2rc1 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.2rc2 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -36,16 +36,14 @@
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
 ---------- ## Command line usage: ### Directory Scan: direnumerate -
 t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
 t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate -log
 test.log -key ERROR ### IP Info: direnumerate -t 8.8.8.8 -i ## Scripts usage:
 ### Directory Scan in Websites: ```python from direnumerate import DirScan url
 = "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan(url)
-enum.dir_enum(wordlist) ``` ---------- ### User Accont Scan: ```python from
-direnumerate import UserScan user = "username" found = UserScan(user)
-found.found_users() ``` ---------- ### Port Scan: ```python from direnumerate
-import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443] scan = PortScan
-(ip) scan.scan_ports(list_ports) ``` ---------- ### Finds patterns in logs:
-```python from direnumerate import FindPatterns log = "test.log" key = "ERROR"
-fp = FindPatterns(log) fp.find_in_log(keyword=key) ``` ### IP Info: ```python
-from direnumerate import InfoIp ip = "8.8.8.8" ipinfo = InfoIp(ip)
-ipinfo.show_info() ``` ----------
+enum.dir_enum(wordlist) ``` ---------- ### Port Scan: ```python from
+direnumerate import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443]
+scan = PortScan(ip) scan.scan_ports(list_ports) ``` ---------- ### Finds
+patterns in logs: ```python from direnumerate import FindPatterns log =
+"test.log" key = "ERROR" fp = FindPatterns(log) fp.find_in_log(keyword=key) ```
+### IP Info: ```python from direnumerate import InfoIp ip = "8.8.8.8" ipinfo =
+InfoIp(ip) ipinfo.show_info() ``` ----------
```

### Comparing `direnumerate-3.2rc1/README.md` & `direnumerate-3.2rc2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -65,28 +65,14 @@
 wordlist = "wordlist.txt"
 
 enum = DirScan(url)
 enum.dir_enum(wordlist)
 ```
 ----------
 
-### User Accont Scan:
-
-```python
-
-from direnumerate import UserScan
-
-user = "username"
-
-found = UserScan(user)
-found.found_users()
-
-```
-----------
-
 ### Port Scan:
 
 ```python
 
 from direnumerate import PortScan
 
 ip = "44.228.249.3"
```

#### html2text {}

```diff
@@ -16,16 +16,14 @@
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
 ---------- ## Command line usage: ### Directory Scan: direnumerate -
 t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
 t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate -log
 test.log -key ERROR ### IP Info: direnumerate -t 8.8.8.8 -i ## Scripts usage:
 ### Directory Scan in Websites: ```python from direnumerate import DirScan url
 = "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan(url)
-enum.dir_enum(wordlist) ``` ---------- ### User Accont Scan: ```python from
-direnumerate import UserScan user = "username" found = UserScan(user)
-found.found_users() ``` ---------- ### Port Scan: ```python from direnumerate
-import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443] scan = PortScan
-(ip) scan.scan_ports(list_ports) ``` ---------- ### Finds patterns in logs:
-```python from direnumerate import FindPatterns log = "test.log" key = "ERROR"
-fp = FindPatterns(log) fp.find_in_log(keyword=key) ``` ### IP Info: ```python
-from direnumerate import InfoIp ip = "8.8.8.8" ipinfo = InfoIp(ip)
-ipinfo.show_info() ``` ----------
+enum.dir_enum(wordlist) ``` ---------- ### Port Scan: ```python from
+direnumerate import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443]
+scan = PortScan(ip) scan.scan_ports(list_ports) ``` ---------- ### Finds
+patterns in logs: ```python from direnumerate import FindPatterns log =
+"test.log" key = "ERROR" fp = FindPatterns(log) fp.find_in_log(keyword=key) ```
+### IP Info: ```python from direnumerate import InfoIp ip = "8.8.8.8" ipinfo =
+InfoIp(ip) ipinfo.show_info() ``` ----------
```

### Comparing `direnumerate-3.2rc1/direnumerate/__init__.py` & `direnumerate-3.2rc2/direnumerate/__init__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.2rc1/direnumerate/__main__.py` & `direnumerate-3.2rc2/direnumerate/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         if url_verify == ":":
             url = url.replace("http://", "https://")
             self.url = url
 
         elif url_verify == "s":
             self.url = url
 
+        else:
+            self.url = "https://" + url
 
     def dir_enum(self, wordlist_file, verbose: bool = False):
         """
         Perform directory enumeration.
 
         This method reads paths from a wordlist file, appends them to the URL, and sends HTTP requests to
         check for the existence of the resources. It prints the results based on the response status code.
```

### Comparing `direnumerate-3.2rc1/direnumerate/cli.py` & `direnumerate-3.2rc2/direnumerate/cli.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.2rc1/direnumerate/createlist.py` & `direnumerate-3.2rc2/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.2rc1/direnumerate/ipcalculator.py` & `direnumerate-3.2rc2/direnumerate/ipcalculator.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.2rc1/direnumerate.egg-info/PKG-INFO` & `direnumerate-3.2rc2/direnumerate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.2rc1
+Version: 3.2rc2
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -98,28 +98,14 @@
 wordlist = "wordlist.txt"
 
 enum = DirScan(url)
 enum.dir_enum(wordlist)
 ```
 ----------
 
-### User Accont Scan:
-
-```python
-
-from direnumerate import UserScan
-
-user = "username"
-
-found = UserScan(user)
-found.found_users()
-
-```
-----------
-
 ### Port Scan:
 
 ```python
 
 from direnumerate import PortScan
 
 ip = "44.228.249.3"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.2rc1 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.2rc2 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -36,16 +36,14 @@
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
 ---------- ## Command line usage: ### Directory Scan: direnumerate -
 t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
 t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate -log
 test.log -key ERROR ### IP Info: direnumerate -t 8.8.8.8 -i ## Scripts usage:
 ### Directory Scan in Websites: ```python from direnumerate import DirScan url
 = "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan(url)
-enum.dir_enum(wordlist) ``` ---------- ### User Accont Scan: ```python from
-direnumerate import UserScan user = "username" found = UserScan(user)
-found.found_users() ``` ---------- ### Port Scan: ```python from direnumerate
-import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443] scan = PortScan
-(ip) scan.scan_ports(list_ports) ``` ---------- ### Finds patterns in logs:
-```python from direnumerate import FindPatterns log = "test.log" key = "ERROR"
-fp = FindPatterns(log) fp.find_in_log(keyword=key) ``` ### IP Info: ```python
-from direnumerate import InfoIp ip = "8.8.8.8" ipinfo = InfoIp(ip)
-ipinfo.show_info() ``` ----------
+enum.dir_enum(wordlist) ``` ---------- ### Port Scan: ```python from
+direnumerate import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443]
+scan = PortScan(ip) scan.scan_ports(list_ports) ``` ---------- ### Finds
+patterns in logs: ```python from direnumerate import FindPatterns log =
+"test.log" key = "ERROR" fp = FindPatterns(log) fp.find_in_log(keyword=key) ```
+### IP Info: ```python from direnumerate import InfoIp ip = "8.8.8.8" ipinfo =
+InfoIp(ip) ipinfo.show_info() ``` ----------
```

### Comparing `direnumerate-3.2rc1/pyproject.toml` & `direnumerate-3.2rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "3.2-rc1"
+version = "3.2-rc2"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

