# Comparing `tmp/cryptmoji-2.0.0.tar.gz` & `tmp/cryptmoji-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptmoji-2.0.0.tar", max compression
+gzip compressed data, was "cryptmoji-2.1.0.tar", max compression
```

## Comparing `cryptmoji-2.0.0.tar` & `cryptmoji-2.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      105 2022-09-15 07:14:30.573630 cryptmoji-2.0.0/cryptmoji/__init__.py
--rw-r--r--   0        0        0    13293 2022-09-15 07:14:56.385952 cryptmoji-2.0.0/cryptmoji/data.py
--rw-r--r--   0        0        0     1336 2022-09-15 07:15:19.021040 cryptmoji-2.0.0/cryptmoji/main.py
--rw-r--r--   0        0        0     1094 2022-09-04 12:17:14.880279 cryptmoji-2.0.0/LICENSE
--rw-r--r--   0        0        0     1161 2022-09-15 07:16:23.520519 cryptmoji-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      651 2022-09-07 13:36:47.700468 cryptmoji-2.0.0/README.md
--rw-r--r--   0        0        0     1230 2022-09-15 07:16:42.300898 cryptmoji-2.0.0/setup.py
--rw-r--r--   0        0        0     1777 2022-09-15 07:16:42.300898 cryptmoji-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      105 2023-04-26 03:44:58.000000 cryptmoji-2.1.0/cryptmoji/__init__.py
+-rw-r--r--   0        0        0      736 2024-05-13 09:06:41.074540 cryptmoji-2.1.0/cryptmoji/cli.py
+-rw-r--r--   0        0        0    13293 2022-09-15 07:14:58.000000 cryptmoji-2.1.0/cryptmoji/data.py
+-rw-r--r--   0        0        0     1400 2024-05-13 07:18:19.674068 cryptmoji-2.1.0/cryptmoji/main.py
+-rw-r--r--   0        0        0     1094 2022-09-04 12:17:16.000000 cryptmoji-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1569 2024-05-13 09:06:41.075540 cryptmoji-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1377 2024-05-13 09:06:41.074540 cryptmoji-2.1.0/README.md
+-rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 cryptmoji-2.1.0/PKG-INFO
```

### Comparing `cryptmoji-2.0.0/cryptmoji/data.py` & `cryptmoji-2.1.0/cryptmoji/data.py`

 * *Files identical despite different names*

### Comparing `cryptmoji-2.0.0/cryptmoji/main.py` & `cryptmoji-2.1.0/cryptmoji/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,55 @@
+from typing import Union
 from cryptmoji.data import EMOJIS
 
 LENGTH = len(EMOJIS)
 
 
-def encrypt(text: str, key: str = None) -> str:
+def encrypt(text: str, *, key: Union[str, None] = None) -> str:
     """
     Encrypts a string to emojis.
-    
+
     Args
     ----
     text: str
         The string to encrypt
     key: str
         The string to use for increasing complexity of encryption
-    
+
     Returns
     -------
     encrypted: str
         The encrypted string
     """
-    if key is not None:
-        char_2_int = [ord(text[i]) + ord(key[i % len(key)]) for i in range(len(text))]
-    else:  # key is None
-        char_2_int = [ord(text[i]) for i in range(len(text))]
-    text = [EMOJIS[i % LENGTH] for i in char_2_int]
-    return "".join(text)
+    iterator = range(len(text))
+    if key is None:
+        char_2_int = [ord(text[i]) for i in iterator]
+    else:  # key is not None
+        char_2_int = [ord(text[i]) + ord(key[i % len(key)]) for i in iterator]
+    char_arr = [EMOJIS[i % LENGTH] for i in char_2_int]
+    return "".join(char_arr)
 
 
-def decrypt(text: str, key: str = None) -> str:
+def decrypt(text: str, *, key: Union[str, None] = None) -> str:
     """
     Decrypts a string from emojis.
 
     Args
     ----
     text: str
         The string to decrypt
     key: str
         The string used encryption
-    
+
     Returns
     -------
     encrypted: str
         The decrypted string
     """
     emojis_2_int = [EMOJIS.index(i) for i in text]
+    iterator = range(len(emojis_2_int))
     if key is not None:
-        decrypted = [
-            emojis_2_int[i] - ord(key[i % len(key)]) for i in range(len(emojis_2_int))
-        ]
+        decrypted = [emojis_2_int[i] - ord(key[i % len(key)]) for i in iterator]
     else:
-        decrypted = [emojis_2_int[i] for i in range(len(emojis_2_int))]
-    text = [chr(i) for i in decrypted]
-    return "".join(text)
+        decrypted = [emojis_2_int[i] for i in iterator]
+    char_arr = [chr(i) for i in decrypted]
+    return "".join(char_arr)
```

### Comparing `cryptmoji-2.0.0/LICENSE` & `cryptmoji-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptmoji-2.0.0/PKG-INFO` & `cryptmoji-2.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,95 @@
 Metadata-Version: 2.1
 Name: cryptmoji
-Version: 2.0.0
+Version: 2.1.0
 Summary: Encrypt Text using emojis!
 Home-page: https://github.com/Siddhesh-Agarwal/cryptmoji
 License: MIT
-Keywords: encryption,emoji,cipher
+Keywords: encryption,emoji,cipher,cryptography,cryptmoji
 Author: Siddhesh Agarwal
 Author-email: siddhesh.agarwal@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7.0,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Project-URL: Documentation, https://siddhesh-agarwal.github.io/cryptmoji/
 Project-URL: Repository, https://github.com/Siddhesh-Agarwal/cryptmoji
 Description-Content-Type: text/markdown
 
-# 🐱‍👤 Cryptmoji
+# 🥷 Cryptmoji
 
 A simple emoji-based encryption-decryption library.
+
+![Downloads](https://static.pepy.tech/personalized-badge/cryptmoji?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads)
 _______________________
 
 ## 📥 Installation
 
-pip install the library:
+You can use the [pip](https://pypi.org/project/pip/) package manager to install the library.
 
 ```sh
 pip install cryptmoji
 ```
 
+or use [poetry](https://python-poetry.org/):
+
+```sh
+poetry add cryptmoji
+```
+
+> Check the [Documentation](https://siddhesh-agarwal.github.io/cryptmoji/)
+
 ## 📝 Usage
 
 ```python
-from cryptmoji import Cryptmoji
+from cryptmoji import encrypt, decrypt
 
-text = "Hello World!"
+text = "Hello, world!"
 key = "random_key" # makes the encryption stronger (optional)
 
-a = Cryptmoji(text, key=key)
 # The encrypt and decrypt functions return the value
-encrypted = a.encrypt()
-print(encrypted)
-# 🎚️🎨🎼🎲🏀🍯🎓🎼🎹🏂🎸🍤
+decrypted = decrypt(encrypted, key=key)
+print(decrypted)
+# '🎽🏉🏭🏣🏴🎐🍵🐀🏧🐉🏴🏈🎆'
 
 # The encrypt and decrypt functions change the value in-place too
-a.decrypt() 
+decrypted = decrypt(encrypted, key=key)
 print(decrypted)
-# Hello World!
+# 'Hello, world!'
+```
+
+## Command line tool
+
+### Installation
+
+```sh
+pip install cryptmoji[cli]
+```
+
+### Usage
+
+```sh
+$ cryptmoji encrypt "Hello World"
+Key (optional):
+🎿🏑🏸🏹🐁🍻🏑🐁🐄🏤🏪
+
+$ cryptmoji decrypt "🎿🏑🏸🏹🐁🍻🏑🐁🐄🏤🏪"
+Key (optional):
+Hello World
 ```
```

