# Comparing `tmp/openhexa_toolbox-0.2.1.tar.gz` & `tmp/openhexa_toolbox-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa_toolbox-0.2.1.tar", last modified: Fri May 10 15:23:56 2024, max compression
+gzip compressed data, was "openhexa_toolbox-0.2.2.tar", last modified: Mon May 13 08:57:20 2024, max compression
```

## Comparing `openhexa_toolbox-0.2.1.tar` & `openhexa_toolbox-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.427989 openhexa_toolbox-0.2.1/openhexa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.427989 openhexa_toolbox-0.2.1/openhexa/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.427989 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/dhis2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/periods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 15:23:56.000000 openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:23:56.431989 openhexa_toolbox-0.2.1/tests/dhis2/
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/tests/dhis2/test_dhis2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/tests/dhis2/test_dhis2_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 15:23:31.000000 openhexa_toolbox-0.2.1/tests/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.187732 openhexa_toolbox-0.2.2/openhexa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.187732 openhexa_toolbox-0.2.2/openhexa/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.187732 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/periods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/tests/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/tests/dhis2/test_dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/tests/dhis2/test_dhis2_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/tests/test_lib.py
```

### Comparing `openhexa_toolbox-0.2.1/LICENSE` & `openhexa_toolbox-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.1/PKG-INFO` & `openhexa_toolbox-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.1 Summary: A set of
+Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.2 Summary: A set of
 tools to acquire & process data from various sources Author-email: Bluesquare
 bluesquarehub.com> Maintainer-email: Bluesquare
 bluesquarehub.com> License: MIT License Copyright (c) 2023 Bluesquare
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `openhexa_toolbox-0.2.1/README.md` & `openhexa_toolbox-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/api.py` & `openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/api.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/dhis2.py` & `openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/dhis2.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         """
         params = {"fields": "id,name,level,path,geometry"}
         if filter:
             params["filter"] = filter
         org_units = []
         for page in self.client.api.get_paged(
             "organisationUnits",
-            params=filter,
+            params=params,
             page_size=1000,
         ):
             page = page.json()
             for ou in page["organisationUnits"]:
                 org_units.append(
                     {
                         "id": ou.get("id"),
```

### Comparing `openhexa_toolbox-0.2.1/openhexa/toolbox/dhis2/periods.py` & `openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/periods.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/api.py` & `openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/api.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/parse.py` & `openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/parse.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.1/openhexa/toolbox/kobo/utils.py` & `openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/utils.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/PKG-INFO` & `openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.1 Summary: A set of
+Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.2 Summary: A set of
 tools to acquire & process data from various sources Author-email: Bluesquare
 bluesquarehub.com> Maintainer-email: Bluesquare
 bluesquarehub.com> License: MIT License Copyright (c) 2023 Bluesquare
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `openhexa_toolbox-0.2.1/openhexa.toolbox.egg-info/SOURCES.txt` & `openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.1/pyproject.toml` & `openhexa_toolbox-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openhexa.toolbox"
-version = "0.2.1"
+version = "0.2.2"
 description = "A set of tools to acquire & process data from various sources"
 authors = [{ name = "Bluesquare", email = "dev@bluesquarehub.com" }]
 maintainers = [{ name = "Bluesquare", email = "dev@bluesquarehub.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `openhexa_toolbox-0.2.1/tests/dhis2/test_dhis2.py` & `openhexa_toolbox-0.2.2/tests/dhis2/test_dhis2.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.1/tests/dhis2/test_dhis2_periods.py` & `openhexa_toolbox-0.2.2/tests/dhis2/test_dhis2_periods.py`

 * *Files identical despite different names*

