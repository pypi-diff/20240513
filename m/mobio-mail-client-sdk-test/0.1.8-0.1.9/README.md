# Comparing `tmp/mobio-mail-client-sdk-test-0.1.8.tar.gz` & `tmp/mobio-mail-client-sdk-test-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-mail-client-sdk-test-0.1.8.tar", last modified: Thu Jan  4 10:25:19 2024, max compression
+gzip compressed data, was "mobio-mail-client-sdk-test-0.1.9.tar", last modified: Thu Jan  4 10:48:22 2024, max compression
```

## Comparing `mobio-mail-client-sdk-test-0.1.8.tar` & `mobio-mail-client-sdk-test-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:25:19.053370 mobio-mail-client-sdk-test-0.1.8/
--rw-r--r--   0 root         (0) root         (0)     1293 2024-01-04 10:25:19.053370 mobio-mail-client-sdk-test-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:25:19.020369 mobio-mail-client-sdk-test-0.1.8/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:25:19.021369 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:25:19.034370 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/
--rw-r--r--   0 root         (0) root         (0)      384 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1415 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/consts.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/errors.py
--rw-r--r--   0 root         (0) root         (0)     7054 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/folder.py
--rw-r--r--   0 root         (0) root         (0)     2059 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/imap_utf7.py
--rw-r--r--   0 root         (0) root         (0)    17294 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/mailbox.py
--rw-r--r--   0 root         (0) root         (0)    10754 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/message.py
--rw-r--r--   0 root         (0) root         (0)    16182 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:25:19.038370 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/
--rw-r--r--   0 root         (0) root         (0)      292 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       95 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/constants.py
--rw-r--r--   0 root         (0) root         (0)     7680 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/html_quotations.py
--rw-r--r--   0 root         (0) root         (0)    21157 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/quotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:25:19.041370 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/
--rw-r--r--   0 root         (0) root         (0)     1242 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5840 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/bruteforce.py
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:25:19.042370 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/data/
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3288 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/extraction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:25:19.046370 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2124 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/classifier.py
--rw-r--r--   0 root         (0) root         (0)     6068 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/dataset.py
--rw-r--r--   0 root         (0) root         (0)     3059 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/featurespace.py
--rw-r--r--   0 root         (0) root         (0)     6804 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/helpers.py
--rw-r--r--   0 root         (0) root         (0)     4327 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/utils.py
--rw-r--r--   0 root         (0) root         (0)     7389 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:25:19.052370 mobio-mail-client-sdk-test-0.1.8/mobio_mail_client_sdk_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1293 2024-01-04 10:25:18.000000 mobio-mail-client-sdk-test-0.1.8/mobio_mail_client_sdk_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1375 2024-01-04 10:25:18.000000 mobio-mail-client-sdk-test-0.1.8/mobio_mail_client_sdk_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-04 10:25:18.000000 mobio-mail-client-sdk-test-0.1.8/mobio_mail_client_sdk_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-01-04 10:25:18.000000 mobio-mail-client-sdk-test-0.1.8/mobio_mail_client_sdk_test.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-01-04 10:25:18.000000 mobio-mail-client-sdk-test-0.1.8/mobio_mail_client_sdk_test.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-04 10:25:19.054370 mobio-mail-client-sdk-test-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9093 2024-01-04 10:25:18.000000 mobio-mail-client-sdk-test-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:48:22.568563 mobio-mail-client-sdk-test-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1293 2024-01-04 10:48:22.567563 mobio-mail-client-sdk-test-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:48:22.540562 mobio-mail-client-sdk-test-0.1.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:48:22.541562 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:48:22.552562 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/
+-rw-r--r--   0 root         (0) root         (0)      384 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/consts.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/folder.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/imap_utf7.py
+-rw-r--r--   0 root         (0) root         (0)    17294 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/mailbox.py
+-rw-r--r--   0 root         (0) root         (0)    10754 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/message.py
+-rw-r--r--   0 root         (0) root         (0)    16182 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:48:22.556563 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/
+-rw-r--r--   0 root         (0) root         (0)      316 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       95 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7702 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/html_quotations.py
+-rw-r--r--   0 root         (0) root         (0)    21203 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/quotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:48:22.559563 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/
+-rw-r--r--   0 root         (0) root         (0)     1356 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/bruteforce.py
+-rw-r--r--   0 root         (0) root         (0)       54 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:48:22.560562 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/data/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3380 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/extraction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:48:22.563563 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/classifier.py
+-rw-r--r--   0 root         (0) root         (0)     6115 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3105 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/featurespace.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4350 2024-01-04 10:47:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-04 10:48:22.567563 mobio-mail-client-sdk-test-0.1.9/mobio_mail_client_sdk_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1293 2024-01-04 10:48:22.000000 mobio-mail-client-sdk-test-0.1.9/mobio_mail_client_sdk_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1375 2024-01-04 10:48:22.000000 mobio-mail-client-sdk-test-0.1.9/mobio_mail_client_sdk_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-04 10:48:22.000000 mobio-mail-client-sdk-test-0.1.9/mobio_mail_client_sdk_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-01-04 10:48:22.000000 mobio-mail-client-sdk-test-0.1.9/mobio_mail_client_sdk_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-01-04 10:48:22.000000 mobio-mail-client-sdk-test-0.1.9/mobio_mail_client_sdk_test.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2024-01-04 10:24:49.000000 mobio-mail-client-sdk-test-0.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-04 10:48:22.568563 mobio-mail-client-sdk-test-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9093 2024-01-04 10:48:21.000000 mobio-mail-client-sdk-test-0.1.9/setup.py
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/PKG-INFO` & `mobio-mail-client-sdk-test-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-mail-client-sdk-test
-Version: 0.1.8
+Version: 0.1.9
 Summary: Mobio mail client SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mail client,imap
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/consts.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/consts.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/errors.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/errors.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/folder.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/folder.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/imap_utf7.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/imap_utf7.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/mailbox.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/mailbox.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/message.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/message.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/query.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/query.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/html_quotations.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/html_quotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The module's functions operate on message bodies trying to extract original
 messages (without quoted messages) from html
 """
 
 from __future__ import absolute_import
 import regex as re
 
-from talon.utils import cssselect 
+from mobio.sdks.mail_client.talon.utils import cssselect
 
 CHECKPOINT_PREFIX = '#!%!'
 CHECKPOINT_SUFFIX = '!%!#'
 CHECKPOINT_PATTERN = re.compile(CHECKPOINT_PREFIX + '\d+' + CHECKPOINT_SUFFIX)
 
 # HTML quote indicators (tag ids)
 QUOTE_IDS = ['OLK_SRC_BODY_SECTION']
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/quotations.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/quotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import logging
 from copy import deepcopy
 
 import regex as re
 from lxml import etree, html
 from six.moves import range
 
-from talon import html_quotations
-from talon.utils import (get_delimiter, html_document_fromstring,
+from mobio.sdks.mail_client.talon import html_quotations
+from mobio.sdks.mail_client.talon.utils import (get_delimiter, html_document_fromstring,
                          html_tree_to_text)
 
 log = logging.getLogger(__name__)
 
 
 RE_FWD = re.compile("^[-]+[ ]*Forwarded message[ ]*[-]+\s*$", re.I | re.M)
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/__init__.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,18 +19,21 @@
 * signature/data/train.data and
 * signature/data/classifier
 """
 
 from __future__ import absolute_import
 import os
 
-from talon.signature import extraction
-from talon.signature.extraction import extract
-from talon.signature.learning import classifier
+from mobio.sdks.mail_client.talon.signature import extraction
+from mobio.sdks.mail_client.talon.signature.extraction import extract
+from mobio.sdks.mail_client.talon.signature.learning import classifier
 
 
 def initialize():
     data_dir = os.path.join(os.path.dirname(__file__), 'data')
     extractor_filename = os.path.join(data_dir, 'classifier')
     extractor_data_filename = os.path.join(data_dir, 'train.data')
     extraction.EXTRACTOR = classifier.load(extractor_filename,
                                            extractor_data_filename)
+
+if __name__ == "__main__":
+    initialize()
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/bruteforce.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/bruteforce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import absolute_import
 
 import logging
 
 import regex as re
 
-from talon.signature.constants import (SIGNATURE_MAX_LINES,
+from mobio.sdks.mail_client.talon.signature.constants import (SIGNATURE_MAX_LINES,
                                        TOO_LONG_SIGNATURE_LINE)
-from talon.utils import get_delimiter
+from mobio.sdks.mail_client.talon.utils import get_delimiter
 
 log = logging.getLogger(__name__)
 
 # regex to fetch signature based on common signature words
 RE_SIGNATURE = re.compile(r'''
                (
                    (?:
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/extraction.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/extraction.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from __future__ import absolute_import
 
 import logging
 
 import numpy
 import regex as re
-from talon.signature.bruteforce import get_signature_candidate
-from talon.signature.learning.featurespace import features, build_pattern
-from talon.signature.learning.helpers import has_signature
-from talon.utils import get_delimiter
+from mobio.sdks.mail_client.talon.signature.bruteforce import get_signature_candidate
+from mobio.sdks.mail_client.talon.signature.learning.featurespace import features, build_pattern
+from mobio.sdks.mail_client.talon.signature.learning.helpers import has_signature
+from mobio.sdks.mail_client.talon.utils import get_delimiter
 
 log = logging.getLogger(__name__)
 
 EXTRACTOR = None
 
 # regex signature pattern for reversed lines
 # assumes that all long lines have been excluded
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/classifier.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/classifier.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/dataset.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from __future__ import absolute_import
 
 import os
 
 import regex as re
 from six.moves import range
 
-from talon.signature.constants import SIGNATURE_MAX_LINES
-from talon.signature.learning.featurespace import build_pattern, features
+from mobio.sdks.mail_client.talon.signature.constants import SIGNATURE_MAX_LINES
+from  mobio.sdks.mail_client.talon.signature.learning.featurespace import build_pattern, features
 
 SENDER_SUFFIX = '_sender'
 BODY_SUFFIX = '_body'
 
 SIGNATURE_ANNOTATION = '#sig#'
 REPLY_ANNOTATION = '#reply#'
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/featurespace.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/featurespace.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 into classifiers features space.
 
 The body and the message sender string are converted into unicode before
 applying features to them.
 """
 
 from __future__ import absolute_import
-from talon.signature.constants import (SIGNATURE_MAX_LINES,
+from mobio.sdks.mail_client.talon.signature.constants import (SIGNATURE_MAX_LINES,
                                        TOO_LONG_SIGNATURE_LINE)
-from talon.signature.learning.helpers import *
+from mobio.sdks.mail_client.talon.signature.learning.helpers import *
 from six.moves import zip
 from functools import reduce
 
 
 def features(sender=''):
     '''Returns a list of signature features.'''
     return [
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/signature/learning/helpers.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/signature/learning/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 * regexp's constants used when evaluating signature's features
 
 """
 import unicodedata
 
 import regex as re
 
-from talon.signature.constants import SIGNATURE_MAX_LINES
+from mobio.sdks.mail_client.talon.signature.constants import SIGNATURE_MAX_LINES
 
 rc = re.compile
 
 RE_EMAIL = rc('\S@\S')
 RE_RELAX_PHONE = rc('(\(? ?[\d]{2,3} ?\)?.{,3}?){2,}')
 RE_URL = rc(r"""https?://|www\.[\S]+\.[\S]""")
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/talon/utils.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/talon/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import html5lib
 import regex as re
 from html5lib import HTMLParser
 from lxml.cssselect import CSSSelector
 from lxml.etree import _Element
 from lxml.html import html5parser
 
-from talon.constants import RE_DELIMITER
+from mobio.sdks.mail_client.talon.constants import RE_DELIMITER
 
 
 def get_delimiter(msg_body: str) -> str:
     delimiter = RE_DELIMITER.search(msg_body)
     if delimiter:
         delimiter = delimiter.group()
     else:
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio/sdks/mail_client/utils.py` & `mobio-mail-client-sdk-test-0.1.9/mobio/sdks/mail_client/utils.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio_mail_client_sdk_test.egg-info/PKG-INFO` & `mobio-mail-client-sdk-test-0.1.9/mobio_mail_client_sdk_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-mail-client-sdk-test
-Version: 0.1.8
+Version: 0.1.9
 Summary: Mobio mail client SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mail client,imap
```

### Comparing `mobio-mail-client-sdk-test-0.1.8/mobio_mail_client_sdk_test.egg-info/SOURCES.txt` & `mobio-mail-client-sdk-test-0.1.9/mobio_mail_client_sdk_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-test-0.1.8/setup.py` & `mobio-mail-client-sdk-test-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         requirements = []
         # with open(Requirements.__requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='0.1.8'
+version_dev='0.1.9'
 version_prod='0.1.5'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -52,15 +52,15 @@
     name="mobio-mail-client-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.8',  # Required
+    version='0.1.9',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio mail client SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

