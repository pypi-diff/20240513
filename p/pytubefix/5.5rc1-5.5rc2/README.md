# Comparing `tmp/pytubefix-5.5rc1.tar.gz` & `tmp/pytubefix-5.5rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubefix-5.5rc1.tar", last modified: Sat May 11 22:35:27 2024, max compression
+gzip compressed data, was "pytubefix-5.5rc2.tar", last modified: Mon May 13 17:10:03 2024, max compression
```

## Comparing `pytubefix-5.5rc1.tar` & `pytubefix-5.5rc2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/
--rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/LICENSE
--rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/MANIFEST.in
--rw-r--r--   0 juan      (1000) juan      (1000)     4343 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     3011 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-05-11 22:32:47.000000 pytubefix-5.5rc1/pyproject.toml
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.885305 pytubefix-5.5rc1/pytubefix/
--rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    20063 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6593 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/chapters.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    16972 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      781 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/colors.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.889305 pytubefix-5.5rc1/pytubefix/contrib/
--rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/contrib/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/contrib/channel.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/contrib/playlist.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/contrib/search.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4099 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18343 2024-05-11 22:30:55.000000 pytubefix-5.5rc1/pytubefix/extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     9943 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17742 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/innertube.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4276 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/jsinterp.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/monostate.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5948 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14359 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     8736 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    16049 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/streams.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-05-11 22:34:05.000000 pytubefix-5.5rc1/pytubefix/version.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/pytubefix.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     4343 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/tests/
--rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_main.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_streams.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 17:10:03.241515 pytubefix-5.5rc2/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1101 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/LICENSE
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       18 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/MANIFEST.in
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     4343 2024-05-13 17:10:03.241515 pytubefix-5.5rc2/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3011 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/README.md
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1524 2024-05-13 16:54:22.000000 pytubefix-5.5rc2/pyproject.toml
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 17:10:03.229516 pytubefix-5.5rc2/pytubefix/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      657 2024-05-13 16:53:16.000000 pytubefix-5.5rc2/pytubefix/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    22728 2024-05-13 16:53:16.000000 pytubefix-5.5rc2/pytubefix/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     6593 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/captions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1358 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/chapters.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     5645 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/cipher.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    16972 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      781 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/colors.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 17:10:03.233516 pytubefix-5.5rc2/pytubefix/contrib/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        0 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/contrib/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    19995 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/contrib/channel.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    14600 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/contrib/playlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    11072 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/contrib/search.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     4099 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/exceptions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18343 2024-05-13 16:53:16.000000 pytubefix-5.5rc2/pytubefix/extract.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     9943 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/helpers.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    17742 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/innertube.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     4276 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/itags.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    41663 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/jsinterp.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1339 2024-05-13 16:53:16.000000 pytubefix-5.5rc2/pytubefix/keymoments.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1483 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/metadata.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      478 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/monostate.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     5948 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/parser.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    14359 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/query.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     8736 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/request.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    16049 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/pytubefix/streams.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-05-13 16:54:11.000000 pytubefix-5.5rc2/pytubefix/version.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 17:10:03.241515 pytubefix-5.5rc2/pytubefix.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     4343 2024-05-13 17:10:03.000000 pytubefix-5.5rc2/pytubefix.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1053 2024-05-13 17:10:03.000000 pytubefix-5.5rc2/pytubefix.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-13 17:10:03.000000 pytubefix-5.5rc2/pytubefix.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       49 2024-05-13 17:10:03.000000 pytubefix-5.5rc2/pytubefix.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       10 2024-05-13 17:10:03.000000 pytubefix-5.5rc2/pytubefix.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-13 17:10:03.241515 pytubefix-5.5rc2/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 17:10:03.241515 pytubefix-5.5rc2/tests/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     6579 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_captions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1360 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_cipher.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18009 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3626 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_exceptions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2963 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_extract.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     5060 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_helpers.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      279 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_itags.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1939 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_main.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      501 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_metadata.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1412 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_parser.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     6172 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_query.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1882 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_request.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    13661 2024-05-13 16:52:39.000000 pytubefix-5.5rc2/tests/test_streams.py
```

### Comparing `pytubefix-5.5rc1/LICENSE` & `pytubefix-5.5rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/PKG-INFO` & `pytubefix-5.5rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.5rc1
+Version: 5.5rc2
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.5rc1 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.5rc2 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.5rc1/README.md` & `pytubefix-5.5rc2/README.md`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pyproject.toml` & `pytubefix-5.5rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubefix"
-version = "5.5-rc1"
+version = "5.5-rc2"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python3 library for downloading YouTube Videos."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT license"}
```

### Comparing `pytubefix-5.5rc1/pytubefix/__init__.py` & `pytubefix-5.5rc2/pytubefix/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 __js__ = None
 __js_url__ = None
 
 from pytubefix.version import __version__
 from pytubefix.streams import Stream
 from pytubefix.captions import Caption
 from pytubefix.chapters import Chapter
+from pytubefix.keymoments import KeyMoment
 from pytubefix.query import CaptionQuery, StreamQuery
 from pytubefix.__main__ import YouTube
 from pytubefix.contrib.playlist import Playlist
 from pytubefix.contrib.channel import Channel
 from pytubefix.contrib.search import Search
```

### Comparing `pytubefix-5.5rc1/pytubefix/__main__.py` & `pytubefix-5.5rc2/pytubefix/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -404,14 +404,89 @@
                 chapter_end = int(
                     chapters_data[i + 1]['chapterRenderer']['timeRangeStartMillis'] / 1000
                 )
 
             result.append(pytubefix.Chapter(chapter_data, chapter_end - chapter_start))
 
         return result
+    
+    @property
+    def key_moments(self) -> List[pytubefix.KeyMoment]:
+        """Get a list of :class:`KeyMoment <KeyMoment>`.
+
+        :rtype: List[KeyMoment]
+        """
+        try:
+            mutations = self.initial_data['frameworkUpdates']['entityBatchUpdate']['mutations']
+            found = False
+            for mutation in mutations:
+                if mutation.get('payload', {}).get('macroMarkersListEntity', {}).get('markersList', {}).get('markerType') == "MARKER_TYPE_TIMESTAMPS":
+                    key_moments_data = mutation['payload']['macroMarkersListEntity']['markersList']['markers']
+                    found = True
+                    break
+
+            if not found:
+                return []
+        except (KeyError, IndexError):
+            return []
+
+        result: List[pytubefix.KeyMoment] = []
+
+        for i, key_moment_data in enumerate(key_moments_data):
+            key_moment_start = int(
+                int(key_moment_data['startMillis']) / 1000
+            )
+
+            if i == len(key_moments_data) - 1:
+                key_moment_end = self.length
+            else:
+                key_moment_end = int(
+                    int(key_moments_data[i + 1]['startMillis']) / 1000
+                )
+
+            result.append(pytubefix.KeyMoment(key_moment_data, key_moment_end - key_moment_start))
+
+        return result
+    
+    @property
+    def replayed_heatmap(self) -> List[Dict[str, float]]:
+        """Get a list of : `Dict<str, float>`.
+
+        :rtype: List[Dict[str, float]]
+        """
+        try:
+            mutations = self.initial_data['frameworkUpdates']['entityBatchUpdate']['mutations']
+            found = False
+            for mutation in mutations:
+                if mutation.get('payload', {}).get('macroMarkersListEntity', {}).get('markersList', {}).get('markerType') == "MARKER_TYPE_HEATMAP":
+                    heatmaps_data = mutation['payload']['macroMarkersListEntity']['markersList']['markers']
+                    found = True
+                    break
+
+            if not found:
+                return []
+        except (KeyError, IndexError):
+            return []
+
+        result: List[Dict[str, float]] = []
+
+        for i, heatmap_data in enumerate(heatmaps_data):
+            heatmap_start = int(heatmap_data['startMillis']) / 1000
+            duration = int(heatmap_data['durationMillis']) / 1000
+
+
+            norm_intensity = float(heatmap_data['intensityScoreNormalized'])
+
+            result.append({
+                "start_seconds": heatmap_start,
+                "duration": duration,
+                "norm_intensity": norm_intensity
+            })
+
+        return result
 
     @property
     def streams(self) -> StreamQuery:
         """Interface to query both adaptive (DASH) and progressive streams.
 
         :rtype: :class:`StreamQuery <StreamQuery>`.
         """
```

### Comparing `pytubefix-5.5rc1/pytubefix/captions.py` & `pytubefix-5.5rc2/pytubefix/captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/chapters.py` & `pytubefix-5.5rc2/pytubefix/chapters.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/cipher.py` & `pytubefix-5.5rc2/pytubefix/cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/cli.py` & `pytubefix-5.5rc2/pytubefix/cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/colors.py` & `pytubefix-5.5rc2/pytubefix/colors.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/contrib/channel.py` & `pytubefix-5.5rc2/pytubefix/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/contrib/playlist.py` & `pytubefix-5.5rc2/pytubefix/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/contrib/search.py` & `pytubefix-5.5rc2/pytubefix/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/exceptions.py` & `pytubefix-5.5rc2/pytubefix/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/extract.py` & `pytubefix-5.5rc2/pytubefix/extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/helpers.py` & `pytubefix-5.5rc2/pytubefix/helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/innertube.py` & `pytubefix-5.5rc2/pytubefix/innertube.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/itags.py` & `pytubefix-5.5rc2/pytubefix/itags.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/jsinterp.py` & `pytubefix-5.5rc2/pytubefix/jsinterp.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/metadata.py` & `pytubefix-5.5rc2/pytubefix/metadata.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/parser.py` & `pytubefix-5.5rc2/pytubefix/parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/query.py` & `pytubefix-5.5rc2/pytubefix/query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/request.py` & `pytubefix-5.5rc2/pytubefix/request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix/streams.py` & `pytubefix-5.5rc2/pytubefix/streams.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/pytubefix.egg-info/PKG-INFO` & `pytubefix-5.5rc2/pytubefix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.5rc1
+Version: 5.5rc2
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.5rc1 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.5rc2 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.5rc1/pytubefix.egg-info/SOURCES.txt` & `pytubefix-5.5rc2/pytubefix.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 pytubefix/colors.py
 pytubefix/exceptions.py
 pytubefix/extract.py
 pytubefix/helpers.py
 pytubefix/innertube.py
 pytubefix/itags.py
 pytubefix/jsinterp.py
+pytubefix/keymoments.py
 pytubefix/metadata.py
 pytubefix/monostate.py
 pytubefix/parser.py
 pytubefix/query.py
 pytubefix/request.py
 pytubefix/streams.py
 pytubefix/version.py
```

### Comparing `pytubefix-5.5rc1/tests/test_captions.py` & `pytubefix-5.5rc2/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_cipher.py` & `pytubefix-5.5rc2/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_cli.py` & `pytubefix-5.5rc2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_exceptions.py` & `pytubefix-5.5rc2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_extract.py` & `pytubefix-5.5rc2/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_helpers.py` & `pytubefix-5.5rc2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_main.py` & `pytubefix-5.5rc2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_parser.py` & `pytubefix-5.5rc2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_query.py` & `pytubefix-5.5rc2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_request.py` & `pytubefix-5.5rc2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc1/tests/test_streams.py` & `pytubefix-5.5rc2/tests/test_streams.py`

 * *Files identical despite different names*

