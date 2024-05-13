# Comparing `tmp/bisos.facter-0.7.tar.gz` & `tmp/bisos.facter-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisos.facter-0.7.tar", last modified: Sat May 11 04:46:11 2024, max compression
+gzip compressed data, was "bisos.facter-0.8.tar", last modified: Sun May 12 04:40:28 2024, max compression
```

## Comparing `bisos.facter-0.7.tar` & `bisos.facter-0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-10 16:52:15.000000 bisos.facter-0.7/MANIFEST.in
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1651 2024-05-11 04:46:11.186286 bisos.facter-0.7/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      677 2024-05-11 04:46:10.000000 bisos.facter-0.7/README.rst
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      112 2024-05-10 16:52:15.000000 bisos.facter-0.7/TITLE.txt
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/bin/
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.7/bin/facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.7/bin/roInv-facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.7/bin/roPerf-facter.cs
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/bisos/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.7/bisos/__init__.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/bisos/facter/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.7/bisos/facter/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.7/bisos/facter/facter.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.7/bisos/facter/facter_csu.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:46:11.186286 bisos.facter-0.7/bisos.facter.egg-info/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1651 2024-05-11 04:46:10.000000 bisos.facter-0.7/bisos.facter.egg-info/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      430 2024-05-11 04:46:11.000000 bisos.facter-0.7/bisos.facter.egg-info/SOURCES.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:46:10.000000 bisos.facter-0.7/bisos.facter.egg-info/dependency_links.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:46:10.000000 bisos.facter-0.7/bisos.facter.egg-info/not-zip-safe
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       72 2024-05-11 04:46:11.000000 bisos.facter-0.7/bisos.facter.egg-info/requires.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-11 04:46:11.000000 bisos.facter-0.7/bisos.facter.egg-info/top_level.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-11 04:46:10.000000 bisos.facter-0.7/lh-agpl3-LICENSE.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-11 04:46:11.186286 bisos.facter-0.7/setup.cfg
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1797 2024-05-11 04:44:54.000000 bisos.facter-0.7/setup.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-12 04:31:16.000000 bisos.facter-0.8/MANIFEST.in
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1993 2024-05-12 04:40:28.342722 bisos.facter-0.8/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1350 2024-05-12 04:31:16.000000 bisos.facter-0.8/README.org
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      112 2024-05-10 16:52:15.000000 bisos.facter-0.8/TITLE.txt
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/bin/
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.8/bin/facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.8/bin/roInv-facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.8/bin/roPerf-facter.cs
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/bisos/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.8/bisos/__init__.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/bisos/facter/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.8/bisos/facter/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.8/bisos/facter/facter.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.8/bisos/facter/facter_csu.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-12 04:40:28.342722 bisos.facter-0.8/bisos.facter.egg-info/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1993 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      430 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/SOURCES.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/dependency_links.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/not-zip-safe
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       72 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/requires.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-12 04:40:28.000000 bisos.facter-0.8/bisos.facter.egg-info/top_level.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-12 04:40:27.000000 bisos.facter-0.8/lh-agpl3-LICENSE.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-12 04:40:28.342722 bisos.facter-0.8/setup.cfg
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1896 2024-05-12 04:39:04.000000 bisos.facter-0.8/setup.py
```

### Comparing `bisos.facter-0.7/PKG-INFO` & `bisos.facter-0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.facter
-Version: 0.7
+Version: 0.8
 Summary: bisos.facter: Adoption and adaptation of facter to Python and PyCS-Framework and BISOS for use with BISOS-CMDB.
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
@@ -21,52 +21,63 @@
 Requires: blee
 Requires: blee.csPlayer
 Requires: bisos.transit
 Requires: bisos.b
 Requires: bisos.banna
 Requires: bisos.common
 
-============
-bisos.facter
-============
-
-.. contents::
-   :depth: 3
-..
-
 Overview
 ========
 
 bisos.facter: Adoption and adaptation of facter to Python and
 PyCS-Framework and BISOS for use with BISOS-CMDB.
 
-Support
-=======
+Mention What is BISOS.
 
-| For support, criticism, comments and questions; please contact the
-  author/maintainer
-| `Mohsen Banan <http://mohsen.1.banan.byname.net>`__ at:
-  http://mohsen.1.banan.byname.net/contact
+About facter
+============
 
-Documentation
-=============
+Facter gathers information about the system, which can be used as
+variables. Facter is part of puppet, but it can b used without puppet.
 
-Part of ByStar Digital Ecosystem http://www.by-star.net.
+To install facter:
 
-This module’s primary documentation is in
-http://www.by-star.net/PLPC/180047
+.. code:: bash
+
+   sudo apt-get install -y facter
+
+bisos.facter Is A Standalone Piece Of BISOS
+===========================================
+
+bisos.facter is a standalone piece of BISOS. It can be used byitself.
 
 Installation
 ============
 
 ::
 
-   sudo pip install bisos.facter
+   pip install bisos.facter
 
 Usage
 =====
 
 ::
 
    bin/facter.cs
 
+Support
+=======
+
+| For support, criticism, comments and questions; please contact the
+  author/maintainer
+| `Mohsen Banan <http://mohsen.1.banan.byname.net>`__ at:
+  http://mohsen.1.banan.byname.net/contact
+
+Documentation
+=============
+
+Part of ByStar Digital Ecosystem http://www.by-star.net.
+
+This module's primary documentation is in
+http://www.by-star.net/PLPC/180047
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bisos.facter-0.7/bin/facter.cs` & `bisos.facter-0.8/bin/facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.7/bin/roInv-facter.cs` & `bisos.facter-0.8/bin/roInv-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.7/bin/roPerf-facter.cs` & `bisos.facter-0.8/bin/roPerf-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.7/bisos/facter/facter.py` & `bisos.facter-0.8/bisos/facter/facter.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.7/bisos/facter/facter_csu.py` & `bisos.facter-0.8/bisos/facter/facter_csu.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.7/bisos.facter.egg-info/PKG-INFO` & `bisos.facter-0.8/bisos.facter.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.facter
-Version: 0.7
+Version: 0.8
 Summary: bisos.facter: Adoption and adaptation of facter to Python and PyCS-Framework and BISOS for use with BISOS-CMDB.
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
@@ -21,52 +21,63 @@
 Requires: blee
 Requires: blee.csPlayer
 Requires: bisos.transit
 Requires: bisos.b
 Requires: bisos.banna
 Requires: bisos.common
 
-============
-bisos.facter
-============
-
-.. contents::
-   :depth: 3
-..
-
 Overview
 ========
 
 bisos.facter: Adoption and adaptation of facter to Python and
 PyCS-Framework and BISOS for use with BISOS-CMDB.
 
-Support
-=======
+Mention What is BISOS.
 
-| For support, criticism, comments and questions; please contact the
-  author/maintainer
-| `Mohsen Banan <http://mohsen.1.banan.byname.net>`__ at:
-  http://mohsen.1.banan.byname.net/contact
+About facter
+============
 
-Documentation
-=============
+Facter gathers information about the system, which can be used as
+variables. Facter is part of puppet, but it can b used without puppet.
 
-Part of ByStar Digital Ecosystem http://www.by-star.net.
+To install facter:
 
-This module’s primary documentation is in
-http://www.by-star.net/PLPC/180047
+.. code:: bash
+
+   sudo apt-get install -y facter
+
+bisos.facter Is A Standalone Piece Of BISOS
+===========================================
+
+bisos.facter is a standalone piece of BISOS. It can be used byitself.
 
 Installation
 ============
 
 ::
 
-   sudo pip install bisos.facter
+   pip install bisos.facter
 
 Usage
 =====
 
 ::
 
    bin/facter.cs
 
+Support
+=======
+
+| For support, criticism, comments and questions; please contact the
+  author/maintainer
+| `Mohsen Banan <http://mohsen.1.banan.byname.net>`__ at:
+  http://mohsen.1.banan.byname.net/contact
+
+Documentation
+=============
+
+Part of ByStar Digital Ecosystem http://www.by-star.net.
+
+This module's primary documentation is in
+http://www.by-star.net/PLPC/180047
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bisos.facter-0.7/lh-agpl3-LICENSE.txt` & `bisos.facter-0.8/lh-agpl3-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.7/setup.py` & `bisos.facter-0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 #!/usr/bin/env python
 
 import setuptools
 # import sys
 
+import pypandoc
+
 
 def readme():
     with open('TITLE.txt') as f:
         return f.readline().rstrip('\n')
 
 
-def longDescription():
+def longDescriptionOld():
     with open('README.rst') as f:
         return f.read()
 
+def longDescription():
+    return pypandoc.convert_file('README.org', 'rst')
+
+
 
 # from setuphelpers import get_version, require_python
 # from setuptools import setup
 
 # __version__ = get_version('unisos/icm/__init__.py')
-__version__ = '0.7'
+__version__ = '0.8'
 
 
 requires = [
     "bisos",
     "blee",
     "blee.csPlayer",
     "bisos.transit",   # is used in bisos.b
```

