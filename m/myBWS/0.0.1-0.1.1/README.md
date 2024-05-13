# Comparing `tmp/myBWS-0.0.1.tar.gz` & `tmp/myBWS-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myBWS-0.0.1.tar", last modified: Tue Apr  9 20:02:48 2024, max compression
+gzip compressed data, was "dist\myBWS-0.1.1.tar", last modified: Mon May 13 07:25:52 2024, max compression
```

## Comparing `myBWS-0.0.1.tar` & `myBWS-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:02:48.385215 myBWS-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-09 20:02:48.338357 myBWS-0.0.1/BWS/
--rw-rw-rw-   0        0        0        0 2024-04-08 18:48:46.000000 myBWS-0.0.1/BWS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:02:48.340365 myBWS-0.0.1/BWS/api/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:16:08.000000 myBWS-0.0.1/BWS/api/__init__.py
--rw-rw-rw-   0        0        0      788 2024-04-09 20:01:44.000000 myBWS-0.0.1/BWS/api/api.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:02:48.343887 myBWS-0.0.1/BWS/database/
--rw-rw-rw-   0        0        0        0 2024-04-06 22:16:04.000000 myBWS-0.0.1/BWS/database/__init__.py
--rw-rw-rw-   0        0        0     7587 2024-04-09 17:47:23.000000 myBWS-0.0.1/BWS/database/db_interactions.py
--rw-rw-rw-   0        0        0        0 2024-04-06 19:43:23.000000 myBWS-0.0.1/BWS/database/sqlite.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:02:48.347403 myBWS-0.0.1/BWS/model/
--rw-rw-rw-   0        0        0     3057 2024-04-09 17:37:24.000000 myBWS-0.0.1/BWS/model/__init__.py
--rw-rw-rw-   0        0        0     1350 2024-04-09 17:47:42.000000 myBWS-0.0.1/BWS/model/analysis.py
--rw-rw-rw-   0        0        0     1144 2024-04-06 18:16:08.000000 myBWS-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      784 2024-04-09 20:02:48.383709 myBWS-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      427 2024-04-06 18:16:08.000000 myBWS-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 20:02:48.383709 myBWS-0.0.1/myBWS.egg-info/
--rw-rw-rw-   0        0        0      784 2024-04-09 20:02:48.000000 myBWS-0.0.1/myBWS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2024-04-09 20:02:48.000000 myBWS-0.0.1/myBWS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:02:48.000000 myBWS-0.0.1/myBWS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      515 2024-04-09 20:02:48.000000 myBWS-0.0.1/myBWS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-09 20:02:48.000000 myBWS-0.0.1/myBWS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 20:02:48.386224 myBWS-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1656 2024-04-09 20:02:16.000000 myBWS-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:25:52.453976 myBWS-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-13 07:25:52.369365 myBWS-0.1.1/BWS/
+-rw-rw-rw-   0        0        0      105 2024-05-06 18:52:45.000000 myBWS-0.1.1/BWS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:25:52.405098 myBWS-0.1.1/BWS/api/
+-rw-rw-rw-   0        0        0       90 2024-05-10 20:03:51.000000 myBWS-0.1.1/BWS/api/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-05-12 20:35:42.000000 myBWS-0.1.1/BWS/api/api_company_details.py
+-rw-rw-rw-   0        0        0     9130 2024-05-12 20:40:30.000000 myBWS-0.1.1/BWS/api/api_part2.py
+-rw-rw-rw-   0        0        0     1008 2024-05-12 20:43:14.000000 myBWS-0.1.1/BWS/api/api_part3.py
+-rw-rw-rw-   0        0        0      879 2024-05-12 20:41:47.000000 myBWS-0.1.1/BWS/api/api_update.py
+-rw-rw-rw-   0        0        0       46 2024-05-10 20:03:51.000000 myBWS-0.1.1/BWS/api/main.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:25:52.413090 myBWS-0.1.1/BWS/database/
+-rw-rw-rw-   0        0        0       38 2024-05-09 09:55:25.000000 myBWS-0.1.1/BWS/database/__init__.py
+-rw-rw-rw-   0        0        0    20357 2024-05-12 20:33:45.000000 myBWS-0.1.1/BWS/database/db_interactions.py
+-rw-rw-rw-   0        0        0      529 2024-05-06 16:46:20.000000 myBWS-0.1.1/BWS/database/sqlite.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:25:52.415181 myBWS-0.1.1/BWS/logger/
+-rw-rw-rw-   0        0        0       35 2024-05-06 18:59:43.000000 myBWS-0.1.1/BWS/logger/__init__.py
+-rw-rw-rw-   0        0        0     1548 2024-05-06 18:53:35.000000 myBWS-0.1.1/BWS/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:25:52.415181 myBWS-0.1.1/BWS/model/
+-rw-rw-rw-   0        0        0      100 2024-05-09 10:04:02.000000 myBWS-0.1.1/BWS/model/__init__.py
+-rw-rw-rw-   0        0        0     3772 2024-05-12 19:20:12.000000 myBWS-0.1.1/BWS/model/analysis.py
+-rw-rw-rw-   0        0        0     8174 2024-05-12 19:20:12.000000 myBWS-0.1.1/BWS/utils.py
+-rw-rw-rw-   0        0        0     1160 2024-04-10 18:19:11.000000 myBWS-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1552 2024-05-13 07:25:52.453976 myBWS-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2024-05-13 07:17:02.000000 myBWS-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 07:25:52.441522 myBWS-0.1.1/myBWS.egg-info/
+-rw-rw-rw-   0        0        0     1552 2024-05-13 07:25:51.000000 myBWS-0.1.1/myBWS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-13 07:25:51.000000 myBWS-0.1.1/myBWS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:25:51.000000 myBWS-0.1.1/myBWS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1077 2024-05-13 07:25:51.000000 myBWS-0.1.1/myBWS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-13 07:25:51.000000 myBWS-0.1.1/myBWS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 07:25:52.455174 myBWS-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2594 2024-05-13 07:24:25.000000 myBWS-0.1.1/setup.py
```

### Comparing `myBWS-0.0.1/LICENSE` & `myBWS-0.1.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Aram Barseghyan, Sergo Poghosyan, Arevik Papikyan, Nare Stepanyan.
+Copyright (c) 2024 Aram Barseghyan, Sergo Poghosyan, Arevik Papikyan, Nare Stepanyan, Elen Sukiasyan.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `myBWS-0.0.1/setup.py` & `myBWS-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,40 +16,71 @@
     classifiers=[
         "Development Status :: 3 - Alpha"
     ],
     python_requires=">=3.10, <3.12", 
     install_requires = [
         "annotated-types==0.6.0",
         "anyio==4.3.0",
+        "Babel==2.14.0",
+        "backports.tarfile==1.0.0",
+        "build==1.2.1",
+        "certifi==2024.2.2",
+        "charset-normalizer==3.3.2",
         "click==8.1.7",
         "colorama==0.4.6",
+        "docutils==0.21",
         "fastapi==0.110.0",
         "ghp-import==2.1.0",
+        "h11==0.14.0",
         "idna==3.6",
+        "importlib_metadata==7.1.0",
+        "jaraco.classes==3.4.0",
+        "jaraco.context==5.3.0",
+        "jaraco.functools==4.0.0",
         "Jinja2==3.1.3",
+        "keyring==25.1.0",
         "Markdown==3.6",
+        "markdown-it-py==3.0.0",
         "MarkupSafe==2.1.5",
+        "mdurl==0.1.2",
         "mergedeep==1.3.4",
-        "mkdocs==1.5.3",
+        "more-itertools==10.2.0",
+        "nh3==0.2.17",
         "numpy==1.26.4",
         "packaging==24.0",
+        "paginate==0.5.6",
         "pandas==2.2.1",
         "pathspec==0.12.1",
+        "pkginfo==1.10.0",
         "platformdirs==4.2.0",
         "pydantic==2.6.4",
         "pydantic_core==2.16.3",
+        "Pygments==2.17.2",
+        "pymdown-extensions==10.8",
+        "pyproject_hooks==1.0.0",
         "pyreadr==0.5.0",
         "python-dateutil==2.9.0.post0",
         "pytz==2024.1",
+        "pywin32-ctypes==0.2.2",
         "PyYAML==6.0.1",
         "pyyaml_env_tag==0.1",
+        "readme_renderer==43.0",
+        "regex==2024.4.16",
+        "requests==2.31.0",
+        "requests-toolbelt==1.0.0",
+        "rfc3986==2.0.0",
+        "rich==13.7.1",
+        "scipy==1.13.0",
         "six==1.16.0",
         "sniffio==1.3.1",
         "starlette==0.36.3",
+        "twine==5.0.0",
         "typing==3.7.4.3",
-        "typing_extensions==4.10.0",
         "tzdata==2024.1",
-        "watchdog==4.0.0"
-    ],
+        "urllib3==2.2.1",
+        "uvicorn==0.29.0",
+        "watchdog==4.0.0",
+        "zipp==3.18.1"
+        ],
     packages=find_packages(include=["BWS", 'BWS.*']),
-    version = "0.0.1"  
+    version = "0.1.1"  
 )
```

