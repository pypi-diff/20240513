# Comparing `tmp/extrautilities-0.3.tar.gz` & `tmp/extrautilities-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-0.3.tar", last modified: Mon May 13 17:30:38 2024, max compression
+gzip compressed data, was "extrautilities-0.4.tar", last modified: Mon May 13 17:46:03 2024, max compression
```

## Comparing `extrautilities-0.3.tar` & `extrautilities-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 17:30:38.723534 extrautilities-0.3/
-drwxrwxrwx   0        0        0        0 2024-05-13 17:30:38.709870 extrautilities-0.3/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.3/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.3/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     1400 2024-05-13 17:30:18.000000 extrautilities-0.3/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0     2349 2024-05-13 17:30:38.723029 extrautilities-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 17:30:38.722198 extrautilities-0.3/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     2349 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 17:30:38.000000 extrautilities-0.3/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 17:30:38.723534 extrautilities-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-13 17:30:35.000000 extrautilities-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:46:03.700928 extrautilities-0.4/
+drwxrwxrwx   0        0        0        0 2024-05-13 17:46:03.688244 extrautilities-0.4/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.4/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.4/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     1978 2024-05-13 17:45:06.000000 extrautilities-0.4/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0     2361 2024-05-13 17:46:03.700428 extrautilities-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1514 2024-05-12 12:05:10.000000 extrautilities-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 17:46:03.699423 extrautilities-0.4/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     2361 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 17:46:03.000000 extrautilities-0.4/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 17:46:03.700928 extrautilities-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2024-05-13 17:46:00.000000 extrautilities-0.4/setup.py
```

### Comparing `extrautilities-0.3/ExtraUtils/RateLimit.py` & `extrautilities-0.4/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.3/ExtraUtils/asyncTokens.py` & `extrautilities-0.4/ExtraUtils/asyncTokens.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,62 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import rsa
+from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives import hashes
+from cryptography.hazmat.primitives.serialization import load_pem_public_key
 
 # RSA Schlüsselpaar generieren
-def gen_keypair():
+def generiere_rsa_schluesselpaar():
     priv_key = rsa.generate_private_key(
         public_exponent=65537,
         key_size=2048,
         backend=default_backend()
     )
     pub_key = priv_key.public_key()
     return (priv_key, pub_key)
 
 # Nachricht mit dem öffentlichen Schlüssel verschlüsseln
 def encrypt(nachricht, pub_key):
-    return pub_key.encrypt(
+    message = pub_key.encrypt(
         nachricht.encode(),
         padding.OAEP(
             mgf=padding.MGF1(algorithm=hashes.SHA256()),
             algorithm=hashes.SHA256(),
             label=None
         )
     )
+    return message
+
+def serialize_key(key):
+    return key.public_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo
+    ).decode('utf-8')
+
+def deserialize_key(key):
+    pub_key = load_pem_public_key(
+        key.encode('utf-8'),
+        backend=default_backend()
+    )
+    return pub_key
+
 
 # Nachricht mit dem privaten Schlüssel entschlüsseln
 def decrypt(message, priv_key):
-    decrypted = priv_key.decrypt(
+    entschluesselte_nachricht = priv_key.decrypt(
         message,
         padding.OAEP(
             mgf=padding.MGF1(algorithm=hashes.SHA256()),
             algorithm=hashes.SHA256(),
             label=None
         )
     )
-    return decrypted.decode()
+    return entschluesselte_nachricht.decode()
+
+# Beispiel
+priv_key, pub_key = generiere_rsa_schluesselpaar()
+message = verschluesseln("Geheime Nachricht", pub_key)
+print(f"Verschlüsselt: {message}")
 
-# Example
-# priv_key, pub_key = generiere_rsa_schluesselpaar()
-# message = verschluesseln("Geheime Nachricht", pub_key)
-# print(f"Verschlüsselt: {message}")
-# 
-# decrypted = decrypt(message, priv_key)
-# print(f"Entschlüsselt: {decrypted}")
+entschluesselte_nachricht = decrypt(message, priv_key)
+print(f"Entschlüsselt: {entschluesselte_nachricht}")
```

### Comparing `extrautilities-0.3/PKG-INFO` & `extrautilities-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.3
+Version: 0.4
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
-Keywords: RateLimit
+Keywords: RateLimit,asyncTokens
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `extrautilities-0.3/README.md` & `extrautilities-0.4/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-0.3/extrautilities.egg-info/PKG-INFO` & `extrautilities-0.4/extrautilities.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.3
+Version: 0.4
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
-Keywords: RateLimit
+Keywords: RateLimit,asyncTokens
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `extrautilities-0.3/setup.py` & `extrautilities-0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
@@ -18,10 +18,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
-    keywords='RateLimit',
+    keywords='RateLimit, asyncTokens',
     install_requires=["extradecorators", "cryptography"],
 )
```

