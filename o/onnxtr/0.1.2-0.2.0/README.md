# Comparing `tmp/onnxtr-0.1.2.tar.gz` & `tmp/onnxtr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxtr-0.1.2.tar", last modified: Fri May 10 13:51:56 2024, max compression
+gzip compressed data, was "onnxtr-0.2.0.tar", last modified: Mon May 13 10:40:57 2024, max compression
```

## Comparing `onnxtr-0.1.2.tar` & `onnxtr-0.2.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.514306 onnxtr-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 13:51:43.000000 onnxtr-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-05-10 13:51:56.514306 onnxtr-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-10 13:51:43.000000 onnxtr-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.498305 onnxtr-0.1.2/onnxtr/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.502306 onnxtr-0.1.2/onnxtr/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/contrib/artefacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/contrib/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.502306 onnxtr-0.1.2/onnxtr/io/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/io/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/io/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/io/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/io/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/io/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.502306 onnxtr-0.1.2/onnxtr/models/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.502306 onnxtr-0.1.2/onnxtr/models/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.506306 onnxtr-0.1.2/onnxtr/models/classification/models/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/classification/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/classification/models/mobilenet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.506306 onnxtr-0.1.2/onnxtr/models/classification/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/classification/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/classification/predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/classification/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.506306 onnxtr-0.1.2/onnxtr/models/detection/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.506306 onnxtr-0.1.2/onnxtr/models/detection/models/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/models/differentiable_binarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/models/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/models/linknet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.506306 onnxtr-0.1.2/onnxtr/models/detection/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/postprocessor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.506306 onnxtr-0.1.2/onnxtr/models/detection/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/detection/zoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.506306 onnxtr-0.1.2/onnxtr/models/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.506306 onnxtr-0.1.2/onnxtr/models/preprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/preprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/preprocessor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.506306 onnxtr-0.1.2/onnxtr/models/recognition/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.510306 onnxtr-0.1.2/onnxtr/models/recognition/models/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/models/crnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/models/master.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/models/parseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/models/sar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/models/vitstr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.510306 onnxtr-0.1.2/onnxtr/models/recognition/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/predictor/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/recognition/zoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/models/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.510306 onnxtr-0.1.2/onnxtr/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/transforms/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.510306 onnxtr-0.1.2/onnxtr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/common_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17002 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/multithreading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/reconstitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-10 13:51:43.000000 onnxtr-0.1.2/onnxtr/utils/vocabs.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 13:51:56.000000 onnxtr-0.1.2/onnxtr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:51:56.510306 onnxtr-0.1.2/onnxtr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-05-10 13:51:56.000000 onnxtr-0.1.2/onnxtr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-10 13:51:56.000000 onnxtr-0.1.2/onnxtr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:51:56.000000 onnxtr-0.1.2/onnxtr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-10 13:51:56.000000 onnxtr-0.1.2/onnxtr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 13:51:56.000000 onnxtr-0.1.2/onnxtr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:51:56.000000 onnxtr-0.1.2/onnxtr.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-10 13:51:43.000000 onnxtr-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:51:56.514306 onnxtr-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-10 13:51:43.000000 onnxtr-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.167072 onnxtr-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 10:40:44.000000 onnxtr-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-05-13 10:40:57.167072 onnxtr-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-13 10:40:44.000000 onnxtr-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.151072 onnxtr-0.2.0/onnxtr/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.151072 onnxtr-0.2.0/onnxtr/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/contrib/artefacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/contrib/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.155072 onnxtr-0.2.0/onnxtr/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/io/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/io/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/io/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/io/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.155072 onnxtr-0.2.0/onnxtr/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.155072 onnxtr-0.2.0/onnxtr/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.155072 onnxtr-0.2.0/onnxtr/models/classification/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/classification/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/classification/models/mobilenet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.155072 onnxtr-0.2.0/onnxtr/models/classification/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/classification/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/classification/predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/classification/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.159072 onnxtr-0.2.0/onnxtr/models/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.159072 onnxtr-0.2.0/onnxtr/models/detection/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/models/differentiable_binarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/models/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/models/linknet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.159072 onnxtr-0.2.0/onnxtr/models/detection/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/postprocessor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.159072 onnxtr-0.2.0/onnxtr/models/detection/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/detection/zoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.159072 onnxtr-0.2.0/onnxtr/models/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.159072 onnxtr-0.2.0/onnxtr/models/preprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/preprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/preprocessor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.159072 onnxtr-0.2.0/onnxtr/models/recognition/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.163072 onnxtr-0.2.0/onnxtr/models/recognition/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/models/crnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/models/master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/models/parseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/models/sar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/models/vitstr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.163072 onnxtr-0.2.0/onnxtr/models/recognition/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/predictor/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/recognition/zoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/models/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.163072 onnxtr-0.2.0/onnxtr/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/transforms/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.163072 onnxtr-0.2.0/onnxtr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17002 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/multithreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/reconstitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-13 10:40:44.000000 onnxtr-0.2.0/onnxtr/utils/vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 10:40:56.000000 onnxtr-0.2.0/onnxtr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:40:57.163072 onnxtr-0.2.0/onnxtr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-05-13 10:40:57.000000 onnxtr-0.2.0/onnxtr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-13 10:40:57.000000 onnxtr-0.2.0/onnxtr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:40:57.000000 onnxtr-0.2.0/onnxtr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-13 10:40:57.000000 onnxtr-0.2.0/onnxtr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 10:40:57.000000 onnxtr-0.2.0/onnxtr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:40:57.000000 onnxtr-0.2.0/onnxtr.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-13 10:40:44.000000 onnxtr-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:40:57.167072 onnxtr-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-13 10:40:44.000000 onnxtr-0.2.0/setup.py
```

### Comparing `onnxtr-0.1.2/LICENSE` & `onnxtr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/PKG-INFO` & `onnxtr-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxtr
-Version: 0.1.2
+Version: 0.2.0
 Summary: Onnx Text Recognition (OnnxTR): docTR Onnx-Wrapper for high-performance OCR on documents.
 Author-email: Felix Dittrich <felixdittrich92@gmail.com>
 Maintainer: Felix Dittrich
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -271,25 +271,26 @@
 </p>
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
 ![Build Status](https://github.com/felixdittrich92/onnxtr/workflows/builds/badge.svg)
 [![codecov](https://codecov.io/gh/felixdittrich92/OnnxTR/graph/badge.svg?token=WVFRCQBOLI)](https://codecov.io/gh/felixdittrich92/OnnxTR)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/4fff4d764bb14fb8b4f4afeb9587231b)](https://app.codacy.com/gh/felixdittrich92/OnnxTR/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![CodeFactor](https://www.codefactor.io/repository/github/felixdittrich92/onnxtr/badge)](https://www.codefactor.io/repository/github/felixdittrich92/onnxtr)
-[![Pypi](https://img.shields.io/badge/pypi-v0.1.1-blue.svg)](https://pypi.org/project/OnnxTR/)
+[![Pypi](https://img.shields.io/badge/pypi-v0.2.0-blue.svg)](https://pypi.org/project/OnnxTR/)
 
 > :warning: Please note that this is a wrapper around the [doctr](https://github.com/mindee/doctr) library to provide a Onnx pipeline for docTR. For feature requests, which are not directly related to the Onnx pipeline, please refer to the base project.
 
 **Optical Character Recognition made seamless & accessible to anyone, powered by Onnx**
 
 What you can expect from this repository:
 
 - efficient ways to parse textual information (localize and identify each word) from your documents
-- a Onnx pipeline for docTR, a wrapper around the [doctr](https://github.com/mindee/doctr) library
+- a Onnx pipeline for docTR, a wrapper around the [doctr](https://github.com/mindee/doctr) library - no PyTorch or TensorFlow dependencies
 - more lightweight package with faster inference latency and less required resources
+- 8-Bit quantized models for faster inference on CPU
 
 ![OCR_example](https://github.com/felixdittrich92/OnnxTR/raw/main/docs/images/ocr.png)
 
 ## Installation
 
 ### Prerequisites
 
@@ -354,14 +355,17 @@
     # Additional parameters - meta information
     detect_orientation=False,  # set to `True` if the orientation of the pages should be detected (default: False)
     detect_language=False, # set to `True` if the language of the pages should be detected (default: False)
     # DocumentBuilder specific parameters
     resolve_lines=True,  # whether words should be automatically grouped into lines (default: True)
     resolve_blocks=True,  # whether lines should be automatically grouped into blocks (default: True)
     paragraph_break=0.035,  # relative length of the minimum space separating paragraphs (default: 0.035)
+    # OnnxTR specific parameters
+    # NOTE: 8-Bit quantized models are not available for FAST detection models and can in general lead to poorer accuracy
+    load_in_8_bit=False,  # set to `True` to load 8-bit quantized models instead of the full precision onces (default: False)
 )
 # PDF
 doc = DocumentFile.from_pdf("path/to/your/doc.pdf")
 # Analyze
 result = model(doc)
 # Display the result (requires matplotlib & mplcursors to be installed)
 result.show()
@@ -434,17 +438,17 @@
         [
             'db_resnet34',
             'db_resnet50',
             'db_mobilenet_v3_large',
             'linknet_resnet18',
             'linknet_resnet34',
             'linknet_resnet50',
-            'fast_tiny',
-            'fast_small',
-            'fast_base'
+            'fast_tiny',  # No 8-bit support
+            'fast_small',  # No 8-bit support
+            'fast_base'  # No 8-bit support
         ],
     'recognition archs':
         [
             'crnn_vgg16_bn',
             'crnn_mobilenet_v3_small',
             'crnn_mobilenet_v3_large',
             'sar_resnet31',
@@ -465,22 +469,44 @@
 NOTE:
 
 - `pretrained` is the default in OnnxTR, and not available as a parameter.
 - docTR specific environment variables (e.g.: DOCTR_CACHE_DIR -> ONNXTR_CACHE_DIR) needs to be replaced with `ONNXTR_` prefix.
 
 ### Benchmarks
 
-The benchmarks was measured on a `i7-14700K Intel CPU`.
+The CPU benchmarks was measured on a `i7-14700K Intel CPU`.
 
-MORE BENCHMARKS COMING SOON
+The GPU benchmarks was measured on a `RTX 4080 Nvidia GPU`.
 
-|Dataset                         |docTR (CPU) - v0.8.1           |OnnxTR (CPU) - v0.1.1          |
+Benchmarking performed on the FUNSD dataset and CORD dataset.
+
+docTR / OnnxTR models used for the benchmarks are `fast_base` (full precision) | `db_resnet50` (8-bit variant) for detection and `crnn_vgg16_bn` for recognition.
+
+The smallest combination in OnnxTR (docTR) of `db_mobilenet_v3_large` and `crnn_mobilenet_v3_small` takes as comparison `~0.17s / Page` on the FUNSD dataset and `~0.12s / Page` on the CORD dataset in **full precision**.
+
+- CPU benchmarks:
+
+|Library                         |FUNSD (199 pages)              |CORD  (900 pages)              |
+|--------------------------------|-------------------------------|-------------------------------|
+|docTR (CPU) - v0.8.1            | ~1.29s / Page                 | ~0.60s / Page                 |
+|**OnnxTR (CPU)** - v0.1.2       | ~0.57s / Page                 | **~0.25s / Page**             |
+|**OnnxTR (CPU) 8-bit** - v0.1.2 | **~0.38s / Page**             | **~0.14s / Page**             |
+|EasyOCR (CPU) - v1.7.1          | ~1.96s / Page                 | ~1.75s / Page                 |
+|**PyTesseract (CPU)** - v0.3.10 | **~0.50s / Page**             | ~0.52s / Page                 |
+|Surya (line) (CPU) - v0.4.4     | ~48.76s / Page                | ~35.49s / Page                |
+
+- GPU benchmarks:
+
+|Library                         |FUNSD (199 pages)              |CORD  (900 pages)              |
 |--------------------------------|-------------------------------|-------------------------------|
-|FUNSD (199 pages)               | ~1.29s / Page                 | ~0.57s / Page                 |
-|CORD  (900 pages)               | ~0.60s / Page                 | ~0.25s / Page                 |
+|docTR (GPU) - v0.8.1            | ~0.07s / Page                 | ~0.05s / Page                 |
+|**docTR (GPU) float16** - v0.8.1| **~0.06s / Page**             | **~0.03s / Page**             |
+|OnnxTR (GPU) - v0.1.2           | **~0.06s / Page**             | ~0.04s / Page                 |
+|EasyOCR (GPU) - v1.7.1          | ~0.31s / Page                 | ~0.19s / Page                 |
+|Surya (GPU) float16 - v0.4.4    | ~3.70s / Page                 | ~2.81s / Page                 |
 
 ## Citation
 
 If you wish to cite please refer to the base project citation, feel free to use this [BibTeX](http://www.bibtex.org/) reference:
 
 ```bibtex
 @misc{doctr2021,
```

### Comparing `onnxtr-0.1.2/README.md` & `onnxtr-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 </p>
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
 ![Build Status](https://github.com/felixdittrich92/onnxtr/workflows/builds/badge.svg)
 [![codecov](https://codecov.io/gh/felixdittrich92/OnnxTR/graph/badge.svg?token=WVFRCQBOLI)](https://codecov.io/gh/felixdittrich92/OnnxTR)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/4fff4d764bb14fb8b4f4afeb9587231b)](https://app.codacy.com/gh/felixdittrich92/OnnxTR/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![CodeFactor](https://www.codefactor.io/repository/github/felixdittrich92/onnxtr/badge)](https://www.codefactor.io/repository/github/felixdittrich92/onnxtr)
-[![Pypi](https://img.shields.io/badge/pypi-v0.1.1-blue.svg)](https://pypi.org/project/OnnxTR/)
+[![Pypi](https://img.shields.io/badge/pypi-v0.2.0-blue.svg)](https://pypi.org/project/OnnxTR/)
 
 > :warning: Please note that this is a wrapper around the [doctr](https://github.com/mindee/doctr) library to provide a Onnx pipeline for docTR. For feature requests, which are not directly related to the Onnx pipeline, please refer to the base project.
 
 **Optical Character Recognition made seamless & accessible to anyone, powered by Onnx**
 
 What you can expect from this repository:
 
 - efficient ways to parse textual information (localize and identify each word) from your documents
-- a Onnx pipeline for docTR, a wrapper around the [doctr](https://github.com/mindee/doctr) library
+- a Onnx pipeline for docTR, a wrapper around the [doctr](https://github.com/mindee/doctr) library - no PyTorch or TensorFlow dependencies
 - more lightweight package with faster inference latency and less required resources
+- 8-Bit quantized models for faster inference on CPU
 
 ![OCR_example](https://github.com/felixdittrich92/OnnxTR/raw/main/docs/images/ocr.png)
 
 ## Installation
 
 ### Prerequisites
 
@@ -86,14 +87,17 @@
     # Additional parameters - meta information
     detect_orientation=False,  # set to `True` if the orientation of the pages should be detected (default: False)
     detect_language=False, # set to `True` if the language of the pages should be detected (default: False)
     # DocumentBuilder specific parameters
     resolve_lines=True,  # whether words should be automatically grouped into lines (default: True)
     resolve_blocks=True,  # whether lines should be automatically grouped into blocks (default: True)
     paragraph_break=0.035,  # relative length of the minimum space separating paragraphs (default: 0.035)
+    # OnnxTR specific parameters
+    # NOTE: 8-Bit quantized models are not available for FAST detection models and can in general lead to poorer accuracy
+    load_in_8_bit=False,  # set to `True` to load 8-bit quantized models instead of the full precision onces (default: False)
 )
 # PDF
 doc = DocumentFile.from_pdf("path/to/your/doc.pdf")
 # Analyze
 result = model(doc)
 # Display the result (requires matplotlib & mplcursors to be installed)
 result.show()
@@ -166,17 +170,17 @@
         [
             'db_resnet34',
             'db_resnet50',
             'db_mobilenet_v3_large',
             'linknet_resnet18',
             'linknet_resnet34',
             'linknet_resnet50',
-            'fast_tiny',
-            'fast_small',
-            'fast_base'
+            'fast_tiny',  # No 8-bit support
+            'fast_small',  # No 8-bit support
+            'fast_base'  # No 8-bit support
         ],
     'recognition archs':
         [
             'crnn_vgg16_bn',
             'crnn_mobilenet_v3_small',
             'crnn_mobilenet_v3_large',
             'sar_resnet31',
@@ -197,22 +201,44 @@
 NOTE:
 
 - `pretrained` is the default in OnnxTR, and not available as a parameter.
 - docTR specific environment variables (e.g.: DOCTR_CACHE_DIR -> ONNXTR_CACHE_DIR) needs to be replaced with `ONNXTR_` prefix.
 
 ### Benchmarks
 
-The benchmarks was measured on a `i7-14700K Intel CPU`.
+The CPU benchmarks was measured on a `i7-14700K Intel CPU`.
 
-MORE BENCHMARKS COMING SOON
+The GPU benchmarks was measured on a `RTX 4080 Nvidia GPU`.
 
-|Dataset                         |docTR (CPU) - v0.8.1           |OnnxTR (CPU) - v0.1.1          |
+Benchmarking performed on the FUNSD dataset and CORD dataset.
+
+docTR / OnnxTR models used for the benchmarks are `fast_base` (full precision) | `db_resnet50` (8-bit variant) for detection and `crnn_vgg16_bn` for recognition.
+
+The smallest combination in OnnxTR (docTR) of `db_mobilenet_v3_large` and `crnn_mobilenet_v3_small` takes as comparison `~0.17s / Page` on the FUNSD dataset and `~0.12s / Page` on the CORD dataset in **full precision**.
+
+- CPU benchmarks:
+
+|Library                         |FUNSD (199 pages)              |CORD  (900 pages)              |
+|--------------------------------|-------------------------------|-------------------------------|
+|docTR (CPU) - v0.8.1            | ~1.29s / Page                 | ~0.60s / Page                 |
+|**OnnxTR (CPU)** - v0.1.2       | ~0.57s / Page                 | **~0.25s / Page**             |
+|**OnnxTR (CPU) 8-bit** - v0.1.2 | **~0.38s / Page**             | **~0.14s / Page**             |
+|EasyOCR (CPU) - v1.7.1          | ~1.96s / Page                 | ~1.75s / Page                 |
+|**PyTesseract (CPU)** - v0.3.10 | **~0.50s / Page**             | ~0.52s / Page                 |
+|Surya (line) (CPU) - v0.4.4     | ~48.76s / Page                | ~35.49s / Page                |
+
+- GPU benchmarks:
+
+|Library                         |FUNSD (199 pages)              |CORD  (900 pages)              |
 |--------------------------------|-------------------------------|-------------------------------|
-|FUNSD (199 pages)               | ~1.29s / Page                 | ~0.57s / Page                 |
-|CORD  (900 pages)               | ~0.60s / Page                 | ~0.25s / Page                 |
+|docTR (GPU) - v0.8.1            | ~0.07s / Page                 | ~0.05s / Page                 |
+|**docTR (GPU) float16** - v0.8.1| **~0.06s / Page**             | **~0.03s / Page**             |
+|OnnxTR (GPU) - v0.1.2           | **~0.06s / Page**             | ~0.04s / Page                 |
+|EasyOCR (GPU) - v1.7.1          | ~0.31s / Page                 | ~0.19s / Page                 |
+|Surya (GPU) float16 - v0.4.4    | ~3.70s / Page                 | ~2.81s / Page                 |
 
 ## Citation
 
 If you wish to cite please refer to the base project citation, feel free to use this [BibTeX](http://www.bibtex.org/) reference:
 
 ```bibtex
 @misc{doctr2021,
```

### Comparing `onnxtr-0.1.2/onnxtr/contrib/artefacts.py` & `onnxtr-0.2.0/onnxtr/contrib/artefacts.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/contrib/base.py` & `onnxtr-0.2.0/onnxtr/contrib/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/file_utils.py` & `onnxtr-0.2.0/onnxtr/file_utils.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/io/elements.py` & `onnxtr-0.2.0/onnxtr/io/elements.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/io/html.py` & `onnxtr-0.2.0/onnxtr/io/html.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/io/image.py` & `onnxtr-0.2.0/onnxtr/io/image.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/io/pdf.py` & `onnxtr-0.2.0/onnxtr/io/pdf.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/io/reader.py` & `onnxtr-0.2.0/onnxtr/io/reader.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/_utils.py` & `onnxtr-0.2.0/onnxtr/models/_utils.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/builder.py` & `onnxtr-0.2.0/onnxtr/models/builder.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/classification/models/mobilenet.py` & `onnxtr-0.2.0/onnxtr/models/classification/models/mobilenet.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 default_cfgs: Dict[str, Dict[str, Any]] = {
     "mobilenet_v3_small_crop_orientation": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 256, 256),
         "classes": [0, -90, 180, 90],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/mobilenet_v3_small_crop_orientation-5620cf7e.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/mobilenet_v3_small_crop_orientation_static_8_bit-4cfaa621.onnx",
     },
     "mobilenet_v3_small_page_orientation": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 512, 512),
         "classes": [0, -90, 180, 90],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/mobilenet_v3_small_page_orientation-d3f76d79.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/mobilenet_v3_small_page_orientation_static_8_bit-3e5ef3dc.onnx",
     },
 }
 
 
 class MobileNetV3(Engine):
     """MobileNetV3 Onnx loader
 
@@ -60,61 +62,70 @@
     ) -> np.ndarray:
         return self.run(x)
 
 
 def _mobilenet_v3(
     arch: str,
     model_path: str,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> MobileNetV3:
+    # Patch the url
+    model_path = default_cfgs[arch]["url_8_bit"] if load_in_8_bit and "http" in model_path else model_path
     _cfg = deepcopy(default_cfgs[arch])
     return MobileNetV3(model_path, cfg=_cfg, **kwargs)
 
 
 def mobilenet_v3_small_crop_orientation(
-    model_path: str = default_cfgs["mobilenet_v3_small_crop_orientation"]["url"], **kwargs: Any
+    model_path: str = default_cfgs["mobilenet_v3_small_crop_orientation"]["url"],
+    load_in_8_bit: bool = False,
+    **kwargs: Any,
 ) -> MobileNetV3:
     """MobileNetV3-Small architecture as described in
     `"Searching for MobileNetV3",
     <https://arxiv.org/pdf/1905.02244.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import mobilenet_v3_small_crop_orientation
     >>> model = mobilenet_v3_small_crop_orientation()
     >>> input_tensor = np.random.rand((1, 3, 256, 256))
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the MobileNetV3 architecture
 
     Returns:
     -------
         MobileNetV3
     """
-    return _mobilenet_v3("mobilenet_v3_small_crop_orientation", model_path, **kwargs)
+    return _mobilenet_v3("mobilenet_v3_small_crop_orientation", model_path, load_in_8_bit, **kwargs)
 
 
 def mobilenet_v3_small_page_orientation(
-    model_path: str = default_cfgs["mobilenet_v3_small_page_orientation"]["url"], **kwargs: Any
+    model_path: str = default_cfgs["mobilenet_v3_small_page_orientation"]["url"],
+    load_in_8_bit: bool = False,
+    **kwargs: Any,
 ) -> MobileNetV3:
     """MobileNetV3-Small architecture as described in
     `"Searching for MobileNetV3",
     <https://arxiv.org/pdf/1905.02244.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import mobilenet_v3_small_page_orientation
     >>> model = mobilenet_v3_small_page_orientation()
     >>> input_tensor = np.random.rand((1, 3, 512, 512))
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the MobileNetV3 architecture
 
     Returns:
     -------
         MobileNetV3
     """
-    return _mobilenet_v3("mobilenet_v3_small_page_orientation", model_path, **kwargs)
+    return _mobilenet_v3("mobilenet_v3_small_page_orientation", model_path, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/classification/predictor/base.py` & `onnxtr-0.2.0/onnxtr/models/classification/predictor/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     """Implements an object able to detect the reading direction of a text box or a page.
     4 possible orientations: 0, 90, 180, 270 (-90) degrees counter clockwise.
 
     Args:
     ----
         pre_processor: transform inputs for easier batched model inference
         model: core classification architecture (backbone + classification head)
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
     """
 
     _children_names: List[str] = ["pre_processor", "model"]
 
     def __init__(
         self,
         pre_processor: PreProcessor,
```

### Comparing `onnxtr-0.1.2/onnxtr/models/classification/zoo.py` & `onnxtr-0.2.0/onnxtr/models/classification/zoo.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,67 +10,70 @@
 from .predictor import OrientationPredictor
 
 __all__ = ["crop_orientation_predictor", "page_orientation_predictor"]
 
 ORIENTATION_ARCHS: List[str] = ["mobilenet_v3_small_crop_orientation", "mobilenet_v3_small_page_orientation"]
 
 
-def _orientation_predictor(arch: str, **kwargs: Any) -> OrientationPredictor:
+def _orientation_predictor(arch: str, load_in_8_bit: bool = False, **kwargs: Any) -> OrientationPredictor:
     if arch not in ORIENTATION_ARCHS:
         raise ValueError(f"unknown architecture '{arch}'")
 
     # Load directly classifier from backbone
-    _model = classification.__dict__[arch]()
+    _model = classification.__dict__[arch](load_in_8_bit=load_in_8_bit)
     kwargs["mean"] = kwargs.get("mean", _model.cfg["mean"])
     kwargs["std"] = kwargs.get("std", _model.cfg["std"])
     kwargs["batch_size"] = kwargs.get("batch_size", 128 if "crop" in arch else 4)
     input_shape = _model.cfg["input_shape"][1:]
     predictor = OrientationPredictor(
-        PreProcessor(input_shape, preserve_aspect_ratio=True, symmetric_pad=True, **kwargs), _model
+        PreProcessor(input_shape, preserve_aspect_ratio=True, symmetric_pad=True, **kwargs),
+        _model,
     )
     return predictor
 
 
 def crop_orientation_predictor(
-    arch: Any = "mobilenet_v3_small_crop_orientation", **kwargs: Any
+    arch: Any = "mobilenet_v3_small_crop_orientation", load_in_8_bit: bool = False, **kwargs: Any
 ) -> OrientationPredictor:
     """Crop orientation classification architecture.
 
     >>> import numpy as np
     >>> from onnxtr.models import crop_orientation_predictor
     >>> model = crop_orientation_predictor(arch='mobilenet_v3_small_crop_orientation')
     >>> input_crop = (255 * np.random.rand(256, 256, 3)).astype(np.uint8)
     >>> out = model([input_crop])
 
     Args:
     ----
         arch: name of the architecture to use (e.g. 'mobilenet_v3_small_crop_orientation')
+        load_in_8_bit: load the 8-bit quantized version of the model
         **kwargs: keyword arguments to be passed to the OrientationPredictor
 
     Returns:
     -------
         OrientationPredictor
     """
-    return _orientation_predictor(arch, **kwargs)
+    return _orientation_predictor(arch, load_in_8_bit, **kwargs)
 
 
 def page_orientation_predictor(
-    arch: Any = "mobilenet_v3_small_page_orientation", **kwargs: Any
+    arch: Any = "mobilenet_v3_small_page_orientation", load_in_8_bit: bool = False, **kwargs: Any
 ) -> OrientationPredictor:
     """Page orientation classification architecture.
 
     >>> import numpy as np
     >>> from onnxtr.models import page_orientation_predictor
     >>> model = page_orientation_predictor(arch='mobilenet_v3_small_page_orientation')
     >>> input_page = (255 * np.random.rand(512, 512, 3)).astype(np.uint8)
     >>> out = model([input_page])
 
     Args:
     ----
         arch: name of the architecture to use (e.g. 'mobilenet_v3_small_page_orientation')
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments to be passed to the OrientationPredictor
 
     Returns:
     -------
         OrientationPredictor
     """
-    return _orientation_predictor(arch, **kwargs)
+    return _orientation_predictor(arch, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/detection/core.py` & `onnxtr-0.2.0/onnxtr/models/detection/core.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/detection/models/differentiable_binarization.py` & `onnxtr-0.2.0/onnxtr/models/detection/models/differentiable_binarization.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 
 default_cfgs: Dict[str, Dict[str, Any]] = {
     "db_resnet50": {
         "input_shape": (3, 1024, 1024),
         "mean": (0.798, 0.785, 0.772),
         "std": (0.264, 0.2749, 0.287),
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/db_resnet50-69ba0015.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/db_resnet50_static_8_bit-09a6104f.onnx",
     },
     "db_resnet34": {
         "input_shape": (3, 1024, 1024),
         "mean": (0.798, 0.785, 0.772),
         "std": (0.264, 0.2749, 0.287),
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/db_resnet34-b4873198.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/db_resnet34_static_8_bit-027e2c7f.onnx",
     },
     "db_mobilenet_v3_large": {
         "input_shape": (3, 1024, 1024),
         "mean": (0.798, 0.785, 0.772),
         "std": (0.264, 0.2749, 0.287),
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/db_mobilenet_v3_large-1866973f.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/db_mobilenet_v3_large_static_8_bit-51659bb9.onnx",
     },
 }
 
 
 class DBNet(Engine):
     """DBNet Onnx loader
 
@@ -83,77 +86,89 @@
 
         return out
 
 
 def _dbnet(
     arch: str,
     model_path: str,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> DBNet:
+    # Patch the url
+    model_path = default_cfgs[arch]["url_8_bit"] if load_in_8_bit and "http" in model_path else model_path
     # Build the model
     return DBNet(model_path, cfg=default_cfgs[arch], **kwargs)
 
 
-def db_resnet34(model_path: str = default_cfgs["db_resnet34"]["url"], **kwargs: Any) -> DBNet:
+def db_resnet34(
+    model_path: str = default_cfgs["db_resnet34"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> DBNet:
     """DBNet as described in `"Real-time Scene Text Detection with Differentiable Binarization"
     <https://arxiv.org/pdf/1911.08947.pdf>`_, using a ResNet-34 backbone.
 
     >>> import numpy as np
     >>> from onnxtr.models import db_resnet34
     >>> model = db_resnet34()
     >>> input_tensor = np.random.rand(1, 3, 1024, 1024)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the DBNet architecture
 
     Returns:
     -------
         text detection architecture
     """
-    return _dbnet("db_resnet34", model_path, **kwargs)
+    return _dbnet("db_resnet34", model_path, load_in_8_bit, **kwargs)
 
 
-def db_resnet50(model_path: str = default_cfgs["db_resnet50"]["url"], **kwargs: Any) -> DBNet:
+def db_resnet50(
+    model_path: str = default_cfgs["db_resnet50"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> DBNet:
     """DBNet as described in `"Real-time Scene Text Detection with Differentiable Binarization"
     <https://arxiv.org/pdf/1911.08947.pdf>`_, using a ResNet-50 backbone.
 
     >>> import numpy as np
     >>> from onnxtr.models import db_resnet50
     >>> model = db_resnet50()
     >>> input_tensor = np.random.rand(1, 3, 1024, 1024)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the DBNet architecture
 
     Returns:
     -------
         text detection architecture
     """
-    return _dbnet("db_resnet50", model_path, **kwargs)
+    return _dbnet("db_resnet50", model_path, load_in_8_bit, **kwargs)
 
 
-def db_mobilenet_v3_large(model_path: str = default_cfgs["db_mobilenet_v3_large"]["url"], **kwargs: Any) -> DBNet:
+def db_mobilenet_v3_large(
+    model_path: str = default_cfgs["db_mobilenet_v3_large"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> DBNet:
     """DBNet as described in `"Real-time Scene Text Detection with Differentiable Binarization"
     <https://arxiv.org/pdf/1911.08947.pdf>`_, using a MobileNet V3 Large backbone.
 
     >>> import numpy as np
     >>> from onnxtr.models import db_mobilenet_v3_large
     >>> model = db_mobilenet_v3_large()
     >>> input_tensor = np.random.rand(1, 3, 1024, 1024)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the DBNet architecture
 
     Returns:
     -------
         text detection architecture
     """
-    return _dbnet("db_mobilenet_v3_large", model_path, **kwargs)
+    return _dbnet("db_mobilenet_v3_large", model_path, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/detection/models/fast.py` & `onnxtr-0.2.0/onnxtr/models/detection/models/fast.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2021-2024, Mindee | Felix Dittrich.
 
 # This program is licensed under the Apache License 2.0.
 # See LICENSE or go to <https://opensource.org/licenses/Apache-2.0> for full license details.
 
+import logging
 from typing import Any, Dict, Optional
 
 import numpy as np
 from scipy.special import expit
 
 from ...engine import Engine
 from ..postprocessor.base import GeneralDetectionPostProcessor
@@ -84,77 +85,83 @@
 
         return out
 
 
 def _fast(
     arch: str,
     model_path: str,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> FAST:
+    if load_in_8_bit:
+        logging.warning("FAST models do not support 8-bit quantization yet. Loading full precision model...")
     # Build the model
     return FAST(model_path, cfg=default_cfgs[arch], **kwargs)
 
 
-def fast_tiny(model_path: str = default_cfgs["fast_tiny"]["url"], **kwargs: Any) -> FAST:
+def fast_tiny(model_path: str = default_cfgs["fast_tiny"]["url"], load_in_8_bit: bool = False, **kwargs: Any) -> FAST:
     """FAST as described in `"FAST: Faster Arbitrarily-Shaped Text Detector with Minimalist Kernel Representation"
     <https://arxiv.org/pdf/2111.02394.pdf>`_, using a tiny TextNet backbone.
 
     >>> import numpy as np
     >>> from onnxtr.models import fast_tiny
     >>> model = fast_tiny()
     >>> input_tensor = np.random.rand(1, 3, 1024, 1024)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the DBNet architecture
 
     Returns:
     -------
         text detection architecture
     """
-    return _fast("fast_tiny", model_path, **kwargs)
+    return _fast("fast_tiny", model_path, load_in_8_bit, **kwargs)
 
 
-def fast_small(model_path: str = default_cfgs["fast_small"]["url"], **kwargs: Any) -> FAST:
+def fast_small(model_path: str = default_cfgs["fast_small"]["url"], load_in_8_bit: bool = False, **kwargs: Any) -> FAST:
     """FAST as described in `"FAST: Faster Arbitrarily-Shaped Text Detector with Minimalist Kernel Representation"
     <https://arxiv.org/pdf/2111.02394.pdf>`_, using a small TextNet backbone.
 
     >>> import numpy as np
     >>> from onnxtr.models import fast_small
     >>> model = fast_small()
     >>> input_tensor = np.random.rand(1, 3, 1024, 1024)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the DBNet architecture
 
     Returns:
     -------
         text detection architecture
     """
-    return _fast("fast_small", model_path, **kwargs)
+    return _fast("fast_small", model_path, load_in_8_bit, **kwargs)
 
 
-def fast_base(model_path: str = default_cfgs["fast_base"]["url"], **kwargs: Any) -> FAST:
+def fast_base(model_path: str = default_cfgs["fast_base"]["url"], load_in_8_bit: bool = False, **kwargs: Any) -> FAST:
     """FAST as described in `"FAST: Faster Arbitrarily-Shaped Text Detector with Minimalist Kernel Representation"
     <https://arxiv.org/pdf/2111.02394.pdf>`_, using a base TextNet backbone.
 
     >>> import numpy as np
     >>> from onnxtr.models import fast_base
     >>> model = fast_base()
     >>> input_tensor = np.random.rand(1, 3, 1024, 1024)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the DBNet architecture
 
     Returns:
     -------
         text detection architecture
     """
-    return _fast("fast_base", model_path, **kwargs)
+    return _fast("fast_base", model_path, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/detection/models/linknet.py` & `onnxtr-0.2.0/onnxtr/models/detection/models/linknet.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 
 default_cfgs: Dict[str, Dict[str, Any]] = {
     "linknet_resnet18": {
         "input_shape": (3, 1024, 1024),
         "mean": (0.798, 0.785, 0.772),
         "std": (0.264, 0.2749, 0.287),
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/linknet_resnet18-e0e0b9dc.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/linknet_resnet18_static_8_bit-3b3a37dd.onnx",
     },
     "linknet_resnet34": {
         "input_shape": (3, 1024, 1024),
         "mean": (0.798, 0.785, 0.772),
         "std": (0.264, 0.2749, 0.287),
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/linknet_resnet34-93e39a39.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/linknet_resnet34_static_8_bit-2824329d.onnx",
     },
     "linknet_resnet50": {
         "input_shape": (3, 1024, 1024),
         "mean": (0.798, 0.785, 0.772),
         "std": (0.264, 0.2749, 0.287),
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/linknet_resnet50-15d8c4ec.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/linknet_resnet50_static_8_bit-65d6b0b8.onnx",
     },
 }
 
 
 class LinkNet(Engine):
     """LinkNet Onnx loader
 
@@ -84,77 +87,89 @@
 
         return out
 
 
 def _linknet(
     arch: str,
     model_path: str,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> LinkNet:
+    # Patch the url
+    model_path = default_cfgs[arch]["url_8_bit"] if load_in_8_bit and "http" in model_path else model_path
     # Build the model
     return LinkNet(model_path, cfg=default_cfgs[arch], **kwargs)
 
 
-def linknet_resnet18(model_path: str = default_cfgs["linknet_resnet18"]["url"], **kwargs: Any) -> LinkNet:
+def linknet_resnet18(
+    model_path: str = default_cfgs["linknet_resnet18"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> LinkNet:
     """LinkNet as described in `"LinkNet: Exploiting Encoder Representations for Efficient Semantic Segmentation"
     <https://arxiv.org/pdf/1707.03718.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import linknet_resnet18
     >>> model = linknet_resnet18()
     >>> input_tensor = np.random.rand(1, 3, 1024, 1024)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the LinkNet architecture
 
     Returns:
     -------
         text detection architecture
     """
-    return _linknet("linknet_resnet18", model_path, **kwargs)
+    return _linknet("linknet_resnet18", model_path, load_in_8_bit, **kwargs)
 
 
-def linknet_resnet34(model_path: str = default_cfgs["linknet_resnet34"]["url"], **kwargs: Any) -> LinkNet:
+def linknet_resnet34(
+    model_path: str = default_cfgs["linknet_resnet34"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> LinkNet:
     """LinkNet as described in `"LinkNet: Exploiting Encoder Representations for Efficient Semantic Segmentation"
     <https://arxiv.org/pdf/1707.03718.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import linknet_resnet34
     >>> model = linknet_resnet34()
     >>> input_tensor = np.random.rand(1, 3, 1024, 1024)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the LinkNet architecture
 
     Returns:
     -------
         text detection architecture
     """
-    return _linknet("linknet_resnet34", model_path, **kwargs)
+    return _linknet("linknet_resnet34", model_path, load_in_8_bit, **kwargs)
 
 
-def linknet_resnet50(model_path: str = default_cfgs["linknet_resnet50"]["url"], **kwargs: Any) -> LinkNet:
+def linknet_resnet50(
+    model_path: str = default_cfgs["linknet_resnet50"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> LinkNet:
     """LinkNet as described in `"LinkNet: Exploiting Encoder Representations for Efficient Semantic Segmentation"
     <https://arxiv.org/pdf/1707.03718.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import linknet_resnet50
     >>> model = linknet_resnet50()
     >>> input_tensor = np.random.rand(1, 3, 1024, 1024)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the LinkNet architecture
 
     Returns:
     -------
         text detection architecture
     """
-    return _linknet("linknet_resnet50", model_path, **kwargs)
+    return _linknet("linknet_resnet50", model_path, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/detection/postprocessor/base.py` & `onnxtr-0.2.0/onnxtr/models/detection/postprocessor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/detection/predictor/base.py` & `onnxtr-0.2.0/onnxtr/models/detection/predictor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/detection/zoo.py` & `onnxtr-0.2.0/onnxtr/models/detection/zoo.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,20 +20,22 @@
     "linknet_resnet50",
     "fast_tiny",
     "fast_small",
     "fast_base",
 ]
 
 
-def _predictor(arch: Any, assume_straight_pages: bool = True, **kwargs: Any) -> DetectionPredictor:
+def _predictor(
+    arch: Any, assume_straight_pages: bool = True, load_in_8_bit: bool = False, **kwargs: Any
+) -> DetectionPredictor:
     if isinstance(arch, str):
         if arch not in ARCHS:
             raise ValueError(f"unknown architecture '{arch}'")
 
-        _model = detection.__dict__[arch](assume_straight_pages=assume_straight_pages)
+        _model = detection.__dict__[arch](assume_straight_pages=assume_straight_pages, load_in_8_bit=load_in_8_bit)
     else:
         if not isinstance(arch, (detection.DBNet, detection.LinkNet, detection.FAST)):
             raise ValueError(f"unknown architecture: {type(arch)}")
 
         _model = arch
         _model.postprocessor.assume_straight_pages = assume_straight_pages
 
@@ -46,28 +48,30 @@
     )
     return predictor
 
 
 def detection_predictor(
     arch: Any = "fast_base",
     assume_straight_pages: bool = True,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> DetectionPredictor:
     """Text detection architecture.
 
     >>> import numpy as np
     >>> from onnxtr.models import detection_predictor
     >>> model = detection_predictor(arch='db_resnet50')
     >>> input_page = (255 * np.random.rand(600, 800, 3)).astype(np.uint8)
     >>> out = model([input_page])
 
     Args:
     ----
         arch: name of the architecture or model itself to use (e.g. 'db_resnet50')
         assume_straight_pages: If True, fit straight boxes to the page
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: optional keyword arguments passed to the architecture
 
     Returns:
     -------
         Detection predictor
     """
-    return _predictor(arch, assume_straight_pages, **kwargs)
+    return _predictor(arch, assume_straight_pages, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/engine.py` & `onnxtr-0.2.0/onnxtr/models/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,12 +39,12 @@
             inputs = shape_translate(inputs, format="BHWC")  # sanity check
         else:
             inputs = shape_translate(inputs, format="BCHW")
         if isinstance(self.fixed_batch_size, int) and self.fixed_batch_size != 0:  # dynamic batch size is a string
             inputs = np.broadcast_to(inputs, (self.fixed_batch_size, *inputs.shape))
             # combine the results
             logits = np.concatenate(
-                [self.runtime.run(self.output_name, {"input": batch})[0] for batch in inputs], axis=0
+                [self.runtime.run(self.output_name, {self.runtime_inputs.name: batch})[0] for batch in inputs], axis=0
             )
         else:
-            logits = self.runtime.run(self.output_name, {"input": inputs})[0]
+            logits = self.runtime.run(self.output_name, {self.runtime_inputs.name: inputs})[0]
         return shape_translate(logits, format="BHWC")
```

### Comparing `onnxtr-0.1.2/onnxtr/models/predictor/base.py` & `onnxtr-0.2.0/onnxtr/models/predictor/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,30 +27,34 @@
         assume_straight_pages: if True, speeds up the inference by assuming you only pass straight pages
             without rotated textual elements.
         straighten_pages: if True, estimates the page general orientation based on the median line orientation.
             Then, rotates page before passing it to the deep learning modules. The final predictions will be remapped
             accordingly. Doing so will improve performances for documents with page-uniform rotations.
         preserve_aspect_ratio: if True, resize preserving the aspect ratio (with padding)
         symmetric_pad: if True and preserve_aspect_ratio is True, pas the image symmetrically.
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword args of `DocumentBuilder`
     """
 
     crop_orientation_predictor: Optional[OrientationPredictor]
 
     def __init__(
         self,
         assume_straight_pages: bool = True,
         straighten_pages: bool = False,
         preserve_aspect_ratio: bool = True,
         symmetric_pad: bool = True,
+        load_in_8_bit: bool = False,
         **kwargs: Any,
     ) -> None:
         self.assume_straight_pages = assume_straight_pages
         self.straighten_pages = straighten_pages
-        self.crop_orientation_predictor = None if assume_straight_pages else crop_orientation_predictor()
+        self.crop_orientation_predictor = (
+            None if assume_straight_pages else crop_orientation_predictor(load_in_8_bit=load_in_8_bit)
+        )
         self.doc_builder = DocumentBuilder(**kwargs)
         self.preserve_aspect_ratio = preserve_aspect_ratio
         self.symmetric_pad = symmetric_pad
         self.hooks: List[Callable] = []
 
     @staticmethod
     def _generate_crops(
```

### Comparing `onnxtr-0.1.2/onnxtr/models/predictor/predictor.py` & `onnxtr-0.2.0/onnxtr/models/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/preprocessor/base.py` & `onnxtr-0.2.0/onnxtr/models/preprocessor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/core.py` & `onnxtr-0.2.0/onnxtr/models/recognition/core.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/models/crnn.py` & `onnxtr-0.2.0/onnxtr/models/recognition/models/crnn.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,28 +20,31 @@
 default_cfgs: Dict[str, Dict[str, Any]] = {
     "crnn_vgg16_bn": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 32, 128),
         "vocab": VOCABS["legacy_french"],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/crnn_vgg16_bn-662979cc.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/crnn_vgg16_bn_static_8_bit-bce050c7.onnx",
     },
     "crnn_mobilenet_v3_small": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 32, 128),
         "vocab": VOCABS["french"],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/crnn_mobilenet_v3_small-bded4d49.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/crnn_mobilenet_v3_small_static_8_bit-4949006f.onnx",
     },
     "crnn_mobilenet_v3_large": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 32, 128),
         "vocab": VOCABS["french"],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/crnn_mobilenet_v3_large-d42e8185.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/crnn_mobilenet_v3_large_static_8_bit-459e856d.onnx",
     },
 }
 
 
 class CRNNPostProcessor(RecognitionPostProcessor):
     """Postprocess raw prediction of the model (logits) to a list of words using CTC decoding
 
@@ -144,83 +147,95 @@
 
         return out
 
 
 def _crnn(
     arch: str,
     model_path: str,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> CRNN:
     kwargs["vocab"] = kwargs.get("vocab", default_cfgs[arch]["vocab"])
 
     _cfg = deepcopy(default_cfgs[arch])
     _cfg["vocab"] = kwargs["vocab"]
     _cfg["input_shape"] = kwargs.get("input_shape", default_cfgs[arch]["input_shape"])
+    # Patch the url
+    model_path = default_cfgs[arch]["url_8_bit"] if load_in_8_bit and "http" in model_path else model_path
 
     # Build the model
     return CRNN(model_path, cfg=_cfg, **kwargs)
 
 
-def crnn_vgg16_bn(model_path: str = default_cfgs["crnn_vgg16_bn"]["url"], **kwargs: Any) -> CRNN:
+def crnn_vgg16_bn(
+    model_path: str = default_cfgs["crnn_vgg16_bn"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> CRNN:
     """CRNN with a VGG-16 backbone as described in `"An End-to-End Trainable Neural Network for Image-based
     Sequence Recognition and Its Application to Scene Text Recognition" <https://arxiv.org/pdf/1507.05717.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import crnn_vgg16_bn
     >>> model = crnn_vgg16_bn()
     >>> input_tensor = np.random.rand(1, 3, 32, 128)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the CRNN architecture
 
     Returns:
     -------
         text recognition architecture
     """
-    return _crnn("crnn_vgg16_bn", model_path, **kwargs)
+    return _crnn("crnn_vgg16_bn", model_path, load_in_8_bit, **kwargs)
 
 
-def crnn_mobilenet_v3_small(model_path: str = default_cfgs["crnn_mobilenet_v3_small"]["url"], **kwargs: Any) -> CRNN:
+def crnn_mobilenet_v3_small(
+    model_path: str = default_cfgs["crnn_mobilenet_v3_small"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> CRNN:
     """CRNN with a MobileNet V3 Small backbone as described in `"An End-to-End Trainable Neural Network for Image-based
     Sequence Recognition and Its Application to Scene Text Recognition" <https://arxiv.org/pdf/1507.05717.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import crnn_mobilenet_v3_small
     >>> model = crnn_mobilenet_v3_small()
     >>> input_tensor = np.random.rand(1, 3, 32, 128)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the CRNN architecture
 
     Returns:
     -------
         text recognition architecture
     """
-    return _crnn("crnn_mobilenet_v3_small", model_path, **kwargs)
+    return _crnn("crnn_mobilenet_v3_small", model_path, load_in_8_bit, **kwargs)
 
 
-def crnn_mobilenet_v3_large(model_path: str = default_cfgs["crnn_mobilenet_v3_large"]["url"], **kwargs: Any) -> CRNN:
+def crnn_mobilenet_v3_large(
+    model_path: str = default_cfgs["crnn_mobilenet_v3_large"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> CRNN:
     """CRNN with a MobileNet V3 Large backbone as described in `"An End-to-End Trainable Neural Network for Image-based
     Sequence Recognition and Its Application to Scene Text Recognition" <https://arxiv.org/pdf/1507.05717.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import crnn_mobilenet_v3_large
     >>> model = crnn_mobilenet_v3_large()
     >>> input_tensor = np.random.rand(1, 3, 32, 128)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the CRNN architecture
 
     Returns:
     -------
         text recognition architecture
     """
-    return _crnn("crnn_mobilenet_v3_large", model_path, **kwargs)
+    return _crnn("crnn_mobilenet_v3_large", model_path, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/models/master.py` & `onnxtr-0.2.0/onnxtr/models/recognition/models/master.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 default_cfgs: Dict[str, Dict[str, Any]] = {
     "master": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 32, 128),
         "vocab": VOCABS["french"],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/master-b1287fcd.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/master_dynamic_8_bit-d8bd8206.onnx",
     },
 }
 
 
 class MASTER(Engine):
     """MASTER Onnx loader
 
@@ -108,38 +109,42 @@
 
         return list(zip(word_values, np.clip(probs, 0, 1).astype(float).tolist()))
 
 
 def _master(
     arch: str,
     model_path: str,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> MASTER:
     # Patch the config
     _cfg = deepcopy(default_cfgs[arch])
     _cfg["input_shape"] = kwargs.get("input_shape", _cfg["input_shape"])
     _cfg["vocab"] = kwargs.get("vocab", _cfg["vocab"])
 
     kwargs["vocab"] = _cfg["vocab"]
+    # Patch the url
+    model_path = default_cfgs[arch]["url_8_bit"] if load_in_8_bit and "http" in model_path else model_path
 
     return MASTER(model_path, cfg=_cfg, **kwargs)
 
 
-def master(model_path: str = default_cfgs["master"]["url"], **kwargs: Any) -> MASTER:
+def master(model_path: str = default_cfgs["master"]["url"], load_in_8_bit: bool = False, **kwargs: Any) -> MASTER:
     """MASTER as described in paper: <https://arxiv.org/pdf/1910.02562.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import master
     >>> model = master()
     >>> input_tensor = np.random.rand(1, 3, 32, 128)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keywoard arguments passed to the MASTER architecture
 
     Returns:
     -------
         text recognition architecture
     """
-    return _master("master", model_path, **kwargs)
+    return _master("master", model_path, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/models/parseq.py` & `onnxtr-0.2.0/onnxtr/models/recognition/models/parseq.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 default_cfgs: Dict[str, Dict[str, Any]] = {
     "parseq": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 32, 128),
         "vocab": VOCABS["french"],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/parseq-00b40714.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/parseq_dynamic_8_bit-5b04d9f7.onnx",
     },
 }
 
 
 class PARSeq(Engine):
     """PARSeq Onnx loader
 
     Args:
     ----
+        model_path: path to onnx model file
         vocab: vocabulary used for encoding
         cfg: dictionary containing information about the model
         **kwargs: additional arguments to be passed to `Engine`
     """
 
     def __init__(
         self,
@@ -95,40 +97,44 @@
 
         return list(zip(word_values, probs))
 
 
 def _parseq(
     arch: str,
     model_path: str,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> PARSeq:
     # Patch the config
     _cfg = deepcopy(default_cfgs[arch])
     _cfg["vocab"] = kwargs.get("vocab", _cfg["vocab"])
     _cfg["input_shape"] = kwargs.get("input_shape", _cfg["input_shape"])
 
     kwargs["vocab"] = _cfg["vocab"]
+    # Patch the url
+    model_path = default_cfgs[arch]["url_8_bit"] if load_in_8_bit and "http" in model_path else model_path
 
     # Build the model
     return PARSeq(model_path, cfg=_cfg, **kwargs)
 
 
-def parseq(model_path: str = default_cfgs["parseq"]["url"], **kwargs: Any) -> PARSeq:
+def parseq(model_path: str = default_cfgs["parseq"]["url"], load_in_8_bit: bool = False, **kwargs: Any) -> PARSeq:
     """PARSeq architecture from
     `"Scene Text Recognition with Permuted Autoregressive Sequence Models" <https://arxiv.org/pdf/2207.06966>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import parseq
     >>> model = parseq()
     >>> input_tensor = np.random.rand(1, 3, 32, 128)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the PARSeq architecture
 
     Returns:
     -------
         text recognition architecture
     """
-    return _parseq("parseq", model_path, **kwargs)
+    return _parseq("parseq", model_path, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/models/sar.py` & `onnxtr-0.2.0/onnxtr/models/recognition/models/sar.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 default_cfgs: Dict[str, Dict[str, Any]] = {
     "sar_resnet31": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 32, 128),
         "vocab": VOCABS["french"],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/sar_resnet31-395f8005.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/sar_resnet31_static_8_bit-c07316bc.onnx",
     },
 }
 
 
 class SAR(Engine):
     """SAR Onnx loader
 
@@ -95,40 +96,46 @@
 
         return list(zip(word_values, np.clip(probs, 0, 1).astype(float).tolist()))
 
 
 def _sar(
     arch: str,
     model_path: str,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> SAR:
     # Patch the config
     _cfg = deepcopy(default_cfgs[arch])
     _cfg["vocab"] = kwargs.get("vocab", _cfg["vocab"])
     _cfg["input_shape"] = kwargs.get("input_shape", _cfg["input_shape"])
 
     kwargs["vocab"] = _cfg["vocab"]
+    # Patch the url
+    model_path = default_cfgs[arch]["url_8_bit"] if load_in_8_bit and "http" in model_path else model_path
 
     # Build the model
     return SAR(model_path, cfg=_cfg, **kwargs)
 
 
-def sar_resnet31(model_path: str = default_cfgs["sar_resnet31"]["url"], **kwargs: Any) -> SAR:
+def sar_resnet31(
+    model_path: str = default_cfgs["sar_resnet31"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> SAR:
     """SAR with a resnet-31 feature extractor as described in `"Show, Attend and Read:A Simple and Strong
     Baseline for Irregular Text Recognition" <https://arxiv.org/pdf/1811.00751.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import sar_resnet31
     >>> model = sar_resnet31()
     >>> input_tensor = np.random.rand(1, 3, 32, 128)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: keyword arguments of the SAR architecture
 
     Returns:
     -------
         text recognition architecture
     """
-    return _sar("sar_resnet31", model_path, **kwargs)
+    return _sar("sar_resnet31", model_path, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/models/vitstr.py` & `onnxtr-0.2.0/onnxtr/models/recognition/models/vitstr.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 default_cfgs: Dict[str, Dict[str, Any]] = {
     "vitstr_small": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 32, 128),
         "vocab": VOCABS["french"],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/vitstr_small-3ff9c500.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/vitstr_small_dynamic_8_bit-bec6c796.onnx",
     },
     "vitstr_base": {
         "mean": (0.694, 0.695, 0.693),
         "std": (0.299, 0.296, 0.301),
         "input_shape": (3, 32, 128),
         "vocab": VOCABS["french"],
         "url": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.0.1/vitstr_base-ff62f5be.onnx",
+        "url_8_bit": "https://github.com/felixdittrich92/OnnxTR/releases/download/v0.1.2/vitstr_base_dynamic_8_bit-976c7cd6.onnx",
     },
 }
 
 
 class ViTSTR(Engine):
     """ViTSTR Onnx loader
 
@@ -105,62 +107,71 @@
 
         return list(zip(word_values, probs))
 
 
 def _vitstr(
     arch: str,
     model_path: str,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> ViTSTR:
     # Patch the config
     _cfg = deepcopy(default_cfgs[arch])
     _cfg["vocab"] = kwargs.get("vocab", _cfg["vocab"])
     _cfg["input_shape"] = kwargs.get("input_shape", _cfg["input_shape"])
 
     kwargs["vocab"] = _cfg["vocab"]
+    # Patch the url
+    model_path = default_cfgs[arch]["url_8_bit"] if load_in_8_bit and "http" in model_path else model_path
 
     # Build the model
     return ViTSTR(model_path, cfg=_cfg, **kwargs)
 
 
-def vitstr_small(model_path: str = default_cfgs["vitstr_small"]["url"], **kwargs: Any) -> ViTSTR:
+def vitstr_small(
+    model_path: str = default_cfgs["vitstr_small"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> ViTSTR:
     """ViTSTR-Small as described in `"Vision Transformer for Fast and Efficient Scene Text Recognition"
     <https://arxiv.org/pdf/2105.08582.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import vitstr_small
     >>> model = vitstr_small()
     >>> input_tensor = np.random.rand(1, 3, 32, 128)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
-        kwargs: keyword arguments of the ViTSTR architecture
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
+        **kwargs: keyword arguments of the ViTSTR architecture
 
     Returns:
     -------
         text recognition architecture
     """
-    return _vitstr("vitstr_small", model_path, **kwargs)
+    return _vitstr("vitstr_small", model_path, load_in_8_bit, **kwargs)
 
 
-def vitstr_base(model_path: str = default_cfgs["vitstr_base"]["url"], **kwargs: Any) -> ViTSTR:
+def vitstr_base(
+    model_path: str = default_cfgs["vitstr_base"]["url"], load_in_8_bit: bool = False, **kwargs: Any
+) -> ViTSTR:
     """ViTSTR-Base as described in `"Vision Transformer for Fast and Efficient Scene Text Recognition"
     <https://arxiv.org/pdf/2105.08582.pdf>`_.
 
     >>> import numpy as np
     >>> from onnxtr.models import vitstr_base
     >>> model = vitstr_base()
     >>> input_tensor = np.random.rand(1, 3, 32, 128)
     >>> out = model(input_tensor)
 
     Args:
     ----
         model_path: path to onnx model file, defaults to url in default_cfgs
-        kwargs: keyword arguments of the ViTSTR architecture
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
+        **kwargs: keyword arguments of the ViTSTR architecture
 
     Returns:
     -------
         text recognition architecture
     """
-    return _vitstr("vitstr_base", model_path, **kwargs)
+    return _vitstr("vitstr_base", model_path, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/predictor/_utils.py` & `onnxtr-0.2.0/onnxtr/models/recognition/predictor/_utils.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/predictor/base.py` & `onnxtr-0.2.0/onnxtr/models/recognition/predictor/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/utils.py` & `onnxtr-0.2.0/onnxtr/models/recognition/utils.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/models/recognition/zoo.py` & `onnxtr-0.2.0/onnxtr/models/recognition/zoo.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     "master",
     "vitstr_small",
     "vitstr_base",
     "parseq",
 ]
 
 
-def _predictor(arch: Any, **kwargs: Any) -> RecognitionPredictor:
+def _predictor(arch: Any, load_in_8_bit: bool = False, **kwargs: Any) -> RecognitionPredictor:
     if isinstance(arch, str):
         if arch not in ARCHS:
             raise ValueError(f"unknown architecture '{arch}'")
 
-        _model = recognition.__dict__[arch]()
+        _model = recognition.__dict__[arch](load_in_8_bit=load_in_8_bit)
     else:
         if not isinstance(
             arch, (recognition.CRNN, recognition.SAR, recognition.MASTER, recognition.ViTSTR, recognition.PARSeq)
         ):
             raise ValueError(f"unknown architecture: {type(arch)}")
         _model = arch
 
@@ -43,27 +43,30 @@
     kwargs["batch_size"] = kwargs.get("batch_size", 1024)
     input_shape = _model.cfg["input_shape"][1:]
     predictor = RecognitionPredictor(PreProcessor(input_shape, preserve_aspect_ratio=True, **kwargs), _model)
 
     return predictor
 
 
-def recognition_predictor(arch: Any = "crnn_vgg16_bn", **kwargs: Any) -> RecognitionPredictor:
+def recognition_predictor(
+    arch: Any = "crnn_vgg16_bn", load_in_8_bit: bool = False, **kwargs: Any
+) -> RecognitionPredictor:
     """Text recognition architecture.
 
     Example::
         >>> import numpy as np
         >>> from onnxtr.models import recognition_predictor
         >>> model = recognition_predictor()
         >>> input_page = (255 * np.random.rand(32, 128, 3)).astype(np.uint8)
         >>> out = model([input_page])
 
     Args:
     ----
         arch: name of the architecture or model itself to use (e.g. 'crnn_vgg16_bn')
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         **kwargs: optional parameters to be passed to the architecture
 
     Returns:
     -------
         Recognition predictor
     """
-    return _predictor(arch, **kwargs)
+    return _predictor(arch, load_in_8_bit, **kwargs)
```

### Comparing `onnxtr-0.1.2/onnxtr/models/zoo.py` & `onnxtr-0.2.0/onnxtr/models/zoo.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,29 +19,32 @@
     preserve_aspect_ratio: bool = True,
     symmetric_pad: bool = True,
     det_bs: int = 4,
     reco_bs: int = 1024,
     detect_orientation: bool = False,
     straighten_pages: bool = False,
     detect_language: bool = False,
+    load_in_8_bit: bool = False,
     **kwargs,
 ) -> OCRPredictor:
     # Detection
     det_predictor = detection_predictor(
         det_arch,
         batch_size=det_bs,
         assume_straight_pages=assume_straight_pages,
         preserve_aspect_ratio=preserve_aspect_ratio,
         symmetric_pad=symmetric_pad,
+        load_in_8_bit=load_in_8_bit,
     )
 
     # Recognition
     reco_predictor = recognition_predictor(
         reco_arch,
         batch_size=reco_bs,
+        load_in_8_bit=load_in_8_bit,
     )
 
     return OCRPredictor(
         det_predictor,
         reco_predictor,
         assume_straight_pages=assume_straight_pages,
         preserve_aspect_ratio=preserve_aspect_ratio,
@@ -59,14 +62,15 @@
     assume_straight_pages: bool = True,
     preserve_aspect_ratio: bool = True,
     symmetric_pad: bool = True,
     export_as_straight_boxes: bool = False,
     detect_orientation: bool = False,
     straighten_pages: bool = False,
     detect_language: bool = False,
+    load_in_8_bit: bool = False,
     **kwargs: Any,
 ) -> OCRPredictor:
     """End-to-end OCR architecture using one model for localization, and another for text recognition.
 
     >>> import numpy as np
     >>> from onnxtr.models import ocr_predictor
     >>> model = ocr_predictor('db_resnet50', 'crnn_vgg16_bn')
@@ -90,14 +94,15 @@
             page. Doing so will slightly deteriorate the overall latency.
         straighten_pages: if True, estimates the page general orientation
             based on the segmentation map median line orientation.
             Then, rotates page before passing it again to the deep learning detection module.
             Doing so will improve performances for documents with page-uniform rotations.
         detect_language: if True, the language prediction will be added to the predictions for each
             page. Doing so will slightly deteriorate the overall latency.
+        load_in_8_bit: whether to load the the 8-bit quantized model, defaults to False
         kwargs: keyword args of `OCRPredictor`
 
     Returns:
     -------
         OCR predictor
     """
     return _predictor(
@@ -106,9 +111,10 @@
         assume_straight_pages=assume_straight_pages,
         preserve_aspect_ratio=preserve_aspect_ratio,
         symmetric_pad=symmetric_pad,
         export_as_straight_boxes=export_as_straight_boxes,
         detect_orientation=detect_orientation,
         straighten_pages=straighten_pages,
         detect_language=detect_language,
+        load_in_8_bit=load_in_8_bit,
         **kwargs,
     )
```

### Comparing `onnxtr-0.1.2/onnxtr/transforms/base.py` & `onnxtr-0.2.0/onnxtr/transforms/base.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/utils/common_types.py` & `onnxtr-0.2.0/onnxtr/utils/common_types.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/utils/data.py` & `onnxtr-0.2.0/onnxtr/utils/data.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/utils/fonts.py` & `onnxtr-0.2.0/onnxtr/utils/fonts.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/utils/geometry.py` & `onnxtr-0.2.0/onnxtr/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/utils/multithreading.py` & `onnxtr-0.2.0/onnxtr/utils/multithreading.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/utils/reconstitution.py` & `onnxtr-0.2.0/onnxtr/utils/reconstitution.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/utils/repr.py` & `onnxtr-0.2.0/onnxtr/utils/repr.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/utils/visualization.py` & `onnxtr-0.2.0/onnxtr/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr/utils/vocabs.py` & `onnxtr-0.2.0/onnxtr/utils/vocabs.py`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr.egg-info/PKG-INFO` & `onnxtr-0.2.0/onnxtr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxtr
-Version: 0.1.2
+Version: 0.2.0
 Summary: Onnx Text Recognition (OnnxTR): docTR Onnx-Wrapper for high-performance OCR on documents.
 Author-email: Felix Dittrich <felixdittrich92@gmail.com>
 Maintainer: Felix Dittrich
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -271,25 +271,26 @@
 </p>
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
 ![Build Status](https://github.com/felixdittrich92/onnxtr/workflows/builds/badge.svg)
 [![codecov](https://codecov.io/gh/felixdittrich92/OnnxTR/graph/badge.svg?token=WVFRCQBOLI)](https://codecov.io/gh/felixdittrich92/OnnxTR)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/4fff4d764bb14fb8b4f4afeb9587231b)](https://app.codacy.com/gh/felixdittrich92/OnnxTR/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![CodeFactor](https://www.codefactor.io/repository/github/felixdittrich92/onnxtr/badge)](https://www.codefactor.io/repository/github/felixdittrich92/onnxtr)
-[![Pypi](https://img.shields.io/badge/pypi-v0.1.1-blue.svg)](https://pypi.org/project/OnnxTR/)
+[![Pypi](https://img.shields.io/badge/pypi-v0.2.0-blue.svg)](https://pypi.org/project/OnnxTR/)
 
 > :warning: Please note that this is a wrapper around the [doctr](https://github.com/mindee/doctr) library to provide a Onnx pipeline for docTR. For feature requests, which are not directly related to the Onnx pipeline, please refer to the base project.
 
 **Optical Character Recognition made seamless & accessible to anyone, powered by Onnx**
 
 What you can expect from this repository:
 
 - efficient ways to parse textual information (localize and identify each word) from your documents
-- a Onnx pipeline for docTR, a wrapper around the [doctr](https://github.com/mindee/doctr) library
+- a Onnx pipeline for docTR, a wrapper around the [doctr](https://github.com/mindee/doctr) library - no PyTorch or TensorFlow dependencies
 - more lightweight package with faster inference latency and less required resources
+- 8-Bit quantized models for faster inference on CPU
 
 ![OCR_example](https://github.com/felixdittrich92/OnnxTR/raw/main/docs/images/ocr.png)
 
 ## Installation
 
 ### Prerequisites
 
@@ -354,14 +355,17 @@
     # Additional parameters - meta information
     detect_orientation=False,  # set to `True` if the orientation of the pages should be detected (default: False)
     detect_language=False, # set to `True` if the language of the pages should be detected (default: False)
     # DocumentBuilder specific parameters
     resolve_lines=True,  # whether words should be automatically grouped into lines (default: True)
     resolve_blocks=True,  # whether lines should be automatically grouped into blocks (default: True)
     paragraph_break=0.035,  # relative length of the minimum space separating paragraphs (default: 0.035)
+    # OnnxTR specific parameters
+    # NOTE: 8-Bit quantized models are not available for FAST detection models and can in general lead to poorer accuracy
+    load_in_8_bit=False,  # set to `True` to load 8-bit quantized models instead of the full precision onces (default: False)
 )
 # PDF
 doc = DocumentFile.from_pdf("path/to/your/doc.pdf")
 # Analyze
 result = model(doc)
 # Display the result (requires matplotlib & mplcursors to be installed)
 result.show()
@@ -434,17 +438,17 @@
         [
             'db_resnet34',
             'db_resnet50',
             'db_mobilenet_v3_large',
             'linknet_resnet18',
             'linknet_resnet34',
             'linknet_resnet50',
-            'fast_tiny',
-            'fast_small',
-            'fast_base'
+            'fast_tiny',  # No 8-bit support
+            'fast_small',  # No 8-bit support
+            'fast_base'  # No 8-bit support
         ],
     'recognition archs':
         [
             'crnn_vgg16_bn',
             'crnn_mobilenet_v3_small',
             'crnn_mobilenet_v3_large',
             'sar_resnet31',
@@ -465,22 +469,44 @@
 NOTE:
 
 - `pretrained` is the default in OnnxTR, and not available as a parameter.
 - docTR specific environment variables (e.g.: DOCTR_CACHE_DIR -> ONNXTR_CACHE_DIR) needs to be replaced with `ONNXTR_` prefix.
 
 ### Benchmarks
 
-The benchmarks was measured on a `i7-14700K Intel CPU`.
+The CPU benchmarks was measured on a `i7-14700K Intel CPU`.
 
-MORE BENCHMARKS COMING SOON
+The GPU benchmarks was measured on a `RTX 4080 Nvidia GPU`.
 
-|Dataset                         |docTR (CPU) - v0.8.1           |OnnxTR (CPU) - v0.1.1          |
+Benchmarking performed on the FUNSD dataset and CORD dataset.
+
+docTR / OnnxTR models used for the benchmarks are `fast_base` (full precision) | `db_resnet50` (8-bit variant) for detection and `crnn_vgg16_bn` for recognition.
+
+The smallest combination in OnnxTR (docTR) of `db_mobilenet_v3_large` and `crnn_mobilenet_v3_small` takes as comparison `~0.17s / Page` on the FUNSD dataset and `~0.12s / Page` on the CORD dataset in **full precision**.
+
+- CPU benchmarks:
+
+|Library                         |FUNSD (199 pages)              |CORD  (900 pages)              |
+|--------------------------------|-------------------------------|-------------------------------|
+|docTR (CPU) - v0.8.1            | ~1.29s / Page                 | ~0.60s / Page                 |
+|**OnnxTR (CPU)** - v0.1.2       | ~0.57s / Page                 | **~0.25s / Page**             |
+|**OnnxTR (CPU) 8-bit** - v0.1.2 | **~0.38s / Page**             | **~0.14s / Page**             |
+|EasyOCR (CPU) - v1.7.1          | ~1.96s / Page                 | ~1.75s / Page                 |
+|**PyTesseract (CPU)** - v0.3.10 | **~0.50s / Page**             | ~0.52s / Page                 |
+|Surya (line) (CPU) - v0.4.4     | ~48.76s / Page                | ~35.49s / Page                |
+
+- GPU benchmarks:
+
+|Library                         |FUNSD (199 pages)              |CORD  (900 pages)              |
 |--------------------------------|-------------------------------|-------------------------------|
-|FUNSD (199 pages)               | ~1.29s / Page                 | ~0.57s / Page                 |
-|CORD  (900 pages)               | ~0.60s / Page                 | ~0.25s / Page                 |
+|docTR (GPU) - v0.8.1            | ~0.07s / Page                 | ~0.05s / Page                 |
+|**docTR (GPU) float16** - v0.8.1| **~0.06s / Page**             | **~0.03s / Page**             |
+|OnnxTR (GPU) - v0.1.2           | **~0.06s / Page**             | ~0.04s / Page                 |
+|EasyOCR (GPU) - v1.7.1          | ~0.31s / Page                 | ~0.19s / Page                 |
+|Surya (GPU) float16 - v0.4.4    | ~3.70s / Page                 | ~2.81s / Page                 |
 
 ## Citation
 
 If you wish to cite please refer to the base project citation, feel free to use this [BibTeX](http://www.bibtex.org/) reference:
 
 ```bibtex
 @misc{doctr2021,
```

### Comparing `onnxtr-0.1.2/onnxtr.egg-info/SOURCES.txt` & `onnxtr-0.2.0/onnxtr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/onnxtr.egg-info/requires.txt` & `onnxtr-0.2.0/onnxtr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `onnxtr-0.1.2/pyproject.toml` & `onnxtr-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 tracker = "https://github.com/felixdittrich92/OnnxTR/issues"
 changelog = "https://github.com/felixdittrich92/OnnxTR/releases"
 
 [tool.setuptools]
 zip-safe = true
 
 [tool.setuptools.packages.find]
-exclude = ["tests*"]
+exclude = ["tests*", "scripts*"]
 
 [tool.mypy]
 files = "onnxtr/"
 show_error_codes = true
 pretty = true
 warn_unused_ignores = true
 warn_redundant_casts = true
@@ -146,14 +146,15 @@
 [tool.ruff.lint.isort]
 known-first-party = ["onnxtr", "utils"]
 known-third-party = ["onnxruntime", "cv2"]
 
 [tool.ruff.lint.per-file-ignores]
 "onnxtr/models/**.py" = ["N806", "F841"]
 "tests/**.py" = ["D"]
+"scripts/**.py" = ["D"]
 ".github/**.py" = ["D"]
 
 
 [tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.coverage.run]
```

### Comparing `onnxtr-0.1.2/setup.py` & `onnxtr-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 from pathlib import Path
 
 from setuptools import setup
 
 PKG_NAME = "onnxtr"
-VERSION = os.getenv("BUILD_VERSION", "0.1.2a0")
+VERSION = os.getenv("BUILD_VERSION", "0.2.0a0")
 
 
 if __name__ == "__main__":
     print(f"Building wheel {PKG_NAME}-{VERSION}")
 
     # Dynamically set the __version__ attribute
     cwd = Path(__file__).parent.absolute()
```

