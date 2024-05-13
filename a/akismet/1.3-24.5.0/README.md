# Comparing `tmp/akismet-1.3.tar.gz` & `tmp/akismet-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akismet-1.3.tar", last modified: Tue Feb 20 06:39:59 2024, max compression
+gzip compressed data, was "akismet-24.5.0.tar", last modified: Mon May 13 00:25:52 2024, max compression
```

## Comparing `akismet-1.3.tar` & `akismet-24.5.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-20 06:39:59.313392 akismet-1.3/
--rw-r--r--   0 james      (503) staff       (20)      273 2023-07-06 06:29:44.000000 akismet-1.3/.editorconfig
--rw-r--r--   0 james      (503) staff       (20)       71 2023-07-06 06:29:48.000000 akismet-1.3/.flake8
--rw-r--r--   0 james      (503) staff       (20)     1041 2024-02-19 23:45:16.000000 akismet-1.3/.pre-commit-config.yaml
--rw-r--r--   0 james      (503) staff       (20)      295 2023-11-14 06:48:02.000000 akismet-1.3/.readthedocs.yaml
--rw-r--r--   0 james      (503) staff       (20)     3185 2023-11-19 00:06:48.000000 akismet-1.3/CONTRIBUTING.rst
--rw-r--r--   0 james      (503) staff       (20)     1546 2024-01-02 03:24:27.000000 akismet-1.3/LICENSE
--rw-r--r--   0 james      (503) staff       (20)      287 2023-11-18 09:36:15.000000 akismet-1.3/MANIFEST.in
--rw-r--r--   0 james      (503) staff       (20)     4397 2024-02-20 06:39:59.313197 akismet-1.3/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)     2895 2024-02-20 01:37:00.000000 akismet-1.3/README.rst
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-20 06:39:59.310273 akismet-1.3/docs/
--rw-r--r--   0 james      (503) staff       (20)      607 2017-05-26 06:28:40.000000 akismet-1.3/docs/Makefile
--rw-r--r--   0 james      (503) staff       (20)      367 2023-11-19 02:04:17.000000 akismet-1.3/docs/async_client.rst
--rw-r--r--   0 james      (503) staff       (20)     1404 2024-02-19 23:45:43.000000 akismet-1.3/docs/conf.py
--rw-r--r--   0 james      (503) staff       (20)      395 2023-12-01 07:15:23.000000 akismet-1.3/docs/exceptions.rst
--rw-r--r--   0 james      (503) staff       (20)     6794 2024-02-20 02:09:06.000000 akismet-1.3/docs/faq.rst
--rw-r--r--   0 james      (503) staff       (20)      603 2023-11-29 08:01:25.000000 akismet-1.3/docs/index.rst
--rw-r--r--   0 james      (503) staff       (20)     2649 2024-02-20 01:39:29.000000 akismet-1.3/docs/install.rst
--rw-r--r--   0 james      (503) staff       (20)      805 2017-05-26 06:28:40.000000 akismet-1.3/docs/make.bat
--rw-r--r--   0 james      (503) staff       (20)     1447 2023-11-15 06:08:10.000000 akismet-1.3/docs/misc.rst
--rw-r--r--   0 james      (503) staff       (20)      174 2023-11-29 07:45:26.000000 akismet-1.3/docs/spelling_wordlist.txt
--rw-r--r--   0 james      (503) staff       (20)      363 2023-11-19 02:04:24.000000 akismet-1.3/docs/sync_client.rst
--rw-r--r--   0 james      (503) staff       (20)     4016 2024-02-20 02:00:31.000000 akismet-1.3/docs/testing.rst
--rw-r--r--   0 james      (503) staff       (20)     5390 2024-01-02 03:28:16.000000 akismet-1.3/docs/upgrade.rst
--rw-r--r--   0 james      (503) staff       (20)    10211 2024-02-20 01:57:39.000000 akismet-1.3/docs/usage.rst
--rw-r--r--   0 james      (503) staff       (20)    10546 2024-02-20 02:28:35.000000 akismet-1.3/noxfile.py
--rw-r--r--   0 james      (503) staff       (20)     1720 2024-01-15 23:29:55.000000 akismet-1.3/pyproject.toml
--rw-r--r--   0 james      (503) staff       (20)       38 2024-02-20 06:39:59.313433 akismet-1.3/setup.cfg
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-20 06:39:59.306977 akismet-1.3/src/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-20 06:39:59.311178 akismet-1.3/src/akismet/
--rw-r--r--   0 james      (503) staff       (20)     3272 2024-02-20 01:37:10.000000 akismet-1.3/src/akismet/__init__.py
--rw-r--r--   0 james      (503) staff       (20)    22643 2024-02-20 01:58:13.000000 akismet-1.3/src/akismet/_async_client.py
--rw-r--r--   0 james      (503) staff       (20)     4433 2024-02-19 23:45:43.000000 akismet-1.3/src/akismet/_common.py
--rw-r--r--   0 james      (503) staff       (20)     1439 2024-02-19 23:45:43.000000 akismet-1.3/src/akismet/_exceptions.py
--rw-r--r--   0 james      (503) staff       (20)     8963 2024-02-20 06:01:45.000000 akismet-1.3/src/akismet/_legacy_client.py
--rw-r--r--   0 james      (503) staff       (20)    22525 2024-02-20 01:58:00.000000 akismet-1.3/src/akismet/_sync_client.py
--rw-r--r--   0 james      (503) staff       (20)      436 2024-02-20 06:36:33.000000 akismet-1.3/src/akismet/_version.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-20 06:39:59.312684 akismet-1.3/src/akismet.egg-info/
--rw-r--r--   0 james      (503) staff       (20)     4397 2024-02-20 06:39:59.000000 akismet-1.3/src/akismet.egg-info/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)      876 2024-02-20 06:39:59.000000 akismet-1.3/src/akismet.egg-info/SOURCES.txt
--rw-r--r--   0 james      (503) staff       (20)        1 2024-02-20 06:39:59.000000 akismet-1.3/src/akismet.egg-info/dependency_links.txt
--rw-r--r--   0 james      (503) staff       (20)      139 2024-02-20 06:39:59.000000 akismet-1.3/src/akismet.egg-info/requires.txt
--rw-r--r--   0 james      (503) staff       (20)        8 2024-02-20 06:39:59.000000 akismet-1.3/src/akismet.egg-info/top_level.txt
-drwxr-xr-x   0 james      (503) staff       (20)        0 2024-02-20 06:39:59.312480 akismet-1.3/tests/
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-19 07:04:53.000000 akismet-1.3/tests/__init__.py
--rw-r--r--   0 james      (503) staff       (20)     4743 2024-02-19 23:45:43.000000 akismet-1.3/tests/base.py
--rw-r--r--   0 james      (503) staff       (20)     9993 2024-02-19 23:45:43.000000 akismet-1.3/tests/end_to_end.py
--rw-r--r--   0 james      (503) staff       (20)    18163 2024-02-19 23:45:43.000000 akismet-1.3/tests/test_async_client.py
--rw-r--r--   0 james      (503) staff       (20)    10695 2024-02-19 23:45:43.000000 akismet-1.3/tests/test_legacy_client.py
--rw-r--r--   0 james      (503) staff       (20)    17703 2024-02-19 23:45:43.000000 akismet-1.3/tests/test_sync_client.py
--rw-r--r--   0 james      (503) staff       (20)     6562 2022-05-27 04:42:48.000000 akismet-1.3/tox.ini
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-13 00:25:52.682927 akismet-24.5.0/
+-rw-r--r--   0 james      (503) staff       (20)      273 2023-07-06 06:29:44.000000 akismet-24.5.0/.editorconfig
+-rw-r--r--   0 james      (503) staff       (20)       97 2024-04-17 07:23:40.000000 akismet-24.5.0/.flake8
+-rw-r--r--   0 james      (503) staff       (20)     1041 2024-02-19 23:45:16.000000 akismet-24.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 james      (503) staff       (20)      295 2023-11-14 06:48:02.000000 akismet-24.5.0/.readthedocs.yaml
+-rw-r--r--   0 james      (503) staff       (20)     3185 2023-11-19 00:06:48.000000 akismet-24.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 james      (503) staff       (20)     1546 2024-01-02 03:24:27.000000 akismet-24.5.0/LICENSE
+-rw-r--r--   0 james      (503) staff       (20)      287 2023-11-18 09:36:15.000000 akismet-24.5.0/MANIFEST.in
+-rw-r--r--   0 james      (503) staff       (20)     4952 2024-05-13 00:25:52.682731 akismet-24.5.0/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)     3450 2024-05-12 22:31:08.000000 akismet-24.5.0/README.rst
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-13 00:25:52.679197 akismet-24.5.0/docs/
+-rw-r--r--   0 james      (503) staff       (20)      607 2017-05-26 06:28:40.000000 akismet-24.5.0/docs/Makefile
+-rw-r--r--   0 james      (503) staff       (20)      367 2023-11-19 02:04:17.000000 akismet-24.5.0/docs/async_client.rst
+-rw-r--r--   0 james      (503) staff       (20)     7459 2024-05-06 05:54:43.000000 akismet-24.5.0/docs/changelog.rst
+-rw-r--r--   0 james      (503) staff       (20)     1404 2024-02-24 08:11:57.000000 akismet-24.5.0/docs/conf.py
+-rw-r--r--   0 james      (503) staff       (20)      395 2023-12-01 07:15:23.000000 akismet-24.5.0/docs/exceptions.rst
+-rw-r--r--   0 james      (503) staff       (20)     6363 2024-04-29 06:47:40.000000 akismet-24.5.0/docs/faq.rst
+-rw-r--r--   0 james      (503) staff       (20)      621 2024-04-19 07:52:43.000000 akismet-24.5.0/docs/index.rst
+-rw-r--r--   0 james      (503) staff       (20)     2649 2024-02-27 07:30:04.000000 akismet-24.5.0/docs/install.rst
+-rw-r--r--   0 james      (503) staff       (20)      805 2017-05-26 06:28:40.000000 akismet-24.5.0/docs/make.bat
+-rw-r--r--   0 james      (503) staff       (20)     1447 2023-11-15 06:08:10.000000 akismet-24.5.0/docs/misc.rst
+-rw-r--r--   0 james      (503) staff       (20)      239 2024-05-06 05:57:27.000000 akismet-24.5.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 james      (503) staff       (20)      363 2023-11-19 02:04:24.000000 akismet-24.5.0/docs/sync_client.rst
+-rw-r--r--   0 james      (503) staff       (20)      623 2024-05-06 05:52:10.000000 akismet-24.5.0/docs/test_clients.rst
+-rw-r--r--   0 james      (503) staff       (20)     8338 2024-04-21 06:57:26.000000 akismet-24.5.0/docs/testing.rst
+-rw-r--r--   0 james      (503) staff       (20)    19976 2024-05-12 23:13:45.000000 akismet-24.5.0/docs/usage.rst
+-rw-r--r--   0 james      (503) staff       (20)    10544 2024-04-21 06:49:12.000000 akismet-24.5.0/noxfile.py
+-rw-r--r--   0 james      (503) staff       (20)     1786 2024-05-12 22:39:30.000000 akismet-24.5.0/pyproject.toml
+-rw-r--r--   0 james      (503) staff       (20)       38 2024-05-13 00:25:52.682971 akismet-24.5.0/setup.cfg
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-13 00:25:52.676003 akismet-24.5.0/src/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-13 00:25:52.680356 akismet-24.5.0/src/akismet/
+-rw-r--r--   0 james      (503) staff       (20)     3910 2024-05-12 21:32:38.000000 akismet-24.5.0/src/akismet/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)    24754 2024-04-29 06:22:20.000000 akismet-24.5.0/src/akismet/_async_client.py
+-rw-r--r--   0 james      (503) staff       (20)     4760 2024-05-12 22:48:36.000000 akismet-24.5.0/src/akismet/_common.py
+-rw-r--r--   0 james      (503) staff       (20)     1439 2024-04-09 06:24:58.000000 akismet-24.5.0/src/akismet/_exceptions.py
+-rw-r--r--   0 james      (503) staff       (20)     8955 2024-04-10 02:05:47.000000 akismet-24.5.0/src/akismet/_legacy_client.py
+-rw-r--r--   0 james      (503) staff       (20)    24585 2024-04-29 06:23:30.000000 akismet-24.5.0/src/akismet/_sync_client.py
+-rw-r--r--   0 james      (503) staff       (20)    11401 2024-05-12 23:34:52.000000 akismet-24.5.0/src/akismet/_test_clients.py
+-rw-r--r--   0 james      (503) staff       (20)      438 2024-05-13 00:25:01.000000 akismet-24.5.0/src/akismet/_version.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-13 00:25:52.682207 akismet-24.5.0/src/akismet.egg-info/
+-rw-r--r--   0 james      (503) staff       (20)     4952 2024-05-13 00:25:52.000000 akismet-24.5.0/src/akismet.egg-info/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)      956 2024-05-13 00:25:52.000000 akismet-24.5.0/src/akismet.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (503) staff       (20)        1 2024-05-13 00:25:52.000000 akismet-24.5.0/src/akismet.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (503) staff       (20)      139 2024-05-13 00:25:52.000000 akismet-24.5.0/src/akismet.egg-info/requires.txt
+-rw-r--r--   0 james      (503) staff       (20)        8 2024-05-13 00:25:52.000000 akismet-24.5.0/src/akismet.egg-info/top_level.txt
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-13 00:25:52.682013 akismet-24.5.0/tests/
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-19 07:04:53.000000 akismet-24.5.0/tests/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)     1946 2024-04-17 07:24:29.000000 akismet-24.5.0/tests/base.py
+-rw-r--r--   0 james      (503) staff       (20)     9939 2024-04-21 08:02:26.000000 akismet-24.5.0/tests/end_to_end.py
+-rw-r--r--   0 james      (503) staff       (20)    19693 2024-04-23 06:54:43.000000 akismet-24.5.0/tests/test_async_client.py
+-rw-r--r--   0 james      (503) staff       (20)    10814 2024-04-17 06:40:03.000000 akismet-24.5.0/tests/test_legacy_client.py
+-rw-r--r--   0 james      (503) staff       (20)    19054 2024-04-23 06:58:32.000000 akismet-24.5.0/tests/test_sync_client.py
+-rw-r--r--   0 james      (503) staff       (20)     5585 2024-04-21 08:01:22.000000 akismet-24.5.0/tests/test_test_clients.py
+-rw-r--r--   0 james      (503) staff       (20)     6562 2022-05-27 04:42:48.000000 akismet-24.5.0/tox.ini
```

### Comparing `akismet-1.3/.pre-commit-config.yaml` & `akismet-24.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akismet-1.3/CONTRIBUTING.rst` & `akismet-24.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `akismet-1.3/LICENSE` & `akismet-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `akismet-1.3/PKG-INFO` & `akismet-24.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: akismet
-Version: 1.3
+Version: 24.5.0
 Summary: A Python interface to the Akismet spam-filtering service.
-Author: Michael Foord
-Author-email: James Bennett <james@b-list.org>
+Author: Michael Foord, James Bennett
+Maintainer: James Bennett
 License: BSD-3-Clause
-Project-URL: documentation, https://akismet.readthedocs.io
-Project-URL: homepage, https://github.com/ubernostrum/akismet
+Project-URL: Documentation, https://akismet.readthedocs.io
+Project-URL: Source Code, https://github.com/ubernostrum/akismet
 Keywords: akismet,spam,spam-filtering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -52,25 +52,27 @@
 
 * ``akismet.AsyncClient`` is an Akismet API client which performs
   asynchronous (``async``/``await``/non-blocking) HTTP requests to the
   Akismet web service.
 
 Aside from one being sync and the other async, the two clients expose
 identical APIs, and implement all methods of `the Akismet web API
-<https://akismet.com/developers/>`_, including the v1.2 key and API
-usage metrics.
+<https://akismet.com/developers/>`_.
 
 To use this library, you will need to obtain an Akismet API key and
 register a site for use with the Akismet web service; you can do this
 at <https://akismet.com>. Once you have a key and corresponding
 registered site URL to use with it, place them in the environment
 variables ``PYTHON_AKISMET_API_KEY`` and ``PYTHON_AKISMET_BLOG_URL``,
 and they will be automatically detected and used.
 
 You can then construct a client instance and call its methods. For
+creating a long-lived API client instance, it's recommended that you
+use the ``validated_client()`` constructor method, which will
+automatically validate your API key with the Akismet web service. For
 example, to check a submitted forum post for spam:
 
 .. code-block:: python
 
    import akismet
 
    akismet_client = akismet.SyncClient.validated_client()
@@ -95,22 +97,45 @@
        user_ip=submitter_ip,
        comment_content=submitted_content,
        comment_type="forum-post",
        comment_author=submitter_name
    ):
        # This piece of content was classified as spam; handle it appropriately.
 
-Note that in both cases the client instance is created via the
-alternate constructor ``validated_client()``. This is recommended
-instead of using the default constructor (i.e., directly calling
-``akismet.SyncClient()`` or ``akismet.AsyncClient()``); the
-``validated_client()`` constructor will perform automatic discovery of
-the environment-variable configuration and validate the configuration
-with the Akismet web service before returning the client, while
-directly constructing an instance will not (so if you do directly
-construct an instance, you must manually provide and validate its
-configuration).
+You can also use either client class as a context manager. This does
+*not* require the ``validated_client()`` constructor, because your API
+key is validated on entering the ``with`` block.
+
+.. code-block:: python
+
+   import akismet
+
+   with akismet.SyncClient() as akismet_client:
+       if akismet_client.comment_check(
+           user_ip=submitter_ip,
+           comment_content=submitted_content,
+           comment_type="forum-post",
+           comment_author=submitter_name
+       ):
+           # This piece of content was classified as spam; handle it appropriately.
+
+Or using the asynchronous client:
+
+.. code-block:: python
+
+   import akismet
+
+   async with akismet.AsyncClient() as akismet_client:
+       if await akismet_client.comment_check(
+           user_ip=submitter_ip,
+           comment_content=submitted_content,
+           comment_type="forum-post",
+           comment_author=submitter_name
+       ):
+           # This piece of content was classified as spam; handle it appropriately.
+
+
 
 See `the documentation <http://akismet.readthedocs.io/>`_ for full
 details.
 
 The original version of this library was written by Michael Foord.
```

### Comparing `akismet-1.3/docs/Makefile` & `akismet-24.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `akismet-1.3/docs/conf.py` & `akismet-24.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `akismet-1.3/docs/faq.rst` & `akismet-24.5.0/docs/faq.rst`

 * *Files 13% similar despite different names*

```diff
@@ -44,111 +44,106 @@
 including comments, contact-form submissions, user signups and more. See
 `Akismet's documentation of the comment check operation
 <https://akismet.com/developers/comment-check/>`_ for details.
 
 
 .. _alt-constructor:
 
-Why shouldn't I create the client directly?
--------------------------------------------
+Why doesn't the default constructor validate the config?
+--------------------------------------------------------
 
-Both of the API clients provide a ``classmethod`` which serves as an alternate
-constructor: :meth:`akismet.SyncClient.validated_client` and
-:meth:`akismet.AsyncClient.validated_client`, and you're encouraged to use
-these alternate constructors when you need an instance of one of the clients.
-
-The short explanation for this is that the ``validated_client()`` constructor
-will automatically read your Akismet API key and site URL from environment
-variables (``PYTHON_AKISMET_API_KEY`` and ``PYTHON_AKISMET_BLOG_URL``) and
-validate them via the ``verify_key`` operation before returning the API client
-instance to you, and this is highly useful behavior.
-
-If you don't use the ``validated_client()`` constructor, you'll need to
-construct your own :class:`~akismet.Config` to pass in to the default
-constructor, and you'll want to ensure you call the verify-key operation to
-validate that configuration.
-
-The longer explanation is that the ``validated_client()`` constructor allows
-both the sync and async clients to provide the same
-interface. :class:`~akismet.SyncClient` could easily just read the
-configuration and do the validation in its own ``__init__()`` method. But
-:class:`~akismet.AsyncClient` cannot do this, because its
+Both of the Akismet API clients provide an alternate constructor --
+:meth:`akismet.SyncClient.validated_client` and
+:meth:`akismet.AsyncClient.validated_client` -- and you're encouraged to use
+these nearly any time you want an instance of an Akismet API client (the
+exception is using a client as a context manager -- see below), because the
+``validated_client()`` constructor will validate your Akismet configuration
+(via the verify-key API operation) automatically. If you don't do this, you'll
+need to call ``verify_key()`` manually (and ideally only once for each client
+instance).
+
+The technical reason for this is that the ``validated_client()`` constructor
+allows both the sync and async clients to provide the same
+interface. :class:`~akismet.SyncClient` could perform the validation in its
+``__init__()`` method, but :class:`~akismet.AsyncClient` cannot, because its
 :meth:`~akismet.AsyncClient.verify_key` method is asynchronous; calling it in
 ``__init__()`` would require making the ``__init__()`` method asynchronous too,
 and an async ``__init__()`` is not currently supported by Python.
 
 This limitation does not apply to classmethods used as alternate constructors,
-so to provide a useful constructor that does automatic discovery and validation
-of your Akismet configuration, :class:`~akismet.AsyncClient` defines the
-alternate constructor :meth:`~akismet.AsyncClient.validated_client`. And to
-ensure both client classes have the same interface,
-:class:`~akismet.SyncClient` also provides a
+so to perform automatic validation of your Akismet configuration,
+:class:`~akismet.AsyncClient` defines the alternate constructor
+:meth:`~akismet.AsyncClient.validated_client`. And to ensure both client
+classes have the same interface, :class:`~akismet.SyncClient` also provides a
 :meth:`~akismet.SyncClient.validated_client` constructor.
 
+Using either client class as a context manager does not have this technical
+limitation (the entry method of an async context manager is async, so the
+verify-key operation can be called there), so using one of the Akismet client
+classes as a context manager does not require using the alternate constructor.
+
 
 How do I check my key?
 ----------------------
 
-The simplest way is to set your key and site URL in the standard environment
-variables (``PYTHON_AKISMET_API_KEY`` / ``PYTHON_AKISMET_BLOG_URL``), and then
-call either :meth:`akismet.SyncClient.validated_client` or
-:meth:`akismet.AsyncClient.validated_client`; the ``validated_client()``
-constructor automatically verifies the key and URL for you, and will raise
-:exc:`~akismet.APIKeyError` if the key is invalid.
+The simplest way is to either:
+
+* Use :meth:`akismet.SyncClient.validated_client` /
+  :meth:`akismet.AsyncClient.validated_client`, or
+
+* Create a client as a context manager (e.g., ``with akismet.SyncClient() as
+  akismet_client`` or ``async with akismet.AsyncClient() as akismet_client``)
+
+Either of these approaches automatically verifies the key and URL for you, and
+will raise :exc:`~akismet.APIKeyError` if the key is invalid.
 
 If you're not able to do this, you can also manually instantiate a client and
 then call its ``verify_key()`` method, passing the key and URL you want to
 check as the arguments. For example:
 
 .. tab:: Sync
 
    .. code-block:: python
 
       import akismet
 
-      config = akismet.Config(key=key_to_test, url=url_to_test)
-      client = akismet.SyncClient(config=config)
+      client = akismet.SyncClient()
       if not client.verify_key(key_to_test, url_to_test):
           # The key/URL were invalid.
 
 .. tab:: Async
 
    .. code-block:: python
 
       import akismet
 
-      config = akismet.Config(key=key_to_test, url=url_to_test)
-      client = akismet.AyncClient(config=config)
+      client = akismet.AyncClient()
       if not await client.verify_key(key_to_test, url_to_test):
           # The key/URL were invalid.
 
 
 How can I test that it's working?
 ---------------------------------
 
-The documentation :ref:`includes a section <testing>` on how to run
-``akismet``'s unit test suite.
-
-If you want to manually perform your own tests, you can also instantiate an
-Akismet client class and call its methods. When doing so, it is recommended
-that you pass the optional keyword argument ``is_test=1`` to the comment-check,
-submit-ham, and submit-spam operations; this tells the Akismet web service that
-you are only issuing requests for testing purposes, and will not result in any
-submissions being incorporated into Akismet's training corpus.
+``akismet`` provides test-client implementations you can use in your own
+application's tests; it also provides its own thorough test suite you can run
+to verify its behavior, and you can perform some live end-to-end testing
+through the standard Akismet API clients. See :ref:`the testing guide
+<testing>` for details.
 
 
 What user-agent string is sent by ``akismet``?
 ----------------------------------------------
 
 The Akismet web service documentation recommends sending a string identifying
 the application or platform with version, and Akismet plugin/implementation
 name with version. In accordance with this, ``akismet`` sends an HTTP
 ``User-Agent`` based on the versions of Python and ``akismet`` in use. For
-example, ``akismet`` 1.3 on Python 3.10.4 will send ``akismet.py/1.3 | Python
-3.10.4``.
+example, ``akismet`` 24.4.0 on Python 3.10.4 will send ``akismet.py/24.4.0 |
+Python 3.10.4``.
 
 
 Does ``akismet`` support the "pro-tip" header?
 ----------------------------------------------
 
 For content determined to be "blatant" spam (and thus which does not need to be
 placed into a queue for review by a human), the Akismet web service will add
```

### Comparing `akismet-1.3/docs/index.rst` & `akismet-24.5.0/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 
 .. toctree::
    :caption: API reference
    :maxdepth: 1
 
    sync_client
    async_client
+   test_clients
    exceptions
    misc
 
 .. toctree::
    :caption: Other documentation
    :maxdepth: 1
 
    testing
-   upgrade
+   changelog
    faq
 
 .. seealso::
 
    `The developer documentation for the Akismet web service
    <https://akismet.com/developers/>`_ is useful for familiarizing yourself
    with the available API operations and features.
```

### Comparing `akismet-1.3/docs/install.rst` & `akismet-24.5.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `akismet-1.3/docs/make.bat` & `akismet-24.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `akismet-1.3/docs/misc.rst` & `akismet-24.5.0/docs/misc.rst`

 * *Files identical despite different names*

### Comparing `akismet-1.3/noxfile.py` & `akismet-24.5.0/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     )
     clean()
 
 
 @nox.session(python=["3.12"], tags=["formatters"])
 def format_isort(session: nox.Session) -> None:
     """
-    Check code formating with Black.
+    Check import order with isort.
 
     """
     session.install("isort")
     session.run(f"python{session.python}", "-Im", "isort", "--version")
     session.run(
         f"python{session.python}",
         "-Im",
```

### Comparing `akismet-1.3/pyproject.toml` & `akismet-24.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 authors = [
-  {name = "James Bennett", email = "james@b-list.org"},
   {name = "Michael Foord"},
+  {name = "James Bennett"}
+]
+maintainers = [
+  {name = "James Bennett"}
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
@@ -30,16 +33,16 @@
 dynamic = ["version"]
 keywords = ["akismet", "spam", "spam-filtering"]
 license = {text = "BSD-3-Clause"}
 readme = "README.rst"
 requires-python = ">=3.8"
 
 [project.urls]
-documentation = "https://akismet.readthedocs.io"
-homepage = "https://github.com/ubernostrum/akismet"
+"Documentation" = "https://akismet.readthedocs.io"
+"Source Code" = "https://github.com/ubernostrum/akismet"
 
 [project.optional-dependencies]
 docs = [
   "furo",
   "matplotlib",
   "sphinx",
   "sphinx-copybutton",
@@ -57,14 +60,16 @@
 [tool.black]
 target-version = ["py38", "py39", "py310", "py311", "py312"]
 
 [tool.coverage.report]
 fail_under = 100
 
 [tool.interrogate]
+fail-under = 100
+ignore-init-method = true
 ignore-init-module = true
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint]
 disable = [
```

### Comparing `akismet-1.3/src/akismet/__init__.py` & `akismet-24.5.0/src/akismet/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 * :class:`akismet.SyncClient` is an Akismet API client which performs synchronous
   (blocking) HTTP requests to the Akismet web service.
 
 * :class:`akismet.AsyncClient` is an Akismet API client which performs asynchronous
   (``async``/``await``/non-blocking) HTTP requests to the Akismet web service.
 
 Aside from one being sync and the other async, the two clients expose identical APIs,
-and implement all methods of `the Akismet web API <https://akismet.com/developers/>`_,
-including the v1.2 key and API usage metrics.
+and implement all methods of `the Akismet web API <https://akismet.com/developers/>`_.
 
 To use this library, you will need to obtain an Akismet API key and register a site for
 use with the Akismet web service; you can do this at <https://akismet.com>. Once you
 have a key and corresponding registered site URL to use with it, place them in the
 environment variables ``PYTHON_AKISMET_API_KEY`` and ``PYTHON_AKISMET_BLOG_URL``, and
 they will be automatically detected and used.
 
-You can then construct a client instance and call its methods. For example, to check a
-submitted forum post for spam:
+You can then construct a client instance and call its methods. For creating a long-lived
+API client instance, it's recommended that you use the ``validated_client()``
+constructor method, which will automatically validate your API key with the Akismet web
+service. For example, to check a submitted forum post for spam:
 
 .. code-block:: python
 
    import akismet
 
    akismet_client = akismet.SyncClient.validated_client()
 
@@ -48,22 +49,45 @@
        user_ip=submitter_ip,
        comment_content=submitted_content,
        comment_type="forum-post",
        comment_author=submitter_name
    ):
        # This piece of content was classified as spam; handle it appropriately.
 
-Note that in both cases the client instance is created via the alternate constructor
-``validated_client()``. This is recommended instead of using the default constructor
-(i.e., directly calling ``akismet.SyncClient()`` or ``akismet.AsyncClient()``); the
-``validated_client()`` constructor will perform automatic discovery of the
-environment-variable configuration and validate the configuration with the Akismet web
-service before returning the client, while directly constructing an instance will not
-(so if you do directly construct an instance, you must manually provide and validate its
-configuration).
+You can also use either client class as a context manager. This does *not* require the
+``validated_client()`` constructor, because your API key is validated on entering the
+``with`` block.
+
+.. code-block:: python
+
+   import akismet
+
+   with akismet.SyncClient() as akismet_client:
+       if akismet_client.comment_check(
+           user_ip=submitter_ip,
+           comment_content=submitted_content,
+           comment_type="forum-post",
+           comment_author=submitter_name
+       ):
+           # This piece of content was classified as spam; handle it appropriately.
+
+Or using the asynchronous client:
+
+.. code-block:: python
+
+   import akismet
+
+   async with akismet.AsyncClient() as akismet_client:
+       if await akismet_client.comment_check(
+           user_ip=submitter_ip,
+           comment_content=submitted_content,
+           comment_type="forum-post",
+           comment_author=submitter_name
+       ):
+           # This piece of content was classified as spam; handle it appropriately.
 
 """
 
 # SPDX-License-Identifier: BSD-3-Clause
 
 from ._async_client import AsyncClient
 from ._common import USER_AGENT, CheckResponse, Config
@@ -73,14 +97,15 @@
     ConfigurationError,
     ProtocolError,
     RequestError,
     UnknownArgumentError,
 )
 from ._legacy_client import Akismet
 from ._sync_client import SyncClient
+from ._test_clients import TestAsyncClient, TestSyncClient
 from ._version import LIBRARY_VERSION
 
 __version__ = LIBRARY_VERSION
 
 __all__ = [
     "APIKeyError",
     "Akismet",
@@ -88,11 +113,12 @@
     "AsyncClient",
     "CheckResponse",
     "Config",
     "ConfigurationError",
     "ProtocolError",
     "RequestError",
     "SyncClient",
+    "TestAsyncClient",
+    "TestSyncClient",
     "UnknownArgumentError",
     "USER_AGENT",
-    "__version__",
 ]
```

### Comparing `akismet-1.3/src/akismet/_async_client.py` & `akismet-24.5.0/src/akismet/_async_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Asynchronous Akismet API client implementation.
 
 """
 
 # SPDX-License-Identifier: BSD-3-Clause
 
-import textwrap
-from typing import TYPE_CHECKING, Optional, Union
+from types import TracebackType
+from typing import TYPE_CHECKING, Literal, Optional, Type, Union
 
 import httpx
 
 from . import _common, _exceptions
 
 if TYPE_CHECKING:  # pragma: no cover
     import akismet
@@ -45,113 +45,133 @@
 
     This will automatically read the API key and site URL from the environment
     variables, instantiate a client, and use its :meth:`verify_key` method to ensure the
     key and URL are valid before returning the client instance to you. See :ref:`the FAQ
     <alt-constructor>` for the technical reasons why the default constructor does not
     have this behavior.
 
-    **Advanced/unusual use cases:** Instantiate the client directly. You must construct
-    a :class:`~akismet.Config` instance with your API key and site URL, and they will
-    *not* be automatically validated for you.
+    If you don't want to or can't use the environment variables to configure Akismet,
+    you can also explicitly configure by creating a :class:`~akismet.Config` instance
+    with your API key and site URL, and passing it as the constructor argument
+    ``config``:
 
     .. code-block:: python
 
        import akismet
        config = akismet.Config(key=your_api_key, url=your_site_url)
-       akismet_client = akismet.AsyncClient(config=config)
+       akismet_client = await akismet.AsyncClient.validated_client(config=config)
 
-    .. warning:: **Consequences of invalid configurationn**
-
-       If you construct an Akismet API client manually and provide an invalid key or
-       URL, all operations of the Akismet web service, other than key verification, will
-       reply with an invalid-key message. This will cause all client methods other than
-       :meth:`verify_key` to raise :exc:`akismet.APIKeyError`. To avoid this situation,
-       it is strongly recommended that you call :meth:`verify_key` to validate your
-       configuration prior to calling any other methods.
+    If you rely on environment variable configuration and the complete configuration
+    cannot be found in the environment variables, :meth:`validated_client` will raise
+    :exc:`~akismet.ConfigurationError`. If the API key and URL you supply are invalid
+    according to :meth:`verify_key` -- regardless of whether you provided them via
+    environment variables or an explicit :class:`~akismet.Config` --
+    :meth:`validated_client` will raise :exc:`~akismet.APIKeyError`.
 
     If you want to modify the HTTP request behavior -- for example, to support a
     required HTTP proxy -- you can construct a custom ``httpx.AsyncClient`` and pass it
     as the keyword argument ``http_client`` to either :meth:`validated_client` or the
     default constructor. See :data:`akismet.USER_AGENT` for the default user-agent
     string used by the Akismet API clients, and <https://www.python-httpx.org> for the
     full documentation of the HTTPX module.
 
+    Note that if you only want to set a custom request timeout threshold (the default is
+    1 second), you can specify it by setting the environment variable
+    ``PYTHON_AKISMET_TIMEOUT`` to a value that can be parsed into a :class:`float` or
+    :class:`int` and represents the desired timeout in seconds.
+
+    You can also use this class as a context manager; when doing so, you do *not* need
+    to use the :meth:`validated_client` constructor, as the context manager can perform
+    the validation for you when entering the ``with`` block:
+
     .. code-block:: python
 
        import akismet
-       import httpx
 
-       from your_app.config import settings
+       async with akismet.AsyncClient() as akismet_client:
+           # Use the client here. It will be automatically cleaned up when the "with"
+           # block exits.
+
+    **Unusual/advanced use cases:** Invoke the default constructor. It accepts the same
+    set of arguments as the :meth:`validated_client` constructor, and its behavior is
+    identical *except* for the fact that it will not automatically validate your
+    configuration, so you must remember to do so manually. You should only invoke the
+    default constructor if you are absolutely certain that you need to avoid the
+    automatic validation performed by :meth:`validated_client`.
 
-       akismet_client = await akismet.AsyncClient.validated_client(
-           http_client=httpx.AsyncClient(
-               proxy=settings.PROXY_URL,
-               headers={"User-Agent": akismet.USER_AGENT}
-           )
-       )
+    .. warning:: **Consequences of invalid configurationn**
 
-    Note that if you only want to set a custom request timeout threshold (the default is
-    1 second), you can specify it by setting the environment variable
-    ``PYTHON_AKISMET_TIMEOUT`` to a value that can be parsed into a :class:`float` or
-    :class:`int`.
+       If you construct an Akismet API client through the default constructor and
+       provide an invalid key or URL, all operations of the Akismet web service, other
+       than key verification, will reply with an invalid-key message. This will cause
+       all client methods other than :meth:`verify_key` to raise
+       :exc:`~akismet.APIKeyError`. To avoid this situation, it is strongly recommended
+       that you call :meth:`verify_key` to validate your configuration prior to calling
+       any other methods, at which point you likely should be using
+       :meth:`validated_client` anyway.
 
-    :param config: An Akismet :class:`~akismet.Config`, consisting of an API key and
-       site URL.
+    :param config: An optional Akismet :class:`~akismet.Config`, consisting of an API
+       key and site URL.
 
     :param http_client: An optional ``httpx`` async HTTP client instance to
        use. Generally you should only pass this in if you need significantly customized
        HTTP-client behavior, and if you do pass this argument you are responsible for
        setting an appropriate ``User-Agent`` (see :data:`~akismet.USER_AGENT`), timeout,
        and other configuration values. If all you want is to change the default timeout
-       (1 second), store the desired timeout as a floating-point or integer value in the
-       environment variable ``PYTHON_AKISMET_TIMEOUT``.
+       (1 second), store the desired timeout, in seconds, as a floating-point or integer
+       value in the environment variable ``PYTHON_AKISMET_TIMEOUT``.
 
     """
 
     _http_client: httpx.AsyncClient
-    _config: _common.Config
+    _config: "akismet.Config"
 
     # Constructors.
     # ----------------------------------------------------------------------------
 
     def __init__(
         self,
-        config: _common.Config,
+        config: Optional["akismet.Config"] = None,
         http_client: Optional[httpx.AsyncClient] = None,
     ) -> None:
         """
         Default constructor.
 
         You will almost always want to use :meth:`validated_client` instead.
 
         """
+        self._config = config if config is not None else _common._try_discover_config()
         self._http_client = http_client or _common._get_async_http_client()
-        self._config = config
 
     @classmethod
     async def validated_client(
-        cls, http_client: Optional[httpx.AsyncClient] = None
+        cls,
+        config: Optional["akismet.Config"] = None,
+        http_client: Optional[httpx.AsyncClient] = None,
     ) -> "AsyncClient":
         """
         Constructor of :class:`AsyncClient`.
 
         This is usually preferred over the default ``AsyncClient()`` constructor,
-        because this constructor will discover and validate the Akismet configuration
-        (API key and URL) prior to returning the client instance. The Akismet API key
-        will be read from the environment variable ``PYTHON_AKISMET_API_KEY``, and the
-        registered site URL from the environment variable ``PYTHON_AKISMET_BLOG_URL``.
+        because this constructor will validate the Akismet configuration (API key and
+        URL) prior to returning the client instance.
+
+        :param config: An optional explicit Akismet :class:`~akismet.Config`, consisting
+           of an API key and site URL; if not passed, the configuration will be read
+           from the environment variables ``PYTHON_AKISMET_API_KEY`` and
+           ``PYTHON_AKISMET_BLOG_URL``.
 
         :param http_client: An optional ``httpx`` async HTTP client instance to
            use. Generally you should only pass this in if you need significantly
            customized HTTP-client behavior, and if you do pass this argument you are
            responsible for setting an appropriate ``User-Agent`` (see
            :data:`~akismet.USER_AGENT`), timeout, and other configuration values. If all
            you want is to change the default timeout (1 second), store the desired
-           timeout as a floating-point or integer value in the environment variable
-           ``PYTHON_AKISMET_TIMEOUT``.
+           timeout, in seconds, as a floating-point or integer value in the environment
+           variable ``PYTHON_AKISMET_TIMEOUT``.
 
         :raises akismet.APIKeyError: When the discovered Akismet configuration is
            invalid according to :meth:`verify_key`.
 
         :raises akismet.ConfigurationError: When the Akismet configuration is partially
            or completely missing, or when the supplied site URL is in the wrong format
            (does not begin with ``http://`` or ``https://``).
@@ -160,29 +180,40 @@
         # While the synchronous version of the client could perform the config discovery
         # and validation in __init__(), here we cannot because this client's
         # verify_key() method is async, and its underlying HTTP client is async. So
         # calling into them would require making __init__ into an async method, and
         # Python does not currently allow __init__() to be usefully async. But a
         # classmethod *can* be async, so we define and encourage the use of an
         # alternative constructor in order to achieve API consistency.
-        config = _common._try_discover_config()
         instance = cls(config=config, http_client=http_client)
-        if not await instance.verify_key(config.key, config.url):
-            raise _exceptions.APIKeyError(
-                textwrap.dedent(
-                    f"""
-                    Akismet API key and/or blog URL were invalid.
-
-                    Found API key: {config.key}
-                    Found blog URL: {config.url}
-                    """
-                )
-            )
+        if not await instance.verify_key():
+            _common._configuration_error(instance._config)
         return instance
 
+    # Async context-manager protocol.
+    # ----------------------------------------------------------------------------
+
+    async def __aenter__(self) -> "AsyncClient":
+        """
+        Entry method of the async context manager.
+
+        """
+        if not await self.verify_key():
+            _common._configuration_error(self._config)
+        return self
+
+    async def __aexit__(
+        self, exc_type: Type[BaseException], exc: BaseException, tb: TracebackType
+    ):
+        """
+        Exit method of the async context manager.
+
+        """
+        await self._http_client.aclose()
+
     # Internal/helper methods.
     # ----------------------------------------------------------------------------
 
     async def _request(
         self,
         method: _common._REQUEST_METHODS,
         version: str,
@@ -277,15 +308,15 @@
            <https://akismet.com/developers/comment-check/>`_ for details of supported
            optional argument names.
 
         """
         unknown_args = [k for k in kwargs if k not in _common._OPTIONAL_KEYS]
         if unknown_args:
             raise _exceptions.UnknownArgumentError(
-                f"Received unknown argument(s) for Akismet operation {endpoint}"
+                f"Received unknown argument(s) for Akismet operation {endpoint}: "
                 f"{', '.join(unknown_args)}"
             )
         data = {
             "api_key": self._config.key,
             "blog": self._config.url,
             "user_ip": user_ip,
             **kwargs,
@@ -451,15 +482,15 @@
         """
         return await self._submit(_common._SUBMIT_SPAM, user_ip, **kwargs)
 
     async def key_sites(  # pylint: disable=too-many-arguments
         self,
         month: Optional[str] = None,
         url_filter: Optional[str] = None,
-        result_format: Optional[str] = None,
+        result_format: Literal["csv", "json"] = "json",
         order: Optional[str] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
     ) -> Union[dict, str]:
         """
         Return Akismet API usage statistics keyed by site.
 
@@ -515,32 +546,38 @@
 
         """
         response = await self._get_request(
             _common._API_V12, _common._USAGE_LIMIT, params={"api_key": self._config.key}
         )
         return response.json()
 
-    async def verify_key(self, key: str, url: str) -> bool:
+    async def verify_key(
+        self, key: Optional[str] = None, url: Optional[str] = None
+    ) -> bool:
         """
         Verify an Akismet API key and URL.
 
         Return :data:`True` if the key and URL are valid, :data:`False` otherwise.
 
         In general, you should not need to explicitly call this method. The
         :meth:`validated_client` constructor will ensure this method is called during
-        client construction, after which the now-verified key/URL can be trusted.
+        client construction, after which the now-verified key/URL can be trusted. If
+        neither ``key`` nor ``url`` are provided, the key and URL currently in use by
+        this client will be checked.
 
         :param key: The API key to check.
 
         :param url: The URL to check.
 
         :raises akismet.ProtocolError: When an unexpected/invalid response type is
            received from the Akismet API.
 
         """
+        if not all([key, url]):
+            key, url = self._config
         response = await self._request(
             "POST", _common._API_V11, _common._VERIFY_KEY, {"key": key, "blog": url}
         )
         if response.text == "valid":
             return True
         if response.text == "invalid":
             return False
```

### Comparing `akismet-1.3/src/akismet/_common.py` & `akismet-24.5.0/src/akismet/_common.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,27 +83,44 @@
 
 class Config(typing.NamedTuple):
     """
     A :func:`~collections.namedtuple` representing Akismet configuration, consisting
     of a key and a URL.
 
     You only need to use this if you're manually configuring an Akismet API client
-    (which should be rare) rather than letting the ``validated_client()`` constructor
-    automatically read the configuration from environment variables.
+    rather than letting the configuration be read automatically from environment
+    variables.
 
     """
 
     key: str
     url: str
 
 
 # Private helper functions.
 # -------------------------------------------------------------------------------
 
 
+def _configuration_error(config: Config) -> typing.NoReturn:
+    """
+    Raise an appropriate exception for invalid configuration.
+
+    """
+    raise _exceptions.APIKeyError(
+        textwrap.dedent(
+            f"""
+            Akismet API key and/or blog URL were invalid.
+
+            Found API key: {config.key}
+            Found URL: {config.url}
+            """
+        )
+    )
+
+
 def _get_async_http_client() -> httpx.AsyncClient:
     """
     Return an asynchronous HTTP client for interacting with the Akismet API.
 
     """
     return httpx.AsyncClient(headers={"User-Agent": USER_AGENT}, timeout=_TIMEOUT)
```

### Comparing `akismet-1.3/src/akismet/_exceptions.py` & `akismet-24.5.0/src/akismet/_exceptions.py`

 * *Files identical despite different names*

### Comparing `akismet-1.3/src/akismet/_legacy_client.py` & `akismet-24.5.0/src/akismet/_legacy_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,16 @@
         blog_url: Optional[str] = None,
         http_client: Optional[httpx.Client] = None,
     ):
         warnings.warn(
             textwrap.dedent(
                 """
             The akismet.Akismet API client is deprecated and will be removed in
-            version 2.0. Please migrate to either akismet.SyncClient or
-            akismet.AsyncClient.  """,
+            2025. Please migrate to either akismet.SyncClient or akismet.AsyncClient.
+            """,
             ),
             DeprecationWarning,
             stacklevel=2,
         )
         maybe_key = key if key is not None else os.getenv(_common._KEY_ENV_VAR, "")
         maybe_url = (
             blog_url if blog_url is not None else os.getenv(_common._URL_ENV_VAR, "")
```

### Comparing `akismet-1.3/src/akismet/_sync_client.py` & `akismet-24.5.0/src/akismet/_sync_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Synchronous Akismet API client implementation.
 
 """
 
 # SPDX-License-Identifier: BSD-3-Clause
 
-import textwrap
-from typing import TYPE_CHECKING, Optional, Union
+from types import TracebackType
+from typing import TYPE_CHECKING, Literal, Optional, Type, Union
 
 import httpx
 
 from . import _common, _exceptions
 
 if TYPE_CHECKING:  # pragma: no cover
     import akismet
@@ -45,111 +45,133 @@
 
     This will automatically read the API key and site URL from the environment
     variables, instantiate a client, and use its :meth:`verify_key` method to ensure the
     key and URL are valid before returning the client instance to you. See :ref:`the FAQ
     <alt-constructor>` for the technical reasons why the default constructor does not
     have this behavior.
 
-    **Advanced/unusual use cases:** Instantiate the client directly. You must construct
-    a :class:`~akismet.Config` instance with your API key and site URL, and they will
-    *not* be automatically validated for you.
+    If you don't want to or can't use the environment variables to configure Akismet,
+    you can also explicitly configure by creating a :class:`~akismet.Config` instance
+    with your API key and site URL, and passing it as the constructor argument
+    ``config``:
 
     .. code-block:: python
 
        import akismet
        config = akismet.Config(key=your_api_key, url=your_site_url)
-       akismet_client = akismet.SyncClient(config=config)
+       akismet_client = akismet.SyncClient.validated_client(config=config)
 
-    .. warning:: **Consequences of invalid configurationn**
-
-       If you construct an Akismet API client manually and provide an invalid key or
-       URL, all operations of the Akismet web service, other than key verification, will
-       reply with an invalid-key message. This will cause all client methods other than
-       :meth:`verify_key` to raise :exc:`akismet.APIKeyError`. To avoid this situation,
-       it is strongly recommended that you call :meth:`verify_key` to validate your
-       configuration prior to calling any other methods.
+    If you rely on environment variable configuration and the complete configuration
+    cannot be found in the environment variables, :meth:`validated_client` will raise
+    :exc:`~akismet.ConfigurationError`. If the API key and URL you supply are invalid
+    according to :meth:`verify_key` -- regardless of whether you provided them via
+    environment variables or an explicit :class:`~akismet.Config` --
+    :meth:`validated_client` will raise :exc:`~akismet.APIKeyError`.
 
     If you want to modify the HTTP request behavior -- for example, to support a
     required HTTP proxy -- you can construct a custom ``httpx.Client`` and pass it as
     the keyword argument ``http_client`` to either :meth:`validated_client` or the
     default constructor. See :data:`akismet.USER_AGENT` for the default user-agent
     string used by the Akismet API clients, and <https://www.python-httpx.org> for the
     full documentation of the HTTPX module.
 
-    .. code-block:: python
+    Note that if you only want to set a custom request timeout threshold (the default is
+    1 second), you can specify it by setting the environment variable
+    ``PYTHON_AKISMET_TIMEOUT`` to a value that can be parsed into a :class:`float` or
+    :class:`int` and represents the desired timeout in seconds.
 
-       import akismet
-       import httpx
+    You can also use this class as a context manager; when doing so, you do *not* need
+    to use the :meth:`validated_client` constructor, as the context manager can perform
+    the validation for you when entering the ``with`` block.
 
-       from your_app.config import settings
+    .. code-block:: python
 
-       akismet_client = akismet.SyncClient.validated_client(
-           http_client=httpx.Client(
-               proxy=settings.PROXY_URL,
-               headers={"User-Agent": akismet.USER_AGENT}
-           )
-       )
+       import akismet
 
-    Note that if you only want to set a custom request timeout threshold (the default is
-    1 second), you can specify it by setting the environment variable
-    ``PYTHON_AKISMET_TIMEOUT`` to a value that can be parsed into a :class:`float` or
-    :class:`int`.
+       with akismet.SyncClient() as akismet_client:
+           # Use the client here. It will be automatically cleaned up when the "with"
+           # block exits.
+
+    **Unusual/advanced use cases:** Invoke the default constructor. It accepts the same
+    set of arguments as the :meth:`validated_client` constructor, and its behavior is
+    identical *except* for the fact that it will not automatically validate your
+    configuration, so you must remember to do so manually. You should only invoke the
+    default constructor if you are absolutely certain that you need to avoid the
+    automatic validation performed by :meth:`validated_client`.
 
-    :param config: An Akismet :class:`~akismet.Config`, consisting of an API key and
-       site URL.
+    .. warning:: **Consequences of invalid configurationn**
 
-    :param http_client: An optional custom ``httpx`` HTTP client instance to
-       use. Generally you should only pass this in if you need significantly customized
-       HTTP-client behavior, and if you do pass this argument you are responsible for
-       setting an appropriate ``User-Agent`` (see :data:`~akismet.USER_AGENT`), timeout,
-       and other configuration values. If all you want is to change the default timeout
-       (1 second), store the desired timeout as a floating-point or integer value in the
-       environment variable ``PYTHON_AKISMET_TIMEOUT``.
+       If you construct an Akismet API client through the default constructor and
+       provide an invalid key or URL, all operations of the Akismet web service, other
+       than key verification, will reply with an invalid-key message. This will cause
+       all client methods other than :meth:`verify_key` to raise
+       :exc:`~akismet.APIKeyError`. To avoid this situation, it is strongly recommended
+       that you call :meth:`verify_key` to validate your configuration prior to calling
+       any other methods, at which point you likely should be using
+       :meth:`validated_client` anyway.
+
+    :param config: An optional Akismet :class:`~akismet.Config`, consisting of an API
+       key and site URL.
+
+    :param http_client: An optional ``httpx`` HTTP client instance to use. Generally you
+       should only pass this in if you need significantly customized HTTP-client
+       behavior, and if you do pass this argument you are responsible for setting an
+       appropriate ``User-Agent`` (see :data:`~akismet.USER_AGENT`), timeout, and other
+       configuration values. If all you want is to change the default timeout (1
+       second), store the desired timeout, in seconds, as a floating-point or integer
+       value in the environment variable ``PYTHON_AKISMET_TIMEOUT``.
 
     """
 
     _http_client: httpx.Client
-    _config: _common.Config
+    _config: "akismet.Config"
 
     # Constructors.
     # ----------------------------------------------------------------------------
 
     def __init__(
-        self, config: _common.Config, http_client: Optional[httpx.Client] = None
+        self,
+        config: Optional["akismet.Config"] = None,
+        http_client: Optional[httpx.Client] = None,
     ) -> None:
         """
         Default constructor.
 
         You will almost always want to use :meth:`validated_client` instead.
 
         """
+        self._config = config if config is not None else _common._try_discover_config()
         self._http_client = http_client or _common._get_sync_http_client()
-        self._config = config
 
     @classmethod
     def validated_client(
-        cls, http_client: Optional[httpx.Client] = None
+        cls,
+        config: Optional["akismet.Config"] = None,
+        http_client: Optional[httpx.Client] = None,
     ) -> "SyncClient":
         """
         Constructor of :class:`SyncClient`.
 
         This is usually preferred over the default ``SyncClient()`` constructor, because
-        this constructor will discover and validate the Akismet configuration (API key
-        and URL) prior to returning the client instance. The Akismet API key will be
-        read from the environment variable ``PYTHON_AKISMET_API_KEY``, and the
-        registered site URL from the environment variable ``PYTHON_AKISMET_BLOG_URL``.
+        this constructor will validate the Akismet configuration (API key and URL) prior
+        to returning the client instance.
+
+        :param config: An optional explicit Akismet :class:`~akismet.Config`, consisting
+           of an API key and site URL; if not passed, the configuration will be read
+           from the environment variables ``PYTHON_AKISMET_API_KEY`` and
+           ``PYTHON_AKISMET_BLOG_URL``.
 
         :param http_client: An optional custom ``httpx`` HTTP client instance to
            use. Generally you should only pass this in if you need significantly
            customized HTTP-client behavior, and if you do pass this argument you are
            responsible for setting an appropriate ``User-Agent`` (see
            :data:`~akismet.USER_AGENT`), timeout, and other configuration values. If all
            you want is to change the default timeout (1 second), store the desired
-           timeout as a floating-point or integer value in the environment variable
-           ``PYTHON_AKISMET_TIMEOUT``.
+           timeout, in seconds, as a floating-point or integer value in the environment
+           variable ``PYTHON_AKISMET_TIMEOUT``.
 
         :raises akismet.APIKeyError: When the discovered Akismet configuration is
            invalid according to :meth:`verify_key`.
 
         :raises akismet.ConfigurationError: When the Akismet configuration is partially
            or completely missing, or when the supplied site URL is in the wrong format
            (does not begin with ``http://`` or ``https://``).
@@ -159,29 +181,40 @@
         # __init__(). However, we want to ensure parity between this class' API and the
         # async client's API, and the async client would not be able to perform config
         # validation in __init__(): the async client would need to call an async HTTP
         # request method, which would require the client's __init__() to become async,
         # and Python does not currently allow __init__() to be usefully async. But a
         # classmethod *can* be async, so we define and encourage the use of an alternate
         # constructor in order to achieve API consistency.
-        config = _common._try_discover_config()
         instance = cls(config=config, http_client=http_client)
-        if not instance.verify_key(config.key, config.url):
-            raise _exceptions.APIKeyError(
-                textwrap.dedent(
-                    f"""
-                    Akismet API key and/or blog URL were invalid.
-
-                    Found API key: {config.key}
-                    Found blog URL: {config.url}
-                    """
-                )
-            )
+        if not instance.verify_key():
+            _common._configuration_error(instance._config)
         return instance
 
+    # Context-manager protocol.
+    # ----------------------------------------------------------------------------
+
+    def __enter__(self) -> "SyncClient":
+        """
+        Entry method of the context manager.
+
+        """
+        if not self.verify_key():
+            _common._configuration_error(self._config)
+        return self
+
+    def __exit__(
+        self, exc_type: Type[BaseException], exc: BaseException, tb: TracebackType
+    ):
+        """
+        Exit method of the context manager.
+
+        """
+        self._http_client.close()
+
     # Internal/helper methods.
     # ----------------------------------------------------------------------------
 
     def _request(
         self,
         method: _common._REQUEST_METHODS,
         version: str,
@@ -274,15 +307,15 @@
            <https://akismet.com/developers/comment-check/>`_ for details of supported
            optional argument names.
 
         """
         unknown_args = [k for k in kwargs if k not in _common._OPTIONAL_KEYS]
         if unknown_args:
             raise _exceptions.UnknownArgumentError(
-                f"Received unknown argument(s) for Akismet operation {endpoint}"
+                f"Received unknown argument(s) for Akismet operation {endpoint}: "
                 f"{', '.join(unknown_args)}"
             )
         data = {
             "api_key": self._config.key,
             "blog": self._config.url,
             "user_ip": user_ip,
             **kwargs,
@@ -446,15 +479,15 @@
         """
         return self._submit(_common._SUBMIT_SPAM, user_ip, **kwargs)
 
     def key_sites(  # pylint: disable=too-many-arguments
         self,
         month: Optional[str] = None,
         url_filter: Optional[str] = None,
-        result_format: Optional[str] = None,
+        result_format: Literal["csv", "json"] = "json",
         order: Optional[str] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
     ) -> Union[dict, str]:
         """
         Return Akismet API usage statistics keyed by site.
 
@@ -510,32 +543,36 @@
 
         """
         response = self._get_request(
             _common._API_V12, _common._USAGE_LIMIT, params={"api_key": self._config.key}
         )
         return response.json()
 
-    def verify_key(self, key: str, url: str) -> bool:
+    def verify_key(self, key: Optional[str] = None, url: Optional[str] = None) -> bool:
         """
         Verify an Akismet API key and URL.
 
         Return :data:`True` if the key and URL are valid, :data:`False` otherwise.
 
         In general, you should not need to explicitly call this method. The
         :meth:`validated_client` constructor will ensure this method is called during
-        client construction, after which the now-verified key/URL can be trusted.
+        client construction, after which the now-verified key/URL can be trusted. If
+        neither ``key`` nor ``url`` are provided, the key and URL currently in use by
+        this client will be checked.
 
         :param key: The API key to check.
 
         :param url: The URL to check.
 
         :raises akismet.ProtocolError: When an unexpected/invalid response type is
            received from the Akismet API.
 
         """
+        if not all([key, url]):
+            key, url = self._config
         response = self._request(
             "POST", _common._API_V11, _common._VERIFY_KEY, {"key": key, "blog": url}
         )
         if response.text == "valid":
             return True
         if response.text == "invalid":
             return False
```

### Comparing `akismet-1.3/src/akismet.egg-info/PKG-INFO` & `akismet-24.5.0/src/akismet.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: akismet
-Version: 1.3
+Version: 24.5.0
 Summary: A Python interface to the Akismet spam-filtering service.
-Author: Michael Foord
-Author-email: James Bennett <james@b-list.org>
+Author: Michael Foord, James Bennett
+Maintainer: James Bennett
 License: BSD-3-Clause
-Project-URL: documentation, https://akismet.readthedocs.io
-Project-URL: homepage, https://github.com/ubernostrum/akismet
+Project-URL: Documentation, https://akismet.readthedocs.io
+Project-URL: Source Code, https://github.com/ubernostrum/akismet
 Keywords: akismet,spam,spam-filtering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -52,25 +52,27 @@
 
 * ``akismet.AsyncClient`` is an Akismet API client which performs
   asynchronous (``async``/``await``/non-blocking) HTTP requests to the
   Akismet web service.
 
 Aside from one being sync and the other async, the two clients expose
 identical APIs, and implement all methods of `the Akismet web API
-<https://akismet.com/developers/>`_, including the v1.2 key and API
-usage metrics.
+<https://akismet.com/developers/>`_.
 
 To use this library, you will need to obtain an Akismet API key and
 register a site for use with the Akismet web service; you can do this
 at <https://akismet.com>. Once you have a key and corresponding
 registered site URL to use with it, place them in the environment
 variables ``PYTHON_AKISMET_API_KEY`` and ``PYTHON_AKISMET_BLOG_URL``,
 and they will be automatically detected and used.
 
 You can then construct a client instance and call its methods. For
+creating a long-lived API client instance, it's recommended that you
+use the ``validated_client()`` constructor method, which will
+automatically validate your API key with the Akismet web service. For
 example, to check a submitted forum post for spam:
 
 .. code-block:: python
 
    import akismet
 
    akismet_client = akismet.SyncClient.validated_client()
@@ -95,22 +97,45 @@
        user_ip=submitter_ip,
        comment_content=submitted_content,
        comment_type="forum-post",
        comment_author=submitter_name
    ):
        # This piece of content was classified as spam; handle it appropriately.
 
-Note that in both cases the client instance is created via the
-alternate constructor ``validated_client()``. This is recommended
-instead of using the default constructor (i.e., directly calling
-``akismet.SyncClient()`` or ``akismet.AsyncClient()``); the
-``validated_client()`` constructor will perform automatic discovery of
-the environment-variable configuration and validate the configuration
-with the Akismet web service before returning the client, while
-directly constructing an instance will not (so if you do directly
-construct an instance, you must manually provide and validate its
-configuration).
+You can also use either client class as a context manager. This does
+*not* require the ``validated_client()`` constructor, because your API
+key is validated on entering the ``with`` block.
+
+.. code-block:: python
+
+   import akismet
+
+   with akismet.SyncClient() as akismet_client:
+       if akismet_client.comment_check(
+           user_ip=submitter_ip,
+           comment_content=submitted_content,
+           comment_type="forum-post",
+           comment_author=submitter_name
+       ):
+           # This piece of content was classified as spam; handle it appropriately.
+
+Or using the asynchronous client:
+
+.. code-block:: python
+
+   import akismet
+
+   async with akismet.AsyncClient() as akismet_client:
+       if await akismet_client.comment_check(
+           user_ip=submitter_ip,
+           comment_content=submitted_content,
+           comment_type="forum-post",
+           comment_author=submitter_name
+       ):
+           # This piece of content was classified as spam; handle it appropriately.
+
+
 
 See `the documentation <http://akismet.readthedocs.io/>`_ for full
 details.
 
 The original version of this library was written by Michael Foord.
```

### Comparing `akismet-1.3/src/akismet.egg-info/SOURCES.txt` & `akismet-24.5.0/src/akismet.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,37 +7,40 @@
 MANIFEST.in
 README.rst
 noxfile.py
 pyproject.toml
 tox.ini
 docs/Makefile
 docs/async_client.rst
+docs/changelog.rst
 docs/conf.py
 docs/exceptions.rst
 docs/faq.rst
 docs/index.rst
 docs/install.rst
 docs/make.bat
 docs/misc.rst
 docs/spelling_wordlist.txt
 docs/sync_client.rst
+docs/test_clients.rst
 docs/testing.rst
-docs/upgrade.rst
 docs/usage.rst
 src/akismet/__init__.py
 src/akismet/_async_client.py
 src/akismet/_common.py
 src/akismet/_exceptions.py
 src/akismet/_legacy_client.py
 src/akismet/_sync_client.py
+src/akismet/_test_clients.py
 src/akismet/_version.py
 src/akismet.egg-info/PKG-INFO
 src/akismet.egg-info/SOURCES.txt
 src/akismet.egg-info/dependency_links.txt
 src/akismet.egg-info/requires.txt
 src/akismet.egg-info/top_level.txt
 tests/__init__.py
 tests/base.py
 tests/end_to_end.py
 tests/test_async_client.py
 tests/test_legacy_client.py
-tests/test_sync_client.py
+tests/test_sync_client.py
+tests/test_test_clients.py
```

### Comparing `akismet-1.3/tests/end_to_end.py` & `akismet-24.5.0/tests/end_to_end.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             os.environ[_common._URL_ENV_VAR] = self.site_url
 
     def test_verify_key_valid(self):
         """
         ``verify_key()`` returns True when the config is valid.
 
         """
-        assert self.client.verify_key(self.api_key, self.site_url)
+        assert self.client.verify_key()
 
     def test_verify_key_invalid(self):
         """
         ``verify_key()`` returns False when the config is invalid.
 
         """
         assert not self.client.verify_key(BAD_KEY, BAD_URL)
@@ -174,15 +174,15 @@
             os.environ[_common._URL_ENV_VAR] = self.site_url
 
     async def test_verify_key_valid(self):
         """
         ``verify_key()`` returns True when the config is valid.
 
         """
-        assert await self.client.verify_key(self.api_key, self.site_url)
+        assert await self.client.verify_key()
 
     async def test_verify_key_invalid(self):
         """
         ``verify_key()`` returns False when the config is invalid.
 
         """
         assert not await self.client.verify_key(BAD_KEY, BAD_URL)
```

### Comparing `akismet-1.3/tests/test_async_client.py` & `akismet-24.5.0/tests/test_async_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,195 @@
 """
 Tests for the asynchronous Akismet API client.
 
 """
 
 # SPDX-License-Identifier: BSD-3-Clause
 
+import csv
 import os
-import textwrap
+import typing
 from http import HTTPStatus
+from unittest import mock
 
 import httpx
 
 import akismet
-from akismet import _common
+from akismet import _common, _test_clients
 
-from .base import AsyncAkismetTests
+from . import base
 
 
-class AsyncAkismetConstructorTests(AsyncAkismetTests):
+def make_fixed_response_async_client(
+    response_text: str = "true",
+    status_code: HTTPStatus = HTTPStatus.OK,
+    response_json: typing.Optional[dict] = None,
+) -> httpx.AsyncClient:
     """
-    Test the ``client()`` constructor of the asynchronous Akismet API client.
+    Return an asynchronous HTTP client that produces a fixed repsonse, for use in
+    testing.
 
     """
+    return httpx.AsyncClient(
+        transport=base.make_fixed_response_transport(
+            response_text, status_code, response_json
+        )
+    )
+
+
+def make_exception_async_client(
+    exception_class: Exception, message: str = "Error!"
+) -> httpx.AsyncClient:
+    """
+    Return an asynchronous HTTP client that raises the given exception/message.
+
+    """
+    return mock.AsyncMock(
+        spec_set=httpx.AsyncClient,
+        get=mock.AsyncMock(side_effect=exception_class(message)),
+        post=mock.AsyncMock(side_effect=exception_class(message)),
+    )
+
+
+class ValidConfig(akismet.TestAsyncClient):
+    """
+    Test client with valid config.
+
+    """
+
+    verify_key_response = True
+
+
+class InvalidConfig(akismet.TestAsyncClient):
+    """
+    Test client with invalid config.
+
+    """
+
+    verify_key_response = False
+
+
+class AlwaysBlatantSpam(akismet.TestAsyncClient):
+    """
+    Test client which marks all content as "blatant" spam.
+
+    """
+
+    comment_check_response = akismet.CheckResponse.DISCARD
+
+
+class AlwaysSpam(akismet.TestAsyncClient):
+    """
+    Test client which marks all content as spam.
+
+    """
+
+    comment_check_response = akismet.CheckResponse.SPAM
+
+
+class NeverSpam(akismet.TestAsyncClient):
+    """
+    Test client which marks all content as not spam.
+
+    """
+
+    comment_check_response = akismet.CheckResponse.HAM
+
+
+class AsyncAkismetConstructorTests(base.AsyncAkismetTests):
+    """
+    Test the constructors of the asynchronous Akismet API client.
+
+    """
+
+    async def test_construct_config_explicit(self):
+        """
+        Passing explicit config to the default constructor uses that config.
+
+        """
+        config = akismet.Config(key="other-invalid-test-key", url=self.config.url)
+        async with ValidConfig(config=config) as client:
+            assert client._config == config
+
+    async def test_construct_config_alternate_constructor_explicit(self):
+        """
+        Passing explicit config to the alternate constructor uses that config.
+
+        """
+        config = akismet.Config(key="other-invalid-test-key", url=self.config.url)
+        client = await ValidConfig.validated_client(config=config)
+        assert client._config == config
+
+    async def test_construct_config_from_env(self):
+        """
+        Instantiating via the default constructor, without passing explicit config,
+        reads the config from the environment.
+
+        """
+        config = akismet.Config(key=self.api_key, url=self.site_url)
+        async with ValidConfig() as client:
+            assert client._config == config
+
+    async def test_construct_alternate_constructor_config_from_env(self):
+        """
+        Instantiating via the alternate constructor, without passing explicit
+        config, reads the config from the environment.
+
+        """
+        config = akismet.Config(key=self.api_key, url=self.site_url)
+        client = await ValidConfig.validated_client()
+        assert client._config == config
 
     async def test_construct_config_valid(self):
         """
         With a valid configuration, constructing a client succeeds.
 
         """
-        await akismet.AsyncClient.validated_client(
-            http_client=self.custom_response_async_client()
-        )
+        await ValidConfig.validated_client()
 
     async def test_construct_config_invalid_key(self):
         """
         With an invalid API key, constructing a client raises an APIKeyError.
 
         """
         with self.assertRaises(akismet.APIKeyError):
-            await akismet.AsyncClient.validated_client(
-                http_client=self.custom_response_async_client(config_valid=False)
-            )
+            await InvalidConfig.validated_client()
+
+    async def test_construct_config_valid_context_manager(self):
+        """
+        With a valid configuration, constructing a client as a context manager succeeds.
+
+        """
+        async with ValidConfig():
+            pass
+
+    async def test_construct_config_invalid_key_context_manager(self):
+        """
+        With an invalid API key, constructing a client as a context manager raises
+        an APIKeyError.
+
+        """
+        with self.assertRaises(akismet.APIKeyError):
+            async with InvalidConfig():
+                pass
+
+    async def test_construct_config_valid_explicit(self):
+        """
+        With an explicit valid configuration, constructing a client succeeds.
+
+        """
+        await ValidConfig.validated_client(config=self.config)
+
+    async def test_construct_config_invalid_key_explicit(self):
+        """
+        With an explicit invalid API key, constructing a client raises an APIKeyError.
+
+        """
+        with self.assertRaises(akismet.APIKeyError):
+            await InvalidConfig.validated_client(config=self.config)
 
     async def test_construct_config_bad_url(self):
         """
         With an invalid URL, constructing a client raises a ConfigurationError.
 
         """
         try:
@@ -60,33 +205,29 @@
         ConfigurationError.
 
         """
         try:
             if _common._KEY_ENV_VAR in os.environ:
                 del os.environ[_common._KEY_ENV_VAR]
             with self.assertRaises(akismet.ConfigurationError):
-                await akismet.AsyncClient.validated_client(
-                    http_client=self.custom_response_async_client()
-                )
+                await ValidConfig.validated_client()
         finally:
             os.environ[_common._KEY_ENV_VAR] = self.api_key
 
     async def test_construct_config_missing_url(self):
         """
         Without a registered site URL present, constructing a client raises a
         ConfigurationError.
 
         """
         try:
             if _common._URL_ENV_VAR in os.environ:
                 del os.environ[_common._URL_ENV_VAR]
             with self.assertRaises(akismet.ConfigurationError):
-                await akismet.AsyncClient.validated_client(
-                    http_client=self.custom_response_async_client()
-                )
+                await ValidConfig.validated_client()
         finally:
             os.environ[_common._URL_ENV_VAR] = self.site_url
 
     async def test_construct_config_missing_all(self):
         """
         Without any config present, constructing a client raises a
         ConfigurationError.
@@ -94,49 +235,44 @@
         """
         try:
             if _common._KEY_ENV_VAR in os.environ:
                 del os.environ[_common._KEY_ENV_VAR]
             if _common._URL_ENV_VAR in os.environ:
                 del os.environ[_common._URL_ENV_VAR]
             with self.assertRaises(akismet.ConfigurationError):
-                await akismet.AsyncClient.validated_client(
-                    http_client=self.custom_response_async_client()
-                )
+                await ValidConfig.validated_client()
         finally:
             os.environ[_common._KEY_ENV_VAR] = self.api_key
             os.environ[_common._URL_ENV_VAR] = self.site_url
 
     async def test_construct_default_client(self):
         """
         Constructing a client without an explicit HTTP client uses the default HTTP
         client.
 
         """
-        client = akismet.AsyncClient(config=self.config)
+        client = akismet.AsyncClient()
         http_client = client._http_client
         assert "user-agent" in http_client.headers
         assert http_client.headers["user-agent"] == _common.USER_AGENT
 
 
-class AsyncAkismetAPITests(AsyncAkismetTests):
+class AsyncAkismetAPITests(base.AsyncAkismetTests):
     """
     Test the API behavior of the asynchronous Akismet API client.
 
     """
 
     async def test_unsupported_request_method(self):
         """
         Attempting to make a request with an unsupported method raises
         ``AkismetError``.
 
         """
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(),
-        )
+        client = ValidConfig()
         # The tested set of methods here are all the methods that are in Python 3.11's
         # http.HTTPMethod enum but not supported for Akismet requests.
         for bad_method in (
             "CONNECT",
             "DELETE",
             "HEAD",
             "OPTIONS",
@@ -154,40 +290,51 @@
                     )
 
     async def test_verify_key_valid(self):
         """
         ``verify_key()`` returns True when the config is valid.
 
         """
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(),
-        )
-        assert await client.verify_key(key=self.api_key, url=self.site_url)
+        async with ValidConfig() as client:
+            assert await client.verify_key()
 
     async def test_verify_key_invalid(self):
         """
         ``verify_key()`` returns False when the config is invalid.
 
         """
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(config_valid=False),
-        )
+        client = InvalidConfig()
+        assert not await client.verify_key()
+
+    async def test_verify_key_valid_explicit(self):
+        """
+        ``verify_key()`` returns True when the config is valid and explicitly passed
+        in.
+
+        """
+        async with ValidConfig() as client:
+            assert await client.verify_key(key=self.api_key, url=self.site_url)
+
+    async def test_verify_key_invalid_explicit(self):
+        """
+        ``verify_key()`` returns False when the config is invalid and explicitly
+        passed in.
+
+        """
+        client = InvalidConfig()
         assert not await client.verify_key(key=self.api_key, url=self.site_url)
 
     async def test_request_with_invalid_key(self):
         """
         The request methods other than ``verify_key()`` raise
         ``akismet.APIKeyError`` if called with an invalid API key/URL.
 
         """
         client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(response_text="invalid"),
+            http_client=make_fixed_response_async_client(response_text="invalid"),
         )
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.APIKeyError):
                     await getattr(client, method)(**self.common_kwargs)
         for method in ("key_sites", "usage_limit"):
             with self.subTest(method=method):
@@ -196,204 +343,160 @@
 
     async def test_comment_check_spam(self):
         """
         ``comment_check()`` returns the SPAM value when Akismet declares the content
         to be spam.
 
         """
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(response_text="true"),
-        )
-        assert (
-            await client.comment_check(comment_content="test", **self.common_kwargs)
-            == akismet.CheckResponse.SPAM
-        )
+        async with AlwaysSpam() as client:
+            assert (
+                await client.comment_check(comment_content="test", **self.common_kwargs)
+                == akismet.CheckResponse.SPAM
+            )
 
     async def test_comment_check_spam_discard(self):
         """
         ``comment_check()`` returns the DISCARD value when Akismet declares the content
         to be spam and sends the "discard"" header value.
 
         """
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(
-                response_text="true", headers={"X-akismet-pro-tip": "discard"}
-            ),
-        )
-        assert (
-            await client.comment_check(comment_content="test", **self.common_kwargs)
-            == akismet.CheckResponse.DISCARD
-        )
+        async with AlwaysBlatantSpam() as client:
+            assert (
+                await client.comment_check(comment_content="test", **self.common_kwargs)
+                == akismet.CheckResponse.DISCARD
+            )
 
     async def test_comment_check_ham(self):
         """
         ``comment_check()`` returns the HAM value when Akismet declares the content
         to be ham.
 
         """
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(response_text="false"),
-        )
-        assert (
-            await client.comment_check(comment_content="test", **self.common_kwargs)
-            == akismet.CheckResponse.HAM
-        )
+        async with NeverSpam() as client:
+            assert (
+                await client.comment_check(comment_content="test", **self.common_kwargs)
+                == akismet.CheckResponse.HAM
+            )
 
     async def test_submit_ham(self):
         """
         ``submit_ham()`` returns True when Akismet accepts the submission.
 
         """
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(
-                response_text=_common._SUBMISSION_RESPONSE
-            ),
-        )
-        assert await client.submit_ham(**self.common_kwargs)
+        async with ValidConfig() as client:
+            assert await client.submit_ham(**self.common_kwargs)
 
     async def test_submit_spam(self):
         """
         ``submit_spam()`` returns True when Akismet accepts the submission.
 
         """
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(
-                response_text=_common._SUBMISSION_RESPONSE
-            ),
-        )
-        assert await client.submit_spam(**self.common_kwargs)
+        async with ValidConfig() as client:
+            assert await client.submit_spam(**self.common_kwargs)
 
     async def test_key_sites_json(self):
         """
-        ``key_sites()`` returns key usage information in JSON format by async default.
+        ``key_sites()`` returns key usage information in JSON format by default.
 
         """
-        # Sample response data taken from Akismet's dev docs.
-        response_json = {
-            "2022-09": [
-                {
-                    "site": "site6735.example.com",
-                    "api_calls": "2072",
-                    "spam": "2069",
-                    "ham": "3",
-                    "missed_spam": "0",
-                    "false_positives": "4",
-                    "is_revoked": False,
-                },
-                {
-                    "site": "site4748.example.com",
-                    "api_calls": "1633",
-                    "spam": "3",
-                    "ham": "1630",
-                    "missed_spam": "0",
-                    "false_positives": "0",
-                    "is_revoked": True,
-                },
-            ],
-            "limit": 10,
-            "offset": 0,
-            "total": 2,
-        }
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(response_json=response_json),
-        )
-        assert await client.key_sites() == response_json
+        async with ValidConfig() as client:
+            response_json = await client.key_sites()
+        for key in ["2022-09", "limit", "offset", "total"]:
+            assert key in response_json
+        sites = response_json["2022-09"]
+        for site in sites:
+            for key in [
+                "site",
+                "api_calls",
+                "spam",
+                "ham",
+                "missed_spam",
+                "false_positives",
+                "is_revoked",
+            ]:
+                assert key in site
 
     async def test_key_sites_csv(self):
         """
         ``key_sites()`` returns key usage information in CSV format when requested.
 
         """
-        # Sample response data taken from Akismet's dev docs.
-        response_csv = textwrap.dedent(
-            """
-        Active sites for 123YourAPIKey during 2022-09 (limit:10, offset: 0, total: 4)
-        Site,Total API Calls,Spam,Ham,Missed Spam,False Positives,Is Revoked
-        site6735.example.com,14446,33,13,0,9,false
-        site3026.example.com,8677,101,6,0,0,false
-        site3737.example.com,4230,65,5,2,0,true
-        site5653.example.com,2921,30,1,2,6,false
-        """
-        )
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(response_text=response_csv),
-        )
-        assert await client.key_sites(result_format="csv") == response_csv
+        async with ValidConfig() as client:
+            first, *rest = (await client.key_sites(result_format="csv")).splitlines()
+        assert first.startswith("Active sites for")
+        reader = csv.DictReader(rest)
+        row = next(reader)
+        assert set(row.keys()) == {
+            "Site",
+            "Total API Calls",
+            "Spam",
+            "Ham",
+            "Missed Spam",
+            "False Positives",
+            "Is Revoked",
+        }
 
     async def test_usage_limit(self):
         """
         ``usage_limit()`` returns the API usage statistics in JSON format.
 
         """
-        # Sample response data taken from Akismet's dev docs.
-        response_json = {
-            "limit": 350000,
-            "usage": 7463,
-            "percentage": "2.13",
-            "throttled": False,
+        async with ValidConfig() as client:
+            response_json = await client.usage_limit()
+        assert set(response_json.keys()) == {
+            "limit",
+            "usage",
+            "percentage",
+            "throttled",
         }
-        client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(response_json=response_json),
-        )
-        assert await client.usage_limit() == response_json
 
 
-class AsyncAkismetErrorTests(AsyncAkismetTests):
+class AsyncAkismetErrorTests(base.AsyncAkismetTests):
     """
     Test the error behavior of the asynchronous Akismet API client.
 
     """
 
     async def test_error_status(self):
         """
         RequestError is raised when a POST request to Akismet responds with an HTTP
         status code indicating an error.
 
         """
         codes = [code for code in HTTPStatus if 400 <= code <= 599]
         for code in codes:
             client = akismet.AsyncClient(
-                config=self.config,
-                http_client=self.custom_response_async_client(status_code=code),
+                http_client=make_fixed_response_async_client(status_code=code),
             )
-        with self.subTest(method="verify_key"):
-            with self.assertRaises(akismet.RequestError):
-                await client.verify_key(self.config.key, self.config.url)
-        for method in ("comment_check", "submit_ham", "submit_spam"):
-            with self.subTest(method=method):
-                with self.assertRaises(akismet.RequestError):
-                    await getattr(client, method)(**self.common_kwargs)
-        for method in ("key_sites", "usage_limit"):
-            with self.subTest(method=method):
+            with self.subTest(method="verify_key"):
                 with self.assertRaises(akismet.RequestError):
-                    await getattr(client, method)()
+                    await client.verify_key()
+            for method in ("comment_check", "submit_ham", "submit_spam"):
+                with self.subTest(method=method):
+                    with self.assertRaises(akismet.RequestError):
+                        await getattr(client, method)(**self.common_kwargs)
+            for method in ("key_sites", "usage_limit"):
+                with self.subTest(method=method):
+                    with self.assertRaises(akismet.RequestError):
+                        await getattr(client, method)()
 
     async def test_error_timeout(self):
         """
         RequestError is raised when the request to Akismet times out.
 
         """
 
         client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.exception_async_client(
+            http_client=make_exception_async_client(
                 httpx.TimeoutException, "Timed out."
             ),
         )
         with self.subTest(method="verify_key"):
             with self.assertRaises(akismet.RequestError):
-                await client.verify_key(self.config.key, self.config.url)
+                await client.verify_key()
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
                     await getattr(client, method)(**self.common_kwargs)
         for method in ("key_sites", "usage_limit"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
@@ -401,20 +504,19 @@
 
     async def test_error_other_httpx(self):
         """
         RequestError is raised when a generic ``httpx`` request error occurs.
 
         """
         client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.exception_async_client(httpx.RequestError),
+            http_client=make_exception_async_client(httpx.RequestError),
         )
         with self.subTest(method="verify_key"):
             with self.assertRaises(akismet.RequestError):
-                await client.verify_key(self.config.key, self.config.url)
+                await client.verify_key()
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
                     await getattr(client, method)(**self.common_kwargs)
         for method in ("key_sites", "usage_limit"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
@@ -423,20 +525,19 @@
     async def test_error_other(self):
         """
         RequestError is raised when any other (non-``httpx``) exception occurs during
         the request.
 
         """
         client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.exception_async_client(TypeError),
+            http_client=make_exception_async_client(TypeError),
         )
         with self.subTest(method="verify_key"):
             with self.assertRaises(akismet.RequestError):
-                await client.verify_key(self.config.key, self.config.url)
+                await client.verify_key()
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
                     await getattr(client, method)(**self.common_kwargs)
         for method in ("key_sites", "usage_limit"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
@@ -445,63 +546,51 @@
     async def test_unknown_argument(self):
         """
         UnknownArgumentError is raised when an argument outside the supported set is
         passed to one of the POST request methods.
 
         """
         client = akismet.AsyncClient(
-            config=self.config, http_client=self.custom_response_async_client()
+            http_client=_test_clients._make_test_async_http_client()
         )
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.UnknownArgumentError):
                     await getattr(client, method)(bad_argument=1, **self.common_kwargs)
 
     async def test_protocol_error_comment_check(self):
         """
         ProtocolError is raised when ``comment_check()`` receives an unexpected
         response.
 
         """
         client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(response_text="bad"),
+            http_client=make_fixed_response_async_client(response_text="bad"),
         )
         with self.assertRaises(akismet.ProtocolError):
             await client.comment_check(**self.common_kwargs)
 
     async def test_protocol_error_submit_ham_spam(self):
         """
         ProtocolError is raised when ``submit_ham()`` or ``submit_spam()`` receive an
         unexpected response.
 
         """
         client = akismet.AsyncClient(
-            config=self.config,
-            http_client=self.custom_response_async_client(response_text="bad"),
+            http_client=make_fixed_response_async_client(response_text="bad"),
         )
         for method in ("submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.ProtocolError):
                     await getattr(client, method)(**self.common_kwargs)
 
     async def test_protocol_error_verify_key(self):
         """
         ProtocolError is raised when ``verify_key()`` receives an unexpected response.
 
         """
 
-        def _handler(  # pylint: disable=unused-argument
-            request: httpx.Request,
-        ) -> httpx.Response:
-            """
-            Mock transport handler which returns a controlled response.
-
-            """
-            return httpx.Response(status_code=HTTPStatus.OK, content="bad")
-
         client = akismet.AsyncClient(
-            config=self.config,
-            http_client=httpx.AsyncClient(transport=httpx.MockTransport(_handler)),
+            http_client=make_fixed_response_async_client(response_text="bad"),
         )
         with self.assertRaises(akismet.ProtocolError):
-            await client.verify_key(self.config.key, self.config.url)
+            await client.verify_key()
```

### Comparing `akismet-1.3/tests/test_legacy_client.py` & `akismet-24.5.0/tests/test_legacy_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 Tests for the deprectaed legacy Akismet API client.
 
 """
 
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
-from http import HTTPStatus
-
-import httpx
 
 import akismet
-from akismet import _common
+from akismet import _common, _test_clients
 
 from . import base
+from .test_sync_client import make_fixed_response_sync_client
 
 
 class LegacyAkismetConfigurationTests(base.AkismetTests):
     """
     Tests configuration of the legacy Akismet API class.
 
     """
@@ -31,89 +29,97 @@
         """
         Configuring via explicit arguments succeeds.
 
         """
         api = akismet.Akismet(
             key=self.api_key,
             blog_url=self.site_url,
-            http_client=self.custom_response_sync_client(),
+            http_client=_test_clients._make_test_sync_http_client(),
         )
         self.assertEqual(self.api_key, api.api_key)
         self.assertEqual(self.site_url, api.blog_url)
 
     def test_bad_config_args(self):
         """
         Configuring with bad arguments fails.
 
         """
         with self.assertRaises(akismet.APIKeyError):
             akismet.Akismet(
                 key="invalid",
                 blog_url="http://invalid",
-                http_client=self.custom_response_sync_client(config_valid=False),
+                http_client=_test_clients._make_test_sync_http_client(
+                    verify_key_response=False
+                ),
             )
 
     def test_config_from_env(self):
         """
         Configuring via environment variables succeeds.
 
         """
         api = akismet.Akismet(
             key=None,
             blog_url=None,
-            http_client=self.custom_response_sync_client(),
+            http_client=_test_clients._make_test_sync_http_client(),
         )
         self.assertEqual(self.api_key, api.api_key)
         self.assertEqual(self.site_url, api.blog_url)
 
-        api = akismet.Akismet(http_client=self.custom_response_sync_client())
+        api = akismet.Akismet(http_client=_test_clients._make_test_sync_http_client())
         self.assertEqual(self.api_key, api.api_key)
         self.assertEqual(self.site_url, api.blog_url)
 
     def test_bad_config_env(self):
         """
         Configuring with bad environment variables fails.
 
         """
         try:
             os.environ[_common._KEY_ENV_VAR] = "invalid"
             os.environ[_common._URL_ENV_VAR] = "http://invalid"
             with self.assertRaises(akismet.APIKeyError):
                 akismet.Akismet(
-                    http_client=self.custom_response_sync_client(config_valid=False)
+                    http_client=_test_clients._make_test_sync_http_client(
+                        verify_key_response=False
+                    )
                 )
         finally:
             os.environ[_common._KEY_ENV_VAR] = self.api_key
             os.environ[_common._URL_ENV_VAR] = self.site_url
 
     def test_bad_config_missing_key(self):
         """
         Configuring with missing key fails.
 
         """
         try:
             del os.environ[_common._KEY_ENV_VAR]
             with self.assertRaises(akismet.ConfigurationError):
                 akismet.Akismet(
-                    http_client=self.custom_response_sync_client(config_valid=False)
+                    http_client=_test_clients._make_test_sync_http_client(
+                        verify_key_response=False
+                    )
                 )
         finally:
             os.environ[_common._KEY_ENV_VAR] = self.api_key
             os.environ[_common._URL_ENV_VAR] = self.site_url
 
     def test_bad_config_missing_url(self):
         """
         Configuring with missing URL fails.
 
         """
         try:
             del os.environ[_common._URL_ENV_VAR]
             with self.assertRaises(akismet.ConfigurationError):
                 akismet.Akismet(
-                    http_client=self.custom_response_sync_client(config_valid=False)
+                    http_client=_test_clients._make_test_sync_http_client(
+                        verify_key_response=False
+                    )
                 )
         finally:
             os.environ[_common._URL_ENV_VAR] = self.site_url
 
     def test_bad_url(self):
         """
         Configuring with a bad URL fails.
@@ -127,42 +133,48 @@
             "https//example.com",
         )
         for url in bad_urls:
             with self.assertRaises(akismet.ConfigurationError):
                 akismet.Akismet(
                     key=self.api_key,
                     blog_url=url,
-                    http_client=self.custom_response_sync_client(config_valid=False),
+                    http_client=_test_clients._make_test_sync_http_client(
+                        verify_key_response=False
+                    ),
                 )
 
     def test_missing_config(self):
         """
         Instantiating without any configuration fails.
 
         """
         with self.assertRaises(akismet.ConfigurationError):
             akismet.Akismet(
                 key=None,
                 blog_url=None,
-                http_client=self.custom_response_sync_client(config_valid=False),
+                http_client=_test_clients._make_test_sync_http_client(
+                    verify_key_response=False
+                ),
             )
         with self.assertRaises(akismet.ConfigurationError):
             akismet.Akismet(
-                http_client=self.custom_response_sync_client(config_valid=False)
+                http_client=_test_clients._make_test_sync_http_client(
+                    verify_key_response=False
+                )
             )
 
     def test_user_agent(self):
         """
         The Akismet class creates the correct user-agent string.
 
         """
         api = akismet.Akismet(
             key=self.api_key,
             blog_url=self.site_url,
-            http_client=self.custom_response_sync_client(),
+            http_client=_test_clients._make_test_sync_http_client(),
         )
         self.assertEqual(api.user_agent_header["User-Agent"], _common.USER_AGENT)
 
 
 class LegacyAkismetAPITests(base.AkismetTests):
     """
     Tests implementation of the legacy Akismet API.
@@ -179,142 +191,127 @@
         The verify_key operation succeeds with a valid key and URL.
 
         """
         self.assertTrue(
             akismet.Akismet.verify_key(
                 self.api_key,
                 self.site_url,
-                http_client=self.custom_response_sync_client(),
+                http_client=_test_clients._make_test_sync_http_client(),
             )
         )
 
     def test_verify_key_invalid(self):
         """
         The verify_key operation fails with an invalid key and URL.
 
         """
         self.assertFalse(
             akismet.Akismet.verify_key(
                 "invalid",
                 "http://invalid",
-                http_client=self.custom_response_sync_client(config_valid=False),
+                http_client=_test_clients._make_test_sync_http_client(
+                    verify_key_response=False
+                ),
             )
         )
 
     def test_comment_check_spam(self):
         """
         The comment_check method correctly identifies spam.
 
         """
         check_kwargs = {
             # Akismet guarantees this will be classified spam.
             "comment_author": "viagra-test-123",
             **self.base_kwargs,
         }
-        api = akismet.Akismet(
-            http_client=self.custom_response_sync_client(response_text="true"),
-        )
+        api = akismet.Akismet(http_client=_test_clients._make_test_sync_http_client())
         self.assertTrue(api.comment_check(**check_kwargs))
 
     def test_comment_check_not_spam(self):
         """
         The comment_check method correctly identifies non-spam.
 
         """
         check_kwargs = {
             # Akismet guarantees this will not be classified spam.
             "user_role": "administrator",
             **self.base_kwargs,
         }
         api = akismet.Akismet(
-            http_client=self.custom_response_sync_client(response_text="false"),
+            http_client=_test_clients._make_test_sync_http_client(
+                comment_check_response=_common.CheckResponse.HAM
+            )
         )
         self.assertFalse(api.comment_check(**check_kwargs))
 
     def test_submit_spam(self):
         """
         The submit_spam method succeeds.
 
         """
         spam_kwargs = {
             "comment_type": "comment",
             "comment_author": "viagra-test-123",
             "comment_content": "viagra-test-123",
             **self.base_kwargs,
         }
-        api = akismet.Akismet(
-            http_client=self.custom_response_sync_client(
-                response_text=_common._SUBMISSION_RESPONSE
-            ),
-        )
+        api = akismet.Akismet(http_client=_test_clients._make_test_sync_http_client())
         self.assertTrue(api.submit_spam(**spam_kwargs))
 
     def test_submit_ham(self):
         """
         The submit_ham method succeeds.
 
         """
         ham_kwargs = {
             "comment_type": "comment",
             "comment_author": "Legitimate Author",
             "comment_content": "This is a legitimate comment.",
             "user_role": "administrator",
             **self.base_kwargs,
         }
-        api = akismet.Akismet(
-            http_client=self.custom_response_sync_client(
-                response_text=_common._SUBMISSION_RESPONSE
-            ),
-        )
+        api = akismet.Akismet(http_client=_test_clients._make_test_sync_http_client())
         self.assertTrue(api.submit_ham(**ham_kwargs))
 
     def test_unexpected_verify_key_response(self):
         """
         Unexpected verify_key API responses are correctly handled.
 
         """
 
-        def _handler(  # pylint: disable=unused-argument
-            request: httpx.Request,
-        ) -> httpx.Response:
-            """
-            Mock transport handler which returns a controlled response.
-
-            """
-            return httpx.Response(status_code=HTTPStatus.OK, content="bad")
-
         api = akismet.Akismet(
-            http_client=self.custom_response_sync_client(),
+            http_client=_test_clients._make_test_sync_http_client(),
         )
         with self.assertRaises(akismet.ProtocolError):
             api.verify_key(
                 self.api_key,
                 self.site_url,
-                http_client=httpx.Client(transport=httpx.MockTransport(_handler)),
+                http_client=make_fixed_response_sync_client(response_text="bad"),
             )
 
     def test_unexpected_comment_check_response(self):
         """
         Unexpected comment_check API responses are correctly handled.
 
         """
         api = akismet.Akismet(
-            http_client=self.custom_response_sync_client(response_text="bad"),
+            http_client=make_fixed_response_sync_client(response_text="valid"),
         )
         with self.assertRaises(akismet.ProtocolError):
             check_kwargs = {"comment_author": "viagra-test-123", **self.base_kwargs}
             api.comment_check(**check_kwargs)
 
     def test_unexpected_submit_spam_response(self):
         """
         Unexpected submit_spam API responses are correctly handled.
 
         """
         api = akismet.Akismet(
-            http_client=self.custom_response_sync_client(response_text="bad"),
+            http_client=make_fixed_response_sync_client(response_text="valid"),
         )
         with self.assertRaises(akismet.ProtocolError):
             spam_kwargs = {
                 "comment_type": "comment",
                 "comment_author": "viagra-test-123",
                 "comment_content": "viagra-test-123",
                 **self.base_kwargs,
@@ -323,15 +320,15 @@
 
     def test_unexpected_submit_ham_response(self):
         """
         Unexpected submit_ham API responses are correctly handled.
 
         """
         api = akismet.Akismet(
-            http_client=self.custom_response_sync_client(response_text="bad"),
+            http_client=make_fixed_response_sync_client(response_text="valid"),
         )
         with self.assertRaises(akismet.ProtocolError):
             ham_kwargs = {
                 "comment_type": "comment",
                 "comment_author": "Legitimate Author",
                 "comment_content": "This is a legitimate comment.",
                 "user_role": "administrator",
@@ -342,11 +339,11 @@
     def test_unknown_kwargs(self):
         """
         Unknown Akismet arguments are correctly rejected.
 
         """
         bad_kwargs = {"bad_arg": "bad_val", **self.base_kwargs}
         api = akismet.Akismet(
-            http_client=self.custom_response_sync_client(),
+            http_client=_test_clients._make_test_sync_http_client(),
         )
         with self.assertRaises(akismet.UnknownArgumentError):
             api.comment_check(**bad_kwargs)
```

### Comparing `akismet-1.3/tests/test_sync_client.py` & `akismet-24.5.0/tests/test_sync_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,195 @@
 """
 Tests for the synchronous Akismet API client.
 
 """
 
 # SPDX-License-Identifier: BSD-3-Clause
 
+import csv
 import os
-import textwrap
+import typing
 from http import HTTPStatus
+from unittest import mock
 
 import httpx
 
 import akismet
-from akismet import _common
+from akismet import _common, _test_clients
 
-from .base import AkismetTests
+from . import base
 
 
-class SyncAkismetConstructorTests(AkismetTests):
+def make_fixed_response_sync_client(
+    response_text: str = "true",
+    status_code: HTTPStatus = HTTPStatus.OK,
+    response_json: typing.Optional[dict] = None,
+) -> httpx.Client:
     """
-    Test the ``client()`` constructor of the synchronous Akismet API client.
+    Return a synchronous HTTP client that produces a fixed repsonse, for use in
+    testing.
 
     """
+    return httpx.Client(
+        transport=base.make_fixed_response_transport(
+            response_text, status_code, response_json
+        )
+    )
+
+
+def make_exception_sync_client(
+    exception_class: Exception, message: str = "Error!"
+) -> httpx.Client:
+    """
+    Return a synchronous HTTP client that raises the given exception/message.
+
+    """
+    return mock.Mock(
+        spec_set=httpx.Client,
+        get=mock.Mock(side_effect=exception_class(message)),
+        post=mock.Mock(side_effect=exception_class(message)),
+    )
+
+
+class ValidConfig(akismet.TestSyncClient):
+    """
+    Test client with valid config.
+
+    """
+
+    verify_key_response = True
+
+
+class InvalidConfig(akismet.TestSyncClient):
+    """
+    Test client with invalid config.
+
+    """
+
+    verify_key_response = False
+
+
+class AlwaysBlatantSpam(akismet.TestSyncClient):
+    """
+    Test client which marks all content as "blatant" spam.
+
+    """
+
+    comment_check_response = akismet.CheckResponse.DISCARD
+
+
+class AlwaysSpam(akismet.TestSyncClient):
+    """
+    Test client which marks all content as spam.
+
+    """
+
+    comment_check_response = akismet.CheckResponse.SPAM
+
+
+class NeverSpam(akismet.TestSyncClient):
+    """
+    Test client which marks all content as not spam.
+
+    """
+
+    comment_check_response = akismet.CheckResponse.HAM
+
+
+class SyncAkismetConstructorTests(base.AkismetTests):
+    """
+    Test the constructors of the synchronous Akismet API client.
+
+    """
+
+    def test_construct_config_explicit(self):
+        """
+        Passing explicit config to the default constructor uses that config.
+
+        """
+        config = akismet.Config(key="other-invalid-test-key", url=self.config.url)
+        with ValidConfig(config=config) as client:
+            assert client._config == config
+
+    def test_construct_config_alternate_constructor_explicit(self):
+        """
+        Passing explicit config to the alternate constructor uses that config.
+
+        """
+        config = akismet.Config(key="other-invalid-test-key", url=self.config.url)
+        client = ValidConfig.validated_client(config=config)
+        assert client._config == config
+
+    def test_construct_config_from_env(self):
+        """
+        Instantiating via the default constructor, without passing explicit config,
+        reads the config from the environment.
+
+        """
+        config = akismet.Config(key=self.api_key, url=self.site_url)
+        with ValidConfig() as client:
+            assert client._config == config
+
+    def test_construct_alternate_constructor_config_from_env(self):
+        """
+        Instantiating via the alternate constructor, without passing explicit
+        config, reads the config from the environment.
+
+        """
+        config = akismet.Config(key=self.api_key, url=self.site_url)
+        client = ValidConfig.validated_client()
+        assert client._config == config
 
     def test_construct_config_valid(self):
         """
         With a valid configuration, constructing a client succeeds.
 
         """
-        akismet.SyncClient.validated_client(
-            http_client=self.custom_response_sync_client()
-        )
+        ValidConfig.validated_client()
 
     def test_construct_config_invalid_key(self):
         """
         With an invalid API key, constructing a client raises an APIKeyError.
 
         """
         with self.assertRaises(akismet.APIKeyError):
-            akismet.SyncClient.validated_client(
-                http_client=self.custom_response_sync_client(config_valid=False)
-            )
+            InvalidConfig.validated_client()
+
+    def test_construct_config_valid_context_manager(self):
+        """
+        With a valid configuration, constructing a client as a context manager succeeds.
+
+        """
+        with ValidConfig():
+            pass
+
+    def test_construct_config_invalid_key_context_manager(self):
+        """
+        With an invalid API key, constructing a client as a context manager raises
+        an APIKeyError.
+
+        """
+        with self.assertRaises(akismet.APIKeyError):
+            with InvalidConfig():
+                pass
+
+    def test_construct_config_valid_explicit(self):
+        """
+        With an explicit valid configuration, constructing a client succeeds.
+
+        """
+        ValidConfig.validated_client(config=self.config)
+
+    def test_construct_config_invalid_key_explicit(self):
+        """
+        With an explicit invalid API key, constructing a client raises an APIKeyError.
+
+        """
+        with self.assertRaises(akismet.APIKeyError):
+            InvalidConfig.validated_client(config=self.config)
 
     def test_construct_config_bad_url(self):
         """
         With an invalid URL, constructing a client raises a ConfigurationError.
 
         """
         try:
@@ -60,33 +205,29 @@
         ConfigurationError.
 
         """
         try:
             if _common._KEY_ENV_VAR in os.environ:
                 del os.environ[_common._KEY_ENV_VAR]
             with self.assertRaises(akismet.ConfigurationError):
-                akismet.SyncClient.validated_client(
-                    http_client=self.custom_response_sync_client()
-                )
+                ValidConfig.validated_client()
         finally:
             os.environ[_common._KEY_ENV_VAR] = self.api_key
 
     def test_construct_config_missing_url(self):
         """
         Without a registered site URL present, constructing a client raises a
         ConfigurationError.
 
         """
         try:
             if _common._URL_ENV_VAR in os.environ:
                 del os.environ[_common._URL_ENV_VAR]
             with self.assertRaises(akismet.ConfigurationError):
-                akismet.SyncClient.validated_client(
-                    http_client=self.custom_response_sync_client()
-                )
+                ValidConfig.validated_client()
         finally:
             os.environ[_common._URL_ENV_VAR] = self.site_url
 
     def test_construct_config_missing_all(self):
         """
         Without any config present, constructing a client raises a
         ConfigurationError.
@@ -94,49 +235,44 @@
         """
         try:
             if _common._KEY_ENV_VAR in os.environ:
                 del os.environ[_common._KEY_ENV_VAR]
             if _common._URL_ENV_VAR in os.environ:
                 del os.environ[_common._URL_ENV_VAR]
             with self.assertRaises(akismet.ConfigurationError):
-                akismet.SyncClient.validated_client(
-                    http_client=self.custom_response_sync_client()
-                )
+                ValidConfig.validated_client()
         finally:
             os.environ[_common._KEY_ENV_VAR] = self.api_key
             os.environ[_common._URL_ENV_VAR] = self.site_url
 
     def test_construct_default_client(self):
         """
         Constructing a client without an explicit HTTP client uses the default HTTP
         client.
 
         """
-        client = akismet.SyncClient(config=self.config)
+        client = akismet.SyncClient()
         http_client = client._http_client
         assert "user-agent" in http_client.headers
         assert http_client.headers["user-agent"] == _common.USER_AGENT
 
 
-class SyncAkismetAPITests(AkismetTests):
+class SyncAkismetAPITests(base.AkismetTests):
     """
     Test the API behavior of the synchronous Akismet API client.
 
     """
 
     def test_unsupported_request_method(self):
         """
         Attempting to make a request with an unsupported method raises
         ``AkismetError``.
 
         """
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(),
-        )
+        client = ValidConfig()
         # The tested set of methods here are all the methods that are in Python 3.11's
         # http.HTTPMethod enum but not supported for Akismet requests.
         for bad_method in (
             "CONNECT",
             "DELETE",
             "HEAD",
             "OPTIONS",
@@ -154,40 +290,51 @@
                     )
 
     def test_verify_key_valid(self):
         """
         ``verify_key()`` returns True when the config is valid.
 
         """
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(),
-        )
-        assert client.verify_key(key=self.api_key, url=self.site_url)
+        with ValidConfig() as client:
+            assert client.verify_key()
 
     def test_verify_key_invalid(self):
         """
         ``verify_key()`` returns False when the config is invalid.
 
         """
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(config_valid=False),
-        )
+        client = InvalidConfig()
+        assert not client.verify_key()
+
+    def test_verify_key_valid_explicit(self):
+        """
+        ``verify_key()`` returns True when the config is valid and explicitly passed
+        in.
+
+        """
+        with ValidConfig() as client:
+            assert client.verify_key(key=self.api_key, url=self.site_url)
+
+    def test_verify_key_invalid_explicit(self):
+        """
+        ``verify_key()`` returns False when the config is invalid and explicitly
+        passed in.
+
+        """
+        client = InvalidConfig()
         assert not client.verify_key(key=self.api_key, url=self.site_url)
 
     def test_request_with_invalid_key(self):
         """
         The request methods other than ``verify_key()`` raise
         ``akismet.APIKeyError`` if called with an invalid API key/URL.
 
         """
         client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(response_text="invalid"),
+            http_client=make_fixed_response_sync_client(response_text="invalid"),
         )
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.APIKeyError):
                     getattr(client, method)(**self.common_kwargs)
         for method in ("key_sites", "usage_limit"):
             with self.subTest(method=method):
@@ -196,204 +343,160 @@
 
     def test_comment_check_spam(self):
         """
         ``comment_check()`` returns the SPAM value when Akismet declares the content
         to be spam.
 
         """
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(response_text="true"),
-        )
-        assert (
-            client.comment_check(comment_content="test", **self.common_kwargs)
-            == akismet.CheckResponse.SPAM
-        )
+        with AlwaysSpam() as client:
+            assert (
+                client.comment_check(comment_content="test", **self.common_kwargs)
+                == akismet.CheckResponse.SPAM
+            )
 
     def test_comment_check_spam_discard(self):
         """
         ``comment_check()`` returns the DISCARD value when Akismet declares the content
         to be spam and sends the "discard"" header value.
 
         """
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(
-                response_text="true", headers={"X-akismet-pro-tip": "discard"}
-            ),
-        )
-        assert (
-            client.comment_check(comment_content="test", **self.common_kwargs)
-            == akismet.CheckResponse.DISCARD
-        )
+        with AlwaysBlatantSpam() as client:
+            assert (
+                client.comment_check(comment_content="test", **self.common_kwargs)
+                == akismet.CheckResponse.DISCARD
+            )
 
     def test_comment_check_ham(self):
         """
         ``comment_check()`` returns the HAM value when Akismet declares the content
         to be ham.
 
         """
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(response_text="false"),
-        )
-        assert (
-            client.comment_check(comment_content="test", **self.common_kwargs)
-            == akismet.CheckResponse.HAM
-        )
+        with NeverSpam() as client:
+            assert (
+                client.comment_check(comment_content="test", **self.common_kwargs)
+                == akismet.CheckResponse.HAM
+            )
 
     def test_submit_ham(self):
         """
         ``submit_ham()`` returns True when Akismet accepts the submission.
 
         """
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(
-                response_text=_common._SUBMISSION_RESPONSE
-            ),
-        )
-        assert client.submit_ham(**self.common_kwargs)
+        with ValidConfig() as client:
+            assert client.submit_ham(**self.common_kwargs)
 
     def test_submit_spam(self):
         """
         ``submit_spam()`` returns True when Akismet accepts the submission.
 
         """
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(
-                response_text=_common._SUBMISSION_RESPONSE
-            ),
-        )
-        assert client.submit_spam(**self.common_kwargs)
+        with ValidConfig() as client:
+            assert client.submit_spam(**self.common_kwargs)
 
     def test_key_sites_json(self):
         """
         ``key_sites()`` returns key usage information in JSON format by default.
 
         """
-        # Sample response data taken from Akismet's dev docs.
-        response_json = {
-            "2022-09": [
-                {
-                    "site": "site6735.example.com",
-                    "api_calls": "2072",
-                    "spam": "2069",
-                    "ham": "3",
-                    "missed_spam": "0",
-                    "false_positives": "4",
-                    "is_revoked": False,
-                },
-                {
-                    "site": "site4748.example.com",
-                    "api_calls": "1633",
-                    "spam": "3",
-                    "ham": "1630",
-                    "missed_spam": "0",
-                    "false_positives": "0",
-                    "is_revoked": True,
-                },
-            ],
-            "limit": 10,
-            "offset": 0,
-            "total": 2,
-        }
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(response_json=response_json),
-        )
-        assert client.key_sites() == response_json
+        with ValidConfig() as client:
+            response_json = client.key_sites()
+        for key in ["2022-09", "limit", "offset", "total"]:
+            assert key in response_json
+        sites = response_json["2022-09"]
+        for site in sites:
+            for key in [
+                "site",
+                "api_calls",
+                "spam",
+                "ham",
+                "missed_spam",
+                "false_positives",
+                "is_revoked",
+            ]:
+                assert key in site
 
     def test_key_sites_csv(self):
         """
         ``key_sites()`` returns key usage information in CSV format when requested.
 
         """
-        # Sample response data taken from Akismet's dev docs.
-        response_csv = textwrap.dedent(
-            """
-        Active sites for 123YourAPIKey during 2022-09 (limit:10, offset: 0, total: 4)
-        Site,Total API Calls,Spam,Ham,Missed Spam,False Positives,Is Revoked
-        site6735.example.com,14446,33,13,0,9,false
-        site3026.example.com,8677,101,6,0,0,false
-        site3737.example.com,4230,65,5,2,0,true
-        site5653.example.com,2921,30,1,2,6,false
-        """
-        )
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(response_text=response_csv),
-        )
-        assert client.key_sites(result_format="csv") == response_csv
+        with ValidConfig() as client:
+            first, *rest = (client.key_sites(result_format="csv")).splitlines()
+        assert first.startswith("Active sites for")
+        reader = csv.DictReader(rest)
+        row = next(reader)
+        assert set(row.keys()) == {
+            "Site",
+            "Total API Calls",
+            "Spam",
+            "Ham",
+            "Missed Spam",
+            "False Positives",
+            "Is Revoked",
+        }
 
     def test_usage_limit(self):
         """
         ``usage_limit()`` returns the API usage statistics in JSON format.
 
         """
-        # Sample response data taken from Akismet's dev docs.
-        response_json = {
-            "limit": 350000,
-            "usage": 7463,
-            "percentage": "2.13",
-            "throttled": False,
+        with ValidConfig() as client:
+            response_json = client.usage_limit()
+        assert set(response_json.keys()) == {
+            "limit",
+            "usage",
+            "percentage",
+            "throttled",
         }
-        client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(response_json=response_json),
-        )
-        assert client.usage_limit() == response_json
 
 
-class SyncAkismetErrorTests(AkismetTests):
+class SyncAkismetErrorTests(base.AkismetTests):
     """
     Test the error behavior of the synchronous Akismet API client.
 
     """
 
     def test_error_status(self):
         """
         RequestError is raised when a POST request to Akismet responds with an HTTP
         status code indicating an error.
 
         """
         codes = [code for code in HTTPStatus if 400 <= code <= 599]
         for code in codes:
             client = akismet.SyncClient(
-                config=self.config,
-                http_client=self.custom_response_sync_client(status_code=code),
+                http_client=make_fixed_response_sync_client(status_code=code),
             )
-        with self.subTest(method="verify_key"):
-            with self.assertRaises(akismet.RequestError):
-                client.verify_key(self.config.key, self.config.url)
-        for method in ("comment_check", "submit_ham", "submit_spam"):
-            with self.subTest(method=method):
-                with self.assertRaises(akismet.RequestError):
-                    getattr(client, method)(**self.common_kwargs)
-        for method in ("key_sites", "usage_limit"):
-            with self.subTest(method=method):
+            with self.subTest(method="verify_key"):
                 with self.assertRaises(akismet.RequestError):
-                    getattr(client, method)()
+                    client.verify_key()
+            for method in ("comment_check", "submit_ham", "submit_spam"):
+                with self.subTest(method=method):
+                    with self.assertRaises(akismet.RequestError):
+                        getattr(client, method)(**self.common_kwargs)
+            for method in ("key_sites", "usage_limit"):
+                with self.subTest(method=method):
+                    with self.assertRaises(akismet.RequestError):
+                        getattr(client, method)()
 
     def test_error_timeout(self):
         """
         RequestError is raised when the request to Akismet times out.
 
         """
 
         client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.exception_sync_client(
+            http_client=make_exception_sync_client(
                 httpx.TimeoutException, "Timed out."
             ),
         )
         with self.subTest(method="verify_key"):
             with self.assertRaises(akismet.RequestError):
-                client.verify_key(self.config.key, self.config.url)
+                client.verify_key()
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
                     getattr(client, method)(**self.common_kwargs)
         for method in ("key_sites", "usage_limit"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
@@ -401,20 +504,19 @@
 
     def test_error_other_httpx(self):
         """
         RequestError is raised when a generic ``httpx`` request error occurs.
 
         """
         client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.exception_sync_client(httpx.RequestError),
+            http_client=make_exception_sync_client(httpx.RequestError),
         )
         with self.subTest(method="verify_key"):
             with self.assertRaises(akismet.RequestError):
-                client.verify_key(self.config.key, self.config.url)
+                client.verify_key()
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
                     getattr(client, method)(**self.common_kwargs)
         for method in ("key_sites", "usage_limit"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
@@ -423,20 +525,19 @@
     def test_error_other(self):
         """
         RequestError is raised when any other (non-``httpx``) exception occurs during
         the request.
 
         """
         client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.exception_sync_client(TypeError),
+            http_client=make_exception_sync_client(TypeError),
         )
         with self.subTest(method="verify_key"):
             with self.assertRaises(akismet.RequestError):
-                client.verify_key(self.config.key, self.config.url)
+                client.verify_key()
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
                     getattr(client, method)(**self.common_kwargs)
         for method in ("key_sites", "usage_limit"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.RequestError):
@@ -445,63 +546,51 @@
     def test_unknown_argument(self):
         """
         UnknownArgumentError is raised when an argument outside the supported set is
         passed to one of the POST request methods.
 
         """
         client = akismet.SyncClient(
-            config=self.config, http_client=self.custom_response_sync_client()
+            http_client=_test_clients._make_test_async_http_client()
         )
         for method in ("comment_check", "submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.UnknownArgumentError):
                     getattr(client, method)(bad_argument=1, **self.common_kwargs)
 
     def test_protocol_error_comment_check(self):
         """
         ProtocolError is raised when ``comment_check()`` receives an unexpected
         response.
 
         """
         client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(response_text="bad"),
+            http_client=make_fixed_response_sync_client(response_text="bad"),
         )
         with self.assertRaises(akismet.ProtocolError):
             client.comment_check(**self.common_kwargs)
 
     def test_protocol_error_submit_ham_spam(self):
         """
         ProtocolError is raised when ``submit_ham()`` or ``submit_spam()`` receive an
         unexpected response.
 
         """
         client = akismet.SyncClient(
-            config=self.config,
-            http_client=self.custom_response_sync_client(response_text="bad"),
+            http_client=make_fixed_response_sync_client(response_text="bad"),
         )
         for method in ("submit_ham", "submit_spam"):
             with self.subTest(method=method):
                 with self.assertRaises(akismet.ProtocolError):
                     getattr(client, method)(**self.common_kwargs)
 
     def test_protocol_error_verify_key(self):
         """
         ProtocolError is raised when ``verify_key()`` receives an unexpected response.
 
         """
 
-        def _handler(  # pylint: disable=unused-argument
-            request: httpx.Request,
-        ) -> httpx.Response:
-            """
-            Mock transport handler which returns a controlled response.
-
-            """
-            return httpx.Response(status_code=HTTPStatus.OK, content="bad")
-
         client = akismet.SyncClient(
-            config=self.config,
-            http_client=httpx.Client(transport=httpx.MockTransport(_handler)),
+            http_client=make_fixed_response_sync_client(response_text="bad"),
         )
         with self.assertRaises(akismet.ProtocolError):
-            client.verify_key(self.config.key, self.config.url)
+            client.verify_key()
```

### Comparing `akismet-1.3/tox.ini` & `akismet-24.5.0/tox.ini`

 * *Files identical despite different names*

