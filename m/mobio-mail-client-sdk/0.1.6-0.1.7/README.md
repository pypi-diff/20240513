# Comparing `tmp/mobio-mail-client-sdk-0.1.6.tar.gz` & `tmp/mobio_mail_client_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-mail-client-sdk-0.1.6.tar", last modified: Fri Jan  5 04:24:41 2024, max compression
+gzip compressed data, was "mobio_mail_client_sdk-0.1.7.tar", last modified: Mon May 13 09:21:24 2024, max compression
```

## Comparing `mobio-mail-client-sdk-0.1.6.tar` & `mobio_mail_client_sdk-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 04:24:41.040188 mobio-mail-client-sdk-0.1.6/
--rw-r--r--   0 root         (0) root         (0)     1482 2024-01-05 04:24:41.037188 mobio-mail-client-sdk-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 04:24:40.991186 mobio-mail-client-sdk-0.1.6/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 04:24:40.991186 mobio-mail-client-sdk-0.1.6/mobio/sdks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 04:24:41.004187 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/
--rw-r--r--   0 root         (0) root         (0)      384 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1415 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/consts.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/errors.py
--rw-r--r--   0 root         (0) root         (0)     7054 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/folder.py
--rw-r--r--   0 root         (0) root         (0)     2059 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/imap_utf7.py
--rw-r--r--   0 root         (0) root         (0)    17294 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/mailbox.py
--rw-r--r--   0 root         (0) root         (0)    10754 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/message.py
--rw-r--r--   0 root         (0) root         (0)    16182 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 04:24:41.025187 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/talon/
--rw-r--r--   0 root         (0) root         (0)      163 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/talon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       95 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/talon/constants.py
--rw-r--r--   0 root         (0) root         (0)     7695 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/talon/html_quotations.py
--rw-r--r--   0 root         (0) root         (0)    21178 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/talon/quotations.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/talon/utils.py
--rw-r--r--   0 root         (0) root         (0)     7389 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 04:24:41.036188 mobio-mail-client-sdk-0.1.6/mobio_mail_client_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1482 2024-01-05 04:24:40.000000 mobio-mail-client-sdk-0.1.6/mobio_mail_client_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      825 2024-01-05 04:24:40.000000 mobio-mail-client-sdk-0.1.6/mobio_mail_client_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-05 04:24:40.000000 mobio-mail-client-sdk-0.1.6/mobio_mail_client_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-01-05 04:24:40.000000 mobio-mail-client-sdk-0.1.6/mobio_mail_client_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       89 2024-01-05 04:24:40.000000 mobio-mail-client-sdk-0.1.6/mobio_mail_client_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-01-05 04:24:40.000000 mobio-mail-client-sdk-0.1.6/mobio_mail_client_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2024-01-05 04:24:10.000000 mobio-mail-client-sdk-0.1.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-05 04:24:41.040188 mobio-mail-client-sdk-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9302 2024-01-05 04:24:40.000000 mobio-mail-client-sdk-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:21:24.242996 mobio_mail_client_sdk-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1482 2024-05-13 09:21:24.242996 mobio_mail_client_sdk-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:21:24.208995 mobio_mail_client_sdk-0.1.7/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:21:24.208995 mobio_mail_client_sdk-0.1.7/mobio/sdks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:21:24.218995 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/consts.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/folder.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/imap_utf7.py
+-rw-r--r--   0 root         (0) root         (0)    17533 2024-05-13 09:20:21.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/mailbox.py
+-rw-r--r--   0 root         (0) root         (0)    10754 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/message.py
+-rw-r--r--   0 root         (0) root         (0)    16182 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:21:24.222995 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/talon/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/talon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       95 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/talon/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7695 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/talon/html_quotations.py
+-rw-r--r--   0 root         (0) root         (0)    21178 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/talon/quotations.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/talon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:21:24.241996 mobio_mail_client_sdk-0.1.7/mobio_mail_client_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1482 2024-05-13 09:21:24.000000 mobio_mail_client_sdk-0.1.7/mobio_mail_client_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      825 2024-05-13 09:21:24.000000 mobio_mail_client_sdk-0.1.7/mobio_mail_client_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 09:21:24.000000 mobio_mail_client_sdk-0.1.7/mobio_mail_client_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-13 09:21:24.000000 mobio_mail_client_sdk-0.1.7/mobio_mail_client_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-13 09:21:24.000000 mobio_mail_client_sdk-0.1.7/mobio_mail_client_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-13 09:21:24.000000 mobio_mail_client_sdk-0.1.7/mobio_mail_client_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-13 07:08:55.000000 mobio_mail_client_sdk-0.1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 09:21:24.243996 mobio_mail_client_sdk-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-05-13 09:21:23.000000 mobio_mail_client_sdk-0.1.7/setup.py
```

### Comparing `mobio-mail-client-sdk-0.1.6/PKG-INFO` & `mobio_mail_client_sdk-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-mail-client-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Mobio mail client SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mail client,imap
```

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/consts.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/consts.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/errors.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/errors.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/folder.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/folder.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/imap_utf7.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/imap_utf7.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/mailbox.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/mailbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         for fetch_item in (self._fetch_in_bulk if bulk else self._fetch_by_one)(nums, message_parts, reverse):  # noqa
             mail_message = self.email_message_class(fetch_item)
             if miss_no_uid and not mail_message.uid:
                 continue
             yield mail_message
 
     def select_search(self, mailbox = "INBOX", criteria: Criteria = 'ALL', charset: str = 'US-ASCII',
-                      mark_seen=False, reverse=False, headers_only=False):
+                      mark_seen=False, reverse=False, headers_only=False, list_uid_exists=None):
         """
         Mail message generator in current folder by search criteria
         :param criteria: message search criteria (see examples at ./doc/imap_search_criteria.txt)
         :param charset: IANA charset, indicates charset of the strings that appear in the search criteria. See rfc2978
         :param miss_no_uid: miss emails without uid
         :param reverse: in order from the larger date to the smaller
 
@@ -147,15 +147,20 @@
         message_parts = "(BODY{}[{}] UID FLAGS RFC822.SIZE)".format(
             '' if mark_seen else '.PEEK', 'HEADER' if headers_only else '')
         encoded_criteria = criteria if type(criteria) is bytes else str(criteria).encode(charset)
         select_result = self.box.select(mailbox=mailbox, readonly=False)
         check_command_status(select_result, MailboxFolderSelectError)
         search_result = self.box.search(charset, encoded_criteria)
         check_command_status(search_result, MailboxNumbersError)
-        for mail_id in search_result[1][0].decode().split():
+        list_uid_response = search_result[1][0].decode().split()
+        if list_uid_exists:
+            list_uid_new = list(set(list_uid_response).difference(list_uid_exists))
+        else:
+            list_uid_new = list_uid_response
+        for mail_id in list_uid_new:
             print("select_search mail_id: {}".format(mail_id))
             fetch_result = self.box.fetch(
                 mail_id, message_parts
             )  ## Fetch mail data.
             check_command_status(fetch_result, MailboxFetchError)
             # for built_fetch_item in chunks((reversed if reverse else iter)(fetch_result[1]), 2):
             mail_message = self.email_message_class(fetch_result[1])
```

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/message.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/message.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/query.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/query.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/talon/html_quotations.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/talon/html_quotations.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/talon/quotations.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/talon/quotations.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/talon/utils.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/talon/utils.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio/sdks/mail_client/utils.py` & `mobio_mail_client_sdk-0.1.7/mobio/sdks/mail_client/utils.py`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/mobio_mail_client_sdk.egg-info/PKG-INFO` & `mobio_mail_client_sdk-0.1.7/mobio_mail_client_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-mail-client-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Mobio mail client SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mail client,imap
```

### Comparing `mobio-mail-client-sdk-0.1.6/mobio_mail_client_sdk.egg-info/SOURCES.txt` & `mobio_mail_client_sdk-0.1.7/mobio_mail_client_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-mail-client-sdk-0.1.6/setup.py` & `mobio_mail_client_sdk-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         # with open(Requirements.__requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
 version_dev='0.1.15'
-version_prod='0.1.6'
+version_prod='0.1.7'
 
 run_mode=''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -60,15 +60,15 @@
     name="mobio-mail-client-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.6',  # Required
+    version='0.1.7',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio mail client SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

