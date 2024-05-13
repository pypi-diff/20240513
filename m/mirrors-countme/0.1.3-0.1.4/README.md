# Comparing `tmp/mirrors_countme-0.1.3.tar.gz` & `tmp/mirrors_countme-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirrors_countme-0.1.3.tar", max compression
+gzip compressed data, was "mirrors_countme-0.1.4.tar", max compression
```

## Comparing `mirrors_countme-0.1.3.tar` & `mirrors_countme-0.1.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0    34916 2024-05-06 14:25:25.791218 mirrors_countme-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     9890 2024-05-06 14:25:25.791218 mirrors_countme-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-06 14:25:25.791218 mirrors_countme-0.1.3/mirrors_countme/__init__.py
--rw-r--r--   0        0        0      709 2024-05-06 14:25:25.791218 mirrors_countme-0.1.3/mirrors_countme/constants.py
--rw-r--r--   0        0        0     2937 2024-05-06 14:25:25.791218 mirrors_countme-0.1.3/mirrors_countme/matchers.py
--rw-r--r--   0        0        0     2246 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/output_items.py
--rw-r--r--   0        0        0     1826 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/parse.py
--rw-r--r--   0        0        0     5683 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/progress.py
--rw-r--r--   0        0        0     2318 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/readers.py
--rw-r--r--   0        0        0     6773 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/regex.py
--rw-r--r--   0        0        0        0 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/scripts/__init__.py
--rwxr-xr-x   0        0        0     3677 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/scripts/countme_delete_totals.py
--rwxr-xr-x   0        0        0     4011 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/scripts/countme_parse_access_log.py
--rwxr-xr-x   0        0        0     1521 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/scripts/countme_totals.py
--rwxr-xr-x   0        0        0     6985 2024-05-06 14:25:25.792218 mirrors_countme-0.1.3/mirrors_countme/scripts/countme_trim_raw.py
--rw-r--r--   0        0        0    11868 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/mirrors_countme/totals.py
--rw-r--r--   0        0        0     4467 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/mirrors_countme/util.py
--rw-r--r--   0        0        0      147 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/mirrors_countme/version.py
--rw-r--r--   0        0        0     5876 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/mirrors_countme/writers.py
--rw-r--r--   0        0        0     1900 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0      960 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/scripts/countme-csv2sqlite.sh
--rwxr-xr-x   0        0        0     1642 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/scripts/countme-fix-dbs.sh
--rwxr-xr-x   0        0        0     3885 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/scripts/countme-regenerate-dbs.sh
--rwxr-xr-x   0        0        0      620 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/scripts/countme-sqlite2csv.sh
--rwxr-xr-x   0        0        0     5778 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/scripts/countme-update-rawdb.sh
--rwxr-xr-x   0        0        0     2170 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/scripts/countme-update-totals.sh
--rwxr-xr-x   0        0        0     2560 2024-05-06 14:25:25.793218 mirrors_countme-0.1.3/scripts/countme-weekly-totals-ui.sh
--rwxr-xr-x   0        0        0     2059 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/scripts/rezip
--rwxr-xr-x   0        0        0     2157 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/scripts/split-totals-db.sh
--rw-r--r--   0        0        0        0 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      192 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/common.py
--rw-r--r--   0        0        0      563 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/scripts/__init__.py
--rw-r--r--   0        0        0     6407 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/scripts/test_countme_delete_totals.py
--rw-r--r--   0        0        0     4834 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/scripts/test_countme_parse_access_log.py
--rw-r--r--   0        0        0     1860 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/scripts/test_countme_totals.py
--rw-r--r--   0        0        0    11698 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/scripts/test_countme_trim_raw.py
--rw-r--r--   0        0        0     6050 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/test_integrate.py
--rw-r--r--   0        0        0     3655 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/test_matchers.py
--rw-r--r--   0        0        0     1169 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/test_output_items.py
--rw-r--r--   0        0        0     4246 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/test_parse.py
--rw-r--r--   0        0        0    12497 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/test_progress.py
--rw-r--r--   0        0        0     3795 2024-05-06 14:25:25.794218 mirrors_countme-0.1.3/tests/test_readers.py
--rw-r--r--   0        0        0     6911 2024-05-06 14:25:25.795218 mirrors_countme-0.1.3/tests/test_regex.py
--rw-r--r--   0        0        0    15472 2024-05-06 14:25:25.795218 mirrors_countme-0.1.3/tests/test_totals.py
--rw-r--r--   0        0        0     4168 2024-05-06 14:25:25.795218 mirrors_countme-0.1.3/tests/test_util.py
--rw-r--r--   0        0        0      336 2024-05-06 14:25:25.795218 mirrors_countme-0.1.3/tests/test_version.py
--rw-r--r--   0        0        0    10593 2024-05-06 14:25:25.795218 mirrors_countme-0.1.3/tests/test_writers.py
--rw-r--r--   0        0        0    11314 1970-01-01 00:00:00.000000 mirrors_countme-0.1.3/setup.py
--rw-r--r--   0        0        0    10567 1970-01-01 00:00:00.000000 mirrors_countme-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34916 2024-05-13 15:39:28.476907 mirrors_countme-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0     9890 2024-05-13 15:39:28.477907 mirrors_countme-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 15:39:28.477907 mirrors_countme-0.1.4/mirrors_countme/__init__.py
+-rw-r--r--   0        0        0      709 2024-05-13 15:39:28.477907 mirrors_countme-0.1.4/mirrors_countme/constants.py
+-rw-r--r--   0        0        0     2937 2024-05-13 15:39:28.477907 mirrors_countme-0.1.4/mirrors_countme/matchers.py
+-rw-r--r--   0        0        0     2246 2024-05-13 15:39:28.477907 mirrors_countme-0.1.4/mirrors_countme/output_items.py
+-rw-r--r--   0        0        0     1826 2024-05-13 15:39:28.477907 mirrors_countme-0.1.4/mirrors_countme/parse.py
+-rw-r--r--   0        0        0     5683 2024-05-13 15:39:28.478907 mirrors_countme-0.1.4/mirrors_countme/progress.py
+-rw-r--r--   0        0        0     2318 2024-05-13 15:39:28.478907 mirrors_countme-0.1.4/mirrors_countme/readers.py
+-rw-r--r--   0        0        0     6773 2024-05-13 15:39:28.478907 mirrors_countme-0.1.4/mirrors_countme/regex.py
+-rw-r--r--   0        0        0        0 2024-05-13 15:39:28.478907 mirrors_countme-0.1.4/mirrors_countme/scripts/__init__.py
+-rwxr-xr-x   0        0        0     3677 2024-05-13 15:39:28.479907 mirrors_countme-0.1.4/mirrors_countme/scripts/countme_delete_totals.py
+-rwxr-xr-x   0        0        0     4011 2024-05-13 15:39:28.479907 mirrors_countme-0.1.4/mirrors_countme/scripts/countme_parse_access_log.py
+-rwxr-xr-x   0        0        0     1521 2024-05-13 15:39:28.479907 mirrors_countme-0.1.4/mirrors_countme/scripts/countme_totals.py
+-rwxr-xr-x   0        0        0     6985 2024-05-13 15:39:28.479907 mirrors_countme-0.1.4/mirrors_countme/scripts/countme_trim_raw.py
+-rw-r--r--   0        0        0    11868 2024-05-13 15:39:28.479907 mirrors_countme-0.1.4/mirrors_countme/totals.py
+-rw-r--r--   0        0        0     4467 2024-05-13 15:39:28.479907 mirrors_countme-0.1.4/mirrors_countme/util.py
+-rw-r--r--   0        0        0      147 2024-05-13 15:39:28.479907 mirrors_countme-0.1.4/mirrors_countme/version.py
+-rw-r--r--   0        0        0     5876 2024-05-13 15:39:28.479907 mirrors_countme-0.1.4/mirrors_countme/writers.py
+-rw-r--r--   0        0        0     1908 2024-05-13 15:39:28.480907 mirrors_countme-0.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0      960 2024-05-13 15:39:28.480907 mirrors_countme-0.1.4/scripts/countme-csv2sqlite.sh
+-rwxr-xr-x   0        0        0     1642 2024-05-13 15:39:28.480907 mirrors_countme-0.1.4/scripts/countme-fix-dbs.sh
+-rwxr-xr-x   0        0        0     3885 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/scripts/countme-regenerate-dbs.sh
+-rwxr-xr-x   0        0        0     2059 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/scripts/countme-rezip
+-rwxr-xr-x   0        0        0     2157 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/scripts/countme-split-totals-db.sh
+-rwxr-xr-x   0        0        0      620 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/scripts/countme-sqlite2csv.sh
+-rwxr-xr-x   0        0        0     5778 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/scripts/countme-update-rawdb.sh
+-rwxr-xr-x   0        0        0     2170 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/scripts/countme-update-totals.sh
+-rwxr-xr-x   0        0        0     2560 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/scripts/countme-weekly-totals-ui.sh
+-rw-r--r--   0        0        0        0 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/tests/common.py
+-rw-r--r--   0        0        0      563 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/tests/scripts/__init__.py
+-rw-r--r--   0        0        0     6407 2024-05-13 15:39:28.481907 mirrors_countme-0.1.4/tests/scripts/test_countme_delete_totals.py
+-rw-r--r--   0        0        0     4834 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/scripts/test_countme_parse_access_log.py
+-rw-r--r--   0        0        0     1860 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/scripts/test_countme_totals.py
+-rw-r--r--   0        0        0    11698 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/scripts/test_countme_trim_raw.py
+-rw-r--r--   0        0        0     6050 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/test_integrate.py
+-rw-r--r--   0        0        0     3655 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/test_matchers.py
+-rw-r--r--   0        0        0     1169 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/test_output_items.py
+-rw-r--r--   0        0        0     4246 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/test_parse.py
+-rw-r--r--   0        0        0    12497 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/test_progress.py
+-rw-r--r--   0        0        0     3795 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/test_readers.py
+-rw-r--r--   0        0        0     6911 2024-05-13 15:39:28.482907 mirrors_countme-0.1.4/tests/test_regex.py
+-rw-r--r--   0        0        0    15472 2024-05-13 15:39:28.483907 mirrors_countme-0.1.4/tests/test_totals.py
+-rw-r--r--   0        0        0     4168 2024-05-13 15:39:28.483907 mirrors_countme-0.1.4/tests/test_util.py
+-rw-r--r--   0        0        0      336 2024-05-13 15:39:28.483907 mirrors_countme-0.1.4/tests/test_version.py
+-rw-r--r--   0        0        0    10593 2024-05-13 15:39:28.483907 mirrors_countme-0.1.4/tests/test_writers.py
+-rw-r--r--   0        0        0    11314 1970-01-01 00:00:00.000000 mirrors_countme-0.1.4/setup.py
+-rw-r--r--   0        0        0    10567 1970-01-01 00:00:00.000000 mirrors_countme-0.1.4/PKG-INFO
```

### Comparing `mirrors_countme-0.1.3/LICENSE.md` & `mirrors_countme-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/README.md` & `mirrors_countme-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/constants.py` & `mirrors_countme-0.1.4/mirrors_countme/constants.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/matchers.py` & `mirrors_countme-0.1.4/mirrors_countme/matchers.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/output_items.py` & `mirrors_countme-0.1.4/mirrors_countme/output_items.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/parse.py` & `mirrors_countme-0.1.4/mirrors_countme/parse.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/progress.py` & `mirrors_countme-0.1.4/mirrors_countme/progress.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/readers.py` & `mirrors_countme-0.1.4/mirrors_countme/readers.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/regex.py` & `mirrors_countme-0.1.4/mirrors_countme/regex.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/scripts/countme_delete_totals.py` & `mirrors_countme-0.1.4/mirrors_countme/scripts/countme_delete_totals.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/scripts/countme_parse_access_log.py` & `mirrors_countme-0.1.4/mirrors_countme/scripts/countme_parse_access_log.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/scripts/countme_totals.py` & `mirrors_countme-0.1.4/mirrors_countme/scripts/countme_totals.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/scripts/countme_trim_raw.py` & `mirrors_countme-0.1.4/mirrors_countme/scripts/countme_trim_raw.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/totals.py` & `mirrors_countme-0.1.4/mirrors_countme/totals.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/util.py` & `mirrors_countme-0.1.4/mirrors_countme/util.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/mirrors_countme/writers.py` & `mirrors_countme-0.1.4/mirrors_countme/writers.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/pyproject.toml` & `mirrors_countme-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mirrors-countme"
-version = "0.1.3"
+version = "0.1.4"
 description = "Parse access logs and count hosts for DNF mirrors"
 authors = [
     "Will Woods",
     "Stephen Smoogen <smooge@smoogespace.com>",
     "Adam Saleh <asaleh@redhat.com>",
     "Patrik Polakovič <patrik@alphamail.org>",
     "Nils Philippsen <nils@redhat.com>",
@@ -19,15 +19,15 @@
 readme = "README.md"
 repository = "http://github.com/fedora-infra/mirrors-countme"
 packages = [
     { include = "mirrors_countme" },
 ]
 include = [
     { path = "scripts/*.sh", format = "sdist" },
-    { path = "scripts/rezip", format = "sdist" },
+    { path = "scripts/countme-rezip", format = "sdist" },
     { path = "tests", format = "sdist" },
 ]
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
```

### Comparing `mirrors_countme-0.1.3/scripts/countme-csv2sqlite.sh` & `mirrors_countme-0.1.4/scripts/countme-csv2sqlite.sh`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/scripts/countme-fix-dbs.sh` & `mirrors_countme-0.1.4/scripts/countme-fix-dbs.sh`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/scripts/countme-regenerate-dbs.sh` & `mirrors_countme-0.1.4/scripts/countme-regenerate-dbs.sh`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/scripts/countme-sqlite2csv.sh` & `mirrors_countme-0.1.4/scripts/countme-sqlite2csv.sh`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/scripts/countme-update-rawdb.sh` & `mirrors_countme-0.1.4/scripts/countme-update-rawdb.sh`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/scripts/countme-update-totals.sh` & `mirrors_countme-0.1.4/scripts/countme-update-totals.sh`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/scripts/countme-weekly-totals-ui.sh` & `mirrors_countme-0.1.4/scripts/countme-weekly-totals-ui.sh`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/scripts/rezip` & `mirrors_countme-0.1.4/scripts/countme-rezip`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/scripts/split-totals-db.sh` & `mirrors_countme-0.1.4/scripts/countme-split-totals-db.sh`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/conftest.py` & `mirrors_countme-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/scripts/test_countme_delete_totals.py` & `mirrors_countme-0.1.4/tests/scripts/test_countme_delete_totals.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/scripts/test_countme_parse_access_log.py` & `mirrors_countme-0.1.4/tests/scripts/test_countme_parse_access_log.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/scripts/test_countme_totals.py` & `mirrors_countme-0.1.4/tests/scripts/test_countme_totals.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/scripts/test_countme_trim_raw.py` & `mirrors_countme-0.1.4/tests/scripts/test_countme_trim_raw.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_integrate.py` & `mirrors_countme-0.1.4/tests/test_integrate.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_matchers.py` & `mirrors_countme-0.1.4/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_output_items.py` & `mirrors_countme-0.1.4/tests/test_output_items.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_parse.py` & `mirrors_countme-0.1.4/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_progress.py` & `mirrors_countme-0.1.4/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_readers.py` & `mirrors_countme-0.1.4/tests/test_readers.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_regex.py` & `mirrors_countme-0.1.4/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_totals.py` & `mirrors_countme-0.1.4/tests/test_totals.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_util.py` & `mirrors_countme-0.1.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/tests/test_writers.py` & `mirrors_countme-0.1.4/tests/test_writers.py`

 * *Files identical despite different names*

### Comparing `mirrors_countme-0.1.3/setup.py` & `mirrors_countme-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                      'countme-totals = '
                      'mirrors_countme.scripts.countme_totals:cli',
                      'countme-trim-raw = '
                      'mirrors_countme.scripts.countme_trim_raw:cli']}
 
 setup_kwargs = {
     'name': 'mirrors-countme',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Parse access logs and count hosts for DNF mirrors',
     'long_description': '# mirrors-countme\n\nParse http `access_log` data, find DNF `countme` requests, and output\nstructured data that lets us estimate the number of people using various\nFedora releases.\n\nSee [Changes/DNF Better Counting] for more info about the `countme` feature in\ngeneral.\n\n## How it works\n\nThe short version:\n\n* Starting in Fedora 32, DNF adds "countme=N" to one random HTTP request\n  per week for each repo that has its `countme` setting enabled.\n* `parse-access-log.py` parses logs from mirrors.fedoraproject.org, finds\n  those requests, and yields the following information:\n    * request timestamp, repo & arch\n    * client OS name, version, variant, and arch\n    * client "age", from 1-4: 1 week, 1 month, 6 months, or >6 months.\n* We use that data to make cool charts & graphs and estimate how many Fedora\n  users there are and what they\'re using.\n\n## Technical details\n\n### Client behavior & configuration\n\nDNF 4.2.9 added the `countme` option, which [dnf.conf(5)] describes like so:\n\n>    Determines whether a special flag should be added to a single, randomly\n>    chosen metalink/mirrorlist query each week.\n>    This allows the repository owner to estimate the number of systems\n>    consuming it, by counting such queries over a week\'s time, which is much\n>    more accurate than just counting unique IP addresses (which is subject to\n>    both overcounting and undercounting due to short DHCP leases and NAT,\n>    respectively).\n>\n>    The flag is a simple "countme=N" parameter appended to the metalink and\n>    mirrorlist URL, where N is an integer representing the "longevity" bucket\n>    this system belongs to.\n>    The following 4 buckets are defined, based on how many full weeks have\n>    passed since the beginning of the week when this system was installed: 1 =\n>    first week, 2 = first month (2-4 weeks), 3 = six months (5-24 weeks) and 4\n>    = more than six months (> 24 weeks).\n>    This information is meant to help distinguish short-lived installs from\n>    long-term ones, and to gather other statistics about system lifecycle.\n\nNote that the default is False, because we don\'t want to enable this for every\nrepo you have configured.\n\nStarting with Fedora 32, we set `countme=1` in Fedora official repo configs:\n\n```\n[updates]\nname=Fedora $releasever - $basearch - Updates\n#baseurl=http://download.example/pub/fedora/linux/updates/$releasever/Everything/$basearch/\nmetalink=https://mirrors.fedoraproject.org/metalink?repo=updates-released-f$releasever&arch=$basearch\nenabled=1\ncountme=1\nrepo_gpgcheck=0\ntype=rpm\ngpgcheck=1\nmetadata_expire=6h\ngpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-fedora-$releasever-$basearch\nskip_if_unavailable=False\n```\n\nThis means that the default configuration only adds "countme=N" when using\nofficial Fedora repos, which are all done via HTTPS connections to\nmirrors.fedoraproject.org. "countme=N" does _not_ get added in subsequent\nrequests to the chosen mirror(s).\n\n### Privacy, randomization, and user counting\n\nDNF makes a serious effort to keep the `countme` data anonymous _and_ accurate\nby only sending `countme` with one _random_ request to each enabled repo _per\nweek_. So how does it decide when the week starts, and how does it choose\nwhich request?\n\nFirst, all clients use the same "week": Week 0 started at timestamp 345600\n(Mon 05 Jan 1970 00:00:00 - the first Monday of POSIX time), and weeks are\nexactly 604800 (7&times;24&times;60&times;60) seconds long.\n\nSecond, all clients have the same random chance - currently 1:4 - to send\n`countme` with any request in a given week. Once it\'s been sent, the client\nwon\'t send another `countme` for that repo for the rest of the week.\n\nThe default update interval for the `updates` repo is 6 hours, which means\nthat clients who use `dnf-makecache.service` will probably send `countme`\nsometime in the first 24 hours of a given week - and nothing for the rest of\nthe week.\n\nThis means that _daily_ totals of users are unreliably variable, since the\nstart of the week will have more `countme` requests than the end of the week.\nBut the weekly totals should be a consistent, representative sample of the\ntotal population.\n\nFor more details on how libdnf handles the randomization, see\n[libdnf/repo/Repo.cpp:addCountmeFlag()].\n\n### Data collected\n\nThe only data we look at is in the HTTP request itself. Our log lines are in\nthe standard Combined Log Format, like so[^IPvBeefy]:\n\n```\n240.159.140.173 - - [29/Mar/2020:16:04:28 +0000] "GET /metalink?repo=fedora-modular-32&arch=x86_64&countme=1 HTTP/2.0" 200 18336 "-" "libdnf (Fedora 32; workstation; Linux.x86_64)"\n```\n\n\nWe only look at log lines where the request is "GET", the query string includes\n"countme=N", the result is 200 or 302, and the User-Agent string matches the\nlibdnf User-Agent header.\n\nThe only data we use are the timestamp, the query parameters (`repo`, `arch`,\n`countme`), and the libdnf User-Agent data.\n\n#### libdnf User-Agent data\n\nAs in the log line above, the User-Agent header that libdnf sends looks like this:\n\n```\nUser-Agent: libdnf (Fedora 32; workstation; Linux.x86_64)\n```\n\nThis string is assembled in [libdnf/utils/os-release.cpp:getUserAgent()] and\nthe format is as follows:\n\n```\n{product} ({os_name} {os_version}; {os_variant}; {os_canon}.{os_arch})\n```\n\nwhere the values are:\n\n`product`\n:  "libdnf"\n\n`os_name`\n:  [/etc/os-release] `NAME`\n\n`os_version`\n:  [/etc/os-release] `VERSION_ID`\n\n`os_variant`\n:  [/etc/os-release] `VARIANT_ID`\n\n`os_canon`\n:  rpm `%_os` (via libdnf `getCanonOS()`)\n\n`os_arch`\n:  rpm `%_arch` (via libdnf `getBaseArch()`)\n\n(Older versions of libdnf sent `libdnf/{LIBDNF_VERSION}` for the `product`,\nbut the version string was dropped in libdnf 0.37.2 due to privacy concerns;\nsee [libdnf commit d8d0984].)\n\n#### `repo=`, `arch=`, `countme=`\n\nThe `repo=` and `arch=` values are exactly what\'s set in the URL in the `.repo`\nfile.\n\n`repo` is whatever string appears after `repo=` in the repo\'s `metalink` URL.\nThe values that are accepted for `repo` are determined by [mirrormanager];\nsee [mirrormanager2/lib/repomap.py] for some of the gnarly details there.\n\n`arch` is usually set as `arch=$basearch`, which means that `os_arch` and\n`repo_arch` are usually the same value. But it _is_ valid for a client to\nuse a repo with an `arch=` that\'s different from rpm\'s `%_arch` - for example,\nan i686 system could use an i386 repo - so `repo_arch` and `os_arch` _may_ be\ndifferent values.\n\n`countme`, as discussed in [dnf.conf(5)], is a value from 1 to 4 indicating\nthe "age" of the system, counted in _full_ weeks since the system was\nfirst installed. The values are:\n\n1. One week or less (0-1 weeks)\n2. Up to one month (2-4 weeks)\n3. Up to six months (5-24 weeks)\n4. More than six months (25+ weeks)\n\nThese are defined in [libdnf/repo/Repo.cpp:COUNTME\\_BUCKETS].\n\n\n## OK but how do we actually use it in Fedora?\n\nBecause the raw log data contains IP and timestamps that could be used to\ntrack or identify users, we run the parsing and counting inside private parts\nof the Fedora infrastructure and only publish the anonymous aggregate data.\n\nIn practice, this is a three-part process:\n\n1. Run `countme-update-rawdb.sh` daily to parse log data into `rawdb`\n  * `rawdb` is a SQLite database of structured data for each `countme` hit\n  * Kept private since it contains IP addresses and timestamps\n  * Typical log data: ~6GB/day\n  * Typical parsing time: ~5min (Intel Core i7-6770HQ, 2.60GHz)\n  * Typical rawdb size: ~8MB/day for F32; I\'d guess keeping 1 year of data for\n    3 concurrent releases would take about 10GB.\n  * Retaining historical data lets us quickly recalculate counts if we\n    discover significant errors due to misconfigured/malicious clients\n2. Run `countme-update-totals.sh` to read `rawdb` and update `totalsdb`\n  * Counts up hits for each week, grouped by:\n    * System info: `os_name`, `os_version`, `os_variant`, `os_arch`, `sys_age`\n    * Repo requested: `repo_tag`, `repo_arch`\n  * Only generates data for weeks where we have complete log data\n  * No timestamps or IP addresses\n  * Typical parsing time: small, <=~5s\n  * Typical totalsdb size: ~55KB/week (~700 rows/week) for F32\n  * After update, (re)generate `totals.csv`\n3. Publish updated `totals.db` and `totals.csv`\n  * See https://data-analysis.fedoraproject.org/csv-reports/countme/\n  * Might end up in different places/forms in the future\n  * Can also run countme-weekly-totals-ui.sh command to see text data easily.\n\n## Contributing\n\nYou need to be legally allowed to submit any contribution to this project.\nWhat this means in detail is laid out at the [Developer Certificate of Origin]\nwebsite. The mechanism by which you certify this is adding a `Signed-off-by`\ntrailer to git commit log messages, you can do this by using the\n`--signoff/-s` option to `git commit`.\n\n[^IPvBeefy]: Don\'t worry, 240.159.140.173 is a fake IP address. Actually,\n             it\'s the 4-byte UTF-8 encoding for &#x1f32d;, U+1F32D HOT DOG.\n\n[Changes/DNF Better Counting]: https://fedoraproject.org/wiki/Changes/DNF_Better_Counting\n[dnf.conf(5)]: https://dnf.readthedocs.io/en/latest/conf_ref.html\n[/etc/os-release]: http://man7.org/linux/man-pages/man5/os-release.5.html\n[mirrormanager]: https://github.com/fedora-infra/mirrormanager2\n[mirrormanager2/lib/repomap.py]: https://github.com/fedora-infra/mirrormanager2/blob/master/mirrormanager2/lib/repomap.py\n[libdnf commit d8d0984]: https://github.com/rpm-software-management/libdnf/commit/d8d0984\n[libdnf/utils/os-release.cpp:getUserAgent()]: https://github.com/rpm-software-management/libdnf/blob/0.47.0/libdnf/utils/os-release.cpp#L108\n[libdnf/repo/Repo.cpp:addCountmeFlag()]: https://github.com/rpm-software-management/libdnf/blob/0.47.0/libdnf/repo/Repo.cpp#L1051\n[libdnf/repo/Repo.cpp:COUNTME\\_BUCKETS]: https://github.com/rpm-software-management/libdnf/blob/0.47.0/libdnf/repo/Repo.cpp#L92\n[Developer Certificate of Origin]: https://developercertificate.org\n',
     'author': 'Will Woods',
     'author_email': 'None',
     'maintainer': 'Fedora Infrastructure',
     'maintainer_email': 'admin@fedoraproject.org',
     'url': 'http://github.com/fedora-infra/mirrors-countme',
```

### Comparing `mirrors_countme-0.1.3/PKG-INFO` & `mirrors_countme-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirrors-countme
-Version: 0.1.3
+Version: 0.1.4
 Summary: Parse access logs and count hosts for DNF mirrors
 Home-page: http://github.com/fedora-infra/mirrors-countme
 License: GPL-3.0-or-later
 Author: Will Woods
 Maintainer: Fedora Infrastructure
 Maintainer-email: admin@fedoraproject.org
 Requires-Python: >=3.11,<4.0
```

