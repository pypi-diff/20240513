# Comparing `tmp/didcomm_messaging-0.1.1a0.tar.gz` & `tmp/didcomm_messaging-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didcomm_messaging-0.1.1a0.tar", last modified: Tue Apr 23 18:55:15 2024, max compression
+gzip compressed data, was "didcomm_messaging-0.1.1a1.tar", last modified: Mon Apr 29 22:21:32 2024, max compression
```

## Comparing `didcomm_messaging-0.1.1a0.tar` & `didcomm_messaging-0.1.1a1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11357 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/LICENSE
--rw-r--r--   0        0        0     3592 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/README.md
--rw-r--r--   0        0        0     4855 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/__init__.py
--rw-r--r--   0        0        0      221 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/__init__.py
--rw-r--r--   0        0        0       52 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/__init__.py
--rw-r--r--   0        0        0    13927 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/askar.py
--rw-r--r--   0        0        0     7510 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/authlib.py
--rw-r--r--   0        0        0      646 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/basic.py
--rw-r--r--   0        0        0     4084 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/base.py
--rw-r--r--   0        0        0    15121 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/jwe.py
--rw-r--r--   0        0        0       42 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/__init__.py
--rw-r--r--   0        0        0     3880 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/multibase.py
--rw-r--r--   0        0        0     2264 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/multicodec.py
--rw-r--r--   0        0        0     6742 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/packaging.py
--rw-r--r--   0        0        0    12388 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/quickstart.py
--rw-r--r--   0        0        0     2487 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/__init__.py
--rw-r--r--   0        0        0     1227 2024-04-23 18:54:50.378221 didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/peer.py
--rw-r--r--   0        0        0     3811 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/web.py
--rw-r--r--   0        0        0     5947 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/didcomm_messaging/routing.py
--rw-r--r--   0        0        0     1590 2024-04-23 18:55:15.950390 didcomm_messaging-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/__init__.py
--rw-r--r--   0        0        0      678 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/crypto/__init__.py
--rw-r--r--   0        0        0     6607 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/crypto/test_askar.py
--rw-r--r--   0        0        0     3166 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/crypto/test_askar_x_authlib.py
--rw-r--r--   0        0        0     2124 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/crypto/test_authlib.py
--rw-r--r--   0        0        0      740 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/test_didresolver.py
--rw-r--r--   0        0        0     2787 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/test_didweb.py
--rw-r--r--   0        0        0     2197 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/test_packaging.py
--rw-r--r--   0        0        0      771 2024-04-23 18:54:50.382221 didcomm_messaging-0.1.1a0/tests/test_secrets.py
--rw-r--r--   0        0        0     4314 1970-01-01 00:00:00.000000 didcomm_messaging-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0     3592 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/README.md
+-rw-r--r--   0        0        0     4855 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/backend/__init__.py
+-rw-r--r--   0        0        0    13927 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/backend/askar.py
+-rw-r--r--   0        0        0     7510 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/backend/authlib.py
+-rw-r--r--   0        0        0      646 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/backend/basic.py
+-rw-r--r--   0        0        0     4084 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/base.py
+-rw-r--r--   0        0        0    15121 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/jwe.py
+-rw-r--r--   0        0        0       42 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/multiformats/__init__.py
+-rw-r--r--   0        0        0     3880 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/multiformats/multibase.py
+-rw-r--r--   0        0        0     2264 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/multiformats/multicodec.py
+-rw-r--r--   0        0        0     6742 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/packaging.py
+-rw-r--r--   0        0        0    18364 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/quickstart.py
+-rw-r--r--   0        0        0     2487 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/resolver/__init__.py
+-rw-r--r--   0        0        0     1227 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/resolver/peer.py
+-rw-r--r--   0        0        0     3811 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/resolver/web.py
+-rw-r--r--   0        0        0     5947 2024-04-29 22:21:08.000252 didcomm_messaging-0.1.1a1/didcomm_messaging/routing.py
+-rw-r--r--   0        0        0     1590 2024-04-29 22:21:32.648178 didcomm_messaging-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/crypto/__init__.py
+-rw-r--r--   0        0        0     6607 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/crypto/test_askar.py
+-rw-r--r--   0        0        0     3166 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/crypto/test_askar_x_authlib.py
+-rw-r--r--   0        0        0     2124 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/crypto/test_authlib.py
+-rw-r--r--   0        0        0      740 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/test_didresolver.py
+-rw-r--r--   0        0        0     2787 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/test_didweb.py
+-rw-r--r--   0        0        0     2197 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/test_packaging.py
+-rw-r--r--   0        0        0      771 2024-04-29 22:21:08.004252 didcomm_messaging-0.1.1a1/tests/test_secrets.py
+-rw-r--r--   0        0        0     4314 1970-01-01 00:00:00.000000 didcomm_messaging-0.1.1a1/PKG-INFO
```

### Comparing `didcomm_messaging-0.1.1a0/LICENSE` & `didcomm_messaging-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/README.md` & `didcomm_messaging-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/__init__.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/askar.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/backend/askar.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/authlib.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/backend/authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/backend/basic.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/backend/basic.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/base.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/base.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/crypto/jwe.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/crypto/jwe.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/multibase.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/multiformats/multibase.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/multiformats/multicodec.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/multiformats/multicodec.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/packaging.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/packaging.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/__init__.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/peer.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/resolver/peer.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/resolver/web.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/resolver/web.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/didcomm_messaging/routing.py` & `didcomm_messaging-0.1.1a1/didcomm_messaging/routing.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/pyproject.toml` & `didcomm_messaging-0.1.1a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "didcomm-messaging"
-version = "0.1.1a0"
+version = "0.1.1a1"
 description = "DIDComm Messaging implemented with swappable backends."
 authors = [
     { name = "Daniel Bluhm", email = "dbluhm@pm.me" },
     { name = "Colton Wolkins", email = "colton@indicio.tech" },
     { name = "Micah Peltier", email = "micah@indicio.tech" },
 ]
 dependencies = [
```

### Comparing `didcomm_messaging-0.1.1a0/tests/conftest.py` & `didcomm_messaging-0.1.1a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/tests/crypto/test_askar.py` & `didcomm_messaging-0.1.1a1/tests/crypto/test_askar.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/tests/crypto/test_askar_x_authlib.py` & `didcomm_messaging-0.1.1a1/tests/crypto/test_askar_x_authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/tests/crypto/test_authlib.py` & `didcomm_messaging-0.1.1a1/tests/crypto/test_authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/tests/test_didresolver.py` & `didcomm_messaging-0.1.1a1/tests/test_didresolver.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/tests/test_didweb.py` & `didcomm_messaging-0.1.1a1/tests/test_didweb.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/tests/test_packaging.py` & `didcomm_messaging-0.1.1a1/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/tests/test_secrets.py` & `didcomm_messaging-0.1.1a1/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a0/PKG-INFO` & `didcomm_messaging-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didcomm-messaging
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: DIDComm Messaging implemented with swappable backends.
 Author-Email: Daniel Bluhm <dbluhm@pm.me>, Colton Wolkins <colton@indicio.tech>, Micah Peltier <micah@indicio.tech>
 License: Apache-2.0
 Requires-Python: >=3.9
 Requires-Dist: base58>=2.1.1
 Requires-Dist: pydid>=0.4.2
 Requires-Dist: aries-askar>=0.2.9; extra == "askar"
```

