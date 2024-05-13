# Comparing `tmp/cdnmon-0.2.6.tar.gz` & `tmp/cdnmon-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdnmon-0.2.6.tar", max compression
+gzip compressed data, was "cdnmon-0.3.1.tar", max compression
```

## Comparing `cdnmon-0.2.6.tar` & `cdnmon-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      960 2023-06-06 08:29:49.673136 cdnmon-0.2.6/README.md
--rw-r--r--   0        0        0     1531 2023-06-06 08:29:49.673136 cdnmon-0.2.6/cdnmon/__init__.py
--rw-r--r--   0        0        0      404 2023-06-06 08:29:49.673136 cdnmon-0.2.6/cdnmon/config.py
--rw-r--r--   0        0        0       40 2023-06-06 08:29:49.673136 cdnmon-0.2.6/cdnmon/settings.py
--rw-r--r--   0        0        0      426 2023-06-06 08:29:49.673136 cdnmon-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 cdnmon-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-13 15:07:35.205142 cdnmon-0.3.1/README.md
+-rw-r--r--   0        0        0     1481 2024-05-13 15:07:35.205142 cdnmon-0.3.1/cdnmon/__init__.py
+-rw-r--r--   0        0        0      404 2024-05-13 15:07:35.205142 cdnmon-0.3.1/cdnmon/config.py
+-rw-r--r--   0        0        0       40 2024-05-13 15:07:35.205142 cdnmon-0.3.1/cdnmon/settings.py
+-rw-r--r--   0        0        0      426 2024-05-13 15:07:35.205142 cdnmon-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 cdnmon-0.3.1/PKG-INFO
```

### Comparing `cdnmon-0.2.6/PKG-INFO` & `cdnmon-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: cdnmon
-Version: 0.2.6
+Version: 0.3.1
 Summary: 
 Author: Yihang Wang
 Author-email: wangyihanger@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Introduction
@@ -50,20 +51,26 @@
 ### Get the IP ranges of a specific CDN
 
 ```python
 from cdnmon import Endpoint
 
 endpoint = Endpoint(access_token="")
 cdn = endpoint.get_cdn(name="cloudflare")
-latest_ipv4_networks = cdn.ipv4_networks[-1]
-for latest_ipv4_network in cdn.latest_ipv4_networks:
-    print(latest_ipv4_network.networks)
-    print(latest_ipv4_network.updated_at)
-    print(latest_ipv4_network.source)
+latest_ipv4_networks = cdn["ipv4_networks"][-1]
+print("Updated at:", latest_ipv4_networks["updated_at"])
+print("Source:", latest_ipv4_networks["source"])
+print("Networks:")
+for latest_ipv4_network in latest_ipv4_networks["networks"]:
+    print(latest_ipv4_network)
 ```
 
+## TODO
+
+- [ ] Support downloading ingress / egress nodes list
+- [ ] Add type annotations
+
 ## FAQ
 
 ### How to obtain an access token?
 
 Please contact <wangyihanger@gmail.com>.
```

