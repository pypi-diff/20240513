# Comparing `tmp/wild_code-0.4.0.tar.gz` & `tmp/wild_code-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_code-0.4.0.tar", last modified: Sun May 12 00:36:31 2024, max compression
+gzip compressed data, was "wild_code-0.4.3.tar", last modified: Sun May 12 22:22:37 2024, max compression
```

## Comparing `wild_code-0.4.0.tar` & `wild_code-0.4.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:53.208150 wild_code-0.4.0/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-11 18:05:22.000000 wild_code-0.4.0/.dockerignore
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.409448 wild_code-0.4.0/.github/
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.408497 wild_code-0.4.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-10 14:48:48.000000 wild_code-0.4.0/.github/ISSUE_TEMPLATE/buggy_contract.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-07 17:11:36.000000 wild_code-0.4.0/.github/ISSUE_TEMPLATE/buggy_test.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-07 17:11:36.000000 wild_code-0.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-07 17:11:36.000000 wild_code-0.4.0/.github/ISSUE_TEMPLATE/model_eval_request.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-07 17:11:36.000000 wild_code-0.4.0/.gitignore
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-07 17:11:36.000000 wild_code-0.4.0/.pre-commit-config.yaml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-07 17:11:36.000000 wild_code-0.4.0/CITATION.cff
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      757 2024-05-11 23:30:52.000000 wild_code-0.4.0/Dockerfile
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-07 17:11:36.000000 wild_code-0.4.0/LICENSE
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-07 17:11:36.000000 wild_code-0.4.0/MANIFEST.in
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10797 2024-05-12 00:33:53.201888 wild_code-0.4.0/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9684 2024-05-11 23:45:13.000000 wild_code-0.4.0/README.md
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-07 17:11:36.000000 wild_code-0.4.0/pyproject.toml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-11 23:46:21.000000 wild_code-0.4.0/release.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      155 2024-05-11 23:46:56.000000 wild_code-0.4.0/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1348 2024-05-11 20:16:24.000000 wild_code-0.4.0/run.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1237 2024-05-12 00:33:53.224755 wild_code-0.4.0/setup.cfg
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.414260 wild_code-0.4.0/tests/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-07 17:11:36.000000 wild_code-0.4.0/tests/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-07 17:11:36.000000 wild_code-0.4.0/tests/test_legacy_sanitizer.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-07 17:11:36.000000 wild_code-0.4.0/tests/test_treesitter_sanitizer.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:53.178377 wild_code-0.4.0/wild_code.egg-info/
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10797 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/SOURCES.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/dependency_links.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/entry_points.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/requires.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/top_level.txt
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.443536 wild_code-0.4.0/wildcode/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-12 00:33:52.000000 wild_code-0.4.0/wildcode/_version.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.432472 wild_code-0.4.0/wildcode/data/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/data/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/data/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1612 2024-05-10 15:13:52.000000 wild_code-0.4.0/wildcode/data/wildcodebench.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.437948 wild_code-0.4.0/wildcode/eval/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7214 2024-05-11 17:29:07.000000 wild_code-0.4.0/wildcode/eval/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/eval/_special_oracle.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5715 2024-05-11 17:28:58.000000 wild_code-0.4.0/wildcode/eval/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8279 2024-05-10 22:27:09.000000 wild_code-0.4.0/wildcode/evaluate.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.452117 wild_code-0.4.0/wildcode/gen/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/gen/__init__.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.451450 wild_code-0.4.0/wildcode/gen/util/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2159 2024-05-11 17:28:48.000000 wild_code-0.4.0/wildcode/gen/util/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/gen/util/anthropic_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/gen/util/openai_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5550 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/generate.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/inspect.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/lecacy_sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    14089 2024-05-09 02:01:13.000000 wild_code-0.4.0/wildcode/model.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7991 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/syncheck.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:59.203994 wild_code-0.4.3/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-12 22:19:33.000000 wild_code-0.4.3/.dockerignore
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.216561 wild_code-0.4.3/.github/
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.216113 wild_code-0.4.3/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-12 22:19:33.000000 wild_code-0.4.3/.github/ISSUE_TEMPLATE/buggy_contract.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-12 22:19:33.000000 wild_code-0.4.3/.github/ISSUE_TEMPLATE/buggy_test.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-12 22:19:33.000000 wild_code-0.4.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-12 22:19:33.000000 wild_code-0.4.3/.github/ISSUE_TEMPLATE/model_eval_request.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-12 22:19:33.000000 wild_code-0.4.3/.gitignore
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-12 22:19:33.000000 wild_code-0.4.3/.pre-commit-config.yaml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-12 22:19:33.000000 wild_code-0.4.3/CITATION.cff
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      757 2024-05-12 22:19:33.000000 wild_code-0.4.3/Dockerfile
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-12 22:19:33.000000 wild_code-0.4.3/LICENSE
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-12 22:19:33.000000 wild_code-0.4.3/MANIFEST.in
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10938 2024-05-12 22:19:59.196091 wild_code-0.4.3/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9825 2024-05-12 22:19:33.000000 wild_code-0.4.3/README.md
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-12 22:19:33.000000 wild_code-0.4.3/pyproject.toml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-12 22:19:33.000000 wild_code-0.4.3/release.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      156 2024-05-12 22:19:33.000000 wild_code-0.4.3/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1348 2024-05-12 22:19:33.000000 wild_code-0.4.3/run.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1237 2024-05-12 22:19:59.220794 wild_code-0.4.3/setup.cfg
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.221269 wild_code-0.4.3/tests/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-12 22:19:33.000000 wild_code-0.4.3/tests/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-12 22:19:33.000000 wild_code-0.4.3/tests/test_legacy_sanitizer.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-12 22:19:33.000000 wild_code-0.4.3/tests/test_treesitter_sanitizer.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:59.169551 wild_code-0.4.3/wild_code.egg-info/
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10938 2024-05-12 22:19:57.000000 wild_code-0.4.3/wild_code.egg-info/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/entry_points.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/requires.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/top_level.txt
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.255855 wild_code-0.4.3/wildcode/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-12 22:19:57.000000 wild_code-0.4.3/wildcode/_version.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.244229 wild_code-0.4.3/wildcode/data/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/data/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/data/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1612 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/data/wildcodebench.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.250298 wild_code-0.4.3/wildcode/eval/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7214 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/eval/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/eval/_special_oracle.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5715 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/eval/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8279 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/evaluate.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.267472 wild_code-0.4.3/wildcode/gen/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/gen/__init__.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.266954 wild_code-0.4.3/wildcode/gen/util/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2159 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/gen/util/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/gen/util/anthropic_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/gen/util/openai_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5558 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/generate.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/inspect.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/lecacy_sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    14089 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/model.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7991 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/syncheck.py
```

### Comparing `wild_code-0.4.0/.dockerignore` & `wild_code-0.4.3/.dockerignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/.github/ISSUE_TEMPLATE/buggy_contract.yml` & `wild_code-0.4.3/.github/ISSUE_TEMPLATE/buggy_contract.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/.github/ISSUE_TEMPLATE/buggy_test.yml` & `wild_code-0.4.3/.github/ISSUE_TEMPLATE/buggy_test.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/.github/ISSUE_TEMPLATE/model_eval_request.yml` & `wild_code-0.4.3/.github/ISSUE_TEMPLATE/model_eval_request.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/.gitignore` & `wild_code-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/Dockerfile` & `wild_code-0.4.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/LICENSE` & `wild_code-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/PKG-INFO` & `wild_code-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.4.0
+Version: 0.4.3
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -116,18 +116,23 @@
 ```
 
 </div>
 </details>
 
 ### Code Generation
 
+You are suggested to use `flash-attn` for generating code samples.
+```shell
+pip install -U flash-attn
+```
+
 To generate code samples from a model, you can use the following command:
 
 ```shell
-wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
+wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
 ```
 The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
@@ -182,15 +187,15 @@
 
 ### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
 # mount the current directory to the container
-docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl
+docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl --check-gt-only
 # ...Or locally ⚠️
 wildcode.evaluate --dataset wildcodebench --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.4.0 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.4.3 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
@@ -55,20 +55,22 @@
 ```shell pip install wild-code --upgrade ``` â¬ Install nightly version ::
 click to expand ::
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
-### Code Generation To generate code samples from a model, you can use the
-following command: ```shell wildcode.generate --model [model_name] --dataset
-[wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples]
---resume --backend [vllm|hf|openai] ``` The generated code samples will be
-stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-
-[n_samples].jsonl`. ð¤ Structure of `problem`? :: click to expand ::
+### Code Generation You are suggested to use `flash-attn` for generating code
+samples. ```shell pip install -U flash-attn ``` To generate code samples from a
+model, you can use the following command: ```shell wildcode.generate --model
+[model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp]
+--n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
+``` The generated code samples will be stored in a file named `[model_name]--
+wildcodebench--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
+`problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation + `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
 [temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
 `get_wildcodebench()` > 2. `solution` (optional): Self-contained solution
@@ -88,18 +90,18 @@
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
 ### Code Evaluation You are strongly recommended to use a sandbox such as
 [docker](https://docs.docker.com/get-docker/): ```shell # mount the current
 directory to the container docker run -v $(pwd) terryzho/wildcode:latest --
-dataset wildcodebench --samples samples.jsonl # ...Or locally â ï¸
-wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ``` ...Or if
-you want to try it locally regardless of the risks â ï¸: First, install the
-dependencies for WildCodeBench: ```shell pip install -r https://
+dataset wildcodebench --samples samples.jsonl --check-gt-only # ...Or locally
+â ï¸ wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ```
+...Or if you want to try it locally regardless of the risks â ï¸: First,
+install the dependencies for WildCodeBench: ```shell pip install -r https://
 raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/
 requirements.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
 dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
 very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
 OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
 solution's runtime. > > Additionally, you are **NOT** encouraged to make your
 test-bed over stressed while running evaluation. > For example, using `--
```

### Comparing `wild_code-0.4.0/README.md` & `wild_code-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,18 +82,23 @@
 ```
 
 </div>
 </details>
 
 ### Code Generation
 
+You are suggested to use `flash-attn` for generating code samples.
+```shell
+pip install -U flash-attn
+```
+
 To generate code samples from a model, you can use the following command:
 
 ```shell
-wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
+wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
 ```
 The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
@@ -148,15 +153,15 @@
 
 ### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
 # mount the current directory to the container
-docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl
+docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl --check-gt-only
 # ...Or locally ⚠️
 wildcode.evaluate --dataset wildcodebench --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
```

#### html2text {}

```diff
@@ -40,20 +40,22 @@
 ```shell pip install wild-code --upgrade ``` â¬ Install nightly version ::
 click to expand ::
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
-### Code Generation To generate code samples from a model, you can use the
-following command: ```shell wildcode.generate --model [model_name] --dataset
-[wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples]
---resume --backend [vllm|hf|openai] ``` The generated code samples will be
-stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-
-[n_samples].jsonl`. ð¤ Structure of `problem`? :: click to expand ::
+### Code Generation You are suggested to use `flash-attn` for generating code
+samples. ```shell pip install -U flash-attn ``` To generate code samples from a
+model, you can use the following command: ```shell wildcode.generate --model
+[model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp]
+--n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
+``` The generated code samples will be stored in a file named `[model_name]--
+wildcodebench--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
+`problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation + `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
 [temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
 `get_wildcodebench()` > 2. `solution` (optional): Self-contained solution
@@ -73,18 +75,18 @@
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
 ### Code Evaluation You are strongly recommended to use a sandbox such as
 [docker](https://docs.docker.com/get-docker/): ```shell # mount the current
 directory to the container docker run -v $(pwd) terryzho/wildcode:latest --
-dataset wildcodebench --samples samples.jsonl # ...Or locally â ï¸
-wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ``` ...Or if
-you want to try it locally regardless of the risks â ï¸: First, install the
-dependencies for WildCodeBench: ```shell pip install -r https://
+dataset wildcodebench --samples samples.jsonl --check-gt-only # ...Or locally
+â ï¸ wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ```
+...Or if you want to try it locally regardless of the risks â ï¸: First,
+install the dependencies for WildCodeBench: ```shell pip install -r https://
 raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/
 requirements.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
 dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
 very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
 OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
 solution's runtime. > > Additionally, you are **NOT** encouraged to make your
 test-bed over stressed while running evaluation. > For example, using `--
```

### Comparing `wild_code-0.4.0/release.sh` & `wild_code-0.4.3/release.sh`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/run.sh` & `wild_code-0.4.3/run.sh`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/setup.cfg` & `wild_code-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/tests/test_legacy_sanitizer.py` & `wild_code-0.4.3/tests/test_legacy_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/tests/test_treesitter_sanitizer.py` & `wild_code-0.4.3/tests/test_treesitter_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wild_code.egg-info/PKG-INFO` & `wild_code-0.4.3/wild_code.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.4.0
+Version: 0.4.3
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -116,18 +116,23 @@
 ```
 
 </div>
 </details>
 
 ### Code Generation
 
+You are suggested to use `flash-attn` for generating code samples.
+```shell
+pip install -U flash-attn
+```
+
 To generate code samples from a model, you can use the following command:
 
 ```shell
-wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
+wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
 ```
 The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
@@ -182,15 +187,15 @@
 
 ### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
 # mount the current directory to the container
-docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl
+docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl --check-gt-only
 # ...Or locally ⚠️
 wildcode.evaluate --dataset wildcodebench --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.4.0 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.4.3 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
@@ -55,20 +55,22 @@
 ```shell pip install wild-code --upgrade ``` â¬ Install nightly version ::
 click to expand ::
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
-### Code Generation To generate code samples from a model, you can use the
-following command: ```shell wildcode.generate --model [model_name] --dataset
-[wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples]
---resume --backend [vllm|hf|openai] ``` The generated code samples will be
-stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-
-[n_samples].jsonl`. ð¤ Structure of `problem`? :: click to expand ::
+### Code Generation You are suggested to use `flash-attn` for generating code
+samples. ```shell pip install -U flash-attn ``` To generate code samples from a
+model, you can use the following command: ```shell wildcode.generate --model
+[model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp]
+--n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
+``` The generated code samples will be stored in a file named `[model_name]--
+wildcodebench--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
+`problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation + `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
 [temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
 `get_wildcodebench()` > 2. `solution` (optional): Self-contained solution
@@ -88,18 +90,18 @@
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
 ### Code Evaluation You are strongly recommended to use a sandbox such as
 [docker](https://docs.docker.com/get-docker/): ```shell # mount the current
 directory to the container docker run -v $(pwd) terryzho/wildcode:latest --
-dataset wildcodebench --samples samples.jsonl # ...Or locally â ï¸
-wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ``` ...Or if
-you want to try it locally regardless of the risks â ï¸: First, install the
-dependencies for WildCodeBench: ```shell pip install -r https://
+dataset wildcodebench --samples samples.jsonl --check-gt-only # ...Or locally
+â ï¸ wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ```
+...Or if you want to try it locally regardless of the risks â ï¸: First,
+install the dependencies for WildCodeBench: ```shell pip install -r https://
 raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/
 requirements.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
 dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
 very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
 OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
 solution's runtime. > > Additionally, you are **NOT** encouraged to make your
 test-bed over stressed while running evaluation. > For example, using `--
```

### Comparing `wild_code-0.4.0/wild_code.egg-info/SOURCES.txt` & `wild_code-0.4.3/wild_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/data/utils.py` & `wild_code-0.4.3/wildcode/data/utils.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/data/wildcodebench.py` & `wild_code-0.4.3/wildcode/data/wildcodebench.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/eval/__init__.py` & `wild_code-0.4.3/wildcode/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/eval/utils.py` & `wild_code-0.4.3/wildcode/eval/utils.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/evaluate.py` & `wild_code-0.4.3/wildcode/evaluate.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/gen/__init__.py` & `wild_code-0.4.3/wildcode/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/gen/util/__init__.py` & `wild_code-0.4.3/wildcode/gen/util/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/gen/util/anthropic_request.py` & `wild_code-0.4.3/wildcode/gen/util/anthropic_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/gen/util/openai_request.py` & `wild_code-0.4.3/wildcode/gen/util/openai_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/generate.py` & `wild_code-0.4.3/wildcode/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                     num_samples=n_samples - sidx,
                 )
                 assert outputs, "No outputs from model!"
                 if model.is_direct_completion():
                     samples = [
                         dict(
                             task_id=task_id,
-                            solution=prompt+completion,
+                            solution=task["prompt"]+completion,
                         )
                         for task_id, completion in zip([task_id]*len(outputs), outputs)
                     ]
                 else:
                     samples = [
                         dict(
                             task_id=task_id,
```

### Comparing `wild_code-0.4.0/wildcode/inspect.py` & `wild_code-0.4.3/wildcode/inspect.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/lecacy_sanitize.py` & `wild_code-0.4.3/wildcode/lecacy_sanitize.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/model.py` & `wild_code-0.4.3/wildcode/model.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/sanitize.py` & `wild_code-0.4.3/wildcode/sanitize.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.0/wildcode/syncheck.py` & `wild_code-0.4.3/wildcode/syncheck.py`

 * *Files identical despite different names*

