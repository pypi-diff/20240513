# Comparing `tmp/etoolkit-1.2.0.tar.gz` & `tmp/etoolkit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etoolkit-1.2.0.tar", last modified: Sat Apr 23 16:53:08 2022, max compression
+gzip compressed data, was "etoolkit-2.0.0.tar", last modified: Mon May 13 19:54:01 2024, max compression
```

## Comparing `etoolkit-1.2.0.tar` & `etoolkit-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 sgs       (1000) sgs       (1000)        0 2022-04-23 16:53:08.193660 etoolkit-1.2.0/
--rw-r--r--   0 sgs       (1000) sgs       (1000)    35147 2022-04-23 16:37:06.000000 etoolkit-1.2.0/COPYING
--rw-r--r--   0 sgs       (1000) sgs       (1000)    35147 2022-04-23 16:37:06.000000 etoolkit-1.2.0/LICENSE
--rw-r--r--   0 sgs       (1000) sgs       (1000)    11685 2022-04-23 16:53:08.193660 etoolkit-1.2.0/PKG-INFO
--rw-r--r--   0 sgs       (1000) sgs       (1000)    10506 2022-04-23 16:37:06.000000 etoolkit-1.2.0/README.md
--rw-r--r--   0 sgs       (1000) sgs       (1000)      195 2022-04-23 16:37:06.000000 etoolkit-1.2.0/pyproject.toml
--rw-r--r--   0 sgs       (1000) sgs       (1000)     1262 2022-04-23 16:53:08.193660 etoolkit-1.2.0/setup.cfg
-drwxr-xr-x   0 sgs       (1000) sgs       (1000)        0 2022-04-23 16:53:08.192660 etoolkit-1.2.0/src/
-drwxr-xr-x   0 sgs       (1000) sgs       (1000)        0 2022-04-23 16:53:08.192660 etoolkit-1.2.0/src/etoolkit/
--rw-r--r--   0 sgs       (1000) sgs       (1000)     1169 2022-04-23 16:37:06.000000 etoolkit-1.2.0/src/etoolkit/__init__.py
--rw-r--r--   0 sgs       (1000) sgs       (1000)    10072 2022-04-23 16:37:06.000000 etoolkit-1.2.0/src/etoolkit/__main__.py
--rwxr-xr-x   0 sgs       (1000) sgs       (1000)    14334 2022-04-23 16:37:06.000000 etoolkit-1.2.0/src/etoolkit/etoolkit.py
-drwxr-xr-x   0 sgs       (1000) sgs       (1000)        0 2022-04-23 16:53:08.193660 etoolkit-1.2.0/src/etoolkit.egg-info/
--rw-r--r--   0 sgs       (1000) sgs       (1000)    11685 2022-04-23 16:53:07.000000 etoolkit-1.2.0/src/etoolkit.egg-info/PKG-INFO
--rw-r--r--   0 sgs       (1000) sgs       (1000)      343 2022-04-23 16:53:08.000000 etoolkit-1.2.0/src/etoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 sgs       (1000) sgs       (1000)        1 2022-04-23 16:53:07.000000 etoolkit-1.2.0/src/etoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 sgs       (1000) sgs       (1000)       52 2022-04-23 16:53:07.000000 etoolkit-1.2.0/src/etoolkit.egg-info/entry_points.txt
--rw-r--r--   0 sgs       (1000) sgs       (1000)       18 2022-04-23 16:53:08.000000 etoolkit-1.2.0/src/etoolkit.egg-info/requires.txt
--rw-r--r--   0 sgs       (1000) sgs       (1000)        9 2022-04-23 16:53:08.000000 etoolkit-1.2.0/src/etoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 sgs       (1000) users      (100)        0 2024-05-13 19:54:01.835456 etoolkit-2.0.0/
+-rw-r--r--   0 sgs       (1000) users      (100)    35147 2021-12-10 19:50:42.000000 etoolkit-2.0.0/COPYING
+-rw-r--r--   0 sgs       (1000) users      (100)    35147 2021-12-10 19:50:53.000000 etoolkit-2.0.0/LICENSE
+-rw-r--r--   0 sgs       (1000) users      (100)    14697 2024-05-13 19:54:01.835456 etoolkit-2.0.0/PKG-INFO
+-rw-r--r--   0 sgs       (1000) users      (100)    13470 2024-05-13 11:28:15.000000 etoolkit-2.0.0/README.md
+-rw-r--r--   0 sgs       (1000) users      (100)      220 2023-01-10 12:23:36.000000 etoolkit-2.0.0/pyproject.toml
+-rw-r--r--   0 sgs       (1000) users      (100)     1303 2024-05-13 19:54:01.836457 etoolkit-2.0.0/setup.cfg
+drwxr-xr-x   0 sgs       (1000) users      (100)        0 2024-05-13 19:54:01.835456 etoolkit-2.0.0/src/
+drwxr-xr-x   0 sgs       (1000) users      (100)        0 2024-05-13 19:54:01.835456 etoolkit-2.0.0/src/etoolkit/
+-rw-r--r--   0 sgs       (1000) users      (100)     1170 2024-05-13 09:50:18.000000 etoolkit-2.0.0/src/etoolkit/__init__.py
+-rw-r--r--   0 sgs       (1000) users      (100)    14311 2024-05-13 11:03:15.000000 etoolkit-2.0.0/src/etoolkit/__main__.py
+-rw-r--r--   0 sgs       (1000) users      (100)    18455 2024-05-13 09:54:45.000000 etoolkit-2.0.0/src/etoolkit/etoolkit.py
+drwxr-xr-x   0 sgs       (1000) users      (100)        0 2024-05-13 19:54:01.835456 etoolkit-2.0.0/src/etoolkit.egg-info/
+-rw-r--r--   0 sgs       (1000) users      (100)    14697 2024-05-13 19:54:01.000000 etoolkit-2.0.0/src/etoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 sgs       (1000) users      (100)      436 2024-05-13 19:54:01.000000 etoolkit-2.0.0/src/etoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 sgs       (1000) users      (100)        1 2024-05-13 19:54:01.000000 etoolkit-2.0.0/src/etoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 sgs       (1000) users      (100)       52 2024-05-13 19:54:01.000000 etoolkit-2.0.0/src/etoolkit.egg-info/entry_points.txt
+-rw-r--r--   0 sgs       (1000) users      (100)       18 2024-05-13 19:54:01.000000 etoolkit-2.0.0/src/etoolkit.egg-info/requires.txt
+-rw-r--r--   0 sgs       (1000) users      (100)        9 2024-05-13 19:54:01.000000 etoolkit-2.0.0/src/etoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 sgs       (1000) users      (100)        0 2024-05-13 19:54:01.835456 etoolkit-2.0.0/tests/
+-rw-r--r--   0 sgs       (1000) users      (100)     6122 2024-05-06 12:41:40.000000 etoolkit-2.0.0/tests/test_cli.py
+-rw-r--r--   0 sgs       (1000) users      (100)     3151 2024-05-06 12:38:07.000000 etoolkit-2.0.0/tests/test_envtoolkit_instance.py
+-rw-r--r--   0 sgs       (1000) users      (100)     7533 2024-05-13 08:37:42.000000 etoolkit-2.0.0/tests/test_envtoolkit_instance_static.py
```

### Comparing `etoolkit-1.2.0/COPYING` & `etoolkit-2.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `etoolkit-1.2.0/LICENSE` & `etoolkit-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etoolkit-1.2.0/PKG-INFO` & `etoolkit-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: etoolkit
-Version: 1.2.0
-Summary: A simple toolkit for setting environment variables in a flexible way
-Home-page: https://github.com/blackm0re/etoolkit
-Author: attr: etoolkit.__author__
-Author-email: sgs@pichove.org
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/blackm0re/etoolkit/issues
-Project-URL: Source, https://github.com/blackm0re/etoolkit
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYING
-
 # etoolkit
 
 *etoolkit* is a simple toolkit for defining and setting environment variables
 in a flexible and secure way.
 
 
 ## General
@@ -46,15 +17,15 @@
 - the ability to spawn a child process with the defined variables
 
 - support for macros
 
 
 ## Requirements
 
-Apart from Python >= 3.7, the only requirement is
+Apart from Python >= 3.8, the only requirement is
 [cryptography](https://pypi.org/project/cryptography/)
 
 
 ## Overview
 
 In a typical UNIX environment, env. variables are usually set in one
 or more of the initialization / startup files like f.i. */etc/profile*,
@@ -94,20 +65,105 @@
 
 ### Gentoo
 
    ```bash
    # add sgs' custom repository using app-eselect/eselect-repository
    eselect repository add sgs
 
-   # ... or using layman (obsolete)
-   layman -a sgs
-
    emerge dev-python/etoolkit
    ```
 
+## Encryption & decryption scheme
+
+The etoolkit encryption format is currently at version 2.
+Encrypted values start with *enc-val$2$*.
+
+This new version introduces padding for values that are shorter than 32 bytes.
+The idea behind padding is to generate (32 - value length) random bytes and
+append them to the original value.
+That prevents a potential attacker from knowing the length of the encrypted
+short value (f.i. password, PIN number, username... etc).
+
+Values encrypted in the old format (*enc-val$1$*) can still be decrypted
+seamlessly.
+
+Authenticated encryption with associated data (AEAD) is implemented using
+AES-GCM.
+
+
+### Encryption
+
+Input:
+
+- plain-text value to be encrypted (P)
+
+- plain-text master-password used for key derivation (M)
+
+
+Output:
+
+- an encrypted value digest (base64) (B)
+
+
+Operation:
+
+- generate 32 bytes of random data to be used as a salt (S)
+
+- derive a 32 bytes key (K): K = scrypt(M, S, n=2**14, r=8, p=1)
+
+- use the first 12 bytes of S as nonce (NONCE)
+
+- calculate the padding length (L) as 32 - length of P, if P < 32, 0 otherwise
+
+- set the padding length bytes (N) (2bytes) to "%02d", if L > 0, "-1" otherwise
+
+- generate L bytes of random data to be used for padding (D)
+
+- encrypt and auth. P, auth.only S (E): E = AES_GCM_ENC(K, NONCE, N + P + D, S)
+
+- encrypted value digest (B) = enc-val$2$:BASE64_ENCODE(S)$BASE64_ENCODE(E)
+
+example:
+enc-val$2$uYpZM1VfAGq0CDZL2duITs076CQj+hIFEgx+F4mn80o=$UWP5YeRsh5/2vZ2J1UOS+BJti73Kbp6C1pJmCo8hFSujpe35X/XpzBegJJpo86AiCsNsUS6B6JM=
+
+
+### Decryption
+
+Input:
+
+- encrypted value digest (base64) (B)
+
+- plain-text master-password used for key derivation (M)
+
+
+Output:
+
+- plain-text password (P)
+
+
+Operation:
+
+- remove the prefix (enc-val$2$) from B and split the remaining value by '$'
+
+- base64-decode the salt (S): S = BASE64_DECODE(B1)
+
+- base64-decode the rest of the data (E): E = BASE64_DECODE(B2)
+
+- derive a 32 bytes key (K): K = scrypt(M, S, n=2**14, r=8, p=1)
+
+- use the first 12 bytes of S as nonce (NONCE)
+
+- decrypt the encrypted data (D): D = AES_GCM_DECRYPT(K, NONCE, E, S)
+
+- fetch the first 2 bytes (padding length bytes) (N): N = D[0 : 2]
+
+- calculate the padding length (L): L = INT(N) if N != "-1", 0 otherwise
+
+- fetch the plain-text (P): P = D[2 : -L] if L != 0, D[2 :] otherwise
+
 
 ## Setup and examples
 
 Most users (including me) will simply use the command line interface (CLI).
 
 
 ### CLI
@@ -226,14 +282,25 @@
 One can also spawn a different process than an interactive shell by using the
 *-s* / *--spawn* parameter.
 
    ```bash
    etoolkit --spawn /bin/othershell <instance-name>
    ```
 
+It is possible to re-encrypt all encrypted values in a specific instance or in
+all defined instances either by using the same or a new master password.
+
+   ```bash
+   etoolkit --reencrypt all
+   ```
+
+will prompt for the current master password, then for a new master password
+(with confirmation) and finally the new config file (if "all") or instance
+contents will be displayed.
+
 Contact the author for questions and suggestions! :)
 
 
 ### Using the *EtoolkitInstance* class
 
 *etoolkit* comes with its own *etoolkit* package that contains the
 *EtoolkitInstance* class.
@@ -248,56 +315,55 @@
    ```python
    import os
 
    import etoolkit
 
 
    # using some static methods in order to create encrypted values
-   etoolkit.EtoolkitInstance.encrypt('the very secret passwd', 'secret1')
-   # Out: 'enc-val$1$Y/TBb1F3siHTw6qZg9ERzZfA8PLPf2CwGSQLpu9jYWw=$FT5tS9o+ABvsxogIXpJim16Gz5SVtV8='
+   etoolkit.EtoolkitInstance.encrypt('The very secret passwd', 'secret1')
+   # Out: 'enc-val$2$NDdp6WMbX7gdEyzGM5nI4jhyer4XL+BoQwAHtL2CXHw=$+Pztn1pfaXKjPpem5PIQrCNxR9pyE6zqgSoGg9qXvmhH6VsNQvUTmiaOvUFl35EbiYE='
 
-   etoolkit.EtoolkitInstance.encrypt('the very secret passwd', 'secret2')
-   # Out: 'enc-val$1$vIBcoCNiYrsDLtF41uLuSEnppBjhliD0B8jwcBJcj/c=$KwOGe/y1dlxktDaCnJPIVNuaQ4Q7yNo='
+   etoolkit.EtoolkitInstance.encrypt('The very secret passwd', 'secret2')
+   # Out: 'enc-val$2$H953GxW+qrYXIp+I97lJBmG1gv89wxcfmTu7PEpZzjE=$Tb3F8/izDbHAMklpIjYk73JAiav+w8ZhrMsO93FlQjGh4MTChjp2Yen5BxSBOWLvCD4='
 
 
    # The encrypted values will be used in our configuration structure
    # The following structure defines the 3 instances: default, dev and secret
    instances = {
        "general": {
        },
        "instances": {
            "_default": {
-               "ETOOLKIT_PROMPT": "(%i)",
-               "PYTHONPATH": "/home/user/%i/python",
+             "ETOOLKIT_PROMPT": "(%i)",
+             "ETOOLKIT_SENSITIVE": ["DB_CONNECTION", "ETOOLKIT_TEST_PASSWORD"]
            },
            "dev": {
                "ETOOLKIT_PARENT": "_default",
-               "PYTHONPATH": "%p:/home/user/%i/.pythonpath",
+               "PYTHONPATH": ":/home/user/.pythonpath",
+               "DB_CONNECTION": "enc-val$2$RAgDei59tUvDAkrBmxROqRaV/NxNFEI2eJIOP7sG/b8=$yse7zawHCzQCU31sZj4oJYLGonz1M7oqHqCilXLHkywa9nMPALypmVzi3QekekYuLeb5XVTmmp84NHoPn1M052otoRHSp+TMPsqBPRabfriIKEK4XQ=="
            },
            "secret": {
                "ETOOLKIT_PARENT": "_default",
-               "ETOOLKIT_SENSITIVE": ["PASSWORD"],
                "GNUPGHOME": "%h/private/.gnupg",
-               "PASSWORD": "enc-val$1$vIBcoCNiYrsDLtF41uLuSEnppBjhliD0B8jwcBJcj/c=$KwOGe/y1dlxktDaCnJPIVNuaQ4Q7yNo="
+               "ETOOLKIT_TEST_PASSWORD": "enc-val$2$RCSZqq9pWrRDoCVYVHopyu1LzaJGfv8roVviqrLTBxM=$+YYrZbwTBuG0Pl+WMQrvxLUtq5j8qYuQqzoIwgoGt7AaWZCJz+E7qoDeg3wke70ST8U="
            }
        }
    }
 
-
-   dev_instance = etoolkit.EtoolkitInstance('dev', instances)
+   secret_instance = etoolkit.EtoolkitInstance('secret', instances)
 
    # fetch the variables before the processing stage (calling get_environ())
    # since raw_env_variables is a dict, it can be modified (f.i. .update())
-   dev_instance.raw_env_variables
+   secret_instance.raw_env_variables
 
-   dev_instance.master_password = 'the very secret passwd'  # or perhaps using getpass
-   env_vars = dev_instance.get_env()
-   print(env_vars['PASSWORD'])  # outputs: 'secret2'
+   secret_instance.master_password = 'The very secret passwd'  # or perhaps using getpass
+   env_vars = secret_instance.get_environ()
+   print(env_vars['ETOOLKIT_TEST_PASSWORD'])  # outputs: 'secret1'
    
-   inst.dump_env(env_vars)  # prints all values, with the exception of 'PASSWORD'
+   secret_instance.env_to_str(env_vars)  # prints all values, with the exception of 'ETOOLKIT_TEST_PASSWORD'
 
    # set the env. variables.
    os.environ.update(env_vars)
    ```
 
 
 ### Tips
@@ -342,15 +408,13 @@
 ## Author
 
 Simeon Simeonov - sgs @ LiberaChat
 
 
 ## [License](https://github.com/blackm0re/etoolkit/blob/master/LICENSE)
 
-Copyright (C) 2021-2022 Simeon Simeonov
+Copyright (C) 2021-2024 Simeon Simeonov
 All rights reserved.
 
 [Licensed](https://github.com/blackm0re/etoolkit/blob/master/LICENSE) under the
 GNU General Public License v3.0 or later.
 SPDX-License-Identifier: GPL-3.0-or-later
-
-
```

### Comparing `etoolkit-1.2.0/setup.cfg` & `etoolkit-2.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
+	Programming Language :: Python :: 3.13
 	Operating System :: POSIX
 	Topic :: Security :: Cryptography
 project_urls = 
 	Bug Tracker = https://github.com/blackm0re/etoolkit/issues
 	Source = https://github.com/blackm0re/etoolkit
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	cryptography>=3.2
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
```

### Comparing `etoolkit-1.2.0/src/etoolkit/__init__.py` & `etoolkit-2.0.0/src/etoolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # etoolkit
-# Copyright (C) 2021-2022 Simeon Simeonov
+# Copyright (C) 2021-2024 Simeon Simeonov
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """A simple toolkit for setting environment variables in a flexible way"""
+
 from .etoolkit import EtoolkitInstance, EtoolkitInstanceError
 
 __author__ = 'Simeon Simeonov'
-__version__ = '1.2.0'
+__version__ = '2.0.0'
 __license__ = 'GPL3'
 
 
 def int_or_str(value):
     """Returns int value of value when possible"""
     try:
         return int(value)
```

### Comparing `etoolkit-1.2.0/src/etoolkit/etoolkit.py` & `etoolkit-2.0.0/src/etoolkit/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,420 +1,472 @@
 # etoolkit
-# Copyright (C) 2021-2022 Simeon Simeonov
+# Copyright (C) 2021-2024 Simeon Simeonov
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""The main module of the etoolkit package"""
-import base64
+"""
+CLI entry point for the etoolkit package
+
+Examples
+--------
+python -m etoolkit -h
+
+python -m etoolkit -p
+
+"""
+
+import argparse
+import errno
 import getpass
-import hashlib
+import io
+import json
+import logging
 import os
+import subprocess
+import sys
 
-from cryptography.exceptions import InvalidTag
-from cryptography.hazmat.primitives.ciphers.aead import AESGCM
+import etoolkit
 
+DEFAULT_LOG_FORMAT = '%(levelname)s: %(message)s'
+DEFAULT_LOG_LEVEL = logging.WARNING
 
-class EtoolkitInstanceError(Exception):
-    """EtoolkitInstanceError - Generic exceptions related to instances"""
+logger = logging.getLogger(__name__)
 
 
-class EtoolkitInstance:
-    """A basic class representing a single instance"""
-
-    def __init__(self, name: str, data: dict):
-        """
-        :param name: Instance name
-        :type name: str
-
-        :param data: .etoolkit.json alike dict
-        :type data: dict
-        """
-        self._name = name
-        self._parent = None
-        self._raw_env_variables = {}
-        self._sensitive_env_variables = []
-        self._master_password = None
-        self._master_password_hash = None
-        self._prompt_func = None  # function to use when prompting for input
-        try:
-            inst_data = data['instances'][name]
-        except KeyError as e:
-            raise EtoolkitInstanceError(f'Unknown instance "{name}"') from e
-        if inst_data.get('ETOOLKIT_PARENT'):
-            self._parent = EtoolkitInstance(inst_data['ETOOLKIT_PARENT'], data)
-            self._raw_env_variables.update(self._parent.raw_env_variables)
-            self._sensitive_env_variables.extend(
-                self._parent.sensitive_env_variables
-            )
-        if inst_data.get('ETOOLKIT_SENSITIVE'):
-            if not isinstance(inst_data['ETOOLKIT_SENSITIVE'], list):
-                raise EtoolkitInstanceError(
-                    '"ETOOLKIT_SENSITIVE" must be a list'
-                )
-            self._sensitive_env_variables.extend(
-                inst_data['ETOOLKIT_SENSITIVE']
-            )
-        self._raw_env_variables.update(inst_data)
-        # remove non env. variable data
-        self._raw_env_variables.pop('ETOOLKIT_PARENT', None)
-        self._raw_env_variables.pop('ETOOLKIT_SENSITIVE', None)
-        if 'general' in data and 'MASTER_PASSWORD_HASH' in data['general']:
-            self._master_password_hash = data['general'][
-                'MASTER_PASSWORD_HASH'
-            ]
+class EtoolkitCLIHandler:
+    """
+    Helper class used for handleing the growing amount of arguments
 
-    @property
-    def master_password(self) -> str:
-        """master_password-property"""
-        if self._master_password is not None:
-            return self._master_password
-        return None if self._parent is None else self._parent.master_password
-
-    @master_password.setter
-    def master_password(self, value):
-        """master_password-property setter"""
-        self._master_password = value
-        if self._parent is not None and self._parent.master_password is None:
-            self._parent.master_password = value
-
-    @property
-    def master_password_hash(self) -> str:
-        """master_password_hash-property"""
-        return self._master_password_hash
-
-    @master_password_hash.setter
-    def master_password_hash(self, value):
-        """master_password_hash-property setter"""
-        self._master_password_hash = value
-
-    @property
-    def name(self) -> str:
-        """name-property"""
-        return self._name
-
-    @property
-    def prompt_func(self):
-        """prompt_func-property"""
-        return self._prompt_func
-
-    @prompt_func.setter
-    def prompt_func(self, value):
-        """prompt_func-property setter"""
-        self._prompt_func = value
-        if self._parent is not None and self._parent.prompt_func is None:
-            # will be set even if None
-            self._parent.prompt_func = value
-
-    @property
-    def raw_env_variables(self) -> dict:
-        """raw_env_variables-property"""
-        return self._raw_env_variables
-
-    @property
-    def sensitive_env_variables(self) -> list:
-        """sensitive_env_variables-property"""
-        return self._sensitive_env_variables
-
-    @staticmethod
-    def confirm_password_prompt(
-        password_hash: str = None, confirm: bool = True
-    ) -> str:
-        """
-        Prompts for master password and then for confirmation if `confirm` True
-
-        :param password_hash: Hash to compare with instead of confirm
-        :type password_hash: str
-
-        :param confirm: Confirm the password (and see if there is a match)
-        :type confirm: bool
-
-        :return: Password provided by the user
-        :rtype: str
-        """
-        try:
-            while True:
-                pass1 = getpass.getpass('Type master password: ')
-                if password_hash:
-                    if EtoolkitInstance.password_matches(pass1, password_hash):
-                        return pass1
-                    print('Wrong password')
-                    continue
-                if confirm:
-                    pass2 = getpass.getpass('Confirm master password: ')
-                    if not pass1 or pass1 != pass2:
-                        print('The passwords are either empty or do not match')
-                        continue
-                return pass1.strip()
-        except Exception as e:
-            raise EtoolkitInstanceError('Prompt error') from e
-
-    @staticmethod
-    def decrypt(password: str, edata: str) -> str:
-        """
-        Decrypts `edata` using `password`.
-
-        `edata` is in the following format:
-        enc-val$`version-num`$`bas64-salt`$`base64-encrypted_data`
-
-        :param password: The password to generate the key with
-        :type password: str
-
-        :param edata: The data to be decrypted
-        :type edata: str
-
-        :return: The output string / decrypted data
-        :rtype: str
-        """
-        # check for supported versions
-        if not edata.startswith('enc-val$1$'):
-            raise EtoolkitInstanceError(
-                f'Unsupported encryption format: {edata}'
-            )
-        try:
-            salt, data = [base64.b64decode(t) for t in edata[10:].split('$')]
-            nonce = salt[:12]
-            aesgcm = AESGCM(
-                hashlib.scrypt(
-                    password.encode('utf-8'),
-                    salt=salt,
-                    n=2**14,
-                    r=8,
-                    p=1,
-                    dklen=32,
-                )
-            )
-            return aesgcm.decrypt(nonce, data, salt).decode()
-        except InvalidTag as e:
-            raise EtoolkitInstanceError(
-                f'Invalid tag when decrypting: {edata}'
-            ) from e
-        except Exception as e:
-            raise EtoolkitInstanceError(
-                f'Error when decrypting: {edata}'
-            ) from e
-
-    @staticmethod
-    def encrypt(password: str, data: str) -> str:
-        """
-        Encrypts `data` using `password`.
-
-        The output string is in the following format:
-        enc-val$`version-num`$`bas64-salt`$`base64-encrypted_data`
-
-        :param password: The password to generate the key with
-        :type password: str
-
-        :param data: The data to be encrypted
-        :type data: str
-
-        :return: The output string
-        :rtype: str
-        """
-        salt = os.urandom(32)
-        aesgcm = AESGCM(
-            hashlib.scrypt(
-                password.encode('utf-8'),
-                salt=salt,
-                n=2**14,
-                r=8,
-                p=1,
-                dklen=32,
-            )
-        )
-        nonce = salt[:12]
-        edata = aesgcm.encrypt(nonce, data.encode('utf-8'), salt)
-        return (
-            f'enc-val$1${base64.b64encode(salt).decode()}$'
-            f'{base64.b64encode(edata).decode()}'
-        )
+    This class consists mostly of interactive methods and is not intended as
+    a part of the etoolkit API
+    """
 
-    @staticmethod
-    def get_new_password_hash(password: str) -> str:
+    def __init__(self, args: argparse.Namespace, config_dict: dict):
         """
-        Returns a complete password hash based on `password`
+        :param args: The parsed argparse arguments sent by the caller
+        :type args: argparse.Namespace
 
-        This password hash is *not* used as a key when encrypting / decrypting
-        but only for optional check if a correct master password is provided.
+        :param config_dict: The config file structure
+        :type config_dict: dict
+        """
+        self._args = args
+        self._config_dict = config_dict
+
+        self._password_hash = None
+        if 'general' in config_dict:
+            self._password_hash = config_dict['general'].get(
+                'MASTER_PASSWORD_HASH'
+            )
 
-        :param password: The plaintext password
-        :type password: str
+        self._password_from_env = os.environ.get('ETOOLKIT_MASTER_PASSWORD')
 
-        :return: The hashed version of `password`
-        :rtype: str
+    def decrypt_value(self):
         """
-        hash_algo = 'sha256'
-        iterations = 100000
-        salt = os.urandom(32)
-        key = hashlib.pbkdf2_hmac(
-            hash_algo, password.encode('utf-8'), salt, iterations
-        )
-        return (
-            f'pbkdf2_{hash_algo}${iterations}$'
-            f'{base64.b64encode(salt).decode()}$'
-            f'{base64.b64encode(key).decode()}'
-        )
+        Interactive method for decrypting value(s)
+
+        Prompts for master key password and then prompts for a value to decrypt
 
-    @staticmethod
-    def parse_value(value, macros: dict):
+        The decrypted value is printed to stdout
         """
-        Returns the value with all macros replaced by their values
+        pipe_input = None
+        if not os.isatty(sys.stdin.fileno()):
+            pipe_input = sys.stdin.read().strip()
 
-        If `value` is not of type 'str' simply return `value`
+        if (
+            self._args.master_password_prompt
+            or self._password_from_env is None
+        ):
+            password = self._password_prompt()
+        else:
+            password = self._password_from_env
+
+        if pipe_input:
+            # the input came from stdin. No need to prompt
+            print(
+                'Decrypted value: '
+                f'{etoolkit.EtoolkitInstance.decrypt(password, pipe_input)}'
+            )
+            return
+        while True:
+            try:
+                value = input('Value: ')
+                print(
+                    'Decrypted value: '
+                    f'{etoolkit.EtoolkitInstance.decrypt(password, value)}'
+                )
+                if not self._args.multiple_values:
+                    break
+            except KeyboardInterrupt:
+                print(os.linesep)
+                break
+        return
 
-        :param value: A simple value
-        :type value: object
+    def encrypt_value(self):
+        """
+        Interactive method for encrypting value(s)
 
-        :param macros: Macros mapping
-        :type macros: dict
+        Prompts for master key password and then prompts for a value to encrypt
 
-        :return: New value with all macros replaced by their values
-        :rtype: object
+        The encrypted value is printed to stdout
         """
-        if not isinstance(value, str):
-            return value
-        for key, val in macros.items():
-            value = value.replace(key, val)
-        return value
+        pipe_input = None
+        if not os.isatty(sys.stdin.fileno()):
+            pipe_input = sys.stdin.read().strip()
 
-    @staticmethod
-    def password_matches(password: str, password_hash: str) -> bool:
-        """
-        Checks `password` agains s stored password hash
+        if (
+            self._args.master_password_prompt
+            or self._password_from_env is None
+        ):
+            password = self._password_prompt_confirm()
+        else:
+            password = self._password_from_env
+
+        if pipe_input:
+            # the input came from stdin. No need to prompt
+            print(
+                'Encrypted value: '
+                f'{etoolkit.EtoolkitInstance.encrypt(password, pipe_input)}'
+            )
+            return
 
-        Hash format: pbkdf2_hashalgo$ietarations$salt-base64$key-base64
+        while True:
+            try:
+                if self._args.echo:
+                    value = input('Value: ')
+                else:
+                    value = getpass.getpass('Value: ')
+                print(
+                    'Encrypted value: '
+                    f'{etoolkit.EtoolkitInstance.encrypt(password, value)}'
+                )
+                if not self._args.multiple_values:
+                    break
+            except KeyboardInterrupt:
+                print(os.linesep)
+                break
+        return
 
-        :param password: password
-        :type password: str
+    def generate_master_password_hash(self):
+        """
+        Interactive method for generating password hash
 
-        :param password_hash: The pbkdf2_hmac password hash
-        :type password_hash: str
+        Prompts for master key password and then for confirmation
 
-        :return: True if the password matches or password_hash is None,
-        :rtype: bool
+        The generated hash is printed to stdout
         """
-        if password_hash is None:
-            return True
-        # format: pbkdf2_hashalgo$ietarations$salt-base64$key-base64
-        try:
-            tokens = password_hash.split('$')
-            key = hashlib.pbkdf2_hmac(
-                tokens[0].split('_')[1],
-                password.encode('utf-8'),
-                base64.b64decode(tokens[2]),
-                int(tokens[1]),
+        phash = etoolkit.EtoolkitInstance.get_new_password_hash(
+            etoolkit.EtoolkitInstance.confirm_password_prompt()
+        )
+        print(f'Master password hash: {phash}')
+
+    def list(self):
+        """Lists all instances defined in the config file"""
+
+        for instance_name in sorted(
+            filter(
+                lambda s: not s.startswith('_'),
+                self._config_dict.get('instances', {}).keys(),
             )
-            return key == base64.b64decode(tokens[3])
-        except Exception:
-            return False
+        ):
+            print(instance_name)
 
-    def dump_env(self, env: dict):
-        """
-        Prints an environment dict to stdout.
+    def load_instance(self):
+        """Loads a single specified instance from the config file"""
 
-        :param env: The environment dict
-        :type env: dict
-        """
-        for key, value in env.items():
-            if key in self._sensitive_env_variables:
-                print(f'{key}: ***')
-                continue
-            print(f'{key}: {value}')
+        inst = etoolkit.EtoolkitInstance(
+            self._args.instance, self._config_dict
+        )
+
+        if (
+            self._args.master_password_prompt
+            or self._password_from_env is None
+        ):
+            inst.prompt_func = (
+                etoolkit.EtoolkitInstance.confirm_password_prompt
+            )
 
-    def get_environ(self) -> dict:
+        env = inst.get_environ()
+
+        if self._args.dump_output:
+            print(inst.env_to_str(env))
+
+        os.environ.update(env)
+
+        if self._args.spawn:
+            subprocess.run(self._args.spawn.split(), check=False)
+        else:
+            subprocess.run(
+                os.environ.get('SHELL', 'bash').split(), check=False
+            )
+
+    def reencrypt(self):
         """
-        Generates a new environ dict
+        Interactive method that prints new configuration data (JSON) to stdout
+
+        Prompts for master key password and then for a new password,
+        which may be the same as the current password
 
-        :return: New environment dict with all macros replaced by their values
-        :rtype: dict
+        All existing encrypted values are decrypted using the current password
+        and then encrypted with the new password
         """
-        macros = {
-            '%h': os.path.expanduser('~'),
-            '%i': self.name,
-            # '%f': self.get_full_name(),
-            '%u': getpass.getuser(),
-        }
-        new_env = {}
-        for key, value in sorted(
-            self._raw_env_variables.items(), key=lambda x: x[0]
+        print('(Current password) ', end='', flush=True)
+        if (
+            self._args.master_password_prompt
+            or self._password_from_env is None
         ):
-            if not value:
-                # perhaps unset instead of skipping?
-                continue
-            if isinstance(value, str) and '%p' in value:
-                macros['%p'] = (
-                    self._parent.get_environ().get(key, '')
-                    if self._parent is not None
-                    else ''
-                )
-            if isinstance(value, str) and value.startswith('enc-val$1$'):
-                value = self._decrypt_value(value)
-            if isinstance(value, str) and value.endswith(':'):
-                # if 'value' ends with ':', append the existing value of
-                # os.environ[key] after the value of 'value'
-                new_env[key] = self.parse_value(
-                    value, macros
-                ) + os.environ.get(key, '')
-            elif isinstance(value, str) and value.startswith(':'):
-                # if 'value' starts with ':', append after the existing value
-                # of os.environ[key]
-                new_env[key] = os.environ.get(key, '') + self.parse_value(
-                    value, macros
+            password = self._password_prompt()
+        else:
+            password = self._password_from_env
+
+        print('(New password) ', end='', flush=True)
+        new_password = etoolkit.EtoolkitInstance.confirm_password_prompt()
+
+        if self._args.reencrypt != 'all':
+            # re-encrypt a single instance
+            inst = etoolkit.EtoolkitInstance(
+                self._args.reencrypt, self._config_dict
+            )
+            print(
+                json.dumps(
+                    inst.get_reencrypted_instance_data(new_password, password),
+                    indent=4,
                 )
-            else:
-                # completely overwrite the existing value of os.environ[key]
-                new_env[key] = self.parse_value(value, macros)
-        return new_env
-
-    def get_full_name(self, delimiter: str = '') -> str:
-        """
-        Returns the entire instance inheritence path separated by `delimiter`
+            )
+            return
 
-        The format is:
-        `grandparent-name`<delimiter>`parent-name`<delimiter>`instance-name`
+        # re-encrypt all
+        new_config_dict = dict(self._config_dict)
+        if (
+            'general' in new_config_dict
+            and 'MASTER_PASSWORD_HASH' in new_config_dict['general']
+        ):
+            new_config_dict['general']['MASTER_PASSWORD_HASH'] = (
+                etoolkit.EtoolkitInstance.get_new_password_hash(new_password)
+            )
 
-        :param delimiter: Delimiter to separate parent instance names by
-        :type delimiter: str
+        for instance_name in self._config_dict['instances']:
+            inst = etoolkit.EtoolkitInstance(instance_name, self._config_dict)
+            new_config_dict['instances'][instance_name] = (
+                inst.get_reencrypted_instance_data(new_password, password)
+            )
+        print(json.dumps(new_config_dict, indent=4))
 
-        :return: Path in case this instance has parent, instance.name otherwise
-        :rtype: str
+    def _password_prompt(self) -> str:
         """
-        if self._parent is None:
-            return self.name
-        return self._parent.get_full_name(delimiter) + delimiter + self.name
-
-    def _decrypt_value(self, evalue: str) -> str:
+        Wrapper for EtoolkitInstance.confirm_password_prompt(confirm=False)
         """
-        Decrypts an encrypted value using the master password
+        return etoolkit.EtoolkitInstance.confirm_password_prompt(
+            self._password_hash, False
+        )
 
-        The method prompts for the master password when it encounters its
-        first encrypted value since the creation of its EtoolkitInstance
-        object
+    def _password_prompt_confirm(self) -> str:
+        """
+        Wrapper for EtoolkitInstance.confirm_password_prompt(confirm=True)
+        """
+        return etoolkit.EtoolkitInstance.confirm_password_prompt(
+            self._password_hash
+        )
 
-        `evalue` is in the following format:
-        enc-val$`version-num`$`bas64-salt`$`base64-encrypted_data`
 
-        :param evalue: Encrypted value to be decrypted
-        :type evalue: str
+def main(inargs=None):
+    """main entry point"""
 
-        :return: Decrypted value
-        :rtype: str
-        """
-        if self._master_password is None:
-            if self._prompt_func is None:
-                raise EtoolkitInstanceError(
-                    'Neither password or prompt function set'
-                )
-            # use master_password setter in order to propagate to parent
-            self.master_password = self._prompt_func(
-                self._master_password_hash, confirm=False
+    parser = argparse.ArgumentParser(
+        prog=__package__,
+        epilog=(
+            f'%(prog)s {etoolkit.__version__} by Simeon Simeonov '
+            '(sgs @ LiberaChat)'
+        ),
+        description='The following options are available',
+    )
+    group = parser.add_mutually_exclusive_group(required=True)
+    group.add_argument(
+        'instance',
+        metavar='<instance>',
+        nargs='?',
+        type=str,
+        help='The instance to be loaded',
+    )
+    group.add_argument(
+        '-d',
+        '--decrypt-value',
+        dest='decrypt_value',
+        action='store_true',
+        required=False,
+        help=(
+            'Prompt for master password & value to decrypt, '
+            'display the decrypted value and exit'
+        ),
+    )
+    group.add_argument(
+        '-e',
+        '--encrypt-value',
+        dest='encrypt_value',
+        action='store_true',
+        required=False,
+        help=(
+            'Prompt for master password & value to encrypt, '
+            'display the encrypted value and exit'
+        ),
+    )
+    group.add_argument(
+        '-l',
+        '--list',
+        dest='list',
+        action='store_true',
+        required=False,
+        help='List all defined instances',
+    )
+    group.add_argument(
+        '-p',
+        '--generate-master-password-hash',
+        dest='password_hash',
+        action='store_true',
+        required=False,
+        help='Prompt for master password, display the generated hash and exit',
+    )
+    group.add_argument(
+        '-r',
+        '--reencrypt',
+        metavar='<instance | all>',
+        type=str,
+        default='',
+        dest='reencrypt',
+        required=False,
+        help=(
+            'Prompt for current master password, new master password and '
+            're-encrypt either all encrypted values or only those for a '
+            'given instance'
+        ),
+    )
+    parser.add_argument(
+        '-c',
+        '--config-file',
+        metavar='<path>',
+        type=str,
+        default=os.path.expanduser(
+            os.environ.get('ETOOLKIT_CONFIG', '~/.etoolkit.json')
+        ),
+        dest='config_file',
+        help='JSON config file (default: ~/.etoolkit.json)',
+    )
+    parser.add_argument(
+        '-E',
+        '--echo',
+        dest='echo',
+        action='store_true',
+        help='Display the value to be encrypted (used together with -e)',
+    )
+    parser.add_argument(
+        '-m',
+        '--multiple-values',
+        dest='multiple_values',
+        action='store_true',
+        help=(
+            'Prompt for more than one value when '
+            'encrypting / decrypting until terminated '
+            '(Ctrl+C) (used together with -d / -e)'
+        ),
+    )
+    parser.add_argument(
+        '-P',
+        '--master-password-prompt',
+        dest='master_password_prompt',
+        action='store_true',
+        help=(
+            'Force prompt for the master password even if the env. variable '
+            '"ETOOLKIT_MASTER_PASSWORD" is set'
+        ),
+    )
+    parser.add_argument(
+        '-q',
+        '--no-output',
+        dest='dump_output',
+        action='store_false',
+        default=True,
+        help='Do not print environment variables to stdout',
+    )
+    parser.add_argument(
+        '-s',
+        '--spawn',
+        metavar='<path>',
+        type=str,
+        default='',
+        dest='spawn',
+        help='Spawn another process than $SHELL',
+    )
+    parser.add_argument(
+        '-v',
+        '--version',
+        action='version',
+        version=f'%(prog)s {etoolkit.__version__}',
+        help='Display program-version and exit',
+    )
+    args = parser.parse_args(inargs)
+    try:
+        with io.open(args.config_file, encoding='utf-8') as fp:
+            config_dict = json.load(fp)
+    except FileNotFoundError as err:
+        # do not raise exception if config-file is missing for:
+        # - decrypting value
+        # - encrypting value
+        # - password hash generation
+        if args.password_hash or args.decrypt_value or args.encrypt_value:
+            logger.warning(
+                'Configuration file %s is missing, although not required '
+                'by the provided parameters',
+                args.config_file,
             )
-        return EtoolkitInstance.decrypt(self._master_password, evalue)
+            config_dict = {}
+        else:
+            logger.error('Configuration file %s is missing', args.config_file)
+            raise SystemExit(errno.EIO) from err
+    except Exception as exp:
+        logger.exception('Unable to parse %r', args.config_file)
+        raise SystemExit(errno.EIO) from exp
+    try:
+        etoolkit_cli_handler = EtoolkitCLIHandler(args, config_dict)
+        if args.decrypt_value:
+            etoolkit_cli_handler.decrypt_value()
+            sys.exit(0)
+        if args.encrypt_value:
+            etoolkit_cli_handler.encrypt_value()
+            sys.exit(0)
+        if args.password_hash:
+            etoolkit_cli_handler.generate_master_password_hash()
+            sys.exit(0)
+        if args.list:
+            etoolkit_cli_handler.list()
+            sys.exit(0)
+        if args.reencrypt:
+            etoolkit_cli_handler.reencrypt()
+            sys.exit(0)
+
+        etoolkit_cli_handler.load_instance()
+    except KeyboardInterrupt:
+        logger.debug('KeyboardInterrupt')
+        print(os.linesep)
+        sys.exit(0)
+    except etoolkit.EtoolkitInstanceError as err:
+        logger.error('EtoolkitInstanceError: %s', err)
+        sys.exit(1)
+    except subprocess.CalledProcessError as err:
+        logger.error('Unable to spawn shell process: %s', err)
+        sys.exit(1)
+    except Exception:
+        logger.exception('Unexpected exception')
+        sys.exit(1)
+
+
+if __name__ == '__main__':
+    logging.basicConfig(level=DEFAULT_LOG_LEVEL, format=DEFAULT_LOG_FORMAT)
+    main()
```

### Comparing `etoolkit-1.2.0/src/etoolkit.egg-info/PKG-INFO` & `etoolkit-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: etoolkit
-Version: 1.2.0
+Version: 2.0.0
 Summary: A simple toolkit for setting environment variables in a flexible way
 Home-page: https://github.com/blackm0re/etoolkit
 Author: attr: etoolkit.__author__
 Author-email: sgs@pichove.org
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/blackm0re/etoolkit/issues
 Project-URL: Source, https://github.com/blackm0re/etoolkit
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYING
+Requires-Dist: cryptography>=3.2
 
 # etoolkit
 
 *etoolkit* is a simple toolkit for defining and setting environment variables
 in a flexible and secure way.
 
 
@@ -46,15 +46,15 @@
 - the ability to spawn a child process with the defined variables
 
 - support for macros
 
 
 ## Requirements
 
-Apart from Python >= 3.7, the only requirement is
+Apart from Python >= 3.8, the only requirement is
 [cryptography](https://pypi.org/project/cryptography/)
 
 
 ## Overview
 
 In a typical UNIX environment, env. variables are usually set in one
 or more of the initialization / startup files like f.i. */etc/profile*,
@@ -94,20 +94,105 @@
 
 ### Gentoo
 
    ```bash
    # add sgs' custom repository using app-eselect/eselect-repository
    eselect repository add sgs
 
-   # ... or using layman (obsolete)
-   layman -a sgs
-
    emerge dev-python/etoolkit
    ```
 
+## Encryption & decryption scheme
+
+The etoolkit encryption format is currently at version 2.
+Encrypted values start with *enc-val$2$*.
+
+This new version introduces padding for values that are shorter than 32 bytes.
+The idea behind padding is to generate (32 - value length) random bytes and
+append them to the original value.
+That prevents a potential attacker from knowing the length of the encrypted
+short value (f.i. password, PIN number, username... etc).
+
+Values encrypted in the old format (*enc-val$1$*) can still be decrypted
+seamlessly.
+
+Authenticated encryption with associated data (AEAD) is implemented using
+AES-GCM.
+
+
+### Encryption
+
+Input:
+
+- plain-text value to be encrypted (P)
+
+- plain-text master-password used for key derivation (M)
+
+
+Output:
+
+- an encrypted value digest (base64) (B)
+
+
+Operation:
+
+- generate 32 bytes of random data to be used as a salt (S)
+
+- derive a 32 bytes key (K): K = scrypt(M, S, n=2**14, r=8, p=1)
+
+- use the first 12 bytes of S as nonce (NONCE)
+
+- calculate the padding length (L) as 32 - length of P, if P < 32, 0 otherwise
+
+- set the padding length bytes (N) (2bytes) to "%02d", if L > 0, "-1" otherwise
+
+- generate L bytes of random data to be used for padding (D)
+
+- encrypt and auth. P, auth.only S (E): E = AES_GCM_ENC(K, NONCE, N + P + D, S)
+
+- encrypted value digest (B) = enc-val$2$:BASE64_ENCODE(S)$BASE64_ENCODE(E)
+
+example:
+enc-val$2$uYpZM1VfAGq0CDZL2duITs076CQj+hIFEgx+F4mn80o=$UWP5YeRsh5/2vZ2J1UOS+BJti73Kbp6C1pJmCo8hFSujpe35X/XpzBegJJpo86AiCsNsUS6B6JM=
+
+
+### Decryption
+
+Input:
+
+- encrypted value digest (base64) (B)
+
+- plain-text master-password used for key derivation (M)
+
+
+Output:
+
+- plain-text password (P)
+
+
+Operation:
+
+- remove the prefix (enc-val$2$) from B and split the remaining value by '$'
+
+- base64-decode the salt (S): S = BASE64_DECODE(B1)
+
+- base64-decode the rest of the data (E): E = BASE64_DECODE(B2)
+
+- derive a 32 bytes key (K): K = scrypt(M, S, n=2**14, r=8, p=1)
+
+- use the first 12 bytes of S as nonce (NONCE)
+
+- decrypt the encrypted data (D): D = AES_GCM_DECRYPT(K, NONCE, E, S)
+
+- fetch the first 2 bytes (padding length bytes) (N): N = D[0 : 2]
+
+- calculate the padding length (L): L = INT(N) if N != "-1", 0 otherwise
+
+- fetch the plain-text (P): P = D[2 : -L] if L != 0, D[2 :] otherwise
+
 
 ## Setup and examples
 
 Most users (including me) will simply use the command line interface (CLI).
 
 
 ### CLI
@@ -226,14 +311,25 @@
 One can also spawn a different process than an interactive shell by using the
 *-s* / *--spawn* parameter.
 
    ```bash
    etoolkit --spawn /bin/othershell <instance-name>
    ```
 
+It is possible to re-encrypt all encrypted values in a specific instance or in
+all defined instances either by using the same or a new master password.
+
+   ```bash
+   etoolkit --reencrypt all
+   ```
+
+will prompt for the current master password, then for a new master password
+(with confirmation) and finally the new config file (if "all") or instance
+contents will be displayed.
+
 Contact the author for questions and suggestions! :)
 
 
 ### Using the *EtoolkitInstance* class
 
 *etoolkit* comes with its own *etoolkit* package that contains the
 *EtoolkitInstance* class.
@@ -248,56 +344,55 @@
    ```python
    import os
 
    import etoolkit
 
 
    # using some static methods in order to create encrypted values
-   etoolkit.EtoolkitInstance.encrypt('the very secret passwd', 'secret1')
-   # Out: 'enc-val$1$Y/TBb1F3siHTw6qZg9ERzZfA8PLPf2CwGSQLpu9jYWw=$FT5tS9o+ABvsxogIXpJim16Gz5SVtV8='
+   etoolkit.EtoolkitInstance.encrypt('The very secret passwd', 'secret1')
+   # Out: 'enc-val$2$NDdp6WMbX7gdEyzGM5nI4jhyer4XL+BoQwAHtL2CXHw=$+Pztn1pfaXKjPpem5PIQrCNxR9pyE6zqgSoGg9qXvmhH6VsNQvUTmiaOvUFl35EbiYE='
 
-   etoolkit.EtoolkitInstance.encrypt('the very secret passwd', 'secret2')
-   # Out: 'enc-val$1$vIBcoCNiYrsDLtF41uLuSEnppBjhliD0B8jwcBJcj/c=$KwOGe/y1dlxktDaCnJPIVNuaQ4Q7yNo='
+   etoolkit.EtoolkitInstance.encrypt('The very secret passwd', 'secret2')
+   # Out: 'enc-val$2$H953GxW+qrYXIp+I97lJBmG1gv89wxcfmTu7PEpZzjE=$Tb3F8/izDbHAMklpIjYk73JAiav+w8ZhrMsO93FlQjGh4MTChjp2Yen5BxSBOWLvCD4='
 
 
    # The encrypted values will be used in our configuration structure
    # The following structure defines the 3 instances: default, dev and secret
    instances = {
        "general": {
        },
        "instances": {
            "_default": {
-               "ETOOLKIT_PROMPT": "(%i)",
-               "PYTHONPATH": "/home/user/%i/python",
+             "ETOOLKIT_PROMPT": "(%i)",
+             "ETOOLKIT_SENSITIVE": ["DB_CONNECTION", "ETOOLKIT_TEST_PASSWORD"]
            },
            "dev": {
                "ETOOLKIT_PARENT": "_default",
-               "PYTHONPATH": "%p:/home/user/%i/.pythonpath",
+               "PYTHONPATH": ":/home/user/.pythonpath",
+               "DB_CONNECTION": "enc-val$2$RAgDei59tUvDAkrBmxROqRaV/NxNFEI2eJIOP7sG/b8=$yse7zawHCzQCU31sZj4oJYLGonz1M7oqHqCilXLHkywa9nMPALypmVzi3QekekYuLeb5XVTmmp84NHoPn1M052otoRHSp+TMPsqBPRabfriIKEK4XQ=="
            },
            "secret": {
                "ETOOLKIT_PARENT": "_default",
-               "ETOOLKIT_SENSITIVE": ["PASSWORD"],
                "GNUPGHOME": "%h/private/.gnupg",
-               "PASSWORD": "enc-val$1$vIBcoCNiYrsDLtF41uLuSEnppBjhliD0B8jwcBJcj/c=$KwOGe/y1dlxktDaCnJPIVNuaQ4Q7yNo="
+               "ETOOLKIT_TEST_PASSWORD": "enc-val$2$RCSZqq9pWrRDoCVYVHopyu1LzaJGfv8roVviqrLTBxM=$+YYrZbwTBuG0Pl+WMQrvxLUtq5j8qYuQqzoIwgoGt7AaWZCJz+E7qoDeg3wke70ST8U="
            }
        }
    }
 
-
-   dev_instance = etoolkit.EtoolkitInstance('dev', instances)
+   secret_instance = etoolkit.EtoolkitInstance('secret', instances)
 
    # fetch the variables before the processing stage (calling get_environ())
    # since raw_env_variables is a dict, it can be modified (f.i. .update())
-   dev_instance.raw_env_variables
+   secret_instance.raw_env_variables
 
-   dev_instance.master_password = 'the very secret passwd'  # or perhaps using getpass
-   env_vars = dev_instance.get_env()
-   print(env_vars['PASSWORD'])  # outputs: 'secret2'
+   secret_instance.master_password = 'The very secret passwd'  # or perhaps using getpass
+   env_vars = secret_instance.get_environ()
+   print(env_vars['ETOOLKIT_TEST_PASSWORD'])  # outputs: 'secret1'
    
-   inst.dump_env(env_vars)  # prints all values, with the exception of 'PASSWORD'
+   secret_instance.env_to_str(env_vars)  # prints all values, with the exception of 'ETOOLKIT_TEST_PASSWORD'
 
    # set the env. variables.
    os.environ.update(env_vars)
    ```
 
 
 ### Tips
@@ -342,15 +437,13 @@
 ## Author
 
 Simeon Simeonov - sgs @ LiberaChat
 
 
 ## [License](https://github.com/blackm0re/etoolkit/blob/master/LICENSE)
 
-Copyright (C) 2021-2022 Simeon Simeonov
+Copyright (C) 2021-2024 Simeon Simeonov
 All rights reserved.
 
 [Licensed](https://github.com/blackm0re/etoolkit/blob/master/LICENSE) under the
 GNU General Public License v3.0 or later.
 SPDX-License-Identifier: GPL-3.0-or-later
-
-
```

