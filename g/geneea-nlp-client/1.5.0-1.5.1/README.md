# Comparing `tmp/geneea-nlp-client-1.5.0.tar.gz` & `tmp/geneea-nlp-client-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneea-nlp-client-1.5.0.tar", last modified: Fri May 10 09:34:46 2024, max compression
+gzip compressed data, was "geneea-nlp-client-1.5.1.tar", last modified: Mon May 13 12:31:13 2024, max compression
```

## Comparing `geneea-nlp-client-1.5.0.tar` & `geneea-nlp-client-1.5.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.902675 geneea-nlp-client-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-10 09:34:46.902675 geneea-nlp-client-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.882675 geneea-nlp-client-1.5.0/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.886675 geneea-nlp-client-1.5.0/examples/g3/
--rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/entitiesToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/languageToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     1485 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/quickStart.py
--rw-rw-rw-   0 root         (0) root         (0)     2890 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/quickStartAll.py
--rw-rw-rw-   0 root         (0) root         (0)     2034 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/quickStartEntities.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/relationsToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/sentimentToExcel.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.886675 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1609 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.886675 geneea-nlp-client-1.5.0/geneeanlpclient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.890675 geneea-nlp-client-1.5.0/geneeanlpclient/common/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/common.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/dictutil.py
--rw-rw-rw-   0 root         (0) root         (0)     2809 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/restutil.py
--rw-rw-rw-   0 root         (0) root         (0)     5410 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/ud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.894675 geneea-nlp-client-1.5.0/geneeanlpclient/g3/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2952 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/client.py
--rw-rw-rw-   0 root         (0) root         (0)    29568 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/f2converter.py
--rw-rw-rw-   0 root         (0) root         (0)    57073 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/model.py
--rw-rw-rw-   0 root         (0) root         (0)    16707 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/reader.py
--rw-rw-rw-   0 root         (0) root         (0)    18574 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/request.py
--rw-rw-rw-   0 root         (0) root         (0)     8244 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/writer.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-10 09:34:46.902675 geneea-nlp-client-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1480 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.894675 geneea-nlp-client-1.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.894675 geneea-nlp-client-1.5.0/tests/geneeanlpclient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.898675 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2743 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_common.py
--rw-rw-rw-   0 root         (0) root         (0)     4103 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_jsonutil.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_ud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.902675 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/generate.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_charSpan.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_f2converter.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     9172 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_rw.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_tokenSupport.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_tokenutils.py
--rw-rw-rw-   0 root         (0) root         (0)     5447 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_treeBuilder.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.150021 geneea-nlp-client-1.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-13 12:31:13.150021 geneea-nlp-client-1.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.146021 geneea-nlp-client-1.5.1/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/examples/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.146021 geneea-nlp-client-1.5.1/examples/g3/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/examples/g3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/examples/g3/entitiesToExcel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/examples/g3/languageToExcel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/examples/g3/quickStart.py
+-rw-rw-rw-   0 root         (0) root         (0)     2890 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/examples/g3/quickStartAll.py
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/examples/g3/quickStartEntities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/examples/g3/relationsToExcel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/examples/g3/sentimentToExcel.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.146021 geneea-nlp-client-1.5.1/geneea_nlp_client.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-13 12:31:12.000000 geneea-nlp-client-1.5.1/geneea_nlp_client.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-05-13 12:31:12.000000 geneea-nlp-client-1.5.1/geneea_nlp_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-13 12:31:12.000000 geneea-nlp-client-1.5.1/geneea_nlp_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-13 12:31:12.000000 geneea-nlp-client-1.5.1/geneea_nlp_client.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-13 12:31:12.000000 geneea-nlp-client-1.5.1/geneea_nlp_client.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.146021 geneea-nlp-client-1.5.1/geneeanlpclient/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.146021 geneea-nlp-client-1.5.1/geneeanlpclient/common/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/common/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/common/dictutil.py
+-rw-rw-rw-   0 root         (0) root         (0)     2809 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/common/restutil.py
+-rw-rw-rw-   0 root         (0) root         (0)     5410 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/common/ud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.150021 geneea-nlp-client-1.5.1/geneeanlpclient/g3/
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/g3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/g3/client.py
+-rw-rw-rw-   0 root         (0) root         (0)    29568 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/g3/f2converter.py
+-rw-rw-rw-   0 root         (0) root         (0)    57481 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/g3/model.py
+-rw-rw-rw-   0 root         (0) root         (0)    16707 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/g3/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    18574 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/g3/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     8244 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/geneeanlpclient/g3/writer.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-13 12:31:13.150021 geneea-nlp-client-1.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.150021 geneea-nlp-client-1.5.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.150021 geneea-nlp-client-1.5.1/tests/geneeanlpclient/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.150021 geneea-nlp-client-1.5.1/tests/geneeanlpclient/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2743 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/common/test_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4103 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/common/test_jsonutil.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/common/test_ud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 12:31:13.150021 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_charSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_f2converter.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     9172 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_rw.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_tokenSupport.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_tokenutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2024-05-13 12:31:03.000000 geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_treeBuilder.py
```

### Comparing `geneea-nlp-client-1.5.0/LICENSE` & `geneea-nlp-client-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/PKG-INFO` & `geneea-nlp-client-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneea-nlp-client
-Version: 1.5.0
+Version: 1.5.1
 Summary: The SDK library and command-line interface to Geneea Interpretor, an NLP REST API.
 Home-page: https://geneea.com
 Author: Geneea Analytics s.r.o
 Author-email: support@geneea.com
 License: UNKNOWN
 Project-URL: Documentation, https://help.geneea.com/sdk/index.html
 Project-URL: Source Code, https://bitbucket.org/geneea/sdk
```

### Comparing `geneea-nlp-client-1.5.0/examples/g3/entitiesToExcel.py` & `geneea-nlp-client-1.5.1/examples/g3/entitiesToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/examples/g3/languageToExcel.py` & `geneea-nlp-client-1.5.1/examples/g3/languageToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/examples/g3/quickStart.py` & `geneea-nlp-client-1.5.1/examples/g3/quickStart.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/examples/g3/quickStartAll.py` & `geneea-nlp-client-1.5.1/examples/g3/quickStartAll.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/examples/g3/quickStartEntities.py` & `geneea-nlp-client-1.5.1/examples/g3/quickStartEntities.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/examples/g3/relationsToExcel.py` & `geneea-nlp-client-1.5.1/examples/g3/relationsToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/examples/g3/sentimentToExcel.py` & `geneea-nlp-client-1.5.1/examples/g3/sentimentToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/PKG-INFO` & `geneea-nlp-client-1.5.1/geneea_nlp_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneea-nlp-client
-Version: 1.5.0
+Version: 1.5.1
 Summary: The SDK library and command-line interface to Geneea Interpretor, an NLP REST API.
 Home-page: https://geneea.com
 Author: Geneea Analytics s.r.o
 Author-email: support@geneea.com
 License: UNKNOWN
 Project-URL: Documentation, https://help.geneea.com/sdk/index.html
 Project-URL: Source Code, https://bitbucket.org/geneea/sdk
```

### Comparing `geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/SOURCES.txt` & `geneea-nlp-client-1.5.1/geneea_nlp_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/common/common.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/common/common.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/common/dictutil.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/common/dictutil.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/common/restutil.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/common/restutil.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/common/ud.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/common/ud.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/g3/client.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/g3/client.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/g3/f2converter.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/g3/f2converter.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/g3/model.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/g3/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -927,14 +927,24 @@
         self.intValue: Optional[int] = intValue
         """ Actual value if the type is integer """
         self.strValue: Optional[str] = strValue
         """ Actual value if the type is string (including datetime values and GPS coordinates) """
         if boolValue is None and floatValue is None and intValue is None and strValue is None:
             raise ValueError(f'At least one value has to be set for GkbProperty {name} ({valueGkbId})')
 
+    def __eq__(self, other):
+        if not isinstance(other, GkbProperty):
+            return False
+        return (self.name == other.name
+                and self.valueGkbId == self.valueGkbId
+                and self.boolValue == self.boolValue
+                and self.floatValue == self.floatValue
+                and self.intValue == self.intValue
+                and self.strValue == self.strValue)
+
     def __hash__(self):
         return hash((self.name, self.valueGkbId, self.boolValue, self.floatValue, self.intValue, self.strValue))
 
     def __str__(self):
         return objToStr(self, ('name', 'valueGkbId', 'boolValue', 'floatValue', 'intValue', 'strValue'))
 
     def __repr__(self):
```

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/g3/reader.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/g3/reader.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/g3/request.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/g3/request.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/geneeanlpclient/g3/writer.py` & `geneea-nlp-client-1.5.1/geneeanlpclient/g3/writer.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/setup.py` & `geneea-nlp-client-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', mode='r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='geneea-nlp-client',
-    version='1.5.0',
+    version='1.5.1',
 
     author='Geneea Analytics s.r.o',
     author_email='support@geneea.com',
     description='The SDK library and command-line interface to Geneea Interpretor, an NLP REST API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='geneea python interpretor nlp nlu api cli',
```

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_common.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/common/test_common.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_jsonutil.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/common/test_jsonutil.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/examples.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/examples.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/generate.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/generate.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_analysis.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_analysis.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_charSpan.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_charSpan.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_f2converter.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_f2converter.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_request.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_request.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_rw.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_rw.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_tokenSupport.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_tokenSupport.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_tokenutils.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_tokenutils.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_treeBuilder.py` & `geneea-nlp-client-1.5.1/tests/geneeanlpclient/g3/test_treeBuilder.py`

 * *Files identical despite different names*

