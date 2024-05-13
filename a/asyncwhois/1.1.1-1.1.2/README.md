# Comparing `tmp/asyncwhois-1.1.1.tar.gz` & `tmp/asyncwhois-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncwhois-1.1.1.tar", last modified: Sun May 12 23:32:44 2024, max compression
+gzip compressed data, was "asyncwhois-1.1.2.tar", last modified: Mon May 13 18:13:13 2024, max compression
```

## Comparing `asyncwhois-1.1.1.tar` & `asyncwhois-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1088 2021-10-05 12:08:13.000000 asyncwhois-1.1.1/LICENSE
--rw-rw-r--   0 joe       (1000) joe       (1000)       68 2021-10-05 12:08:13.000000 asyncwhois-1.1.1/MANIFEST.in
--rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)     8386 2024-02-09 18:43:48.000000 asyncwhois-1.1.1/README.md
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/asyncwhois/
--rw-rw-r--   0 joe       (1000) joe       (1000)    24538 2024-05-12 23:25:30.000000 asyncwhois-1.1.1/asyncwhois/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     8253 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/asyncwhois/client.py
--rw-rw-r--   0 joe       (1000) joe       (1000)      166 2023-02-13 17:04:50.000000 asyncwhois-1.1.1/asyncwhois/errors.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    12916 2023-10-12 17:12:26.000000 asyncwhois-1.1.1/asyncwhois/parse.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    14331 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/asyncwhois/parse_rir.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    69492 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/asyncwhois/parse_tld.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     8994 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/asyncwhois/query.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/asyncwhois.egg-info/
--rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      516 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       62 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/requires.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       11 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/top_level.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)      239 2021-10-05 12:08:13.000000 asyncwhois-1.1.1/pyproject.toml
--rw-rw-r--   0 joe       (1000) joe       (1000)     1047 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/setup.cfg
--rw-rw-r--   0 joe       (1000) joe       (1000)     1784 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/setup.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/tests/
--rw-rw-r--   0 joe       (1000) joe       (1000)      676 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/tests/test_not_found.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     1476 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/tests/test_package_methods.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     2741 2023-10-12 17:12:26.000000 asyncwhois-1.1.1/tests/test_parser_methods.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    59474 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/tests/test_parser_output.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     1250 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/tests/test_query.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1088 2021-10-05 12:08:13.000000 asyncwhois-1.1.2/LICENSE
+-rw-rw-r--   0 joe       (1000) joe       (1000)       68 2021-10-05 12:08:13.000000 asyncwhois-1.1.2/MANIFEST.in
+-rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)     8386 2024-02-09 18:43:48.000000 asyncwhois-1.1.2/README.md
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.978112 asyncwhois-1.1.2/asyncwhois/
+-rw-rw-r--   0 joe       (1000) joe       (1000)    24538 2024-05-13 18:13:00.000000 asyncwhois-1.1.2/asyncwhois/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     8253 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/asyncwhois/client.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)      166 2023-02-13 17:04:50.000000 asyncwhois-1.1.2/asyncwhois/errors.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    12916 2023-10-12 17:12:26.000000 asyncwhois-1.1.2/asyncwhois/parse.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    14331 2024-05-13 17:56:47.000000 asyncwhois-1.1.2/asyncwhois/parse_rir.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    69492 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/asyncwhois/parse_tld.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     8994 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/asyncwhois/query.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/asyncwhois/servers/
+-rw-rw-r--   0 joe       (1000) joe       (1000)    46078 2024-05-12 23:25:10.000000 asyncwhois-1.1.2/asyncwhois/servers/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    15501 2024-05-12 23:25:10.000000 asyncwhois-1.1.2/asyncwhois/servers/ipv4.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/asyncwhois.egg-info/
+-rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      574 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       62 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       11 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/top_level.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)      239 2021-10-05 12:08:13.000000 asyncwhois-1.1.2/pyproject.toml
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1047 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/setup.cfg
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1806 2024-05-13 17:58:59.000000 asyncwhois-1.1.2/setup.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/tests/
+-rw-rw-r--   0 joe       (1000) joe       (1000)      676 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/tests/test_not_found.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1476 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/tests/test_package_methods.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     2741 2023-10-12 17:12:26.000000 asyncwhois-1.1.2/tests/test_parser_methods.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    59474 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/tests/test_parser_output.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1250 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/tests/test_query.py
```

### Comparing `asyncwhois-1.1.1/LICENSE` & `asyncwhois-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/PKG-INFO` & `asyncwhois-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python utility for querying and parsing WHOIS information for Domains, IPv4s, IPv6s, and AS numbers.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.1.1/README.md` & `asyncwhois-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/asyncwhois/__init__.py` & `asyncwhois-1.1.2/asyncwhois/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "DomainClient",
     "NumberClient",
     "NotFoundError",
     "WhoIsError",
     "GeneralError",
     "QueryError",
 ]
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 
 def whois(
     search_term: Union[str, ipaddress.IPv4Address, ipaddress.IPv6Address],
     authoritative_only: bool = False,
     ignore_not_found: bool = False,
     proxy_url: str = None,
```

### Comparing `asyncwhois-1.1.1/asyncwhois/client.py` & `asyncwhois-1.1.2/asyncwhois/client.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/asyncwhois/parse.py` & `asyncwhois-1.1.2/asyncwhois/parse.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/asyncwhois/parse_rir.py` & `asyncwhois-1.1.2/asyncwhois/parse_rir.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/asyncwhois/parse_tld.py` & `asyncwhois-1.1.2/asyncwhois/parse_tld.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/asyncwhois/query.py` & `asyncwhois-1.1.2/asyncwhois/query.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/asyncwhois.egg-info/PKG-INFO` & `asyncwhois-1.1.2/asyncwhois.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python utility for querying and parsing WHOIS information for Domains, IPv4s, IPv6s, and AS numbers.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.1.1/asyncwhois.egg-info/SOURCES.txt` & `asyncwhois-1.1.2/asyncwhois.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -12,12 +12,14 @@
 asyncwhois/parse_tld.py
 asyncwhois/query.py
 asyncwhois.egg-info/PKG-INFO
 asyncwhois.egg-info/SOURCES.txt
 asyncwhois.egg-info/dependency_links.txt
 asyncwhois.egg-info/requires.txt
 asyncwhois.egg-info/top_level.txt
+asyncwhois/servers/__init__.py
+asyncwhois/servers/ipv4.py
 tests/test_not_found.py
 tests/test_package_methods.py
 tests/test_parser_methods.py
 tests/test_parser_output.py
 tests/test_query.py
```

### Comparing `asyncwhois-1.1.1/setup.cfg` & `asyncwhois-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/setup.py` & `asyncwhois-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,11 +43,11 @@
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development",
         "Topic :: Security",
         "Framework :: AsyncIO",
     ],
     url="https://github.com/pogzyb/asyncwhois",
-    packages=["asyncwhois"],
+    packages=["asyncwhois", "asyncwhois.servers"],
     package_dir={"asyncwhois": "asyncwhois"},
     python_requires=">=3.9",
 )
```

### Comparing `asyncwhois-1.1.1/tests/test_not_found.py` & `asyncwhois-1.1.2/tests/test_not_found.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/tests/test_package_methods.py` & `asyncwhois-1.1.2/tests/test_package_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/tests/test_parser_methods.py` & `asyncwhois-1.1.2/tests/test_parser_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/tests/test_parser_output.py` & `asyncwhois-1.1.2/tests/test_parser_output.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.1/tests/test_query.py` & `asyncwhois-1.1.2/tests/test_query.py`

 * *Files identical despite different names*

