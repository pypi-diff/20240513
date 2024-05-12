# Comparing `tmp/asyncwhois-1.1.0.tar.gz` & `tmp/asyncwhois-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncwhois-1.1.0.tar", last modified: Fri Feb  9 18:44:01 2024, max compression
+gzip compressed data, was "asyncwhois-1.1.1.tar", last modified: Sun May 12 23:32:44 2024, max compression
```

## Comparing `asyncwhois-1.1.0.tar` & `asyncwhois-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-02-09 18:44:01.702369 asyncwhois-1.1.0/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1088 2021-10-05 12:08:13.000000 asyncwhois-1.1.0/LICENSE
--rw-rw-r--   0 joe       (1000) joe       (1000)       68 2021-10-05 12:08:13.000000 asyncwhois-1.1.0/MANIFEST.in
--rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-02-09 18:44:01.702369 asyncwhois-1.1.0/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)     8386 2024-02-09 18:43:48.000000 asyncwhois-1.1.0/README.md
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-02-09 18:44:01.702369 asyncwhois-1.1.0/asyncwhois/
--rw-rw-r--   0 joe       (1000) joe       (1000)    24538 2024-02-09 18:43:48.000000 asyncwhois-1.1.0/asyncwhois/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     8253 2024-02-09 18:37:40.000000 asyncwhois-1.1.0/asyncwhois/client.py
--rw-rw-r--   0 joe       (1000) joe       (1000)      166 2023-02-13 17:04:50.000000 asyncwhois-1.1.0/asyncwhois/errors.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    12916 2023-10-12 17:12:26.000000 asyncwhois-1.1.0/asyncwhois/parse.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    14331 2024-02-09 18:37:40.000000 asyncwhois-1.1.0/asyncwhois/parse_rir.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    69492 2024-02-09 18:37:40.000000 asyncwhois-1.1.0/asyncwhois/parse_tld.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     8994 2024-02-09 18:37:40.000000 asyncwhois-1.1.0/asyncwhois/query.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    72914 2024-02-07 19:20:10.000000 asyncwhois-1.1.0/asyncwhois/servers.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-02-09 18:44:01.702369 asyncwhois-1.1.0/asyncwhois.egg-info/
--rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-02-09 18:44:01.000000 asyncwhois-1.1.0/asyncwhois.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      538 2024-02-09 18:44:01.000000 asyncwhois-1.1.0/asyncwhois.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2024-02-09 18:44:01.000000 asyncwhois-1.1.0/asyncwhois.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       62 2024-02-09 18:44:01.000000 asyncwhois-1.1.0/asyncwhois.egg-info/requires.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       11 2024-02-09 18:44:01.000000 asyncwhois-1.1.0/asyncwhois.egg-info/top_level.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)      239 2021-10-05 12:08:13.000000 asyncwhois-1.1.0/pyproject.toml
--rw-rw-r--   0 joe       (1000) joe       (1000)     1047 2024-02-09 18:44:01.702369 asyncwhois-1.1.0/setup.cfg
--rw-rw-r--   0 joe       (1000) joe       (1000)     1784 2024-02-09 18:37:40.000000 asyncwhois-1.1.0/setup.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-02-09 18:44:01.702369 asyncwhois-1.1.0/tests/
--rw-rw-r--   0 joe       (1000) joe       (1000)      676 2024-02-09 18:37:40.000000 asyncwhois-1.1.0/tests/test_not_found.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     1476 2024-02-09 18:37:40.000000 asyncwhois-1.1.0/tests/test_package_methods.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     2741 2023-10-12 17:12:26.000000 asyncwhois-1.1.0/tests/test_parser_methods.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    59474 2024-02-09 18:37:40.000000 asyncwhois-1.1.0/tests/test_parser_output.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     1250 2024-02-09 18:37:40.000000 asyncwhois-1.1.0/tests/test_query.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1088 2021-10-05 12:08:13.000000 asyncwhois-1.1.1/LICENSE
+-rw-rw-r--   0 joe       (1000) joe       (1000)       68 2021-10-05 12:08:13.000000 asyncwhois-1.1.1/MANIFEST.in
+-rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)     8386 2024-02-09 18:43:48.000000 asyncwhois-1.1.1/README.md
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/asyncwhois/
+-rw-rw-r--   0 joe       (1000) joe       (1000)    24538 2024-05-12 23:25:30.000000 asyncwhois-1.1.1/asyncwhois/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     8253 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/asyncwhois/client.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)      166 2023-02-13 17:04:50.000000 asyncwhois-1.1.1/asyncwhois/errors.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    12916 2023-10-12 17:12:26.000000 asyncwhois-1.1.1/asyncwhois/parse.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    14331 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/asyncwhois/parse_rir.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    69492 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/asyncwhois/parse_tld.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     8994 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/asyncwhois/query.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/asyncwhois.egg-info/
+-rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      516 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       62 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       11 2024-05-12 23:32:44.000000 asyncwhois-1.1.1/asyncwhois.egg-info/top_level.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)      239 2021-10-05 12:08:13.000000 asyncwhois-1.1.1/pyproject.toml
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1047 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/setup.cfg
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1784 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/setup.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-12 23:32:44.331663 asyncwhois-1.1.1/tests/
+-rw-rw-r--   0 joe       (1000) joe       (1000)      676 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/tests/test_not_found.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1476 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/tests/test_package_methods.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     2741 2023-10-12 17:12:26.000000 asyncwhois-1.1.1/tests/test_parser_methods.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    59474 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/tests/test_parser_output.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1250 2024-02-09 18:37:40.000000 asyncwhois-1.1.1/tests/test_query.py
```

### Comparing `asyncwhois-1.1.0/LICENSE` & `asyncwhois-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/PKG-INFO` & `asyncwhois-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python utility for querying and parsing WHOIS information for Domains, IPv4s, IPv6s, and AS numbers.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.1.0/README.md` & `asyncwhois-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/asyncwhois/__init__.py` & `asyncwhois-1.1.1/asyncwhois/__init__.py`

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
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 
 def whois(
     search_term: Union[str, ipaddress.IPv4Address, ipaddress.IPv6Address],
     authoritative_only: bool = False,
     ignore_not_found: bool = False,
     proxy_url: str = None,
@@ -64,15 +64,15 @@
     :param ignore_not_found:  If False (default), the `NotFoundError` exception is raised if the query output
         contains "no such domain" language. If True, asyncwhois will not raise `NotFoundError` exceptions.
     :param proxy_url: Optional SOCKS4 or SOCKS5 proxy url (e.g. 'socks5://host:port')
     :param timeout: Connection timeout. Default is 10 seconds.
     :param tldextract_obj: An optional preconfigured instance of `tldextract.TLDExtract` (used for parsing URLs)
     :returns: a tuple containing the WHOIS query text and a dictionary of key values parsed from the text
     """
-    if isinstance(search_term, (ipaddress.IPv6Address, ipaddress.IPv6Address)):
+    if isinstance(search_term, (ipaddress.IPv4Address, ipaddress.IPv6Address)):
         return NumberClient(
             authoritative_only=authoritative_only,
             proxy_url=proxy_url,
             timeout=timeout,
         ).whois(search_term)
     elif isinstance(search_term, str):
         try:
@@ -110,15 +110,15 @@
     :param search_term: Any domain, URL, IPv4, or IPv6
     :param authoritative_only: If False (default), asyncwhois returns the entire WHOIS query chain,
         otherwise if True, only the authoritative response is returned.
     :param whodap_client: An optional preconfigured instance of either an ASN, DNS, IPv4, or IPv6 `whodap` client
     :param tldextract_obj: An optional preconfigured instance of `tldextract.TLDExtract` (used for parsing URLs)
     :returns: a tuple containing the WHOIS query text and a dictionary of key values parsed from the text
     """
-    if isinstance(search_term, (ipaddress.IPv6Address, ipaddress.IPv6Address)):
+    if isinstance(search_term, (ipaddress.IPv4Address, ipaddress.IPv6Address)):
         return NumberClient(
             authoritative_only=authoritative_only,
             whodap_client=whodap_client,
         ).rdap(search_term)
     elif isinstance(search_term, str):
         try:
             search_term = convert_to_ip(search_term)
@@ -157,15 +157,15 @@
     :param ignore_not_found:  If False (default), the `NotFoundError` exception is raised if the query output
         contains "no such domain" language. If True, asyncwhois will not raise `NotFoundError` exceptions.
     :param proxy_url: Optional SOCKS4 or SOCKS5 proxy url (e.g. 'socks5://host:port')
     :param timeout: Connection timeout. Default is 10 seconds.
     :param tldextract_obj: An optional preconfigured instance of `tldextract.TLDExtract` (used for parsing URLs)
     :returns: a tuple containing the WHOIS query text and a dictionary of key values parsed from the text
     """
-    if isinstance(search_term, (ipaddress.IPv6Address, ipaddress.IPv6Address)):
+    if isinstance(search_term, (ipaddress.IPv4Address, ipaddress.IPv6Address)):
         return await NumberClient(
             authoritative_only=authoritative_only,
             proxy_url=proxy_url,
             timeout=timeout,
         ).aio_whois(search_term)
     elif isinstance(search_term, str):
         try:
@@ -203,15 +203,15 @@
     :param search_term: Any domain, URL, IPv4, or IPv6
     :param authoritative_only: If False (default), asyncwhois returns the entire WHOIS query chain,
         otherwise if True, only the authoritative response is returned.
     :param whodap_client: An optional preconfigured instance of either an ASN, DNS, IPv4, or IPv6 `whodap` client
     :param tldextract_obj: An optional preconfigured instance of `tldextract.TLDExtract` (used for parsing URLs)
     :returns: a tuple containing the WHOIS query text and a dictionary of key values parsed from the text
     """
-    if isinstance(search_term, (ipaddress.IPv6Address, ipaddress.IPv6Address)):
+    if isinstance(search_term, (ipaddress.IPv4Address, ipaddress.IPv6Address)):
         return await NumberClient(
             authoritative_only=authoritative_only,
             whodap_client=whodap_client,
         ).aio_rdap(search_term)
     elif isinstance(search_term, str):
         try:
             search_term = convert_to_ip(search_term)
```

### Comparing `asyncwhois-1.1.0/asyncwhois/client.py` & `asyncwhois-1.1.1/asyncwhois/client.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/asyncwhois/parse.py` & `asyncwhois-1.1.1/asyncwhois/parse.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/asyncwhois/parse_rir.py` & `asyncwhois-1.1.1/asyncwhois/parse_rir.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/asyncwhois/parse_tld.py` & `asyncwhois-1.1.1/asyncwhois/parse_tld.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/asyncwhois/query.py` & `asyncwhois-1.1.1/asyncwhois/query.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/asyncwhois.egg-info/PKG-INFO` & `asyncwhois-1.1.1/asyncwhois.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python utility for querying and parsing WHOIS information for Domains, IPv4s, IPv6s, and AS numbers.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.1.0/asyncwhois.egg-info/SOURCES.txt` & `asyncwhois-1.1.1/asyncwhois.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 asyncwhois/__init__.py
 asyncwhois/client.py
 asyncwhois/errors.py
 asyncwhois/parse.py
 asyncwhois/parse_rir.py
 asyncwhois/parse_tld.py
 asyncwhois/query.py
-asyncwhois/servers.py
 asyncwhois.egg-info/PKG-INFO
 asyncwhois.egg-info/SOURCES.txt
 asyncwhois.egg-info/dependency_links.txt
 asyncwhois.egg-info/requires.txt
 asyncwhois.egg-info/top_level.txt
 tests/test_not_found.py
 tests/test_package_methods.py
```

### Comparing `asyncwhois-1.1.0/setup.cfg` & `asyncwhois-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/setup.py` & `asyncwhois-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/tests/test_not_found.py` & `asyncwhois-1.1.1/tests/test_not_found.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/tests/test_package_methods.py` & `asyncwhois-1.1.1/tests/test_package_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/tests/test_parser_methods.py` & `asyncwhois-1.1.1/tests/test_parser_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/tests/test_parser_output.py` & `asyncwhois-1.1.1/tests/test_parser_output.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.0/tests/test_query.py` & `asyncwhois-1.1.1/tests/test_query.py`

 * *Files identical despite different names*

