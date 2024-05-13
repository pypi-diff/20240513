# Comparing `tmp/clipp-1.0.4.tar.gz` & `tmp/clipp-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipp-1.0.4.tar", last modified: Sat May 11 09:14:38 2024, max compression
+gzip compressed data, was "clipp-1.0.5.tar", last modified: Mon May 13 06:44:55 2024, max compression
```

## Comparing `clipp-1.0.4.tar` & `clipp-1.0.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.187219 clipp-1.0.4/
--rw-rw-r--   0 ben       (1000) ben       (1000)      193 2024-05-11 09:10:31.000000 clipp-1.0.4/.gitignore
--rw-rw-r--   0 ben       (1000) ben       (1000)    35149 2024-05-11 08:53:35.000000 clipp-1.0.4/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)    51409 2024-05-11 09:14:38.186219 clipp-1.0.4/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)    10520 2024-05-11 09:06:38.000000 clipp-1.0.4/README-PYPI.rst
--rw-rw-r--   0 ben       (1000) ben       (1000)    10570 2024-05-11 09:06:38.000000 clipp-1.0.4/README.rst
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.174219 clipp-1.0.4/clipp/
--rw-rw-r--   0 ben       (1000) ben       (1000)      417 2024-05-11 09:06:38.000000 clipp-1.0.4/clipp/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)    77860 2024-05-11 08:53:35.000000 clipp-1.0.4/clipp/core.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     8526 2024-05-11 08:54:11.000000 clipp-1.0.4/clipp/utils.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.185219 clipp-1.0.4/clipp.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)    51409 2024-05-11 09:14:38.000000 clipp-1.0.4/clipp.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)     2146 2024-05-11 09:14:38.000000 clipp-1.0.4/clipp.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        1 2024-05-11 09:14:38.000000 clipp-1.0.4/clipp.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       41 2024-05-11 09:14:38.000000 clipp-1.0.4/clipp.egg-info/requires.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        6 2024-05-11 09:14:38.000000 clipp-1.0.4/clipp.egg-info/top_level.txt
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.177219 clipp-1.0.4/docs/
--rw-rw-r--   0 ben       (1000) ben       (1000)      230 2024-05-11 09:06:38.000000 clipp-1.0.4/docs/.buildinfo
--rw-rw-r--   0 ben       (1000) ben       (1000)        0 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/.nojekyll
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.177219 clipp-1.0.4/docs/_sources/
--rw-rw-r--   0 ben       (1000) ben       (1000)       89 2024-05-11 08:53:36.000000 clipp-1.0.4/docs/_sources/clipp.rst.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)      430 2024-05-11 08:53:36.000000 clipp-1.0.4/docs/_sources/index.rst.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       52 2024-05-11 08:53:36.000000 clipp-1.0.4/docs/_sources/modules.rst.txt
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.179219 clipp-1.0.4/docs/_static/
--rw-rw-r--   0 ben       (1000) ben       (1000)    15094 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/_static/basic.css
--rw-rw-r--   0 ben       (1000) ben       (1000)     4472 2024-05-11 08:56:25.000000 clipp-1.0.4/docs/_static/doctools.js
--rw-rw-r--   0 ben       (1000) ben       (1000)      323 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/_static/documentation_options.js
--rw-rw-r--   0 ben       (1000) ben       (1000)      286 2024-05-11 08:56:25.000000 clipp-1.0.4/docs/_static/file.png
--rw-rw-r--   0 ben       (1000) ben       (1000)     4758 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/_static/language_data.js
--rw-rw-r--   0 ben       (1000) ben       (1000)       90 2024-05-11 08:56:25.000000 clipp-1.0.4/docs/_static/minus.png
--rw-rw-r--   0 ben       (1000) ben       (1000)       90 2024-05-11 08:56:25.000000 clipp-1.0.4/docs/_static/plus.png
--rw-rw-r--   0 ben       (1000) ben       (1000)    13656 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/_static/pygments.css
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.180219 clipp-1.0.4/docs/_static/scripts/
--rw-rw-r--   0 ben       (1000) ben       (1000)    81602 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/scripts/bootstrap.js
--rw-rw-r--   0 ben       (1000) ben       (1000)      237 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/scripts/bootstrap.js.LICENSE.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)   332914 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/scripts/bootstrap.js.map
--rw-rw-r--   0 ben       (1000) ben       (1000)     9399 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/scripts/pydata-sphinx-theme.js
--rw-rw-r--   0 ben       (1000) ben       (1000)    44317 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/scripts/pydata-sphinx-theme.js.map
--rw-rw-r--   0 ben       (1000) ben       (1000)    18732 2024-05-11 08:56:25.000000 clipp-1.0.4/docs/_static/searchtools.js
--rw-rw-r--   0 ben       (1000) ben       (1000)     5123 2024-05-11 08:56:25.000000 clipp-1.0.4/docs/_static/sphinx_highlight.js
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.181219 clipp-1.0.4/docs/_static/styles/
--rw-rw-r--   0 ben       (1000) ben       (1000)   208854 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/styles/bootstrap.css
--rw-rw-r--   0 ben       (1000) ben       (1000)   555088 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/styles/bootstrap.css.map
--rw-rw-r--   0 ben       (1000) ben       (1000)    72327 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/styles/pydata-sphinx-theme.css
--rw-rw-r--   0 ben       (1000) ben       (1000)   294060 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/styles/pydata-sphinx-theme.css.map
--rw-rw-r--   0 ben       (1000) ben       (1000)      106 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/styles/theme.css
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.172219 clipp-1.0.4/docs/_static/vendor/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.172219 clipp-1.0.4/docs/_static/vendor/fontawesome/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.181219 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/
--rw-rw-r--   0 ben       (1000) ben       (1000)     7427 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/LICENSE.txt
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.181219 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/css/
--rw-rw-r--   0 ben       (1000) ben       (1000)   102621 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/css/all.min.css
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.183219 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/js/
--rw-rw-r--   0 ben       (1000) ben       (1000)  1485766 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/js/all.min.js
--rw-rw-r--   0 ben       (1000) ben       (1000)      219 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.184219 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/
--rw-rw-r--   0 ben       (1000) ben       (1000)   207972 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
--rw-rw-r--   0 ben       (1000) ben       (1000)   117372 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
--rw-rw-r--   0 ben       (1000) ben       (1000)    68004 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
--rw-rw-r--   0 ben       (1000) ben       (1000)    25452 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
--rw-rw-r--   0 ben       (1000) ben       (1000)   419720 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
--rw-rw-r--   0 ben       (1000) ben       (1000)   156496 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
--rw-rw-r--   0 ben       (1000) ben       (1000)    10832 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
--rw-rw-r--   0 ben       (1000) ben       (1000)     4792 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
--rw-rw-r--   0 ben       (1000) ben       (1000)     1983 2024-05-11 08:56:26.000000 clipp-1.0.4/docs/_static/webpack-macros.html
--rw-rw-r--   0 ben       (1000) ben       (1000)    90535 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/clipp.html
--rw-rw-r--   0 ben       (1000) ben       (1000)    16254 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/genindex.html
--rw-rw-r--   0 ben       (1000) ben       (1000)    12872 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/index.html
--rw-rw-r--   0 ben       (1000) ben       (1000)    18607 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/modules.html
--rw-rw-r--   0 ben       (1000) ben       (1000)      519 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/objects.inv
--rw-rw-r--   0 ben       (1000) ben       (1000)    10976 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/py-modindex.html
--rw-rw-r--   0 ben       (1000) ben       (1000)    11296 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/search.html
--rw-rw-r--   0 ben       (1000) ben       (1000)     8701 2024-05-11 09:05:21.000000 clipp-1.0.4/docs/searchindex.js
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.185219 clipp-1.0.4/docsrc/
--rw-rw-r--   0 ben       (1000) ben       (1000)      711 2024-05-11 08:53:36.000000 clipp-1.0.4/docsrc/Makefile
--rw-rw-r--   0 ben       (1000) ben       (1000)       89 2024-05-11 08:53:36.000000 clipp-1.0.4/docsrc/clipp.rst
--rw-rw-r--   0 ben       (1000) ben       (1000)     2592 2024-05-11 08:53:36.000000 clipp-1.0.4/docsrc/conf.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      430 2024-05-11 08:53:36.000000 clipp-1.0.4/docsrc/index.rst
--rw-rw-r--   0 ben       (1000) ben       (1000)       52 2024-05-11 08:53:36.000000 clipp-1.0.4/docsrc/modules.rst
--rwxrwxr-x   0 ben       (1000) ben       (1000)      161 2024-05-11 08:53:36.000000 clipp-1.0.4/mkdocs.sh
--rw-rw-r--   0 ben       (1000) ben       (1000)      565 2024-05-11 08:53:36.000000 clipp-1.0.4/pyproject.toml
--rw-rw-r--   0 ben       (1000) ben       (1000)      132 2024-05-11 08:53:36.000000 clipp-1.0.4/requirements.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       38 2024-05-11 09:14:38.187219 clipp-1.0.4/setup.cfg
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-11 09:14:38.185219 clipp-1.0.4/tests/
--rw-rw-r--   0 ben       (1000) ben       (1000)     1990 2024-05-11 08:53:36.000000 clipp-1.0.4/tests/conftest.py
--rw-rw-r--   0 ben       (1000) ben       (1000)    15946 2024-05-11 08:53:36.000000 clipp-1.0.4/tests/test_core.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     5591 2024-05-11 08:53:36.000000 clipp-1.0.4/tests/test_utils.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.172133 clipp-1.0.5/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      193 2024-05-11 09:10:31.000000 clipp-1.0.5/.gitignore
+-rw-rw-r--   0 ben       (1000) ben       (1000)    35149 2024-05-11 08:53:35.000000 clipp-1.0.5/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)    51401 2024-05-13 06:44:55.171133 clipp-1.0.5/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)    10512 2024-05-13 06:39:09.000000 clipp-1.0.5/README-PYPI.rst
+-rw-rw-r--   0 ben       (1000) ben       (1000)    10566 2024-05-13 06:39:08.000000 clipp-1.0.5/README.rst
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.133132 clipp-1.0.5/clipp/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      417 2024-05-13 06:39:08.000000 clipp-1.0.5/clipp/__init__.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)    77891 2024-05-13 02:37:03.000000 clipp-1.0.5/clipp/core.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     8526 2024-05-11 08:54:11.000000 clipp-1.0.5/clipp/utils.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.168133 clipp-1.0.5/clipp.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)    51401 2024-05-13 06:44:54.000000 clipp-1.0.5/clipp.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)     2146 2024-05-13 06:44:55.000000 clipp-1.0.5/clipp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)        1 2024-05-13 06:44:54.000000 clipp-1.0.5/clipp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       41 2024-05-13 06:44:54.000000 clipp-1.0.5/clipp.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)        6 2024-05-13 06:44:54.000000 clipp-1.0.5/clipp.egg-info/top_level.txt
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.140133 clipp-1.0.5/docs/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      230 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/.buildinfo
+-rw-rw-r--   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/.nojekyll
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.141132 clipp-1.0.5/docs/_sources/
+-rw-rw-r--   0 ben       (1000) ben       (1000)       89 2024-05-11 08:53:36.000000 clipp-1.0.5/docs/_sources/clipp.rst.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)      430 2024-05-11 08:53:36.000000 clipp-1.0.5/docs/_sources/index.rst.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       52 2024-05-11 08:53:36.000000 clipp-1.0.5/docs/_sources/modules.rst.txt
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.146133 clipp-1.0.5/docs/_static/
+-rw-rw-r--   0 ben       (1000) ben       (1000)    15094 2024-05-13 06:44:10.000000 clipp-1.0.5/docs/_static/basic.css
+-rw-rw-r--   0 ben       (1000) ben       (1000)     4472 2024-05-11 08:56:25.000000 clipp-1.0.5/docs/_static/doctools.js
+-rw-rw-r--   0 ben       (1000) ben       (1000)      323 2024-05-13 06:44:10.000000 clipp-1.0.5/docs/_static/documentation_options.js
+-rw-rw-r--   0 ben       (1000) ben       (1000)      286 2024-05-11 08:56:25.000000 clipp-1.0.5/docs/_static/file.png
+-rw-rw-r--   0 ben       (1000) ben       (1000)     4758 2024-05-13 06:44:10.000000 clipp-1.0.5/docs/_static/language_data.js
+-rw-rw-r--   0 ben       (1000) ben       (1000)       90 2024-05-11 08:56:25.000000 clipp-1.0.5/docs/_static/minus.png
+-rw-rw-r--   0 ben       (1000) ben       (1000)       90 2024-05-11 08:56:25.000000 clipp-1.0.5/docs/_static/plus.png
+-rw-rw-r--   0 ben       (1000) ben       (1000)    13656 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/_static/pygments.css
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.148132 clipp-1.0.5/docs/_static/scripts/
+-rw-rw-r--   0 ben       (1000) ben       (1000)    81602 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/scripts/bootstrap.js
+-rw-rw-r--   0 ben       (1000) ben       (1000)      237 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)   332914 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/scripts/bootstrap.js.map
+-rw-rw-r--   0 ben       (1000) ben       (1000)     9399 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/scripts/pydata-sphinx-theme.js
+-rw-rw-r--   0 ben       (1000) ben       (1000)    44317 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/scripts/pydata-sphinx-theme.js.map
+-rw-rw-r--   0 ben       (1000) ben       (1000)    18732 2024-05-11 08:56:25.000000 clipp-1.0.5/docs/_static/searchtools.js
+-rw-rw-r--   0 ben       (1000) ben       (1000)     5123 2024-05-11 08:56:25.000000 clipp-1.0.5/docs/_static/sphinx_highlight.js
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.154132 clipp-1.0.5/docs/_static/styles/
+-rw-rw-r--   0 ben       (1000) ben       (1000)   208854 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/styles/bootstrap.css
+-rw-rw-r--   0 ben       (1000) ben       (1000)   555088 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/styles/bootstrap.css.map
+-rw-rw-r--   0 ben       (1000) ben       (1000)    72327 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/styles/pydata-sphinx-theme.css
+-rw-rw-r--   0 ben       (1000) ben       (1000)   294060 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/styles/pydata-sphinx-theme.css.map
+-rw-rw-r--   0 ben       (1000) ben       (1000)      106 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/styles/theme.css
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.128132 clipp-1.0.5/docs/_static/vendor/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.128132 clipp-1.0.5/docs/_static/vendor/fontawesome/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.154132 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     7427 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/LICENSE.txt
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.155133 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/css/
+-rw-rw-r--   0 ben       (1000) ben       (1000)   102621 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/css/all.min.css
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.159133 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/js/
+-rw-rw-r--   0 ben       (1000) ben       (1000)  1485766 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/js/all.min.js
+-rw-rw-r--   0 ben       (1000) ben       (1000)      219 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.164132 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/
+-rw-rw-r--   0 ben       (1000) ben       (1000)   207972 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
+-rw-rw-r--   0 ben       (1000) ben       (1000)   117372 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
+-rw-rw-r--   0 ben       (1000) ben       (1000)    68004 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
+-rw-rw-r--   0 ben       (1000) ben       (1000)    25452 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
+-rw-rw-r--   0 ben       (1000) ben       (1000)   419720 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
+-rw-rw-r--   0 ben       (1000) ben       (1000)   156496 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
+-rw-rw-r--   0 ben       (1000) ben       (1000)    10832 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
+-rw-rw-r--   0 ben       (1000) ben       (1000)     4792 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1983 2024-05-11 08:56:26.000000 clipp-1.0.5/docs/_static/webpack-macros.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)    90535 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/clipp.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)    16254 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/genindex.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)    12872 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/index.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)    18607 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/modules.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)      519 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/objects.inv
+-rw-rw-r--   0 ben       (1000) ben       (1000)    10976 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/py-modindex.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)    11296 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/search.html
+-rw-rw-r--   0 ben       (1000) ben       (1000)     8701 2024-05-13 06:44:11.000000 clipp-1.0.5/docs/searchindex.js
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.167132 clipp-1.0.5/docsrc/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      711 2024-05-11 08:53:36.000000 clipp-1.0.5/docsrc/Makefile
+-rw-rw-r--   0 ben       (1000) ben       (1000)       89 2024-05-11 08:53:36.000000 clipp-1.0.5/docsrc/clipp.rst
+-rw-rw-r--   0 ben       (1000) ben       (1000)     2592 2024-05-11 08:53:36.000000 clipp-1.0.5/docsrc/conf.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      430 2024-05-11 08:53:36.000000 clipp-1.0.5/docsrc/index.rst
+-rw-rw-r--   0 ben       (1000) ben       (1000)       52 2024-05-11 08:53:36.000000 clipp-1.0.5/docsrc/modules.rst
+-rwxrwxr-x   0 ben       (1000) ben       (1000)      161 2024-05-11 08:53:36.000000 clipp-1.0.5/mkdocs.sh
+-rw-rw-r--   0 ben       (1000) ben       (1000)      565 2024-05-11 08:53:36.000000 clipp-1.0.5/pyproject.toml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      132 2024-05-11 08:53:36.000000 clipp-1.0.5/requirements.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       38 2024-05-13 06:44:55.172133 clipp-1.0.5/setup.cfg
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-05-13 06:44:55.168133 clipp-1.0.5/tests/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1990 2024-05-11 08:53:36.000000 clipp-1.0.5/tests/conftest.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)    15946 2024-05-11 08:53:36.000000 clipp-1.0.5/tests/test_core.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     5591 2024-05-11 08:53:36.000000 clipp-1.0.5/tests/test_utils.py
```

### Comparing `clipp-1.0.4/LICENSE` & `clipp-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/PKG-INFO` & `clipp-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipp
-Version: 1.0.4
+Version: 1.0.5
 Summary: A POSIX-compliant CLI parser.
 Author: Ben Ohling
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,15 +688,15 @@
 
 #####
 Clipp
 #####
 
 .. The shorthand for line blocks doesn't render properly on github, so we are forced to use the line-break substitution.
 
-| **Latest Version:** 1.0.4
+| **Latest Version:** 1.0.5
 | **Status:** Beta, active development
 
 Clipp is a POSIX-compliant, CLI parser library for building command-line interfaces, designed to be flexible, intelligent, and uncompromisingly simple. The package is similar to argparse but aims to be more intuitive and less cumbersome. Clipp allows for greater code re-use than argparse and is much more scalable. In terms of parser latency, clipp typically outperforms argparse. Though clipp is much more minimalist than argparse, its API has most of the features you would expect to find in a command-line parsing library.
 
 .. contents:: Table of Contents
 
 Documentation
@@ -822,15 +822,15 @@
 	integer               An integer value.
 
 	Options:
 	--help, -h            Display this help message.
 	--mod, -m             Compute the sum mod N, where N is a valid
 	                      integer.
 	$ python3 -m sum 1 2 3 --mod
-	Namespace(globals={}, locals={'sum': {'value': 6, '--mod': 2}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'mod': 2}}, extra=[])
 
 
 In the command-line example above, we see that "--mod" now appears in the locals dictionary under "sum" (our command). Since no argument was supplied to "--mod", its value is equal to that of the ``const`` argument which we passed in the ``add_option`` method. The value of ``const`` is the value used by the parser when an option IS encountered but no arguments are received. The counterpart to the ``const`` argument is ``default`` which represents the value used by the parser whenever an option is NOT encountered at the command-line. Whether an option supports ``default`` or ``const`` is ultimately determined by its quota.
 
 .. admonition:: **Note**
 
 	For non-positional options, ``default`` and ``const`` are NOT supported if the parser expects to consume one, **or more**, argument tokens (i.e. ``quota`` > 1 or ``quota`` == "+"). For parameters, ``default`` and ``const`` are **only** supported for zero-or-more quotas (*).
@@ -853,15 +853,15 @@
 	if __name__ == "__main__":
 		processed = command.parse()
 		print(processed)
 
 .. code:: console
 
 	$ python3 -m sum 1 2 3 --hexify
-	Namespace(globals={}, locals={'sum': {'value': 6, '--hexify': True}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'hexify': True}}, extra=[])
 
 Notice that the values used above are boolean values, and the flag we have added ultimately represents a binary option. Clipp has a convenience method for binary flags. Let's adjust the code above and use the ``add_binary_flag`` method instead.
 
 .. code:: python
 
 	...
 
@@ -871,15 +871,15 @@
 	)
 
 	...
 
 .. code:: console
 
 	$ python3 -m sum 1 2 3 --hexify
-	Namespace(globals={}, locals={'sum': {'value': 6, '--hexify': True}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'hexify': True}}, extra=[])
 
 By default, the ``const`` argument of the method ``add_binary_flag`` is set to ``True``, and ``default`` is always the opposite of ``const``.
 
 A flag, however, may not be the best choice. Perhaps we want to allow users to select a particular result type. We can adjust the above code once more.
 
 .. code:: python
 
@@ -905,15 +905,15 @@
 	Options:
 	--help, -h            Display this help message.
 	--mod, -m             Compute the sum mod N, where N is a valid
 	                      integer.
 	--result-type, -t     Convert the result to either hexidecimal (hex)
 	                      or binary (bin).
 	$ python3 -m 1 2 3 -t bin
-	Namespace(globals={}, locals={'sum': {'value': 6, '--result-type': 'bin'}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'result_type': 'bin'}}, extra=[])
 
 At this point, our utility isn't very useful for the end-user. We'll need to make sure that our utility does what it claims if we want happy users.
 
 .. code:: python
 
 	def compute_result(options: dict) -> str:
 		value = options["value"]
```

### Comparing `clipp-1.0.4/README-PYPI.rst` & `clipp-1.0.5/README-PYPI.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #####
 Clipp
 #####
 
 .. The shorthand for line blocks doesn't render properly on github, so we are forced to use the line-break substitution.
 
-| **Latest Version:** 1.0.4
+| **Latest Version:** 1.0.5
 | **Status:** Beta, active development
 
 Clipp is a POSIX-compliant, CLI parser library for building command-line interfaces, designed to be flexible, intelligent, and uncompromisingly simple. The package is similar to argparse but aims to be more intuitive and less cumbersome. Clipp allows for greater code re-use than argparse and is much more scalable. In terms of parser latency, clipp typically outperforms argparse. Though clipp is much more minimalist than argparse, its API has most of the features you would expect to find in a command-line parsing library.
 
 .. contents:: Table of Contents
 
 Documentation
@@ -134,15 +134,15 @@
 	integer               An integer value.
 
 	Options:
 	--help, -h            Display this help message.
 	--mod, -m             Compute the sum mod N, where N is a valid
 	                      integer.
 	$ python3 -m sum 1 2 3 --mod
-	Namespace(globals={}, locals={'sum': {'value': 6, '--mod': 2}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'mod': 2}}, extra=[])
 
 
 In the command-line example above, we see that "--mod" now appears in the locals dictionary under "sum" (our command). Since no argument was supplied to "--mod", its value is equal to that of the ``const`` argument which we passed in the ``add_option`` method. The value of ``const`` is the value used by the parser when an option IS encountered but no arguments are received. The counterpart to the ``const`` argument is ``default`` which represents the value used by the parser whenever an option is NOT encountered at the command-line. Whether an option supports ``default`` or ``const`` is ultimately determined by its quota.
 
 .. admonition:: **Note**
 
 	For non-positional options, ``default`` and ``const`` are NOT supported if the parser expects to consume one, **or more**, argument tokens (i.e. ``quota`` > 1 or ``quota`` == "+"). For parameters, ``default`` and ``const`` are **only** supported for zero-or-more quotas (*).
@@ -165,15 +165,15 @@
 	if __name__ == "__main__":
 		processed = command.parse()
 		print(processed)
 
 .. code:: console
 
 	$ python3 -m sum 1 2 3 --hexify
-	Namespace(globals={}, locals={'sum': {'value': 6, '--hexify': True}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'hexify': True}}, extra=[])
 
 Notice that the values used above are boolean values, and the flag we have added ultimately represents a binary option. Clipp has a convenience method for binary flags. Let's adjust the code above and use the ``add_binary_flag`` method instead.
 
 .. code:: python
 
 	...
 
@@ -183,15 +183,15 @@
 	)
 
 	...
 
 .. code:: console
 
 	$ python3 -m sum 1 2 3 --hexify
-	Namespace(globals={}, locals={'sum': {'value': 6, '--hexify': True}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'hexify': True}}, extra=[])
 
 By default, the ``const`` argument of the method ``add_binary_flag`` is set to ``True``, and ``default`` is always the opposite of ``const``.
 
 A flag, however, may not be the best choice. Perhaps we want to allow users to select a particular result type. We can adjust the above code once more.
 
 .. code:: python
 
@@ -217,15 +217,15 @@
 	Options:
 	--help, -h            Display this help message.
 	--mod, -m             Compute the sum mod N, where N is a valid
 	                      integer.
 	--result-type, -t     Convert the result to either hexidecimal (hex)
 	                      or binary (bin).
 	$ python3 -m 1 2 3 -t bin
-	Namespace(globals={}, locals={'sum': {'value': 6, '--result-type': 'bin'}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'result_type': 'bin'}}, extra=[])
 
 At this point, our utility isn't very useful for the end-user. We'll need to make sure that our utility does what it claims if we want happy users.
 
 .. code:: python
 
 	def compute_result(options: dict) -> str:
 		value = options["value"]
```

### Comparing `clipp-1.0.4/README.rst` & `clipp-1.0.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 	<br />
 
 .. |hr| raw:: html
 
 	<hr />
 
-**Latest Version:** 1.0.4 |br|
-**Status:** Beta, active development
+| **Latest Version:** 1.0.5 |br|
+| **Status:** Beta, active development
 
 Clipp is a POSIX-compliant, CLI parser library for building command-line interfaces, designed to be flexible, intelligent, and uncompromisingly simple. The package is similar to argparse but aims to be more intuitive and less cumbersome. Clipp allows for greater code re-use than argparse and is much more scalable. In terms of parser latency, clipp typically outperforms argparse. Though clipp is much more minimalist than argparse, its API has most of the features you would expect to find in a command-line parsing library.
 
 Documentation
 =============
 
 Up-to-date API documentation can be found here: `<https://jammin93.github.io/clipp/>`_
@@ -144,15 +144,15 @@
 	integer               An integer value.
 
 	Options:
 	--help, -h            Display this help message.
 	--mod, -m             Compute the sum mod N, where N is a valid
 	                      integer.
 	$ python3 -m sum 1 2 3 --mod
-	Namespace(globals={}, locals={'sum': {'value': 6, '--mod': 2}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'mod': 2}}, extra=[])
 
 
 In the command-line example above, we see that "--mod" now appears in the locals dictionary under "sum" (our command). Since no argument was supplied to "--mod", its value is equal to that of the ``const`` argument which we passed in the ``add_option`` method. The value of ``const`` is the value used by the parser when an option IS encountered but no arguments are received. The counterpart to the ``const`` argument is ``default`` which represents the value used by the parser whenever an option is NOT encountered at the command-line. Whether an option supports ``default`` or ``const`` is ultimately determined by its quota.
 
 |hr|
 
 .. admonition:: **Note**
@@ -179,15 +179,15 @@
 	if __name__ == "__main__":
 		processed = command.parse()
 		print(processed)
 
 .. code:: console
 
 	$ python3 -m sum 1 2 3 --hexify
-	Namespace(globals={}, locals={'sum': {'value': 6, '--hexify': True}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'hexify': True}}, extra=[])
 
 Notice that the values used above are boolean values, and the flag we have added ultimately represents a binary option. Clipp has a convenience method for binary flags. Let's adjust the code above and use the ``add_binary_flag`` method instead.
 
 .. code:: python
 
 	...
 
@@ -197,15 +197,15 @@
 	)
 
 	...
 
 .. code:: console
 
 	$ python3 -m sum 1 2 3 --hexify
-	Namespace(globals={}, locals={'sum': {'value': 6, '--hexify': True}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'hexify': True}}, extra=[])
 
 By default, the ``const`` argument of the method ``add_binary_flag`` is set to ``True``, and ``default`` is always the opposite of ``const``.
 
 A flag, however, may not be the best choice. Perhaps we want to allow users to select a particular result type. We can adjust the above code once more.
 
 .. code:: python
 
@@ -231,15 +231,15 @@
 	Options:
 	--help, -h            Display this help message.
 	--mod, -m             Compute the sum mod N, where N is a valid
 	                      integer.
 	--result-type, -t     Convert the result to either hexidecimal (hex)
 	                      or binary (bin).
 	$ python3 -m 1 2 3 -t bin
-	Namespace(globals={}, locals={'sum': {'value': 6, '--result-type': 'bin'}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'result_type': 'bin'}}, extra=[])
 
 At this point, our utility isn't very useful for the end-user. We'll need to make sure that our utility does what it claims if we want happy users.
 
 .. code:: python
 
 	def compute_result(options: dict) -> str:
 		value = options["value"]
```

### Comparing `clipp-1.0.4/clipp/core.py` & `clipp-1.0.5/clipp/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
     def altname(self) -> str:
         """
         The alternative name for the option, used as the key in the namespace
         produced by parsing command-line arguments.
         """
         if self._dest:
             return self._dest
-        return self.name
+        return self.name.lstrip("--").replace("-", "_")
 
     @property
     def is_dependent(self) -> bool:
         """Indicates whether the option is part of a dependent group."""
         return self._is_dependent
 
     @property
```

### Comparing `clipp-1.0.4/clipp/utils.py` & `clipp-1.0.5/clipp/utils.py`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/clipp.egg-info/PKG-INFO` & `clipp-1.0.5/clipp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipp
-Version: 1.0.4
+Version: 1.0.5
 Summary: A POSIX-compliant CLI parser.
 Author: Ben Ohling
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,15 +688,15 @@
 
 #####
 Clipp
 #####
 
 .. The shorthand for line blocks doesn't render properly on github, so we are forced to use the line-break substitution.
 
-| **Latest Version:** 1.0.4
+| **Latest Version:** 1.0.5
 | **Status:** Beta, active development
 
 Clipp is a POSIX-compliant, CLI parser library for building command-line interfaces, designed to be flexible, intelligent, and uncompromisingly simple. The package is similar to argparse but aims to be more intuitive and less cumbersome. Clipp allows for greater code re-use than argparse and is much more scalable. In terms of parser latency, clipp typically outperforms argparse. Though clipp is much more minimalist than argparse, its API has most of the features you would expect to find in a command-line parsing library.
 
 .. contents:: Table of Contents
 
 Documentation
@@ -822,15 +822,15 @@
 	integer               An integer value.
 
 	Options:
 	--help, -h            Display this help message.
 	--mod, -m             Compute the sum mod N, where N is a valid
 	                      integer.
 	$ python3 -m sum 1 2 3 --mod
-	Namespace(globals={}, locals={'sum': {'value': 6, '--mod': 2}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'mod': 2}}, extra=[])
 
 
 In the command-line example above, we see that "--mod" now appears in the locals dictionary under "sum" (our command). Since no argument was supplied to "--mod", its value is equal to that of the ``const`` argument which we passed in the ``add_option`` method. The value of ``const`` is the value used by the parser when an option IS encountered but no arguments are received. The counterpart to the ``const`` argument is ``default`` which represents the value used by the parser whenever an option is NOT encountered at the command-line. Whether an option supports ``default`` or ``const`` is ultimately determined by its quota.
 
 .. admonition:: **Note**
 
 	For non-positional options, ``default`` and ``const`` are NOT supported if the parser expects to consume one, **or more**, argument tokens (i.e. ``quota`` > 1 or ``quota`` == "+"). For parameters, ``default`` and ``const`` are **only** supported for zero-or-more quotas (*).
@@ -853,15 +853,15 @@
 	if __name__ == "__main__":
 		processed = command.parse()
 		print(processed)
 
 .. code:: console
 
 	$ python3 -m sum 1 2 3 --hexify
-	Namespace(globals={}, locals={'sum': {'value': 6, '--hexify': True}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'hexify': True}}, extra=[])
 
 Notice that the values used above are boolean values, and the flag we have added ultimately represents a binary option. Clipp has a convenience method for binary flags. Let's adjust the code above and use the ``add_binary_flag`` method instead.
 
 .. code:: python
 
 	...
 
@@ -871,15 +871,15 @@
 	)
 
 	...
 
 .. code:: console
 
 	$ python3 -m sum 1 2 3 --hexify
-	Namespace(globals={}, locals={'sum': {'value': 6, '--hexify': True}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'hexify': True}}, extra=[])
 
 By default, the ``const`` argument of the method ``add_binary_flag`` is set to ``True``, and ``default`` is always the opposite of ``const``.
 
 A flag, however, may not be the best choice. Perhaps we want to allow users to select a particular result type. We can adjust the above code once more.
 
 .. code:: python
 
@@ -905,15 +905,15 @@
 	Options:
 	--help, -h            Display this help message.
 	--mod, -m             Compute the sum mod N, where N is a valid
 	                      integer.
 	--result-type, -t     Convert the result to either hexidecimal (hex)
 	                      or binary (bin).
 	$ python3 -m 1 2 3 -t bin
-	Namespace(globals={}, locals={'sum': {'value': 6, '--result-type': 'bin'}}, extra=[])
+	Namespace(globals={}, locals={'sum': {'value': 6, 'result_type': 'bin'}}, extra=[])
 
 At this point, our utility isn't very useful for the end-user. We'll need to make sure that our utility does what it claims if we want happy users.
 
 .. code:: python
 
 	def compute_result(options: dict) -> str:
 		value = options["value"]
```

### Comparing `clipp-1.0.4/clipp.egg-info/SOURCES.txt` & `clipp-1.0.5/clipp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/basic.css` & `clipp-1.0.5/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/doctools.js` & `clipp-1.0.5/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/language_data.js` & `clipp-1.0.5/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/pygments.css` & `clipp-1.0.5/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/scripts/bootstrap.js` & `clipp-1.0.5/docs/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/scripts/bootstrap.js.map` & `clipp-1.0.5/docs/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/scripts/pydata-sphinx-theme.js` & `clipp-1.0.5/docs/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/scripts/pydata-sphinx-theme.js.map` & `clipp-1.0.5/docs/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/searchtools.js` & `clipp-1.0.5/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/sphinx_highlight.js` & `clipp-1.0.5/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/styles/bootstrap.css` & `clipp-1.0.5/docs/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/styles/bootstrap.css.map` & `clipp-1.0.5/docs/_static/styles/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/styles/pydata-sphinx-theme.css` & `clipp-1.0.5/docs/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/styles/pydata-sphinx-theme.css.map` & `clipp-1.0.5/docs/_static/styles/pydata-sphinx-theme.css.map`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/LICENSE.txt` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/css/all.min.css` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/css/all.min.css`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/js/all.min.js` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/js/all.min.js`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2` & `clipp-1.0.5/docs/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/_static/webpack-macros.html` & `clipp-1.0.5/docs/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/clipp.html` & `clipp-1.0.5/docs/clipp.html`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/genindex.html` & `clipp-1.0.5/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/index.html` & `clipp-1.0.5/docs/index.html`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/modules.html` & `clipp-1.0.5/docs/modules.html`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/objects.inv` & `clipp-1.0.5/docs/objects.inv`

 * *Files 1% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: Clipp
-# Version: 1.0.3
+# Version: 1.0.5
 # The remainder of this file is compressed using zlib.
 
 clipp.__init__ py:module 0 clipp.html#module-$ -
 clipp.__init__.Command py:class 1 clipp.html#$ -
 clipp.__init__.Command.add_binary_flag py:method 1 clipp.html#$ -
 clipp.__init__.Command.add_fast_flag py:method 1 clipp.html#$ -
 clipp.__init__.Command.add_flag py:method 1 clipp.html#$ -
```

### Comparing `clipp-1.0.4/docs/py-modindex.html` & `clipp-1.0.5/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/search.html` & `clipp-1.0.5/docs/search.html`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docs/searchindex.js` & `clipp-1.0.5/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docsrc/Makefile` & `clipp-1.0.5/docsrc/Makefile`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/docsrc/conf.py` & `clipp-1.0.5/docsrc/conf.py`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/pyproject.toml` & `clipp-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/tests/conftest.py` & `clipp-1.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/tests/test_core.py` & `clipp-1.0.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `clipp-1.0.4/tests/test_utils.py` & `clipp-1.0.5/tests/test_utils.py`

 * *Files identical despite different names*

