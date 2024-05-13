# Comparing `tmp/borneo-5.4.1.tar.gz` & `tmp/borneo-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borneo-5.4.1.tar", last modified: Tue Aug  1 20:58:21 2023, max compression
+gzip compressed data, was "borneo-5.4.2.tar", last modified: Mon May 13 20:16:19 2024, max compression
```

## Comparing `borneo-5.4.1.tar` & `borneo-5.4.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.369788 borneo-5.4.1/
--rwxr-xr-x   0 gfeinber   (503) staff       (20)    13762 2023-08-01 20:49:10.000000 borneo-5.4.1/CHANGELOG.rst
--rw-r--r--   0 gfeinber   (503) staff       (20)     1870 2023-07-07 15:51:41.000000 borneo-5.4.1/LICENSE.txt
--rw-r--r--   0 gfeinber   (503) staff       (20)      105 2023-07-07 15:51:41.000000 borneo-5.4.1/MANIFEST.in
--rw-r--r--   0 gfeinber   (503) staff       (20)    17953 2023-08-01 20:58:21.369627 borneo-5.4.1/PKG-INFO
--rw-r--r--   0 gfeinber   (503) staff       (20)    17014 2023-07-07 15:51:41.000000 borneo-5.4.1/README.rst
--rw-r--r--   0 gfeinber   (503) staff       (20)    19783 2023-07-07 15:51:41.000000 borneo-5.4.1/THIRD_PARTY_LICENSES.txt
--rw-r--r--   0 gfeinber   (503) staff       (20)       38 2023-08-01 20:58:21.369823 borneo-5.4.1/setup.cfg
--rw-r--r--   0 gfeinber   (503) staff       (20)     2580 2023-07-07 15:51:41.000000 borneo-5.4.1/setup.py
-drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.362482 borneo-5.4.1/src/
-drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.367877 borneo-5.4.1/src/borneo/
--rw-r--r--   0 gfeinber   (503) staff       (20)     4316 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/__init__.py
--rw-r--r--   0 gfeinber   (503) staff       (20)     3198 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/auth.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    23978 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/client.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    72485 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/common.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    66359 2023-08-01 19:35:48.000000 borneo-5.4.1/src/borneo/config.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    34126 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/driver.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    16136 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/exception.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    54466 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/http.py
-drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.368870 borneo-5.4.1/src/borneo/iam/
--rw-r--r--   0 gfeinber   (503) staff       (20)      261 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/iam/__init__.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    19923 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/iam/iam.py
-drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.369364 borneo-5.4.1/src/borneo/kv/
--rw-r--r--   0 gfeinber   (503) staff       (20)      371 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/kv/__init__.py
--rw-r--r--   0 gfeinber   (503) staff       (20)      808 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/kv/exception.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    13520 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/kv/kv.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    81993 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/nson.py
--rw-r--r--   0 gfeinber   (503) staff       (20)     2754 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/nson_protocol.py
--rw-r--r--   0 gfeinber   (503) staff       (20)   202405 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/operations.py
--rw-r--r--   0 gfeinber   (503) staff       (20)   109954 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/query.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    34651 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/serde.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    29169 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/serdeutil.py
--rw-r--r--   0 gfeinber   (503) staff       (20)    33675 2023-07-07 15:51:41.000000 borneo-5.4.1/src/borneo/stats.py
--rw-r--r--   0 gfeinber   (503) staff       (20)      215 2023-08-01 20:49:10.000000 borneo-5.4.1/src/borneo/version.py
-drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2023-08-01 20:58:21.368639 borneo-5.4.1/src/borneo.egg-info/
--rw-r--r--   0 gfeinber   (503) staff       (20)    17953 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/PKG-INFO
--rw-r--r--   0 gfeinber   (503) staff       (20)      720 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/SOURCES.txt
--rw-r--r--   0 gfeinber   (503) staff       (20)        1 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/dependency_links.txt
--rw-r--r--   0 gfeinber   (503) staff       (20)       40 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/requires.txt
--rw-r--r--   0 gfeinber   (503) staff       (20)        7 2023-08-01 20:58:21.000000 borneo-5.4.1/src/borneo.egg-info/top_level.txt
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2024-05-13 20:16:19.933317 borneo-5.4.2/
+-rw-r--r--   0 gfeinber   (503) staff       (20)    15059 2024-05-13 19:33:04.000000 borneo-5.4.2/CHANGELOG.md
+-rw-r--r--   0 gfeinber   (503) staff       (20)     1845 2024-03-27 20:44:17.000000 borneo-5.4.2/LICENSE.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)      103 2024-01-27 19:38:29.000000 borneo-5.4.2/MANIFEST.in
+-rw-r--r--   0 gfeinber   (503) staff       (20)    16857 2024-05-13 20:16:19.933189 borneo-5.4.2/PKG-INFO
+-rw-r--r--   0 gfeinber   (503) staff       (20)    15915 2024-02-22 22:41:47.000000 borneo-5.4.2/README.md
+-rw-r--r--   0 gfeinber   (503) staff       (20)    19783 2024-03-27 20:44:17.000000 borneo-5.4.2/THIRD_PARTY_LICENSES.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)       38 2024-05-13 20:16:19.933352 borneo-5.4.2/setup.cfg
+-rw-r--r--   0 gfeinber   (503) staff       (20)     2582 2024-05-13 20:11:22.000000 borneo-5.4.2/setup.py
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2024-05-13 20:16:19.924950 borneo-5.4.2/src/
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2024-05-13 20:16:19.931199 borneo-5.4.2/src/borneo/
+-rw-r--r--   0 gfeinber   (503) staff       (20)     4791 2024-02-22 22:16:45.000000 borneo-5.4.2/src/borneo/__init__.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)     3247 2024-02-22 22:16:45.000000 borneo-5.4.2/src/borneo/auth.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    25527 2024-03-27 20:43:54.000000 borneo-5.4.2/src/borneo/client.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    75600 2024-03-27 20:43:54.000000 borneo-5.4.2/src/borneo/common.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    71740 2024-03-21 22:14:42.000000 borneo-5.4.2/src/borneo/config.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    36733 2024-02-22 22:16:45.000000 borneo-5.4.2/src/borneo/driver.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    16776 2024-03-27 20:43:54.000000 borneo-5.4.2/src/borneo/exception.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    55776 2024-03-27 20:43:54.000000 borneo-5.4.2/src/borneo/http.py
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2024-05-13 20:16:19.932084 borneo-5.4.2/src/borneo/iam/
+-rw-r--r--   0 gfeinber   (503) staff       (20)      261 2024-02-22 22:16:45.000000 borneo-5.4.2/src/borneo/iam/__init__.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    21103 2024-05-09 13:38:28.000000 borneo-5.4.2/src/borneo/iam/iam.py
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2024-05-13 20:16:19.932884 borneo-5.4.2/src/borneo/kv/
+-rw-r--r--   0 gfeinber   (503) staff       (20)      371 2024-02-22 22:16:45.000000 borneo-5.4.2/src/borneo/kv/__init__.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)      808 2024-02-22 22:16:45.000000 borneo-5.4.2/src/borneo/kv/exception.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    13520 2024-02-22 22:16:45.000000 borneo-5.4.2/src/borneo/kv/kv.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    96538 2024-03-27 20:43:54.000000 borneo-5.4.2/src/borneo/nson.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)     3538 2024-03-27 20:43:54.000000 borneo-5.4.2/src/borneo/nson_protocol.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)   227867 2024-03-27 20:43:54.000000 borneo-5.4.2/src/borneo/operations.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)   124187 2024-03-27 20:43:54.000000 borneo-5.4.2/src/borneo/query.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    35041 2024-03-27 20:43:54.000000 borneo-5.4.2/src/borneo/serde.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    30357 2024-04-17 19:41:44.000000 borneo-5.4.2/src/borneo/serdeutil.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)    33676 2024-02-22 22:16:45.000000 borneo-5.4.2/src/borneo/stats.py
+-rw-r--r--   0 gfeinber   (503) staff       (20)      215 2024-05-13 19:33:21.000000 borneo-5.4.2/src/borneo/version.py
+drwxr-xr-x   0 gfeinber   (503) staff       (20)        0 2024-05-13 20:16:19.931750 borneo-5.4.2/src/borneo.egg-info/
+-rw-r--r--   0 gfeinber   (503) staff       (20)    16857 2024-05-13 20:16:19.000000 borneo-5.4.2/src/borneo.egg-info/PKG-INFO
+-rw-r--r--   0 gfeinber   (503) staff       (20)      718 2024-05-13 20:16:19.000000 borneo-5.4.2/src/borneo.egg-info/SOURCES.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)        1 2024-05-13 20:16:19.000000 borneo-5.4.2/src/borneo.egg-info/dependency_links.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)       40 2024-05-13 20:16:19.000000 borneo-5.4.2/src/borneo.egg-info/requires.txt
+-rw-r--r--   0 gfeinber   (503) staff       (20)        7 2024-05-13 20:16:19.000000 borneo-5.4.2/src/borneo.egg-info/top_level.txt
```

### Comparing `borneo-5.4.1/LICENSE.txt` & `borneo-5.4.2/LICENSE.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-Copyright (c) 2018-2023 Oracle and/or its affiliates.  All rights reserved.
+Copyright (c) 2018, 2024 Oracle and/or its affiliates.
 
 The Universal Permissive License (UPL), Version 1.0
 
-Subject to the condition set forth below, permission is hereby granted to any person obtaining a copy
-of this software, associated documentation and/or data (collectively the "Software"), free of charge and
-under any and all copyright rights in the Software, and any and all patent rights owned or freely licensable
-by each licensor hereunder covering either (i) the unmodified Software as contributed to or provided by such
-licensor, or (ii) the Larger Works (as defined below), to deal in both
+Subject to the condition set forth below, permission is hereby granted to any
+person obtaining a copy of this software, associated documentation and/or data
+(collectively the "Software"), free of charge and under any and all copyright
+rights in the Software, and any and all patent rights owned or freely
+licensable by each licensor hereunder covering either (i) the unmodified
+Software as contributed to or provided by such licensor, or (ii) the Larger
+Works (as defined below), to deal in both
 
 (a) the Software, and
-(b) any piece of software and/or hardware listed in the lrgrwrks.txt file if one is included with the
-Software (each a “Larger Work” to which the Software is contributed by such licensors), without restriction,
-including without limitation the rights to copy, create derivative works of, display, perform, and distribute
-the Software and make, use, sell, offer for sale, import, export, have made, and have sold the Software and
-the Larger Work(s), and to sublicense the foregoing rights on either these or other terms.
+(b) any piece of software and/or hardware listed in the lrgrwrks.txt file if
+one is included with the Software (each a "Larger Work" to which the Software
+is contributed by such licensors),
+
+without restriction, including without limitation the rights to copy, create
+derivative works of, display, perform, and distribute the Software and make,
+use, sell, offer for sale, import, export, have made, and have sold the
+Software and the Larger Work(s), and to sublicense the foregoing rights on
+either these or other terms.
 
 This license is subject to the following condition:
-
-The above copyright notice and either this complete permission notice or at a minimum a reference to the UPL
-must be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
+The above copyright notice and either this complete permission notice or at
+a minimum a reference to the UPL must be included in all copies or
+substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `borneo-5.4.1/PKG-INFO` & `borneo-5.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borneo
-Version: 5.4.1
+Version: 5.4.2
 Summary: Oracle NoSQL Database Python SDK
 Home-page: https://nosql-python-sdk.readthedocs.io/en/stable/index.html
 Author: Oracle
 Author-email: george.feinberg@oracle.com
 License: Universal Permissive License 1.0
 Keywords: database,nosql,cloud,development
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,108 +14,82 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Oracle NoSQL Database Python SDK
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+# Oracle NoSQL Database Python SDK
 
-=====
-About
-=====
+## About
 
 This is the Python SDK for Oracle NoSQL Database. Python versions 3.5+ are
 supported. The SDK provides interfaces, documentation, and examples to help
 develop Python applications that connect to the Oracle NoSQL Database Cloud
 Service, Oracle NoSQL Database and to the Oracle NoSQL Cloud Simulator (which
 runs on a local machine).
 
 In order to run the Oracle NoSQL Cloud Simulator, a separate download is
 necessary from the Oracle NoSQL OTN download page. Throughout the documentation,
 the Oracle NoSQL Database Cloud Service and Cloud Simulator are referred to as
 the "cloud service" while the Oracle NoSQL Database is referred to as
-"on-premise." In the `API reference <https://nosql-python-sdk.readthedocs.io/en/
-stable/api.html>`_ classes and interfaces are noted if they are only relevant to
+"on-premise." In the [API reference](https://nosql-python-sdk.readthedocs.io/en/stable/api.html) classes and interfaces are noted if they are only relevant to
 a specific environment.
 
 The on-premise configuration requires a running instance of the Oracle NoSQL
-database. In addition a running proxy service is required. See `Oracle NoSQL
-Database Downloads <https://www.oracle.com/database/technologies/nosql-database-
-server-downloads.html>`_ for downloads, and see `Information about the proxy
-<https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-
-database/22.3/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72>`_ for
+database. In addition a running proxy service is required. See [Oracle NoSQL
+Database Downloads](https://www.oracle.com/database/technologies/nosql-database-server-downloads.html) for downloads, and see [Information about the proxy](https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-database/22.3/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72)  for
 proxy configuration information.
 
 This project is open source and maintained by Oracle Corp. The home page for the
-project is `here <https://nosql-python-sdk.readthedocs.io/en/stable/index.
-html>`_.
+project is [here](https://nosql-python-sdk.readthedocs.io/en/stable/index.html).
 
-============
-Installation
-============
+## Installation
 
 The SDK can be installed using pip. If using Python 3 the command may be pip3::
 
     pip install borneo
 
 If you are using the Oracle NoSQL Database cloud service you will also need to
 install the oci package::
 
     pip install oci
 
-See `the installation guide <https://nosql-python-sdk.readthedocs.io/en/stable/
-installation.html>`_ for additional requirements and and alternative install
+See [the installation guide](https://nosql-python-sdk.readthedocs.io/en/stable/installation.html) for additional requirements and and alternative install
 methods.
 
-========
-Examples
-========
+## Examples
 
-Examples can be found `on GitHub <https://github.com/oracle/nosql-python-sdk/
-tree/master/examples>`_.
+Examples can be found [on GitHub](https://github.com/oracle/nosql-python-sdk/tree/master/examples)
 
 Examples include simple, standalone programs. They include comments about how
 they can be configured and run in the different supported environments.
 
-=============
-Documentation
-=============
-
-The `documentation <https://nosql-python-sdk.readthedocs.io/en/stable>`_ has
-information on using the SDK as well as an `API reference <https://nosql-python-
-sdk.readthedocs.io/en/stable/api.html>`_ describing the classes.
-
-=======
-Changes
-=======
-
-See the `Changelog <https://github.com/oracle/nosql-python-sdk/blob/master/
-CHANGELOG.rst>`_.
-
-====
-Help
-====
+## Documentation
 
- * Open an issue in the `Issues <https://github.com/oracle/nosql-python-sdk/
-   issues>`_ page.
+The [documentation](https://nosql-python-sdk.readthedocs.io/en/stable) has
+information on using the SDK as well as an [API reference](https://nosql-python-sdk.readthedocs.io/en/stable/api.html) describing the classes.
+
+## Changes
+
+See the [Changelog](https://github.com/oracle/nosql-python-sdk/blob/master/CHANGELOG.md)
+
+## Help
+
+ * Open an issue in the [Issues](https://github.com/oracle/nosql-python-sdk/issues) page.
  * Email to nosql_sdk_help_grp@oracle.com.
- * `Oracle NoSQL Developer Forum <https://community.oracle.com/community/
-   groundbreakers/database/nosql_database>`_.
+ * [Oracle NoSQL Developer Forum](https://community.oracle.com/community/groundbreakers/database/nosql_database).
 
 When requesting help please be sure to include as much detail as possible,
 including version of the SDK and **simple**, standalone example code as needed.
 
-==========
-Quickstart
-==========
+## Quickstart
 
 The following is a quick start tutorial to run a simple program in the supported
 environments. The same template source code is used for all environments. The
 first step is to cut the program below and paste it into an editor for minor
 modifications. The instructions assume that is stored as quickstart.py, but you
 can use any name you like. The quickstart example supports 3 environments:
 
@@ -123,275 +97,272 @@
 2. Oracle NoSQL Cloud Simulator
 3. Oracle NoSQL Database on-premise, using the proxy server
 
 See `Running Quickstart`_ to
 run the quickstart program in different environments. The instructions assume
 that the *borneo* package has been installed.
 
-.. code-block:: pycon
-
-    #
-    # Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
-    #
-    # Licensed under the Universal Permissive License v 1.0 as shown at
-    #  https://oss.oracle.com/licenses/upl/
-    #
-
-    #
-    # This is a simple quickstart to demonstrate use of the Python driver for
-    # the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
-    # Database Cloud Service, against the Cloud Simulator, or against an
-    # on-premise Oracle NoSQL database.
-    #
-    # Usage:
-    #   python quickstart.py <cloud | cloudsim | kvstore>
-    #
-    # Use cloud for the Cloud Service
-    # Use cloudsim for the Cloud Simulator
-    # Use kvstore for the on-premise database
-    #
-    # This example is not intended to be an exhaustive overview of the API,
-    # which has a number of additional operations.
-    #
-    # Requirements:
-    #  1. Python 3.5+
-    #  2. Python dependencies (install using pip or other mechanism):
-    #   o requests
-    #   o oci (only if running against the Cloud Service)
-    #  3. If running against the Cloud Simulator, it can be downloaded from
-    #  here:
-    #   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
-    #  It requires Java
-    #  4. If running against the Oracle NoSQL Database Cloud Service an account
-    #  must be used.
-    #
-
-    import sys
-
-    from borneo import (
-        AuthorizationProvider, DeleteRequest, GetRequest,
-        IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
-        QueryRequest, Regions, TableLimits, TableRequest)
-    from borneo.iam import SignatureProvider
-    from borneo.kv import StoreAccessTokenProvider
-
-
-    #
-    # EDIT: these values based on desired region and/or endpoint for a local
-    # server
-    #
-    cloud_region = Regions.EU_ZURICH_1
-    cloudsim_endpoint = 'localhost:8080'
-    kvstore_endpoint = 'localhost:80'
-    cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
-
-    # Cloud Service Only
-    #
-    # EDIT: set these variables to the credentials to use if you are not using
-    # a configuration file in ~/.oci/config
-    # Use of these credentials vs a file is determined by a value of tenancy
-    # other than None.
-    #
-    tenancy = None  # tenancy'd OCID (string)
-    user = None  # user's OCID (string)
-    private_key = 'path-to-private-key-or-private-key-content'
-    fingerprint = 'fingerprint for uploaded public key'
-    # pass phrase (string) for private key, or None if not set
-    pass_phrase = None
-
-
-    class CloudsimAuthorizationProvider(AuthorizationProvider):
-        """
-        Cloud Simulator Only.
-
-        This class is used as an AuthorizationProvider when using the Cloud
-        Simulator, which has no security configuration. It accepts a string
-        tenant_id that is used as a simple namespace for tables.
-        """
-
-        def __init__(self, tenant_id):
-            super(CloudsimAuthorizationProvider, self).__init__()
-            self._tenant_id = tenant_id
-
-        def close(self):
-            pass
-
-        def get_authorization_string(self, request=None):
-            return 'Bearer ' + self._tenant_id
-
-
-    def get_handle(nosql_env):
-        """
-        Returns a NoSQLHandle based on the requested environment. The
-        differences among the supported environments are encapsulated in this
-        method.
-        """
-        if nosql_env == 'cloud':
-            endpoint = cloud_region
-            #
-            # Get credentials using SignatureProvider. SignatureProvider has
-            # several ways to accept credentials. See the documentation:
-            #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
-            #
-            if tenancy is not None:
-                print('Using directly provided credentials')
-                #
-                # Credentials are provided directly
-                #
-                provider = SignatureProvider(tenant_id=tenancy,
-                                             user_id=user,
-                                             fingerprint=fingerprint,
-                                             private_key=private_key,
-                                             pass_phrase=pass_phrase)
-            else:
-                #
-                # Credentials will come from a file.
-                #
-                # By default the file is ~/.oci/config. A config_file = <path>
-                # argument can be passed to specify a different file.
-                #
-                print('Using credentials and DEFAULT profile from ' +
-                      '~/.oci/config')
-                provider = SignatureProvider()
-        elif nosql_env == 'cloudsim':
-            print('Using cloud simulator endpoint ' + cloudsim_endpoint)
-            endpoint = cloudsim_endpoint
-            provider = CloudsimAuthorizationProvider(cloudsim_id)
-
-        elif nosql_env == 'kvstore':
-            print('Using on-premise endpoint ' + kvstore_endpoint)
-            endpoint = kvstore_endpoint
-            provider = StoreAccessTokenProvider()
+``` python
 
+#
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
+#
+# Licensed under the Universal Permissive License v 1.0 as shown at
+#  https://oss.oracle.com/licenses/upl/
+#
+
+#
+# This is a simple quickstart to demonstrate use of the Python driver for
+# the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
+# Database Cloud Service, against the Cloud Simulator, or against an
+# on-premise Oracle NoSQL database.
+#
+# Usage:
+#   python quickstart.py <cloud | cloudsim | kvstore>
+#
+# Use cloud for the Cloud Service
+# Use cloudsim for the Cloud Simulator
+# Use kvstore for the on-premise database
+#
+# This example is not intended to be an exhaustive overview of the API,
+# which has a number of additional operations.
+#
+# Requirements:
+#  1. Python 3.5+
+#  2. Python dependencies (install using pip or other mechanism):
+#   o requests
+#   o oci (only if running against the Cloud Service)
+#  3. If running against the Cloud Simulator, it can be downloaded from
+#  here:
+#   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
+#  It requires Java
+#  4. If running against the Oracle NoSQL Database Cloud Service an account
+#  must be used.
+#
+
+import sys
+
+from borneo import (
+    AuthorizationProvider, DeleteRequest, GetRequest,
+    IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
+    QueryRequest, Regions, TableLimits, TableRequest)
+from borneo.iam import SignatureProvider
+from borneo.kv import StoreAccessTokenProvider
+
+
+#
+# EDIT: these values based on desired region and/or endpoint for a local
+# server
+#
+cloud_region = Regions.EU_ZURICH_1
+cloudsim_endpoint = 'localhost:8080'
+kvstore_endpoint = 'localhost:80'
+cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
+
+# Cloud Service Only
+#
+# EDIT: set these variables to the credentials to use if you are not using
+# a configuration file in ~/.oci/config
+# Use of these credentials vs a file is determined by a value of tenancy
+# other than None.
+#
+tenancy = None  # tenancy'd OCID (string)
+user = None  # user's OCID (string)
+private_key = 'path-to-private-key-or-private-key-content'
+fingerprint = 'fingerprint for uploaded public key'
+# pass phrase (string) for private key, or None if not set
+pass_phrase = None
+
+
+class CloudsimAuthorizationProvider(AuthorizationProvider):
+    """
+    Cloud Simulator Only.
+
+    This class is used as an AuthorizationProvider when using the Cloud
+    Simulator, which has no security configuration. It accepts a string
+    tenant_id that is used as a simple namespace for tables.
+    """
+
+    def __init__(self, tenant_id):
+        super(CloudsimAuthorizationProvider, self).__init__()
+        self._tenant_id = tenant_id
+
+    def close(self):
+        pass
+
+    def get_authorization_string(self, request=None):
+        return 'Bearer ' + self._tenant_id
+
+
+def get_handle(nosql_env):
+    """
+    Returns a NoSQLHandle based on the requested environment. The
+    differences among the supported environments are encapsulated in this
+    method.
+    """
+    if nosql_env == 'cloud':
+        endpoint = cloud_region
+        #
+        # Get credentials using SignatureProvider. SignatureProvider has
+        # several ways to accept credentials. See the documentation:
+        #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
+        #
+        if tenancy is not None:
+            print('Using directly provided credentials')
+            #
+            # Credentials are provided directly
+            #
+            provider = SignatureProvider(tenant_id=tenancy,
+                                         user_id=user,
+                                         fingerprint=fingerprint,
+                                         private_key=private_key,
+                                         pass_phrase=pass_phrase)
         else:
-            raise IllegalArgumentException('Unknown environment: ' + nosql_env)
-
-        return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
-
-
-    def main():
-
-        table_name = 'PythonQuickstart'
-
-        if len(sys.argv) != 2:
-            print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
-            raise SystemExit
-
-        nosql_env = sys.argv[1:][0]
-        print('Using environment: ' + str(nosql_env))
-
-        handle = None
-        try:
-
-            #
-            # Create a handle
             #
-            handle = get_handle(nosql_env)
-
+            # Credentials will come from a file.
             #
-            # Create a table
-            #
-            statement = (
-                'Create table if not exists {} (id integer, sid integer, ' +
-                'name string, primary key(shard(sid), id))').format(table_name)
-            request = TableRequest().set_statement(statement).set_table_limits(
-                TableLimits(30, 10, 1))
-            handle.do_table_request(request, 50000, 3000)
-            print('After create table')
-
-            #
-            # Put a few rows
-            #
-            request = PutRequest().set_table_name(table_name)
-            for i in range(10):
-                value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
-                request.set_value(value)
-                handle.put(request)
-            print('After put of 10 rows')
-
+            # By default the file is ~/.oci/config. A config_file = <path>
+            # argument can be passed to specify a different file.
             #
-            # Get the row
-            #
-            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                table_name)
-            result = handle.get(request)
-            print('After get: ' + str(result))
-
-            #
-            # Query, using a range
-            #
-            statement = (
-                'select * from ' + table_name + ' where id > 2 and id < 8')
-            request = QueryRequest().set_statement(statement)
-            print('Query results for: ' + statement)
-            #
-            # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
-            # may be more results, so queries should generally be run in a loop.
-            # It is possible for single request to return no results but the
-            # query still not done, indicating that the query loop should
-            # continue.
-            #
-            while True:
-                result = handle.query(request)
-                for r in result.get_results():
-                    print('\t' + str(r))
-                if request.is_done():
-                    break
-
-            #
-            # Delete the row
-            #
-            request = DeleteRequest().set_table_name(table_name).set_key(
-                {'id': 1, 'sid': 0})
-            result = handle.delete(request)
-            print('After delete: ' + str(result))
-
-            #
-            # Get again to show deletion
-            #
-            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                table_name)
-            result = handle.get(request)
-            print('After get (should be None): ' + str(result))
-
-            #
-            # Drop the table
-            #
-            request = TableRequest().set_statement(
-                'drop table if exists {} '.format(table_name))
-            result = handle.table_request(request)
-
-            #
-            # Table drop can take time, depending on the state of the system.
-            # If this wait fails the table will still probably been dropped
-            #
-            result.wait_for_completion(handle, 40000, 2000)
-            print('After drop table')
-
-            print('Quickstart is complete')
-        except Exception as e:
-            print(e)
-        finally:
-            # If the handle isn't closed Python will not exit properly
-            if handle is not None:
-                handle.close()
-
-
-    if __name__ == '__main__':
-        main()
-
-Running Quickstart
-==================
+            print('Using credentials and DEFAULT profile from ' +
+                  '~/.oci/config')
+            provider = SignatureProvider()
+    elif nosql_env == 'cloudsim':
+        print('Using cloud simulator endpoint ' + cloudsim_endpoint)
+        endpoint = cloudsim_endpoint
+        provider = CloudsimAuthorizationProvider(cloudsim_id)
+
+    elif nosql_env == 'kvstore':
+        print('Using on-premise endpoint ' + kvstore_endpoint)
+        endpoint = kvstore_endpoint
+        provider = StoreAccessTokenProvider()
+
+    else:
+        raise IllegalArgumentException('Unknown environment: ' + nosql_env)
+
+    return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
+
+
+def main():
+
+    table_name = 'PythonQuickstart'
+
+    if len(sys.argv) != 2:
+        print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
+        raise SystemExit
+
+    nosql_env = sys.argv[1:][0]
+    print('Using environment: ' + str(nosql_env))
+
+    handle = None
+    try:
+
+        #
+        # Create a handle
+        #
+        handle = get_handle(nosql_env)
+
+        #
+        # Create a table
+        #
+        statement = (
+            'Create table if not exists {} (id integer, sid integer, ' +
+            'name string, primary key(shard(sid), id))').format(table_name)
+        request = TableRequest().set_statement(statement).set_table_limits(
+            TableLimits(30, 10, 1))
+        handle.do_table_request(request, 50000, 3000)
+        print('After create table')
+
+        #
+        # Put a few rows
+        #
+        request = PutRequest().set_table_name(table_name)
+        for i in range(10):
+            value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
+            request.set_value(value)
+            handle.put(request)
+        print('After put of 10 rows')
+
+        #
+        # Get the row
+        #
+        request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+            table_name)
+        result = handle.get(request)
+        print('After get: ' + str(result))
+
+        #
+        # Query, using a range
+        #
+        statement = (
+            'select * from ' + table_name + ' where id > 2 and id < 8')
+        request = QueryRequest().set_statement(statement)
+        print('Query results for: ' + statement)
+        #
+        # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
+        # may be more results, so queries should generally be run in a loop.
+        # It is possible for single request to return no results but the
+        # query still not done, indicating that the query loop should
+        # continue.
+        #
+        while True:
+            result = handle.query(request)
+            for r in result.get_results():
+                print('\t' + str(r))
+            if request.is_done():
+                break
+
+        #
+        # Delete the row
+        #
+        request = DeleteRequest().set_table_name(table_name).set_key(
+            {'id': 1, 'sid': 0})
+        result = handle.delete(request)
+        print('After delete: ' + str(result))
+
+        #
+        # Get again to show deletion
+        #
+        request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+            table_name)
+        result = handle.get(request)
+        print('After get (should be None): ' + str(result))
+
+        #
+        # Drop the table
+        #
+        request = TableRequest().set_statement(
+            'drop table if exists {} '.format(table_name))
+        result = handle.table_request(request)
+
+        #
+        # Table drop can take time, depending on the state of the system.
+        # If this wait fails the table will still probably been dropped
+        #
+        result.wait_for_completion(handle, 40000, 2000)
+        print('After drop table')
+
+        print('Quickstart is complete')
+    except Exception as e:
+        print(e)
+    finally:
+        # If the handle isn't closed Python will not exit properly
+        if handle is not None:
+            handle.close()
+
+
+if __name__ == '__main__':
+    main()
+```
+## Running Quickstart
 
-Run Against the Oracle NoSQL Database Cloud Service
-===================================================
+### Run Against the Oracle NoSQL Database Cloud Service
 
 Running against the Cloud Service requires an Oracle Cloud account. See
-`Configure for the Cloud Service <https://nosql-python-sdk.readthedocs.io/en/
-stable/installation.html#configure-for-the-cloud-service>`_ for information on
+[Configure for the Cloud Service](https://nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-the-cloud-service) for information on
 getting an account and acquiring required credentials.
 
 1. Collect the following information:
 
  * Tenancy ID
  * User ID
  * API signing key (private key file in PEM format)
@@ -402,64 +373,59 @@
    credentials in the program:
 
    * Directly provide the credential information. To use this method, modify the
      values of the variables at the top of the program: *tenancy*, *user*,
      *private_key*, *fingerprint*, and *pass_phrase*, setting them to the
      corresponding information you've collected.
    * Using a configuration file. In this case the information you've collected
-     goes into a file, ~/.oci/config. `Configure for the Cloud Service <https://
-     nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-
-     the-cloud-service>`_ describes the contents of the file. It will look like
+     goes into a file, ~/.oci/config. [Configure for the Cloud Service](https://nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-the-cloud-service) describes the contents of the file. It will look like
      this::
 
       [DEFAULT]
       tenancy=<your-tenancy-id>
       user=<your-user-id>
       fingerprint=<fingerprint-of-your-public-key>
       key_file=<path-to-your-private-key-file>
       pass_phrase=<optional-pass-phrase-for-key-file>
 
 3. Decide which region you want to use and modify the *cloud_region* variable to
-   the desired region. See `Regions documentation <https://nosql-python-sdk.
-   readthedocs.io/en/stable/api/borneo.Regions.html>`_ for possible regions. Not
+   the desired region. See [Regions documentation](https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.Regions.html) for possible regions. Not
    all support the Oracle NoSQL Database Cloud Service.
 
 4. Run the program:
 
 .. code-block:: pycon
 
     python quickstart.py cloud
 
-Run Against the Oracle NoSQL Cloud Simulator
-============================================
+### Run Against the Oracle NoSQL Cloud Simulator
 
 Running against the Oracle NoSQL Cloud Simulator requires a running Cloud
-Simulator instance. See `Configure for the Cloud Simulator <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator>`_ for information on how to
+Simulator instance. See [Configure for the Cloud Simulator](https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator) for information on how to
 download and start the Cloud Simulator.
 
 1. Start the Cloud Simulator based on instructions above. Note the HTTP port
    used. By default it is *8080* on *localhost*.
 
 2. The *quickstart.py* program defaults to *localhost:8080* so if the Cloud
    Simulator was started using default values no editing is required.
 
 3. Run the program:
 
 .. code-block:: pycon
 
     python quickstart.py cloudsim
 
-Run Against Oracle NoSQL on-premise
-===================================
+### Run Against Oracle NoSQL on-premise
 
 Running against the Oracle NoSQL Database on-premise requires a running Oracle
 NoSQL Database instance as well as a running NoSQL Proxy server instance. The
 program will connect to the proxy server.
 
-See `Configure for On-Premise Oracle NoSQL Database <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database>`_ for information on how to
+See [Configure for On-Premise Oracle NoSQL Database](https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database) for information on how to
 download and start the database instance and proxy server. The database and
 proxy should be started without security enabled for this quickstart program to
 operate correctly. A secure configuration requires a secure proxy and more
 complex configuration.
 
 1. Start the Oracle NoSQL Database and proxy server based on instructions above.
    Note the HTTP port used. By default the endpoint is *localhost:80*.
@@ -469,27 +435,21 @@
 
 3. Run the program:
 
 .. code-block:: pycon
 
     python quickstart.py kvstore
 
-=======
-License
-=======
+## Contributing
 
-Copyright (C) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+This project welcomes contributions from the community. Before submitting a pull request, please [review our contribution guide](./CONTRIBUTING.md)
 
-This SDK is licensed under the Universal Permissive License 1.0. See `LICENSE
-<./LICENSE.txt>`_ for details.
+## Security
 
-============
-Contributing
-============
+Please consult the [security guide](./SECURITY.md) for our responsible security vulnerability disclosure process
 
-See `CONTRIBUTING <./CONTRIBUTING.rst>`_
+## License
 
-========
-Security
-========
+Copyright (c) 2018, 2024 Oracle and/or its affiliates.
 
-See `SECURITY <./SECURITY.rst>`_
+Released under the Universal Permissive License v1.0 as shown at
+<https://oss.oracle.com/licenses/upl/>.
```

### Comparing `borneo-5.4.1/README.rst` & `borneo-5.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,98 +1,72 @@
-Oracle NoSQL Database Python SDK
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+# Oracle NoSQL Database Python SDK
 
-=====
-About
-=====
+## About
 
 This is the Python SDK for Oracle NoSQL Database. Python versions 3.5+ are
 supported. The SDK provides interfaces, documentation, and examples to help
 develop Python applications that connect to the Oracle NoSQL Database Cloud
 Service, Oracle NoSQL Database and to the Oracle NoSQL Cloud Simulator (which
 runs on a local machine).
 
 In order to run the Oracle NoSQL Cloud Simulator, a separate download is
 necessary from the Oracle NoSQL OTN download page. Throughout the documentation,
 the Oracle NoSQL Database Cloud Service and Cloud Simulator are referred to as
 the "cloud service" while the Oracle NoSQL Database is referred to as
-"on-premise." In the `API reference <https://nosql-python-sdk.readthedocs.io/en/
-stable/api.html>`_ classes and interfaces are noted if they are only relevant to
+"on-premise." In the [API reference](https://nosql-python-sdk.readthedocs.io/en/stable/api.html) classes and interfaces are noted if they are only relevant to
 a specific environment.
 
 The on-premise configuration requires a running instance of the Oracle NoSQL
-database. In addition a running proxy service is required. See `Oracle NoSQL
-Database Downloads <https://www.oracle.com/database/technologies/nosql-database-
-server-downloads.html>`_ for downloads, and see `Information about the proxy
-<https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-
-database/22.3/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72>`_ for
+database. In addition a running proxy service is required. See [Oracle NoSQL
+Database Downloads](https://www.oracle.com/database/technologies/nosql-database-server-downloads.html) for downloads, and see [Information about the proxy](https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-database/22.3/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72)  for
 proxy configuration information.
 
 This project is open source and maintained by Oracle Corp. The home page for the
-project is `here <https://nosql-python-sdk.readthedocs.io/en/stable/index.
-html>`_.
+project is [here](https://nosql-python-sdk.readthedocs.io/en/stable/index.html).
 
-============
-Installation
-============
+## Installation
 
 The SDK can be installed using pip. If using Python 3 the command may be pip3::
 
     pip install borneo
 
 If you are using the Oracle NoSQL Database cloud service you will also need to
 install the oci package::
 
     pip install oci
 
-See `the installation guide <https://nosql-python-sdk.readthedocs.io/en/stable/
-installation.html>`_ for additional requirements and and alternative install
+See [the installation guide](https://nosql-python-sdk.readthedocs.io/en/stable/installation.html) for additional requirements and and alternative install
 methods.
 
-========
-Examples
-========
+## Examples
 
-Examples can be found `on GitHub <https://github.com/oracle/nosql-python-sdk/
-tree/master/examples>`_.
+Examples can be found [on GitHub](https://github.com/oracle/nosql-python-sdk/tree/master/examples)
 
 Examples include simple, standalone programs. They include comments about how
 they can be configured and run in the different supported environments.
 
-=============
-Documentation
-=============
-
-The `documentation <https://nosql-python-sdk.readthedocs.io/en/stable>`_ has
-information on using the SDK as well as an `API reference <https://nosql-python-
-sdk.readthedocs.io/en/stable/api.html>`_ describing the classes.
-
-=======
-Changes
-=======
-
-See the `Changelog <https://github.com/oracle/nosql-python-sdk/blob/master/
-CHANGELOG.rst>`_.
-
-====
-Help
-====
+## Documentation
 
- * Open an issue in the `Issues <https://github.com/oracle/nosql-python-sdk/
-   issues>`_ page.
+The [documentation](https://nosql-python-sdk.readthedocs.io/en/stable) has
+information on using the SDK as well as an [API reference](https://nosql-python-sdk.readthedocs.io/en/stable/api.html) describing the classes.
+
+## Changes
+
+See the [Changelog](https://github.com/oracle/nosql-python-sdk/blob/master/CHANGELOG.md)
+
+## Help
+
+ * Open an issue in the [Issues](https://github.com/oracle/nosql-python-sdk/issues) page.
  * Email to nosql_sdk_help_grp@oracle.com.
- * `Oracle NoSQL Developer Forum <https://community.oracle.com/community/
-   groundbreakers/database/nosql_database>`_.
+ * [Oracle NoSQL Developer Forum](https://community.oracle.com/community/groundbreakers/database/nosql_database).
 
 When requesting help please be sure to include as much detail as possible,
 including version of the SDK and **simple**, standalone example code as needed.
 
-==========
-Quickstart
-==========
+## Quickstart
 
 The following is a quick start tutorial to run a simple program in the supported
 environments. The same template source code is used for all environments. The
 first step is to cut the program below and paste it into an editor for minor
 modifications. The instructions assume that is stored as quickstart.py, but you
 can use any name you like. The quickstart example supports 3 environments:
 
@@ -100,275 +74,272 @@
 2. Oracle NoSQL Cloud Simulator
 3. Oracle NoSQL Database on-premise, using the proxy server
 
 See `Running Quickstart`_ to
 run the quickstart program in different environments. The instructions assume
 that the *borneo* package has been installed.
 
-.. code-block:: pycon
-
-    #
-    # Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
-    #
-    # Licensed under the Universal Permissive License v 1.0 as shown at
-    #  https://oss.oracle.com/licenses/upl/
-    #
-
-    #
-    # This is a simple quickstart to demonstrate use of the Python driver for
-    # the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
-    # Database Cloud Service, against the Cloud Simulator, or against an
-    # on-premise Oracle NoSQL database.
-    #
-    # Usage:
-    #   python quickstart.py <cloud | cloudsim | kvstore>
-    #
-    # Use cloud for the Cloud Service
-    # Use cloudsim for the Cloud Simulator
-    # Use kvstore for the on-premise database
-    #
-    # This example is not intended to be an exhaustive overview of the API,
-    # which has a number of additional operations.
-    #
-    # Requirements:
-    #  1. Python 3.5+
-    #  2. Python dependencies (install using pip or other mechanism):
-    #   o requests
-    #   o oci (only if running against the Cloud Service)
-    #  3. If running against the Cloud Simulator, it can be downloaded from
-    #  here:
-    #   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
-    #  It requires Java
-    #  4. If running against the Oracle NoSQL Database Cloud Service an account
-    #  must be used.
-    #
-
-    import sys
-
-    from borneo import (
-        AuthorizationProvider, DeleteRequest, GetRequest,
-        IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
-        QueryRequest, Regions, TableLimits, TableRequest)
-    from borneo.iam import SignatureProvider
-    from borneo.kv import StoreAccessTokenProvider
-
-
-    #
-    # EDIT: these values based on desired region and/or endpoint for a local
-    # server
-    #
-    cloud_region = Regions.EU_ZURICH_1
-    cloudsim_endpoint = 'localhost:8080'
-    kvstore_endpoint = 'localhost:80'
-    cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
-
-    # Cloud Service Only
-    #
-    # EDIT: set these variables to the credentials to use if you are not using
-    # a configuration file in ~/.oci/config
-    # Use of these credentials vs a file is determined by a value of tenancy
-    # other than None.
-    #
-    tenancy = None  # tenancy'd OCID (string)
-    user = None  # user's OCID (string)
-    private_key = 'path-to-private-key-or-private-key-content'
-    fingerprint = 'fingerprint for uploaded public key'
-    # pass phrase (string) for private key, or None if not set
-    pass_phrase = None
-
-
-    class CloudsimAuthorizationProvider(AuthorizationProvider):
-        """
-        Cloud Simulator Only.
-
-        This class is used as an AuthorizationProvider when using the Cloud
-        Simulator, which has no security configuration. It accepts a string
-        tenant_id that is used as a simple namespace for tables.
-        """
-
-        def __init__(self, tenant_id):
-            super(CloudsimAuthorizationProvider, self).__init__()
-            self._tenant_id = tenant_id
-
-        def close(self):
-            pass
-
-        def get_authorization_string(self, request=None):
-            return 'Bearer ' + self._tenant_id
-
-
-    def get_handle(nosql_env):
-        """
-        Returns a NoSQLHandle based on the requested environment. The
-        differences among the supported environments are encapsulated in this
-        method.
-        """
-        if nosql_env == 'cloud':
-            endpoint = cloud_region
-            #
-            # Get credentials using SignatureProvider. SignatureProvider has
-            # several ways to accept credentials. See the documentation:
-            #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
-            #
-            if tenancy is not None:
-                print('Using directly provided credentials')
-                #
-                # Credentials are provided directly
-                #
-                provider = SignatureProvider(tenant_id=tenancy,
-                                             user_id=user,
-                                             fingerprint=fingerprint,
-                                             private_key=private_key,
-                                             pass_phrase=pass_phrase)
-            else:
-                #
-                # Credentials will come from a file.
-                #
-                # By default the file is ~/.oci/config. A config_file = <path>
-                # argument can be passed to specify a different file.
-                #
-                print('Using credentials and DEFAULT profile from ' +
-                      '~/.oci/config')
-                provider = SignatureProvider()
-        elif nosql_env == 'cloudsim':
-            print('Using cloud simulator endpoint ' + cloudsim_endpoint)
-            endpoint = cloudsim_endpoint
-            provider = CloudsimAuthorizationProvider(cloudsim_id)
-
-        elif nosql_env == 'kvstore':
-            print('Using on-premise endpoint ' + kvstore_endpoint)
-            endpoint = kvstore_endpoint
-            provider = StoreAccessTokenProvider()
+``` python
 
+#
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
+#
+# Licensed under the Universal Permissive License v 1.0 as shown at
+#  https://oss.oracle.com/licenses/upl/
+#
+
+#
+# This is a simple quickstart to demonstrate use of the Python driver for
+# the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
+# Database Cloud Service, against the Cloud Simulator, or against an
+# on-premise Oracle NoSQL database.
+#
+# Usage:
+#   python quickstart.py <cloud | cloudsim | kvstore>
+#
+# Use cloud for the Cloud Service
+# Use cloudsim for the Cloud Simulator
+# Use kvstore for the on-premise database
+#
+# This example is not intended to be an exhaustive overview of the API,
+# which has a number of additional operations.
+#
+# Requirements:
+#  1. Python 3.5+
+#  2. Python dependencies (install using pip or other mechanism):
+#   o requests
+#   o oci (only if running against the Cloud Service)
+#  3. If running against the Cloud Simulator, it can be downloaded from
+#  here:
+#   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
+#  It requires Java
+#  4. If running against the Oracle NoSQL Database Cloud Service an account
+#  must be used.
+#
+
+import sys
+
+from borneo import (
+    AuthorizationProvider, DeleteRequest, GetRequest,
+    IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
+    QueryRequest, Regions, TableLimits, TableRequest)
+from borneo.iam import SignatureProvider
+from borneo.kv import StoreAccessTokenProvider
+
+
+#
+# EDIT: these values based on desired region and/or endpoint for a local
+# server
+#
+cloud_region = Regions.EU_ZURICH_1
+cloudsim_endpoint = 'localhost:8080'
+kvstore_endpoint = 'localhost:80'
+cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
+
+# Cloud Service Only
+#
+# EDIT: set these variables to the credentials to use if you are not using
+# a configuration file in ~/.oci/config
+# Use of these credentials vs a file is determined by a value of tenancy
+# other than None.
+#
+tenancy = None  # tenancy'd OCID (string)
+user = None  # user's OCID (string)
+private_key = 'path-to-private-key-or-private-key-content'
+fingerprint = 'fingerprint for uploaded public key'
+# pass phrase (string) for private key, or None if not set
+pass_phrase = None
+
+
+class CloudsimAuthorizationProvider(AuthorizationProvider):
+    """
+    Cloud Simulator Only.
+
+    This class is used as an AuthorizationProvider when using the Cloud
+    Simulator, which has no security configuration. It accepts a string
+    tenant_id that is used as a simple namespace for tables.
+    """
+
+    def __init__(self, tenant_id):
+        super(CloudsimAuthorizationProvider, self).__init__()
+        self._tenant_id = tenant_id
+
+    def close(self):
+        pass
+
+    def get_authorization_string(self, request=None):
+        return 'Bearer ' + self._tenant_id
+
+
+def get_handle(nosql_env):
+    """
+    Returns a NoSQLHandle based on the requested environment. The
+    differences among the supported environments are encapsulated in this
+    method.
+    """
+    if nosql_env == 'cloud':
+        endpoint = cloud_region
+        #
+        # Get credentials using SignatureProvider. SignatureProvider has
+        # several ways to accept credentials. See the documentation:
+        #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
+        #
+        if tenancy is not None:
+            print('Using directly provided credentials')
+            #
+            # Credentials are provided directly
+            #
+            provider = SignatureProvider(tenant_id=tenancy,
+                                         user_id=user,
+                                         fingerprint=fingerprint,
+                                         private_key=private_key,
+                                         pass_phrase=pass_phrase)
         else:
-            raise IllegalArgumentException('Unknown environment: ' + nosql_env)
-
-        return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
-
-
-    def main():
-
-        table_name = 'PythonQuickstart'
-
-        if len(sys.argv) != 2:
-            print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
-            raise SystemExit
-
-        nosql_env = sys.argv[1:][0]
-        print('Using environment: ' + str(nosql_env))
-
-        handle = None
-        try:
-
-            #
-            # Create a handle
             #
-            handle = get_handle(nosql_env)
-
+            # Credentials will come from a file.
             #
-            # Create a table
-            #
-            statement = (
-                'Create table if not exists {} (id integer, sid integer, ' +
-                'name string, primary key(shard(sid), id))').format(table_name)
-            request = TableRequest().set_statement(statement).set_table_limits(
-                TableLimits(30, 10, 1))
-            handle.do_table_request(request, 50000, 3000)
-            print('After create table')
-
-            #
-            # Put a few rows
-            #
-            request = PutRequest().set_table_name(table_name)
-            for i in range(10):
-                value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
-                request.set_value(value)
-                handle.put(request)
-            print('After put of 10 rows')
-
+            # By default the file is ~/.oci/config. A config_file = <path>
+            # argument can be passed to specify a different file.
             #
-            # Get the row
-            #
-            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                table_name)
-            result = handle.get(request)
-            print('After get: ' + str(result))
-
-            #
-            # Query, using a range
-            #
-            statement = (
-                'select * from ' + table_name + ' where id > 2 and id < 8')
-            request = QueryRequest().set_statement(statement)
-            print('Query results for: ' + statement)
-            #
-            # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
-            # may be more results, so queries should generally be run in a loop.
-            # It is possible for single request to return no results but the
-            # query still not done, indicating that the query loop should
-            # continue.
-            #
-            while True:
-                result = handle.query(request)
-                for r in result.get_results():
-                    print('\t' + str(r))
-                if request.is_done():
-                    break
-
-            #
-            # Delete the row
-            #
-            request = DeleteRequest().set_table_name(table_name).set_key(
-                {'id': 1, 'sid': 0})
-            result = handle.delete(request)
-            print('After delete: ' + str(result))
-
-            #
-            # Get again to show deletion
-            #
-            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                table_name)
-            result = handle.get(request)
-            print('After get (should be None): ' + str(result))
-
-            #
-            # Drop the table
-            #
-            request = TableRequest().set_statement(
-                'drop table if exists {} '.format(table_name))
-            result = handle.table_request(request)
-
-            #
-            # Table drop can take time, depending on the state of the system.
-            # If this wait fails the table will still probably been dropped
-            #
-            result.wait_for_completion(handle, 40000, 2000)
-            print('After drop table')
-
-            print('Quickstart is complete')
-        except Exception as e:
-            print(e)
-        finally:
-            # If the handle isn't closed Python will not exit properly
-            if handle is not None:
-                handle.close()
-
-
-    if __name__ == '__main__':
-        main()
-
-Running Quickstart
-==================
+            print('Using credentials and DEFAULT profile from ' +
+                  '~/.oci/config')
+            provider = SignatureProvider()
+    elif nosql_env == 'cloudsim':
+        print('Using cloud simulator endpoint ' + cloudsim_endpoint)
+        endpoint = cloudsim_endpoint
+        provider = CloudsimAuthorizationProvider(cloudsim_id)
+
+    elif nosql_env == 'kvstore':
+        print('Using on-premise endpoint ' + kvstore_endpoint)
+        endpoint = kvstore_endpoint
+        provider = StoreAccessTokenProvider()
+
+    else:
+        raise IllegalArgumentException('Unknown environment: ' + nosql_env)
+
+    return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
+
+
+def main():
+
+    table_name = 'PythonQuickstart'
+
+    if len(sys.argv) != 2:
+        print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
+        raise SystemExit
+
+    nosql_env = sys.argv[1:][0]
+    print('Using environment: ' + str(nosql_env))
+
+    handle = None
+    try:
+
+        #
+        # Create a handle
+        #
+        handle = get_handle(nosql_env)
+
+        #
+        # Create a table
+        #
+        statement = (
+            'Create table if not exists {} (id integer, sid integer, ' +
+            'name string, primary key(shard(sid), id))').format(table_name)
+        request = TableRequest().set_statement(statement).set_table_limits(
+            TableLimits(30, 10, 1))
+        handle.do_table_request(request, 50000, 3000)
+        print('After create table')
+
+        #
+        # Put a few rows
+        #
+        request = PutRequest().set_table_name(table_name)
+        for i in range(10):
+            value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
+            request.set_value(value)
+            handle.put(request)
+        print('After put of 10 rows')
+
+        #
+        # Get the row
+        #
+        request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+            table_name)
+        result = handle.get(request)
+        print('After get: ' + str(result))
+
+        #
+        # Query, using a range
+        #
+        statement = (
+            'select * from ' + table_name + ' where id > 2 and id < 8')
+        request = QueryRequest().set_statement(statement)
+        print('Query results for: ' + statement)
+        #
+        # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
+        # may be more results, so queries should generally be run in a loop.
+        # It is possible for single request to return no results but the
+        # query still not done, indicating that the query loop should
+        # continue.
+        #
+        while True:
+            result = handle.query(request)
+            for r in result.get_results():
+                print('\t' + str(r))
+            if request.is_done():
+                break
+
+        #
+        # Delete the row
+        #
+        request = DeleteRequest().set_table_name(table_name).set_key(
+            {'id': 1, 'sid': 0})
+        result = handle.delete(request)
+        print('After delete: ' + str(result))
+
+        #
+        # Get again to show deletion
+        #
+        request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+            table_name)
+        result = handle.get(request)
+        print('After get (should be None): ' + str(result))
+
+        #
+        # Drop the table
+        #
+        request = TableRequest().set_statement(
+            'drop table if exists {} '.format(table_name))
+        result = handle.table_request(request)
+
+        #
+        # Table drop can take time, depending on the state of the system.
+        # If this wait fails the table will still probably been dropped
+        #
+        result.wait_for_completion(handle, 40000, 2000)
+        print('After drop table')
+
+        print('Quickstart is complete')
+    except Exception as e:
+        print(e)
+    finally:
+        # If the handle isn't closed Python will not exit properly
+        if handle is not None:
+            handle.close()
+
+
+if __name__ == '__main__':
+    main()
+```
+## Running Quickstart
 
-Run Against the Oracle NoSQL Database Cloud Service
-===================================================
+### Run Against the Oracle NoSQL Database Cloud Service
 
 Running against the Cloud Service requires an Oracle Cloud account. See
-`Configure for the Cloud Service <https://nosql-python-sdk.readthedocs.io/en/
-stable/installation.html#configure-for-the-cloud-service>`_ for information on
+[Configure for the Cloud Service](https://nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-the-cloud-service) for information on
 getting an account and acquiring required credentials.
 
 1. Collect the following information:
 
  * Tenancy ID
  * User ID
  * API signing key (private key file in PEM format)
@@ -379,64 +350,59 @@
    credentials in the program:
 
    * Directly provide the credential information. To use this method, modify the
      values of the variables at the top of the program: *tenancy*, *user*,
      *private_key*, *fingerprint*, and *pass_phrase*, setting them to the
      corresponding information you've collected.
    * Using a configuration file. In this case the information you've collected
-     goes into a file, ~/.oci/config. `Configure for the Cloud Service <https://
-     nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-
-     the-cloud-service>`_ describes the contents of the file. It will look like
+     goes into a file, ~/.oci/config. [Configure for the Cloud Service](https://nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-the-cloud-service) describes the contents of the file. It will look like
      this::
 
       [DEFAULT]
       tenancy=<your-tenancy-id>
       user=<your-user-id>
       fingerprint=<fingerprint-of-your-public-key>
       key_file=<path-to-your-private-key-file>
       pass_phrase=<optional-pass-phrase-for-key-file>
 
 3. Decide which region you want to use and modify the *cloud_region* variable to
-   the desired region. See `Regions documentation <https://nosql-python-sdk.
-   readthedocs.io/en/stable/api/borneo.Regions.html>`_ for possible regions. Not
+   the desired region. See [Regions documentation](https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.Regions.html) for possible regions. Not
    all support the Oracle NoSQL Database Cloud Service.
 
 4. Run the program:
 
 .. code-block:: pycon
 
     python quickstart.py cloud
 
-Run Against the Oracle NoSQL Cloud Simulator
-============================================
+### Run Against the Oracle NoSQL Cloud Simulator
 
 Running against the Oracle NoSQL Cloud Simulator requires a running Cloud
-Simulator instance. See `Configure for the Cloud Simulator <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator>`_ for information on how to
+Simulator instance. See [Configure for the Cloud Simulator](https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator) for information on how to
 download and start the Cloud Simulator.
 
 1. Start the Cloud Simulator based on instructions above. Note the HTTP port
    used. By default it is *8080* on *localhost*.
 
 2. The *quickstart.py* program defaults to *localhost:8080* so if the Cloud
    Simulator was started using default values no editing is required.
 
 3. Run the program:
 
 .. code-block:: pycon
 
     python quickstart.py cloudsim
 
-Run Against Oracle NoSQL on-premise
-===================================
+### Run Against Oracle NoSQL on-premise
 
 Running against the Oracle NoSQL Database on-premise requires a running Oracle
 NoSQL Database instance as well as a running NoSQL Proxy server instance. The
 program will connect to the proxy server.
 
-See `Configure for On-Premise Oracle NoSQL Database <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database>`_ for information on how to
+See [Configure for On-Premise Oracle NoSQL Database](https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database) for information on how to
 download and start the database instance and proxy server. The database and
 proxy should be started without security enabled for this quickstart program to
 operate correctly. A secure configuration requires a secure proxy and more
 complex configuration.
 
 1. Start the Oracle NoSQL Database and proxy server based on instructions above.
    Note the HTTP port used. By default the endpoint is *localhost:80*.
@@ -446,27 +412,21 @@
 
 3. Run the program:
 
 .. code-block:: pycon
 
     python quickstart.py kvstore
 
-=======
-License
-=======
+## Contributing
 
-Copyright (C) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+This project welcomes contributions from the community. Before submitting a pull request, please [review our contribution guide](./CONTRIBUTING.md)
 
-This SDK is licensed under the Universal Permissive License 1.0. See `LICENSE
-<./LICENSE.txt>`_ for details.
+## Security
 
-============
-Contributing
-============
+Please consult the [security guide](./SECURITY.md) for our responsible security vulnerability disclosure process
 
-See `CONTRIBUTING <./CONTRIBUTING.rst>`_
+## License
 
-========
-Security
-========
+Copyright (c) 2018, 2024 Oracle and/or its affiliates.
 
-See `SECURITY <./SECURITY.rst>`_
+Released under the Universal Permissive License v1.0 as shown at
+<https://oss.oracle.com/licenses/upl/>.
```

### Comparing `borneo-5.4.1/THIRD_PARTY_LICENSES.txt` & `borneo-5.4.2/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `borneo-5.4.1/setup.py` & `borneo-5.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 with open_relative('src', 'borneo', 'version.py') as fd:
     version = re.search(
         r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
         fd.read(), re.MULTILINE).group(1)
     if not version:
         raise RuntimeError('Cannot find version information')
 
-with open_relative('README.rst') as f:
+with open_relative('README.md') as f:
     readme = f.read()
 
 requires = [
     'python-dateutil>=2.7.0',
     'requests>=2.12.0'
     # don't install oci by default, it's only used for the cloud
     # 'oci>=2.2.18'
@@ -42,15 +42,15 @@
     url='https://nosql-python-sdk.readthedocs.io/en/stable/index.html',
 
     # Version should match the system release, but may vary as patches
     # are created.
     version=str(version),
     description='Oracle NoSQL Database Python SDK',
     long_description=str(readme),
-    long_description_content_type='text/x-rst',
+    long_description_content_type='text/markdown',
 
     author='Oracle',
     author_email='george.feinberg@oracle.com',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     include_package_data=True,
```

### Comparing `borneo-5.4.1/src/borneo/__init__.py` & `borneo-5.4.2/src/borneo/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 # This environment variable suppresses the import of all services
 # when importing from the OCI SDK. It can greatly speed up
@@ -12,48 +12,53 @@
 
 os.environ['OCI_PYTHON_SDK_NO_SERVICE_IMPORTS'] = '1'
 
 from . import iam
 from . import kv
 from .auth import AuthorizationProvider
 from .common import (
-    Consistency, Durability, FieldRange, PutOption, ResourcePrincipalClaimKeys, State,
-    SystemState, TableLimits, TimeToLive, TimeUnit, UserInfo, Version,
-    IndexInfo, PreparedStatement)
+    Consistency, Durability, FieldRange, PutOption, Replica, ReplicaStats,
+    ResourcePrincipalClaimKeys, State, SystemState, TableLimits, TableUsage,
+    TimeToLive, TimeUnit, UserInfo, Version, IndexInfo, PreparedStatement)
 from .config import (
     DefaultRetryHandler, NoSQLHandleConfig, Region, Regions, RetryHandler,
     StatsProfile)
 from .driver import NoSQLHandle
 from .exception import (
     BatchOperationNumberLimitException, IllegalArgumentException,
     IllegalStateException, IndexExistsException, IndexNotFoundException,
     InvalidAuthorizationException, NoSQLException,
     OperationNotSupportedException, OperationThrottlingException,
     ReadThrottlingException, RequestSizeLimitException, RequestTimeoutException,
     ResourceExistsException, ResourceNotFoundException, RetryableException,
     SecurityInfoNotReadyException, SystemException, TableExistsException,
-    TableNotFoundException, ThrottlingException, WriteThrottlingException)
+    TableNotFoundException, TableNotReadyException, ThrottlingException,
+    UnsupportedQueryVersionException, WriteThrottlingException)
 from .operations import (
-    DeleteRequest, DeleteResult, GetIndexesRequest, GetIndexesResult,
-    GetRequest, GetResult, GetTableRequest, ListTablesRequest, ListTablesResult,
+    AddReplicaRequest, DeleteRequest, DeleteResult, DropReplicaRequest,
+    GetIndexesRequest, GetIndexesResult, GetRequest,
+    GetResult, GetTableRequest, ListTablesRequest, ListTablesResult,
     MultiDeleteRequest, MultiDeleteResult, OperationResult, PrepareRequest,
     PrepareResult, PutRequest, PutResult, QueryRequest, QueryIterableResult,
-    QueryResult, Request, Result, SystemRequest, SystemResult,
+    QueryResult, ReplicaStatsRequest, ReplicaStatsResult, Request, Result,
+    SystemRequest, SystemResult,
     SystemStatusRequest, TableRequest, TableResult, TableUsageRequest,
     TableUsageResult, WriteMultipleRequest, WriteMultipleResult)
 from .stats import (StatsControl)
 from .version import __version__
 
-__all__ = ['AuthorizationProvider',
+__all__ = ['AddReplicaRequest',
+           'AuthorizationProvider',
            'BatchOperationNumberLimitException',
            'Consistency',
            'Durability',
            'DefaultRetryHandler',
            'DeleteRequest',
            'DeleteResult',
+           'DropReplicaRequest',
            'FieldRange',
            'GetIndexesRequest',
            'GetIndexesResult',
            'GetRequest',
            'GetResult',
            'GetTableRequest',
            'IllegalArgumentException',
@@ -80,14 +85,18 @@
            'PutResult',
            'QueryRequest',
            'QueryResult',
            'QueryIterableResult',
            'ReadThrottlingException',
            'Region',
            'Regions',
+           'Replica',
+           'ReplicaStats',
+           'ReplicaStatsRequest',
+           'ReplicaStatsResult',
            'Request',
            'RequestSizeLimitException',
            'RequestTimeoutException',
            'ResourceExistsException',
            'ResourcePrincipalClaimKeys',
            'ResourceNotFoundException',
            'Result',
@@ -101,20 +110,23 @@
            'SystemRequest',
            'SystemResult',
            'SystemState',
            'SystemStatusRequest',
            'TableExistsException',
            'TableLimits',
            'TableNotFoundException',
+           'TableNotReadyException',
            'TableRequest',
            'TableResult',
+           'TableUsage',
            'TableUsageRequest',
            'TableUsageResult',
            'ThrottlingException',
            'TimeToLive',
            'TimeUnit',
+           'UnsupportedQueryVersionException',
            'UserInfo',
            'Version',
            'WriteMultipleRequest',
            'WriteMultipleResult',
            'WriteThrottlingException'
            ]
```

### Comparing `borneo-5.4.1/src/borneo/auth.py` & `borneo-5.4.2/src/borneo/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from abc import ABCMeta, abstractmethod
 
@@ -78,15 +78,16 @@
         :raises IllegalArgumentException: raises the exception if input is not
             a string or none.
         """
         if not CheckValue.is_str(auth_string):
             raise IllegalArgumentException(
                 'Configured AuthorizationProvider requires a non-none string.')
 
-    def set_required_headers(self, request, auth_string, headers):
+    def set_required_headers(self, request, auth_string, headers,
+                                 content = None):
         """
         Internal use only.
 
         Set HTTP headers required by the provider.
 
         :param request: the request being processed.
         :type request: Request
```

### Comparing `borneo-5.4.1/src/borneo/client.py` & `borneo-5.4.2/src/borneo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from logging import DEBUG
 from multiprocessing import pool
@@ -18,15 +18,16 @@
     ByteOutputStream, CheckValue, HttpConstants, LogUtils, SSLAdapter,
     TableLimits, synchronized)
 from .config import DefaultRetryHandler
 from .exception import (IllegalArgumentException,
                         OperationNotSupportedException, RequestSizeLimitException)
 from .http import RateLimiterMap, RequestUtils
 from .kv import StoreAccessTokenProvider
-from .operations import GetTableRequest, QueryResult, TableRequest, WriteRequest
+from .operations import (
+    GetTableRequest, QueryRequest, QueryResult, TableRequest, WriteRequest)
 from .query import QueryDriver
 from .serdeutil import SerdeUtil
 from .stats import StatsControl
 from .version import __version__
 
 
 class Client(object):
@@ -90,14 +91,16 @@
         #
         adapter = SSLAdapter(
             ssl_ctx, pool_connections=self._pool_connections,
             pool_maxsize=self._pool_maxsize, max_retries=5, pool_block=True)
         self._sess.mount(self._url.scheme + '://', adapter)
         if self._proxy_host is not None:
             self._check_and_set_proxy(self._sess)
+        self.query_version = QueryDriver.QUERY_VERSION
+        self._topology_info = None
         self.serial_version = config.get_serial_version()
         # StoreAccessTokenProvider means onprem
         self._is_cloud = not isinstance(self._auth_provider, StoreAccessTokenProvider)
         if config.get_rate_limiting_enabled() and self._is_cloud:
             self._logutils.log_debug(
                 'Starting client with rate limiting enabled')
             self._rate_limiter_map = RateLimiterMap()
@@ -198,29 +201,32 @@
             on the QueryResult.
             """
             if request.is_prepared() and not request.is_simple_query():
                 self._trace(
                     'QueryRequest has no QueryDriver, but is prepared', 2)
                 driver = QueryDriver(request)
                 driver.set_client(self)
-                driver.set_topology_info(request.topology_info())
                 return QueryResult(request, False)
             """
             If we are here, then this is either (a) a simple query or (b) an
             advanced query that has not been prepared already, which also
             implies that this is the 1st execute() call on this query. For a
             non-prepared advanced query, the effect of this 1st execute() call
             is to send the query to the proxy for compilation, get back the
             prepared query, but no query results, create a QueryDriver, and bind
             it with the QueryRequest (see QueryRequestSerializer.deserialize()),
             and return an empty QueryResult.
             """
             self._trace(
                 'QueryRequest has no QueryDriver and is not prepared', 2)
+            request.incr_batch_counter()
+
         timeout_ms = request.get_timeout()
+        if request is QueryRequest or request.is_query_request():
+            request.set_topo_seq_num(self.get_topo_seq_num())
         headers = {'Host': self._url.hostname,
                    'Content-Type': 'application/octet-stream',
                    'Connection': 'keep-alive',
                    'Accept': 'application/octet-stream',
                    'User-Agent': self._user_agent}
 
         # set the session cookie if available
@@ -252,17 +258,35 @@
         request_id = self._next_request_id()
         headers[HttpConstants.REQUEST_ID_HEADER] = request_id
         self.check_request(request)
         # TODO: look at avoiding creating this object on each request
         request_utils = RequestUtils(
             self._sess, self._logutils, request, self._retry_handler, self,
             self._rate_limiter_map)
-        return request_utils.do_post_request(self._request_uri, headers,
-                                             content, timeout_ms,
-                                             self._stats_control)
+        res = request_utils.do_post_request(self._request_uri, headers,
+                                            content, timeout_ms,
+                                            self._stats_control)
+        self._set_topology_info(res.get_topology_info())
+        if res is QueryResult and request.is_query_request():
+            request.set_query_traces(res.get_query_traces())
+        return res
+
+    @synchronized
+    def _set_topology_info(self, topo):
+        if topo is None:
+            return
+        if self.get_topo_seq_num() < topo.get_seq_num():
+            self._topology_info = topo
+
+    def get_topo_seq_num(self):
+        return -1 if self._topology_info is None else \
+          self._topology_info.get_seq_num()
+
+    def get_topology(self):
+        return self._topology_info
 
     # set the session cookie if in return headers (see RequestUtils in http.py)
     @synchronized
     def set_session_cookie(self, cookie):
         # only grab the "session=value" portion of the header
         value = cookie.partition(';')[0]
         if self._logutils.is_enabled_for(DEBUG):
@@ -480,14 +504,32 @@
             'GetTableRequest completed for table "' + table_name + '"')
         # Update/add rate limiters for table.
         if self.update_rate_limiters(table_name, res.get_table_limits()):
             self._logutils.log_info(
                 'Background thread added limiters for table "' + table_name +
                 '"')
 
+    def decrement_query_version(self):
+        """
+        Decrements the query version, if it is greater than the minimum.
+        For internal use only.
+
+        The current minimum value is V3.
+        :returns: true if the version was decremented, false otherwise.
+        :rtype: bool
+        """
+        if self.query_version > QueryDriver.QUERY_V3:
+            self.query_version -= 1
+            msg = ('Unsupported query version error, decrementing ' +
+                   'version to ' + str(self.query_version) +
+                   ' and retrying')
+            self._logutils.log_info(msg)
+            return True
+        return False
+
     def decrement_serial_version(self):
         """
         Decrements the serial version, if it is greater than the minimum.
         For internal use only.
 
         The current minimum value is 2.
         :returns: true if the version was decremented, false otherwise.
@@ -530,14 +572,16 @@
         :param request: the request to be executed by the server.
         :type request: Request
         :param headers: the http headers
         :type headers: Dictionary
         :returns: the bytearray that contains the content.
         :rtype: bytearray
         """
+        # in case it's a query or prepare
+        request.set_query_version(self.query_version)
         content = self._write_content(request)
         headers.update({'Content-Length': str(len(content))})
         return content
 
     def get_stats_control(self):
         return self._stats_control
```

### Comparing `borneo-5.4.1/src/borneo/common.py` & `borneo-5.4.2/src/borneo/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from datetime import datetime
 from decimal import Decimal
@@ -150,24 +150,24 @@
 
     def write_int(self, value):
         val_s = pack('>i', value)
         self.write_value(val_s)
 
     def write_int_at_offset(self, offset, value):
         val_s = pack('>i', value)
-        val_b = bytearray(val_s)
+        val_b = bytes(val_s)
         for index in range(len(val_b)):
             self._content[offset + index] = val_b[index]
 
     def write_short_int(self, value):
         val_s = pack('>h', value)
         self.write_value(val_s)
 
     def write_value(self, value):
-        val_b = bytearray(value)
+        val_b = bytes(value)
         self._content.extend(val_b)
 
     def get_byte_at(self, index):
         return self._content[index]
 
     def get_last_byte(self):
         return self._content[-1]
@@ -482,22 +482,25 @@
 
     # Default namespace header
     REQUEST_NAMESPACE_HEADER = 'x-nosql-default-ns'
 
     # Proxy version info
     RESPONSE_PROXY_INFO = 'x-nosql-version'
 
+    # For OCI content signing
+    X_CONTENT_SHA256 = 'x-content-sha256'
+
     # Creates a URI path from the arguments
     def _make_path(*args):
         path = args[0]
         for index in range(1, len(args)):
             path += '/' + args[index]
         return path
 
-    # The base path to the on-premise security services. All users need a
+    # The base path to the on-premises security services. All users need a
     # leading "/" so add it here.
     KV_SECURITY_PATH = _make_path('/' + NOSQL_VERSION, 'nosql/security')
 
     # The path denoting a NoSQL request
     NOSQL_DATA_PATH = _make_path(NOSQL_VERSION, 'nosql/data')
 
 
@@ -527,25 +530,25 @@
         return self._index_name
 
     def get_field_names(self):
         """
         Returns the list of field names that define the index.
 
         :returns: the field names.
-        :rtype: list(str)
+        :rtype: list[str]
         """
         return self._field_names
 
     def get_field_types(self):
         """
         Returns the list of types of fields that define the index.
 
         :returns: the field types.
-        :rtype: list(str)
-        :versionadded: 5.4.0
+        :rtype: list[str]
+        :versionadded:: 5.4.0
         """
         return self._field_types
 
 
 class JsonNone(object):
     """
     Represents an JSON NONE field value.
@@ -1068,15 +1071,15 @@
     A single instance of PreparedStatement is thread-safe if bind variables are
     not used. If bind variables are to be used and the statement shared among
     threads additional instances of PreparedStatement can be constructed using
     :py:meth:`copy_statement`.
     """
     OPCODE_SELECT = 5
 
-    def __init__(self, sql_text, query_plan, query_schema, topology_info,
+    def __init__(self, sql_text, query_plan, query_schema,
                  proxy_statement, driver_plan, num_iterators, num_registers,
                  external_vars, namespace, table_name, operation):
         """
         Constructs a PreparedStatement. Construction is hidden to eliminate
         application access to the underlying statement, reducing the chance of
         corruption.
         """
@@ -1084,16 +1087,14 @@
         if proxy_statement is None or len(proxy_statement) < 10:
             raise IllegalArgumentException(
                 'Invalid prepared query, cannot be None.')
 
         self._sql_text = sql_text
         self._query_plan = query_plan
         self._query_schema = query_schema
-        # Applicable to advanced queries only.
-        self._topology_info = topology_info
         # The serialized PreparedStatement created at the backend store. It is
         # opaque for the driver. It is received from the proxy and sent back to
         # the proxy every time a new batch of results is needed.
         self._proxy_statement = proxy_statement
         # The part of the query plan that must be executed at the driver. It is
         # received from the proxy when the query is prepared there. It is
         # deserialized by the driver and not sent back to the proxy again.
@@ -1133,15 +1134,15 @@
         is immutable, but does not share its variables.
 
         :returns: a new PreparedStatement using this instance's prepared query.
             Bind variables are uninitialized.
         :rtype: PreparedStatement
         """
         return PreparedStatement(
-            self._sql_text, self._query_plan, self._query_schema, self._topology_info,
+            self._sql_text, self._query_plan, self._query_schema,
             self._proxy_statement, self._driver_query_plan, self._num_iterators,
             self._num_registers, self._variables, self._namespace,
             self._table_name, self._operation)
 
     def does_writes(self):
         # if it's not SELECT, it does writes.
         return self._operation != PreparedStatement.OPCODE_SELECT
@@ -1155,26 +1156,26 @@
 
     def get_query_plan(self):
         """
         Returns a string representation of the query execution plan, if it was
         requested in the :py:class:`PrepareRequest`; None otherwise.
 
         :returns: the string representation of the query execution plan.
-        :rtype: bool
+        :rtype: str
         """
         return self._query_plan
 
     def get_query_schema(self):
         """
         Returns a string representation of the query schema if it was
         requested in the :py:class:`PrepareRequest`; None otherwise.
 
         :returns: the string representation of the query schema.
-        :rtype: bool
-        :versionadded: 5.4.0
+        :rtype: str
+        :versionadded:: 5.4.0
         """
         return self._query_schema
 
     def get_sql_text(self):
         """
         Returns the SQL text of this PreparedStatement.
 
@@ -1220,24 +1221,14 @@
         return self._num_registers
 
     def print_driver_plan(self):
         if self._driver_query_plan is not None:
             return self._driver_query_plan.display()
         return None
 
-    @synchronized
-    def set_topology_info(self, topology_info):
-        if topology_info is None:
-            return
-        if self._topology_info is None:
-            self._topology_info = topology_info
-            return
-        if self._topology_info.get_seq_num() < topology_info.get_seq_num():
-            self._topology_info = topology_info
-
     def set_variable(self, variable, value):
         """
         Binds an external variable to a given value. The variable is identified
         by its name or its position within the query string. The variable that
         appears first in the query text has position 1, the variable that
         appears second has position 2 and so on.
 
@@ -1270,35 +1261,157 @@
             search_id = variable - 1
             for (k, v) in self._variables.items():
                 if v == search_id:
                     return self.set_variable(k, value)
             raise IllegalArgumentException(
                 'There is no external variable at position ' + str(variable))
 
-    def topology_info(self):
-        return self._topology_info
-
-    @synchronized
-    def topology_seq_num(self):
-        return (-1 if self._topology_info is None else
-                self._topology_info.get_seq_num())
-
 
 class PutOption(object):
     """
     Set the put option for put requests.
     """
     IF_ABSENT = 0
     """Set PutOption.IF_ABSENT to perform put if absent operation."""
     IF_PRESENT = 1
     """Set PutOption.IF_PRESENT to perform put if present operation."""
     IF_VERSION = 2
     """Set PutOption.IF_VERSION to perform put if version operation."""
 
 
+class Replica(object):
+    """
+    Cloud service only
+
+    Information representing a single replica. One or more of these
+    is returned in :py:class:`TableResult` for tables that have
+    replicas
+    """
+    def __init__(self):
+        self._replica_name = None
+        self._replica_ocid = None
+        self._write_units = 0
+        self._replica_state = None
+        self._capacity_mode = 0
+
+    def get_state(self):
+        """
+        Returns the state of the replica
+
+        :returns: the state
+        :rtype: State
+        """
+        return self._replica_state
+
+    def get_name(self):
+        """
+        Returns the name of the replica
+
+        :returns: the name
+        :rtype: str
+        """
+        return self._replica_name
+
+    def get_ocid(self):
+        """
+        Returns the OCID of the replica table
+
+        :returns: the OCID
+        :rtype: str
+        """
+        return self._replica_ocid
+
+    def get_write_units(self):
+        """
+        Returns the value of write units for the replica table
+
+        :returns: the units
+        :rtype: int
+        """
+        return self._write_units
+
+    def get_capacity_mode(self):
+        """
+        Returns the :py:class:`TableLimits.CAPACITY_MODE`
+        of the replica table
+
+        :returns: the mode
+        :rtype: :py:class:`TableLimits.CAPACITY_MODE`
+        """
+        if self._capacity_mode == 1:
+            return TableLimits.CAPACITY_MODE.PROVISIONED
+        return TableLimits.CAPACITY_MODE.ON_DEMAND
+
+    def __str__(self):
+        return 'Replica [name=' + str(self.get_name()) + ', ocid=' + \
+          str(self.get_ocid()) + ',state=' + \
+          str(self.get_state()) \
+          + ',mode=' + str(self.get_capacity_mode()) + ',write_units=' + \
+          str(self.get_write_units()) + ']'
+
+
+class ReplicaStats(object):
+    """
+    ReplicaStats contains information about replica lag for a specific
+    replica.
+
+    Replica lag is a measure of how current this table is relative to
+    the remote replica and indicates that this table has not yet received
+    updates that happened within the lag period.
+
+    For example, if the replica lag is 5,000 milliseconds(5 seconds),
+    then this table will have all updates that occurred at the remote
+    replica that are more than 5 seconds old.
+
+    Replica lag is calculated based on how long it took for the latest
+    operation from the table at the remote replica to be replayed at this
+    table. If there have been no application writes for the table at the
+    remote replica, the service uses other mechanisms to calculate an
+    approximation of the lag, and the lag statistic will still be available.
+    """
+    def __init__(self):
+        self._collection_time_millis = 0
+        self._replica_lag = 0
+
+    def get_collection_time(self):
+        """
+        Returns the time the replica lag collection was performed. The value
+        is a time stamp in milliseconds since the Epoch
+
+        :returns: the time
+        :rtype: int
+        """
+        return self._collection_time_millis
+
+    def get_collection_time_str(self):
+        """
+        Returns the collection time as an ISO 8601 formatted string
+
+        :returns: the time
+        :rtype: str
+        """
+        return datetime.fromtimestamp(
+            float(self._collection_time_millis) / 1000). \
+                replace(tzinfo=tz.UTC).isoformat()
+
+    def get_replica_lag(self):
+        """
+        Returns the replica lag collected at the specified time in
+        milliseconds
+
+        :returns: the lag
+        :rtype: int
+        """
+        return self._replica_lag
+
+    def __str__(self):
+        return '[time=' + self.get_collection_time_str() + ',' \
+          'lag=' + str(self._replica_lag) + ']'
+
+
 class ResourcePrincipalClaimKeys(object):
     """
     Claim keys in the resource principal session token(RPST).
 
     They can be used to retrieve resource principal metadata such as its
     compartment and tenancy OCID.
 
@@ -1353,15 +1466,15 @@
     """Represents the table is dropping."""
     UPDATING = 'UPDATING'
     """Represents the table is updating."""
 
 
 class SystemState(object):
     """
-    On-premise only.
+    On-premises only.
 
     The current state of the system request.
     """
     COMPLETE = 'COMPLETE'
     """
     The operation is complete and was successful. Failures are thrown as
     exceptions.
@@ -1371,15 +1484,15 @@
 
 
 class Durability(object):
     """
     Durability defines the durability characteristics associated with a standalone write
     (put or update) operation.
 
-    This is currently only supported in On-Prem installations. It is ignored
+    This is currently only supported in on-premises installations. It is ignored
     in the cloud service.
 
     The overall durability is a function of the SYNC_POLICY and
     ACK_POLICY in effect for the Master, and the SYNC_POLICY in
     effect for each Replica.
 
     SYNC_POLICY represents policies to be used when committing a
@@ -1533,15 +1646,15 @@
         valid.
     :versionchanged: 5.3.0, added optional CAPACITY_MODE
     """
 
     """
     TableLimits includes an optional mode
 
-    :versionadded: 5.3.0
+    :versionadded:: 5.3.0
     """
     CAPACITY_MODE = enum(PROVISIONED=1,
                          ON_DEMAND=2)
 
     # noinspection PyUnresolvedReferences
     def __init__(self, read_units, write_units, storage_gb,
                  mode=CAPACITY_MODE.PROVISIONED):
@@ -1660,28 +1773,28 @@
             ON_DEMAND: Flexible read/write limits.
 
         :param mode: the capacity to use, in gigabytes.
         :type mode: TableLimits.CAPACITY_MODE
         :returns: self.
         :raises IllegalArgumentException: raises the exception if mode is
             invalid.
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         if (mode != TableLimits.CAPACITY_MODE.PROVISIONED and
                 mode != TableLimits.CAPACITY_MODE.ON_DEMAND):
             raise IllegalArgumentException(
                 'TableLimits mode must be one of PROVISIONED or ON_DEMAND')
         self._mode = mode
 
     def get_mode(self):
         """
         Returns the capacity mode of the table.
 
         :returns: mode: PROVISIONED or ON_DEMAND
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         return self._mode
 
     # noinspection PyUnresolvedReferences
     def validate(self):
         if self._storage_gb <= 0:
             raise IllegalArgumentException(
@@ -1821,15 +1934,15 @@
     def get_max_shard_usage_percent(self):
         """
         Returns the percentage of allowed storage usage for the shard with the
         highest usage percentage across all table shards. This can be used as a
         gauge of toal storage available as well as a hint for key distribution.
         :returns: the percentage
         :rtype: int
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._max_shard_usage_percent
 
 
 class TimeUnit(object):
     """
     The time unit to use.
@@ -1975,15 +2088,15 @@
 
     def unit_is_hours(self):
         return self._timeunit == TimeUnit.HOURS
 
 
 class UserInfo(object):
     """
-    On-premise only.
+    On-premises only.
 
     A class that encapsulates the information associated with a user including
     the user id and name in the system.
     """
 
     def __init__(self, user_id, user_name):
         """
```

### Comparing `borneo-5.4.1/src/borneo/config.py` & `borneo-5.4.2/src/borneo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from abc import ABCMeta, abstractmethod
 from copy import deepcopy
@@ -240,20 +240,27 @@
     OC3_EP_BASE = 'https://nosql.{0}.oci.oraclegovcloud.com'
     OC4_EP_BASE = 'https://nosql.{0}.oci.oraclegovcloud.uk'
     OC5_EP_BASE = 'https://nosql.{0}.oci.oraclecloud5.com'
     OC8_EP_BASE = 'https://nosql.{0}.oci.oraclecloud8.com'
     OC9_EP_BASE = 'https://nosql.{0}.oci.oraclecloud9.com'
     OC10_EP_BASE = 'https://nosql.{0}.oci.oraclecloud10.com'
     OC14_EP_BASE = 'https://nosql.{0}.oci.oraclecloud14.com'
+    OC15_EP_BASE = 'https://nosql.{0}.oci.oraclecloud15.com'
     OC16_EP_BASE = 'https://nosql.{0}.oci.oraclecloud16.com'
     OC17_EP_BASE = 'https://nosql.{0}.oci.oraclecloud17.com'
     OC19_EP_BASE = 'https://nosql.{0}.oci.oraclecloud.eu'
     OC20_EP_BASE = 'https://nosql.{0}.oci.oraclecloud20.com'
-    OC22_EP_BASE = 'https://nosql.{0}.oci.oraclecloud22.com'
+    OC21_EP_BASE = 'https://nosql.{0}.oci.oraclecloud21.com'
+    OC22_EP_BASE = 'https://nosql.{0}.oci.psn-pco.it'
     OC24_EP_BASE = 'https://nosql.{0}.oci.oraclecloud24.com'
+    OC25_EP_BASE = 'https://nosql.{0}.oci.nricloud.jp'
+    OC26_EP_BASE = 'https://nosql.{0}.oci.oraclecloud26.com'
+    OC27_EP_BASE = 'https://nosql.{0}.oci.oraclecloud27.com'
+    OC28_EP_BASE = 'https://nosql.{0}.oci.oraclecloud28.com'
+    OC31_EP_BASE = 'https://nosql.{0}.oci.sovereigncloud.nz'
 
     def __init__(self, region_id):
         self._region_id = region_id
 
     def endpoint(self):
         """
         Returns the NoSQL Database Cloud Service endpoint string for this
@@ -278,26 +285,40 @@
             return str.format(Region.OC8_EP_BASE, self._region_id)
         if self._is_oc9_region():
             return str.format(Region.OC9_EP_BASE, self._region_id)
         if self._is_oc10_region():
             return str.format(Region.OC10_EP_BASE, self._region_id)
         if self._is_oc14_region():
             return str.format(Region.OC14_EP_BASE, self._region_id)
+        if self._is_oc15_region():
+            return str.format(Region.OC15_EP_BASE, self._region_id)
         if self._is_oc16_region():
             return str.format(Region.OC16_EP_BASE, self._region_id)
         if self._is_oc17_region():
             return str.format(Region.OC17_EP_BASE, self._region_id)
         if self._is_oc19_region():
             return str.format(Region.OC19_EP_BASE, self._region_id)
         if self._is_oc20_region():
             return str.format(Region.OC20_EP_BASE, self._region_id)
+        if self._is_oc21_region():
+            return str.format(Region.OC21_EP_BASE, self._region_id)
         if self._is_oc22_region():
             return str.format(Region.OC22_EP_BASE, self._region_id)
         if self._is_oc24_region():
             return str.format(Region.OC24_EP_BASE, self._region_id)
+        if self._is_oc25_region():
+            return str.format(Region.OC25_EP_BASE, self._region_id)
+        if self._is_oc26_region():
+            return str.format(Region.OC26_EP_BASE, self._region_id)
+        if self._is_oc27_region():
+            return str.format(Region.OC27_EP_BASE, self._region_id)
+        if self._is_oc28_region():
+            return str.format(Region.OC28_EP_BASE, self._region_id)
+        if self._is_oc31_region():
+            return str.format(Region.OC31_EP_BASE, self._region_id)
         raise IllegalArgumentException(
             'Unable to find endpoint for unknown region ' + self._region_id)
 
     def get_region_id(self):
         """
         Internal use only.
 
@@ -336,14 +357,18 @@
         # Internal use only
         return Regions.OC9_REGIONS.get(self._region_id) is not None
 
     def _is_oc10_region(self):
         # Internal use only
         return Regions.OC10_REGIONS.get(self._region_id) is not None
 
+    def _is_oc15_region(self):
+        # Internal use only
+        return Regions.OC15_REGIONS.get(self._region_id) is not None
+
     def _is_oc14_region(self):
         # Internal use only
         return Regions.OC14_REGIONS.get(self._region_id) is not None
 
     def _is_oc16_region(self):
         # Internal use only
         return Regions.OC16_REGIONS.get(self._region_id) is not None
@@ -356,22 +381,46 @@
         # Internal use only
         return Regions.OC19_REGIONS.get(self._region_id) is not None
 
     def _is_oc20_region(self):
         # Internal use only
         return Regions.OC20_REGIONS.get(self._region_id) is not None
 
+    def _is_oc21_region(self):
+        # Internal use only
+        return Regions.OC21_REGIONS.get(self._region_id) is not None
+
     def _is_oc22_region(self):
         # Internal use only
         return Regions.OC22_REGIONS.get(self._region_id) is not None
 
     def _is_oc24_region(self):
         # Internal use only
         return Regions.OC24_REGIONS.get(self._region_id) is not None
 
+    def _is_oc25_region(self):
+        # Internal use only
+        return Regions.OC25_REGIONS.get(self._region_id) is not None
+
+    def _is_oc26_region(self):
+        # Internal use only
+        return Regions.OC26_REGIONS.get(self._region_id) is not None
+
+    def _is_oc27_region(self):
+        # Internal use only
+        return Regions.OC27_REGIONS.get(self._region_id) is not None
+
+    def _is_oc28_region(self):
+        # Internal use only
+        return Regions.OC28_REGIONS.get(self._region_id) is not None
+
+    def _is_oc31_region(self):
+        # Internal use only
+        return Regions.OC31_REGIONS.get(self._region_id) is not None
+
 
 class Regions(object):
     """
     Cloud service only.
 
     The class contains the regions in the Oracle Cloud Infrastructure at the
     time of this release. The Oracle NoSQL Database Cloud Service is not
@@ -478,14 +527,16 @@
     US_SANJOSE_1 = Region('us-sanjose-1')
     """Region Location: San Jose, CA, AZ """
     CA_MONTREAL_1 = Region('ca-montreal-1')
     """Region Location: Montreal, Canada"""
     CA_TORONTO_1 = Region('ca-toronto-1')
     """Region Location: Toronto, Canada"""
 
+    SA_BOGOTA_1 = Region('sa-bogota-1')
+    """Region Location: Bogota, Colombia"""
     SA_SANTIAGO_1 = Region('sa-santiago-1')
     """Region Location: Santiago, Chile"""
     SA_SAOPAULO_1 = Region('sa-saopaulo-1')
     """Region Location: Sao Paulo, Brazil"""
     SA_VALPARAISO_1 = Region('sa-valparaiso-1')
     """Region Location: Valparaiso, Chile"""
     SA_VINHEDO_1 = Region('sa-vinhedo-1')
@@ -539,14 +590,18 @@
     EU_DCC_DUBLIN_2 = Region('eu-dcc-dublin-2')
     """Region Location: Dublin, Ireland"""
     EU_DCC_RATING_1 = Region('eu-dcc-rating-1')
     """Region Location: Germany"""
     EU_DCC_RATING_2 = Region('eu-dcc-rating-2')
     """Region Location: Germany"""
 
+    # OC15
+    AP_DCC_GAZIPUR_1 = Region('ap-dcc-gazipur-1')
+    """Region Location: Bangladesh"""
+
     # OC16
     US_WESTJORDAN_1 = Region('us-westjordan-1')
     """Region Location: Utah"""
 
     # OC17
     US_DCC_PHOENIX_1 = Region('us-dcc-phoenix-1')
     """Region Location: Phoenix, AZ"""
@@ -561,22 +616,46 @@
     EU_MADRID_2 = Region('eu-madrid-2')
     """Region Location: Madrid, Spain"""
 
     # OC20
     EU_JOVANOVAC_1 = Region('eu-jovanovac-1')
     """Region Location: Serbia"""
 
+    # OC20
+    ME_DCC_DOHA_1 = Region('me-dcc-doha-1')
+    """Region Location: Qatar"""
+
     # OC22
     EU_DCC_ROME_1 = Region('eu-dcc-rome-1')
     """Region Location: Rome, Italy"""
 
     # OC24
     EU_DCC_ZURICH_1 = Region('eu-dcc-zurich-1')
     """Region Location: Zurich, Switzerland"""
 
+    # OC25
+    AP_DCC_TOKYO_1 = Region('ap-dcc-tokyo-1')
+    """Region Location: Tokyo, Japan"""
+
+    # OC26
+    ME_ABUDHABI_3 = Region('me-abudhabi-3')
+    """Region Location: Abudabhi"""
+
+    # OC27
+    US_DCC_SWJORDAN_1 = Region('us-dcc-swjordan-1')
+    """Region Location: Utah, USA"""
+
+    # OC28
+    US_DCC_SWJORDAN_2 = Region('us-dcc-swjordan-2')
+    """Region Location: Utah, USA"""
+
+    # OC31
+    AP_HOBSONVILLE_1 = Region('ap-hobsonville-1')
+    """Region Location: New Zealand"""
+
     # OC1
     OC1_REGIONS = dict()
     """A dict containing the OC1 regions."""
     OC1_REGIONS[AF_JOHANNESBURG_1.get_region_id()] = AF_JOHANNESBURG_1
     # APAC
     OC1_REGIONS[AP_CHUNCHEON_1.get_region_id()] = AP_CHUNCHEON_1
     OC1_REGIONS[AP_HYDERABAD_1.get_region_id()] = AP_HYDERABAD_1
@@ -601,14 +680,15 @@
     OC1_REGIONS[EU_MARSEILLE_1.get_region_id()] = EU_MARSEILLE_1
     OC1_REGIONS[EU_MILAN_1.get_region_id()] = EU_MILAN_1
     OC1_REGIONS[EU_PARIS_1.get_region_id()] = EU_PARIS_1
     OC1_REGIONS[EU_STOCKHOLM_1.get_region_id()] = EU_STOCKHOLM_1
     OC1_REGIONS[EU_ZURICH_1.get_region_id()] = EU_ZURICH_1
 
     # LAD
+    OC1_REGIONS[SA_BOGOTA_1.get_region_id()] = SA_BOGOTA_1
     OC1_REGIONS[SA_SANTIAGO_1.get_region_id()] = SA_SANTIAGO_1
     OC1_REGIONS[SA_SAOPAULO_1.get_region_id()] = SA_SAOPAULO_1
     OC1_REGIONS[SA_VALPARAISO_1.get_region_id()] = SA_VALPARAISO_1
     OC1_REGIONS[SA_VINHEDO_1.get_region_id()] = SA_VINHEDO_1
 
     # North America
     OC1_REGIONS[US_ASHBURN_1.get_region_id()] = US_ASHBURN_1
@@ -667,14 +747,19 @@
     OC14_REGIONS[EU_DCC_MILAN_1.get_region_id()] = EU_DCC_MILAN_1
     OC14_REGIONS[EU_DCC_MILAN_2.get_region_id()] = EU_DCC_MILAN_2
     OC14_REGIONS[EU_DCC_DUBLIN_1.get_region_id()] = EU_DCC_DUBLIN_1
     OC14_REGIONS[EU_DCC_DUBLIN_2.get_region_id()] = EU_DCC_DUBLIN_2
     OC14_REGIONS[EU_DCC_RATING_1.get_region_id()] = EU_DCC_RATING_1
     OC14_REGIONS[EU_DCC_RATING_2.get_region_id()] = EU_DCC_RATING_2
 
+    # OC15
+    OC15_REGIONS = dict()
+    """A dict containing the OC15 regions."""
+    OC15_REGIONS[AP_DCC_GAZIPUR_1.get_region_id()] = AP_DCC_GAZIPUR_1
+
     # OC16
     OC16_REGIONS = dict()
     """A dict containing the OC16 regions."""
     OC16_REGIONS[US_WESTJORDAN_1.get_region_id()] = US_WESTJORDAN_1
 
     # OC17
     OC17_REGIONS = dict()
@@ -690,24 +775,54 @@
     OC19_REGIONS[EU_MADRID_2.get_region_id()] = EU_MADRID_2
 
     # OC20
     OC20_REGIONS = dict()
     """A dict containing the OC20 regions."""
     OC20_REGIONS[EU_JOVANOVAC_1.get_region_id()] = EU_JOVANOVAC_1
 
+    # OC21
+    OC21_REGIONS = dict()
+    """A dict containing the OC21 regions."""
+    OC21_REGIONS[ME_DCC_DOHA_1.get_region_id()] = ME_DCC_DOHA_1
+
     # OC22
     OC22_REGIONS = dict()
     """A dict containing the OC22 regions."""
     OC22_REGIONS[EU_DCC_ROME_1.get_region_id()] = EU_DCC_ROME_1
 
     # OC24
     OC24_REGIONS = dict()
-    """A dict containing the OC22 regions."""
+    """A dict containing the OC24 regions."""
     OC24_REGIONS[EU_DCC_ZURICH_1.get_region_id()] = EU_DCC_ZURICH_1
 
+    # OC25
+    OC25_REGIONS = dict()
+    """A dict containing the OC25 regions."""
+    OC25_REGIONS[AP_DCC_TOKYO_1.get_region_id()] = AP_DCC_TOKYO_1
+
+    # OC26
+    OC26_REGIONS = dict()
+    """A dict containing the OC26 regions."""
+    OC26_REGIONS[ME_ABUDHABI_3.get_region_id()] = ME_ABUDHABI_3
+
+    # OC27
+    OC27_REGIONS = dict()
+    """A dict containing the OC27 regions."""
+    OC27_REGIONS[US_DCC_SWJORDAN_1.get_region_id()] = US_DCC_SWJORDAN_1
+
+    # OC28
+    OC28_REGIONS = dict()
+    """A dict containing the OC28 regions."""
+    OC28_REGIONS[US_DCC_SWJORDAN_2.get_region_id()] = US_DCC_SWJORDAN_2
+
+    # OC31
+    OC31_REGIONS = dict()
+    """A dict containing the OC31 regions."""
+    OC31_REGIONS[AP_HOBSONVILLE_1.get_region_id()] = AP_HOBSONVILLE_1
+
     @staticmethod
     def get_oc1_regions():
         # Internal use only
         return Regions.OC1_REGIONS.values()
 
     @staticmethod
     def get_oc2_regions():
@@ -746,14 +861,19 @@
 
     @staticmethod
     def get_oc14_regions():
         # Internal use only
         return Regions.OC14_REGIONS.values()
 
     @staticmethod
+    def get_oc15_regions():
+        # Internal use only
+        return Regions.OC15_REGIONS.values()
+
+    @staticmethod
     def get_oc16_regions():
         # Internal use only
         return Regions.OC16_REGIONS.values()
 
     @staticmethod
     def get_oc17_regions():
         # Internal use only
@@ -766,24 +886,54 @@
 
     @staticmethod
     def get_oc20_regions():
         # Internal use only
         return Regions.OC20_REGIONS.values()
 
     @staticmethod
+    def get_oc21_regions():
+        # Internal use only
+        return Regions.OC21_REGIONS.values()
+
+    @staticmethod
     def get_oc22_regions():
         # Internal use only
         return Regions.OC22_REGIONS.values()
 
     @staticmethod
     def get_oc24_regions():
         # Internal use only
         return Regions.OC24_REGIONS.values()
 
     @staticmethod
+    def get_oc25_regions():
+        # Internal use only
+        return Regions.OC25_REGIONS.values()
+
+    @staticmethod
+    def get_oc26_regions():
+        # Internal use only
+        return Regions.OC26_REGIONS.values()
+
+    @staticmethod
+    def get_oc27_regions():
+        # Internal use only
+        return Regions.OC27_REGIONS.values()
+
+    @staticmethod
+    def get_oc28_regions():
+        # Internal use only
+        return Regions.OC28_REGIONS.values()
+
+    @staticmethod
+    def get_oc31_regions():
+        # Internal use only
+        return Regions.OC31_REGIONS.values()
+
+    @staticmethod
     def from_region_id(region_id):
         """
         Returns the Region associated with the string value supplied, or None if
         the string does not represent a known region.
 
         :param region_id: the string value of the region.
         :type region_id: str
@@ -808,25 +958,39 @@
         if region is None:
             region = Regions.OC9_REGIONS.get(region_id)
         if region is None:
             region = Regions.OC10_REGIONS.get(region_id)
         if region is None:
             region = Regions.OC14_REGIONS.get(region_id)
         if region is None:
+            region = Regions.OC15_REGIONS.get(region_id)
+        if region is None:
             region = Regions.OC16_REGIONS.get(region_id)
         if region is None:
             region = Regions.OC17_REGIONS.get(region_id)
         if region is None:
             region = Regions.OC19_REGIONS.get(region_id)
         if region is None:
             region = Regions.OC20_REGIONS.get(region_id)
         if region is None:
+            region = Regions.OC21_REGIONS.get(region_id)
+        if region is None:
             region = Regions.OC22_REGIONS.get(region_id)
         if region is None:
             region = Regions.OC24_REGIONS.get(region_id)
+        if region is None:
+            region = Regions.OC25_REGIONS.get(region_id)
+        if region is None:
+            region = Regions.OC26_REGIONS.get(region_id)
+        if region is None:
+            region = Regions.OC27_REGIONS.get(region_id)
+        if region is None:
+            region = Regions.OC28_REGIONS.get(region_id)
+        if region is None:
+            region = Regions.OC31_REGIONS.get(region_id)
         return region
 
 
 class StatsProfile(Enum):
     """
     The following semantics are attached to the StatsProfile values:
        - NONE: no stats are logged.
@@ -850,15 +1014,15 @@
     for use by :py:class:`NoSQLHandle` methods. When creating a
     :py:class:`NoSQLHandle`, the NoSQLHandleConfig instance is copied
     so modification operations on the instance have no effect on existing
     handles which are immutable. NoSQLHandle state with default values can be
     overridden in individual operations.
 
     The service endpoint is used to connect to the Oracle NoSQL Database Cloud
-    Service or, if on-premise, the Oracle NoSQL Database proxy server. It should
+    Service or if on-premises, the Oracle NoSQL Database proxy server. It should
     be a string or a :py:class:`Region`.
 
     If a string is provided to endpoint argument, there is flexibility in how
     endpoints are specified. A fully specified endpoint is of the format:
 
      * http[s]://host:port
 
@@ -1007,18 +1171,18 @@
         :returns: the url.
         :rtype: ParseResult
         """
         return self._service_url
 
     def get_region(self):
         """
-        Cloud service only.
-
         Returns the region will be accessed by the NoSQLHandle.
 
+        Cloud service only.
+
         :returns: the region.
         :rtype: Region
         """
         return self._region
 
     def set_authorization_provider(self, provider):
         """
@@ -1045,48 +1209,48 @@
         :returns: the AuthorizationProvider.
         :rtype: AuthorizationProvider
         """
         return self._auth_provider
 
     def set_default_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the default compartment to use for requests sent using the handle.
         Setting the default is optional and if set it is overridden by any
         compartment specified in a request or table name. If no compartment is
         set for a request, either using this default or by specification in a
         request, the behavior varies with how the application is authenticated:
 
         * If authenticated with a user identity the default is the root
           compartment of the tenancy
         * If authenticated as an instance principal (see
           :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`
           ) the compartment id (OCID) must be specified by either using this
           method or in each Request object. If not an exception is thrown.
 
+        Cloud service only.
+
         :param compartment: may be either the name of a compartment or the id
             (OCID) of a compartment.
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
             is not a string.
         """
         CheckValue.check_str(compartment, 'compartment')
         self._compartment = compartment
         return self
 
     def get_default_compartment(self):
         """
-        Cloud service only.
-
         Returns the default compartment to use for requests or None if not set.
         The value may be a compartment name or id, as set by
         :py:meth:`set_default_compartment`.
 
+        Cloud service only.
+
         :returns: the compartment, or None.
         :rtype: str or None
         """
         return self._compartment
 
     def get_default_timeout(self):
         """
@@ -1263,33 +1427,37 @@
         :returns: the pool size.
         :rtype: int
         """
         return self._pool_maxsize
 
     def set_max_content_length(self, max_content_length):
         """
-        Sets the maximum size in bytes of request payloads. On-premise only.
+        Sets the maximum size in bytes of request payloads.
         This setting is ignored for cloud operations. If not set, or set to
         zero, the default value of 32MB is used.
 
+        On-premises only.
+
         :param max_content_length: the maximum bytes allowed in requests. Pass
             zero to use the default.
         :type max_content_length: int
         :returns: self.
         :raises IllegalArgumentException: raises the exception if
             max_content_length is a negative number.
         """
         CheckValue.check_int_ge_zero(max_content_length, 'max_content_length')
         self._max_content_length = max_content_length
         return self
 
     def get_max_content_length(self):
         """
         Returns the maximum size, in bytes, of a request operation payload.
-        On-premise only. This value is ignored for cloud operations.
+        This value is ignored for cloud operations.
+
+        On-premises only.
 
         :returns: the size.
         :rtype: int
         """
         return self._max_content_length
 
     def set_retry_handler(self, retry_handler):
@@ -1345,68 +1513,68 @@
         :returns: the handler.
         :rtype: RetryHandler
         """
         return self._retry_handler
 
     def set_rate_limiting_enabled(self, enable):
         """
-        Cloud service only.
-
         Enables internal rate limiting.
 
+        Cloud service only.
+
         :param enable: If True, enable internal rate limiting, otherwise disable
             internal rate limiting.
         :type enable: bool
         :returns: self.
         :raises IllegalArgumentException: raises the exception if enable is
             not a boolean.
         """
         CheckValue.check_boolean(enable, 'enable')
         self._rate_limiting_enabled = enable
         return self
 
     def get_rate_limiting_enabled(self):
         """
-        Internal use only.
-
         Returns whether the rate limiting is enabled.
 
+        Internal use only.
+
         :returns: True if rate limiting is enabled, otherwise False.
         :rtype: bool
         """
         return self._rate_limiting_enabled
 
     def set_default_rate_limiting_percentage(self, percent):
         """
-        Cloud service only.
-
         Sets a default percentage of table limits to use. This may be useful for
         cases where a client should only use a portion of full table limits.
         This only applies if rate limiting is enabled using
         :py:meth:`set_rate_limiting_enabled`.
 
         The default for this value is 100.0 (full table limits).
 
+        Cloud service only.
+
         :param percent: the percentage of table limits to use. This value must
             be positive.
         :type percent: int or float or Decimal
         :returns: self.
         :raises IllegalArgumentException: raises the exception if percent is
             not a positive digital number.
         """
         CheckValue.check_float_gt_zero(percent, 'percent')
         self._default_rate_limiter_percentage = float(percent)
         return self
 
     def get_default_rate_limiting_percentage(self):
         """
-        Internal use only.
-
         Returns the default percentage.
 
+        Internal use only.
+
         :returns: the default percentage.
         :rtype: float
         """
         if self._default_rate_limiter_percentage == 0.0:
             return 100.0
         return self._default_rate_limiter_percentage
 
@@ -1508,22 +1676,22 @@
         :returns: the password, or None.
         :rtype: str or None
         """
         return self._proxy_password
 
     def set_ssl_ca_certs(self, ssl_ca_certs):
         """
-        On-premise only.
-
-        When running against on-premise Oracle NoSQL Database with security
+        When running against on-premises Oracle NoSQL Database with security
         enabled, certificates should be specified using this method. Otherwise
         environment variable REQUESTS_CA_BUNDLE should be configured. See `the
         installation guide <https://nosql-python-sdk.readthedocs.io/en/stable/
         installation.html>`_ for the configuration of REQUESTS_CA_BUNDLE.
 
+        On-premises only.
+
         :param ssl_ca_certs: ssl ca certificates.
         :type ssl_ca_certs: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if ssl_ca_certs
             is not a string.
         """
         CheckValue.check_str(ssl_ca_certs, 'ssl_ca_certs')
@@ -1798,31 +1966,31 @@
         return self._serial_version
 
     def set_serial_version(self, version):
         self._serial_version = version
 
     def set_default_namespace(self, namespace):
         """
-        On-premises only.
-
         Sets the default namespace to use for requests that use a table
         name
 
+        On-premises only.
+
         :param namespace: the default namespace.
         :type namespace: str
         :returns: self
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         self._default_namespace = namespace
         return self
 
     def get_default_namespace(self):
         """
-        On-premises only.
-
         Returns the default namespace or None if not set.
 
+        On-premises only.
+
         :returns: the default namespace or None.
         :rtype: str
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._default_namespace
```

### Comparing `borneo-5.4.1/src/borneo/driver.py` & `borneo-5.4.2/src/borneo/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from json import loads
 from logging import FileHandler, Formatter, WARNING, getLogger
@@ -28,15 +28,15 @@
     """
     NoSQLHandle is a handle that can be used to access Oracle NoSQL tables. To
     create a connection represented by NoSQLHandle, request an instance using
     :py:class:`NoSQLHandleConfig`, which allows an application to specify
     default values and other configuration information to be used by the handle.
 
     The same interface is available to both users of the Oracle NoSQL Database
-    Cloud Service and the on-premise Oracle NoSQL Database; however, some
+    Cloud Service and the on-premises Oracle NoSQL Database; however, some
     methods and/or parameters are specific to each environment. The
     documentation has notes about whether a class, method, or parameter is
     environment-specific. Unless otherwise noted they are applicable to both
     environments.
 
     A handle has memory and network resources associated with it. Consequently,
     the :py:meth:`close` method must be invoked to free up the resources when
@@ -185,15 +185,15 @@
 
     def get_table(self, request):
         """
         Gets static information about the specified table including its state,
         provisioned throughput and capacity and schema. Dynamic information such
         as usage is obtained using :py:meth:`get_table_usage`. Throughput,
         capacity and usage information is only available when using the Cloud
-        Service and will be None or not defined on-premise.
+        Service and will be None or not defined on-premises.
 
         :param request: the input parameters for the operation.
         :type request: GetTableRequest
         :returns: the result of the operation.
         :rtype: TableResult
         :raises IllegalArgumentException: raises the exception if request is not
             an instance of :py:class:`GetTableRequest`.
@@ -209,21 +209,21 @@
         # Update rate limiters, if table has limits.
         self._client.update_rate_limiters(
             res.get_table_name(), res.get_table_limits())
         return res
 
     def get_table_usage(self, request):
         """
-        Cloud service only.
-
         Gets dynamic information about the specified table such as the current
         throughput usage. Usage information is collected in time slices and
         returned in individual usage records. It is possible to specify a
         time-based range of usage records using input parameters.
 
+        Cloud service only.
+
         :param request: the input parameters for the operation.
         :type request: TableUsageRequest
         :returns: the result of the operation.
         :rtype: TableUsageResult
         :raises IllegalArgumentException: raises the exception if request is not
             an instance of :py:class:`TableUsageRequest`.
         :raises TableNotFoundException: raises the exception if the specified
@@ -416,25 +416,23 @@
         :type request: QueryRequest
         :returns: the result of the operation.
         :rtype: QueryResult
         :raises IllegalArgumentException: raises the exception if request is not
             an instance of :py:class:`QueryRequest`.
         :raises NoSQLException: raises the exception if the operation cannot be
             performed for any other reason.
-        :versionadded: 5.3.6
+        :versionadded:: 5.3.6
         """
         if not isinstance(request, QueryRequest):
             raise IllegalArgumentException(
                 'The parameter should be an instance of QueryRequest.')
         return QueryIterableResult(request, self)
 
     def system_request(self, request):
         """
-        On-premise only.
-
         Performs a system operation on the system, such as administrative
         operations that don't affect a specific table. For table-specific
         operations use :py:meth:`table_request` or :py:meth:`do_table_request`.
 
         Examples of statements in the :py:class:`SystemRequest` passed to this
         method include:
 
@@ -442,14 +440,16 @@
             CREATE USER some_user IDENTIFIED BY password\n
             CREATE ROLE some_role\n
             GRANT ROLE some_role TO USER some_user
 
         This operation is implicitly asynchronous. The caller must poll using
         methods on :py:class:`SystemResult` to determine when it has completed.
 
+        On-premises only.
+
         :param request: the input parameters for the operation.
         :type request: SystemRequest
         :returns: the result of the operation.
         :rtype: SystemResult
         :raises IllegalArgumentException: raises the exception if request is not
             an instance of :py:class:`SystemRequest`.
         :raises NoSQLException: raises the exception if the operation cannot be
@@ -458,19 +458,19 @@
         if not isinstance(request, SystemRequest):
             raise IllegalArgumentException(
                 'The parameter should be an instance of SystemRequest.')
         return self._execute(request)
 
     def system_status(self, request):
         """
-        On-premise only.
-
         Checks the status of an operation previously performed using
         :py:meth:`system_request`.
 
+        On-premises only.
+
         :param request: the input parameters for the operation.
         :type request: SystemStatusRequest
         :returns: the result of the operation.
         :rtype: SystemResult
         :raises IllegalArgumentException: raises the exception if request is not
             an instance of :py:class:`SystemStatusRequest`.
         :raises NoSQLException: raises the exception if the operation cannot be
@@ -545,18 +545,19 @@
         if self._client is not None:
             self._client.shut_down()
             self._client = None
 
     def do_system_request(self, statement, timeout_ms=30000,
                           poll_interval_ms=1000):
         """
-        On-premise only.
-
         A convenience method that performs a SystemRequest and waits for
         completion of the operation. This is the same as calling
+
+        On-premises only.
+
         :py:meth:`system_request` then calling
         :py:meth:`SystemResult.wait_for_completion`. If the operation fails an
         exception is thrown.
 
         System requests are those related to namespaces and security and are
         generally independent of specific tables. Examples of statements include
 
@@ -616,18 +617,18 @@
                 'The parameter should be an instance of TableRequest.')
         res = self.table_request(request)
         res.wait_for_completion(self, timeout_ms, poll_interval_ms)
         return res
 
     def list_namespaces(self):
         """
-        On-premise only.
-
         Returns the namespaces in a store as a list of string.
 
+        On-premises only.
+
         :returns: the namespaces, or None if none are found.
         :rtype: list(str)
         """
         res = self.do_system_request('show as json namespaces')
         json_res = res.get_result_string()
         if json_res is None:
             return None
@@ -638,18 +639,18 @@
         results = list()
         for namespace in namespaces:
             results.append(namespace)
         return results
 
     def list_roles(self):
         """
-        On-premise only.
-
         Returns the roles in a store as a list of string.
 
+        On-premises only.
+
         :returns: the list of roles, or None if none are found.
         :rtype: list(str)
         """
         res = self.do_system_request('show as json roles')
         json_res = res.get_result_string()
         if json_res is None:
             return None
@@ -660,18 +661,18 @@
         results = list()
         for role in roles:
             results.append(role['name'])
         return results
 
     def list_users(self):
         """
-        On-premise only.
-
         Returns the users in a store as a list of :py:class:`UserInfo`.
 
+        On-premises only.
+
         :returns: the list of users, or None if none are found.
         :rtype: list(UserInfo)
         """
         res = self.do_system_request('show as json users')
         json_res = res.get_result_string()
         if json_res is None:
             return None
@@ -680,14 +681,80 @@
         if users is None:
             return None
         results = list()
         for user in users:
             results.append(UserInfo(user['id'], user['name']))
         return results
 
+    def add_replica(self, request):
+        """
+        Adds a replica to a table
+
+        This operation is implicitly asynchronous. The caller must poll using
+        methods on :py:class:`TableResult` to determine when it has completed.
+
+        Cloud service only.
+
+        :param request: the input parameters for the operation.
+        :type request: AddReplicaRequest
+        :returns: the result of the operation.
+        :rtype: TableResult
+        :raises IllegalArgumentException: raises the exception if any of the
+            parameters are invalid or required parameters are missing.
+        :raises RequestTimeoutException: raises the exception if the operation
+            times out.
+        :raises NoSQLException: raises the exception if the operation cannot be
+            performed for any other reason.
+        :versionadded:: 5.4.2
+        """
+        return self._execute(request)
+
+    def drop_replica(self, request):
+        """
+        Drops a replica from a table
+
+        This operation is implicitly asynchronous. The caller must poll using
+        methods on :py:class:`TableResult` to determine when it has completed.
+
+        Cloud service only.
+
+        :param request: the input parameters for the operation.
+        :type request: DropReplicaRequest
+        :returns: the result of the operation.
+        :rtype: TableResult
+        :raises IllegalArgumentException: raises the exception if any of the
+            parameters are invalid or required parameters are missing.
+        :raises RequestTimeoutException: raises the exception if the operation
+            times out.
+        :raises NoSQLException: raises the exception if the operation cannot be
+            performed for any other reason.
+        :versionadded:: 5.4.2
+        """
+        return self._execute(request)
+
+    def get_replica_stats(self, request):
+        """
+        Gets replica statistics information
+
+        Cloud service only.
+
+        :param request: the input parameters for the operation.
+        :type request: ReplicaStatsRequest
+        :returns: the result of the operation.
+        :rtype: ReplicaStatsResult
+        :raises IllegalArgumentException: raises the exception if any of the
+            parameters are invalid or required parameters are missing.
+        :raises TableNotFoundException: raises the exception if the specified
+            table does not exist.
+        :raises NoSQLException: raises the exception if the operation cannot be
+            performed for any other reason.
+        :versionadded:: 5.4.2
+        """
+        return self._execute(request)
+
     def get_client(self):
         # For testing use
         return self._client
 
     def _execute(self, request):
         # Ensure that the client exists and hasn't been closed.
         if self._client is None:
```

### Comparing `borneo-5.4.1/src/borneo/exception.py` & `borneo-5.4.2/src/borneo/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 
 class IllegalArgumentException(RuntimeError):
@@ -289,14 +289,25 @@
     permission to perform a request.
     """
 
     def __init__(self, message):
         super(UnauthorizedException, self).__init__(message)
 
 
+class UnsupportedQueryVersionException(NoSQLException):
+    """
+    The exception is thrown if the server does not support the current
+    query protocol version
+    :versionadded:: 5.4.2
+    """
+
+    def __init__(self, message):
+        super(UnsupportedQueryVersionException, self).__init__(message)
+
+
 class IndexExistsException(ResourceExistsException):
     """
     The operation attempted to create an index for a table but the named index
     already exists.
     """
 
     def __init__(self, message):
@@ -522,7 +533,20 @@
     that callers use a delay before retrying in order to minimize the chance
     that a retry will also be throttled. Applications should attempt to avoid
     throttling exceptions by rate limiting themselves to the degree possible.
     """
 
     def __init__(self, message):
         super(WriteThrottlingException, self).__init__(message)
+
+
+class TableNotReadyException(RetryableException):
+    """
+    Cloud service only
+
+    An exception that is thrown when an operation is attemped on a replicated
+    table that is not yet fully initialized
+    :versionadded:: 5.4.2
+    """
+
+    def __init__(self, message):
+        super(TableNotReadyException, self).__init__(message)
```

### Comparing `borneo-5.4.1/src/borneo/http.py` & `borneo-5.4.2/src/borneo/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from abc import ABCMeta, abstractmethod
 from io import UnsupportedOperation
@@ -13,16 +13,16 @@
 
 from requests import ConnectionError, Timeout, codes
 
 from .common import ByteInputStream, CheckValue, HttpConstants, synchronized
 from .exception import (
     IllegalStateException, NoSQLException,
     ReadThrottlingException, RequestTimeoutException, RetryableException,
-    SecurityInfoNotReadyException, UnsupportedProtocolException,
-    WriteThrottlingException)
+    SecurityInfoNotReadyException, UnsupportedQueryVersionException,
+    UnsupportedProtocolException, WriteThrottlingException)
 from .serdeutil import SerdeUtil
 
 try:
     from . import config
     from . import kv
     from . import operations
 except ImportError:
@@ -246,19 +246,20 @@
                     except Exception as e:
                         exception = e
                         break
                 # Ensure limiting didn't throw us over the timeout
                 if self._timeout_request(start_ms, timeout_ms):
                     break
                 if self._auth_provider is not None:
+                    content = payload if self.require_content_signed() else None
                     auth_string = self._auth_provider.get_authorization_string(
                         self._request)
                     self._auth_provider.validate_auth_string(auth_string)
                     self._auth_provider.set_required_headers(
-                        self._request, auth_string, headers)
+                        self._request, auth_string, headers, content)
                 num_retried = self._request.get_num_retries()
             if num_retried > 0:
                 self._log_retried(num_retried, exception)
             response = None
             network_time = 0
             if stats_config is not None:
                 time()
@@ -318,15 +319,14 @@
                     self._request.set_rate_limit_delayed_ms(rate_delayed_ms)
                     # Copy retry stats to Result on successful operation.
                     res.set_retry_stats(self._request.get_retry_stats())
                     if stats_config is not None:
                         stats_config.observe(self._request, req_size,
                                              len(response.content),
                                              network_time)
-
                     # check for a Set-Cookie header
                     cookie = response.headers.get('Set-Cookie', None)
                     if cookie is not None and cookie.startswith('session='):
                         self._client.set_session_cookie(cookie)
                     return res
                 else:
                     res = HttpResponse(response.content.decode(),
@@ -400,14 +400,27 @@
                 original exception.
                 """
                 self._request.add_retry_exception(re.__class__.__name__)
                 self._handle_retry(re, self._request)
                 self._request.increment_retries()
                 exception = re
                 continue
+            except UnsupportedQueryVersionException as uqve:
+                if self._client.decrement_query_version():
+                    if self._request is not None:
+                        payload = self._client.serialize_request(self._request,
+                                                                 headers)
+                    self._request.increment_retries()
+                    # don't set exception for this case -- it is misleading
+                    # exception = uqve
+                    continue
+                self._logutils.log_error(
+                    'Client execution UnsupportedQueryVersionException: ' +
+                    str(uqve))
+                raise uqve
             except UnsupportedProtocolException as upe:
                 if self._client.decrement_serial_version():
                     if self._request is not None:
                         payload = self._client.serialize_request(self._request,
                                                                  headers)
                     self._request.increment_retries()
                     # don't set exception for this case -- it is misleading
@@ -453,14 +466,24 @@
         if stats_config is not None:
             stats_config.observe_error(self._request)
         raise RequestTimeoutException(
             'Request timed out after ' + str(num_retried) +
             (' retry.' if num_retried == 0 or num_retried == 1
              else ' retries. ') + str(retry_stats), timeout_ms, exception)
 
+    def require_content_signed(self):
+        """
+        This is only needed for the cloud for cross-region request for
+        Global Active Tables that may need an OBO token. The requests
+        include add/drop replica as well as some DDL requests (indexes)
+        """
+        return isinstance(self._request, operations.AddReplicaRequest) or \
+            isinstance(self._request, operations.DropReplicaRequest) or \
+            isinstance(self._request, operations.TableRequest)
+
     @staticmethod
     def _consume_limiter_units(rl, units, timeout_ms):
         """
         Consume rate limiter units after successful operation. Returns the
         number of milliseconds delayed due to rate limiting.
         """
         if rl is None or units <= 0:
```

### Comparing `borneo-5.4.1/src/borneo/iam/iam.py` & `borneo-5.4.2/src/borneo/iam/iam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 OCI_PYTHON_SDK_NO_SERVICE_IMPORTS = True
 
@@ -19,14 +19,16 @@
     # noinspection PyUnresolvedReferences
     from oci.auth.signers import SecurityTokenSigner
     # noinspection PyUnresolvedReferences
     from oci.auth.signers import EphemeralResourcePrincipalSigner
     # noinspection PyUnresolvedReferences
     from oci.auth.signers import InstancePrincipalsSecurityTokenSigner
     # noinspection PyUnresolvedReferences
+    from oci.auth.signers import OkeWorkloadIdentityResourcePrincipalSigner
+    # noinspection PyUnresolvedReferences
     from oci.auth.signers import get_resource_principals_signer
     # noinspection PyUnresolvedReferences
     from oci.config import from_file
 
     oci = 'yes'
 except ImportError:
     oci = None
@@ -274,22 +276,30 @@
 
     def set_logger(self, logger):
         CheckValue.check_logger(logger, 'logger')
         self._logger = logger
         self._logutils = LogUtils(logger)
         return self
 
-    def set_required_headers(self, request, auth_string, headers):
-        sig_details = self._get_signature_details()
+    def set_required_headers(self, request, auth_string, headers,
+                                 content = None):
+        sig_details = self._get_signature_details(content, headers)
         if sig_details is None:
             return
+        # choose headers from signature:
+        #   authorization, date
+        #   optionally: opc-obo-token, x-content-sha256
+
         headers[HttpConstants.AUTHORIZATION] = sig_details['authorization']
         headers[HttpConstants.DATE] = sig_details['date']
         if sig_details.get(HttpConstants.OPC_OBO_TOKEN) is not None:
             headers[HttpConstants.OPC_OBO_TOKEN] = sig_details['opc-obo-token']
+        if content is not None:
+            headers[HttpConstants.X_CONTENT_SHA256] = \
+                       sig_details['x-content-sha256']
         compartment = request.get_compartment()
         if compartment is None:
             # If request doesn't has compartment, set the tenant id as the
             # default compartment, which is the root compartment in IAM if using
             # user principal. If using an instance principal this value is
             # None.
             compartment = self._get_tenant_ocid()
@@ -379,33 +389,44 @@
         SignatureProvider._check_oci()
         signature_provider = SignatureProvider(
             get_resource_principals_signer())
         return (signature_provider if logger is None else
                 signature_provider.set_logger(logger))
 
     @synchronized
-    def get_signature_details_internal(self):
-        # Visible for testing.
-        request = Request(method='post', url=self._service_url)
-        request = self._provider.without_content_headers(request.prepare())
+    def get_signature_details_internal(self, content=None, headers=None):
+        # Visible for testing
+        # the OCI signing code uses a Request instance even though that
+        # is not what we send (see caller in http.py). The signing ends
+        # up putting the required signature in the headers
+        # NOTE: Signer in OCI is callable object
+        request = Request(method='post', url=self._service_url, data=content, headers=headers)
+        if content is None:
+            request = self._provider.without_content_headers(request.prepare())
+        else:
+            request = self._provider(request.prepare())
         sig_details = request.headers
-        self._signature_cache.set(SignatureProvider.CACHE_KEY, sig_details)
-        self._schedule_refresh()
+        # don't cache content-signed requests (TableRequest, Add/Drop Replica)
+        if content is None:
+            self._signature_cache.set(SignatureProvider.CACHE_KEY, sig_details)
+            self._schedule_refresh()
         return sig_details
 
     @staticmethod
     def _check_oci():
         if oci is None:
             raise ImportError('Package "oci" is required; please install.')
 
-    def _get_signature_details(self):
-        sig_details = self._signature_cache.get(SignatureProvider.CACHE_KEY)
-        if sig_details is not None:
-            return sig_details
-        return self.get_signature_details_internal()
+    def _get_signature_details(self, content=None, headers=None):
+        # don't use cache if signing content
+        if content is None:
+            sig_details = self._signature_cache.get(SignatureProvider.CACHE_KEY)
+            if sig_details is not None:
+                return sig_details
+        return self.get_signature_details_internal(content, headers)
 
     def _get_tenant_ocid(self):
         """
         Get tenant OCID if using user principal.
 
         :returns: tenant OCID of user.
         :rtype: str
@@ -416,20 +437,21 @@
     def _refresh_task(self):
         timeout = self._refresh_ahead
         start_ms = int(round(time() * 1000))
         error_logged = False
         while True:
             try:
                 # refresh security token before create new signature
-                if (isinstance(
-                        self._provider,
-                        InstancePrincipalsSecurityTokenSigner) or
-                        isinstance(
-                            self._provider,
-                            EphemeralResourcePrincipalSigner)):
+                if (
+                    isinstance(self._provider, InstancePrincipalsSecurityTokenSigner)
+                    or isinstance(
+                        self._provider, OkeWorkloadIdentityResourcePrincipalSigner
+                    )
+                    or isinstance(self._provider, EphemeralResourcePrincipalSigner)
+                ):
                     self._provider.refresh_security_token()
 
                 self.get_signature_details_internal()
                 return
             except Exception as e:
                 # Ignore the refresh failure, then sleep and try again until
                 # the timeout. Log the failure the first time only. If the
```

### Comparing `borneo-5.4.1/src/borneo/kv/exception.py` & `borneo-5.4.2/src/borneo/kv/exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from borneo.exception import NoSQLException
```

### Comparing `borneo-5.4.1/src/borneo/kv/kv.py` & `borneo-5.4.2/src/borneo/kv/kv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from base64 import b64encode
 from json import loads
```

### Comparing `borneo-5.4.1/src/borneo/nson.py` & `borneo-5.4.2/src/borneo/nson.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 #
 from base64 import b64encode
 from collections import OrderedDict
 
 import borneo.operations
 from .common import (
     ByteInputStream, ByteOutputStream, Empty, IndexInfo, PreparedStatement,
-    TableLimits, TableUsage, Version)
+    Replica, ReplicaStats, TableLimits, TableUsage, Version)
 from .exception import IllegalArgumentException
 from .nson_protocol import *
 from .query import PlanIter, QueryDriver, TopologyInfo
 from .serde import (math_name_to_value)
 from .serdeutil import (SerdeUtil, RequestSerializer, NsonEventHandler)
 
-
 #
 # Contains methods to serialize and deserialize NSON
 #
 # Maps, arrays, other supported NSON datatypes
 # The supported types and their associated numeric values
 # are defined in serdeutil in SerdeUtil.FIELD_VALUE_TYPE
 #
@@ -93,15 +92,16 @@
     #
 
     @staticmethod
     def read_type(bis, expected_type):
         t = bis.read_byte()
         if t != expected_type:
             raise IllegalArgumentException(
-                'Expected type ' + str(expected_type) + ', received type ' + t)
+                'Expected type ' + str(expected_type) +
+                ', received type ' + str(t))
 
     @staticmethod
     def read_int(bis):
         Nson.read_type(bis, SerdeUtil.FIELD_VALUE_TYPE.INTEGER)
         return SerdeUtil.read_packed_int(bis)
 
     @staticmethod
@@ -321,14 +321,15 @@
             raise IllegalArgumentException(
                 'Unknown value type code: ' + str(t))
 
     @staticmethod
     def iso_time_to_ms(iso_str):
         return SerdeUtil.iso_time_to_ms(iso_str)
 
+
 class NsonSerializer(NsonEventHandler):
     """
     This class serializes an NSON "document." It maintains state for nested
     maps and arrays.
     """
 
     def stop(self):
@@ -879,14 +880,16 @@
             name = walker.get_current_name()
             if name == ERROR_CODE:
                 Proto.handle_error_code(walker)
             elif name == CONSUMED:
                 Proto.read_consumed_capacity(bis, result)
             elif name == ROW:
                 Proto.read_row(bis, result)
+            elif name == TOPOLOGY_INFO:
+                Proto.read_topology_info(bis, result);
             else:
                 walker.skip()
 
         return result
 
 
 #
@@ -960,14 +963,16 @@
             elif name == ROW_VERSION:
                 result.set_version(Version.create_version(
                     Nson.read_binary(bis)))
             elif name == RETURN_INFO:
                 Proto.read_return_info(bis, result)
             elif name == GENERATED:
                 result.set_generated_value(Proto.nson_to_value(bis))
+            elif name == TOPOLOGY_INFO:
+                Proto.read_topology_info(bis, result);
             else:
                 walker.skip()
 
         return result
 
     @staticmethod
     def write_put_request(ns, request):
@@ -1046,14 +1051,16 @@
                 Proto.handle_error_code(walker)
             elif name == CONSUMED:
                 Proto.read_consumed_capacity(bis, result)
             elif name == SUCCESS:
                 result.set_success(Nson.read_boolean(bis))
             elif name == RETURN_INFO:
                 Proto.read_return_info(bis, result)
+            elif name == TOPOLOGY_INFO:
+                Proto.read_topology_info(bis, result);
             else:
                 walker.skip()
 
         return result
 
     @staticmethod
     def write_delete_request(ns, request):
@@ -1540,14 +1547,16 @@
                 Proto.handle_error_code(walker)
             elif name == CONSUMED:
                 Proto.read_consumed_capacity(bis, result)
             elif name == NUM_DELETIONS:
                 result.set_num_deletions(Nson.read_int(bis))
             elif name == CONTINUATION_KEY:
                 result.set_continuation_key(Nson.read_binary(bis))
+            elif name == TOPOLOGY_INFO:
+                Proto.read_topology_info(bis, result);
             else:
                 walker.skip()
 
         return result
 
     #
     # "range": {
@@ -1682,14 +1691,16 @@
                     fname = fwalker.get_current_name()
                     if fname == WM_FAIL_INDEX:
                         result.set_failed_operation_index(Nson.read_int(bis))
                     elif fname == WM_FAIL_RESULT:
                         result.add_result(self._read_operation_result(bis))
                     else:
                         fwalker.skip()
+            elif name == TOPOLOGY_INFO:
+                Proto.read_topology_info(bis, result);
             else:
                 walker.skip()
         return result
 
     #
     # Each op is an anonymous map inside and array of maps
     #
@@ -1770,15 +1781,15 @@
         ns.start_map()  # top-level object
 
         Proto.start_map(ns, HEADER)
         Proto.write_header(ns, SerdeUtil.OP_CODE.PREPARE, request)
         Proto.end_map(ns, HEADER)
 
         Proto.start_map(ns, PAYLOAD)
-        Proto.write_int_map_field(ns, QUERY_VERSION, QueryDriver.QUERY_VERSION)
+        Proto.write_int_map_field(ns, QUERY_VERSION, request.get_query_version())
         Proto.write_string_map_field(ns, STATEMENT, request.get_statement())
         if request.get_query_plan():
             Proto.write_bool_map_field(ns, GET_QUERY_PLAN, request.get_query_plan())
         if request.get_query_schema():
             Proto.write_bool_map_field(ns, GET_QUERY_SCHEMA,
                                        request.get_query_schema())
 
@@ -1831,23 +1842,27 @@
         ns.start_map()  # top-level object
 
         Proto.start_map(ns, HEADER)
         Proto.write_header(ns, SerdeUtil.OP_CODE.QUERY, request)
         Proto.end_map(ns, HEADER)
 
         Proto.start_map(ns, PAYLOAD)
-        Proto.write_int_map_field(ns, QUERY_VERSION, QueryDriver.QUERY_VERSION)
+        Proto.write_int_map_field(ns, QUERY_VERSION, request.get_query_version())
         Proto.write_int_map_field_not_zero(
             ns, MAX_READ_KB, request.get_max_read_kb())
         Proto.write_int_map_field_not_zero(
             ns, MAX_WRITE_KB, request.get_max_write_kb())
         Proto.write_int_map_field_not_zero(
             ns, NUMBER_LIMIT, request.get_limit())
         Proto.write_int_map_field_not_zero(
             ns, TRACE_LEVEL, request.get_trace_level())
+        if request.get_trace_level() > 0:
+            Proto.write_bool_map_field(ns, TRACE_TO_LOG_FILES,
+                                       request.get_log_file_tracing())
+            Proto.write_int_map_field(ns, BATCH_COUNTER, request.get_batch_counter())
         Proto.write_consistency(ns, request.get_consistency())
         Proto.write_consistency(ns, request.get_consistency())
         Proto.write_durability(ns, request)
 
         if request.is_prepared():
             Proto.write_bool_map_field(ns, IS_PREPARED, True)
             Proto.write_bool_map_field(ns, IS_SIMPLE_QUERY, request.is_simple_query())
@@ -1857,21 +1872,30 @@
                 ns, request.get_prepared_statement().get_variables())
         else:
             Proto.write_string_map_field(ns, STATEMENT, request.get_statement())
 
         if request.get_cont_key() is not None:
             Proto.write_bin_map_field(
                 ns, CONTINUATION_KEY, request.get_cont_key())
+        #
+        # server memory consumption is purposely left out as not necessary
+        # at this time (see Java)
+        #
+
         if request.get_math_context() is not None:
             self._write_math_context(ns, request.get_math_context())
         if request.get_shard_id() != -1:
             Proto.write_int_map_field(ns, SHARD_ID, request.get_shard_id())
-        if request.topology_seq_num() != -1:
-            Proto.write_int_map_field(
-                ns, TOPO_SEQ_NUM, request.topology_seq_num())
+
+        if request.get_query_version() >= QueryDriver.QUERY_V4:
+            if request.get_query_name() is not None:
+                Proto.write_string_map_field(ns, QUERY_NAME,
+                                             request.get_query_name())
+            if request.get_virtual_scan() is not None:
+                Proto.write_virtual_scan(ns, request.get_virtual_scan())
 
         Proto.end_map(ns, PAYLOAD)
 
         ns.end_map()  # top-level object
 
     @staticmethod
     def _write_bind_variables(ns, variables):
@@ -1902,14 +1926,198 @@
         Proto.deserialize_prepare_or_query(
             request, result,
             None, None,  # prepare request/result
             bis)
         return result
 
 
+#
+# AddReplicaRequest
+#
+# Header:
+#  Normal header table name required
+#
+# Payload:
+# {
+#   "payload" : {
+#      region: str, required
+#      if not 0 or None, read units, write units, match_etag
+#   }
+# }
+#
+# Non-error response:
+#  TableResult
+#
+class AddReplicaRequestSerializer(RequestSerializer):
+
+    def serialize(self, request, bos, serial_version):
+        ns = NsonSerializer(bos)
+        ns.start_map()  # top-level object
+
+        Proto.start_map(ns, HEADER)
+        Proto.write_header(ns, SerdeUtil.OP_CODE.ADD_REPLICA, request)
+        Proto.end_map(ns, HEADER)
+
+        Proto.start_map(ns, PAYLOAD)
+        Proto.write_string_map_field(ns, REGION, request.get_replica_name())
+        Proto.write_int_map_field_not_zero(ns, READ_UNITS,
+                                               request.get_read_units())
+        Proto.write_int_map_field_not_zero(ns, WRITE_UNITS,
+                                               request.get_write_units())
+        Proto.write_string_map_field(ns, ETAG, request.get_match_etag())
+        Proto.end_map(ns, PAYLOAD)
+
+        ns.end_map()  # top-level object
+
+    def deserialize(self, request, bis, serial_version):
+        return Proto.deserialize_table_result(bis)
+
+#
+# DropReplicaRequest
+#
+# Header:
+#  Normal header table name required
+#
+# Payload:
+# {
+#   "payload" : {
+#      region: str, required
+#      if not None,  match_etag
+#   }
+# }
+#
+# Non-error response:
+#  TableResult
+#
+class DropReplicaRequestSerializer(RequestSerializer):
+
+    def serialize(self, request, bos, serial_version):
+        ns = NsonSerializer(bos)
+        ns.start_map()  # top-level object
+
+        Proto.start_map(ns, HEADER)
+        Proto.write_header(ns, SerdeUtil.OP_CODE.DROP_REPLICA, request)
+        Proto.end_map(ns, HEADER)
+
+        Proto.start_map(ns, PAYLOAD)
+        Proto.write_string_map_field(ns, REGION, request.get_replica_name())
+        Proto.write_string_map_field(ns, ETAG, request.get_match_etag())
+        Proto.end_map(ns, PAYLOAD)
+
+        ns.end_map()  # top-level object
+
+    def deserialize(self, request, bis, serial_version):
+        return Proto.deserialize_table_result(bis)
+
+#
+# ReplicaStatsRequest
+#
+# Header:
+#  Normal header table name required
+#
+# Payload:
+# {
+#   "payload" : {
+#      region: str, required
+#      optional start_time str
+#      optional limit int
+#   }
+# }
+#
+# Non-error response:
+#  GetReplicaStatsResult:
+#
+#   table_name (string)
+#   next_start_time (int)
+#   replica_stats (Map<string, Array<ReplicaStats>>)
+#       key - region (string)
+#       value - array of ReplicaStats
+#       ReplicaStats:
+#         time (int)
+#         replica_lag (int)
+#
+class ReplicaStatsRequestSerializer(RequestSerializer):
+
+    def serialize(self, request, bos, serial_version):
+        ns = NsonSerializer(bos)
+        ns.start_map()  # top-level object
+
+        Proto.start_map(ns, HEADER)
+        Proto.write_header(ns, SerdeUtil.OP_CODE.GET_REPLICA_STATS, request)
+        Proto.end_map(ns, HEADER)
+
+        Proto.start_map(ns, PAYLOAD)
+        Proto.write_string_map_field(ns, REGION, request.get_replica_name())
+        Proto.write_string_map_field(ns, START, request.get_start_time_str())
+        Proto.write_int_map_field_not_zero(ns, LIST_MAX_TO_READ,
+                                               request.get_limit())
+        Proto.end_map(ns, PAYLOAD)
+
+        ns.end_map()  # top-level object
+
+    def deserialize(self, request, bis, serial_version):
+        result = borneo.operations.ReplicaStatsResult()
+        walker = MapWalker(bis)
+        while walker.has_next():
+            walker.next()
+            name = walker.get_current_name()
+            if name == ERROR_CODE:
+                Proto.handle_error_code(walker)
+            elif name == TABLE_NAME:
+                result.set_table_name(Nson.read_string(bis))
+            elif name == NEXT_START_TIME:
+                result.set_next_start_time(Nson.read_long(bis))
+            elif name == REPLICA_STATS:
+                ReplicaStatsRequestSerializer.read_replica_stats(bis, result)
+            else:
+                walker.skip()
+
+        return result
+
+    #
+    # Map, key is string, value is ReplicaStats
+    #  key - region (str)
+    #  value -- array of ReplicaStats
+    #      time (long)
+    #      lag (int)
+    #
+    @staticmethod
+    def read_replica_stats(bis, result):
+        records_map = dict()
+        walker = MapWalker(bis)
+        while walker.has_next():
+            walker.next()
+            replica_name = walker.get_current_name()
+            # value is array of stats
+            t = bis.read_byte()
+            if t != SerdeUtil.FIELD_VALUE_TYPE.ARRAY:
+                raise IllegalArgumentException(
+                    'Bad type in GetReplicaStats: ' + str(t) +
+                    ' should be ARRAY')
+            # consume total size of array
+            SerdeUtil.read_full_int(bis)  # total length in bytes
+            num_elements = SerdeUtil.read_full_int(bis)
+            records = list()
+            for i in range(0,num_elements):
+                stats = ReplicaStats()
+                swalker = MapWalker(bis)
+                while swalker.has_next():
+                    swalker.next()
+                    name = swalker.get_current_name()
+                    if name == TIME:
+                        stats._collection_time_millis = Nson.read_long(bis)
+                    elif name == REPLICA_LAG:
+                        stats._replica_lag = Nson.read_int(bis)
+                    else:
+                        swalker.skip()
+
+                records.append(stats);
+            records_map[replica_name] = records
+        result.set_stats_records(records_map)
+
 # noinspection PyArgumentEqualDefault
 class Proto(object):
     #
     # Common methods for serializers
     #
 
     #
@@ -1919,14 +2127,15 @@
     def write_header(ns, op, request):
         Proto.write_int_map_field(ns, VERSION,
                                   SerdeUtil.SERIAL_VERSION_4)
         if request.get_table_name() is not None:
             Proto.write_string_map_field(ns, TABLE_NAME,
                                          request.get_table_name())
         Proto.write_int_map_field(ns, OP_CODE, op)
+        Proto.write_int_map_field(ns, TOPO_SEQ_NUM, request.get_topo_seq_num())
         Proto.write_int_map_field(ns, TIMEOUT, request.get_timeout())
 
     @staticmethod
     def write_consistency(ns, consistency):
         if consistency is not None:
             Proto.start_map(ns, CONSISTENCY)
             Proto.write_int_map_field(ns, TYPE, consistency)
@@ -2039,14 +2248,24 @@
     @staticmethod
     def write_bin_map_field(ns, name, value):
         if value is not None:
             ns.start_map_field(name)
             ns.binary_value(value)
             ns.end_map_field(name)
 
+    @staticmethod
+    def write_int_array_map_field(ns, name, value):
+        if value is not None:
+            Proto.start_array(ns, name)
+            for v in values:
+                ns.start_array_field()
+                ns.integer_value(v)
+                ns.end_array_field()
+            Proto.end_array(ns, name)
+
     #
     # start/end complex types
     #
     @staticmethod
     def start_map(ns, name):
         ns.start_map_field(name)
         ns.start_map()
@@ -2063,14 +2282,45 @@
 
     @staticmethod
     def end_array(ns, name):
         ns.end_array()
         ns.end_map_field(name)
 
     #
+    #
+    #
+    @staticmethod
+    def write_virtual_scan(ns, vs):
+        start_map(ns, VIRTUAL_SCAN)
+        Proto.write_int_map_field(ns, VIRTUAL_SCAN_SID, vs[VIRTUAL_SCAN_SID])
+        Proto.write_int_map_field(ns, VIRTUAL_SCAN_PID, vs[VIRTUAL_SCAN_PID])
+        info_sent = vs['info_sent']
+        if not info_sent:
+            Proto.write_bin_map_field(ns, VIRTUAL_SCAN_PRIM_KEY,
+                                          vs[VIRTUAL_SCAN_PRIM_KEY])
+            Proto.write_bin_map_field(ns, VIRTUAL_SCAN_SEC_KEY,
+                                          vs[VIRTUAL_SCAN_SEC_KEY])
+            Proto.write_bool_map_field(ns, VIRTUAL_SCAN_MOVE_AFTER,
+                                           vs[VIRTUAL_SCAN_MOVE_AFTER])
+            Proto.write_bin_map_field(ns, VIRTUAL_SCAN_JOIN_DESC_RESUME_KEY,
+                                          vs[VIRTUAL_SCAN_JOIN_DESC_RESUME_KEY])
+            Proto.write_int_array_map_field(ns,
+                                            VIRTUAL_SCAN_JOIN_PATH_TABLES,
+                                            vs[VIRTUAL_SCAN_JOIN_PATH_TABLES])
+            Proto.write_bin_map_field(ns, VIRTUAL_SCAN_JOIN_PATH_KEY,
+                                          vs[VIRTUAL_SCAN_JOIN_PATH_KEY])
+            Proto.write_bin_map_field(ns, VIRTUAL_SCAN_JOIN_PATH_SEC_KEY,
+                                          vs[VIRTUAL_SCAN_JOIN_PATH_SEC_KEY])
+            Proto.write_bool_map_field(ns, VIRTUAL_SCAN_JOIN_PATH_MATCHED,
+                                           vs[VIRTUAL_SCAN_JOIN_PATH_MATCHED])
+
+        end_map(ns, VIRTUAL_SCAN)
+
+
+    #
     # Deserialization/read methods
     #
 
     # TableResult
     # {
     #   "ERROR_CODE" : 0
     #   "TABLE_NAME" : <string>        # required
@@ -2121,14 +2371,20 @@
                 result.set_operation_id(Nson.read_string(bis))
             elif name == FREE_FORM_TAGS:
                 result.set_free_form_tags(json.loads(Nson.read_string(bis)))
             elif name == DEFINED_TAGS:
                 result.set_defined_tags(json.loads(Nson.read_string(bis)))
             elif name == ETAG:
                 result.set_match_etag(Nson.read_string(bis))
+            elif name == SCHEMA_FROZEN:
+                result.set_schema_frozen(Nson.read_boolean(bis))
+            elif name == INITIALIZED:
+                result.set_local_replica_initialized(Nson.read_boolean(bis))
+            elif name == REPLICAS:
+                Proto.read_replicas(bis, result)
             elif name == LIMITS:
                 lw = MapWalker(bis)
                 ru = 0
                 wu = 0
                 sg = 0
                 mode = SerdeUtil.CAPACITY_MODE.PROVISIONED
                 while lw.has_next():
@@ -2145,14 +2401,53 @@
                     else:
                         lw.skip()
                 result.set_table_limits(TableLimits(ru, wu, sg, mode))
             else:
                 walker.skip()
         return result
 
+    @staticmethod
+    def read_replicas(bis, result):
+        # array of replicas
+        t = bis.read_byte()
+        if t != SerdeUtil.FIELD_VALUE_TYPE.ARRAY:
+            raise IllegalArgumentException(
+                'Bad type in ReadReplicas in TableResult: ' + str(t) +
+                ' should be ARRAY')
+        SerdeUtil.read_full_int(bis)  # total length in bytes
+        num_elements = SerdeUtil.read_full_int(bis)
+        replicas = list()
+        for i in range(0,num_elements):
+            replica = Replica()
+            Proto.read_replica(bis, replica)
+            replicas.append(replica)
+        result.set_replicas(replicas)
+
+
+    @staticmethod
+    def read_replica(bis, replica):
+        walker = MapWalker(bis)
+        while walker.has_next():
+            walker.next()
+            name = walker.get_current_name()
+            if name == REGION:
+                replica._replica_name = Nson.read_string(bis)
+            elif name == TABLE_OCID:
+                replica._replica_ocid = Nson.read_string(bis)
+            elif name == WRITE_UNITS:
+                replica._write_units = Nson.read_int(bis)
+            elif name == LIMITS_MODE:
+                replica._capacity_mode = Nson.read_int(bis)
+            elif name == TABLE_STATE:
+                replica._replica_state = (
+                    SerdeUtil.get_table_state(Nson.read_int(bis)))
+            else:
+                walker.skip()
+
+
     # {
     #   SYSOP_STATE: <int>
     #   SYSOP_RESULT: <string>
     #   STATEMENT: <string>
     #   OPERATION_ID: <string>
     # }
     @staticmethod
@@ -2323,18 +2618,20 @@
         # variables used to construct a PreparedStatement as needed
         dpi = None  # driver plan info
         query_plan = None
         query_schema = None
         table_name = None
         namespace = None
         operation = None
-        proxy_topo_seqnum = None
+        proxy_topo_seqnum = -1 # V3 and earlier
+        shard_ids = None # V3 and earlier
         proxy_prepared_query = None
-        shard_ids = None
         cont_key = None
+        virtual_scans = None # array of dict
+        query_traces = None  # dict
 
         walker = MapWalker(bis)
         while walker.has_next():
             walker.next()
             name = walker.get_current_name()
             if name == ERROR_CODE:
                 Proto.handle_error_code(walker)
@@ -2354,72 +2651,138 @@
                 query_schema = Nson.read_string(bis)
             elif name == TABLE_NAME:
                 table_name = Nson.read_string(bis)
             elif name == NAMESPACE:
                 namespace = Nson.read_string(bis)
             elif name == QUERY_OPERATION:
                 operation = Nson.read_int(bis)
-            elif name == PROXY_TOPO_SEQNUM:
-                proxy_topo_seqnum = Nson.read_int(bis)
-            elif name == SHARD_IDS:
-                # array of int
-                shard_ids = Proto.read_nson_int_array(bis)
             elif name == QUERY_RESULTS:
                 # query only
                 Proto.read_query_results(query_result, bis)
             elif name == CONTINUATION_KEY:
                 # query only
                 cont_key = Nson.read_binary(bis)
             elif name == SORT_PHASE1_RESULTS:
                 # query only
                 Proto.read_phase1_results(query_result, bis)
             elif name == REACHED_LIMIT:
                 # query only
                 if query_result is not None:
                     query_result.set_reached_limit(Nson.read_boolean(bis))
+            elif name == TOPOLOGY_INFO:
+                Proto.read_topology_info(bis,
+                  query_result if query_result is not None else prepare_result);
+            # QUERY_V3 and earlier return topo differently
+            elif name == PROXY_TOPO_SEQNUM:
+                proxy_topo_seqnum = Nson.read_int(bis)
+            elif name == SHARD_IDS:
+                shard_ids = Proto.read_nson_int_array(bis)
+            # new in QUERY_V4
+            elif name == VIRTUAL_SCANS:
+                Nson.read_type(bis, SerdeUtil.FIELD_VALUE_TYPE.ARRAY)
+                SerdeUtil.read_full_int(bis) # array size in bytes
+                num_scans = SerdeUtil.read_full_int(bis)
+                virtual_scans = list()
+                for i in range(num_scans):
+                    virtual_scans.append(Proto.read_virtual_scan(bis))
+            elif name == QUERY_BATCH_TRACES:
+                Nson.read_type(bis, SerdeUtil.FIELD_VALUE_TYPE.ARRAY)
+                SerdeUtil.read_full_int(bis) # array size in bytes
+                # divide by 2 because each trace is 2 strings
+                num_traces = SerdeUtil.read_full_int(bis) / 2
+                query_traces = dict()
+                for i in range(num_traces):
+                    name = Nson.read_string(bis)
+                    trace = Nson.read_string(bis)
+                    query_traces[name] = trace
             else:
                 walker.skip()
 
+        # QUERY_V3 and earlier return topo differently
+        res = query_result if query_result is not None else prepare_result
+        if res.get_topology_info() is None and proxy_topo_seqnum >= 0:
+            res.set_topology_info(proxy_topo_seqnum, shard_ids)
+
         # ensure that the continuation key is cleared if not returned,
         # meaning the query is done
         if query_result is not None:
             query_result.set_continuation_key(cont_key)
             query_request.set_cont_key(query_result.get_continuation_key())
+            query_result.set_virtual_scans(virtual_scans)
+            query_result.set_query_traces(query_traces)
 
         # if this was already prepared and is from a query, we are done
         if request_was_prepared:
             return
-        if proxy_topo_seqnum is not None:
-            ti = TopologyInfo(proxy_topo_seqnum, shard_ids)
-        else:
-            ti = None
         if query_request is not None:
             statement = query_request.get_statement()
         else:
             statement = prepare_request.get_statement()
         prepared_statement = PreparedStatement(
-            statement, query_plan, query_schema, ti,
+            statement, query_plan, query_schema,
             proxy_prepared_query,
             None if dpi is None else dpi.get_plan(),
             None if dpi is None else dpi.get_num_iters(),
             None if dpi is None else dpi.get_num_regs(),
             None if dpi is None else dpi.get_vars(),
             namespace,
             table_name,
             operation)
         if prepare_result is not None:
             prepare_result.set_prepared_statement(prepared_statement)
         elif query_request is not None:
             query_request.set_prepared_statement(prepared_statement)
             if not prepared_statement.is_simple_query():
                 driver = QueryDriver(query_request)
-                driver.set_topology_info(prepared_statement.topology_info())
                 driver.set_prep_cost(query_result.get_read_kb())
                 query_result.set_computed(False)
 
+    @staticmethod
+    def read_virtual_scan(bis):
+        vs = dict()
+        vs[VIRTUAL_SCAN_SID] = -1
+        vs[VIRTUAL_SCAN_PID] = -1
+        vs[VIRTUAL_SCAN_PRIM_KEY] = None
+        vs[VIRTUAL_SCAN_SEC_KEY] = None
+        vs[VIRTUAL_SCAN_MOVE_AFTER] = True
+        vs[VIRTUAL_SCAN_JOIN_DESC_RESUME_KEY] = None
+        vs[VIRTUAL_SCAN_JOIN_PATH_TABLES] = None
+        vs[VIRTUAL_SCAN_JOIN_PATH_KEY] = None
+        vs[VIRTUAL_SCAN_JOIN_PATH_SEC_KEY] = None
+        vs[VIRTUAL_SCAN_JOIN_PATH_MATCHED] = False
+
+        walker = MapWalker(bis)
+        while walker.has_next():
+            walker.next()
+            name = walker.get_current_name()
+            if name == VIRTUAL_SCAN_SID:
+                vs[VIRTUAL_SCAN_SID] = Nson.read_int(bis)
+            if name == VIRTUAL_SCAN_PID:
+                vs[VIRTUAL_SCAN_PID] = Nson.read_int(bis)
+            if name == VIRTUAL_SCAN_PRIM_KEY:
+                vs[VIRTUAL_SCAN_PRIM_KEY] = Nson.read_binary(bis)
+            if name == VIRTUAL_SCAN_SEC_KEY:
+                vs[VIRTUAL_SCAN_SEC_KEY] = Nson.read_binary(bis)
+            if name == VIRTUAL_SCAN_MOVE_AFTER:
+                vs[VIRTUAL_SCAN_MOVE_AFTER] = Nson.read_boolean(bis)
+            if name == VIRTUAL_SCAN_JOIN_DESC_RESUME_KEY:
+                vs[VIRTUAL_SCAN_JOIN_DESC_RESUME_KEY] = Nson.read_binary(bis)
+            if name == VIRTUAL_SCAN_JOIN_PATH_KEY:
+                vs[VIRTUAL_SCAN_JOIN_PATH_KEY] = Nson.read_binary(bis)
+            if name == VIRTUAL_SCAN_JOIN_PATH_SEC_KEY:
+                vs[VIRTUAL_SCAN_JOIN_PATH_SEC_KEY] = Nson.read_binary(bis)
+            if name == VIRTUAL_SCAN_JOIN_PATH_TABLES:
+                vs[VIRTUAL_SCAN_JOIN_PATH_TABLES] = Nson.read_nson_int_array(bis)
+            if name == VIRTUAL_SCAN_JOIN_PATH_MATCHED:
+                vs[VIRTUAL_SCAN_JOIN_PATH_MATCHED] = Nson.read_boolean(bis)
+            else:
+                walker.skip()
+        return vs
+
+
     # array of int for shard_ids in query topology info
     @staticmethod
     def read_nson_int_array(bis):
         t = bis.read_byte()
         if t != SerdeUtil.FIELD_VALUE_TYPE.ARRAY:
             raise IllegalArgumentException(
                 'NSON read int array: stream must be located at type ARRAY')
@@ -2460,14 +2823,39 @@
                 SerdeUtil.read_packed_int_array(bis1))
             cont_keys = list()
             for i in range(len(pids)):
                 cont_keys.append(SerdeUtil.read_bytearray(bis1, False))
             query_result.set_partition_cont_keys(cont_keys)
 
     #
+    # {
+    #   PROXY_TOPO_SEQNUM : int
+    #   SHARD_IDS : [int, ...]
+    # }
+    #
+    @staticmethod
+    def read_topology_info(bis, result):
+        proxy_topo_seqnum = -1
+        shard_ids = None
+
+        walker = MapWalker(bis)
+        while walker.has_next():
+            walker.next()
+            name = walker.get_current_name()
+            if name == PROXY_TOPO_SEQNUM:
+                proxy_topo_seqnum = Nson.read_int(bis)
+            elif name == SHARD_IDS:
+                 # int array
+                 shard_ids = Proto.read_nson_int_array(bis)
+            else:
+                walker.skip()
+        if proxy_topo_seqnum >= 0:
+            result.set_topology_info(proxy_topo_seqnum, shard_ids)
+
+    #
     # Handle success/failure in a response. Success is a 0 error code.
     # Failure is a non-zero code and may also include:
     #  Exception message
     #  Consumed capacity
     #  Retry hints if throttling (future)
     # This method throws an appropriately mapped exception on error and
     # nothing on success.
```

### Comparing `borneo-5.4.1/src/borneo/operations.py` & `borneo-5.4.2/src/borneo/operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 from abc import abstractmethod
 from datetime import datetime
 from decimal import Context, ROUND_HALF_EVEN
 from json import loads
 from time import sleep, time
 
 from dateutil import tz
 
 from .common import (
     CheckValue, Consistency, Durability, FieldRange, PreparedStatement,
-    PutOption, State, SystemState, TableLimits, TimeToLive, Version,
-    deprecated)
+    PutOption, ReplicaStats, State, SystemState, TableLimits, TableUsage,
+    TimeToLive, Version, deprecated)
 from .exception import (
     IllegalArgumentException, RequestTimeoutException)
 from .http import RateLimiter
 from .serde import (
     DeleteRequestSerializer, GetIndexesRequestSerializer,
     GetRequestSerializer, GetTableRequestSerializer, ListTablesRequestSerializer,
     MultiDeleteRequestSerializer,
     PrepareRequestSerializer, PutRequestSerializer, QueryRequestSerializer,
     SystemRequestSerializer, SystemStatusRequestSerializer,
     TableRequestSerializer, TableUsageRequestSerializer,
     WriteMultipleRequestSerializer)
+from .query import TopologyInfo
 from .serdeutil import SerdeUtil
 
 try:
     from . import config
     from . import serdeutil
 except ImportError:
     import config
@@ -53,14 +54,15 @@
         self._retry_stats = None
         self._start_time_ms = 0
         self._table_name = None
         self._timeout_ms = 0
         self._write_rate_limiter = None
         self._rate_limit_delayed_ms = 0
         self._namespace = None
+        self._topo_seq_num = -1
 
     def add_retry_delay_ms(self, millis):
         """
         Internal use only.
 
         This adds time to the total time spent processing retries during a
         single request processing operation.
@@ -102,18 +104,18 @@
         :returns: True if the request expects to do writes (incur write units).
         :rtype: boolean
         """
         return False
 
     def get_compartment(self):
         """
-        Cloud service only.
-
         Get the compartment id or name if set for the request.
 
+        Cloud service only.
+
         :returns: compartment id or name if set for the request, otherwise None
             if not set.
         :rtype: str
         """
         return self._compartment
 
     def get_num_retries(self):
@@ -125,25 +127,25 @@
         """
         if self._retry_stats is None:
             return 0
         return self._retry_stats.get_retries()
 
     def get_read_rate_limiter(self):
         """
-        Cloud service only.
-
         Returns the read rate limiter instance used during this request.
 
         This will be the value supplied via :py:meth:`set_read_rate_limiter`, or
         if that was not called, it may be an instance of an internal rate
         limiter that was configured internally during request processing.
 
         This is supplied for stats and tracing/debugging only. The returned
         limiter should be treated as read-only.
 
+        Cloud service only.
+
         :returns: the rate limiter instance used for read operations, or None if
             no limiter was used.
         :rtype: RateLimiter
         """
         return self._read_rate_limiter
 
     def get_retry_delay_ms(self):
@@ -184,29 +186,36 @@
 
         :returns: the table name, or None if not set.
         :returns: str
         """
         return self._table_name
 
     def get_timeout(self):
+        """
+        Returns the timeout to use for the operation, in milliseconds. A value
+        of 0 indicates that the timeout has not been set.
+
+        :returns: the timeout value.
+        :rtype: int
+        """
         return self._timeout_ms
 
     def get_write_rate_limiter(self):
         """
-        Cloud service only.
-
         Returns the write rate limiter instance used during this request.
 
         This will be the value supplied via :py:meth:`set_write_rate_limiter`,
         or if that was not called, it may be an instance of an internal rate
         limiter that was configured internally during request processing.
 
         This is supplied for stats and tracing/debugging only. The returned
         limiter should be treated as read-only.
 
+        Cloud service only.
+
         :returns: the rate limiter instance used for write operations, or None
             if no limiter was used.
         :rtype: RateLimiter
         """
         return self._write_rate_limiter
 
     def is_query_request(self):
@@ -252,22 +261,22 @@
         self._check_config(cfg)
         if self._timeout_ms == 0:
             self._timeout_ms = cfg.get_default_timeout()
         return self
 
     def set_read_rate_limiter(self, rate_limiter):
         """
-        Cloud service only.
-
         Sets a read rate limiter to use for this request.
 
         This will override any internal rate limiter that may have otherwise
         been used during request processing, and it will be used regardless of
         any rate limiter config.
 
+        Cloud service only.
+
         :param rate_limiter: the rate limiter instance to use for read
             operations.
         :type rate_limiter: RateLimiter
         :returns: self.
         :raises IllegalArgumentException: raises the exception if rate_limiter
             is not an instance of RateLimiter.
         """
@@ -303,22 +312,22 @@
         :param start_time_ms: the start time of request processing.
         :type start_time_ms: int
         """
         self._start_time_ms = start_time_ms
 
     def set_write_rate_limiter(self, rate_limiter):
         """
-        Cloud service only.
-
         Sets a write rate limiter to use for this request.
 
         This will override any internal rate limiter that may have otherwise
         been used during request processing, and it will be used regardless of
         any rate limiter config.
 
+        Cloud service only.
+
         :param rate_limiter: the rate limiter instance to use for write
             operations.
         :type rate_limiter: RateLimiter
         :returns: self.
         :raises IllegalArgumentException: raises the exception if rate_limiter
             is not an instance of RateLimiter.
         """
@@ -342,40 +351,40 @@
             not a string.
         """
         CheckValue.check_str(table_name, 'table_name', True)
         self._table_name = table_name
 
     def set_namespace(self, namespace):
         """
+        Sets the namespace to use for the operation. This will override
+        any configured default value.
+
         Internal use only
 
         On-premises only
 
-        Sets the namespace to use for the operation. This will override
-        any configured default value.
-
         :param namespace: the namespace
         :type namespace: str
         :raises IllegalArgumentException: raises the exception if namespace is
             not a string.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         CheckValue.check_str(namespace, 'namespace', True)
         self._namespace = namespace
 
     def get_namespace(self):
         """
-        On-premises only
-
         Returns the namespace to use for the operation or None if not
         set.
 
+        On-premises only
+
         :returns: namespace, or None if not set.
         :rtype: str
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._namespace
 
     def _set_timeout(self, timeout_ms):
         CheckValue.check_int_gt_zero(timeout_ms, 'timeout_ms')
         self._timeout_ms = timeout_ms
 
@@ -411,19 +420,29 @@
     @staticmethod
     def _check_rate_limiter(rate_limiter, name):
         if (rate_limiter is not None and
                 not isinstance(rate_limiter, RateLimiter)):
             raise IllegalArgumentException(
                 name + ' requires an instance of RateLimiter as parameter.')
 
-    @abstractmethod
     def get_request_name(self):
         # type () -> str
         pass
 
+    def set_query_version(self, version):
+        pass
+
+    def set_topo_seq_num(self, num):
+        if self._topo_seq_num < 0:
+            self._topo_seq_num = num;
+        return self
+
+    def get_topo_seq_num(self):
+        return self._topo_seq_num
+
 
 class WriteRequest(Request):
     """
     Represents a base class for the single row modifying operations
     :py:meth:`NoSQLHandle.put` and :py:meth:`NoSQLHandle.delete`.
 
     This class encapsulates the common parameters of table name and the return
@@ -596,26 +615,26 @@
         :returns: the key value, or None if not set.
         :rtype: dict
         """
         return self._key
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -718,32 +737,36 @@
         :returns: True if information should be returned.
         :rtype: bool
         """
         return self._get_return_row()
 
     def set_durability(self, durability):
         """
-        On-premise only. Sets the durability to use for the operation.
+        Sets the durability to use for the operation.
+
+        On-premises only
 
         :param durability: the Durability to use
         :type durability: Durability
         :returns: self.
         :raises IllegalArgumentException: raises the exception if Durability
             is not valid
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         self._set_durability(durability)
         return self
 
     def get_durability(self):
         """
-        On-premise only. Gets the durability to use for the operation or
-        None if not set
+        Gets the durability to use for the operation or
+        None if not set.
+
+        On-premises only
         :returns: the Durability
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         return self._get_durability()
 
     def does_reads(self):
         return self._match_version is not None or self.get_return_row()
 
     def validate(self):
@@ -795,26 +818,26 @@
             not a string.
         """
         super(GetIndexesRequest, self).set_table_name(table_name)
         return self
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -949,24 +972,24 @@
         :returns: the key.
         :rtype: dict
         """
         return self._key
 
     def set_namespace(self, namespace):
         """
-        On-premises only
-
         Sets the namespace to use for the operation. This will override
         any configured default value.
 
+        On-premises only
+
         :param namespace: the namespace
         :type namespace: str
         :raises IllegalArgumentException: raises the exception if namespace is
             not a string.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         super(GetRequest, self).set_namespace(namespace)
         return self
 
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the operation. This is a required
@@ -979,26 +1002,26 @@
             not a string.
         """
         super(GetRequest, self).set_table_name(table_name)
         return self
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -1094,24 +1117,24 @@
         self._operation_id = None
 
     def __str__(self):
         return 'GetTableRequest'
 
     def set_namespace(self, namespace):
         """
-        On-premises only
-
         Sets the namespace to use for the operation. This will override
         any configured default value.
 
+        On-premises only
+
         :param namespace: the namespace
         :type namespace: str
         :raises IllegalArgumentException: raises the exception if namespace is
             not a string.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         super(GetTableRequest, self).set_namespace(namespace)
         return self
 
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the request.
@@ -1123,26 +1146,26 @@
             not a string.
         """
         super(GetTableRequest, self).set_table_name(table_name)
         return self
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -1249,26 +1272,26 @@
         self._namespace = None
 
     def __str__(self):
         return 'ListTablesRequest'
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -1329,36 +1352,36 @@
         :returns: the maximum number of tables to return in a single request.
         :rtype: int
         """
         return self._limit
 
     def set_namespace(self, namespace):
         """
-        On-premise only.
-
         Sets the namespace to use for the list. If not set, all tables
         accessible to the user will be returned. If set, only tables in the
         namespace provided are returned.
 
+        On-premise only.
+
         :param namespace: the namespace to use.
         :type namespace: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if namespace is
             not a string.
         """
         CheckValue.check_str(namespace, 'namespace')
         self._namespace = namespace
         return self
 
     def get_namespace(self):
         """
-        On-premise only.
-
         Returns the namespace to use for the list or None if not set.
 
+        On-premise only.
+
         :returns: the namespace.
         :rtype: str
         """
         return self._namespace
 
     def set_timeout(self, timeout_ms):
         """
@@ -1442,24 +1465,24 @@
         self._durability = None
 
     def __str__(self):
         return 'MultiDeleteRequest'
 
     def set_namespace(self, namespace):
         """
-        On-premises only
-
         Sets the namespace to use for the operation. This will override
         any configured default value.
 
+        On-premises only
+
         :param namespace: the namespace
         :type namespace: str
         :raises IllegalArgumentException: raises the exception if namespace is
             not a string.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         super(MultiDeleteRequest, self).set_namespace(namespace)
         return self
 
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the operation. This is a required
@@ -1496,26 +1519,26 @@
         :returns: the key.
         :rtype: dict
         """
         return self._key
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -1629,39 +1652,43 @@
         :returns: the timeout value.
         :rtype: int
         """
         return super(MultiDeleteRequest, self).get_timeout()
 
     def set_durability(self, durability):
         """
-        On-premise only. Sets the durability to use for the operation.
+        Sets the durability to use for the operation.
+
+        On-premises only
 
         :param durability: the Durability to use
         :type durability: Durability
         :returns: self.
         :raises IllegalArgumentException: raises the exception if Durability
             is not valid
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         if durability is None:
             self._durability = None
             return
         if not isinstance(durability, Durability):
             raise IllegalArgumentException('set_durability requires an ' +
                                            'instance of Durability as parameter.')
         durability.validate()
         self._durability = durability
         return self
 
     def get_durability(self):
         """
-        On-premise only. Gets the durability to use for the operation or
-        None if not set
+        Gets the durability to use for the operation or None if not set
+
+        On-premises only
+
         :returns: the Durability
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         return self._durability
 
     def does_reads(self):
         return True
 
     def does_writes(self):
@@ -1707,30 +1734,37 @@
     """
 
     def __init__(self):
         super(PrepareRequest, self).__init__()
         self._statement = None
         self._get_query_plan = False
         self._get_query_schema = False
+        self._query_version = 0
 
     def __str__(self):
         return 'PrepareRequest'
 
+    def set_query_version(self, version):
+        self._query_version = version
+
+    def get_query_version(self):
+        return self._query_version
+
     def set_namespace(self, namespace):
         """
-        On-premises only
-
         Sets the namespace to use for the operation. This will override
         any configured default value.
 
+        On-premises only
+
         :param namespace: the namespace
         :type namespace: str
         :raises IllegalArgumentException: raises the exception if namespace is
             not a string.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         super(PrepareRequest, self).set_namespace(namespace)
         return self
 
     def set_table_name(self, table_name):
         """
         Sets the table name for a query operation. This is used by rate limiting
@@ -1766,26 +1800,26 @@
         :returns: the statement, or None if it has not been set.
         :rtype: str
         """
         return self._statement
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -1829,29 +1863,29 @@
 
         :param: get_query_schema: True if a JSON representation of the schema
         of the query should be included in the :py:class:`PreparedStatement`.
         :type get_query_schema: bool
         :returns: self.
         :raises IllegalArgumentException: raises the exception if get_query_schema
             is not a boolean.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         CheckValue.check_boolean(get_query_schema, 'get_query_schema')
         self._get_query_schema = get_query_schema
         return self
 
     def get_query_schema(self):
         """
         Returns whether a JSON representation of the schema of the query should
         be included in the :py:class:`PreparedStatement`.
 
         :returns: True if a JSON representation of the schema
         of the query should be included in the :py:class:`PreparedStatement`.
         :rtype: bool
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._get_query_schema
 
     def set_timeout(self, timeout_ms):
         """
         Sets the request timeout value, in milliseconds. This overrides any
         default value set in :py:class:`NoSQLHandleConfig`. The value must be
@@ -1976,26 +2010,26 @@
         :returns: the value, or None if not set.
         :rtype: dict
         """
         return self._value
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -2201,24 +2235,24 @@
         :returns: the timeout value.
         :rtype: int
         """
         return super(PutRequest, self).get_timeout()
 
     def set_namespace(self, namespace):
         """
-        On-premises only
-
         Sets the namespace to use for the operation. This will override
         any configured default value.
 
+        On-premises only
+
         :param namespace: the namespace
         :type namespace: str
         :raises IllegalArgumentException: raises the exception if namespace is
             not a string.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         super(PutRequest, self).set_namespace(namespace)
         return self
 
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the operation.
@@ -2259,32 +2293,36 @@
         :returns: True if information should be returned.
         :rtype: bool
         """
         return self._get_return_row()
 
     def set_durability(self, durability):
         """
-        On-premise only. Sets the durability to use for the operation.
+        Sets the durability to use for the operation.
+
+        On-premises only
 
         :param durability: the Durability to use
         :type durability: Durability
         :returns: self.
         :raises IllegalArgumentException: raises the exception if Durability
             is not valid
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         self._set_durability(durability)
         return self
 
     def get_durability(self):
         """
-        On-premise only. Gets the durability to use for the operation or
-        None if not set
+        Gets the durability to use for the operation or None if not set
+
+        On-premises only
+
         :returns: the Durability
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         return self._get_durability()
 
     def does_reads(self):
         return self._option is not None or self.get_return_row()
 
     def validate(self):
@@ -2391,68 +2429,70 @@
         # sorting.
         self._shard_id = -1
         # The QueryDriver, for advanced queries only.
         self.driver = None
         # An "internal" request is one created and submitted for execution by
         # the ReceiveIter.
         self.is_internal = False
+        # test mode used for query testing
+        self._in_test_mode = False
+        # new with elasticity changes
+        self._query_version = 0
+        self._query_name = None
+        self._virtual_scan = None # a dict if set
+        self._log_file_tracing = False
+        self._driver_query_trace = None
+        self._server_query_traces = None # dict if set
+        self._batch_counter = 0
 
     def __str__(self):
         return 'QueryRequest'
 
     def copy_internal(self):
         # Creates an internal QueryRequest out of the application-provided
         # request.
         internal_req = QueryRequest()
         internal_req.set_compartment(self.get_compartment())
         internal_req.set_table_name(self.get_table_name())
-        internal_req.set_timeout(self.get_timeout())
+        # avoid check on timeout value
+        internal_req._timeout_ms = self._timeout_ms
         internal_req.set_trace_level(self._trace_level)
         internal_req.set_limit(self._limit)
         internal_req.set_max_read_kb(self._max_read_kb)
         internal_req.set_max_write_kb(self._max_write_kb)
         internal_req.set_max_memory_consumption(self._max_memory_consumption)
         internal_req.set_math_context(self._math_context)
-        internal_req.set_consistency(self._consistency)
+        internal_req._consistency = self._consistency
         internal_req.set_durability(self._durability)
-        internal_req.set_prepared_statement(self._prepared_statement)
+        internal_req._prepared_statement = self._prepared_statement
+        internal_req.set_query_version(self._query_version)
         internal_req.driver = self.driver
         internal_req.is_internal = True
+        # new with elasticity
+        internal_req._log_file_tracing = self._log_file_tracing
+        internal_req._query_name = self._query_name
+        internal_req._batch_counter = self._batch_counter
+        internal_req._driver_query_trace = self._driver_query_trace
+        internal_req._topo_seq_num = self._topo_seq_num
+        internal_req._in_test_mode = self._in_test_mode
         return internal_req
 
     def copy(self):
         """
         Copies the query request to start query results from the beginning.
 
-        :versionadded: 5.3.6
+        :versionadded:: 5.3.6
         """
-        copy = QueryRequest()
-        copy._compartment = self.get_compartment()
-        copy._prepared_statement = self.get_table_name()
-        timeout = self.get_timeout()
-        if timeout > 0:
-            copy.set_timeout(timeout)
-        copy.set_trace_level(self._trace_level)
-        copy.set_limit(self._limit)
-        copy.set_max_read_kb(self._max_read_kb)
-        copy.set_max_write_kb(self._max_write_kb)
-        copy.set_max_memory_consumption(self._max_memory_consumption)
-        copy.set_math_context(self._math_context)
-        if self._consistency is not None:
-            copy.set_consistency(self._consistency)
-        if self._durability is not None:
-            copy.set_durability(self._durability)
-        if self._prepared_statement is not None:
-            copy.set_prepared_statement(self._prepared_statement)
+        copy = self.copy_internal()
         copy._statement = self._statement
-        # leave continuationKey null to start from the beginning
-        # copy._continuation_key = self._continuation_key
-        self.is_internal = False
-        self._shard_id = -1
-        self.driver = None
+        copy.is_internal = False
+        copy.driver = None
+        copy.shard_id = -1
+        self._driver_query_trace = None
+        self._batch_counter = 0
 
         return copy
 
     def close(self):
         """
         Terminates the query execution and releases any memory consumed by the
         query at the driver. An application should use this method if it wishes
@@ -2466,33 +2506,70 @@
         query results to be generated. Otherwise False.
 
         :returns: Whether the query execution is finished or not.
         :rtype: bool
         """
         return self._continuation_key is None
 
+    def incr_batch_counter(self):
+        self._batch_counter += 1
+
+    def get_batch_counter(self):
+        return self._batch_counter
+
+    def set_query_version(self, version):
+        self._query_version = version
+        return self
+
+    def get_query_name(self):
+        return self._query_name
+
+    def get_query_version(self):
+        return self._query_version
+
+    def set_virtual_scan(self, vs):
+        self._virtual_scan = vs
+        return self
+
+    def get_virtual_scan(self):
+        self._virtual_scan
+
     def get_table_name(self):
         if self._prepared_statement is None:
             return None
         return self._prepared_statement.get_table_name()
 
+    def set_query_traces(self, traces):
+        self._server_query_traces = traces
+        return self
+
+    def get_query_traces(self):
+        return self._server_query_traces
+
+    def set_log_file_tracing(self, value):
+        self._log_file_tracing = value
+        return self
+
+    def get_log_file_tracing(self):
+        return self._log_file_tracing
+
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -2507,14 +2584,20 @@
             raise IllegalArgumentException('trace level must be <= 32')
         self._trace_level = trace_level
         return self
 
     def get_trace_level(self):
         return self._trace_level
 
+    def set_in_test_mode(self, value):
+        self._in_test_mode = value
+
+    def get_in_test_mode(self):
+        return self._in_test_mode
+
     def set_limit(self, limit):
         """
         Sets the limit on number of items returned by the operation. This allows
         an operation to return less than the default amount of data.
 
         :param limit: the limit in terms of number of items returned.
         :type limit: int
@@ -2682,33 +2765,37 @@
         :returns: the consistency
         :rtype: Consistency
         """
         return self._consistency
 
     def set_durability(self, durability):
         """
-        On-premise only. Sets the durability to use for the operation. Only
+        Sets the durability to use for the operation. Only
         used for queries that do writes or deletes.
 
+        On-premises only
+
         :param durability: the Durability to use
         :type durability: Durability
         :returns: self.
         :raises IllegalArgumentException: raises the exception if Durability
             is not valid
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         self._durability = durability
         return self
 
     def get_durability(self):
         """
-        On-premise only. Gets the durability to use for the operation or
-        None if not set
+        Gets the durability to use for the operation or None if not set
+
+        On-premises only
+
         :returns: the Durability
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._durability
 
     @deprecated
     def set_continuation_key(self, continuation_key):
         """
         Sets the continuation key. This is used to continue an operation that
@@ -2882,18 +2969,14 @@
     def is_simple_query(self):
         return self._prepared_statement.is_simple_query()
 
     def topology_info(self):
         return (None if self._prepared_statement is None else
                 self._prepared_statement.topology_info())
 
-    def topology_seq_num(self):
-        return (-1 if self._prepared_statement is None else
-                self._prepared_statement.topology_seq_num())
-
     def validate(self):
         if self._statement is None and self._prepared_statement is None:
             raise IllegalArgumentException(
                 'Either statement or prepared statement should be set.')
 
     @staticmethod
     def get_serial_version(serial_version):
@@ -2908,17 +2991,17 @@
     def get_request_name(self):
         # type: () -> str
         return "Query"
 
 
 class SystemRequest(Request):
     """
-    On-premise only.
+    On-premises only.
 
-    SystemRequest is an on-premise-only request used to perform any
+    SystemRequest is an on-premises only request used to perform any
     table-independent administrative operation such as create/drop of namespaces
     and security-relevant operations (create/drop users and roles). These
     operations are asynchronous and completion needs to be checked.
 
     Examples of statements used in this object include:
 
         CREATE NAMESPACE mynamespace\n
@@ -3015,17 +3098,17 @@
     def get_request_name(self):
         # type: () -> str
         return "System"
 
 
 class SystemStatusRequest(Request):
     """
-    On-premise only.
+    On-premises only.
 
-    SystemStatusRequest is an on-premise-only request used to check the status
+    SystemStatusRequest is an on-premises only request used to check the status
     of an operation started using a :py:class:`SystemRequest`.
     """
 
     def __init__(self):
         super(SystemStatusRequest, self).__init__()
         self._statement = None
         self._operation_id = None
@@ -3205,47 +3288,47 @@
         :returns: the statement.
         :rtype: str
         """
         return self._statement
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
             is not a str.
         """
         self.set_compartment_internal(compartment)
         return self
 
     def set_table_limits(self, table_limits):
         """
-        Cloud service only.
-
         Sets the table limits to use for the operation. Limits are used in only
         2 cases -- table creation statements and limits modification operations.
         It is not used for other DDL operations.
 
-        If limits are set for an on-premise service they are silently ignored.
+        If limits are set for an on-premises service they are silently ignored.
+
+        Cloud service only.
 
         :param table_limits: the limits.
         :type table_limits: TableLimits
         :returns: self.
         :raises IllegalArgumentException: raises the exception if table_limits
             is not an instance TableLimits.
         """
@@ -3263,96 +3346,98 @@
         :returns: the limits.
         :rtype: TableLimits
         """
         return self._limits
 
     def set_defined_tags(self, tags):
         """
-        Cloud service only.
-
         Sets defined tags
 
+        Cloud service only.
+
         :param tags the tags
-        :type tags: dict(str, dict(str, object))
-        :versionadded: 5.4.0
+        :type tags: dict[str, dict[str, object]]
+        :versionadded:: 5.4.0
         """
         self._defined_tags = tags
 
     def get_defined_tags(self):
         """
-        Cloud service only.
-
         Returns the defined tags or None if not set
 
+        Cloud service only.
+
         :returns: the defined tags.
-        :rtype: dict(str, dict(str, object))
-        :versionadded: 5.4.0
+        :rtype: dict[str, dict[str, object]]
+        :versionadded:: 5.4.0
         """
         return self._defined_tags
 
     def set_free_form_tags(self, tags):
         """
-        Cloud service only.
-
         Sets free_form tags
 
+        Cloud service only.
+
         :param tags the tags
-        :type tags: dict(str, str)
-        :versionadded: 5.4.0
+        :type tags: dict[str, str]
+        :versionadded:: 5.4.0
         """
         self._free_form_tags = tags
 
     def get_free_form_tags(self):
         """
         Returns the free_form tags or None if not set
 
         :returns: the free_form tags.
-        :rtype: dict(str, str)
-        :versionadded: 5.4.0
+        :rtype: dict[str, str]
+        :versionadded:: 5.4.0
         """
         return self._free_form_tags
 
     def set_match_etag(self, etag):
         """
-        Cloud service only.
-
         Sets a ETag to match for the operation to proceed. The ETag must be
         non-null and have been previously returned in :py:class:`TableResult`.
         The ETag is a form of optimistic concurrency control allowing an
         application to ensure no unexpected modifications have been made to the
         table.
 
+        Cloud service only.
+
         :param etag the tag
         :type etag: str
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         self._match_etag = etag
 
     def get_match_etag(self):
         """
+        Returns the match etag or None if not set
+
         Cloud service only.
 
         :returns: the match etag or None if not set
         :rtype: str
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._match_etag
 
     def set_namespace(self, namespace):
         """
-        On-premises only
-
         Sets the namespace to use for the operation. This will override
         any configured default value.
 
+        On-premises only
+
         :param namespace: the namespace
         :type namespace: str
         :raises IllegalArgumentException: raises the exception if namespace is
             not a string.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         super(TableRequest, self).set_namespace(namespace)
         return self
 
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the operation. The table name is only
@@ -3463,24 +3548,24 @@
         self._start_time = 0
         self._end_time = 0
         self._limit = 0
         self._start_index = 0
 
     def set_namespace(self, namespace):
         """
-        On-premises only
-
         Sets the namespace to use for the operation. This will override
         any configured default value.
 
+        On-premises only
+
         :param namespace: the namespace
         :type namespace: str
         :raises IllegalArgumentException: raises the exception if namespace is
             not a string.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         super(TableUsageRequest, self).set_namespace(namespace)
         return self
 
     def set_table_name(self, table_name):
         """
         Sets the table name to use for the request. This is a required
@@ -3493,26 +3578,26 @@
             not a string.
         """
         super(TableUsageRequest, self).set_table_name(table_name)
         return self
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -3642,27 +3727,27 @@
         previous request and can be used to page usage records. If not set
         the list starts a 0
         :param start_index: the numeric index.
         :type start_index: int
         :returns: self.
         :raises IllegalArgumentException: raises the exception if start_index
         is a negative number.
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         CheckValue.check_int_ge_zero(start_index, 'start_index')
         self._start_index = start_index
         return self
 
     def get_start_index(self):
         """
         Returns the start_index for usage records desired.
 
         :returns: the numeric start_index.
         :rtype: int
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._start_index
 
     def set_timeout(self, timeout_ms):
         """
         Sets the request timeout value, in milliseconds. This overrides any
         default value set in :py:class:`NoSQLHandleConfig`. The value must be
@@ -3776,17 +3861,17 @@
                 'DeleteRequest as parameter. Got: ' + str(request))
         CheckValue.check_boolean(abort_if_unsuccessful,
                                  'abort_if_unsuccessful')
         table_name = self.get_table_name()
         if table_name is None:
             self.set_table_name(request.get_table_name())
         else:
-            if WriteMultipleRequest.get_top_table_name(
-                    request.get_table_name().lower()) \
-                    != table_name.lower():
+            if (WriteMultipleRequest.get_top_table_name(
+                    request.get_table_name().lower())
+                    != table_name.lower()):
                 raise IllegalArgumentException(
                     'The parent table_name used for the operation is '
                     'different from that of others: ' + table_name)
         request.validate()
         self._ops.append(self.OperationRequest(request, abort_if_unsuccessful))
         return self
 
@@ -3804,26 +3889,26 @@
         for op in self._ops:
             if single_table_name.lower() != op.get_request().get_table_name().lower():
                 return False
         return True
 
     def set_compartment(self, compartment):
         """
-        Cloud service only.
-
         Sets the name or id of a compartment to be used for this operation.
 
         The compartment may be specified as either a name (or path for nested
         compartments) or as an id (OCID). A name (vs id) can only be used when
         authenticated using a specific user identity. It is *not* available if
         authenticated as an Instance Principal which can be done when calling
         the service from a compute instance in the Oracle Cloud Infrastructure.
         See
         :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
 
+        Cloud service only.
+
         :param compartment: the compartment name or id. If using a nested
             compartment, specify the full compartment path
             compartmentA.compartmentB, but exclude the name of the root
             compartment (tenant).
         :type compartment: str
         :returns: self.
         :raises IllegalArgumentException: raises the exception if compartment
@@ -3892,39 +3977,43 @@
         Removes all of the operations from the WriteMultiple request.
         """
         self.set_table_name(None)
         self._ops = list()
 
     def set_durability(self, durability):
         """
-        On-premise only. Sets the durability to use for the operation.
+        Sets the durability to use for the operation.
+
+        On-premises only
 
         :param durability: the Durability to use
         :type durability: Durability
         :returns: self.
         :raises IllegalArgumentException: raises the exception if Durability
             is not valid
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         if durability is None:
             self._durability = None
             return
         if not isinstance(durability, Durability):
             raise IllegalArgumentException('set_durability requires an ' +
                                            'instance of Durability as parameter.')
         durability.validate()
         self._durability = durability
         return self
 
     def get_durability(self):
         """
-        On-premise only. Gets the durability to use for the operation or
-        None if not set
+        Gets the durability to use for the operation or None if not set
+
+        On-premises only
+
         :returns: the Durability
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         return self._durability
 
     def does_reads(self):
         for op in self._ops:
             req = op.get_request()
             if req.does_reads():
@@ -3963,14 +4052,551 @@
             return self._abort_if_unsuccessful
 
     def get_request_name(self):
         # type: () -> str
         return "WriteMultiple"
 
 
+class AddReplicaRequest(Request):
+    """
+    Cloud service only
+
+    AddReplicaRequest is used to add a new replica (region) to a table
+    """
+
+    def __init__(self):
+        super(AddReplicaRequest, self).__init__()
+        self._replica_name = None
+        self._read_units = 0
+        self._write_units = 0
+        self._match_etag = None
+
+    def __str__(self):
+        return ('AddReplicaRequest: [name=' + str(self.get_table_name()) +
+                ', replica_name=' + str(self._replica_name) + ', read_units=' +
+                str(self._read_units) + ', write_units=' +
+                str(self._write_units) +
+                ', match_etag=' + str(self._match_etag) + ']')
+
+    def set_table_name(self, table_name):
+        """
+        Sets the table name to replicate.
+
+        :param table_name: the name of the table.
+        :type table_name: str
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if table_name is
+            not a string.
+        """
+        super(AddReplicaRequest, self).set_table_name(table_name)
+        return self
+
+    def set_replica_name(self, replica_name):
+        """
+        Sets the replica name(region) to be added.
+
+        :param replica_name: the name of the replica.
+        :type replica_name: str
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if replica_name
+            is not a string.
+        """
+        CheckValue.check_str(replica_name, 'statement')
+        self._replica_name = replica_name
+        return self
+
+    def get_replica_name(self):
+        """
+        Returns the replica name.
+
+        :returns: the replica name, or None if not set.
+        :returns: str
+        """
+        return self._replica_name
+
+    def set_read_units(self, read_units):
+        """
+        Sets the read units for the replica table. This defaults to the units
+        set on the existing table.
+
+        :param read_units: the read units to use, in read units.
+        :type read_units: int
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if read_units is
+            not a integer.
+        """
+        CheckValue.check_int(read_units, 'read_units')
+        self._read_units = read_units
+        return self
+
+    def get_read_units(self):
+        """
+        Returns the read units to use for the replica table. 0 if not set
+
+        :returns: the read units.
+        :rtype: int
+        """
+        return self._read_units
+
+    def set_write_units(self, write_units):
+        """
+        Sets the write units for the replica table. This defaults to the units
+        set on the existing table.
+
+        :param write_units: the write units to use, in write units.
+        :type write_units: int
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if write_units is
+            not a integer.
+        """
+        CheckValue.check_int(write_units, 'write_units')
+        self._write_units = write_units
+        return self
+
+    def get_write_units(self):
+        """
+        Returns the write units to use on the replica table. 0 if not set.
+
+        :returns: the write units.
+        :rtype: int
+        """
+        return self._write_units
+
+    def set_match_etag(self, etag):
+        """
+        Sets a ETag to match for the operation to proceed. The ETag must be
+        non-null and have been previously returned in :py:class:`TableResult`.
+        The ETag is a form of optimistic concurrency control allowing an
+        application to ensure no unexpected modifications have been made to the
+        table.
+
+        :param etag the tag
+        :type etag: str
+        """
+        self._match_etag = etag
+
+    def get_match_etag(self):
+        """
+        Gets the match etag or None if not set
+
+        :returns: the match etag or None if not set
+        :rtype: str
+        """
+        return self._match_etag
+
+    def set_compartment(self, compartment):
+        """
+        Sets the name or id of a compartment to be used for this operation.
+
+        The compartment may be specified as either a name (or path for nested
+        compartments) or as an id (OCID). A name (vs id) can only be used when
+        authenticated using a specific user identity. It is *not* available if
+        authenticated as an Instance Principal which can be done when calling
+        the service from a compute instance in the Oracle Cloud Infrastructure.
+        See
+        :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
+
+        :param compartment: the compartment name or id. If using a nested
+            compartment, specify the full compartment path
+            compartmentA.compartmentB, but exclude the name of the root
+            compartment (tenant).
+        :type compartment: str
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if compartment
+            is not a str.
+        """
+        self.set_compartment_internal(compartment)
+        return self
+
+    def set_timeout(self, timeout_ms):
+        """
+        Sets the request timeout value, in milliseconds. This overrides any
+        default value set in :py:class:`NoSQLHandleConfig`. The value must be
+        positive.
+
+        :param timeout_ms: the timeout value, in milliseconds.
+        :type timeout_ms: int
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if the timeout
+            value is less than or equal to 0.
+        """
+        self._set_timeout(timeout_ms)
+        return self
+
+    def set_defaults(self, cfg):
+        # Use the default request timeout if not set.
+        self._check_config(cfg)
+        if self.get_timeout() == 0:
+            self._set_timeout(cfg.get_default_table_request_timeout())
+        return self
+
+    def validate(self):
+        if self.get_table_name() is None or self._replica_name is None:
+            raise IllegalArgumentException(
+                'AddReplicaRequest requires a table name and replica name.')
+
+    def get_request_name(self):
+        # type: () -> str
+        return "AddReplica"
+
+    @staticmethod
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        return borneo.nson.AddReplicaRequestSerializer()
+        pass
+
+class DropReplicaRequest(Request):
+    """
+    Cloud service only
+
+    DropReplicaRequest is used to drop a replica (region) from a table
+    """
+
+    def __init__(self):
+        super(DropReplicaRequest, self).__init__()
+        self._replica_name = None
+        self._match_etag = None
+
+    def __str__(self):
+        return ('DropReplicaRequest: [name=' + str(self.get_table_name()) +
+                ', replica_name=' + str(self._replica_name) +
+                ', match_etag=' + str(self._match_etag) + ']')
+
+    def set_table_name(self, table_name):
+        """
+        Sets the table name to use for the operation.
+
+        :param table_name: the name of the table.
+        :type table_name: str
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if table_name is
+            not a string.
+        """
+        super(DropReplicaRequest, self).set_table_name(table_name)
+        return self
+
+    def set_replica_name(self, replica_name):
+        """
+        Sets the replica name(region) to be dropped.
+
+        :param replica_name: the name of the replica.
+        :type replica_name: str
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if replica_name
+            is not a string.
+        """
+        CheckValue.check_str(replica_name, 'statement')
+        self._replica_name = replica_name
+        return self
+
+    def get_replica_name(self):
+        """
+        Returns the replica name.
+
+        :returns: the replica name, or None if not set.
+        :returns: str
+        """
+        return self._replica_name
+
+    def set_match_etag(self, etag):
+        """
+        Sets a ETag to match for the operation to proceed. The ETag must be
+        non-null and have been previously returned in :py:class:`TableResult`.
+        The ETag is a form of optimistic concurrency control allowing an
+        application to ensure no unexpected modifications have been made to the
+        table.
+
+        :param etag the tag
+        :type etag: str
+        :returns: self
+        """
+        self._match_etag = etag
+        return self
+
+    def get_match_etag(self):
+        """
+        Gets the match etag or None if not set
+
+        :returns: the match etag or None if not set
+        :rtype: str
+        """
+        return self._match_etag
+
+    def set_compartment(self, compartment):
+        """
+        Sets the name or id of a compartment to be used for this operation.
+
+        The compartment may be specified as either a name (or path for nested
+        compartments) or as an id (OCID). A name (vs id) can only be used when
+        authenticated using a specific user identity. It is *not* available if
+        authenticated as an Instance Principal which can be done when calling
+        the service from a compute instance in the Oracle Cloud Infrastructure.
+        See
+        :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
+
+        :param compartment: the compartment name or id. If using a nested
+            compartment, specify the full compartment path
+            compartmentA.compartmentB, but exclude the name of the root
+            compartment (tenant).
+        :type compartment: str
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if compartment
+            is not a str.
+        """
+        self.set_compartment_internal(compartment)
+        return self
+
+    def set_timeout(self, timeout_ms):
+        """
+        Sets the request timeout value, in milliseconds. This overrides any
+        default value set in :py:class:`NoSQLHandleConfig`. The value must be
+        positive.
+
+        :param timeout_ms: the timeout value, in milliseconds.
+        :type timeout_ms: int
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if the timeout
+            value is less than or equal to 0.
+        """
+        self._set_timeout(timeout_ms)
+        return self
+
+    def set_defaults(self, cfg):
+        # Use the default request timeout if not set.
+        self._check_config(cfg)
+        if self.get_timeout() == 0:
+            self._set_timeout(cfg.get_default_table_request_timeout())
+        return self
+
+    def validate(self):
+        if self.get_table_name() is None or self._replica_name is None:
+            raise IllegalArgumentException(
+                'DropReplicaRequest requires a table name and replica name.')
+
+    def get_request_name(self):
+        # type: () -> str
+        return "DropReplica"
+
+    @staticmethod
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        return borneo.nson.DropReplicaRequestSerializer()
+        pass
+
+class ReplicaStatsRequest(Request):
+    """
+    Cloud service only
+
+    Represents the argument of a :py:meth:`NoSQLHandle.get_replica_stats`.
+    operation which returns stats information for one, or all replicas of
+    a replicated table, returned in :py:class:`ReplicaStatsResult`.
+    This information includes a time series of replica stats, as found in
+    :py:class:`ReplicaStatsResult.ReplicaStats`.
+
+    It is possible to return a range of stats records or, by default, only the
+    most recent stats records if start_time is not specified. Replica stats
+    records are created on a regular basis and maintained for a period of time.
+    Only records for time periods that have completed are returned so that a
+    user never sees changing data for a specific range.
+    """
+
+    def __init__(self):
+        super(ReplicaStatsRequest, self).__init__()
+        self._replica_name = None
+        self._start_time = 0
+        self._limit = 0
+
+    def __str__(self):
+        return ('ReplicaStatsRequest: [name=' + str(self.get_table_name()) +
+                ', replica_name=' + str(self._replica_name) +
+                ', start_time=' + str(self._start_time) +
+                ', limit=' + str(self._limit) + ']')
+
+    def set_table_name(self, table_name):
+        """
+        Sets the table name to use for the operation.
+
+        :param table_name: the name of the table.
+        :type table_name: str
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if table_name is
+            not a string.
+        """
+        super(ReplicaStatsRequest, self).set_table_name(table_name)
+        return self
+
+    def set_replica_name(self, replica_name):
+        """
+        Sets the replica name(region) to be used to query for stats
+        information. If not set information for all replicas is returned.
+
+        :param replica_name: the name of the replica.
+        :type replica_name: str
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if replica_name
+            is not a string.
+        """
+        CheckValue.check_str(replica_name, 'statement')
+        self._replica_name = replica_name
+        return self
+
+    def get_replica_name(self):
+        """
+        Returns the replica name.
+
+        :returns: the replica name, or None if not set.
+        :returns: str
+        """
+        return self._replica_name
+
+    def set_start_time(self, start_time):
+        """
+        Sets the start time to use for the request in milliseconds since the
+        Epoch in UTC time. If no start time is set for this request the most
+        recent complete stats records are returned, the number of records is
+        up to limit set by :py:meth:`ReplicaStatsRequest.set_limit`
+
+        :param start_time the start_time
+        :type start_time: int
+        :returns: self.
+        """
+        self._start_time = start_time
+        return self
+
+    def set_start_time_str(self, start_time):
+        """
+        Sets the start time to use for the request from an ISO 8601 formatted
+        string. If timzone is not specified UTC is used.
+
+        :param start_time the start_time
+        :type start_time: str
+        :returns: self
+        :raises IllegalArgumentException: raises the exception if the
+            start_time string is not a valid format.
+        """
+        self._check_time(start_time)
+        self._start_time = SerdeUtil.iso_time_to_ms(start_time)
+        return self
+
+    def get_start_time(self):
+        """
+        Get the start time to use for the request in milliseconds since
+        the epoch in UTC time
+
+        :returns: the start_time
+        :rtype: int
+        """
+        return self._start_time
+
+    def get_start_time_str(self):
+        """
+        Get the start time to use for the request as an ISO 8601 formatted
+        string. If the start_time is not set, None is returned
+
+        :returns: the start_time or None
+        :rtype: str
+        """
+        if self._start_time == 0:
+            return None
+        return datetime.fromtimestamp(
+            float(self._start_time) / 1000).replace(tzinfo=tz.UTC).isoformat()
+
+    def set_limit(self, limit):
+        """
+        Sets the limit to the number of replica stats records returned per
+        replica (region). The default value is 1000.
+
+        :param: limit the limit
+        :type limit: int
+        :returns: self
+        """
+        CheckValue.check_int_ge_zero(limit, 'limit')
+        self._limit = limit
+        return self
+
+    def get_limit(self):
+        """
+        Gets the limit to the number of replica stats records returned per
+        replica (region). Returns 0 if not set.
+
+        :returns: the limit
+        :rtype: int
+        """
+        return self._limit
+
+    def set_compartment(self, compartment):
+        """
+        Sets the name or id of a compartment to be used for this operation.
+
+        The compartment may be specified as either a name (or path for nested
+        compartments) or as an id (OCID). A name (vs id) can only be used when
+        authenticated using a specific user identity. It is *not* available if
+        authenticated as an Instance Principal which can be done when calling
+        the service from a compute instance in the Oracle Cloud Infrastructure.
+        See
+        :py:meth:`borneo.iam.SignatureProvider.create_with_instance_principal`.
+
+        :param compartment: the compartment name or id. If using a nested
+            compartment, specify the full compartment path
+            compartmentA.compartmentB, but exclude the name of the root
+            compartment (tenant).
+        :type compartment: str
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if compartment
+            is not a str.
+        """
+        self.set_compartment_internal(compartment)
+        return self
+
+    def set_timeout(self, timeout_ms):
+        """
+        Sets the request timeout value, in milliseconds. This overrides any
+        default value set in :py:class:`NoSQLHandleConfig`. The value must be
+        positive.
+
+        :param timeout_ms: the timeout value, in milliseconds.
+        :type timeout_ms: int
+        :returns: self.
+        :raises IllegalArgumentException: raises the exception if the timeout
+            value is less than or equal to 0.
+        """
+        self._set_timeout(timeout_ms)
+        return self
+
+    def set_defaults(self, cfg):
+        # Use the default request timeout if not set.
+        self._check_config(cfg)
+        if self.get_timeout() == 0:
+            self._set_timeout(cfg.get_default_table_request_timeout())
+        return self
+
+    def validate(self):
+        if self.get_table_name() is None:
+            raise IllegalArgumentException(
+                'ReplicaStatsRequest requires a table name.')
+
+    def get_request_name(self):
+        # type: () -> str
+        return "ReplicaStatsRequest"
+
+    @staticmethod
+    def get_serial_version(serial_version):
+        return serial_version
+
+    @staticmethod
+    def create_serializer(serial_version):
+        return borneo.nson.ReplicaStatsRequestSerializer()
+        pass
+
 class Result(object):
     """
     Result is a base class for result classes for all supported operations.
     All state and methods are maintained by extending classes.
     """
 
     def __init__(self):
@@ -3980,14 +4606,15 @@
         """
         self._rate_limit_delayed_ms = 0
         self._read_kb = 0
         self._read_units = 0
         self._retry_stats = None
         self._write_kb = 0
         self._write_units = 0
+        self._topology_info = None
 
     def get_rate_limit_delayed_ms(self):
         """
         Get the time the operation was delayed due to rate limiting. Cloud only.
         If rate limiting is in place, this value will represent the number of
         milliseconds that the operation was delayed due to rate limiting. If the
         value is zero, rate limiting did not apply or the operation did not need
@@ -4006,14 +4633,17 @@
         Returns a stats object with information about retries.
 
         :returns: stats object with retry information, or None if no retries
             were performed.
         """
         return self._retry_stats
 
+    def get_topology_info(self):
+        return self._topology_info
+
     def get_write_units(self):
         # Internal use only.
         return self._write_kb
 
     def set_rate_limit_delayed_ms(self, delay_ms):
         """
         :param delay_ms: the delay in milliseconds.
@@ -4036,14 +4666,20 @@
         Internal use only.
 
         :param retry_stats: the stats object to use.
         :type retry_stats: RetryStats
         """
         self._retry_stats = retry_stats
 
+    def set_topology_info(self, proxy_topo_seqnum, shard_ids):
+        self._topology_info = TopologyInfo(proxy_topo_seqnum, shard_ids)
+
+    def set_topology_info_object(self, info):
+        self._topology_info = info
+
     def set_write_kb(self, write_kb):
         self._write_kb = write_kb
         return self
 
     def set_write_units(self, write_units):
         # type: (int) -> Result
         self._write_units = write_units
@@ -4152,15 +4788,15 @@
         available if the target row exists and the operation failed because of a
         :py:class:`Version` mismatch and the corresponding
         :py:class:`DeleteRequest` the method
         :py:meth:`DeleteRequest.set_return_row` was called with a True value.
 
         :returns: the modification time in milliseconds since January 1, 1970
         :rtype: int
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         return self._get_existing_modification_time()
 
     def get_read_kb(self):
         """
         Returns the read throughput consumed by this operation, in KBytes. This
         is the actual amount of data read by the operation. The number of read
@@ -4398,15 +5034,15 @@
         """
         Returns the index of the last table name returned. This can be provided
         to :py:class:`ListTablesRequest` to be used as a starting point for
         listing tables.
 
         :returns: the index.
         :rtype: int
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._last_index_returned
 
 
 class MultiDeleteResult(Result):
     """
     Represents the result of a :py:meth:`NoSQLHandle.multi_delete` operation.
@@ -4642,15 +5278,15 @@
         available if the conditional put operation failed and the request
         specified that return information be returned using
         :py:meth:`PutRequest.set_return_row`. A value of -1 indicates this
         feature is not available at the connected server.
 
         :returns: the modification time in milliseconds since January 1, 1970
         :rtype: int
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         return self._get_existing_modification_time()
 
     def get_read_kb(self):
         """
         Returns the read throughput consumed by this operation, in KBytes.
         This is the actual amount of data read by the operation. The number of
@@ -4749,28 +5385,42 @@
         # self._continuation_keys fields store the partition id, the number of
         # results, and the continuation key per partition. Finally, the
         # self._is_in_phase1 specifies whether phase 1 is done.
         self._is_in_phase1 = False
         self._num_results_per_pid = None
         self._continuation_keys = None
         self._pids = None
+        self._virtual_scans = None
+        self._query_traces = None
 
     def __str__(self):
         self._compute()
         if self._results is None:
             return None
         res = 'Number of query results: ' + str(len(self._results))
         for result in self._results:
             res += '\n' + str(result)
         return res + '\n'
 
     def set_results(self, results):
         self._results = results
         return self
 
+    def get_virtual_scans(self):
+        return self._virtual_scans
+
+    def set_virtual_scans(self, vscans):
+        self._virtual_scans = vscans
+
+    def get_query_traces(self):
+        return self._query_traces
+
+    def set_query_traces(self, traces):
+        self._query_traces = traces
+
     def get_results(self):
         """
         Returns a list of results for the query. It is possible to have an empty
         list and a non-none continuation key.
 
         :returns: a list of results for the query.
         :rtype: list(dict)
@@ -4932,15 +5582,15 @@
     dictionary. INSERT queries with no RETURNING clause return a dictionary
     indicating the number of rows inserted, for example {'NumRowsInserted': 5}.
     UPDATE queries with no RETURNING clause return a dictionary indicating the
     number of rows updated, for example {'NumRowsUpdated': 3}. DELETE queries
     with no RETURNING clause return a dictionary indicating the number of rows
     deleted, for example {'numRowsDeleted': 2}.
 
-    :versionadded: 5.3.6
+    :versionadded:: 5.3.6
     """
 
     def __init__(self, request, handle):
         # NoSQLHandle handle
         super(QueryIterableResult, self).__init__()
         self.request = request
         self.handle = handle
@@ -4994,15 +5644,15 @@
         return QueryIterator(self)
 
 
 class QueryIterator:
     """
     QueryIterator iterates over all results of a query.
 
-    :versionadded: 5.3.6
+    :versionadded:: 5.3.6
     """
 
     def __init__(self, iterable):
         self._iterable = iterable
         self._internalRequest = iterable.request.copy()
         self._internal_result = None
         self._partialResultList = None
@@ -5010,16 +5660,16 @@
         self._next = None
         self._closed = False
 
     def _compute(self):
         if self._closed:
             return
         if self._partialResultList is None:
-            self._internal_result = \
-                self._iterable.handle.query(self._internalRequest)
+            self._internal_result = (
+                self._iterable.handle.query(self._internalRequest))
             self._partialResultList = self._internal_result.get_results()
             self._partialResultIter = self._partialResultList.__iter__()
             try:
                 self._next = next(self._partialResultIter)
                 return
             except StopIteration:
                 has_next = False
@@ -5028,16 +5678,16 @@
             try:
                 self._next = next(self._partialResultIter)
                 return
             except StopIteration:
                 has_next = False
 
         while not has_next and not self._internalRequest.is_done():
-            self._internal_result = \
-                self._iterable.handle.query(self._internalRequest)
+            self._internal_result = (
+                self._iterable.handle.query(self._internalRequest))
             self._partialResultList = self._internal_result.get_results()
             self._partialResultIter = self._partialResultList.__iter__()
             has_next = True
             try:
                 self._next = next(self._partialResultIter)
             except StopIteration:
                 has_next = False
@@ -5268,14 +5918,17 @@
         self._schema = None
         self._operation_id = None
         self._ocid = None
         self._ddl = None
         self._defined_tags = None  # dict(str, dict(str, object))
         self._match_etag = None  # str
         self._free_form_tags = None  # dict(str, str)
+        self._schema_frozen = False
+        self._local_replica_initialized = False
+        self._replicas = None
 
     def __str__(self):
         tres = ('table name=' + str(self._table_name) + ', state=' +
                 self._state)
         if self._limits is not None:
             tres += ', limits=' + str(self._limits)
 
@@ -5283,43 +5936,121 @@
         if self._ddl is not None:
             tres += ', ddl=' + str(self._ddl)
         elif self._schema is not None:
             tres += ', schema=[' + str(self._schema) + ']'
 
         if self._ocid is not None:
             tres += ', ocid=' + str(self._ocid)
+
+        # TODO: add tags and GAT state
         return tres
 
     def set_compartment_id(self, compartment_id):
         # Internal use only.
         self._compartment_or_namespace = compartment_id
         return self
 
     def set_namespace(self, namespace):
         # Internal use only.
         self._compartment_or_namespace = namespace
         return self
 
-    def get_compartment_id(self):
+    def set_schema_frozen(self, frozen):
+        # Internal use only.
+        self._schema_frozen = frozen
+        return self
+
+    def set_local_replica_initialized(self, replica_initialized):
+        # Internal use only.
+        self._local_replica_initialized = replica_initialized
+        return self
+
+    def set_replicas(self, replicas):
+        # Internal use only.
+        self._replicas = replicas
+        return self
+
+    def get_compartment(self):
         """
+        Returns compartment id of the target table.
+
         Cloud service only.
 
+        :returns: compartment id.
+        :rtype: str
+        """
+        return self._compartment_or_namespace
+
+    def get_compartment_id(self):
+        """
         Returns compartment id of the target table.
 
+        Cloud service only.
+
         :returns: compartment id.
         :rtype: str
         """
         return self._compartment_or_namespace
 
-    def get_namespace(self):
+    def is_schema_frozen(self):
+        """
+        Returns True if the schema for this table is frozen.
+
+        Cloud service only.
+
+        :returns: frozen state
+        :rtype: bool
+        :versionadded:: 5.4.2
         """
-        On-premise service only.
+        return self._schema_frozen
 
+    def is_local_replica_initialized(self):
+        """
+        Returns True if the table is a replica and its initialization
+        process has been completed, otherwise False
+
+        Cloud service only.
+
+        :returns: True if is an initialized replica
+        :rtype: bool
+        :versionadded:: 5.4.2
+        """
+        return self._local_replica_initialized
+
+    def is_replicated(self):
+        """
+        Returns True if the table is replicated
+
+        Cloud service only.
+
+        :returns: True if table is replicated
+        :rtype: bool
+        :versionadded:: 5.4.2
+        """
+        return self._replicas is not None
+
+    def get_replicas(self):
+        """
+        Returns a list of :py:class:`Replica` if the table is replicated,
+        otherwise None
+
+        Cloud service only.
+
+        :returns: list of replicas or None
+        :rtype: list[:py:class:`Replica`]
+        :versionadded:: 5.4.2
+        """
+        return self._replicas
+
+    def get_namespace(self):
+        """
         Returns the namespace of the table or null if it is not in a namespace.
 
+        On-premises only.
+
         :returns: namespace
         :rtype: str
         """
         return self._compartment_or_namespace
 
     def set_table_name(self, table_name):
         self._table_name = table_name
@@ -5351,15 +6082,15 @@
     def set_table_limits(self, limits):
         self._limits = limits
         return self
 
     def get_table_limits(self):
         """
         Returns the throughput and capacity limits for the table. Limits from an
-        on-premise service will always be None.
+        on-premises service will always be None.
 
         :returns: the limits.
         :rtype: TableLimits
         """
         return self._limits
 
     def set_schema(self, schema):
@@ -5398,57 +6129,64 @@
         statement is also altered to reflect the current table schema. This
         value, when non-null, is functionally equivalent to the schema
         returned by :py:meth:`set_schema`.
         table.
 
         :returns: the ddl statement used to create the table
         :rtype: str
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._ddl
 
     def get_table_id(self):
         """
-        Cloud service only.
         Returns the OCID of the table. This value will be null if used with the
-        on-premise service.
+        on-premises service.
+
+        Cloud service only.
 
         :returns: the table OCID
         :rtype: str
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._ocid
 
     def get_match_etag(self):
         """
+        Returns the match etag
+
         Cloud service only.
 
         :returns: the tag
         :rtype: str
-        :versionadded: 5.4.0
+        :versionadded:: 5.4.0
         """
         return self._match_etag
 
     def get_defined_tags(self):
         """
+        Returns defined tags
+
         Cloud service only.
 
         :returns: the tags
-        :rtype: dict(str, dict(str, object))
-        :versionadded: 5.4.0
+        :rtype: dict[str, dict[str, object]]
+        :versionadded:: 5.4.0
         """
         return self._defined_tags
 
     def get_free_form_tags(self):
         """
+        Returns free form tags
+
         Cloud service only.
 
         :returns: the tags
-        :rtype: dict(str, str)
-        :versionadded: 5.4.0
+        :rtype: dict[str, str]
+        :versionadded:: 5.4.0
         """
         return self._free_form_tags
 
     def set_ddl(self, value):
         self._ddl = value
 
     def set_table_id(self, value):
@@ -5515,17 +6253,21 @@
                     'Operation not completed in expected time', wait_millis)
             if res is not None:
                 # only delay after the first get_table.
                 sleep(delay_s)
             res = handle.get_table(get_table)
             # partial "copy" of possibly modified state. Don't modify
             # operationId as that is what we are waiting to complete.
+            # what about? tags, match etags?
             self._state = res.get_state()
             self._limits = res.get_table_limits()
             self._schema = res.get_schema()
+            self._schema_frozen = res.is_schema_frozen()
+            self._local_replica_initialized = res.is_local_replica_initialized()
+            self._replicas = res.get_replicas()
             if self._state in terminal:
                 break
 
 
 class TableUsageResult(Result):
     """
     Cloud service only.
@@ -5567,16 +6309,16 @@
 
     def set_usage_records(self, records):
         self._usage_records = records
         return self
 
     def get_usage_records(self):
         """
-        Returns a list of usage records based on the parameters of the
-        :py:class:`TableUsageRequest` used.
+        Returns a list of :py:class:`TableUsage` records based on the
+        parameters of the :py:class:`TableUsageRequest` used.
 
         :returns: an list of usage records.
         :type: list(TableUsage)
         """
         return self._usage_records
 
     def set_last_index_returned(self, last_index_returned):
@@ -5810,19 +6552,96 @@
 
     def get_existing_modification_time(self):
         """
         Returns the existing row modification time if available.
 
         :returns: the modification time in milliseconds since January 1, 1970
         :rtype: int
-        :versionadded: 5.3.0
+        :versionadded:: 5.3.0
         """
         return self._get_existing_modification_time()
 
 
+class ReplicaStatsResult(Result):
+    """
+    Cloud service only
+
+    ReplicaStatsResult is returned from
+    :py:meth:`NoSQLHandle.get_replicat_stats`. It contains replica statistics
+    for the requested table
+    """
+    def __init__(self):
+        super(ReplicaStatsResult, self).__init__()
+        self._table_name = None
+        self._next_start_time = 0
+        self._stats_record = None # dict<string, ReplicaStats array>
+
+    def get_table_name(self):
+        """
+        Returns the table name used by the operation
+
+        :returns the table name
+        :rtype: str
+        """
+        return self._table_name
+
+    def get_next_start_time(self):
+        """
+        Returns the next start time. This can be provided to a
+        :py:class:`ReplicaStatsRequest` to be used as a starting point for
+        listing stats records
+
+        :returns the next start time
+        :rtype: in
+        """
+        return self._next_start_time
+
+    def get_stats_record(self):
+        """
+        Returns replica statistics information based on the arguments of
+        the :py:class:`ReplicaStatsRequest` used for the request.
+        It contains stats for either one replica or all replicas.
+
+        The stats format is a dict where the key is a replica name and the
+        value is a list of :py:class:`ReplicaStats` objects
+
+        :returns: the stats
+        :rtype: dict
+        """
+        return self._stats_record
+
+    def set_table_name(self, table_name):
+        self._table_name = table_name
+        return self
+
+    def set_next_start_time(self, next_start_time):
+        self._next_start_time = next_start_time
+        return self
+
+    def set_stats_records(self, records):
+        self._stats_record = records
+        return self
+
+    def __str__(self):
+        # consider a prettier output format, JSON or pythonic
+        if self._stats_record is None:
+            records_str = 'None'
+        else:
+            records_str = 'ReplicaStatsResult [table=' + self._table_name + '] '
+            for rep_name, stats in self._stats_record.items():
+                records_str += '[Replica [name=' + rep_name + '['
+                for i in range(0, len(stats)):
+                    stat = stats[i]
+                    records_str += str(stat)
+                    if i < len(stats)-1:
+                        records_str += ','
+                records_str += ']]'
+        return records_str
+
+
 class RetryStats(object):
     """
     A class that maintains stats on retries during a request.
 
     This object tracks statistics about retries performed during requests. It
     can be accessed from within retry handlers (see :py:class:`RetryHandler`) or
     after a request is finished by calling :py:meth:`Request.get_retry_stats`.
@@ -5866,30 +6685,30 @@
 
     def get_exceptions_map(self):
         """
         Internal use only.
 
         Returns the map of exceptions.
 
-        :versionadded: 5.3.6
+        :versionadded:: 5.3.6
         """
         return self._exception_map
 
     def add_exceptions(self, ex_map):
         """
         Internal use only.
 
         Adds all exceptions to the stats object.
 
         This increments the exception count and adds to the count of this type
         of exception class.
 
         :param ex_map: the exceptions map.
         :type ex_map: dict[Exception, int]
-        :versionadded: 5.3.6
+        :versionadded:: 5.3.6
         """
         for k in ex_map.keys():
             num = self.get_num_exceptions(k) + ex_map[k]
             self._exception_map[k] = num
 
     def clear(self):
         """
```

### Comparing `borneo-5.4.1/src/borneo/query.py` & `borneo-5.4.2/src/borneo/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from abc import ABCMeta, abstractmethod
 from collections import OrderedDict
 from datetime import datetime
 from decimal import Decimal, setcontext
+from functools import cmp_to_key
 from sys import getsizeof
 from sys import maxsize as maxvalue
 
 from .common import ByteOutputStream, CheckValue, Empty, JsonNone, enum
 from .exception import (
     IllegalArgumentException, IllegalStateException, NoSQLException,
     QueryException, QueryStateException, RetryableException)
@@ -122,15 +123,15 @@
     If there are no more results to be produced, the next() call will return
     False. Actually, the same is True for all iterators: each next() call on a
     plan iterator produces one item in the result set of that iterator or
     returns False if there are no more results. So, in the most general case,
     the result set of each iterator is a sequence of zero or more items.
 
     The root iterator will always produce dict values, but other iterators may
-    produces different kinds of values.
+    produce different kinds of values.
 
     Iterator state and registers:
 
     As mentioned already, each next() call on an iterator produces at most one
     result item. However, the result items are not returned by the next() call
     directly. Instead, each iterator places its current result (the item
     produced by the current invocation of the next() call) in its "result
@@ -266,16 +267,20 @@
             op_iter = ArithOpIter(bis)
         elif kind == PlanIter.PlanIterKind.CONST:
             op_iter = ConstIter(bis)
         elif kind == PlanIter.PlanIterKind.EXTERNAL_VAR_REF:
             op_iter = ExternalVarRefIter(bis)
         elif kind == PlanIter.PlanIterKind.FIELD_STEP:
             op_iter = FieldStepIter(bis)
+        elif kind == PlanIter.PlanIterKind.FN_COLLECT:
+            op_iter = FuncCollectIter(bis)
         elif kind == PlanIter.PlanIterKind.FN_MIN_MAX:
             op_iter = FuncMinMaxIter(bis)
+        elif kind == PlanIter.PlanIterKind.FN_SIZE:
+            op_iter = FuncSizeIter(bis)
         elif kind == PlanIter.PlanIterKind.FN_SUM:
             op_iter = FuncSumIter(bis)
         elif kind == PlanIter.PlanIterKind.GROUP:
             op_iter = GroupIter(bis)
         elif kind == PlanIter.PlanIterKind.RECV:
             op_iter = ReceiveIter(bis)
         elif kind == PlanIter.PlanIterKind.SFW:
@@ -395,33 +400,37 @@
 
         CONST = 0
         VAR_REF = 1
         EXTERNAL_VAR_REF = 2
         ARITH_OP = 8
         FIELD_STEP = 11
         SFW = 14
+        FN_SIZE = 15
         RECV = 17
         FN_SUM = 39
         FN_MIN_MAX = 41
         SORT = 47
         GROUP = 65
         SORT2 = 66
+        FN_COLLECT = 78
 
         VALUES_TO_NAMES = {0: 'CONST',
                            1: 'VAR_REF',
                            2: 'EXTERNAL_VAR_REF',
                            8: 'ARITH_OP',
                            11: 'FIELD_STEP',
                            14: 'SFW',
+                           15: 'FN_SIZE',
                            17: 'RECV',
                            39: 'FN_SUM',
                            41: 'FN_MIN_MAX',
                            47: 'SORT',
                            65: 'GROUP',
-                           66: 'SORT2'}
+                           66: 'SORT2',
+                           78: 'FN_COLLECT'}
 
         @staticmethod
         def value_of(kvcode):
             name = PlanIter.PlanIterKind.VALUES_TO_NAMES.get(kvcode)
             if name is None:
                 print('Unexpected iterator kind: ' + str(kvcode))
             return name
@@ -432,15 +441,17 @@
     FUNC_CODE = enum(OP_ADD_SUB=14,
                      OP_MULT_DIV=15,
                      FN_COUNT_STAR=42,
                      FN_COUNT=43,
                      FN_COUNT_NUMBERS=44,
                      FN_SUM=45,
                      FN_MIN=47,
-                     FN_MAX=48)
+                     FN_MAX=48,
+                     FN_ARRAY_COLLECT=91,
+                     FN_ARRAY_COLLECT_DISTINCT=92)
 
 
 class ArithOpIter(PlanIter):
     """
     Iterator to implement the arithmetic operators
 
     any_atomic? ArithOp(any?, ....)
@@ -820,14 +831,149 @@
                 result = ctx_item[self._field_name]
             except KeyError:
                 continue
             rcb.set_reg_val(self.result_reg, result)
             return True
 
 
+class FuncCollectIter(PlanIter):
+    """
+    array_collect()
+
+    Implements the array_collect() function.
+    """
+
+    def __init__(self, bis):
+        super(FuncCollectIter, self).__init__(bis)
+        self._is_distinct = bis.read_boolean()
+        self._input_iter = self.deserialize_iter(bis)
+
+    def get_kind(self):
+        return PlanIter.PlanIterKind.value_of(
+            ArithOpIter.PlanIterKind.FN_COLLECT)
+
+    def get_input_iter(self):
+        return self._input_iter
+
+    def open(self, rcb):
+        rcb.set_state(self.state_pos, FuncCollectIter.CollectIterState(rcb))
+        self._input_iter.open(rcb)
+
+    def reset(self, rcb):
+        # don't reset state. It is reset in get_aggr_value
+        self._input_iter.reset(rcb)
+
+    def close(self, rcb):
+        state = rcb.get_state(self.state_pos)
+        if state is None:
+            return
+        self._input_iter.close(rcb)
+        state.close()
+
+    def display_content(self, output, formatter):
+        return self._input_iter.display(output, formatter)
+
+    def next(self, rcb):
+        state = rcb.get_state(self.state_pos)
+        if state.is_done():
+            return False
+        while True:
+            more = self._input_iter.next(rcb)
+            if not more:
+                return True
+            val = rcb.get_reg_val(self._input_iter.get_result_reg())
+            if rcb.get_trace_level() >= 2:
+                rcb.trace('Collecting value ' + str(val))
+            if val is None:
+                continue
+            self.aggregate(rcb, val)
+
+    def aggregate(self, rcb, val):
+        state = rcb.get_state(self.state_pos)
+        if self._is_distinct:
+            size = len(val)
+            for i in range(size):
+                state.get_values().add(Hashable(val[i]))
+                sz = self.sizeof(val[i])
+                rcb.inc_memory_consumption(sz)
+                state._memory_consumption += sz
+        else:
+            # add all values from val to state._array
+            sz = 0
+            for item in val:
+                state.get_array().append(item)
+                sz += self.sizeof(item)
+            rcb.inc_memory_consumption(sz)
+            state._memory_consumption += sz
+
+    def get_aggr_value(self, rcb, reset):
+        state = rcb.get_state(self.state_pos)
+
+        if self._is_distinct:
+            res = list()
+            for item in state.get_values():
+                res.append(item._value)
+
+        else:
+            # not a copy, the array must stay valid
+            res = state.get_array()
+
+        #
+        # QTF issue -- qtf wants to compare expected values. While array_collect
+        # doesn't define an ordering, it is handy for QTF comparisons, so
+        # sort result arrays (ascending)
+        #
+        if rcb.get_request().get_in_test_mode():
+            res.sort(key=cmp_to_key(lambda v1, v2: Compare.compare_total_order(
+                rcb, v1, v2, SortSpec())))
+
+        if rcb.get_trace_level() >= 3:
+            rcb.trace('Collected values = ' + str(res))
+
+        if reset:
+            state.reset()
+
+        return res
+
+    class CollectIterState(PlanIterState):
+
+        def __init__(self, rcb):
+            super(FuncCollectIter.CollectIterState, self).__init__()
+            self._rcb = rcb
+            self._array = list()
+            self._values = set()
+            self._memory_consumption = 0
+
+        def get_values(self):
+            return self._values
+
+        def get_array(self):
+            return self._array
+
+        def get_memory_consumption(self):
+            return self._memory_consumption
+
+        def close(self):
+            super(FuncCollectIter.CollectIterState, self).close()
+            self._array = None
+            self._values = None
+
+        def done(self):
+            super(FuncCollectIter.CollectIterState, self).done()
+            self._array = None
+            self._values = None
+
+        def reset(self):
+            super(FuncCollectIter.CollectIterState, self).reset()
+            self._values = set()
+            self._array = list()
+            self._rcb.dec_memory_consumption(self._memory_consumption)
+            self._memory_consumption = 0
+
+
 class FuncMinMaxIter(PlanIter):
     """
     any_atomic min(any*)
     any_atomic max(any*)
 
     Implements the MIN/MAX aggregate functions. It is needed by the driver to
     compute the total min/max from the partial mins/maxs received from the
@@ -892,39 +1038,98 @@
         if (val is None or isinstance(val, bytearray) or isinstance(val, dict)
                 or isinstance(val, list) or isinstance(val, Empty) or
                 isinstance(val, JsonNone)):
             return
         if state.min_max is None:
             state.min_max = val
             return
-        comp = Compare.compare_atomics(rcb, state.min_max, val, True)
+        comp = Compare.compare_atomics_total_order(rcb, state.min_max, val)
         if rcb.get_trace_level() >= 3:
             rcb.trace('Compared values: \n' + str(state.min_max) + '\n' +
                       str(val) + '\ncomp res = ' + str(comp))
         if fncode == PlanIter.FUNC_CODE.FN_MIN:
             if comp <= 0:
                 return
         else:
             if comp >= 0:
                 return
         if rcb.get_trace_level() >= 2:
             rcb.trace('Setting min/max to ' + str(val))
         state.min_max = val
 
 
+class FuncSizeIter(PlanIter):
+    """
+    """
+
+    def __init__(self, bis):
+        super(FuncSizeIter, self).__init__(bis)
+        self._input_iter = self.deserialize_iter(bis)
+
+    def close(self, rcb):
+        state = rcb.get_state(self.state_pos)
+        if state is not None:
+            self._input_iter.close(rcb)
+            state.close()
+
+    def display_content(self, output, formatter):
+        return self._input_iter.display(output, formatter)
+
+    def get_kind(self):
+        return PlanIter.PlanIterKind.value_of(
+            ArithOpIter.PlanIterKind.FN_SIZE)
+
+    def next(self, rcb):
+        state = rcb.get_state(self.state_pos)
+        if state is None or state.is_done():
+            return False
+
+        more = self._input_iter.next(rcb)
+        if not more:
+            state.done()
+            return False
+
+        val = rcb.get_reg_val(self._input_iter.get_result_reg())
+        if val is None:
+            rcb.set_reg_val(self.result_reg, None)
+            state.done()
+            return True
+        if not isinstance(val, dict) and not isinstance(val, list) \
+                and not isinstance(val, set):
+            raise QueryException(
+                'Invalid type for input to size() function, it must be \n' +
+                'complex. Actual type is: ' + str(type(val)))
+
+        rcb.set_reg_val(self.result_reg, len(val))
+        return True
+
+    def get_input_iter(self):
+        return self._input_iter
+
+    def open(self, rcb):
+        rcb.set_state(self.state_pos, AggrIterState())
+        self._input_iter.open(rcb)
+
+    def reset(self, rcb):
+        self._input_iter.reset(rcb)
+        state = rcb.get_state(self.state_pos)
+        if state is not None:
+            state.reset()
+
+
 class FuncSumIter(PlanIter):
     """
     any_atomic sum(any*)
 
     Implements the SUM aggregate function. It is needed by the driver to re-sum
     partial sums and counts received from the proxy.
 
     Note: The next() method does not actually return a value; it just adds a new
     value (if it is of a numeric type) to the running sum kept in the state.
-    Also the reset() method resets the input iter (so that the next input value
+    Also, the reset() method resets the input iter (so that the next input value
     can be computed), but does not reset the FuncSumState. The state is reset,
     and the current sum value is returned, by the get_aggr_value() method.
     """
 
     def __init__(self, bis):
         super(FuncSumIter, self).__init__(bis)
         self._input_iter = self.deserialize_iter(bis)
@@ -1045,82 +1250,104 @@
 
     def next(self, rcb):
         state = rcb.get_state(self.state_pos)
         if state.is_done():
             return False
         while True:
             if state.results_copy is not None:
+                #
+                # pull results off of the available results in memory
+                #
                 try:
                     (gb_tuple, aggr_tuple) = (
                         state.results_copy.popitem(last=False))
                     res = dict()
                     i = 0
                     while i < self.num_gb_columns:
                         res[self._column_names[i]] = gb_tuple.values[i]
                         i += 1
                     for i in range(i, len(self._column_names)):
-                        aggr = self._get_aggr_value(aggr_tuple, i)
+                        aggr = self._get_aggr_value(rcb, aggr_tuple, i)
                         res[self._column_names[i]] = aggr
+                    # NOTE: this method always copies
                     res = SerdeUtil.convert_value_to_none(res)
                     rcb.set_reg_val(self.result_reg, res)
+                    # popitem() above removed it from the copy, now remove it
+                    # from the actual results dict
                     if self._remove_produced_result:
                         state.results.pop(gb_tuple)
                     return True
                 except KeyError:
                     # Dictionary is empty.
                     state.done()
                     return False
+
+            # look for additional results from the input iterator
             more = self._input.next(rcb)
             if not more:
                 if rcb.reached_limit():
                     return False
                 if self.num_gb_columns == len(self._column_names):
                     state.done()
                     return False
+                # NOTE: Python does a copy of the OrderedDict that is
+                # state.results. Java and other SDKs just create an
+                # iterator. Consider the latter for efficiency
                 state.results_copy = state.results.copy()
                 continue
+
             in_tuple = rcb.get_reg_val(self._input.get_result_reg())
             i = 0
             while i < self.num_gb_columns:
                 col_value = in_tuple.get(self._column_names[i])
                 if isinstance(col_value, Empty):
                     if self._is_distinct:
                         col_value = None
                     else:
                         break
                 state.gb_tuple.values[i] = col_value
                 i += 1
+
             if i < self.num_gb_columns:
+                # keep acquiring more results for the grouping
                 continue
+
             aggr_tuple = state.results.get(state.gb_tuple)
             if aggr_tuple is None:
                 num_aggr_columns = (
                         len(self._column_names) - self.num_gb_columns)
                 gb_tuple = GroupIter.GroupTuple(self.num_gb_columns)
                 aggr_tuple = list()
                 aggr_tuple_size = 0
                 for i in range(num_aggr_columns):
                     val = GroupIter.AggrValue(self._aggr_funcs[i])
                     aggr_tuple.append(val)
                     if self._count_memory:
                         aggr_tuple_size += self.sizeof(val)
+
                 i = 0
                 while i < self.num_gb_columns:
                     gb_tuple.values[i] = state.gb_tuple.values[i]
                     i += 1
+
                 if self._count_memory:
+                    # NOTE: hash/dict overhead is not added
                     sz = self.sizeof(gb_tuple) + aggr_tuple_size
                     rcb.inc_memory_consumption(sz)
+
                 for i in range(i, len(self._column_names)):
                     self._aggregate(rcb, aggr_tuple, i,
                                     in_tuple.get(self._column_names[i]))
+
                 state.results[gb_tuple] = aggr_tuple
+
                 if rcb.get_trace_level() >= 3:
                     rcb.trace('Started new group:\n' +
                               GroupIter._print_result(gb_tuple, aggr_tuple))
+
                 if self.num_gb_columns == len(self._column_names):
                     res = dict()
                     for i in range(self.num_gb_columns):
                         res[self._column_names[i]] = gb_tuple.values[i]
                     res = SerdeUtil.convert_value_to_none(res)
                     rcb.set_reg_val(self.result_reg, res)
                     return True
@@ -1170,15 +1397,16 @@
                 if rcb.get_trace_level() >= 3:
                     rcb.trace('Setting min/max to ' + str(val))
                 if self._count_memory:
                     rcb.inc_memory_consumption(
                         self.sizeof(val) - self.sizeof(aggr_value.value))
                 aggr_value.value = val
                 return
-            comp = Compare.compare_atomics(rcb, aggr_value.value, val, True)
+            comp = Compare.compare_atomics_total_order(rcb, aggr_value.value,
+                                                       val)
             if rcb.get_trace_level() >= 3:
                 rcb.trace('Compared values: \n' + str(aggr_value.value) + '\n' +
                           str(val) + '\ncomp res = ' + str(comp))
             if aggr_kind == PlanIter.FUNC_CODE.FN_MIN:
                 if comp <= 0:
                     return
             else:
@@ -1187,24 +1415,48 @@
             if rcb.get_trace_level() >= 3:
                 rcb.trace('Setting min/max to ' + str(val))
             if (self._count_memory and
                     not isinstance(val, type(aggr_value.value))):
                 rcb.inc_memory_consumption(
                     self.sizeof(val) - self.sizeof(aggr_value.value))
             aggr_value.value = val
+        elif (aggr_kind == PlanIter.FUNC_CODE.FN_ARRAY_COLLECT or
+              aggr_kind == PlanIter.FUNC_CODE.FN_ARRAY_COLLECT_DISTINCT):
+            aggr_value.collect(rcb, val, self._count_memory)
         else:
             raise QueryStateException(
                 'Method not implemented for iterator ' + str(aggr_kind))
 
-    def _get_aggr_value(self, aggr_tuple, column):
+    def _get_aggr_value(self, rcb, aggr_tuple, column):
         aggr_value = aggr_tuple[column - self.num_gb_columns]
         aggr_kind = self._aggr_funcs[column - self.num_gb_columns]
         if (aggr_kind == PlanIter.FUNC_CODE.FN_SUM and
                 not aggr_value.got_numeric_input):
             return None
+
+        if aggr_kind == PlanIter.FUNC_CODE.FN_ARRAY_COLLECT:
+            if rcb.get_request().get_in_test_mode():
+                # QTF wants sorted results
+                aggr_value.value.sort(key=cmp_to_key(lambda v1, v2:
+                                                     Compare.compare_total_order(rcb, v1, v2, SortSpec())))
+
+            return aggr_value.value
+
+        if aggr_kind == PlanIter.FUNC_CODE.FN_ARRAY_COLLECT_DISTINCT:
+            # the value is a set of wrapped objects, unwrap and optionally
+            # sort them
+            newlist = list()
+            for elem in aggr_value.value:
+                newlist.append(elem._value)
+            if rcb.get_request().get_in_test_mode():
+                # QTF wants sorted results
+                newlist.sort(key=cmp_to_key(lambda v1, v2:
+                                            Compare.compare_total_order(rcb, v1, v2, SortSpec())))
+            return newlist
+
         return aggr_value.value
 
     @staticmethod
     def _print_result(gb_tuple, aggr_values):
         output = '['
         for i in range(len(gb_tuple.values)):
             output += str(gb_tuple.values[i]) + ' '
@@ -1222,14 +1474,18 @@
                     kind == PlanIter.FUNC_CODE.FN_COUNT_NUMBERS or
                     kind == PlanIter.FUNC_CODE.FN_COUNT_STAR or
                     kind == PlanIter.FUNC_CODE.FN_SUM):
                 self.value = 0
             elif (kind == PlanIter.FUNC_CODE.FN_MAX or
                   kind == PlanIter.FUNC_CODE.FN_MIN):
                 self.value = None
+            elif kind == PlanIter.FUNC_CODE.FN_ARRAY_COLLECT:
+                self.value = list()
+            elif kind == PlanIter.FUNC_CODE.FN_ARRAY_COLLECT_DISTINCT:
+                self.value = set()
             else:
                 assert False
 
         def add(self, rcb, count_memory, val, ctx):
             setcontext(ctx)
             sz = 0
             if CheckValue.is_int_value(val):
@@ -1265,19 +1521,41 @@
                 elif isinstance(self.value, Decimal):
                     self.value += val
                 else:
                     assert False
             else:
                 assert False
 
+        def sizeof(self, val):
+            return PlanIter.sizeof(val)
+
+        def collect(self, rcb, val, count_memory):
+            if val is None or isinstance(val, Empty):
+                return
+            is_distinct = isinstance(self.value, set)
+            if is_distinct:
+                # value is a set
+                collect_set = self.value
+                for elem in val:
+                    collect_set.add(Hashable(elem))
+                    if count_memory:
+                        rcb.inc_memory_consumption(self.sizeof(elem))
+            else:
+                # value is a list
+                collect_array = self.value
+                collect_array.extend(val)
+                if count_memory:
+                    rcb.inc_memory_consumption(self.sizeof(val))
+
     class GroupIterState(PlanIterState):
 
         def __init__(self, op_iter):
             super(GroupIter.GroupIterState, self).__init__()
             self.gb_tuple = GroupIter.GroupTuple(op_iter.num_gb_columns)
+            # FUTURE: consider dict() which is now ordered
             self.results = OrderedDict()
             self.results_copy = None
 
         def close(self):
             super(GroupIter.GroupIterState, self).close()
             self.gb_tuple = None
             self.results.clear()
@@ -1423,60 +1701,46 @@
         bin_prim_key = self._create_binary_primkey(res)
         if bin_prim_key in state.prim_keys_set:
             if rcb.get_trace_level() >= 1:
                 rcb.trace(
                     'ReceiveIter._check_duplicate() : result was duplicate')
             return True
         else:
-            state.prim_keys_set.append(bin_prim_key)
+            state.prim_keys_set.add(bin_prim_key)
         sz = self.sizeof(bin_prim_key)
         state.memory_consumption += sz
         state.dup_elim_memory += sz
         rcb.inc_memory_consumption(sz)
         return False
 
     def _create_binary_primkey(self, result):
         binary_primkey = bytearray()
         out = ByteOutputStream(binary_primkey)
         for i in range(len(self._prim_key_fields)):
             fval = result.get(self._prim_key_fields[i])
             self._write_value(out, fval, i)
-        return binary_primkey
+        # convert to immutable bytes so that it can be hashed into a set
+        return bytes(binary_primkey)
 
-    def _handle_topology_change(self, rcb, state):
-        new_topo_info = rcb.get_topology_info()
+    def _handle_virtual_scans(self, rcb, state, scanner):
         if ((self.distribution_kind ==
              ReceiveIter.DISTRIBUTION_KIND.ALL_PARTITIONS) or
-                new_topo_info == state.topo_info):
+                scanner.get_virtual_scans() is None):
             return
-        new_shards = new_topo_info.get_shard_ids()
-        curr_shards = state.topo_info.get_shard_ids()
-        for i in range(len(new_shards)):
-            equal = False
-            for j in range(len(curr_shards)):
-                if new_shards[i] == curr_shards[j]:
-                    curr_shards[j] = -1
-                    equal = True
-                    break
-            if equal:
-                continue
-            # We have a new shard
-            ReceiveIter.add_scanner(
-                state.sorted_scanners,
-                ReceiveIter.RemoteScanner(
-                    self, rcb, state, True, new_shards[i]))
-        for j in range(len(curr_shards)):
-            if curr_shards[j] == -1:
-                continue
-            # This shard does not exist any more
-            for scanner in state.sorted_scanners:
-                if scanner.shard_or_part_id == curr_shards[j]:
-                    state.sorted_scanners.remove(scanner)
-                    break
-        state.topo_info = new_topo_info
+
+        for vs in scanner.get_virtual_scans():
+            vsid = state.base_VSID
+            ++state.base_VSID
+            new_scanner = ReceiveIter.RemoteScanner(
+                    self, rcb, state, True, vsid, vs)
+            ReceiveIter.add_scanner(state.sorted_scanners, new_scanner)
+            if rcb.get_trace_level() >= 1:
+                rcb.trace('ReceiveIter: added scanner for virtual scan:\n' + vs)
+
+        scanner._virtual_scans = None
 
     def _init_partition_sort(self, rcb, state):
         """
         Make sure we receive (and cache) at least one result per partition
         (except from partitions that do not contain any results at all).
         """
         assert state.is_in_sort_phase1
@@ -1582,14 +1846,15 @@
             # Scanner had no cached results. If it may have remote results, send
             # a request to fetch more results. Otherwise, throw it away (by
             # leaving it outside sorted_scanners) and continue with another
             # scanner.
             if not scanner.is_done():
                 try:
                     scanner.fetch()
+                    self._handle_virtual_scans(rcb, state, scanner)
                 except RetryableException as e:
                     ReceiveIter.add_scanner(state.sorted_scanners, scanner)
                     raise e
             else:
                 continue
             # We executed a remote fetch. If we got any result or the scanner
             # may have more remote results, put the scanner back into
@@ -1597,19 +1862,18 @@
             if not scanner.is_done():
                 ReceiveIter.add_scanner(state.sorted_scanners, scanner)
             else:
                 if rcb.get_trace_level() >= 1:
                     rcb.trace(
                         'ReceiveIter._sorting_next() : done with ' +
                         'partition/shard ' + str(scanner.shard_or_part_id))
-            self._handle_topology_change(rcb, state)
             # For simplicity, we don't want to allow the possibility of another
-            # remote fetch during the same batch, so whether or not the batch
-            # limit was reached during the above fetch, we set limit flag to
-            # True and return False, thus terminating the current batch.
+            # remote fetch during the same batch. Regardless of whether
+            # the batch limit was reached during the above fetch, we set limit
+            # flag to True and return False, thus terminating the current batch.
             rcb.set_reached_limit(True)
             return False
 
     @staticmethod
     def _write_value(out, value, i):
         if isinstance(value, float):
             out.write_float(value)
@@ -1647,57 +1911,63 @@
             # self.prim_keys_set.
             self.memory_consumption = 0
             # The remote scanner used for non-sorting queries.
             self.scanner = None
             # The remote scanners used for sorting queries. For all-shard
             # queries there is one RemoteScanner per shard. For all-partition
             # queries a RemoteScanner is created for each partition that has at
-            # least one result.
+            # least one result. Sorted scanners are always kept in order of
+            # the first element in each scanner. This means they have to be
+            # re-sorted each time a result is consumed
             self.sorted_scanners = None
             # total_results_size and total_num_results store the total size and
             # number of results fetched by this ReceiveIter so far. They are
             # used to compute the average result size, which is then used to
             # compute the max number of results to fetch from a partition during
             # a sort-phase-2 request for a sorting, all-partition query.
             self.total_num_results = 0
             self.total_results_size = 0
-            # It stores the set of shard ids. Needed for sorting all-shard
-            # queries only.
-            self.topo_info = rcb.get_topology_info()
+            # virtual scans
+            self.base_VSID = -1
             # The prim_keys_set is the hash set used for duplicate elimination.
             # It stores the primary keys (in binary format) of all the results
             # seen so far.
             if op_iter.does_dup_elim():
-                self.prim_keys_set = list()
+                self.prim_keys_set = set()
             else:
                 self.prim_keys_set = None
             if (op_iter.does_sort() and
                     (op_iter.distribution_kind ==
                      ReceiveIter.DISTRIBUTION_KIND.ALL_PARTITIONS)):
+                # TODO: turn this into a sorted set or list to avoid
+                # re-sorting when the first element is removed and the
+                # scanner re-added
                 self.sorted_scanners = list()
             elif (op_iter.does_sort() and
                   (op_iter.distribution_kind ==
                    ReceiveIter.DISTRIBUTION_KIND.ALL_SHARDS)):
-                num_shards = self.topo_info.num_shards()
+                base_topo = rcb.get_base_topo()
+                num_shards = base_topo.num_shards()
                 self.sorted_scanners = list()
                 for i in range(num_shards):
                     ReceiveIter.add_scanner(
                         self.sorted_scanners,
                         ReceiveIter.RemoteScanner(
                             out, rcb, self, True,
-                            self.topo_info.get_shard_id(i)))
+                            base_topo.get_shard_id(i)))
+                self.base_VSID = base_topo.get_last_shard_id() + 1
             else:
                 self.scanner = ReceiveIter.RemoteScanner(
                     out, rcb, self, False, -1)
 
         def clear(self):
             if self.prim_keys_set is not None:
-                del self.prim_keys_set[:]
+                self.prim_keys_set.clear()
             if self.sorted_scanners is not None:
-                del self.sorted_scanners[:]
+                self.sorted_scanners.clear()
 
         def close(self):
             super(ReceiveIter.ReceiveIterState, self).close()
             self.prim_keys_set = None
             self.sorted_scanners = None
 
         def done(self):
@@ -1717,25 +1987,27 @@
 
         For non-ordering queries, there is a single RemoteScanner. It will fetch
         as many as possible results starting from the shard or partition
         specified in self.continuation_key (so it may fetch results from more
         than one shard/partition).
         """
 
-        def __init__(self, out, rcb, state, is_for_shard, spid):
+        def __init__(self, out, rcb, state, is_for_shard, spid, vs = None):
             self._out = out
             self.rcb = rcb
             self.state = state
             self.is_for_shard = is_for_shard
             self.shard_or_part_id = spid
             self.results = None
             self.results_size = 0
             self.next_result_pos = 0
             self.continuation_key = None
             self.more_remote_results = True
+            self.virtual_scan = vs # virtual scan
+            self.virtual_scans = None # virtual scan list
 
         def add_results(self, results, cont_key):
             self.results = results
             self.continuation_key = cont_key
             self.more_remote_results = cont_key is not None
             self._add_memory_consumption()
 
@@ -1752,16 +2024,21 @@
             comp = Compare.sort_results(self.rcb, v1, v2, self._out.sort_fields,
                                         self._out.sort_specs)
             if comp == 0:
                 comp = (-1 if self.shard_or_part_id < other.shard_or_part_id
                         else 1)
             return comp
 
+        def get_virtual_scans(self):
+            return self.virtual_scans
+
         def fetch(self):
-            req = self.rcb.get_request().copy_internal()
+            orig_request = self.rcb.get_request()
+            orig_request.incr_batch_counter()
+            req = orig_request.copy_internal()
             req.set_cont_key(self.continuation_key)
             req.set_shard_id(
                 self.shard_or_part_id if self.is_for_shard else -1)
             if self._out.does_sort() and not self.is_for_shard:
                 self.state.memory_consumption -= self.results_size
                 self.rcb.dec_memory_consumption(self.results_size)
                 num_results = ((req.get_max_memory_consumption() -
@@ -1769,44 +2046,59 @@
                                ((len(self.state.sorted_scanners) + 1) *
                                 (self.state.total_results_size //
                                  self.state.total_num_results)))
                 if num_results > 2048:
                     num_results = 2048
                 req.set_limit(int(num_results))
             if self.rcb.get_trace_level() >= 1:
-                self.rcb.trace('RemoteScanner : executing remote request. '
-                               'spid = ' + str(self.shard_or_part_id))
+                self.rcb.trace('RemoteScanner : executing remote batch. ' +
+                               orig_request.get_batch_counter() +
+                               ', spid = ' + str(self.shard_or_part_id))
+                if self.virtual_scan is not None:
+                    self.rcb.trace(
+                        'RemoteScanner: request is for virtual scan:\n' +
+                        str(self.virtual_scan))
                 assert req.has_driver()
+            if self.virtual_scan is not None:
+                req.set_virtual_scan(self.virtual_scan)
             result = self.rcb.get_client().execute(req)
+            if self.virtual_scan is not None:
+                self.virtual_scan['info_sent'] = True
             self.results = result.get_results_internal()
+            self.virtual_scans = result.get_virtual_scans()
             self.continuation_key = result.get_continuation_key()
             self.next_result_pos = 0
             self.more_remote_results = self.continuation_key is not None
             self.rcb.tally_read_kb(result.get_read_kb())
             self.rcb.tally_read_units(result.get_read_units())
             self.rcb.tally_write_kb(result.get_write_kb())
             assert result.reached_limit() or not self.more_remote_results
+            orig_request.set_query_traces(result.get_query_traces())
             # For simplicity, if the query is a sorting one, we consider the
             # current batch done as soon as we get the response back from the
             # proxy, even if the batch limit was not reached there.
             if result.reached_limit() or self._out.does_sort():
                 self.rcb.set_reached_limit(True)
             if self._out.does_sort() and not self.is_for_shard:
                 self._add_memory_consumption()
             if self.rcb.get_trace_level() >= 1:
-                self.rcb.trace(
-                    'RemoteScanner : got ' + str(len(self.results)) +
-                    ' remote results. More remote results = ' +
-                    str(self.more_remote_results) +
-                    ' reached limit = ' + str(result.reached_limit()) +
-                    ' read KB = ' + str(result.get_read_kb()) +
-                    ' read Units = ' + str(result.get_read_units()) +
-                    ' write KB = ' + str(result.get_write_kb()) +
-                    ' memory consumption = ' +
-                    str(self.state.memory_consumption))
+                msg = ('RemoteScanner : got ' + str(len(self.results)) +
+                           ' remote results. More remote results = ' +
+                           str(self.more_remote_results) +
+                           ' reached limit = ' + str(result.reached_limit()) +
+                           ' read KB = ' + str(result.get_read_kb()) +
+                           ' read Units = ' + str(result.get_read_units()) +
+                           ' write KB = ' + str(result.get_write_kb()) +
+                           ' memory consumption = ' +
+                           str(self.state.memory_consumption))
+                if self.virtual_scans is not None:
+                    # TODO: append vs info to trace msg
+                    pass
+
+                self.rcb.trace(msg)
 
         def has_local_results(self):
             return (self.results is not None and
                     self.next_result_pos < len(self.results))
 
         def is_done(self):
             return (not self.more_remote_results and
@@ -2008,15 +2300,15 @@
                         done = True
                         break
                     rcb.set_reg_val(column_iter.get_result_reg(), None)
                 else:
                     if rcb.get_trace_level() >= 3:
                         rcb.trace(
                             'SFW: Value for SFW column ' + str(i) + ' = ' +
-                            str(rcb.ge_reg_val(column_iter.get_result_reg())))
+                            str(rcb.get_reg_val(column_iter.get_result_reg())))
                 column_iter.reset(rcb)
             if done:
                 continue
             if self._num_gb_columns < 0:
                 if self._is_select_star:
                     break
                 result = dict()
@@ -2149,15 +2441,18 @@
                 self.column_iters[i].get_aggr_value(rcb, True))
         if rcb.get_trace_level() >= 2:
             rcb.trace('SFW: Produced last group : ' + str(result))
         return True
 
     def _trace_current_group(self, rcb, state):
         for i in range(self._num_gb_columns):
-            rcb.trace('SFW: Val ' + str(i) + ' = ' + state.gb_tuple[i])
+            v = state.gb_tuple[i]
+            if v is None:
+                v = 'None'
+            rcb.trace('SFW: Val ' + str(i) + ' = ' + str(v))
         for i in range(self._num_gb_columns, len(self.column_iters)):
             rcb.trace('SFW: Val ' + str(i) + ' = ' +
                       str(self.column_iters[i].get_aggr_value(rcb, False)))
 
     class SFWIterState(PlanIterState):
 
         def __init__(self, op_iter):
@@ -2226,20 +2521,29 @@
                 val = rcb.get_reg_val(self._input.get_result_reg())
                 for field in self._sort_fields:
                     fval = val[field]
                     if isinstance(fval, dict) or isinstance(fval, list):
                         raise QueryException(
                             'Sort expression does not return a single atomic ' +
                             ' value', self.location)
-                self._add_result(state.results, val, rcb)
+                state.results.append(val)
                 if self._count_memory:
                     rcb.inc_memory_consumption(self.sizeof(val))
                 more = self._input.next(rcb)
             if rcb.reached_limit():
                 return False
+            # sort the results using our custom comparator.
+            # See Python doc on sorting and use of funcutils.cmp_to_key
+            # Ideally we might try to use a key function directly
+            # but how to do that is not obvious if even possible. list.sort()
+            # does an in-place sort. Not in-place would use sorted().
+            # Performance seems to be similar for both
+            state.results.sort(
+                key=cmp_to_key(lambda v1, v2: Compare.sort_results(
+                    rcb, v1, v2, self._sort_fields, self._sort_specs)))
             state.set_state(PlanIterState.STATE.RUNNING)
         if state.curr_result < len(state.results):
             val = SerdeUtil.convert_value_to_none(
                 state.results[state.curr_result])
             rcb.set_reg_val(self.result_reg, val)
             state.results[state.curr_result] = None
             state.curr_result += 1
@@ -2253,28 +2557,14 @@
         self._input.open(rcb)
 
     def reset(self, rcb):
         self._input.reset(rcb)
         state = rcb.get_state(self.state_pos)
         state.reset()
 
-    def _add_result(self, sorted_results, result, rcb):
-        inserted = False
-        len_sorted_results = len(sorted_results)
-        if len_sorted_results > 0:
-            for index in range(len_sorted_results):
-                if Compare.sort_results(
-                        rcb, result, sorted_results[index], self._sort_fields,
-                        self._sort_specs) == -1:
-                    sorted_results.insert(index, result)
-                    inserted = True
-                    break
-        if not inserted:
-            sorted_results.append(result)
-
     class SortIterState(PlanIterState):
 
         def __init__(self):
             super(SortIter.SortIterState, self).__init__()
             self.results = list()
             self.curr_result = 0
 
@@ -2354,88 +2644,214 @@
         rcb.set_state(self.state_pos, PlanIterState())
 
     def reset(self, rcb):
         state = rcb.get_state(self.state_pos)
         state.reset()
 
 
+class Hashable(object):
+    """
+    Wraps an object, usually a dict, to make it hashable for sets
+    """
+
+    def __init__(self, val):
+        self._value = val
+
+    def __hash__(self):
+        return Compare.hashcode(self._value)
+
+    def __eq__(self, other):
+        return (isinstance(other, type(self)) and
+                self._value == other._value)
+
+
 class Compare(object):
 
     @staticmethod
-    def compare_atomics(rcb, v0, v1, for_sort=False):
+    def compare_atomics_total_order(rcb, v0, v1, sort_spec=None):
         """
-        Compare 2 atomic values.
-
-        The method throws an exception if either of the 2 values is non-atomic
-        or the values are not comparable. Otherwise, it returns 0 if v0 == v1,
-        1 if v0 > v1, or -1 if v0 < v1.
-
-        Whether the 2 values are comparable depends on the "forSort" parameter.
-        If True, then values that would otherwise be considered non-comparable
-        are assumed to have the following order:
+        Implements a total order among atomic values. The following order is
+        used among values that are not normally comparable with each other:
 
-        numerics < timestamps < strings < booleans < empty < JsonNone < None
+        numerics < timestamps < strings < booleans < binaries < empty
+         < json null < null
         """
         if rcb.get_trace_level() >= 4:
             rcb.trace('Comparing values: \n' + str(v0) + '\n' + str(v1))
+
+        return_value = -1
+
         if v0 is None:
             if v1 is None:
-                return 0
-            if for_sort:
-                return 1
+                return_value = 0
+            else:
+                return_value = 1
         elif isinstance(v0, JsonNone):
             if isinstance(v1, JsonNone):
-                return 0
-            if for_sort:
-                return -1 if v1 is None else 1
+                return_value = 0
+            else:
+                return_value = (-1 if v1 is None else 1)
         elif isinstance(v0, Empty):
             if isinstance(v1, Empty):
-                return 0
-            if for_sort:
-                return -1 if v1 is None or isinstance(v1, JsonNone) else 1
+                return_value = 0
+            else:
+                return_value = (-1 if v1 is None or isinstance(v1, JsonNone)
+                                else 1)
         elif isinstance(v0, bool):
             if isinstance(v1, bool):
-                return -1 if v0 < v1 else (0 if v0 == v1 else 1)
-            if for_sort:
+                return_value = (-1 if v0 < v1 else (0 if v0 == v1 else 1))
+            else:
                 if (CheckValue.is_digit(v1) or isinstance(v1, datetime) or
                         isinstance(v1, str)):
-                    return 1
-                if (v1 is None or isinstance(v1, JsonNone) or
-                        isinstance(v1, Empty)):
-                    return -1
+                    return_value = 1
         elif CheckValue.is_str(v0):
             if CheckValue.is_str(v1):
-                return -1 if v0 < v1 else (0 if v0 == v1 else 1)
-            if for_sort:
+                return_value = (-1 if v0 < v1 else (0 if v0 == v1 else 1))
+            else:
                 if CheckValue.is_digit(v1) or isinstance(v1, datetime):
-                    return 1
-                if (v1 is None or isinstance(v1, JsonNone) or
-                        isinstance(v1, Empty) or isinstance(v1, bool)):
-                    return -1
+                    return_value = 1
         elif isinstance(v0, datetime):
             if isinstance(v1, datetime):
-                return -1 if v0 < v1 else (0 if v0 == v1 else 1)
-            if for_sort:
+                return_value = (-1 if v0 < v1 else (0 if v0 == v1 else 1))
+            else:
                 if CheckValue.is_digit(v1):
-                    return 1
-                if (v1 is None or isinstance(v1, JsonNone) or
-                        isinstance(v1, Empty) or isinstance(v1, bool) or
-                        isinstance(v1, str)):
-                    return -1
+                    return_value = 1
         elif CheckValue.is_digit(v0):
             if CheckValue.is_digit(v1):
-                return -1 if v0 < v1 else (0 if v0 == v1 else 1)
-            if (for_sort and
-                    (v1 is None or isinstance(v1, JsonNone) or isinstance(v1, Empty)
-                     or isinstance(v1, bool) or isinstance(v1, str) or
-                     isinstance(v1, datetime))):
-                return -1
-        raise QueryStateException(
-            'Cannot compare value of type ' + str(type(v0)) +
-            ' with value of type ' + str(type(v1)))
+                return_value = (-1 if v0 < v1 else (0 if v0 == v1 else 1))
+        else:
+            raise QueryStateException(
+                'Cannot compare value of type ' + str(type(v0)) +
+                ' with value of type ' + str(type(v1)))
+
+        if sort_spec is not None:
+            if sort_spec.is_desc:
+                return_value = -return_value
+            if not sort_spec.is_desc and sort_spec.nones_first:
+                if Compare.is_special_value(v0) and not Compare.is_special_value(v1):
+                    return_value = -1
+                if not Compare.is_special_value(v0) and Compare.is_special_value(v1):
+                    return_value = 1
+            elif sort_spec.is_desc and not sort_spec.nones_first:
+                if Compare.is_special_value(v0) and not Compare.is_special_value(v1):
+                    return_value = 1
+                if not Compare.is_special_value(v0) and Compare.is_special_value(v1):
+                    return_value = -1
+
+        return return_value
+
+    @staticmethod
+    def compare_total_order(rcb, v0, v1, sort_spec):
+
+        if isinstance(v0, dict):
+            if isinstance(v1, dict):
+                return Compare.compare_dicts(rcb, v0, v1, sort_spec)
+            elif isinstance(v1, list):
+                return 1 if sort_spec.is_desc else -1
+            else:
+                return -1 if sort_spec.is_desc else 1
+
+        elif isinstance(v0, list):
+            if isinstance(v1, list):
+                return Compare.compare_lists(rcb, v0, v1, sort_spec)
+            else:
+                return -1 if sort_spec.is_desc else 1
+        else:
+            if isinstance(v1, dict) or isinstance(v1, list):
+                return 1 if sort_spec.is_desc else -1
+            else:
+                return Compare.compare_atomics_total_order(rcb, v0,
+                                                           v1, sort_spec)
+
+    @staticmethod
+    def compare_dicts(rcb, v0, v1, sort_spec):
+        inner_spec = sort_spec
+        if sort_spec.is_desc or sort_spec.nones_first:
+            inner_spec = SortSpec()
+
+        # need to iterate over both dicts with keys sorted
+        v0_iter = iter(sorted(v0))
+        v1_iter = iter(sorted(v1))
+
+        v0_key = next(v0_iter, None)
+        v1_key = next(v1_iter, None)
+
+        while v0_key is not None and v1_key is not None:
+            comp = Compare.compare_to(v0_key, v1_key)
+
+            # keys don't match, done
+            if comp != 0:
+                return -comp if sort_spec.is_desc else comp
+
+            # deep compare of values
+            comp = Compare.compare_total_order(rcb, v0.get(v0_key),
+                                               v1.get(v1_key), inner_spec)
+
+            # values don't match
+            if comp != 0:
+                return -comp if sort_spec.is_desc else comp
+
+            v0_key = next(v0_iter, None)
+            v1_key = next(v1_iter, None)
+
+        # all items match so far, if lengths as the same they are equal
+        if len(v0) == len(v1):
+            return 0
+
+        if next(v1_iter, None) is not None:
+            # v1 has more items than v0
+            return 1 if sort_spec.is_desc else -1
+        # v0 has more items than v1
+        return -1 if sort_spec.is_desc else 1
+
+    @staticmethod
+    def compare_lists(rcb, v0, v1, sort_spec):
+        inner_spec = sort_spec
+        if sort_spec.is_desc or sort_spec.nones_first:
+            inner_spec = SortSpec()
+
+        # iterate over both lists
+        v0_iter = iter(v0)
+        v1_iter = iter(v1)
+
+        v0_val = next(v0_iter, None)
+        v1_val = next(v1_iter, None)
+
+        while v0_val is not None and v1_val is not None:
+            # deep compare of values
+            comp = Compare.compare_total_order(rcb, v0_val, v1_val, inner_spec)
+
+            # values don't match
+            if comp != 0:
+                return -comp if sort_spec.is_desc else comp
+
+            v0_val = next(v0_iter, None)
+            v1_val = next(v1_iter, None)
+
+        # all items match so far, if lengths as the same they are equal
+        if len(v0) == len(v1):
+            return 0
+
+        if v1_val is not None:
+            # v1 has more items than v0
+            return 1 if sort_spec.is_desc else -1
+        # v0 has more items than v1
+        return -1 if sort_spec.is_desc else 1
+
+    @staticmethod
+    def is_special_value(value):
+        if value is None or isinstance(value, JsonNone) or \
+                isinstance(value, Empty):
+            return True
+        return False
+
+    @staticmethod
+    def compare_to(this, that):
+        # same as Java compareTo
+        return (this > that) - (this < that)
 
     @staticmethod
     def hashcode(value):
         if value is None:
             return maxvalue
         if isinstance(value, JsonNone):
             return -maxvalue - 1
@@ -2477,15 +2893,15 @@
             return 1 if sort_specs[sort_pos].nones_first else -1
         if isinstance(v0, JsonNone):
             if isinstance(v1, JsonNone):
                 return 0
             return -1 if sort_specs[sort_pos].nones_first else 1
         if isinstance(v1, JsonNone):
             return 1 if sort_specs[sort_pos].nones_first else -1
-        comp = Compare.compare_atomics(rcb, v0, v1, True)
+        comp = Compare.compare_atomics_total_order(rcb, v0, v1)
         return -comp if sort_specs[sort_pos].is_desc else comp
 
     @staticmethod
     def sort_results(rcb, r0, r1, sort_fields, sort_specs):
         for i in range(len(sort_fields)):
             v0 = r0.get(sort_fields[i])
             v1 = r1.get(sort_fields[i])
@@ -2516,24 +2932,25 @@
     """
     Drives the execution of "advanced" queries at the driver and contains all
     the dynamic state needed for this execution. The state is preserved across
     the query requests submitted by the application (i.e., across batches).
     """
     QUERY_V2 = 2
     QUERY_V3 = 3
-    QUERY_VERSION = QUERY_V3
+    # query name added in V4
+    QUERY_V4 = 4
+    QUERY_VERSION = QUERY_V4
     BATCH_SIZE = 100
     DUMMY_CONT_KEY = bytearray()
 
     def __init__(self, request):
         self._client = None
         self._request = request
         request.set_driver(self)
         self._continuation_key = None
-        self._topology_info = None
         self._prep_cost = 0
         self._rcb = None
         # The max number of results the app will receive per NoSQLHandle.query()
         # invocation
         self._batch_size = (request.get_limit() if request.get_limit() > 0 else
                             QueryDriver.BATCH_SIZE)
         self._results = None
@@ -2613,45 +3030,32 @@
 
     def get_client(self):
         return self._client
 
     def get_request(self):
         return self._request
 
-    def get_shard_id(self, i):
-        return self._topology_info.get_shard_id(i)
-
-    def get_topology_info(self):
-        return self._topology_info
-
-    def num_shards(self):
-        return self._topology_info.num_shards()
-
     def set_client(self, client):
         self._client = client
 
     def set_prep_cost(self, prep_cost):
         self._prep_cost = prep_cost
 
-    def set_topology_info(self, topology_info):
-        self._topology_info = topology_info
-
     def _set_query_result(self, result):
         result.set_results(self._results)
         result.set_continuation_key(self._continuation_key)
         result.set_read_kb(self._rcb.get_read_kb())
         result.set_read_units(self._rcb.get_read_units())
         result.set_write_kb(self._rcb.get_write_kb())
         self._results = None
         self._rcb.reset_kb_consumption()
 
     def copy(self, query_request):
         copy = QueryDriver(query_request)
         copy._client = self._client
-        copy._topology_info = self._topology_info
         copy._prep_cost = self._prep_cost
         copy._results = self._results
         copy._error = self._error
         # leave _continuation_key and _rcb null to start from the beginning
         # copy._continuation_key = self._continuation_key
         # copy._rcb = self._rcb
         return copy
@@ -2707,21 +3111,25 @@
         self._iterator_states = [0] * num_iters
         self._registers = [0] * num_regs
         self._reached_limit = False
         self._read_kb = 0
         self._read_units = 0
         self._write_kb = 0
         self._memory_consumption = 0
+        self._base_topo = driver.get_client().get_topology()
         self._math_context = driver.get_request().get_math_context()
         setcontext(self._math_context)
 
     def dec_memory_consumption(self, v):
         self._memory_consumption -= v
         assert self._memory_consumption >= 0
 
+    def get_base_topo(self):
+        return self._base_topo
+
     def get_client(self):
         return self._query_driver.get_client()
 
     def get_consistency(self):
         return self.get_request().get_consistency()
 
     def get_external_var(self, var_id):
@@ -2806,30 +3214,36 @@
         self._read_units += nkb
 
     def tally_write_kb(self, nkb):
         self._write_kb += nkb
 
     @staticmethod
     def trace(msg):
+        # TODO: use request setting of log_file_trace or not, do better
+        # tracing (see Java SDK)
         print('D-QUERY: ' + msg)
 
 
 class SortSpec(object):
     """
     The order-by clause, for each sort expression allows for an optional
     'sort spec', which specifies the relative order of NULLs (less than or
     greater than all other values) and whether the values returned by the sort
     expr should be sorted in ascending or descending order.
 
     The SortSpec class stores these two pieces of information.
     """
 
-    def __init__(self, bis):
-        self.is_desc = bis.read_boolean()
-        self.nones_first = bis.read_boolean()
+    def __init__(self, bis=None):
+        if bis is not None:
+            self.is_desc = bis.read_boolean()
+            self.nones_first = bis.read_boolean()
+        else:
+            self.is_desc = False
+            self.nones_first = False
 
 
 class TopologyInfo(object):
 
     def __init__(self, seq_num, shard_ids):
         self._seq_num = seq_num
         self._shard_ids = shard_ids
@@ -2839,12 +3253,15 @@
 
     def get_shard_id(self, i):
         return self._shard_ids[i]
 
     def get_shard_ids(self):
         return self._shard_ids
 
+    def get_last_shard_id(self):
+        return self._shard_ids[self.num_shards()-1]
+
     def hash_code(self):
         return self._seq_num
 
     def num_shards(self):
         return len(self._shard_ids)
```

### Comparing `borneo-5.4.1/src/borneo/serde.py` & `borneo-5.4.2/src/borneo/serde.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from collections import OrderedDict
 from datetime import datetime
@@ -508,27 +508,26 @@
 class PrepareRequestSerializer(RequestSerializer):
 
     # Prepare a query.
     def serialize(self, request, bos, serial_version):
         BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.PREPARE)
         BinaryProtocol.serialize_request(request, bos)
         SerdeUtil.write_string(bos, request.get_statement())
-        bos.write_short_int(QueryDriver.QUERY_VERSION)
+        bos.write_short_int(request.get_query_version())
         bos.write_boolean(request.get_query_plan())
 
     def deserialize(self, request, bis, serial_version):
         result = operations.PrepareResult()
         BinaryProtocol.deserialize_consumed_capacity(bis, result)
         prep_stmt = PrepareRequestSerializer.deserialize_internal(
-            request.get_statement(), request.get_query_plan(), bis)
-        result.set_prepared_statement(prep_stmt)
+            request.get_statement(), request.get_query_plan(), result, bis)
         return result
 
     @staticmethod
-    def deserialize_internal(sql_text, get_query_plan, bis):
+    def deserialize_internal(sql_text, get_query_plan, prep_result, bis):
         """
         Extract the table name and namespace from the prepared query. This dips
         into the portion of the prepared query that is normally opaque.
 
         int (4 byte)
         byte[] (32 bytes -- hash)
         byte (number of tables)
@@ -561,18 +560,23 @@
             if length > 0:
                 external_vars = dict()
                 for i in range(length):
                     var_name = SerdeUtil.read_string(bis)
                     var_id = bis.read_int()
                     external_vars[var_name] = var_id
             topology_info = BinaryProtocol.read_topology_info(bis)
-        return PreparedStatement(
-            sql_text, query_plan, None, topology_info, proxy_statement,
+        prep = PreparedStatement(
+            sql_text, query_plan, None, proxy_statement,
             driver_plan, num_iterators, num_registers, external_vars,
             namespace, table_name, operation)
+        # NOTE: topo info is no longer in the PreparedStatement, it's in
+        # the result
+        prep_result.set_topology_info_object(topology_info)
+        prep_result.set_prepared_statement(prep)
+        return prep
 
 
 class PutRequestSerializer(RequestSerializer):
     """
     The flag indicates if the serializer is used for a standalone request or a
     sub operation of WriteMultiple request.
 
@@ -610,28 +614,32 @@
         BinaryProtocol.deserialize_generated_value(bis, result)
         return result
 
 
 class QueryRequestSerializer(RequestSerializer):
 
     def serialize(self, request, bos, serial_version):
+        if request.get_query_version() >= QueryDriver.QUERY_V4:
+            raise UnsupportedQueryVersionException(
+                'Query version ' + str(request.get_query_version()) +
+                ' is not supported by the V3 protocol')
         # write unconditional state first.
         BinaryProtocol.write_op_code(bos, SerdeUtil.OP_CODE.QUERY)
         BinaryProtocol.serialize_request(request, bos)
         bos.write_byte(request.get_consistency())
         SerdeUtil.write_packed_int(bos, request.get_limit())
         SerdeUtil.write_packed_int(bos, request.get_max_read_kb())
         SerdeUtil.write_bytearray(bos, request.get_cont_key())
         bos.write_boolean(request.is_prepared())
         # The following 7 fields were added in V2.
-        bos.write_short_int(QueryDriver.QUERY_VERSION)
+        bos.write_short_int(request.get_query_version())
         bos.write_byte(request.get_trace_level())
         SerdeUtil.write_packed_int(bos, request.get_max_write_kb())
         BinaryProtocol.write_math_context(bos, request.get_math_context())
-        SerdeUtil.write_packed_int(bos, request.topology_seq_num())
+        SerdeUtil.write_packed_int(bos, request.get_topo_seq_num())
         SerdeUtil.write_packed_int(bos, request.get_shard_id())
         bos.write_boolean(request.is_prepared() and request.is_simple_query())
         if request.is_prepared():
             ps = request.get_prepared_statement()
             SerdeUtil.write_bytearray_with_int(bos, ps.get_statement())
             if ps.get_variables() is not None:
                 variables = ps.get_variables()
@@ -669,33 +677,32 @@
         BinaryProtocol.deserialize_consumed_capacity(bis, result)
         result.set_continuation_key(SerdeUtil.read_bytearray(bis, False))
         request.set_cont_key(result.get_continuation_key())
         # In V2, if the QueryRequest was not initially prepared, the prepared
         # statement created at the proxy is returned back along with the query
         # results, so that the preparation does not need to be done during each
         # query batch.
+        prep_result = None
         if not is_prepared:
+            prep_result = operations.PrepareResult()
             prep = PrepareRequestSerializer.deserialize_internal(
-                request.get_statement(), False, bis)
+                request.get_statement(), False, prep_result, bis)
             request.set_prepared_statement(prep)
         if prep is not None and not prep.is_simple_query():
             if not is_prepared:
                 assert num_rows == 0
                 driver = QueryDriver(request)
-                driver.set_topology_info(prep.topology_info())
                 driver.set_prep_cost(result.get_read_kb())
                 result.set_computed(False)
+                result.set_topology_info_object(prep_result.get_topology_info())
             else:
                 # In this case, the QueryRequest is an "internal" one.
                 result.set_reached_limit(bis.read_boolean())
                 topology_info = BinaryProtocol.read_topology_info(bis)
-                driver = request.get_driver()
-                if topology_info is not None:
-                    prep.set_topology_info(topology_info)
-                    driver.set_topology_info(topology_info)
+                result.set_topology_info_object(topology_info)
         else:
             results = SerdeUtil.convert_value_to_none(results)
         result.set_results(results)
         return result
 
 
 class SystemRequestSerializer(RequestSerializer):
```

### Comparing `borneo-5.4.1/src/borneo/serdeutil.py` & `borneo-5.4.2/src/borneo/serdeutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 from abc import ABCMeta, abstractmethod
 from datetime import datetime
@@ -21,17 +21,17 @@
     EvolutionLimitException, IllegalArgumentException, IllegalStateException,
     IndexExistsException, IndexLimitException, IndexNotFoundException,
     InvalidAuthorizationException, KeySizeLimitException, NoSQLException,
     OperationNotSupportedException, OperationThrottlingException,
     ReadThrottlingException, RequestSizeLimitException, RequestTimeoutException,
     ResourceExistsException, ResourceNotFoundException, RowSizeLimitException,
     SecurityInfoNotReadyException, SystemException, TableExistsException,
-    TableLimitException, TableNotFoundException, TableSizeException,
-    UnauthorizedException, UnsupportedProtocolException,
-    WriteThrottlingException)
+    TableLimitException, TableNotFoundException, TableNotReadyException,
+    TableSizeException, UnauthorizedException, UnsupportedQueryVersionException,
+    UnsupportedProtocolException, WriteThrottlingException)
 
 from .kv.exception import AuthenticationException
 
 
 #
 # Abstract classes/interfaces related to serialization
 #
@@ -140,14 +140,15 @@
         pass
 
     @abstractmethod
     def stop(self):
         pass
 
 
+# noinspection PyTypeChecker
 class SerdeUtil(object):
     """
     A class to encapsulte static methods used by serialization and
     deserialization of requests. These utility methods can be used by
     multiple protocols. It also includes constants that are shared across
     protocols.
     """
@@ -195,15 +196,19 @@
                    CREATE_TABLE=18,
                    ALTER_TABLE=19,
                    DROP_TABLE=20,
                    CREATE_INDEX=21,
                    DROP_INDEX=22,
                    # added in V2.
                    SYSTEM_REQUEST=23,
-                   SYSTEM_STATUS_REQUEST=24)
+                   SYSTEM_STATUS_REQUEST=24,
+                   # skip some as unused
+                   ADD_REPLICA=33,
+                   DROP_REPLICA=34,
+                   GET_REPLICA_STATS=35)
 
     # System Operation state.
     SYSTEM_STATE = enum(COMPLETE=0,
                         WORKING=1)
 
     # Table state.
     TABLE_STATE = enum(ACTIVE=0,
@@ -238,15 +243,18 @@
                       TABLE_DEPLOYMENT_LIMIT_EXCEEDED=19,
                       TENANT_DEPLOYMENT_LIMIT_EXCEEDED=20,
                       # added in V2.
                       OPERATION_NOT_SUPPORTED=21,
                       ETAG_MISMATCH=22,
                       CANNOT_CANCEL_WORK_REQUEST=23,
                       # added in V3
-                      UNSUPPORTED_PROTOCOL=24)
+                      UNSUPPORTED_PROTOCOL=24,
+                      # added in V4
+                      TABLE_NOT_READY=26,
+                      UNSUPPORTED_QUERY_VERSION=27)
 
     # Error codes for user throttling, range from 50 to 100(exclusive).
     THROTTLING_ERROR = enum(READ_LIMIT_EXCEEDED=50,
                             WRITE_LIMIT_EXCEEDED=51,
                             SIZE_LIMIT_EXCEEDED=52,
                             OPERATION_LIMIT_EXCEEDED=53)
 
@@ -272,14 +280,16 @@
 
     """
     in V3 and above, TableLimits includes a mode
     """
     CAPACITY_MODE = enum(PROVISIONED=1,
                          ON_DEMAND=2)
 
+    # this method always copies. consider a more efficient mechanism
+    # for cases where no conversion is required
     @staticmethod
     def convert_value_to_none(value):
         if isinstance(value, dict):
             return {key: SerdeUtil.convert_value_to_none(val)
                     for (key, val) in value.items()}
         if isinstance(value, list):
             return [SerdeUtil.convert_value_to_none(val) for val in
@@ -339,14 +349,18 @@
         elif code == SerdeUtil.THROTTLING_ERROR.READ_LIMIT_EXCEEDED:
             return ReadThrottlingException(msg)
         elif code == SerdeUtil.THROTTLING_ERROR.SIZE_LIMIT_EXCEEDED:
             return TableSizeException(msg)
         elif code == SerdeUtil.THROTTLING_ERROR.WRITE_LIMIT_EXCEEDED:
             return WriteThrottlingException(msg)
         elif code == SerdeUtil.USER_ERROR.BAD_PROTOCOL_MESSAGE:
+            # newer proxies will return USER_ERROR.UNSUPPORTED_QUERY_VERSION
+            # but older ones don't have that error but do have a defined string
+            if 'Invalid query version' in msg:
+                return UnsupportedQueryVersionException(msg)
             # V2 proxy will return this message if V3 is used in the driver
             if "Invalid driver serial version" in msg:
                 return UnsupportedProtocolException(msg)
             return IllegalArgumentException('Bad protocol message: ' + msg)
         elif (code ==
               SerdeUtil.USER_ERROR.BATCH_OP_NUMBER_LIMIT_EXCEEDED):
             return BatchOperationNumberLimitException(msg)
@@ -385,14 +399,20 @@
             return TableNotFoundException(msg)
         elif (code == SerdeUtil.USER_ERROR.TABLE_DEPLOYMENT_LIMIT_EXCEEDED
               or code == (
                       SerdeUtil.USER_ERROR.TENANT_DEPLOYMENT_LIMIT_EXCEEDED)):
             return DeploymentException(msg)
         elif code == SerdeUtil.USER_ERROR.UNSUPPORTED_PROTOCOL:
             return UnsupportedProtocolException(msg)
+        elif code == SerdeUtil.USER_ERROR.UNSUPPORTED_QUERY_VERSION:
+            return UnsupportedQueryVersionException(msg)
+        elif code == SerdeUtil.USER_ERROR.TABLE_NOT_READY:
+            return TableNotReadyException(msg)
+        elif code == SerdeUtil.USER_ERROR.ETAG_MISMATCH:
+            return IllegalArgumentException(msg)
         else:
             return NoSQLException(
                 'Unknown error code ' + str(code) + ': ' + msg)
 
     @staticmethod
     def read_bytearray(bis, skip):
         """
@@ -815,14 +835,16 @@
             return SerdeUtil.FIELD_VALUE_TYPE.TIMESTAMP
         elif isinstance(value, Decimal) or CheckValue.is_overlong(value):
             return SerdeUtil.FIELD_VALUE_TYPE.NUMBER
         elif value is None:
             return SerdeUtil.FIELD_VALUE_TYPE.NULL
         elif isinstance(value, Empty):
             return SerdeUtil.FIELD_VALUE_TYPE.EMPTY
+        elif isinstance(value, JsonNone):
+            return SerdeUtil.FIELD_VALUE_TYPE.JSON_NULL
         else:
             raise IllegalStateException(
                 'Unknown value type ' + str(type(value)))
 
     #
     # If the stream isn't pointing at an NSON Map there's a problem in the
     # message. The caller will handle it if a non-zero value is returned
```

### Comparing `borneo-5.4.1/src/borneo/stats.py` & `borneo-5.4.2/src/borneo/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
 #
 # Licensed under the Universal Permissive License v 1.0 as shown at
 #  https://oss.oracle.com/licenses/upl/
 #
 
 import pprint
 import sys
@@ -58,15 +58,15 @@
 
     Collection of stats can also be used by using the API:
 
     :py:meth:`NoSQLHandleConfig.set_stats_profile` or
     :py:meth:`StatsControl.set_profile`. At runtime stats collection can be
     enabled selectively by using :py:meth:`StatsControl.start` ond
     :py:meth:`StatsControl.stop`. The following example shows how to use a stats
-    handler and how to control the stas at runtime::
+    handler and how to control the stats at runtime::
 
         def stats_handler(stats):
             # type: (Dict) -> None
             print("Stats : " + str(stats))
         ...
         config = NoSQLHandleConfig( endpoint )
         config.set_stats_profile(StatsProfile.REGULAR)
```

### Comparing `borneo-5.4.1/src/borneo.egg-info/PKG-INFO` & `borneo-5.4.2/src/borneo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borneo
-Version: 5.4.1
+Version: 5.4.2
 Summary: Oracle NoSQL Database Python SDK
 Home-page: https://nosql-python-sdk.readthedocs.io/en/stable/index.html
 Author: Oracle
 Author-email: george.feinberg@oracle.com
 License: Universal Permissive License 1.0
 Keywords: database,nosql,cloud,development
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,108 +14,82 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Oracle NoSQL Database Python SDK
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+# Oracle NoSQL Database Python SDK
 
-=====
-About
-=====
+## About
 
 This is the Python SDK for Oracle NoSQL Database. Python versions 3.5+ are
 supported. The SDK provides interfaces, documentation, and examples to help
 develop Python applications that connect to the Oracle NoSQL Database Cloud
 Service, Oracle NoSQL Database and to the Oracle NoSQL Cloud Simulator (which
 runs on a local machine).
 
 In order to run the Oracle NoSQL Cloud Simulator, a separate download is
 necessary from the Oracle NoSQL OTN download page. Throughout the documentation,
 the Oracle NoSQL Database Cloud Service and Cloud Simulator are referred to as
 the "cloud service" while the Oracle NoSQL Database is referred to as
-"on-premise." In the `API reference <https://nosql-python-sdk.readthedocs.io/en/
-stable/api.html>`_ classes and interfaces are noted if they are only relevant to
+"on-premise." In the [API reference](https://nosql-python-sdk.readthedocs.io/en/stable/api.html) classes and interfaces are noted if they are only relevant to
 a specific environment.
 
 The on-premise configuration requires a running instance of the Oracle NoSQL
-database. In addition a running proxy service is required. See `Oracle NoSQL
-Database Downloads <https://www.oracle.com/database/technologies/nosql-database-
-server-downloads.html>`_ for downloads, and see `Information about the proxy
-<https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-
-database/22.3/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72>`_ for
+database. In addition a running proxy service is required. See [Oracle NoSQL
+Database Downloads](https://www.oracle.com/database/technologies/nosql-database-server-downloads.html) for downloads, and see [Information about the proxy](https://docs.oracle.com/pls/topic/lookup?ctx=en/database/other-databases/nosql-database/22.3/admin&id=NSADM-GUID-C110AF57-8B35-4C48-A82E-2621C6A5ED72)  for
 proxy configuration information.
 
 This project is open source and maintained by Oracle Corp. The home page for the
-project is `here <https://nosql-python-sdk.readthedocs.io/en/stable/index.
-html>`_.
+project is [here](https://nosql-python-sdk.readthedocs.io/en/stable/index.html).
 
-============
-Installation
-============
+## Installation
 
 The SDK can be installed using pip. If using Python 3 the command may be pip3::
 
     pip install borneo
 
 If you are using the Oracle NoSQL Database cloud service you will also need to
 install the oci package::
 
     pip install oci
 
-See `the installation guide <https://nosql-python-sdk.readthedocs.io/en/stable/
-installation.html>`_ for additional requirements and and alternative install
+See [the installation guide](https://nosql-python-sdk.readthedocs.io/en/stable/installation.html) for additional requirements and and alternative install
 methods.
 
-========
-Examples
-========
+## Examples
 
-Examples can be found `on GitHub <https://github.com/oracle/nosql-python-sdk/
-tree/master/examples>`_.
+Examples can be found [on GitHub](https://github.com/oracle/nosql-python-sdk/tree/master/examples)
 
 Examples include simple, standalone programs. They include comments about how
 they can be configured and run in the different supported environments.
 
-=============
-Documentation
-=============
-
-The `documentation <https://nosql-python-sdk.readthedocs.io/en/stable>`_ has
-information on using the SDK as well as an `API reference <https://nosql-python-
-sdk.readthedocs.io/en/stable/api.html>`_ describing the classes.
-
-=======
-Changes
-=======
-
-See the `Changelog <https://github.com/oracle/nosql-python-sdk/blob/master/
-CHANGELOG.rst>`_.
-
-====
-Help
-====
+## Documentation
 
- * Open an issue in the `Issues <https://github.com/oracle/nosql-python-sdk/
-   issues>`_ page.
+The [documentation](https://nosql-python-sdk.readthedocs.io/en/stable) has
+information on using the SDK as well as an [API reference](https://nosql-python-sdk.readthedocs.io/en/stable/api.html) describing the classes.
+
+## Changes
+
+See the [Changelog](https://github.com/oracle/nosql-python-sdk/blob/master/CHANGELOG.md)
+
+## Help
+
+ * Open an issue in the [Issues](https://github.com/oracle/nosql-python-sdk/issues) page.
  * Email to nosql_sdk_help_grp@oracle.com.
- * `Oracle NoSQL Developer Forum <https://community.oracle.com/community/
-   groundbreakers/database/nosql_database>`_.
+ * [Oracle NoSQL Developer Forum](https://community.oracle.com/community/groundbreakers/database/nosql_database).
 
 When requesting help please be sure to include as much detail as possible,
 including version of the SDK and **simple**, standalone example code as needed.
 
-==========
-Quickstart
-==========
+## Quickstart
 
 The following is a quick start tutorial to run a simple program in the supported
 environments. The same template source code is used for all environments. The
 first step is to cut the program below and paste it into an editor for minor
 modifications. The instructions assume that is stored as quickstart.py, but you
 can use any name you like. The quickstart example supports 3 environments:
 
@@ -123,275 +97,272 @@
 2. Oracle NoSQL Cloud Simulator
 3. Oracle NoSQL Database on-premise, using the proxy server
 
 See `Running Quickstart`_ to
 run the quickstart program in different environments. The instructions assume
 that the *borneo* package has been installed.
 
-.. code-block:: pycon
-
-    #
-    # Copyright (c) 2018, 2022 Oracle and/or its affiliates. All rights reserved.
-    #
-    # Licensed under the Universal Permissive License v 1.0 as shown at
-    #  https://oss.oracle.com/licenses/upl/
-    #
-
-    #
-    # This is a simple quickstart to demonstrate use of the Python driver for
-    # the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
-    # Database Cloud Service, against the Cloud Simulator, or against an
-    # on-premise Oracle NoSQL database.
-    #
-    # Usage:
-    #   python quickstart.py <cloud | cloudsim | kvstore>
-    #
-    # Use cloud for the Cloud Service
-    # Use cloudsim for the Cloud Simulator
-    # Use kvstore for the on-premise database
-    #
-    # This example is not intended to be an exhaustive overview of the API,
-    # which has a number of additional operations.
-    #
-    # Requirements:
-    #  1. Python 3.5+
-    #  2. Python dependencies (install using pip or other mechanism):
-    #   o requests
-    #   o oci (only if running against the Cloud Service)
-    #  3. If running against the Cloud Simulator, it can be downloaded from
-    #  here:
-    #   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
-    #  It requires Java
-    #  4. If running against the Oracle NoSQL Database Cloud Service an account
-    #  must be used.
-    #
-
-    import sys
-
-    from borneo import (
-        AuthorizationProvider, DeleteRequest, GetRequest,
-        IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
-        QueryRequest, Regions, TableLimits, TableRequest)
-    from borneo.iam import SignatureProvider
-    from borneo.kv import StoreAccessTokenProvider
-
-
-    #
-    # EDIT: these values based on desired region and/or endpoint for a local
-    # server
-    #
-    cloud_region = Regions.EU_ZURICH_1
-    cloudsim_endpoint = 'localhost:8080'
-    kvstore_endpoint = 'localhost:80'
-    cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
-
-    # Cloud Service Only
-    #
-    # EDIT: set these variables to the credentials to use if you are not using
-    # a configuration file in ~/.oci/config
-    # Use of these credentials vs a file is determined by a value of tenancy
-    # other than None.
-    #
-    tenancy = None  # tenancy'd OCID (string)
-    user = None  # user's OCID (string)
-    private_key = 'path-to-private-key-or-private-key-content'
-    fingerprint = 'fingerprint for uploaded public key'
-    # pass phrase (string) for private key, or None if not set
-    pass_phrase = None
-
-
-    class CloudsimAuthorizationProvider(AuthorizationProvider):
-        """
-        Cloud Simulator Only.
-
-        This class is used as an AuthorizationProvider when using the Cloud
-        Simulator, which has no security configuration. It accepts a string
-        tenant_id that is used as a simple namespace for tables.
-        """
-
-        def __init__(self, tenant_id):
-            super(CloudsimAuthorizationProvider, self).__init__()
-            self._tenant_id = tenant_id
-
-        def close(self):
-            pass
-
-        def get_authorization_string(self, request=None):
-            return 'Bearer ' + self._tenant_id
-
-
-    def get_handle(nosql_env):
-        """
-        Returns a NoSQLHandle based on the requested environment. The
-        differences among the supported environments are encapsulated in this
-        method.
-        """
-        if nosql_env == 'cloud':
-            endpoint = cloud_region
-            #
-            # Get credentials using SignatureProvider. SignatureProvider has
-            # several ways to accept credentials. See the documentation:
-            #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
-            #
-            if tenancy is not None:
-                print('Using directly provided credentials')
-                #
-                # Credentials are provided directly
-                #
-                provider = SignatureProvider(tenant_id=tenancy,
-                                             user_id=user,
-                                             fingerprint=fingerprint,
-                                             private_key=private_key,
-                                             pass_phrase=pass_phrase)
-            else:
-                #
-                # Credentials will come from a file.
-                #
-                # By default the file is ~/.oci/config. A config_file = <path>
-                # argument can be passed to specify a different file.
-                #
-                print('Using credentials and DEFAULT profile from ' +
-                      '~/.oci/config')
-                provider = SignatureProvider()
-        elif nosql_env == 'cloudsim':
-            print('Using cloud simulator endpoint ' + cloudsim_endpoint)
-            endpoint = cloudsim_endpoint
-            provider = CloudsimAuthorizationProvider(cloudsim_id)
-
-        elif nosql_env == 'kvstore':
-            print('Using on-premise endpoint ' + kvstore_endpoint)
-            endpoint = kvstore_endpoint
-            provider = StoreAccessTokenProvider()
+``` python
 
+#
+# Copyright (c) 2018, 2024 Oracle and/or its affiliates. All rights reserved.
+#
+# Licensed under the Universal Permissive License v 1.0 as shown at
+#  https://oss.oracle.com/licenses/upl/
+#
+
+#
+# This is a simple quickstart to demonstrate use of the Python driver for
+# the Oracle NoSQL Database. It can be used to run against the Oracle NoSQL
+# Database Cloud Service, against the Cloud Simulator, or against an
+# on-premise Oracle NoSQL database.
+#
+# Usage:
+#   python quickstart.py <cloud | cloudsim | kvstore>
+#
+# Use cloud for the Cloud Service
+# Use cloudsim for the Cloud Simulator
+# Use kvstore for the on-premise database
+#
+# This example is not intended to be an exhaustive overview of the API,
+# which has a number of additional operations.
+#
+# Requirements:
+#  1. Python 3.5+
+#  2. Python dependencies (install using pip or other mechanism):
+#   o requests
+#   o oci (only if running against the Cloud Service)
+#  3. If running against the Cloud Simulator, it can be downloaded from
+#  here:
+#   http://www.oracle.com/technetwork/topics/cloud/downloads/index.html
+#  It requires Java
+#  4. If running against the Oracle NoSQL Database Cloud Service an account
+#  must be used.
+#
+
+import sys
+
+from borneo import (
+    AuthorizationProvider, DeleteRequest, GetRequest,
+    IllegalArgumentException, NoSQLHandle, NoSQLHandleConfig, PutRequest,
+    QueryRequest, Regions, TableLimits, TableRequest)
+from borneo.iam import SignatureProvider
+from borneo.kv import StoreAccessTokenProvider
+
+
+#
+# EDIT: these values based on desired region and/or endpoint for a local
+# server
+#
+cloud_region = Regions.EU_ZURICH_1
+cloudsim_endpoint = 'localhost:8080'
+kvstore_endpoint = 'localhost:80'
+cloudsim_id = 'cloudsim'  # a fake user id/namespace for the Cloud Simulator
+
+# Cloud Service Only
+#
+# EDIT: set these variables to the credentials to use if you are not using
+# a configuration file in ~/.oci/config
+# Use of these credentials vs a file is determined by a value of tenancy
+# other than None.
+#
+tenancy = None  # tenancy'd OCID (string)
+user = None  # user's OCID (string)
+private_key = 'path-to-private-key-or-private-key-content'
+fingerprint = 'fingerprint for uploaded public key'
+# pass phrase (string) for private key, or None if not set
+pass_phrase = None
+
+
+class CloudsimAuthorizationProvider(AuthorizationProvider):
+    """
+    Cloud Simulator Only.
+
+    This class is used as an AuthorizationProvider when using the Cloud
+    Simulator, which has no security configuration. It accepts a string
+    tenant_id that is used as a simple namespace for tables.
+    """
+
+    def __init__(self, tenant_id):
+        super(CloudsimAuthorizationProvider, self).__init__()
+        self._tenant_id = tenant_id
+
+    def close(self):
+        pass
+
+    def get_authorization_string(self, request=None):
+        return 'Bearer ' + self._tenant_id
+
+
+def get_handle(nosql_env):
+    """
+    Returns a NoSQLHandle based on the requested environment. The
+    differences among the supported environments are encapsulated in this
+    method.
+    """
+    if nosql_env == 'cloud':
+        endpoint = cloud_region
+        #
+        # Get credentials using SignatureProvider. SignatureProvider has
+        # several ways to accept credentials. See the documentation:
+        #  https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.iam.SignatureProvider.html
+        #
+        if tenancy is not None:
+            print('Using directly provided credentials')
+            #
+            # Credentials are provided directly
+            #
+            provider = SignatureProvider(tenant_id=tenancy,
+                                         user_id=user,
+                                         fingerprint=fingerprint,
+                                         private_key=private_key,
+                                         pass_phrase=pass_phrase)
         else:
-            raise IllegalArgumentException('Unknown environment: ' + nosql_env)
-
-        return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
-
-
-    def main():
-
-        table_name = 'PythonQuickstart'
-
-        if len(sys.argv) != 2:
-            print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
-            raise SystemExit
-
-        nosql_env = sys.argv[1:][0]
-        print('Using environment: ' + str(nosql_env))
-
-        handle = None
-        try:
-
-            #
-            # Create a handle
             #
-            handle = get_handle(nosql_env)
-
+            # Credentials will come from a file.
             #
-            # Create a table
-            #
-            statement = (
-                'Create table if not exists {} (id integer, sid integer, ' +
-                'name string, primary key(shard(sid), id))').format(table_name)
-            request = TableRequest().set_statement(statement).set_table_limits(
-                TableLimits(30, 10, 1))
-            handle.do_table_request(request, 50000, 3000)
-            print('After create table')
-
-            #
-            # Put a few rows
-            #
-            request = PutRequest().set_table_name(table_name)
-            for i in range(10):
-                value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
-                request.set_value(value)
-                handle.put(request)
-            print('After put of 10 rows')
-
+            # By default the file is ~/.oci/config. A config_file = <path>
+            # argument can be passed to specify a different file.
             #
-            # Get the row
-            #
-            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                table_name)
-            result = handle.get(request)
-            print('After get: ' + str(result))
-
-            #
-            # Query, using a range
-            #
-            statement = (
-                'select * from ' + table_name + ' where id > 2 and id < 8')
-            request = QueryRequest().set_statement(statement)
-            print('Query results for: ' + statement)
-            #
-            # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
-            # may be more results, so queries should generally be run in a loop.
-            # It is possible for single request to return no results but the
-            # query still not done, indicating that the query loop should
-            # continue.
-            #
-            while True:
-                result = handle.query(request)
-                for r in result.get_results():
-                    print('\t' + str(r))
-                if request.is_done():
-                    break
-
-            #
-            # Delete the row
-            #
-            request = DeleteRequest().set_table_name(table_name).set_key(
-                {'id': 1, 'sid': 0})
-            result = handle.delete(request)
-            print('After delete: ' + str(result))
-
-            #
-            # Get again to show deletion
-            #
-            request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
-                table_name)
-            result = handle.get(request)
-            print('After get (should be None): ' + str(result))
-
-            #
-            # Drop the table
-            #
-            request = TableRequest().set_statement(
-                'drop table if exists {} '.format(table_name))
-            result = handle.table_request(request)
-
-            #
-            # Table drop can take time, depending on the state of the system.
-            # If this wait fails the table will still probably been dropped
-            #
-            result.wait_for_completion(handle, 40000, 2000)
-            print('After drop table')
-
-            print('Quickstart is complete')
-        except Exception as e:
-            print(e)
-        finally:
-            # If the handle isn't closed Python will not exit properly
-            if handle is not None:
-                handle.close()
-
-
-    if __name__ == '__main__':
-        main()
-
-Running Quickstart
-==================
+            print('Using credentials and DEFAULT profile from ' +
+                  '~/.oci/config')
+            provider = SignatureProvider()
+    elif nosql_env == 'cloudsim':
+        print('Using cloud simulator endpoint ' + cloudsim_endpoint)
+        endpoint = cloudsim_endpoint
+        provider = CloudsimAuthorizationProvider(cloudsim_id)
+
+    elif nosql_env == 'kvstore':
+        print('Using on-premise endpoint ' + kvstore_endpoint)
+        endpoint = kvstore_endpoint
+        provider = StoreAccessTokenProvider()
+
+    else:
+        raise IllegalArgumentException('Unknown environment: ' + nosql_env)
+
+    return NoSQLHandle(NoSQLHandleConfig(endpoint, provider))
+
+
+def main():
+
+    table_name = 'PythonQuickstart'
+
+    if len(sys.argv) != 2:
+        print('Usage: python quickstart.py <cloud | cloudsim | kvstore>')
+        raise SystemExit
+
+    nosql_env = sys.argv[1:][0]
+    print('Using environment: ' + str(nosql_env))
+
+    handle = None
+    try:
+
+        #
+        # Create a handle
+        #
+        handle = get_handle(nosql_env)
+
+        #
+        # Create a table
+        #
+        statement = (
+            'Create table if not exists {} (id integer, sid integer, ' +
+            'name string, primary key(shard(sid), id))').format(table_name)
+        request = TableRequest().set_statement(statement).set_table_limits(
+            TableLimits(30, 10, 1))
+        handle.do_table_request(request, 50000, 3000)
+        print('After create table')
+
+        #
+        # Put a few rows
+        #
+        request = PutRequest().set_table_name(table_name)
+        for i in range(10):
+            value = {'id': i, 'sid': 0, 'name': 'myname' + str(i)}
+            request.set_value(value)
+            handle.put(request)
+        print('After put of 10 rows')
+
+        #
+        # Get the row
+        #
+        request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+            table_name)
+        result = handle.get(request)
+        print('After get: ' + str(result))
+
+        #
+        # Query, using a range
+        #
+        statement = (
+            'select * from ' + table_name + ' where id > 2 and id < 8')
+        request = QueryRequest().set_statement(statement)
+        print('Query results for: ' + statement)
+        #
+        # If the :py:meth:`borneo.QueryRequest.is_done` returns False, there
+        # may be more results, so queries should generally be run in a loop.
+        # It is possible for single request to return no results but the
+        # query still not done, indicating that the query loop should
+        # continue.
+        #
+        while True:
+            result = handle.query(request)
+            for r in result.get_results():
+                print('\t' + str(r))
+            if request.is_done():
+                break
+
+        #
+        # Delete the row
+        #
+        request = DeleteRequest().set_table_name(table_name).set_key(
+            {'id': 1, 'sid': 0})
+        result = handle.delete(request)
+        print('After delete: ' + str(result))
+
+        #
+        # Get again to show deletion
+        #
+        request = GetRequest().set_key({'id': 1, 'sid': 0}).set_table_name(
+            table_name)
+        result = handle.get(request)
+        print('After get (should be None): ' + str(result))
+
+        #
+        # Drop the table
+        #
+        request = TableRequest().set_statement(
+            'drop table if exists {} '.format(table_name))
+        result = handle.table_request(request)
+
+        #
+        # Table drop can take time, depending on the state of the system.
+        # If this wait fails the table will still probably been dropped
+        #
+        result.wait_for_completion(handle, 40000, 2000)
+        print('After drop table')
+
+        print('Quickstart is complete')
+    except Exception as e:
+        print(e)
+    finally:
+        # If the handle isn't closed Python will not exit properly
+        if handle is not None:
+            handle.close()
+
+
+if __name__ == '__main__':
+    main()
+```
+## Running Quickstart
 
-Run Against the Oracle NoSQL Database Cloud Service
-===================================================
+### Run Against the Oracle NoSQL Database Cloud Service
 
 Running against the Cloud Service requires an Oracle Cloud account. See
-`Configure for the Cloud Service <https://nosql-python-sdk.readthedocs.io/en/
-stable/installation.html#configure-for-the-cloud-service>`_ for information on
+[Configure for the Cloud Service](https://nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-the-cloud-service) for information on
 getting an account and acquiring required credentials.
 
 1. Collect the following information:
 
  * Tenancy ID
  * User ID
  * API signing key (private key file in PEM format)
@@ -402,64 +373,59 @@
    credentials in the program:
 
    * Directly provide the credential information. To use this method, modify the
      values of the variables at the top of the program: *tenancy*, *user*,
      *private_key*, *fingerprint*, and *pass_phrase*, setting them to the
      corresponding information you've collected.
    * Using a configuration file. In this case the information you've collected
-     goes into a file, ~/.oci/config. `Configure for the Cloud Service <https://
-     nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-
-     the-cloud-service>`_ describes the contents of the file. It will look like
+     goes into a file, ~/.oci/config. [Configure for the Cloud Service](https://nosql-python-sdk.readthedocs.io/en/stable/installation.html#configure-for-the-cloud-service) describes the contents of the file. It will look like
      this::
 
       [DEFAULT]
       tenancy=<your-tenancy-id>
       user=<your-user-id>
       fingerprint=<fingerprint-of-your-public-key>
       key_file=<path-to-your-private-key-file>
       pass_phrase=<optional-pass-phrase-for-key-file>
 
 3. Decide which region you want to use and modify the *cloud_region* variable to
-   the desired region. See `Regions documentation <https://nosql-python-sdk.
-   readthedocs.io/en/stable/api/borneo.Regions.html>`_ for possible regions. Not
+   the desired region. See [Regions documentation](https://nosql-python-sdk.readthedocs.io/en/stable/api/borneo.Regions.html) for possible regions. Not
    all support the Oracle NoSQL Database Cloud Service.
 
 4. Run the program:
 
 .. code-block:: pycon
 
     python quickstart.py cloud
 
-Run Against the Oracle NoSQL Cloud Simulator
-============================================
+### Run Against the Oracle NoSQL Cloud Simulator
 
 Running against the Oracle NoSQL Cloud Simulator requires a running Cloud
-Simulator instance. See `Configure for the Cloud Simulator <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator>`_ for information on how to
+Simulator instance. See [Configure for the Cloud Simulator](https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-cloud-simulator) for information on how to
 download and start the Cloud Simulator.
 
 1. Start the Cloud Simulator based on instructions above. Note the HTTP port
    used. By default it is *8080* on *localhost*.
 
 2. The *quickstart.py* program defaults to *localhost:8080* so if the Cloud
    Simulator was started using default values no editing is required.
 
 3. Run the program:
 
 .. code-block:: pycon
 
     python quickstart.py cloudsim
 
-Run Against Oracle NoSQL on-premise
-===================================
+### Run Against Oracle NoSQL on-premise
 
 Running against the Oracle NoSQL Database on-premise requires a running Oracle
 NoSQL Database instance as well as a running NoSQL Proxy server instance. The
 program will connect to the proxy server.
 
-See `Configure for On-Premise Oracle NoSQL Database <https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database>`_ for information on how to
+See [Configure for On-Premise Oracle NoSQL Database](https://nosql-python-sdk.readthedocs.io/en/latest/installation.html#configure-for-the-on-premise-oracle-nosql-database) for information on how to
 download and start the database instance and proxy server. The database and
 proxy should be started without security enabled for this quickstart program to
 operate correctly. A secure configuration requires a secure proxy and more
 complex configuration.
 
 1. Start the Oracle NoSQL Database and proxy server based on instructions above.
    Note the HTTP port used. By default the endpoint is *localhost:80*.
@@ -469,27 +435,21 @@
 
 3. Run the program:
 
 .. code-block:: pycon
 
     python quickstart.py kvstore
 
-=======
-License
-=======
+## Contributing
 
-Copyright (C) 2018, 2023 Oracle and/or its affiliates. All rights reserved.
+This project welcomes contributions from the community. Before submitting a pull request, please [review our contribution guide](./CONTRIBUTING.md)
 
-This SDK is licensed under the Universal Permissive License 1.0. See `LICENSE
-<./LICENSE.txt>`_ for details.
+## Security
 
-============
-Contributing
-============
+Please consult the [security guide](./SECURITY.md) for our responsible security vulnerability disclosure process
 
-See `CONTRIBUTING <./CONTRIBUTING.rst>`_
+## License
 
-========
-Security
-========
+Copyright (c) 2018, 2024 Oracle and/or its affiliates.
 
-See `SECURITY <./SECURITY.rst>`_
+Released under the Universal Permissive License v1.0 as shown at
+<https://oss.oracle.com/licenses/upl/>.
```

### Comparing `borneo-5.4.1/src/borneo.egg-info/SOURCES.txt` & `borneo-5.4.2/src/borneo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-CHANGELOG.rst
+CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
-README.rst
+README.md
 THIRD_PARTY_LICENSES.txt
 setup.py
 src/borneo/__init__.py
 src/borneo/auth.py
 src/borneo/client.py
 src/borneo/common.py
 src/borneo/config.py
```

