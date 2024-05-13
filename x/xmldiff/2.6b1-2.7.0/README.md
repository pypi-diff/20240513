# Comparing `tmp/xmldiff-2.6b1.tar.gz` & `tmp/xmldiff-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmldiff-2.6b1.tar", last modified: Thu Jan 12 08:50:49 2023, max compression
+gzip compressed data, was "xmldiff-2.7.0.tar", last modified: Mon May 13 12:15:38 2024, max compression
```

## Comparing `xmldiff-2.6b1.tar` & `xmldiff-2.7.0.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.532935 xmldiff-2.6b1/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       74 2023-01-12 08:50:49.000000 xmldiff-2.6b1/.coveragerc
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       46 2023-01-12 08:50:49.000000 xmldiff-2.6b1/.coveralls.yml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      566 2023-01-12 08:50:49.000000 xmldiff-2.6b1/.travis.yml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2751 2023-01-12 08:50:49.000000 xmldiff-2.6b1/CHANGES.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1064 2023-01-12 08:50:49.000000 xmldiff-2.6b1/LICENSE.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      409 2023-01-12 08:50:49.000000 xmldiff-2.6b1/MANIFEST.in
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1058 2023-01-12 08:50:49.000000 xmldiff-2.6b1/Makefile
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7203 2023-01-12 08:50:49.532935 xmldiff-2.6b1/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3333 2023-01-12 08:50:49.000000 xmldiff-2.6b1/README.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      143 2023-01-12 08:50:49.000000 xmldiff-2.6b1/README.txt
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.528935 xmldiff-2.6b1/docs/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7669 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/Makefile
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7260 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/make.bat
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/requirements.txt
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.528935 xmldiff-2.6b1/docs/source/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8636 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/advanced.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    17152 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/api.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3239 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/commandline.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9332 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/conf.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4207 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/contributing.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      842 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/index.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      796 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/installation.rst
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.528935 xmldiff-2.6b1/docs/source/static/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4647 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/static/htmlformatter.xslt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1610 2023-01-12 08:50:49.532935 xmldiff-2.6b1/setup.cfg
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-01-12 08:50:49.000000 xmldiff-2.6b1/setup.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.532935 xmldiff-2.6b1/tests/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       55 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.532935 xmldiff-2.6b1/tests/test_data/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      736 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/all_actions.expected.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      323 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/all_actions.left.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      305 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/all_actions.right.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      134 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/bom_1.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      134 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/bom_2.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      695 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/complex-text-update.expected.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      333 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/complex-text-update.left.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      407 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/complex-text-update.right.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      367 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/example.expected.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      145 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/example.left.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      158 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/example.right.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      156 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/insert-node.diff
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      125 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/insert-node.expected.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       40 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/insert-node.left.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       63 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/insert-node.right.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18828 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/rmldoc.expected.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    17427 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/rmldoc.left.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    17910 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/rmldoc.right.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1482 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/sbt_template.expected.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      939 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/sbt_template.left.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1229 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/sbt_template.right.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    57557 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_diff.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    21656 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_formatting.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6712 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_main.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7664 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_patch.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4972 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_utils.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1730 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/testing.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.528935 xmldiff-2.6b1/xmldiff/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      723 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/actions.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    19328 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/diff.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    80394 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/diff_match_patch.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    30028 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/formatting.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7230 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/main.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5172 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/patch.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4116 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/utils.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.532935 xmldiff-2.6b1/xmldiff.egg-info/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7203 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1698 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/SOURCES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/dependency_links.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       92 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/entry_points.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       82 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/requires.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        8 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/top_level.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/zip-safe
+drwxr-xr-x   0 a748031   (1000) a748031   (1000)        0 2024-05-13 12:15:38.185385 xmldiff-2.7.0/
+-rw-r--r--   0 a748031   (1000) a748031   (1000)       74 2024-05-13 12:15:38.000000 xmldiff-2.7.0/.coveragerc
+-rw-r--r--   0 a748031   (1000) a748031   (1000)       46 2024-05-13 12:15:38.000000 xmldiff-2.7.0/.coveralls.yml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      566 2024-05-13 12:15:38.000000 xmldiff-2.7.0/.travis.yml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     4237 2024-05-13 12:15:38.000000 xmldiff-2.7.0/CHANGES.rst
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      248 2024-05-13 12:15:38.000000 xmldiff-2.7.0/CHANGES.txt
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     1064 2024-05-13 12:15:38.000000 xmldiff-2.7.0/LICENSE.txt
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      409 2024-05-13 12:15:38.000000 xmldiff-2.7.0/MANIFEST.in
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     1058 2024-05-13 12:15:38.000000 xmldiff-2.7.0/Makefile
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     9040 2024-05-13 12:15:38.185385 xmldiff-2.7.0/PKG-INFO
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     3445 2024-05-13 12:15:38.000000 xmldiff-2.7.0/README.rst
+drwxr-xr-x   0 a748031   (1000) a748031   (1000)        0 2024-05-13 12:15:38.175385 xmldiff-2.7.0/docs/
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     7669 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/Makefile
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     7260 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/make.bat
+-rw-r--r--   0 a748031   (1000) a748031   (1000)       23 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/requirements.txt
+drwxr-xr-x   0 a748031   (1000) a748031   (1000)        0 2024-05-13 12:15:38.175385 xmldiff-2.7.0/docs/source/
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     8783 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/source/advanced.rst
+-rw-r--r--   0 a748031   (1000) a748031   (1000)    18116 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/source/api.rst
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     3239 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/source/commandline.rst
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     9337 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/source/conf.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     4207 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/source/contributing.rst
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      842 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/source/index.rst
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      796 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/source/installation.rst
+drwxr-xr-x   0 a748031   (1000) a748031   (1000)        0 2024-05-13 12:15:38.175385 xmldiff-2.7.0/docs/source/static/
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     4647 2024-05-13 12:15:38.000000 xmldiff-2.7.0/docs/source/static/htmlformatter.xslt
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     1611 2024-05-13 12:15:38.185385 xmldiff-2.7.0/setup.cfg
+-rw-r--r--   0 a748031   (1000) a748031   (1000)       38 2024-05-13 12:15:38.000000 xmldiff-2.7.0/setup.py
+drwxr-xr-x   0 a748031   (1000) a748031   (1000)        0 2024-05-13 12:15:38.175385 xmldiff-2.7.0/tests/
+-rw-r--r--   0 a748031   (1000) a748031   (1000)       55 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/__init__.py
+drwxr-xr-x   0 a748031   (1000) a748031   (1000)        0 2024-05-13 12:15:38.175385 xmldiff-2.7.0/tests/test_data/
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      881 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/all_actions.expected.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      430 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/all_actions.left.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      413 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/all_actions.right.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      134 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/bom_1.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      134 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/bom_2.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      695 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/complex-text-update.expected.html
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      333 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/complex-text-update.left.html
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      407 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/complex-text-update.right.html
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      367 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/example.expected.html
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      145 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/example.left.html
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      158 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/example.right.html
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      156 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/insert-node.diff
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      125 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/insert-node.expected.html
+-rw-r--r--   0 a748031   (1000) a748031   (1000)       40 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/insert-node.left.html
+-rw-r--r--   0 a748031   (1000) a748031   (1000)       63 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/insert-node.right.html
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      273 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/namespace.expected.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      119 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/namespace.left.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      102 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/namespace.right.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)    18828 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/rmldoc.expected.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)    17427 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/rmldoc.left.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)    17910 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/rmldoc.right.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     1482 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/sbt_template.expected.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      939 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/sbt_template.left.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     1229 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_data/sbt_template.right.xml
+-rw-r--r--   0 a748031   (1000) a748031   (1000)    57588 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_diff.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)    23847 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_formatting.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     6712 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_main.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     8294 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_patch.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     4971 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/test_utils.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     1730 2024-05-13 12:15:38.000000 xmldiff-2.7.0/tests/testing.py
+drwxr-xr-x   0 a748031   (1000) a748031   (1000)        0 2024-05-13 12:15:38.175385 xmldiff-2.7.0/xmldiff/
+-rw-r--r--   0 a748031   (1000) a748031   (1000)        0 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff/__init__.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)      844 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff/actions.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)    20168 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff/diff.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)    80401 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff/diff_match_patch.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)    33782 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff/formatting.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     7630 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff/main.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     5817 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff/patch.py
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     4280 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff/utils.py
+drwxr-xr-x   0 a748031   (1000) a748031   (1000)        0 2024-05-13 12:15:38.175385 xmldiff-2.7.0/xmldiff.egg-info/
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     9040 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff.egg-info/PKG-INFO
+-rw-r--r--   0 a748031   (1000) a748031   (1000)     1809 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff.egg-info/SOURCES.txt
+-rw-r--r--   0 a748031   (1000) a748031   (1000)        1 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff.egg-info/dependency_links.txt
+-rw-r--r--   0 a748031   (1000) a748031   (1000)       92 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff.egg-info/entry_points.txt
+-rw-r--r--   0 a748031   (1000) a748031   (1000)       82 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff.egg-info/requires.txt
+-rw-r--r--   0 a748031   (1000) a748031   (1000)        8 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff.egg-info/top_level.txt
+-rw-r--r--   0 a748031   (1000) a748031   (1000)        1 2024-05-13 12:15:38.000000 xmldiff-2.7.0/xmldiff.egg-info/zip-safe
```

### Comparing `xmldiff-2.6b1/.travis.yml` & `xmldiff-2.7.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/LICENSE.txt` & `xmldiff-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/Makefile` & `xmldiff-2.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/PKG-INFO` & `xmldiff-2.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmldiff
-Version: 2.6b1
+Version: 2.7.0
 Summary: Creates diffs of XML files
 Home-page: https://github.com/Shoobx/xmldiff
 Author: Lennart Regebro
 Author-email: lregebro@shoobx.com
 License: MIT
 Project-URL: Source Code, https://github.com/Shoobx/xmldiff
 Keywords: xml,html,diff
@@ -12,24 +12,30 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Provides-Extra: devenv
+Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: lxml>=3.1.0
+Provides-Extra: devenv
+Requires-Dist: black; extra == "devenv"
+Requires-Dist: coverage; extra == "devenv"
+Requires-Dist: flake8; extra == "devenv"
+Requires-Dist: zest.releaser[recommended]; extra == "devenv"
 
 xmldiff
 ========
 
 .. image:: https://travis-ci.org/Shoobx/xmldiff.svg?branch=master
   :target: https://travis-ci.org/Shoobx/xmldiff
 
@@ -113,23 +119,74 @@
 
  * Albertas Agejevas, alga@shoobx.com
 
  * Greg Kempe, greg@laws.africa
 
  * Filip Demski, glamhoth@protonmail.com
 
-The diff algorithm is based on "`Change Detection in Hierarchically Structured Information <http://ilpubs.stanford.edu/115/1/1995-46.pdf>`_",
+ * Jacek Chałupka, krunchfrompoland@gmail.com
+
+ * Thomas Pfitzinger, thpfitzinger@web.de
+
+The diff algorithm is based on
+"`Change Detection in Hierarchically Structured Information <http://infolab.stanford.edu/c3/papers/html/tdiff3-8/tdiff3-8.html>`_",
 and the text diff is using Google's ``diff_match_patch`` algorithm.
 
 Changes
 =======
 
+2.7.0 (2024-05-13)
+------------------
+
+- Changed the comparison to make accurate and standard more accurate,
+  although fast gets less accurate as a result.
+
+- Changed usage of deprecated `pkg_resources` package to `importlib.metadata`.
+
+- A `use_replace` flag was added to the `XMLFormatter` by Thomas Pfitzinger.
+  It changes text replacement from delete and insert tags to a replace tag.
+  It's not currently accessaible thtough the CLI, the question is it is better
+  to add a new formatter name, or an option to pass in formatter flags.
+
+  - Added option to XMLFormatter to use replace tags
+  - in _make_diff_tags after diffing, neighboring delete/insert diffs are joined to a replace tag
+  - the deleted text is added as an attribute ("old-text")
+  - the inserted text is the element's text
+
+2.6.3 (2023-05-21)
+------------------
+
+- And there was a namespace bug in the patch as well. #118
+
+
+2.6.2 (2023-05-21)
+------------------
+
+- Solved an error in the xmlformatter when using default namespaces. #89
+
+
+2.6.1 (2023-04-05)
+------------------
+
+- #108: Fixed an error that happens if using namespaces like ns0 or ns1.
+
+
+2.6 (2023-04-03)
+----------------
+
+- Added `InsertNamespace` and `DeleteNamespace` actions for better handling
+  of changing namespaces. Should improve any "Unknown namespace prefix"
+  errors. Changing the URI of a a namespace prefix is not supported, and will
+  raise an error.
+
 2.6b1 (2023-01-12)
 ------------------
 
+- Used geometric mean for the node_ratio, for better handling of simple nodes.
+
 - Added an experimental --best-match method that is slower, but generate
   smaller diffs when you have many nodes that are similar.
 
 - The -F argument now also affects the --fast-match stage.
 
 
 2.5 (2023-01-11)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xmldiff-2.6b1/README.rst` & `xmldiff-2.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -84,9 +84,14 @@
 
  * Albertas Agejevas, alga@shoobx.com
 
  * Greg Kempe, greg@laws.africa
 
  * Filip Demski, glamhoth@protonmail.com
 
-The diff algorithm is based on "`Change Detection in Hierarchically Structured Information <http://ilpubs.stanford.edu/115/1/1995-46.pdf>`_",
+ * Jacek Chałupka, krunchfrompoland@gmail.com
+
+ * Thomas Pfitzinger, thpfitzinger@web.de
+
+The diff algorithm is based on
+"`Change Detection in Hierarchically Structured Information <http://infolab.stanford.edu/c3/papers/html/tdiff3-8/tdiff3-8.html>`_",
 and the text diff is using Google's ``diff_match_patch`` algorithm.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xmldiff-2.6b1/docs/Makefile` & `xmldiff-2.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/docs/make.bat` & `xmldiff-2.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/docs/source/advanced.rst` & `xmldiff-2.7.0/docs/source/advanced.rst`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,21 @@
 the output can in some cases be less than useful,
 especially in the case where formatting is added:
 
 .. doctest::
   :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
 
   >>> left = '<body><p>My Fine Content</p></body>'
-  >>> right = '<body><p>My <i>Fine</i> Content</p></body>'
+  >>> right = '<body><p><b>My <i>Fine</i> Content</b></p></body>'
   >>> result = main.diff_texts(left, right, formatter=formatter)
   >>> print(result)
   <body xmlns:diff="http://namespaces.shoobx.com/diff">
-    <p diff:insert="">My <i diff:insert="">Fine</i><diff:insert> Content</diff:insert></p>
+    <p diff:insert="">
+      <b diff:insert="" diff:rename="p">My <i diff:insert="">Fine</i><diff:insert> Content</diff:insert></b>
+    </p>
     <p diff:delete="">My Fine Content</p>
   </body>
   <BLANKLINE>
 
 Notice how the the whole text was inserted with formatting,
 and the whole unformatted text was deleted.
 The XMLFormatter supports a better handling of text with the ``text_tags`` and ``formatting_tags`` parameters. Here is a simple and incomplete example with some common HTML tags:
@@ -62,15 +64,17 @@
   >>> formatter=formatting.XMLFormatter(
   ...     text_tags=('p', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'li'),
   ...     formatting_tags=('b', 'u', 'i', 'strike', 'em', 'super',
   ...                      'sup', 'sub', 'link', 'a', 'span'))
   >>> result = main.diff_texts(left, right, formatter=formatter)
   >>> print(result)
   <body xmlns:diff="http://namespaces.shoobx.com/diff">
-    <p>My <i diff:insert-formatting="">Fine</i> Content</p>
+    <p>
+      <b diff:insert-formatting="">My <i diff:insert-formatting="">Fine</i> Content</b>
+    </p>
   </body>
 
 This gives a result that flags the ``<i>`` tag as new formatting.
 This more compact output is much more useful and easier to transform into a visual output.
 
 
 Making a Visual Diff
@@ -130,15 +134,17 @@
   >>> formatter = HTMLFormatter(
   ...     text_tags=('p', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'li'),
   ...     formatting_tags=('b', 'u', 'i', 'strike', 'em', 'super',
   ...                      'sup', 'sub', 'link', 'a', 'span'))
   >>> result = main.diff_texts(left, right, formatter=formatter)
   >>> print(result)
   <body xmlns:diff="http://namespaces.shoobx.com/diff">
-    <p>My <i class="insert-formatting">Fine</i> Content</p>
+    <p>
+      <b class="insert-formatting">My <i class="insert-formatting">Fine</i> Content</b>
+    </p>
   </body>
 
 You can then add into your CSS files classes that make inserted text green,
 deleted text red with an overstrike,
 and formatting changes could for example be blue.
 This makes it easy to see what has been changed in a HTML document.
```

### Comparing `xmldiff-2.6b1/docs/source/api.rst` & `xmldiff-2.7.0/docs/source/api.rst`

 * *Files 3% similar despite different names*

```diff
@@ -444,14 +444,50 @@
 
   >>> left = '<document><node>Content</node></document>'
   >>> right = '<document><!-- A comment --><node>Content</node></document>'
   >>> main.diff_texts(left, right)
   [InsertComment(target='/document[1]', position=0, text=' A comment ')]
 
 
+``InsertNamespace(prefix, uri)``
+................................
+
+Adds a new namespace to the XML document. You need to have this before
+adding a node that uses a namespace that is not in the original XML tree.
+
+Example:
+
+.. doctest::
+  :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+  >>> left = '<document></document>'
+  >>> right = '<document xmlns:new="http://theuri"></document>'
+  >>> main.diff_texts(left, right)
+  [InsertNamespace(prefix='new', uri='http://theuri')]
+
+
+``DeleteNamespace(prefix)``
+................................
+
+Removes a namespace from the XML document. You don't need to handle this,
+strictly speaking, nothing will break if there is an unused namespace,
+but `xmldiff` will return this action.
+
+Example:
+
+.. doctest::
+  :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
+
+  >>> left = '<document xmlns:new="http://theuri"></document>'
+  >>> right = '<document></document>'
+  >>> main.diff_texts(left, right)
+  [DeleteNamespace(prefix='new')]
+
+
+
 The patching API
 ----------------
 
 There is also an API to patch files using the diff output:
 
 .. doctest::
   :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
```

### Comparing `xmldiff-2.6b1/docs/source/commandline.rst` & `xmldiff-2.7.0/docs/source/commandline.rst`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/docs/source/conf.py` & `xmldiff-2.7.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.doctest",
     "sphinx.ext.coverage",
-    "sphinxarg.ext",
+    #    "sphinxarg.ext",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -62,15 +62,15 @@
 # release = u'2.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command-line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
```

### Comparing `xmldiff-2.6b1/docs/source/contributing.rst` & `xmldiff-2.7.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/docs/source/index.rst` & `xmldiff-2.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/docs/source/installation.rst` & `xmldiff-2.7.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/docs/source/static/htmlformatter.xslt` & `xmldiff-2.7.0/docs/source/static/htmlformatter.xslt`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/setup.cfg` & `xmldiff-2.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [metadata]
 name = xmldiff
-version = 2.6b1
+version = 2.7.0
 description = Creates diffs of XML files
 long_description = file: README.rst, CHANGES.rst
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Intended Audience :: End Users/Desktop
 	Topic :: Text Processing :: Markup :: XML
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: PyPy
 keywords = xml, html, diff
 author = Lennart Regebro
 author_email = lregebro@shoobx.com
 url = https://github.com/Shoobx/xmldiff
 license = MIT
 project_urls = 
 	Source Code = https://github.com/Shoobx/xmldiff
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 zip_safe = True
 include_package_data = True
 packages = find:
 package_dir = 
 	= .
 install_requires = 
 	setuptools
```

### Comparing `xmldiff-2.6b1/tests/test_data/complex-text-update.expected.html` & `xmldiff-2.7.0/tests/test_data/complex-text-update.expected.html`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/tests/test_data/rmldoc.expected.xml` & `xmldiff-2.7.0/tests/test_data/rmldoc.expected.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/tests/test_data/rmldoc.left.xml` & `xmldiff-2.7.0/tests/test_data/rmldoc.left.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/tests/test_data/rmldoc.right.xml` & `xmldiff-2.7.0/tests/test_data/rmldoc.right.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/tests/test_data/sbt_template.expected.xml` & `xmldiff-2.7.0/tests/test_data/sbt_template.expected.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/tests/test_data/sbt_template.left.xml` & `xmldiff-2.7.0/tests/test_data/sbt_template.left.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/tests/test_data/sbt_template.right.xml` & `xmldiff-2.7.0/tests/test_data/sbt_template.right.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/tests/test_diff.py` & `xmldiff-2.7.0/tests/test_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,20 +179,20 @@
 
         self.assertEqual(differ.leaf_ratio(left, right), 1.0)
 
         # These nodes have slightly different text, but no children
         left = lefttree.xpath("/document/story/section[2]/para")[0]
         right = righttree.xpath("/document/story/section[2]/para")[0]
 
-        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.75)
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.80952380)
 
         # These nodes should not be very similar
         left = lefttree.xpath("/document/story/section[1]/para")[0]
         right = righttree.xpath("/document/story/section[1]/para")[0]
-        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.45614035087719)
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.53731343)
 
     def test_compare_different_nodes(self):
         left = """<document>
     <story firstPageTemplate="FirstPage">
         <section ref="2" single-ref="2">
             <para>First paragraph</para>
             <para>Second paragraph</para>
@@ -289,15 +289,15 @@
 
         # Make some choice comparisons here.
 
         left = differ.left.xpath("/document/story/section[1]")[0]
         right = differ.right.xpath("/document/story/section[1]")[0]
 
         # These are very similar
-        self.assertEqual(differ.leaf_ratio(left, right), 0.9)
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.9210526)
         # And one out of two children in common
         self.assertEqual(differ.child_ratio(left, right), 0.5)
         # But different id's, hence 0 as match
         self.assertEqual(differ.node_ratio(left, right), 0)
 
         # Here's the ones with the same id:
         left = differ.left.xpath("/document/story/section[1]")[0]
@@ -308,15 +308,15 @@
         # But same id's, hence 1 as match
         self.assertEqual(differ.node_ratio(left, right), 1.0)
 
         # The last ones are completely similar, but only one
         # has an xml:id, so they do not match.
         left = differ.left.xpath("/document/story/section[3]")[0]
         right = differ.right.xpath("/document/story/section[3]")[0]
-        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.81818181818)
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.8666667)
         self.assertEqual(differ.child_ratio(left, right), 1.0)
         self.assertEqual(differ.node_ratio(left, right), 0)
 
     def test_compare_with_uniqueattrs(self):
         # `uniqueattrs` can be pairs of (tag, attribute) as well as just string
         # attributes.
         left = dedent(
@@ -372,15 +372,15 @@
 
         # Make some choice comparisons here.
 
         left = differ.left.xpath("/document/story/section[1]")[0]
         right = differ.right.xpath("/document/story/section[1]")[0]
 
         # These are very similar
-        self.assertEqual(differ.leaf_ratio(left, right), 0.90625)
+        self.assertEqual(differ.leaf_ratio(left, right), 0.925)
         # And one out of two children in common
         self.assertEqual(differ.child_ratio(left, right), 0.5)
         # But different names, hence 0 as match
         self.assertEqual(differ.node_ratio(left, right), 0)
 
         # Here's the ones with the same tag and name attribute:
         left = differ.left.xpath("/document/story/section[1]")[0]
@@ -391,25 +391,25 @@
         # But same id's, hence 1 as match
         self.assertEqual(differ.node_ratio(left, right), 1.0)
 
         # The last ones are completely similar, but only one
         # has an name, so they do not match.
         left = differ.left.xpath("/document/story/section[3]")[0]
         right = differ.right.xpath("/document/story/section[3]")[0]
-        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.78260869565)
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.8387097)
         self.assertEqual(differ.child_ratio(left, right), 1.0)
         self.assertEqual(differ.node_ratio(left, right), 0)
 
         # Now these are structurally similar, have the same name, but
         # one of them is not a section, so the uniqueattr does not match
         left = differ.left.xpath("/document/story/section[1]")[0]
         right = differ.right.xpath("/document/story/subsection[1]")[0]
-        self.assertAlmostEqual(differ.leaf_ratio(left, right), 1.0)
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.9638554)
         self.assertEqual(differ.child_ratio(left, right), 0.5)
-        self.assertAlmostEqual(differ.node_ratio(left, right), 0.7905694150420949)
+        self.assertAlmostEqual(differ.node_ratio(left, right), 0.7677947)
 
     def test_compare_node_rename(self):
         left = """<document>
   <para>First paragraph</para>
   <para attr="value">Second paragraph</para>
   <para attr="value">Third paragraph</para>
 </document>
@@ -426,32 +426,32 @@
         differ.set_trees(etree.fromstring(left), etree.fromstring(right))
         differ.match()
 
         # Make some choice comparisons here.
         left = differ.left.xpath("/document/para[1]")[0]
         right = differ.right.xpath("/document/section[1]")[0]
 
-        # These have different tags, but should still match
-        self.assertEqual(differ.leaf_ratio(left, right), 1.0)
+        # These have different tags, so don't match that great any more
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.7441860)
 
         # These have different tags, and different attribute value,
         # but still similar enough
         left = differ.left.xpath("/document/para[2]")[0]
         right = differ.right.xpath("/document/section[2]")[0]
 
-        # These have different tags, but should still match
-        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.76190476190476)
+        # These have different tags, so don't match that great any more
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.6578947)
 
         # These have different tags, and different attribute value,
         # but still similar enough
         left = differ.left.xpath("/document/para[3]")[0]
         right = differ.right.xpath("/document/section[3]")[0]
 
         # These are too different
-        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.45161290322580)
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.4)
 
     def test_compare_namespaces(self):
         left = """<document>
   <foo:para xmlns:foo="someuri">First paragraph</foo:para>
 </document>
 """
 
@@ -468,40 +468,40 @@
         left = differ.left.xpath(
             "/document/foo:para[1]", namespaces={"foo": "someuri"}
         )[0]
         right = differ.right.xpath(
             "/document/foo:para[1]", namespaces={"foo": "otheruri"}
         )[0]
 
-        # These have different namespaces, but should still match
-        self.assertEqual(differ.leaf_ratio(left, right), 1.0)
+        # These have different namespaces, but should still match OK
+        self.assertAlmostEqual(differ.leaf_ratio(left, right), 0.915254237)
 
     def test_different_ratio_modes(self):
         node1 = etree.Element("para")
         node1.text = "This doesn't match at all"
         node2 = etree.Element("para")
         node2.text = "It's completely different"
         node3 = etree.Element("para")
         node3.text = "Completely different from before"
 
         # These texts are very different
         differ = Differ(ratio_mode="accurate")
-        self.assertAlmostEqual(differ.leaf_ratio(node1, node2), 0.24)
+        self.assertAlmostEqual(differ.leaf_ratio(node1, node2), 0.3666667)
         # However, the quick_ratio doesn't catch that, and think they match
         differ = Differ(ratio_mode="fast")
-        self.assertAlmostEqual(differ.leaf_ratio(node1, node2), 0.64)
+        self.assertAlmostEqual(differ.leaf_ratio(node1, node2), 0.7)
         # It still realizes these sentences are different, though.
         differ = Differ(ratio_mode="fast")
-        self.assertAlmostEqual(differ.leaf_ratio(node1, node3), 0.4561403508)
+        self.assertAlmostEqual(differ.leaf_ratio(node1, node3), 0.53731343)
         # Faster thinks the first two are the same!
         differ = Differ(ratio_mode="faster")
         self.assertAlmostEqual(differ.leaf_ratio(node1, node2), 1.0)
         # And that the third is almost the same
         differ = Differ(ratio_mode="faster")
-        self.assertAlmostEqual(differ.leaf_ratio(node1, node3), 0.8771929824)
+        self.assertAlmostEqual(differ.leaf_ratio(node1, node3), 0.89552238)
 
         # Invalid modes raise error:
         with self.assertRaises(ValueError):
             differ = Differ(ratio_mode="allezlebleus")
 
 
 class MatchTests(unittest.TestCase):
@@ -636,15 +636,14 @@
                 ("/document/story/section[3]", "/document/story/section[4]"),
                 ("/document/story", "/document/story"),
                 ("/document", "/document"),
             ],
         )
 
     def test_change_attribs(self):
-
         left = """<document>
     <story firstPageTemplate="FirstPage">
         <section xml:id="oldfirst" ref="3" single-ref="3">
             <para>First</para>
         </section>
         <section xml:id="oldlast" ref="4" single-ref="4">
             <para>Last</para>
```

### Comparing `xmldiff-2.6b1/tests/test_formatting.py` & `xmldiff-2.7.0/tests/test_formatting.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,62 +12,62 @@
 
 
 class PlaceholderMakerTests(unittest.TestCase):
     def test_get_placeholder(self):
         replacer = formatting.PlaceholderMaker()
         # Get a placeholder:
         ph = replacer.get_placeholder(etree.Element("tag"), formatting.T_OPEN, None)
-        self.assertEqual(ph, "\ue005")
+        self.assertEqual(ph, "\ue007")
         # Do it again:
         ph = replacer.get_placeholder(etree.Element("tag"), formatting.T_OPEN, None)
-        self.assertEqual(ph, "\ue005")
+        self.assertEqual(ph, "\ue007")
         # Get another one
         ph = replacer.get_placeholder(etree.Element("tag"), formatting.T_CLOSE, ph)
-        self.assertEqual(ph, "\ue006")
+        self.assertEqual(ph, "\ue008")
 
     def test_do_element(self):
         replacer = formatting.PlaceholderMaker(["p"], ["b"])
 
         # Formatting tags get replaced, and the content remains
         text = "<p>This is a tag with <b>formatted</b> text.</p>"
         element = etree.fromstring(text)
         replacer.do_element(element)
 
         self.assertEqual(
             etree.tounicode(element),
-            "<p>This is a tag with \ue006formatted\ue005 text.</p>",
+            "<p>This is a tag with \ue008formatted\ue007 text.</p>",
         )
 
         replacer.undo_element(element)
         self.assertEqual(etree.tounicode(element), text)
 
         # Non formatting tags get replaced with content
         text = "<p>This is a tag with <foo>formatted</foo> text.</p>"
         element = etree.fromstring(text)
         replacer.do_element(element)
         result = etree.tounicode(element)
-        self.assertEqual(result, "<p>This is a tag with \ue007 text.</p>")
+        self.assertEqual(result, "<p>This is a tag with \ue009 text.</p>")
 
         # Single formatting tags still get two placeholders.
         text = "<p>This is a <b/> with <foo/> text.</p>"
         element = etree.fromstring(text)
         replacer.do_element(element)
         result = etree.tounicode(element)
-        self.assertEqual(result, "<p>This is a \ue009\ue008 with \ue00a text.</p>")
+        self.assertEqual(result, "<p>This is a \ue00b\ue00a with \ue00c text.</p>")
 
     def test_do_undo_element(self):
         replacer = formatting.PlaceholderMaker(["p"], ["b"])
 
         # Formatting tags get replaced, and the content remains
         text = "<p>This <is/> a <f>tag</f> with <b>formatted</b> text.</p>"
         element = etree.fromstring(text)
         replacer.do_element(element)
 
         self.assertEqual(
-            element.text, "This \ue005 a \ue006 with \ue008formatted" "\ue007 text."
+            element.text, "This \ue007 a \ue008 with \ue00aformatted" "\ue009 text."
         )
 
         replacer.undo_element(element)
         result = etree.tounicode(element)
         self.assertEqual(result, text)
 
     def test_do_undo_element_double_format(self):
@@ -75,15 +75,15 @@
 
         # Formatting tags get replaced, and the content remains
         text = "<p>This is <u>doubly <b>formatted</b></u> text.</p>"
         element = etree.fromstring(text)
         replacer.do_element(element)
 
         self.assertEqual(
-            element.text, "This is \ue006doubly \ue008formatted\ue007" "\ue005 text."
+            element.text, "This is \ue008doubly \ue00aformatted\ue009" "\ue007 text."
         )
 
         replacer.undo_element(element)
         result = etree.tounicode(element)
         self.assertEqual(result, text)
 
     def test_rml_bug(self):
@@ -106,25 +106,25 @@
                 "i",
             ),
         )
         replacer.do_tree(tree)
         after_diff = """<document xmlns:diff="http://namespaces.shoobx.com/diff">
   <section>
     <para>
-      <insert>\ue005</insert>.
-      \ue007\ue009At Will Employment\ue008\ue006
+      <insert>\ue007</insert>.
+      \ue009\ue00bAt Will Employment\ue00a\ue008
       .\u201c<insert>New </insert>Text\u201d
     </para>
   </section>
 </document>"""
 
         # The diff formatting will find some text to insert.
         delete_attrib = "{%s}delete-format" % formatting.DIFF_NS
-        replacer.placeholder2tag["\ue006"].element.attrib[delete_attrib] = ""
-        replacer.placeholder2tag["\ue007"].element.attrib[delete_attrib] = ""
+        replacer.placeholder2tag["\ue008"].element.attrib[delete_attrib] = ""
+        replacer.placeholder2tag["\ue009"].element.attrib[delete_attrib] = ""
         tree = etree.fromstring(after_diff)
         replacer.undo_tree(tree)
         result = etree.tounicode(tree)
         expected = """<document xmlns:diff="http://namespaces.shoobx.com/diff">
   <section>
     <para>
       <insert><ref>4</ref></insert>.
@@ -149,15 +149,15 @@
             # Formatting tags get replaced, and the content remains
             text = "<p>This <is/> a <f>tag</f> with <b>some</b> text.</p>"
             element = etree.fromstring(text)
             replacer.do_element(element)
 
             #
             self.assertEqual(
-                element.text, "This \uf904 a \uf905 with \uf907some" "\uf906 text."
+                element.text, "This \uf906 a \uf907 with \uf909some" "\uf908 text."
             )
 
             try:
                 # If this is a wide build, also test what happens if we
                 # get over 8192 substitutions, and overflow the 2-byte code.
                 # (On narrow builds this will give an error)
                 formatting.PLACEHOLDER_START = 0xFFFF
@@ -168,30 +168,30 @@
                 text = "<p>This <is/> a <f>tag</f> with <b>some</b> text.</p>"
                 element = etree.fromstring(text)
                 replacer.do_element(element)
 
                 # This should raise an error on a narrow build
                 self.assertEqual(
                     element.text,
-                    "This \U00010004 a \U00010005 with \U00010007some"
-                    "\U00010006 text.",
+                    "This \U00010006 a \U00010007 with \U00010009some"
+                    "\U00010008 text.",
                 )
             except ValueError:
                 if sys.maxunicode > 0x10000:
                     # This is a wide build, we should NOT get an error
                     raise
 
         finally:
             # Set it back
             formatting.PLACEHOLDER_START = orig_start
 
 
 class XMLFormatTests(unittest.TestCase):
-    def _format_test(self, left, action, expected):
-        formatter = formatting.XMLFormatter(pretty_print=False)
+    def _format_test(self, left, action, expected, use_replace=False):
+        formatter = formatting.XMLFormatter(pretty_print=False, use_replace=use_replace)
         result = formatter.format([action], etree.fromstring(left))
         self.assertEqual(result, expected)
 
     def test_incorrect_xpaths(self):
         left = '<document><node a="v"/><node>Text</node></document>'
         expected = START + ' diff:delete-attr="a">Text' + END
 
@@ -313,14 +313,59 @@
             START + "/><diff:delete>This is</diff:delete>"
             "<diff:insert>Also</diff:insert> a bit of text, ri<diff:delete>"
             "ght</diff:delete><diff:insert>ck</diff:insert></document>"
         )
 
         self._format_test(left, action, expected)
 
+    def test_replace_text_in(self):
+        left = '<document><node attr="val"/></document>'
+        action = actions.UpdateTextIn("/document/node", "Text")
+        expected = START + ' attr="val"><diff:insert>Text</diff:insert>' + END
+
+        self._format_test(left, action, expected, use_replace=True)
+
+        left = "<document><node>This is a bit of text, right" + END
+        action = actions.UpdateTextIn("/document/node", "Also a bit of text, rick")
+        expected = (
+            START + '><diff:replace old-text="This is">Also</diff:replace>'
+            ' a bit of text, ri<diff:replace old-text="ght">ck'
+            "</diff:replace>" + END
+        )
+
+        self._format_test(left, action, expected, use_replace=True)
+
+    def test_replace_text_after_1(self):
+        left = "<document><node/><node/></document>"
+        action = actions.UpdateTextAfter("/document/node[1]", "Text")
+        expected = START + "/><diff:insert>Text</diff:insert>" "<node/></document>"
+
+        self._format_test(left, action, expected, use_replace=True)
+
+    def test_replace_text_after_2(self):
+        left = "<document><node/>This is a bit of text, right</document>"
+        action = actions.UpdateTextAfter("/document/node", "Also a bit of text, rick")
+        expected = (
+            START + '/><diff:replace old-text="This is">Also</diff:replace>'
+            ' a bit of text, ri<diff:replace old-text="ght">ck'
+            "</diff:replace></document>"
+        )
+
+        self._format_test(left, action, expected, use_replace=True)
+
+    def test_replace_complete_text(self):
+        left = "<document><node>aaaaaaa bbbbbb</node></document>"
+        action = actions.UpdateTextIn("/document/node", "ccccc dddd eee")
+        expected = (
+            START + '><diff:replace old-text="aaaaaaa bbbbbb">ccccc dddd eee'
+            "</diff:replace>" + END
+        )
+
+        self._format_test(left, action, expected, use_replace=True)
+
 
 class DiffFormatTests(unittest.TestCase):
     def _format_test(self, action, expected):
         formatter = formatting.DiffFormatter()
         result = formatter.format([action], None)
         self.assertEqual(result, expected)
 
@@ -484,14 +529,16 @@
         here = os.path.split(__file__)[0]
         lfile = os.path.join(here, "test_data", "all_actions.left.xml")
         rfile = os.path.join(here, "test_data", "all_actions.right.xml")
 
         formatter = formatting.XmlDiffFormatter()
         result = main.diff_files(lfile, rfile, formatter=formatter)
         expected = (
+            "[insert-namespace, space, http://namespaces.shoobx.com/outerspace]\n"
+            "[delete-namespace, name]\n"
             "[move-after, /document/node[2], /document/tag[1]]\n"
             "[insert-comment, /document[1], 0,  Insert a new comment ]\n"
             '[update, /document/node[1]/@name, "was updated"]\n'
             "[remove, /document/node[1]/@attribute]\n"
             "[insert, /document/node[1], \n"
             "<@newtribute>\n"
             "renamed\n"
@@ -501,43 +548,40 @@
             "is new\n"
             "</@this>]\n"
             "[remove, /document/node[1]/@attr]\n"
             '[update, /document/node[1]/text()[1], "\\n    Modified\\n  "]\n'
             '[update, /document/node[1]/text()[2], "\\n    '
             'New tail content\\n  "]\n'
             "[rename, /document/node[2], nod]\n"
-            "[insert-after, /document/tail[1], \n"
-            "<new/>]\n"
+            "[rename, /document/name:space[1], {http://namespaces.shoobx.com/outerspace}name]\n"
+            '[update, /document/space:name[1]/text()[2], "\\n  "]\n'
             "[remove, /document/tail[1]]"
         )
         self.assertEqual(result, expected)
 
 
 class FormatterFileTests(unittest.TestCase):
-
     formatter = None  # Override this
     maxDiff = None
 
     def process(self, left, right):
         return main.diff_files(left, right, formatter=self.formatter)
 
 
 class XMLFormatterFileTests(FormatterFileTests):
-
     # The XMLFormatter has no text or formatting tags, so
     formatter = formatting.XMLFormatter(
         pretty_print=False, normalize=formatting.WS_TEXT
     )
 
 
 # Also test the bits that handle text tags:
 
 
 class HTMLFormatterFileTests(FormatterFileTests):
-
     # We use a few tags for the placeholder tests.
     # <br/> is intentionally left out, to test an edge case
     # with empty non-formatting tags in text.
     formatter = formatting.XMLFormatter(
         normalize=formatting.WS_BOTH,
         pretty_print=True,
         text_tags=("p", "h1", "h2", "h3", "h4", "h5", "h6", "li"),
```

### Comparing `xmldiff-2.6b1/tests/test_main.py` & `xmldiff-2.7.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/tests/test_patch.py` & `xmldiff-2.7.0/tests/test_patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     InsertComment,
 )
 
 from .testing import compare_elements
 
 
 class PatcherTests(unittest.TestCase):
-
     patcher = Patcher()
 
     def _test(self, start, action, end):
         tree = etree.fromstring(start)
         self.patcher.handle_action(action, tree)
         self.assertEqual(etree.tounicode(tree), end)
 
@@ -113,14 +112,29 @@
 
         left = etree.parse(lfile)
         right = etree.parse(rfile)
         diff = diff_trees(left, right)
         result = Patcher().patch(diff, left)
 
         # This example has top level comments, and lxml doesn't deal well
+        # with that, so the trees are not EXACTLY the same, the trailing
+        # top level comment differs, but that's OK.
+        compare_elements(result, right.getroot())
+
+    def test_diff_default_namespace(self):
+        here = os.path.split(__file__)[0]
+        lfile = os.path.join(here, "test_data", "namespace.left.xml")
+        rfile = os.path.join(here, "test_data", "namespace.right.xml")
+
+        left = etree.parse(lfile)
+        right = etree.parse(rfile)
+        diff = diff_trees(left, right)
+        result = Patcher().patch(diff, left)
+
+        # This example has top level comments, and lxml doesn't deal well
         # with that, so the trees are not EXACTLY the same, the trailing
         # top level comment differs, but that's OK.
         compare_elements(result, right.getroot())
 
 
 TEST_DIFF = """[delete, node]
 [insert, target, tag, 0]
```

### Comparing `xmldiff-2.6b1/tests/test_utils.py` & `xmldiff-2.7.0/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,14 @@
         for x, y in utils.longest_common_subsequence(left, right):
             self.assertEqual(left[x], right[y])
             res.append(left[x])
 
         self.assertEqual("".join(res), result)
 
     def test_lcs(self):
-
         self._diff("ABCDEF", "ABCDEF", "ABCDEF")
 
         self._diff("ABCDEF", "GHIJKL", "")
 
         self._diff("ABCDEF", "ACDQRB", "ACD")
 
         self._diff("CXCDEFX", "CDEFX", "CDEFX")
```

### Comparing `xmldiff-2.6b1/tests/testing.py` & `xmldiff-2.7.0/tests/testing.py`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6b1/xmldiff/actions.py` & `xmldiff-2.7.0/xmldiff/actions.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,7 +11,10 @@
 
 UpdateAttrib = namedtuple("UpdateAttrib", "node name value")
 DeleteAttrib = namedtuple("DeleteAttrib", "node name")
 InsertAttrib = namedtuple("InsertAttrib", "node name value")
 RenameAttrib = namedtuple("RenameAttrib", "node oldname newname")
 
 InsertComment = namedtuple("InsertComment", "target position text")
+
+InsertNamespace = namedtuple("InsertNamespace", "prefix uri")
+DeleteNamespace = namedtuple("DeleteNamespace", "prefix")
```

### Comparing `xmldiff-2.6b1/xmldiff/diff.py` & `xmldiff-2.7.0/xmldiff/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,15 +219,15 @@
             match = sqrt((match**2 + child_ratio**2) / 2)
         return match
 
     def node_text(self, node):
         if node in self._text_cache:
             return self._text_cache[node]
         # Get the texts and the tag as a start
-        texts = node.xpath("text()")
+        texts = [node.tag] + node.xpath("text()")
 
         # Then add attributes and values
         for tag, value in sorted(self.node_attribs(node).items()):
             if tag[0] == "{":
                 tag = tag.split(
                     "}",
                 )[-1]
@@ -422,14 +422,35 @@
             self._inorder.add(rchild)
 
     def diff(self, left=None, right=None):
         # Make sure the matching is done first, diff() needs the l2r/r2l maps.
         if not self._matches:
             self.match(left, right)
 
+        # First, deal with namespaces:
+        rnsmap = self.right.nsmap
+        lnsmap = self.left.nsmap
+        for k, v in rnsmap.items():
+            # Make sure it's registered:
+            if k is not None and not utils.RESERVED_NS.match(k):
+                etree.register_namespace(k, v)
+            if k not in lnsmap:
+                yield actions.InsertNamespace(k, v)
+            elif lnsmap[k] != v:
+                raise RuntimeError(
+                    "Sorry, we do not support changing the URI of namespaces in xmldiff"
+                )
+
+        for k, v in lnsmap.items():
+            # Make sure it's registered:
+            if k is not None and not utils.RESERVED_NS.match(k):
+                etree.register_namespace(k, v)
+            if k not in rnsmap:
+                yield actions.DeleteNamespace(k)
+
         # The paper talks about the five phases, and then does four of them
         # in one phase, in a different order that described. This
         # implementation in turn differs in order yet again.
         ltree = self.left.getroottree()
 
         for rnode in utils.breadth_first_traverse(self.right):
             # (a)
```

### Comparing `xmldiff-2.6b1/xmldiff/diff_match_patch.py` & `xmldiff-2.7.0/xmldiff/diff_match_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
     # The data structure representing a diff is an array of tuples:
     # [(DIFF_DELETE, "Hello"), (DIFF_INSERT, "Goodbye"), (DIFF_EQUAL, " world.")]
     # which means: delete "Hello", add "Goodbye" and keep " world."
     DIFF_DELETE = -1
     DIFF_INSERT = 1
     DIFF_EQUAL = 0
+    DIFF_REPLACE = 2
 
     def diff_main(self, text1, text2, checklines=True, deadline=None):
         """Find the differences between two texts.  Simplifies the problem by
           stripping any common prefix or suffix off the texts before diffing.
 
         Args:
           text1: Old string to be diffed.
@@ -1131,15 +1132,15 @@
         Args:
           diffs: Array of diff tuples.
 
         Returns:
           HTML representation.
         """
         html = []
-        for (op, data) in diffs:
+        for op, data in diffs:
             text = (
                 data.replace("&", "&amp;")
                 .replace("<", "&lt;")
                 .replace(">", "&gt;")
                 .replace("\n", "&para;<br>")
             )
             if op == self.DIFF_INSERT:
@@ -1156,30 +1157,30 @@
         Args:
           diffs: Array of diff tuples.
 
         Returns:
           Source text.
         """
         text = []
-        for (op, data) in diffs:
+        for op, data in diffs:
             if op != self.DIFF_INSERT:
                 text.append(data)
         return "".join(text)
 
     def diff_text2(self, diffs):
         """Compute and return the destination text (all equalities and insertions).
 
         Args:
           diffs: Array of diff tuples.
 
         Returns:
           Destination text.
         """
         text = []
-        for (op, data) in diffs:
+        for op, data in diffs:
             if op != self.DIFF_DELETE:
                 text.append(data)
         return "".join(text)
 
     def diff_levenshtein(self, diffs):
         """Compute the Levenshtein distance; the number of inserted, deleted or
         substituted characters.
@@ -1189,15 +1190,15 @@
 
         Returns:
           Number of changes.
         """
         levenshtein = 0
         insertions = 0
         deletions = 0
-        for (op, data) in diffs:
+        for op, data in diffs:
             if op == self.DIFF_INSERT:
                 insertions += len(data)
             elif op == self.DIFF_DELETE:
                 deletions += len(data)
             elif op == self.DIFF_EQUAL:
                 # A deletion and an insertion is one substitution.
                 levenshtein += max(insertions, deletions)
@@ -1215,15 +1216,15 @@
         Args:
           diffs: Array of diff tuples.
 
         Returns:
           Delta text.
         """
         text = []
-        for (op, data) in diffs:
+        for op, data in diffs:
             if op == self.DIFF_INSERT:
                 # High ascii will raise UnicodeDecodeError.  Use Unicode instead.
                 data = data.encode("utf-8")
                 text.append("+" + urllib.parse.quote(data, "!~*'();/?:@&=+$,# "))
             elif op == self.DIFF_DELETE:
                 text.append("-%d" % len(data))
             elif op == self.DIFF_EQUAL:
@@ -1703,15 +1704,15 @@
                         > self.Patch_DeleteThreshold
                     ):
                         # The end points match, but the content is unacceptably bad.
                         results[-1] = False
                     else:
                         self.diff_cleanupSemanticLossless(diffs)
                         index1 = 0
-                        for (op, data) in patch.diffs:
+                        for op, data in patch.diffs:
                             if op != self.DIFF_EQUAL:
                                 index2 = self.diff_xIndex(diffs, index1)
                             if op == self.DIFF_INSERT:  # Insertion
                                 text = (
                                     text[: start_loc + index2]
                                     + data
                                     + text[start_loc + index2 :]
@@ -2002,15 +2003,15 @@
             coords2 = str(self.start2) + ",0"
         elif self.length2 == 1:
             coords2 = str(self.start2 + 1)
         else:
             coords2 = str(self.start2 + 1) + "," + str(self.length2)
         text = ["@@ -", coords1, " +", coords2, " @@\n"]
         # Escape the body of the patch with %xx notation.
-        for (op, data) in self.diffs:
+        for op, data in self.diffs:
             if op == diff_match_patch.DIFF_INSERT:
                 text.append("+")
             elif op == diff_match_patch.DIFF_DELETE:
                 text.append("-")
             elif op == diff_match_patch.DIFF_EQUAL:
                 text.append(" ")
             # High ascii will raise UnicodeDecodeError.  Use Unicode instead.
```

### Comparing `xmldiff-2.6b1/xmldiff/formatting.py` & `xmldiff-2.7.0/xmldiff/formatting.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 DIFF_NS = "http://namespaces.shoobx.com/diff"
 DIFF_PREFIX = "diff"
 
 INSERT_NAME = "{%s}insert" % DIFF_NS
 DELETE_NAME = "{%s}delete" % DIFF_NS
+REPLACE_NAME = "{%s}replace" % DIFF_NS
 RENAME_NAME = "{%s}rename" % DIFF_NS
 
 # Flags for whitespace handling in the text aware formatters:
 WS_BOTH = 3  # Normalize ignorable whitespace and text whitespace
 WS_TEXT = 2  # Normalize whitespace only inside text tags
 WS_TAGS = 1  # Delete ignorable whitespace (between tags)
 WS_NONE = 0  # Preserve all whitespace
@@ -100,17 +101,22 @@
         insert_close = self.get_placeholder(insert_elem, T_CLOSE, None)
         insert_open = self.get_placeholder(insert_elem, T_OPEN, insert_close)
 
         delete_elem = etree.Element(DELETE_NAME)
         delete_close = self.get_placeholder(delete_elem, T_CLOSE, None)
         delete_open = self.get_placeholder(delete_elem, T_OPEN, delete_close)
 
+        replace_elem = etree.Element(REPLACE_NAME)
+        replace_close = self.get_placeholder(replace_elem, T_CLOSE, None)
+        replace_open = self.get_placeholder(replace_elem, T_OPEN, replace_close)
+
         self.diff_tags = {
             "insert": (insert_open, insert_close),
             "delete": (delete_open, delete_close),
+            "replace": (replace_open, replace_close),
         }
 
     def get_placeholder(self, element, ttype, close_ph):
         tag = etree.tounicode(element)
         ph = self.tag2placeholder.get((tag, ttype, close_ph))
         if ph is not None:
             return ph
@@ -224,34 +230,44 @@
                         self.undo_element(child)
                         parent.insert(index, child)
                         index += 1
 
     def undo_tree(self, tree):
         self.undo_element(tree)
 
-    def mark_diff(self, ph, action):
+    def mark_diff(self, ph, action, attributes=None):
         entry = self.placeholder2tag[ph]
         if entry.ttype == T_CLOSE:
             # Close tag, nothing to mark
             return ph
 
         # Mark the tag as having a diff-action. We do need to
         # make a copy of it and get a new placeholder:
         elem = entry.element
         elem = deepcopy(elem)
         if self.is_formatting(elem):
             # Formatting element, add a diff attribute
             action += "-formatting"
         elem.attrib[f"{{{DIFF_NS}}}{action}"] = ""
+        if attributes is not None:
+            for attrib, value in attributes.items():
+                elem.attrib[attrib] = value
 
         # And make a new placeholder for this new entry:
         return self.get_placeholder(elem, entry.ttype, entry.close_ph)
 
-    def wrap_diff(self, text, action):
+    def wrap_diff(self, text, action, attributes=None):
         open_ph, close_ph = self.diff_tags[action]
+        if attributes is not None and len(attributes) > 0:
+            entry = self.placeholder2tag[open_ph]
+            elem = entry.element
+            elem = deepcopy(elem)
+            for attrib, value in attributes.items():
+                elem.attrib[attrib] = value
+            open_ph = self.get_placeholder(elem, entry.ttype, entry.close_ph)
         return open_ph + text + close_ph
 
 
 class XMLFormatter(BaseFormatter):
     """A formatter that also replaces formatting tags with unicode characters
 
     The idea of this differ is to replace structured content (in this case XML
@@ -291,24 +307,33 @@
     ``finalize(tree)`` method to convert all the placeholders back into
     structural content before formatting.
 
     The ``normalize`` parameter decides how to normalize whitespace.
     WS_TEXT normalizes only inside text_tags, WS_TAGS will remove ignorable
     whitespace between tags, WS_BOTH do both, and WS_NONE will preserve
     all whitespace.
+
+    The ``use_replace`` flag decides, if a replace tag (with the old text
+    as an attribute) should be used instead of one delete and one insert tag.
     """
 
     def __init__(
-        self, normalize=WS_NONE, pretty_print=True, text_tags=(), formatting_tags=()
+        self,
+        normalize=WS_NONE,
+        pretty_print=True,
+        text_tags=(),
+        formatting_tags=(),
+        use_replace=False,
     ):
         # Mapping from placeholders -> structural content and vice versa.
         self.normalize = normalize
         self.pretty_print = pretty_print
         self.text_tags = text_tags
         self.formatting_tags = formatting_tags
+        self.use_replace = use_replace
         self.placeholderer = PlaceholderMaker(
             text_tags=text_tags, formatting_tags=formatting_tags
         )
 
     def prepare(self, left_tree, right_tree):
         """prepare() is run on the trees before diffing
 
@@ -331,22 +356,23 @@
         # and also because we don't want to modify the original tree.
         result = deepcopy(orig_tree)
         if isinstance(result, etree._ElementTree):
             root = result.getroot()
         else:
             root = result
 
+        self._nsmap = [(DIFF_PREFIX, DIFF_NS)]
         etree.register_namespace(DIFF_PREFIX, DIFF_NS)
 
         for action in diff:
             self.handle_action(action, root)
 
         self.finalize(root)
 
-        etree.cleanup_namespaces(result, top_nsmap={DIFF_PREFIX: DIFF_NS})
+        etree.cleanup_namespaces(result, top_nsmap=dict(self._nsmap))
         return self.render(result)
 
     def render(self, result):
         return etree.tounicode(result, pretty_print=self.pretty_print)
 
     def handle_action(self, action, result):
         action_type = type(action)
@@ -365,14 +391,19 @@
             parent.remove(element)
 
     def _xpath(self, node, xpath):
         # This method finds an element with xpath and makes sure that
         # one and exactly one element is found. This is to protect against
         # formatting a diff on the wrong tree, or against using ambiguous
         # edit script xpaths.
+
+        # First, make a namespace map that uses the left tree's URI's:
+        nsmap = dict(self._nsmap)
+        nsmap.update(node.nsmap)
+
         if xpath[0] == "/":
             root = True
             xpath = xpath[1:]
         else:
             root = False
 
         if "/" in xpath:
@@ -389,19 +420,20 @@
             index = 0
             multiple = True
 
         if root:
             path = "/" + path
 
         matches = []
-        for match in node.xpath(path, namespaces=node.nsmap):
+        if None in nsmap:
+            del nsmap[None]
+        for match in node.xpath(path, namespaces=nsmap):
             # Skip nodes that have been deleted
             if DELETE_NAME not in match.attrib:
                 matches.append(match)
-
         if index >= len(matches):
             raise ValueError(
                 "xpath {}[{}] not found at {}.".format(
                     path, index + 1, utils.getpath(node)
                 )
             )
         if len(matches) > 1 and multiple:
@@ -559,52 +591,92 @@
                     # stack_op > op, so I removed the handling, and
                     # put in an assert
                     if stack_entry is not None:
                         assert stack_op <= op
                         new_diff.append((op, seg))
         return new_diff
 
+    def _join_delete_insert(self, diffs):
+        new_diffs = []
+        skip_next = False
+        for i in range(len(diffs) - 1):
+            if skip_next:
+                skip_next = False
+                continue
+            op, text = diffs[i]
+            next_op, next_text = diffs[i + 1]
+            # insert, then delete
+            if (
+                op == diff_match_patch.DIFF_INSERT
+                and next_op == diff_match_patch.DIFF_DELETE
+            ):
+                new_diffs.append((diff_match_patch.DIFF_REPLACE, text, next_text))
+                skip_next = True  # also skip upcoming delete
+            # delete, then insert
+            elif (
+                next_op == diff_match_patch.DIFF_INSERT
+                and op == diff_match_patch.DIFF_DELETE
+            ):
+                new_diffs.append((diff_match_patch.DIFF_REPLACE, next_text, text))
+                skip_next = True  # also skip upcoming insert
+            else:
+                new_diffs.append(diffs[i])
+        # append last diff, if it shouldn't be skipped
+        if not skip_next:
+            new_diffs.append(diffs[-1])
+        return new_diffs
+
     def _make_diff_tags(self, left_value, right_value, node, target=None):
         if bool(self.normalize & WS_TEXT):
             left_value = utils.cleanup_whitespace(left_value or "").strip()
             right_value = utils.cleanup_whitespace(right_value or "").strip()
 
         text_diff = diff_match_patch()
         diff = text_diff.diff_main(left_value or "", right_value or "")
         text_diff.diff_cleanupSemantic(diff)
-
         diff = self._realign_placeholders(diff)
 
+        if self.use_replace:
+            diff = self._join_delete_insert(diff)
         cur_child = None
         if target is None:
             target = node
         else:
             cur_child = node
 
-        for op, text in diff:
-            if op == 0:
+        for d in diff:
+            op = d[0]
+            text = d[1]
+            if op == diff_match_patch.DIFF_REPLACE:
+                old_text = d[2]
+
+            if op == diff_match_patch.DIFF_EQUAL:
                 if cur_child is None:
                     node.text = (node.text or "") + text
                 else:
                     cur_child.tail = (cur_child.tail or "") + text
                 continue
 
-            if op == -1:
+            attributes = {}
+            if op == diff_match_patch.DIFF_DELETE:
                 action = "delete"
-            elif op == 1:
+            elif op == diff_match_patch.DIFF_INSERT:
                 action = "insert"
+            elif op == diff_match_patch.DIFF_REPLACE:
+                action = "replace"
+                attributes["old-text"] = old_text
 
             if self.placeholderer.is_placeholder(text):
-                ph = self.placeholderer.mark_diff(text, action)
+                ph = self.placeholderer.mark_diff(text, action, attributes)
 
                 if cur_child is None:
                     node.text = (node.text or "") + ph
 
             else:
-                new_text = self.placeholderer.wrap_diff(text, action)
+                new_text = self.placeholderer.wrap_diff(text, action, attributes)
 
                 if cur_child is None:
                     node.text = (node.text or "") + new_text
                 else:
                     cur_child.tail = (cur_child.tail or "") + new_text
 
     def _handle_UpdateTextIn(self, action, tree):
@@ -628,14 +700,22 @@
         right_value = action.text
         node.tail = None
 
         self._make_diff_tags(left_value, right_value, node, node.getparent())
 
         return node
 
+    def _handle_InsertNamespace(self, action, tree):
+        # There is no way to mark this so it's visible, so we'll just update the tree
+        self._nsmap.append((action.prefix, action.uri))
+
+    def _handle_DeleteNamespace(self, action, tree):
+        # This will be handled by the namespace cleanup
+        pass
+
     # There is no InsertComment handler, as this formatter removes all comments
 
 
 class DiffFormatter(BaseFormatter):
     def __init__(self, normalize=WS_TAGS, pretty_print=False):
         self.normalize = normalize
         # No pretty print support, nothing to be pretty about
@@ -698,14 +778,27 @@
         return (
             "insert-comment",
             action.target,
             str(action.position),
             json.dumps(action.text),
         )
 
+    def _handle_InsertNamespace(self, action):
+        return (
+            "insert-namespace",
+            action.prefix,
+            action.uri,
+        )
+
+    def _handle_DeleteNamespace(self, action):
+        return (
+            "delete-namespace",
+            action.prefix,
+        )
+
 
 class XmlDiffFormatter(BaseFormatter):
     """A formatter for an output trying to be xmldiff 0.6 compatible"""
 
     def __init__(self, normalize=WS_TAGS, pretty_print=False):
         self.normalize = normalize
         # No pretty print support, nothing to be pretty about
@@ -788,8 +881,14 @@
     def _handle_UpdateTextAfter(self, action, orig_tree):
         yield "update", action.node + "/text()[2]", json.dumps(action.text)
 
     def _handle_RenameNode(self, action, orig_tree):
         yield "rename", action.node, action.tag
 
     def _handle_InsertComment(self, action, orig_tree):
-        yield ("insert-comment", action.target, str(action.position), action.text)
+        yield "insert-comment", action.target, str(action.position), action.text
+
+    def _handle_InsertNamespace(self, action, orig_tree):
+        yield "insert-namespace", action.prefix, action.uri
+
+    def _handle_DeleteNamespace(self, action, orig_tree):
+        yield "delete-namespace", action.prefix
```

### Comparing `xmldiff-2.6b1/xmldiff/main.py` & `xmldiff-2.7.0/xmldiff/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """All major API points and command-line tools"""
-import pkg_resources
+from importlib import metadata
 
-from argparse import ArgumentParser
+from argparse import ArgumentParser, ArgumentTypeError
 from lxml import etree
 from xmldiff import diff, formatting, patch
 
-__version__ = pkg_resources.require("xmldiff")[0].version
+__version__ = metadata.version("xmldiff")
 
 FORMATTERS = {
     "diff": formatting.DiffFormatter,
     "xml": formatting.XMLFormatter,
     "old": formatting.XmlDiffFormatter,
 }
 
@@ -49,14 +49,27 @@
 def diff_files(left, right, diff_options=None, formatter=None):
     """Takes two filenames or streams, and diffs the XML in those files"""
     return _diff(
         etree.parse, left, right, diff_options=diff_options, formatter=formatter
     )
 
 
+def validate_F(arg):
+    """Type function for argparse - a float within some predefined bounds"""
+    try:
+        F = float(arg)
+    except ValueError:
+        raise ArgumentTypeError("Must be a floating point number")
+    if F <= 0:
+        raise ArgumentTypeError("F can not be zero or lower")
+    if F > 1:
+        raise ArgumentTypeError("F can not be above 1")
+    return F
+
+
 def make_diff_parser():
     parser = ArgumentParser(
         description="Create a diff for two XML files.", add_help=False
     )
     parser.add_argument("file1", type=str, help="The first input file.")
     parser.add_argument("file2", type=str, help="The second input file.")
     parser.add_argument(
@@ -91,15 +104,15 @@
         "-p",
         "--pretty-print",
         action="store_true",
         help="Try to make XML output more readable.",
     )
     parser.add_argument(
         "-F",
-        type=float,
+        type=validate_F,
         help="A value between 0 and 1 that determines how "
         "similar nodes must be to match.",
     )
     parser.add_argument(
         "--unique-attributes",
         type=str,
         nargs="?",
```

### Comparing `xmldiff-2.6b1/xmldiff/patch.py` & `xmldiff-2.7.0/xmldiff/patch.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,81 +2,97 @@
 from csv import reader
 from json import loads
 from lxml import etree
 from xmldiff import actions
 
 
 class Patcher:
+    @property
+    def nsmap(self):
+        return getattr(self, "_nsmap", {})
+
     def patch(self, actions, tree):
         if isinstance(tree, etree._ElementTree):
             tree = tree.getroot()
 
+        # Save the namespace:
+        self._nsmap = tree.nsmap
+        if None in self._nsmap:
+            del self._nsmap[None]
+
         # Copy the tree so we don't modify the original
         result = deepcopy(tree)
 
         for action in actions:
             self.handle_action(action, result)
 
         return result
 
     def handle_action(self, action, tree):
         action_type = type(action)
         method = getattr(self, "_handle_" + action_type.__name__)
         method(action, tree)
 
     def _handle_DeleteNode(self, action, tree):
-        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
         node.getparent().remove(node)
 
     def _handle_InsertNode(self, action, tree):
-        target = tree.xpath(action.target, namespaces=tree.nsmap)[0]
+        target = tree.xpath(action.target, namespaces=self.nsmap)[0]
         node = target.makeelement(action.tag)
         target.insert(action.position, node)
 
     def _handle_RenameNode(self, action, tree):
-        tree.xpath(action.node, namespaces=tree.nsmap)[0].tag = action.tag
+        tree.xpath(action.node, namespaces=self.nsmap)[0].tag = action.tag
 
     def _handle_MoveNode(self, action, tree):
-        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
         node.getparent().remove(node)
         target = tree.xpath(action.target)[0]
         target.insert(action.position, node)
 
     def _handle_UpdateTextIn(self, action, tree):
-        tree.xpath(action.node, namespaces=tree.nsmap)[0].text = action.text
+        tree.xpath(action.node, namespaces=self.nsmap)[0].text = action.text
 
     def _handle_UpdateTextAfter(self, action, tree):
-        tree.xpath(action.node, namespaces=tree.nsmap)[0].tail = action.text
+        tree.xpath(action.node, namespaces=self.nsmap)[0].tail = action.text
 
     def _handle_UpdateAttrib(self, action, tree):
-        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
         # This should not be used to insert new attributes.
         assert action.name in node.attrib
         node.attrib[action.name] = action.value
 
     def _handle_DeleteAttrib(self, action, tree):
-        del tree.xpath(action.node, namespaces=tree.nsmap)[0].attrib[action.name]
+        del tree.xpath(action.node, namespaces=self.nsmap)[0].attrib[action.name]
 
     def _handle_InsertAttrib(self, action, tree):
-        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
         # This should not be used to update existing attributes.
         assert action.name not in node.attrib
         node.attrib[action.name] = action.value
 
     def _handle_RenameAttrib(self, action, tree):
-        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
         assert action.oldname in node.attrib
         assert action.newname not in node.attrib
         node.attrib[action.newname] = node.attrib[action.oldname]
         del node.attrib[action.oldname]
 
     def _handle_InsertComment(self, action, tree):
         target = tree.xpath(action.target)[0]
         target.insert(action.position, etree.Comment(action.text))
 
+    def _handle_InsertNamespace(self, action, tree):
+        self.nsmap[action.prefix] = action.uri
+
+    def _handle_DeleteNamespace(self, action, tree):
+        # Nothing needs to be done, it will be handled by cleanup
+        pass
+
 
 class DiffParser:
     """Makes a text diff into a list of actions"""
 
     def parse(self, diff):
         incomplete = ""
 
@@ -138,7 +154,13 @@
         return actions.InsertAttrib(node, name, loads(value))
 
     def _handle_rename_attribute(self, node, oldname, newname):
         return actions.RenameAttrib(node, oldname, newname)
 
     def _handle_insert_comment(self, target, position, text):
         return actions.InsertComment(target, int(position), loads(text))
+
+    def _handle_insert_namespace(self, prefix, uri):
+        return actions.InsertNamespace(prefix, uri)
+
+    def _handle_delete_namespace(self, prefix):
+        return actions.DeleteNamespace(prefix)
```

### Comparing `xmldiff-2.6b1/xmldiff/utils.py` & `xmldiff-2.7.0/xmldiff/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import re
 
 from operator import eq
 
+# This namespace is reserved for lxml internal use, which only
+# means we get an error if we try registering it:
+RESERVED_NS = re.compile(r"ns\d+", flags=re.ASCII)
+
 
 def post_order_traverse(node):
     for child in node.getchildren():
         # PY3: Man, I want yield from!
         yield from post_order_traverse(child)
     yield node
 
@@ -29,15 +33,14 @@
 
 # LCS from Myers: An O(ND) Difference Algorithm and Its Variations. This
 # implementation uses Chris Marchetti's technique of only keeping the history
 # per dpath, and not per node, so it should be vastly less memory intensive.
 # It also skips any items that are equal in the beginning and end, speeding
 # up the search, and using even less memory.
 def longest_common_subsequence(left_sequence, right_sequence, eqfn=eq):
-
     start = 0
     lend = lslen = len(left_sequence)
     rend = rslen = len(right_sequence)
 
     # Trim off the matching items at the beginning
     while (
         start < lend
```

### Comparing `xmldiff-2.6b1/xmldiff.egg-info/PKG-INFO` & `xmldiff-2.7.0/xmldiff.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmldiff
-Version: 2.6b1
+Version: 2.7.0
 Summary: Creates diffs of XML files
 Home-page: https://github.com/Shoobx/xmldiff
 Author: Lennart Regebro
 Author-email: lregebro@shoobx.com
 License: MIT
 Project-URL: Source Code, https://github.com/Shoobx/xmldiff
 Keywords: xml,html,diff
@@ -12,24 +12,30 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Provides-Extra: devenv
+Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: lxml>=3.1.0
+Provides-Extra: devenv
+Requires-Dist: black; extra == "devenv"
+Requires-Dist: coverage; extra == "devenv"
+Requires-Dist: flake8; extra == "devenv"
+Requires-Dist: zest.releaser[recommended]; extra == "devenv"
 
 xmldiff
 ========
 
 .. image:: https://travis-ci.org/Shoobx/xmldiff.svg?branch=master
   :target: https://travis-ci.org/Shoobx/xmldiff
 
@@ -113,23 +119,74 @@
 
  * Albertas Agejevas, alga@shoobx.com
 
  * Greg Kempe, greg@laws.africa
 
  * Filip Demski, glamhoth@protonmail.com
 
-The diff algorithm is based on "`Change Detection in Hierarchically Structured Information <http://ilpubs.stanford.edu/115/1/1995-46.pdf>`_",
+ * Jacek Chałupka, krunchfrompoland@gmail.com
+
+ * Thomas Pfitzinger, thpfitzinger@web.de
+
+The diff algorithm is based on
+"`Change Detection in Hierarchically Structured Information <http://infolab.stanford.edu/c3/papers/html/tdiff3-8/tdiff3-8.html>`_",
 and the text diff is using Google's ``diff_match_patch`` algorithm.
 
 Changes
 =======
 
+2.7.0 (2024-05-13)
+------------------
+
+- Changed the comparison to make accurate and standard more accurate,
+  although fast gets less accurate as a result.
+
+- Changed usage of deprecated `pkg_resources` package to `importlib.metadata`.
+
+- A `use_replace` flag was added to the `XMLFormatter` by Thomas Pfitzinger.
+  It changes text replacement from delete and insert tags to a replace tag.
+  It's not currently accessaible thtough the CLI, the question is it is better
+  to add a new formatter name, or an option to pass in formatter flags.
+
+  - Added option to XMLFormatter to use replace tags
+  - in _make_diff_tags after diffing, neighboring delete/insert diffs are joined to a replace tag
+  - the deleted text is added as an attribute ("old-text")
+  - the inserted text is the element's text
+
+2.6.3 (2023-05-21)
+------------------
+
+- And there was a namespace bug in the patch as well. #118
+
+
+2.6.2 (2023-05-21)
+------------------
+
+- Solved an error in the xmlformatter when using default namespaces. #89
+
+
+2.6.1 (2023-04-05)
+------------------
+
+- #108: Fixed an error that happens if using namespaces like ns0 or ns1.
+
+
+2.6 (2023-04-03)
+----------------
+
+- Added `InsertNamespace` and `DeleteNamespace` actions for better handling
+  of changing namespaces. Should improve any "Unknown namespace prefix"
+  errors. Changing the URI of a a namespace prefix is not supported, and will
+  raise an error.
+
 2.6b1 (2023-01-12)
 ------------------
 
+- Used geometric mean for the node_ratio, for better handling of simple nodes.
+
 - Added an experimental --best-match method that is slower, but generate
   smaller diffs when you have many nodes that are similar.
 
 - The -F argument now also affects the --fast-match stage.
 
 
 2.5 (2023-01-11)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xmldiff-2.6b1/xmldiff.egg-info/SOURCES.txt` & `xmldiff-2.7.0/xmldiff.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 .coveragerc
 .coveralls.yml
 .travis.yml
 CHANGES.rst
+CHANGES.txt
 LICENSE.txt
 MANIFEST.in
 Makefile
 README.rst
-README.txt
 setup.cfg
 setup.py
 ./xmldiff/__init__.py
 ./xmldiff/actions.py
 ./xmldiff/diff.py
 ./xmldiff/diff_match_patch.py
 ./xmldiff/formatting.py
@@ -46,14 +46,17 @@
 tests/test_data/example.expected.html
 tests/test_data/example.left.html
 tests/test_data/example.right.html
 tests/test_data/insert-node.diff
 tests/test_data/insert-node.expected.html
 tests/test_data/insert-node.left.html
 tests/test_data/insert-node.right.html
+tests/test_data/namespace.expected.xml
+tests/test_data/namespace.left.xml
+tests/test_data/namespace.right.xml
 tests/test_data/rmldoc.expected.xml
 tests/test_data/rmldoc.left.xml
 tests/test_data/rmldoc.right.xml
 tests/test_data/sbt_template.expected.xml
 tests/test_data/sbt_template.left.xml
 tests/test_data/sbt_template.right.xml
 xmldiff.egg-info/PKG-INFO
```

