# Comparing `tmp/pylliterate-0.0.5.tar.gz` & `tmp/pylliterate-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylliterate-0.0.5.tar", max compression
+gzip compressed data, was "pylliterate-0.0.6.tar", max compression
```

## Comparing `pylliterate-0.0.5.tar` & `pylliterate-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1100 2024-05-08 21:48:46.550511 pylliterate-0.0.5/LICENSE
--rw-r--r--   0        0        0    10157 2024-05-10 21:07:14.944125 pylliterate-0.0.5/pylliterate/__init__.py
--rw-r--r--   0        0        0      273 2024-04-24 20:27:28.869868 pylliterate-0.0.5/pylliterate/__main__.py
--rw-r--r--   0        0        0     3439 2024-05-10 20:54:10.623176 pylliterate-0.0.5/pylliterate/cli.py
--rw-r--r--   0        0        0     4135 2024-05-10 21:07:14.959765 pylliterate-0.0.5/pylliterate/config.py
--rw-r--r--   0        0        0    15018 2024-05-10 21:02:57.167931 pylliterate-0.0.5/pylliterate/core.py
--rw-r--r--   0        0        0      736 2024-05-10 20:18:17.432177 pylliterate-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8544 2024-04-30 05:00:19.884025 pylliterate-0.0.5/Readme.md
--rw-r--r--   0        0        0     9039 1970-01-01 00:00:00.000000 pylliterate-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-13 04:49:32.292423 pylliterate-0.0.6/LICENSE
+-rw-r--r--   0        0        0    10157 2024-05-13 04:49:32.292930 pylliterate-0.0.6/pylliterate/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-24 20:27:28.869868 pylliterate-0.0.6/pylliterate/__main__.py
+-rw-r--r--   0        0        0     3439 2024-05-13 04:49:32.293936 pylliterate-0.0.6/pylliterate/cli.py
+-rw-r--r--   0        0        0     4135 2024-05-13 04:49:32.294935 pylliterate-0.0.6/pylliterate/config.py
+-rw-r--r--   0        0        0    15018 2024-05-13 04:49:32.296071 pylliterate-0.0.6/pylliterate/core.py
+-rw-r--r--   0        0        0      737 2024-05-13 04:50:54.562706 pylliterate-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8544 2024-04-30 05:00:19.884025 pylliterate-0.0.6/Readme.md
+-rw-r--r--   0        0        0     9040 1970-01-01 00:00:00.000000 pylliterate-0.0.6/PKG-INFO
```

### Comparing `pylliterate-0.0.5/LICENSE` & `pylliterate-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.5/pylliterate/__init__.py` & `pylliterate-0.0.6/pylliterate/__init__.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.5/pylliterate/cli.py` & `pylliterate-0.0.6/pylliterate/cli.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.5/pylliterate/config.py` & `pylliterate-0.0.6/pylliterate/config.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.5/pylliterate/core.py` & `pylliterate-0.0.6/pylliterate/core.py`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.5/pyproject.toml` & `pylliterate-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pylliterate"
-version = "0.0.5"
+version = "0.0.6"
 description = "Unobtrusive literate programming experience for Python pragmatists"
 # Poetry is ignoring multiple autors configuration line but's ok :)
 authors = ["Alejandro Piad <alepiad@gmail.com>", "Jesús Enrique Fuentes <jesusefg12@gmail.com>"]
 
 license = "MIT"
 readme = "Readme.md"
 
 [tool.poetry.scripts]
 pylliterate = "pylliterate.cli:app"
 
 [tool.poetry.dependencies]
 python="^3.12"
 typer = "^0.12.3"
-rich = "^9.0.1"
+rich = "^13.7.1"
 PyYAML = "^6.0.1"
 pydantic = "^2.7.1"
 watchdog = "^2.3.1"
 
 [tool.poetry.dev-dependencies]
 mkdocs = "1.5.3"
 black = "24.4.0"
```

### Comparing `pylliterate-0.0.5/Readme.md` & `pylliterate-0.0.6/Readme.md`

 * *Files identical despite different names*

### Comparing `pylliterate-0.0.5/PKG-INFO` & `pylliterate-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pylliterate
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unobtrusive literate programming experience for Python pragmatists
 License: MIT
 Author: Alejandro Piad
 Author-email: alepiad@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
-Requires-Dist: rich (>=9.0.1,<10.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Requires-Dist: watchdog (>=2.3.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Pylliterate: python illiterate programing
 
 [<img alt="PyPI" src="https://img.shields.io/pypi/v/pylliterate">](https://pypi.org/project/pylliterate)
```

