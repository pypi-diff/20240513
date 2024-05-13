# Comparing `tmp/extrautilities-0.4.tar.gz` & `tmp/extrautilities-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-0.4.tar", last modified: Mon May 13 17:46:03 2024, max compression
+gzip compressed data, was "extrautilities-0.5.tar", last modified: Mon May 13 17:51:26 2024, max compression
```

## Comparing `extrautilities-0.4.tar` & `extrautilities-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 17:46:03.700928 extrautilities-0.4/
-drwxrwxrwx   0        0        0        0 2024-05-13 17:46:03.688244 extrautilities-0.4/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.4/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.4/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     1978 2024-05-13 17:45:06.000000 extrautilities-0.4/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0     2361 2024-05-13 17:46:03.700428 extrautilities-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 17:46:03.699423 extrautilities-0.4/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     2361 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 17:46:03.700928 extrautilities-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1069 2024-05-13 17:46:00.000000 extrautilities-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:51:26.125938 extrautilities-0.5/
+drwxrwxrwx   0        0        0        0 2024-05-13 17:51:26.114409 extrautilities-0.5/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.5/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.5/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     1783 2024-05-13 17:50:19.000000 extrautilities-0.5/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0     2361 2024-05-13 17:51:26.125434 extrautilities-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 17:51:26.124829 extrautilities-0.5/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     2361 2024-05-13 17:51:26.000000 extrautilities-0.5/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-13 17:51:26.000000 extrautilities-0.5/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:51:26.000000 extrautilities-0.5/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-13 17:51:26.000000 extrautilities-0.5/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 17:51:26.000000 extrautilities-0.5/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 17:51:26.125938 extrautilities-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2024-05-13 17:51:25.000000 extrautilities-0.5/setup.py
```

### Comparing `extrautilities-0.4/ExtraUtils/RateLimit.py` & `extrautilities-0.5/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.4/ExtraUtils/asyncTokens.py` & `extrautilities-0.5/ExtraUtils/asyncTokens.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.serialization import load_pem_public_key
 
-# RSA Schlüsselpaar generieren
+
 def generiere_rsa_schluesselpaar():
     priv_key = rsa.generate_private_key(
         public_exponent=65537,
         key_size=2048,
         backend=default_backend()
     )
     pub_key = priv_key.public_key()
     return (priv_key, pub_key)
 
-# Nachricht mit dem öffentlichen Schlüssel verschlüsseln
 def encrypt(nachricht, pub_key):
     message = pub_key.encrypt(
         nachricht.encode(),
         padding.OAEP(
             mgf=padding.MGF1(algorithm=hashes.SHA256()),
             algorithm=hashes.SHA256(),
             label=None
         )
     )
     return message
 
-def serialize_key(key):
+def serial(key):
     return key.public_bytes(
         encoding=serialization.Encoding.PEM,
         format=serialization.PublicFormat.SubjectPublicKeyInfo
     ).decode('utf-8')
 
-def deserialize_key(key):
+def load(key):
     pub_key = load_pem_public_key(
         key.encode('utf-8'),
         backend=default_backend()
     )
     return pub_key
 
-
-# Nachricht mit dem privaten Schlüssel entschlüsseln
 def decrypt(message, priv_key):
-    entschluesselte_nachricht = priv_key.decrypt(
+    decrypted_message = priv_key.decrypt(
         message,
         padding.OAEP(
             mgf=padding.MGF1(algorithm=hashes.SHA256()),
             algorithm=hashes.SHA256(),
             label=None
         )
     )
-    return entschluesselte_nachricht.decode()
-
-# Beispiel
-priv_key, pub_key = generiere_rsa_schluesselpaar()
-message = verschluesseln("Geheime Nachricht", pub_key)
-print(f"Verschlüsselt: {message}")
+    return decrypted_message.decode()
 
-entschluesselte_nachricht = decrypt(message, priv_key)
-print(f"Entschlüsselt: {entschluesselte_nachricht}")
+# Example:
+# priv_key, pub_key = generiere_rsa_schluesselpaar()
+# message = encrypt("Geheime Nachricht", pub_key)
+# print(f"Verschlüsselt: {message}")
+# 
+# decrypted_message = decrypt(message, priv_key)
+# print(f"Entschlüsselt: {decrypted_message}")
```

### Comparing `extrautilities-0.4/PKG-INFO` & `extrautilities-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.4
+Version: 0.5
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,asyncTokens
 Platform: UNKNOWN
```

### Comparing `extrautilities-0.4/README.md` & `extrautilities-0.5/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-0.4/extrautilities.egg-info/PKG-INFO` & `extrautilities-0.5/extrautilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.4
+Version: 0.5
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,asyncTokens
 Platform: UNKNOWN
```

### Comparing `extrautilities-0.4/setup.py` & `extrautilities-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
```

