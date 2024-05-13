# Comparing `tmp/PyStratum-Common-1.1.1.tar.gz` & `tmp/pystratum_common-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyStratum-Common-1.1.1.tar", last modified: Sun Jan 30 12:41:00 2022, max compression
+gzip compressed data, was "pystratum_common-2.0.0.tar", last modified: Mon May 13 08:22:33 2024, max compression
```

## Comparing `PyStratum-Common-1.1.1.tar` & `pystratum_common-2.0.0.tar`

### file list

```diff
@@ -1,45 +1,108 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-01-30 12:41:00.247277 PyStratum-Common-1.1.1/
--rw-rw-r--   0 water     (1000) water     (1000)     4602 2022-01-30 12:41:00.247277 PyStratum-Common-1.1.1/PKG-INFO
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-01-30 12:41:00.245277 PyStratum-Common-1.1.1/PyStratum_Common.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)     4602 2022-01-30 12:41:00.000000 PyStratum-Common-1.1.1/PyStratum_Common.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)     1424 2022-01-30 12:41:00.000000 PyStratum-Common-1.1.1/PyStratum_Common.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2022-01-30 12:41:00.000000 PyStratum-Common-1.1.1/PyStratum_Common.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)       28 2022-01-30 12:41:00.000000 PyStratum-Common-1.1.1/PyStratum_Common.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       17 2022-01-30 12:41:00.000000 PyStratum-Common-1.1.1/PyStratum_Common.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)     3613 2020-10-17 07:34:51.000000 PyStratum-Common-1.1.1/README.rst
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-01-30 12:41:00.245277 PyStratum-Common-1.1.1/pystratum_common/
--rw-rw-r--   0 water     (1000) water     (1000)     5768 2020-10-17 07:44:02.000000 PyStratum-Common-1.1.1/pystratum_common/ConstantClass.py
--rw-rw-r--   0 water     (1000) water     (1000)     5520 2020-10-15 20:23:27.000000 PyStratum-Common-1.1.1/pystratum_common/DocBlockReflection.py
--rw-rw-r--   0 water     (1000) water     (1000)     1311 2020-10-16 07:10:32.000000 PyStratum-Common-1.1.1/pystratum_common/MetadataDataLayer.py
--rw-rw-r--   0 water     (1000) water     (1000)     1872 2020-11-08 10:37:39.000000 PyStratum-Common-1.1.1/pystratum_common/Util.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-16 08:32:08.000000 PyStratum-Common-1.1.1/pystratum_common/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-01-30 12:41:00.245277 PyStratum-Common-1.1.1/pystratum_common/backend/
--rw-rw-r--   0 water     (1000) water     (1000)     7431 2020-10-17 06:42:54.000000 PyStratum-Common-1.1.1/pystratum_common/backend/CommonConstantWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)    15107 2020-10-17 05:00:17.000000 PyStratum-Common-1.1.1/pystratum_common/backend/CommonRoutineLoaderWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)     6523 2020-10-17 07:04:55.000000 PyStratum-Common-1.1.1/pystratum_common/backend/CommonRoutineWrapperGeneratorWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-16 08:31:55.000000 PyStratum-Common-1.1.1/pystratum_common/backend/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-01-30 12:41:00.246277 PyStratum-Common-1.1.1/pystratum_common/exception/
--rw-rw-r--   0 water     (1000) water     (1000)      260 2020-10-15 19:51:10.000000 PyStratum-Common-1.1.1/pystratum_common/exception/LoaderException.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-15 16:55:08.000000 PyStratum-Common-1.1.1/pystratum_common/exception/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-01-30 12:41:00.246277 PyStratum-Common-1.1.1/pystratum_common/helper/
--rw-rw-r--   0 water     (1000) water     (1000)     1220 2020-10-17 07:04:55.000000 PyStratum-Common-1.1.1/pystratum_common/helper/DataTypeHelper.py
--rw-rw-r--   0 water     (1000) water     (1000)    26473 2022-01-30 12:32:31.000000 PyStratum-Common-1.1.1/pystratum_common/helper/RoutineLoaderHelper.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-16 08:31:55.000000 PyStratum-Common-1.1.1/pystratum_common/helper/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2022-01-30 12:41:00.247277 PyStratum-Common-1.1.1/pystratum_common/wrapper/
--rw-rw-r--   0 water     (1000) water     (1000)     2122 2020-10-17 07:36:19.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/BulkWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      911 2020-10-16 09:42:34.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/FunctionsWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      934 2020-10-16 09:42:34.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/LogWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      979 2020-10-16 09:42:34.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/MultiWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      932 2020-10-16 09:42:34.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/NoneWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      952 2020-10-16 09:42:34.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/Row0Wrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      942 2020-10-15 22:25:37.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/Row1Wrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)     3256 2020-10-17 07:04:55.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/RowsWithIndexWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)     3267 2020-10-17 07:04:55.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/RowsWithKeyWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      978 2020-10-16 09:42:34.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/RowsWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      964 2020-10-16 09:42:34.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/Singleton0Wrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      959 2020-10-16 09:42:34.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/Singleton1Wrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)      955 2020-10-16 09:42:34.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/TableWrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)     9640 2020-10-17 07:04:55.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/Wrapper.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-15 16:55:08.000000 PyStratum-Common-1.1.1/pystratum_common/wrapper/__init__.py
--rw-rw-r--   0 water     (1000) water     (1000)       38 2022-01-30 12:41:00.247277 PyStratum-Common-1.1.1/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)     1215 2022-01-30 12:40:57.000000 PyStratum-Common-1.1.1/setup.py
+-rw-r--r--   0        0        0     1091 2020-10-15 19:51:10.000000 pystratum_common-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3590 2024-05-13 08:15:59.064665 pystratum_common-2.0.0/README.rst
+-rw-r--r--   0        0        0     1111 2024-05-13 08:22:33.181330 pystratum_common-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5586 2024-05-13 05:53:40.903728 pystratum_common-2.0.0/pystratum_common/ConstantClass.py
+-rw-r--r--   0        0        0     5421 2024-05-12 09:43:16.589780 pystratum_common-2.0.0/pystratum_common/DocBlockReflection.py
+-rw-r--r--   0        0        0     1280 2024-05-13 05:53:40.916728 pystratum_common-2.0.0/pystratum_common/MetadataDataLayer.py
+-rw-r--r--   0        0        0     1842 2024-05-13 06:04:41.988038 pystratum_common-2.0.0/pystratum_common/Util.py
+-rw-r--r--   0        0        0        0 2020-10-16 08:32:08.000000 pystratum_common-2.0.0/pystratum_common/__init__.py
+-rw-r--r--   0        0        0     7422 2024-05-13 05:54:11.972400 pystratum_common-2.0.0/pystratum_common/backend/CommonConstantWorker.py
+-rw-r--r--   0        0        0    14998 2024-05-13 05:54:11.969400 pystratum_common-2.0.0/pystratum_common/backend/CommonRoutineLoaderWorker.py
+-rw-r--r--   0        0        0     6417 2024-05-13 05:54:11.966400 pystratum_common-2.0.0/pystratum_common/backend/CommonRoutineWrapperGeneratorWorker.py
+-rw-r--r--   0        0        0        0 2020-10-16 08:31:55.000000 pystratum_common-2.0.0/pystratum_common/backend/__init__.py
+-rw-r--r--   0        0        0      260 2020-10-15 19:51:10.000000 pystratum_common-2.0.0/pystratum_common/exception/LoaderException.py
+-rw-r--r--   0        0        0        0 2020-10-15 16:55:08.000000 pystratum_common-2.0.0/pystratum_common/exception/__init__.py
+-rw-r--r--   0        0        0     1176 2024-05-13 06:04:41.991038 pystratum_common-2.0.0/pystratum_common/helper/DataTypeHelper.py
+-rw-r--r--   0        0        0    26137 2024-05-13 06:04:41.882036 pystratum_common-2.0.0/pystratum_common/helper/RoutineLoaderHelper.py
+-rw-r--r--   0        0        0        0 2020-10-16 08:31:55.000000 pystratum_common-2.0.0/pystratum_common/helper/__init__.py
+-rw-r--r--   0        0        0     2041 2024-05-12 09:43:16.660782 pystratum_common-2.0.0/pystratum_common/wrapper/BulkWrapper.py
+-rw-r--r--   0        0        0      868 2024-05-12 09:43:16.594780 pystratum_common-2.0.0/pystratum_common/wrapper/FunctionsWrapper.py
+-rw-r--r--   0        0        0      891 2024-05-12 09:43:16.665782 pystratum_common-2.0.0/pystratum_common/wrapper/LogWrapper.py
+-rw-r--r--   0        0        0      936 2024-05-12 09:43:16.693782 pystratum_common-2.0.0/pystratum_common/wrapper/MultiWrapper.py
+-rw-r--r--   0        0        0      889 2024-05-12 09:43:16.603781 pystratum_common-2.0.0/pystratum_common/wrapper/NoneWrapper.py
+-rw-r--r--   0        0        0      909 2024-05-12 09:43:16.656782 pystratum_common-2.0.0/pystratum_common/wrapper/Row0Wrapper.py
+-rw-r--r--   0        0        0      899 2024-05-12 09:43:16.641781 pystratum_common-2.0.0/pystratum_common/wrapper/Row1Wrapper.py
+-rw-r--r--   0        0        0     3205 2024-05-12 09:43:16.636781 pystratum_common-2.0.0/pystratum_common/wrapper/RowsWithIndexWrapper.py
+-rw-r--r--   0        0        0     3216 2024-05-12 09:43:16.686782 pystratum_common-2.0.0/pystratum_common/wrapper/RowsWithKeyWrapper.py
+-rw-r--r--   0        0        0      935 2024-05-12 09:43:16.645781 pystratum_common-2.0.0/pystratum_common/wrapper/RowsWrapper.py
+-rw-r--r--   0        0        0      921 2024-05-12 09:43:16.695783 pystratum_common-2.0.0/pystratum_common/wrapper/Singleton0Wrapper.py
+-rw-r--r--   0        0        0      916 2024-05-12 09:43:16.670782 pystratum_common-2.0.0/pystratum_common/wrapper/Singleton1Wrapper.py
+-rw-r--r--   0        0        0      912 2024-05-12 09:43:16.576780 pystratum_common-2.0.0/pystratum_common/wrapper/TableWrapper.py
+-rw-r--r--   0        0        0     9533 2024-05-13 06:04:41.984038 pystratum_common-2.0.0/pystratum_common/wrapper/Wrapper.py
+-rw-r--r--   0        0        0        0 2020-10-15 16:55:08.000000 pystratum_common-2.0.0/pystratum_common/wrapper/__init__.py
+-rw-r--r--   0        0        0     6258 2020-10-17 07:29:36.000000 pystratum_common-2.0.0/test/DocBlockReflectionTest.py
+-rw-r--r--   0        0        0        0 2020-10-17 07:29:58.000000 pystratum_common-2.0.0/test/__init__.py
+-rw-r--r--   0        0        0    58078 2024-05-13 07:13:04.281699 pystratum_common-2.0.0/test/coverage.xml
+-rw-r--r--   0        0        0    33868 2024-05-13 06:49:50.185761 pystratum_common-2.0.0/test/html/class_index.html
+-rw-r--r--   0        0        0    18620 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/coverage_html.js
+-rw-r--r--   0        0        0    24699 2024-05-13 06:49:50.145760 pystratum_common-2.0.0/test/html/coverage_html_cb_da166b87.js
+-rw-r--r--   0        0        0     1732 2024-05-13 06:49:50.145760 pystratum_common-2.0.0/test/html/favicon_32_cb_58284776.png
+-rw-r--r--   0        0        0   105487 2024-05-13 06:49:50.183761 pystratum_common-2.0.0/test/html/function_index.html
+-rw-r--r--   0        0        0    15886 2024-05-13 06:49:50.157761 pystratum_common-2.0.0/test/html/index.html
+-rw-r--r--   0        0        0      731 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/jquery.ba-throttle-debounce.min.js
+-rw-r--r--   0        0        0     3065 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/jquery.hotkeys.js
+-rw-r--r--   0        0        0     1502 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/jquery.isonscreen.js
+-rw-r--r--   0        0        0    95785 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/jquery.min.js
+-rw-r--r--   0        0        0    12795 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/jquery.tablesorter.min.js
+-rw-r--r--   0        0        0      112 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/keybd_closed.png
+-rw-r--r--   0        0        0     9004 2024-05-13 06:49:50.145760 pystratum_common-2.0.0/test/html/keybd_closed_cb_ce680311.png
+-rw-r--r--   0        0        0      112 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/keybd_open.png
+-rw-r--r--   0        0        0    45663 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_ConstantClass_py.html
+-rw-r--r--   0        0        0    47857 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_DocBlockReflection_py.html
+-rw-r--r--   0        0        0    11969 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_MetadataDataLayer_py.html
+-rw-r--r--   0        0        0    13750 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_Util_py.html
+-rw-r--r--   0        0        0     2617 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common___init___py.html
+-rw-r--r--   0        0        0    53165 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_backend_CommonConstantWorker_py.html
+-rw-r--r--   0        0        0   104377 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_backend_CommonRoutineLoaderWorker_py.html
+-rw-r--r--   0        0        0    49452 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_backend_CommonRoutineWrapperGeneratorWorker_py.html
+-rw-r--r--   0        0        0     2633 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_backend___init___py.html
+-rw-r--r--   0        0        0     4072 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_exception_LoaderException_py.html
+-rw-r--r--   0        0        0     2637 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_exception___init___py.html
+-rw-r--r--   0        0        0    15932 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_BulkWrapper_py.html
+-rw-r--r--   0        0        0     8640 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_FunctionsWrapper_py.html
+-rw-r--r--   0        0        0     8651 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_LogWrapper_py.html
+-rw-r--r--   0        0        0     8700 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_MultiWrapper_py.html
+-rw-r--r--   0        0        0     8651 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_NoneWrapper_py.html
+-rw-r--r--   0        0        0     8671 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_Row0Wrapper_py.html
+-rw-r--r--   0        0        0     8661 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_Row1Wrapper_py.html
+-rw-r--r--   0        0        0    28173 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_RowsWithIndexWrapper_py.html
+-rw-r--r--   0        0        0    28120 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_RowsWithKeyWrapper_py.html
+-rw-r--r--   0        0        0     8697 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_RowsWrapper_py.html
+-rw-r--r--   0        0        0     8695 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_Singleton0Wrapper_py.html
+-rw-r--r--   0        0        0     8690 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_Singleton1Wrapper_py.html
+-rw-r--r--   0        0        0     8676 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_TableWrapper_py.html
+-rw-r--r--   0        0        0    66542 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper_Wrapper_py.html
+-rw-r--r--   0        0        0     2633 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/pystratum_common_wrapper___init___py.html
+-rw-r--r--   0        0        0    10566 2024-05-13 06:49:50.158761 pystratum_common-2.0.0/test/html/status.json
+-rw-r--r--   0        0        0    11680 2020-10-17 08:18:30.000000 pystratum_common-2.0.0/test/html/style.css
+-rw-r--r--   0        0        0    14077 2024-05-13 06:49:50.145760 pystratum_common-2.0.0/test/html/style_cb_8e611ae1.css
+-rw-r--r--   0        0        0    46215 2024-05-13 06:46:43.349648 pystratum_common-2.0.0/test/html/z_0e7e14cddbb2a3de_ConstantClass_py.html
+-rw-r--r--   0        0        0    49094 2024-05-13 06:46:43.359648 pystratum_common-2.0.0/test/html/z_0e7e14cddbb2a3de_DocBlockReflection_py.html
+-rw-r--r--   0        0        0    14119 2024-05-13 06:46:43.361648 pystratum_common-2.0.0/test/html/z_0e7e14cddbb2a3de_MetadataDataLayer_py.html
+-rw-r--r--   0        0        0    15909 2024-05-13 06:46:43.363648 pystratum_common-2.0.0/test/html/z_0e7e14cddbb2a3de_Util_py.html
+-rw-r--r--   0        0        0     4802 2024-05-13 06:46:43.364648 pystratum_common-2.0.0/test/html/z_0e7e14cddbb2a3de___init___py.html
+-rw-r--r--   0        0        0     6241 2024-05-13 06:46:43.389649 pystratum_common-2.0.0/test/html/z_7c672fe110513005_LoaderException_py.html
+-rw-r--r--   0        0        0     4832 2024-05-13 06:46:43.390648 pystratum_common-2.0.0/test/html/z_7c672fe110513005___init___py.html
+-rw-r--r--   0        0        0    55291 2024-05-13 06:46:43.370648 pystratum_common-2.0.0/test/html/z_a1797a3a92e81fc2_CommonConstantWorker_py.html
+-rw-r--r--   0        0        0   105918 2024-05-13 06:46:43.382648 pystratum_common-2.0.0/test/html/z_a1797a3a92e81fc2_CommonRoutineLoaderWorker_py.html
+-rw-r--r--   0        0        0    50760 2024-05-13 06:46:43.387648 pystratum_common-2.0.0/test/html/z_a1797a3a92e81fc2_CommonRoutineWrapperGeneratorWorker_py.html
+-rw-r--r--   0        0        0     4870 2024-05-13 06:46:43.388649 pystratum_common-2.0.0/test/html/z_a1797a3a92e81fc2___init___py.html
+-rw-r--r--   0        0        0    17193 2024-05-13 06:46:43.416649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_BulkWrapper_py.html
+-rw-r--r--   0        0        0    10214 2024-05-13 06:46:43.417649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_FunctionsWrapper_py.html
+-rw-r--r--   0        0        0    10239 2024-05-13 06:46:43.418649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_LogWrapper_py.html
+-rw-r--r--   0        0        0    10274 2024-05-13 06:46:43.419649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_MultiWrapper_py.html
+-rw-r--r--   0        0        0    10229 2024-05-13 06:46:43.421649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_NoneWrapper_py.html
+-rw-r--r--   0        0        0    10247 2024-05-13 06:46:43.422649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_Row0Wrapper_py.html
+-rw-r--r--   0        0        0    10255 2024-05-13 06:46:43.423649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_Row1Wrapper_py.html
+-rw-r--r--   0        0        0    29755 2024-05-13 06:46:43.427649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_RowsWithIndexWrapper_py.html
+-rw-r--r--   0        0        0    29706 2024-05-13 06:46:43.430649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_RowsWithKeyWrapper_py.html
+-rw-r--r--   0        0        0    10299 2024-05-13 06:46:43.432649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_RowsWrapper_py.html
+-rw-r--r--   0        0        0    10283 2024-05-13 06:46:43.433649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_Singleton0Wrapper_py.html
+-rw-r--r--   0        0        0    10280 2024-05-13 06:46:43.434650 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_Singleton1Wrapper_py.html
+-rw-r--r--   0        0        0    10256 2024-05-13 06:46:43.435649 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_TableWrapper_py.html
+-rw-r--r--   0        0        0    67558 2024-05-13 06:46:43.443650 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5_Wrapper_py.html
+-rw-r--r--   0        0        0     4750 2024-05-13 06:46:43.443650 pystratum_common-2.0.0/test/html/z_c5d89eced4b971c5___init___py.html
+-rw-r--r--   0        0        0    11918 2024-05-13 06:46:43.391649 pystratum_common-2.0.0/test/html/z_fb06527ccf23efd5_DataTypeHelper_py.html
+-rw-r--r--   0        0        0   182522 2024-05-13 06:46:43.412649 pystratum_common-2.0.0/test/html/z_fb06527ccf23efd5_RoutineLoaderHelper_py.html
+-rw-r--r--   0        0        0     4828 2024-05-13 06:46:43.414649 pystratum_common-2.0.0/test/html/z_fb06527ccf23efd5___init___py.html
+-rw-r--r--   0        0        0     4580 1970-01-01 00:00:00.000000 pystratum_common-2.0.0/PKG-INFO
```

### Comparing `PyStratum-Common-1.1.1/README.rst` & `pystratum_common-2.0.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-PyStratum Common
-================
-Common parts shared between backends for database systems.
-
-+-----------------------------------------------------------------------------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------+
-| Social                                                                                                                      | Release                                                   | Tests                                                                                                  | Code                                                                                                        |
-+=============================================================================================================================+===========================================================+========================================================================================================+=============================================================================================================+
-| .. image:: https://badges.gitter.im/SetBased/py-stratum.svg                                                                 | .. image:: https://badge.fury.io/py/PyStratum-Common.svg  | .. image:: https://travis-ci.org/DatabaseStratum/py-stratum-common.svg?branch=master                   | .. image:: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-common/badges/quality-score.png?b=master |
-|   :target: https://gitter.im/SetBased/py-stratum?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge  |   :target: https://badge.fury.io/py/PyStratum-Common      |   :target: https://travis-ci.org/DatabaseStratum/py-stratum-common                                     |   :target: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-common/?branch=master                    |
-|                                                                                                                             |                                                           | .. image:: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-common/badges/coverage.png?b=master |                                                                                                             |
-|                                                                                                                             |                                                           |   :target: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-common/?branch=master               |                                                                                                             |
-+-----------------------------------------------------------------------------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------+
-
-Overview
-========
-PyStratum is a tool and library for loading and invoking stored procedures from Python code.
-
-The documentation of PyStratum is available at https://stratum.readthedocs.io/.
-
-License
-=======
-
-This project is licensed under the terms of the MIT license.
+PyStratum Common
+================
+Common parts shared between backends for database systems.
+
++-----------------------------------------------------------------------------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------+
+| Social                                                                                                                      | Release                                                   | Tests                                                                                                  | Code                                                                                                        |
++=============================================================================================================================+===========================================================+========================================================================================================+=============================================================================================================+
+| .. image:: https://badges.gitter.im/SetBased/py-stratum.svg                                                                 | .. image:: https://badge.fury.io/py/PyStratum-Common.svg  | .. image:: https://github.com/DatabaseStratum/py-stratum-common/actions/workflows/unit.yml/badge.svg   | .. image:: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-common/badges/quality-score.png?b=master |
+|   :target: https://gitter.im/SetBased/py-stratum?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge  |   :target: https://badge.fury.io/py/PyStratum-Common      |   :target: https://github.com/DatabaseStratum/py-stratum-common/actions/workflows/unit.yml             |   :target: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-common/?branch=master                    |
+|                                                                                                                             |                                                           | .. image:: https://codecov.io/gh/DatabaseStratum/py-stratum-common/branch/master/graph/badge.svg       |                                                                                                             |
+|                                                                                                                             |                                                           |   :target: https://codecov.io/gh/DatabaseStratum/py-stratum-common                                     |                                                                                                             |
++-----------------------------------------------------------------------------------------------------------------------------+-----------------------------------------------------------+--------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------+
+
+Overview
+========
+PyStratum is a tool and library for loading and invoking stored procedures from Python code.
+
+The documentation of PyStratum is available at https://stratum.readthedocs.io/.
+
+License
+=======
+
+This project is licensed under the terms of the MIT license.
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/ConstantClass.py` & `pystratum_common-2.0.0/pystratum_common/ConstantClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import importlib
 import inspect
 import re
 from typing import Any, Dict, List, Union
 
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 
 class ConstantClass:
     """
     Helper class for loading and modifying the class that acts like a namespace for constants.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, class_name: str, io: StratumStyle):
+    def __init__(self, class_name: str, io: StratumIO):
         """
         Object constructor.
 
-        :param str class_name: The name of class that acts like a namespace for constants.
-        :param PyStratumStyle io: The output decorator.
+        :param class_name: The name of class that acts like a namespace for constants.
+        :param io: The output decorator.
         """
         self.__class_name: str = class_name
         """
         The name of class that acts like a namespace for constants.
         """
 
         self.__module = None
@@ -32,15 +32,15 @@
         """
 
         self.__annotation: str = '# PyStratum'
         """
         The comment after which the auto generated constants must be inserted.
         """
 
-        self._io: StratumStyle = io
+        self._io: StratumIO = io
         """
         The output decorator.
         """
 
         self.__load()
 
     # ------------------------------------------------------------------------------------------------------------------
@@ -58,41 +58,35 @@
 
         self.__module = modules[-2]
 
     # ------------------------------------------------------------------------------------------------------------------
     def file_name(self) -> str:
         """
         Returns the filename of the module with the class that acts like a namespace for constants.
-
-        :rtype: str
         """
         return inspect.getfile(self.__module)
 
     # ------------------------------------------------------------------------------------------------------------------
     def source(self) -> str:
         """
         Returns the source of the module with the class that acts like a namespace for constants.
-
-        :rtype: str
         """
         return inspect.getsource(self.__module)
 
     # ------------------------------------------------------------------------------------------------------------------
     def reload(self) -> None:
         """
         Reloads the module with the class that acts like a namespace for constants.
         """
         importlib.reload(self.__module)
 
     # ------------------------------------------------------------------------------------------------------------------
     def constants(self) -> Dict[str, Any]:
         """
         Gets the constants from the class that acts like a namespace for constants.
-
-        :rtype: dict<str,*>
         """
         ret = {}
 
         name = self.__class_name.split('.')[-1]
         constant_class = getattr(self.__module, name)
         for name, value in constant_class.__dict__.items():
             if re.match(r'^[A-Z][A-Z0-9_]*$', name):
@@ -105,17 +99,15 @@
         """
         Extracts the following info from the source of the module with the class that acts like a namespace for
         constants:
         * Start line with constants
         * Last line with constants
         * Indent for constants
 
-        :param list[str] lines: The source of the module with the class that acts like a namespace for constants.
-
-        :rtype: dict<str,int|str>
+        :param lines: The source of the module with the class that acts like a namespace for constants.
         """
         ret = {'start_line': 0,
                'last_line':  0,
                'indent':     ''}
 
         mode = 1
         count = 0
@@ -145,17 +137,15 @@
         return ret
 
     # ------------------------------------------------------------------------------------------------------------------
     def source_with_constants(self, constants: Dict[str, int]) -> str:
         """
         Returns the source of the module with the class that acts like a namespace for constants with new constants.
 
-        :param dict[str,int] constants: The new constants.
-
-        :rtype: str
+        :param constants: The new constants.
         """
         old_lines = self.source().split("\n")
         info = self.__extract_info(old_lines)
 
         new_lines = old_lines[0:info['start_line']]
 
         for constant, value in sorted(constants.items()):
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/DocBlockReflection.py` & `pystratum_common-2.0.0/pystratum_common/DocBlockReflection.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __init__(self, comment: List[str]):
         """
         Object constructor.
 
-        :param list[str] comment: The comment as a list of strings.
+        :param comment: The comment as a list of strings.
         """
         self._comment: List[str] = comment
         """
         The DocBlock as a list of strings.
         """
 
         self._description: str = ''
@@ -32,42 +32,36 @@
 
         self.__reflect()
 
     # ------------------------------------------------------------------------------------------------------------------
     def get_description(self) -> str:
         """
         Returns the description.
-
-        :rtype: str
         """
         return self._description
 
     # ------------------------------------------------------------------------------------------------------------------
     def get_tag(self, name: str) -> str:
         """
         Returns a tag.
 
         @param str name: The name of the tag.
-
-        :rtype: str
         """
         for tag in self._tags:
             if tag[0] == name:
                 return tag[1]
 
         return ''
 
     # ------------------------------------------------------------------------------------------------------------------
     def get_tags(self, name: str) -> List[str]:
         """
         Returns a list of tags.
 
         @param str name: The name of the tag.
-
-        :rtype: list[str]
         """
         tags = list()
         for tag in self._tags:
             if tag[0] == name:
                 tags.append(tag[1])
 
         return tags
@@ -83,15 +77,15 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def __remove_leading_empty_lines(lines: List[str]) -> List[str]:
         """
         Removes leading empty lines from a list of lines.
 
-        :param list[str] lines: The lines.
+        :param lines: The lines.
         """
         tmp = list()
         empty = True
         for i in range(0, len(lines)):
             empty = empty and lines[i] == ''
             if not empty:
                 tmp.append(lines[i])
@@ -100,15 +94,15 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def __remove_trailing_empty_lines(lines: List[str]) -> List[str]:
         """
         Removes leading empty lines from a list of lines.
 
-        :param list[str] lines: The lines.
+        :param lines: The lines.
         """
         lines.reverse()
         tmp = DocBlockReflection.__remove_leading_empty_lines(lines)
         lines.reverse()
         tmp.reverse()
 
         return tmp
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/MetadataDataLayer.py` & `pystratum_common-2.0.0/pystratum_common/MetadataDataLayer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import os
 
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 
 class MetadataDataLayer:
     """
     Data layer for retrieving metadata and loading stored routines.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle):
+    def __init__(self, io: StratumIO):
         """
         Object constructor.
 
-        :param PyStratumStyle io: The output decorator.
+        :param io: The output decorator.
         """
 
-        self._io: StratumStyle = io
+        self._io: StratumIO = io
         """
         The output decorator.
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _log_query(self, query: str) -> None:
         """
         Logs the query on the console.
 
-        :param str query: The query.
+        :param query: The query.
         """
         query = query.strip()
 
         if os.linesep in query:
             # Query is a multi line query
             self._io.log_very_verbose('Executing query:')
             self._io.log_very_verbose('<sql>{0}</sql>'.format(query))
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/Util.py` & `pystratum_common-2.0.0/pystratum_common/Util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 
 class Util:
     """
-    An utility class with miscellaneous functions that don't belong somewhere else.
+    A utility class with miscellaneous functions that don't belong somewhere else.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
-    def write_two_phases(filename: str, data: str, io: StratumStyle) -> None:
+    def write_two_phases(filename: str, data: str, io: StratumIO) -> None:
         """
         Writes a file in two phase to the filesystem.
 
-        First write the data to a temporary file (in the same directory) and than renames the temporary file. If the
+        First write the data to a temporary file (in the same directory) and then renames the temporary file. If the
         file already exists and its content is equal to the data that must be written no action is taken. This has the
         following advantages:
-        * In case of some write error (e.g. disk full) the original file is kep in tact and no file with partially data
+        * In case of some write error (e.g. disk full) the original file is keept intact and no file with partially data
         is written.
         * Renaming a file is atomic. So, running processes will never read a partially written data.
 
-        :param str filename: The name of the file were the data must be stored.
-        :param str data: The data that must be written.
-        :param StratumStyle io: The output decorator.
+        :param filename: The name of the file were the data must be stored.
+        :param data: The data that must be written.
+        :param io: The output decorator.
         """
         write_flag = True
         if os.path.exists(filename):
             with open(filename, 'r') as file:
                 old_data = file.read()
                 if data == old_data:
                     write_flag = False
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/backend/CommonConstantWorker.py` & `pystratum_common-2.0.0/pystratum_common/backend/CommonConstantWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import abc
 import configparser
 from typing import Dict, Optional
 
 from pystratum_backend.ConstantWorker import ConstantWorker
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
+
 from pystratum_common.ConstantClass import ConstantClass
 from pystratum_common.Util import Util
 
 
 class CommonConstantWorker(ConstantWorker):
     """
     Abstract parent class for RDBMS specific classes for creating constants based on column widths, and auto increment
     columns and labels.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle, config: configparser.ConfigParser):
+    def __init__(self, io: StratumIO, config: configparser.ConfigParser):
         """
         Object constructor.
 
-        :param PyStratumStyle io: The output decorator.
+        :param PyStratumIO io: The output decorator.
         """
         self._constants: Dict[str, int] = {}
         """
         All constants.
         """
 
         self._old_columns: Dict = {}
@@ -48,15 +49,15 @@
         """
 
         self._labels: Dict = {}
         """
         All primary key labels, their widths and constant names.
         """
 
-        self._io: StratumStyle = io
+        self._io: StratumIO = io
         """
         The output decorator.
         """
 
         self._config = config
         """
         The configuration object.
@@ -100,29 +101,29 @@
             self._write_columns()
             self._get_labels()
             self._fill_constants()
             self.__write_constant_class()
             self.disconnect()
             self.__log_number_of_constants()
 
-            self._io.writeln('')
+            self._io.write_line('')
         else:
             self._io.log_verbose('Constants not enabled')
 
         return 0
 
     # ------------------------------------------------------------------------------------------------------------------
     def __log_number_of_constants(self) -> None:
         """
         Logs the number of constants generated.
         """
         n_id = len(self._labels)
         n_widths = len(self._constants) - n_id
 
-        self._io.writeln('')
+        self._io.write_line('')
         self._io.text('Number of constants based on column widths: {0}'.format(n_widths))
         self._io.text('Number of constants based on database IDs : {0}'.format(n_id))
 
     # ------------------------------------------------------------------------------------------------------------------
     def _read_configuration_file(self) -> None:
         """
         Reads parameters from the configuration file.
@@ -150,16 +151,16 @@
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _enhance_columns(self) -> None:
         """
         Enhances old_columns as follows:
-        If the constant name is *, is is replaced with the column name prefixed by prefix in uppercase.
-        Otherwise the constant name is set to uppercase.
+        If the constant name is *, it is replaced with the column name prefixed by prefix in uppercase.
+        Otherwise, the constant name is set to uppercase.
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _merge_columns(self) -> None:
         """
@@ -195,13 +196,11 @@
     # ------------------------------------------------------------------------------------------------------------------
     def __write_constant_class(self) -> None:
         """
         Inserts new and replaces old (if any) constant declaration statements in the class that acts like a namespace
         for constants.
         """
         helper = ConstantClass(self._class_name, self._io)
-
         content = helper.source_with_constants(self._constants)
-
         Util.write_two_phases(helper.file_name(), content, self._io)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/backend/CommonRoutineLoaderWorker.py` & `pystratum_common-2.0.0/pystratum_common/backend/CommonRoutineLoaderWorker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import abc
 import configparser
 import json
 import os
 from typing import Dict, List, Optional
 
 from pystratum_backend.RoutineLoaderWorker import RoutineLoaderWorker
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
+
 from pystratum_common.ConstantClass import ConstantClass
 from pystratum_common.helper.RoutineLoaderHelper import RoutineLoaderHelper
 
 
 class CommonRoutineLoaderWorker(RoutineLoaderWorker):
     """
     Class for loading stored routines into a RDBMS instance from (pseudo) SQL files.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle, config: configparser.ConfigParser):
+    def __init__(self, io: StratumIO, config: configparser.ConfigParser):
         """
         Object constructor.
 
-        :param pystratum.style.PyStratumStyle.PyStratumStyle io: The output decorator.
+        :param io: The output decorator.
         """
         self.error_file_names = set()
         """
         A set with source names that are not loaded into RDBMS instance.
-
-        :type: set
         """
 
         self._pystratum_metadata: Dict = {}
         """
         The meta data of all stored routines.
         """
 
@@ -75,24 +74,22 @@
         """
 
         self.__shadow_directory: Optional[str] = None
         """
         The name of the directory were copies with pure SQL of the stored routine sources must be stored.
         """
 
-        self._io: StratumStyle = io
+        self._io: StratumIO = io
         """
         The output decorator.
         """
 
         self._config = config
         """
         The configuration object.
-
-        :type: ConfigParser 
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute(self, file_names: Optional[List[str]] = None) -> int:
         """
         Loads stored routines into the current schema.
 
@@ -108,15 +105,15 @@
             self.__load_list(file_names)
         else:
             self.__load_all()
 
         if self.error_file_names:
             self.__log_overview_errors()
 
-        self._io.writeln('')
+        self._io.write_line('')
 
         return 1 if self.error_file_names else 0
 
     # ------------------------------------------------------------------------------------------------------------------
     def __log_overview_errors(self) -> None:
         """
         Show info about sources files of stored routines that were not loaded successfully.
@@ -140,18 +137,18 @@
         Disconnects from the RDBMS instance.
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     def _add_replace_pair(self, name: str, value: str, quote: bool):
         """
-        Adds a replace part to the map of replace pairs.
+        Adds a replacement to the map of replacement pairs.
 
-        :param name: The name of the replace pair.
-        :param value: The value of value of the replace pair.
+        :param name: The name of the replacement pair.
+        :param value: The value of the replacement pair.
         """
         key = '@' + name + '@'
         key = key.lower()
 
         class_name = value.__class__.__name__
 
         if class_name in ['int', 'float']:
@@ -166,15 +163,16 @@
 
         self._replace_pairs[key] = value
 
     # ------------------------------------------------------------------------------------------------------------------
     def __load_list(self, file_names: Optional[List[str]]) -> None:
         """
         Loads all stored routines in a list into the RDBMS instance.
-        :param list[str] file_names: The list of files to be loaded.
+
+        :param file_names: The list of files to be loaded.
         """
         self.connect()
         self.find_source_files_from_list(file_names)
         self._get_column_type()
         self.__read_stored_routine_metadata()
         self.__get_constants()
         self._get_old_stored_routine_info()
@@ -206,33 +204,31 @@
         """
         Reads parameters from the configuration file.
         """
         self._source_directory = self._config.get('loader', 'source_directory')
         self._source_file_extension = self._config.get('loader', 'extension')
         self._source_file_encoding = self._config.get('loader', 'encoding')
         self.__shadow_directory = self._config.get('loader', 'shadow_directory', fallback=None)
-
         self._pystratum_metadata_filename = self._config.get('wrapper', 'metadata')
-
         self._constants_class_name = self._config.get('constants', 'class')
 
     # ------------------------------------------------------------------------------------------------------------------
     def __find_source_files(self) -> None:
         """
         Searches recursively for all source files in a directory.
         """
         for dir_path, _, files in os.walk(self._source_directory):
             for name in files:
                 if name.lower().endswith(self._source_file_extension):
                     basename = os.path.splitext(os.path.basename(name))[0]
                     relative_path = os.path.relpath(os.path.join(dir_path, name))
 
                     if basename in self._source_file_names:
-                        self._io.error("Files '{0}' and '{1}' have the same basename.".
-                                       format(self._source_file_names[basename], relative_path))
+                        self._io.error("Files '{0}' and '{1}' have the same basename.".format(
+                                self._source_file_names[basename], relative_path))
                         self.error_file_names.add(relative_path)
                     else:
                         self._source_file_names[basename] = relative_path
 
     # ------------------------------------------------------------------------------------------------------------------
     def __read_stored_routine_metadata(self) -> None:
         """
@@ -255,28 +251,26 @@
     def create_routine_loader_helper(self,
                                      routine_name: str,
                                      pystratum_old_metadata: Dict,
                                      rdbms_old_metadata: Dict) -> RoutineLoaderHelper:
         """
         Creates a Routine Loader Helper object.
 
-        :param str routine_name: The name of the routine.
-        :param dict pystratum_old_metadata: The old metadata of the stored routine from PyStratum.
-        :param dict rdbms_old_metadata:  The old metadata of the stored routine from database instance.
-
-        :rtype: RoutineLoaderHelper
+        :param routine_name: The name of the routine.
+        :param pystratum_old_metadata: The old metadata of the stored routine from PyStratum.
+        :param rdbms_old_metadata:  The old metadata of the stored routine from database instance.
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     def __load_stored_routines(self) -> None:
         """
         Loads all stored routines into the RDBMS instance.
         """
-        self._io.writeln('')
+        self._io.write_line('')
 
         for routine_name in sorted(self._source_file_names):
             if routine_name in self._pystratum_metadata:
                 old_metadata = self._pystratum_metadata[routine_name]
             else:
                 old_metadata = None
 
@@ -342,38 +336,39 @@
             json.dump(self._pystratum_metadata, stream, indent=4, sort_keys=True)
 
     # ------------------------------------------------------------------------------------------------------------------
     def find_source_files_from_list(self, file_names) -> None:
         """
         Finds all source files that actually exists from a list of file names.
 
-        :param list[str] file_names: The list of file names.
+        :param file_names: The list of file names.
         """
         for file_name in file_names:
             if os.path.exists(file_name):
                 routine_name = os.path.splitext(os.path.basename(file_name))[0]
                 if routine_name not in self._source_file_names:
                     self._source_file_names[routine_name] = file_name
                 else:
-                    self._io.error("Files '{0}' and '{1}' have the same basename.".
-                                   format(self._source_file_names[routine_name], file_name))
+                    self._io.error("Files '{0}' and '{1}' have the same basename.".format(
+                            self._source_file_names[routine_name], file_name))
                     self.error_file_names.add(file_name)
             else:
                 self._io.error("File not exists: '{0}'".format(file_name))
                 self.error_file_names.add(file_name)
 
     # ------------------------------------------------------------------------------------------------------------------
     def __get_constants(self) -> None:
         """
-        Gets the constants from the class that acts like a namespace for constants and adds them to the replace pairs.
+        Gets the constants from the class that acts like a namespace for constants and adds them to the replacement
+        pairs.
         """
         helper = ConstantClass(self._constants_class_name, self._io)
         helper.reload()
         constants = helper.constants()
 
         for name, value in constants.items():
             self._add_replace_pair(name, value, True)
 
-        self._io.text('Read {0} constants for substitution from <fso>{1}</fso>'.
-                      format(len(constants), helper.file_name()))
+        self._io.text('Read {0} constants for substitution from <fso>{1}</fso>'.format(len(constants),
+                                                                                       helper.file_name()))
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/backend/CommonRoutineWrapperGeneratorWorker.py` & `pystratum_common-2.0.0/pystratum_common/backend/CommonRoutineWrapperGeneratorWorker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import abc
 import configparser
 import json
 import os
 from typing import Any, Dict, Optional
 
 from pystratum_backend.RoutineWrapperGeneratorWorker import RoutineWrapperGeneratorWorker
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 from pystratum_common.Util import Util
 
 
 class CommonRoutineWrapperGeneratorWorker(RoutineWrapperGeneratorWorker):
     """
     Class for generating a class with wrapper methods for calling stored routines in a MySQL database.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle, config: configparser.ConfigParser):
+    def __init__(self, io: StratumIO, config: configparser.ConfigParser):
         """
         Object constructor.
 
-        :param PyStratumStyle io: The output decorator.
+        :param io: The output decorator.
         """
         self._code: str = ''
         """
         The generated Python code buffer.
         """
 
         self._lob_as_string_flag: bool = False
@@ -52,41 +52,37 @@
         """
 
         self._wrapper_filename: Optional[str] = None
         """
         The filename where the generated wrapper class must be stored.
         """
 
-        self._io: StratumStyle = io
+        self._io: StratumIO = io
         """
         The output decorator.
         """
 
         self._config = config
         """
         The configuration object.
-
-        :type: ConfigParser 
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute(self) -> int:
         """
         The "main" of the wrapper generator. Returns 0 on success, 1 if one or more errors occurred.
-
-        :rtype: int
         """
         self._read_configuration_file()
 
         if self._wrapper_class_name:
             self._io.title('Wrapper')
 
             self.__generate_wrapper_class()
 
-            self._io.writeln('')
+            self._io.write_line('')
         else:
             self._io.log_verbose('Wrapper not enabled')
 
         return 0
 
     # ------------------------------------------------------------------------------------------------------------------
     def __generate_wrapper_class(self) -> None:
@@ -120,16 +116,14 @@
         self._metadata_filename = self._config.get('wrapper', 'metadata')
         self._lob_as_string_flag = bool(self._config.get('wrapper', 'lob_as_string'))
 
     # ------------------------------------------------------------------------------------------------------------------
     def _read_routine_metadata(self) -> Dict:
         """
         Returns the metadata of stored routines.
-
-        :rtype: dict
         """
         metadata = {}
         if os.path.isfile(self._metadata_filename):
             with open(self._metadata_filename, 'r') as file:
                 metadata = json.load(file)
 
         return metadata
@@ -150,15 +144,15 @@
         self._write_line('    """')
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_line(self, text: str = '') -> None:
         """
         Writes a line with Python code to the generate code buffer.
 
-        :param str text: The line with Python code.
+        :param text: The line with Python code.
         """
         if text:
             self._code += str(text) + "\n"
         else:
             self._code += "\n"
 
     # ------------------------------------------------------------------------------------------------------------------
@@ -172,12 +166,12 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _write_routine_function(self, routine: Dict[str, Any]) -> None:
         """
         Generates a complete wrapper method for a stored routine.
 
-        :param dict routine: The metadata of the stored routine.
+        :param routine: The metadata of the stored routine.
         """
         raise NotImplementedError()
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/helper/DataTypeHelper.py` & `pystratum_common-2.0.0/pystratum_common/helper/DataTypeHelper.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,24 @@
     Utility class for deriving information based on a DBMS native data type.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def column_type_to_python_type(self, data_type_info: Dict[str, Any]) -> str:
         """
-        Returns the corresponding Python data type of a DBMS native data type.
+        Returns the corresponding Python data type of DBMS native data type.
 
         :param dict data_type_info: The DBMS native data type metadata.
-
-        :rtype: str
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def column_type_to_python_type_hint(self, data_type_info: Dict[str, Any]) -> str:
         """
         Returns the corresponding Python data type hint of a MySQL data type.
 
         :param dict data_type_info: The MySQL data type metadata.
-
-        :rtype: str
         """
         raise NotImplementedError()
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/helper/RoutineLoaderHelper.py` & `pystratum_common-2.0.0/pystratum_common/helper/RoutineLoaderHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import abc
 import math
 import os
 import re
 import stat
 from typing import Dict, List, Optional, Tuple, Union
 
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 from pystratum_common.DocBlockReflection import DocBlockReflection
 from pystratum_common.exception.LoaderException import LoaderException
 from pystratum_common.helper.DataTypeHelper import DataTypeHelper
 
 
 class RoutineLoaderHelper(metaclass=abc.ABCMeta):
     """
     Class for loading a single stored routine into a RDBMS instance from a (pseudo) SQL file.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __init__(self,
-                 io: StratumStyle,
+                 io: StratumIO,
                  routine_filename: str,
                  routine_file_encoding: str,
                  pystratum_old_metadata: Dict,
                  replace_pairs: Dict[str, str],
                  rdbms_old_metadata: Dict):
         """
         Object constructor.
 
-        :param PyStratumStyle io: The output decorator.
-        :param str routine_filename: The filename of the source of the stored routine.
-        :param str routine_file_encoding: The encoding of the source file.
-        :param dict pystratum_old_metadata: The metadata of the stored routine from PyStratum.
-        :param dict[str,str] replace_pairs: A map from placeholders to their actual values.
-        :param dict rdbms_old_metadata: The old metadata of the stored routine from the RDBMS instance.
+        :param io: The output decorator.
+        :param routine_filename: The filename of the source of the stored routine.
+        :param routine_file_encoding: The encoding of the source file.
+        :param pystratum_old_metadata: The metadata of the stored routine from PyStratum.
+        :param replace_pairs: A map from placeholders to their actual values.
+        :param rdbms_old_metadata: The old metadata of the stored routine from the RDBMS instance.
         """
         self._source_filename: str = routine_filename
         """
         The source filename holding the stored routine.
         """
 
         self._routine_file_encoding: str = routine_file_encoding
@@ -132,33 +132,31 @@
         """
 
         self._columns: Optional[List] = None
         """
         The key or index columns (depending on the designation type) of the stored routine.
         """
 
-        self._io: StratumStyle = io
+        self._io: StratumIO = io
         """
         The output decorator.
         """
 
         self.shadow_directory: Optional[str] = None
         """
         The name of the directory were copies with pure SQL of the stored routine sources must be stored.
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def load_stored_routine(self) -> Union[Dict[str, str], bool]:
         """
         Loads the stored routine into the instance of MySQL.
 
-        Returns the metadata of the stored routine if the stored routine is loaded successfully. Otherwise returns
+        Returns the metadata of the stored routine if the stored routine is loaded successfully. Otherwise, returns
         False.
-
-        :rtype: dict[str,str]|bool
         """
         try:
             self._routine_name = os.path.splitext(os.path.basename(self._source_filename))[0]
 
             if os.path.exists(self._source_filename):
                 if os.path.isfile(self._source_filename):
                     self._m_time = int(os.path.getmtime(self._source_filename))
@@ -210,15 +208,15 @@
                 doc_block_parameters_names.append(parameter['name'])
 
         # Check and show warning if any parameters is missing in doc block.
         for parameter in database_parameters_names:
             if parameter not in doc_block_parameters_names:
                 self._io.warning('Parameter {} is missing in doc block'.format(parameter))
 
-        # Check and show warning if find unknown parameters in doc block.
+        # Check and show warning if found unknown parameters in doc block.
         for parameter in doc_block_parameters_names:
             if parameter not in database_parameters_names:
                 self._io.warning('Unknown parameter {} found in doc block'.format(parameter))
 
     # ------------------------------------------------------------------------------------------------------------------
     def __read_source_file(self) -> None:
         """
@@ -275,27 +273,23 @@
         self._routine_source_code = "\n".join(routine_source)
 
     # ------------------------------------------------------------------------------------------------------------------
     def _log_exception(self, exception: Exception) -> None:
         """
         Logs an exception.
 
-        :param Exception exception: The exception.
-
-        :rtype: None
+        :param exception: The exception.
         """
         self._io.error(str(exception).strip().split(os.linesep))
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _must_reload(self) -> bool:
         """
-        Returns True if the source file must be load or reloaded. Otherwise returns False.
-
-        :rtype: bool
+        Returns whether the source file must be load or reloaded.
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     def __get_placeholders(self) -> None:
         """
         Extracts the placeholders from the stored routine source.
@@ -398,16 +392,14 @@
                         if matches[0][1]:
                             raise LoaderException('Expected: -- type: {}'.format(self._designation_type))
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_specification_positions(self) -> Tuple[int, int]:
         """
         Returns a tuple with the start and end line numbers of the stored routine specification.
-
-        :rtype: tuple
         """
         start = -1
         for (i, line) in enumerate(self._routine_source_code_lines):
             if self._is_start_of_stored_routine(line):
                 start = i
 
         end = -1
@@ -417,30 +409,26 @@
 
         return start, end
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _is_start_of_stored_routine(self, line: str) -> bool:
         """
-        Returns True if a line is the start of the code of the stored routine.
-
-        :param str line: The line with source code of the stored routine.
+        Returns whether a line is the start of the code of the stored routine.
 
-        :rtype: bool
+        :param line: The line with source code of the stored routine.
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     def _is_start_of_stored_routine_body(self, line: str) -> bool:
         """
-        Returns True if a line is the start of the body of the stored routine.
+        Returns whether a line is the start of the body of the stored routine.
 
-        :param str line: The line with source code of the stored routine.
-
-        :rtype: bool
+        :param line: The line with source code of the stored routine.
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     def __get_doc_block_lines(self) -> Tuple[int, int]:
         """
         Returns the start and end line of the DocBlock of the stored routine code.
@@ -487,31 +475,27 @@
                                                                    'description': parts.group(3)})
 
     # ------------------------------------------------------------------------------------------------------------------
     def __get_parameter_doc_description(self, name: str) -> str:
         """
         Returns the description by name of the parameter as found in the DocBlock of the stored routine.
 
-        :param str name: The name of the parameter.
-
-        :rtype: str
+        :param name: The name of the parameter.
         """
         for param in self._doc_block_parts_source['parameters']:
             if param['name'] == name:
                 return param['description']
 
         return ''
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _get_data_type_helper(self) -> DataTypeHelper:
         """
         Returns a data type helper object appropriate for the RDBMS.
-
-        :rtype: DataTypeHelper
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     def __get_doc_block_parts_wrapper(self) -> None:
         """
         Generates the DocBlock parts to be used by the wrapper generator.
@@ -533,16 +517,14 @@
         self._doc_block_parts_wrapper['parameters'] = parameters
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _get_name(self) -> None:
         """
         Extracts the name of the stored routine and the stored routine type (i.e. procedure or function) source.
-
-        :rtype: None
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _load_routine_file(self) -> None:
         """
@@ -558,15 +540,15 @@
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _get_routine_parameters_info(self) -> None:
         """
-        Retrieves information about the stored routine parameters from the meta data of the RDBMS.
+        Retrieves information about the stored routine parameters from the metadata of the RDBMS.
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     def _update_metadata(self) -> None:
         """
         Updates the metadata of the stored routine.
@@ -617,18 +599,18 @@
 
         if '__LINE__' in self._replace:
             del self._replace['__LINE__']
 
     # ------------------------------------------------------------------------------------------------------------------
     def _print_sql_with_error(self, sql: str, error_line: int) -> None:
         """
-        Writes a SQL statement with an syntax error to the output. The line where the error occurs is highlighted.
+        Writes a SQL statement with a syntax error to the output. The line where the error occurs is highlighted.
 
-        :param str sql: The SQL statement.
-        :param int error_line: The line where the error occurs.
+        :param sql: The SQL statement.
+        :param error_line: The line where the error occurs.
         """
         if os.linesep in sql:
             lines = sql.split(os.linesep)
             digits = math.ceil(math.log(len(lines) + 1, 10))
             i = 1
             for line in lines:
                 if i == error_line:
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/BulkWrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/BulkWrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,48 +10,42 @@
     Wrapper method generator for stored procedures with designation type bulk.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'int'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
         return 'int'
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def _get_wrapper_args(routine: Dict[str, Any]) -> str:
         """
         Returns code for the parameters of the wrapper method for the stored routine.
 
-        :param dict[str,*] routine: The routine metadata.
-
-        :rtype: str
+        :param routine: The routine metadata.
         """
         parameters = Wrapper._get_wrapper_args(routine)
 
         return re.sub(r'^self', 'self, bulk_handler', parameters)
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_docstring_parameters(self, routine: Dict[str, Any]) -> None:
         """
         Writes the parameters part of the docstring for the wrapper method of a stored routine.
 
-        :param dict routine: The metadata of the stored routine.
+        :param routine: The metadata of the stored routine.
         """
         self._write_line('')
         self._write_line(':param pystratum.BulkHandler.BulkHandler bulk_handler: '
                          'The bulk handler for processing the selected rows.')
 
         Wrapper._write_docstring_parameters(self, routine)
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/FunctionsWrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/Row0Wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from abc import ABC
 
 from pystratum_common.wrapper.Wrapper import Wrapper
 
 
-class FunctionsWrapper(Wrapper, ABC):
+class Row0Wrapper(Wrapper, ABC):
     """
-    Wrapper method generator for stored functions.
+    Wrapper method generator for stored procedures that are selecting 0 or 1 row.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'Any'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
-        return '*'
+        return 'None|dict[str,*]'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/LogWrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/LogWrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,18 @@
     Wrapper method generator for stored procedures with designation type log.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'int'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
         return 'int'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/MultiWrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/MultiWrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,22 +8,18 @@
     Wrapper method generator for stored procedures with designation type log.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'List[List[Dict[str, Any]]]'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
         return 'list[list[dict[str,*]]]'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/NoneWrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/Singleton0Wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from abc import ABC
 
 from pystratum_common.wrapper.Wrapper import Wrapper
 
 
-class NoneWrapper(Wrapper, ABC):
+class Singleton0Wrapper(Wrapper, ABC):
     """
-    Wrapper method generator for stored procedures without any result set.
+    Wrapper method generator for stored procedures that are selecting 0 or 1 row with one column only.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
-        return 'int'
+        return 'Any'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
-        return 'int'
+        return '*'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/Row0Wrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/RowsWrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from abc import ABC
 
 from pystratum_common.wrapper.Wrapper import Wrapper
 
 
-class Row0Wrapper(Wrapper, ABC):
+class RowsWrapper(Wrapper, ABC):
     """
-    Wrapper method generator for stored procedures that are selecting 0 or 1 row.
+    Wrapper method generator for stored procedures that are selecting 0, 1, or more rows.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
-        return 'Any'
+        return 'List[Dict[str, Any]]'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
-        return 'None|dict[str,*]'
+        return 'list[dict[str,*]]'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/Row1Wrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/Singleton1Wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from abc import ABC
 
 from pystratum_common.wrapper.Wrapper import Wrapper
 
 
-class Row1Wrapper(Wrapper, ABC):
+class Singleton1Wrapper(Wrapper, ABC):
     """
-    Wrapper method generator for stored procedures that are selecting 1 row.
+    Wrapper method generator for stored procedures that are selecting 1 row with one column only.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'Any'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
-        return 'dict[str,*]'
+        return '*'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/RowsWithIndexWrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/RowsWithIndexWrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,29 @@
 from typing import Any, Dict
 
 from pystratum_common.wrapper.Wrapper import Wrapper
 
 
 class RowsWithIndexWrapper(Wrapper):
     """
-    Parent class wrapper wrapper method generator for stored procedures whose result set  must be returned using tree
+    Parent class wrapper method generator for stored procedures whose result set  must be returned using tree
     structure using a combination of non-unique columns.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'Dict'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
         return 'dict'
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _write_execute_rows(self, routine: Dict[str, Any]) -> None:
         raise NotImplementedError()
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/RowsWithKeyWrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/RowsWithKeyWrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,33 +2,29 @@
 from typing import Any, Dict
 
 from pystratum_common.wrapper.Wrapper import Wrapper
 
 
 class RowsWithKeyWrapper(Wrapper):
     """
-    Parent class wrapper wrapper method generator for stored procedures whose result set must be returned using tree
+    Parent class wrapper method generator for stored procedures whose result set must be returned using tree
     structure using a combination of unique columns.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'Dict'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self):
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
         return 'dict'
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _write_execute_rows(self, routine: Dict[str, Any]) -> None:
         raise NotImplementedError()
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/RowsWrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/FunctionsWrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from abc import ABC
 
 from pystratum_common.wrapper.Wrapper import Wrapper
 
 
-class RowsWrapper(Wrapper, ABC):
+class FunctionsWrapper(Wrapper, ABC):
     """
-    Wrapper method generator for stored procedures that are selecting 0, 1, or more rows.
+    Wrapper method generator for stored functions.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
-        return 'List[Dict[str, Any]]'
+        return 'Any'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
-        return 'list[dict[str,*]]'
+        return '*'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/Singleton0Wrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/Row1Wrapper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from abc import ABC
 
 from pystratum_common.wrapper.Wrapper import Wrapper
 
 
-class Singleton0Wrapper(Wrapper, ABC):
+class Row1Wrapper(Wrapper, ABC):
     """
-    Wrapper method generator for stored procedures that are selecting 0 or 1 row with one column only.
+    Wrapper method generator for stored procedures that are selecting 1 row.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'Any'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
-        return '*'
+        return 'dict[str,*]'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/TableWrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/TableWrapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,22 +8,18 @@
     Wrapper method generator for printing the result set of stored procedures in a table format.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
         return 'int'
 
     # ------------------------------------------------------------------------------------------------------------------
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper methods the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper methods to be used in the docstring.
         """
         return 'int'
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Common-1.1.1/pystratum_common/wrapper/Wrapper.py` & `pystratum_common-2.0.0/pystratum_common/wrapper/Wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __init__(self, routine: Dict[str, Any], lob_as_string_flag: bool):
         """
         Object constructor.
 
-        :param dict routine: The metadata of the stored routine.
+        :param routine: The metadata of the stored routine.
         :param bool lob_as_string_flag: If 'True' LOBs must be treated as strings/bytes.
         """
         self._page_width: int = 120
         """
         The maximum number of columns in the source code.
         """
 
@@ -34,15 +34,15 @@
         self._routine: Dict[str, Any] = routine
         """
         The metadata of the stored routine.
         """
 
         self._lob_as_string_flag: bool = lob_as_string_flag == 'True'
         """
-        If True BLOBs and CLOBs must be treated as strings.
+        Whether BLOBs and CLOBs must be treated as strings.
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write(self, text: str) -> None:
         """
         Appends a part of code to the generated code.
 
@@ -51,15 +51,15 @@
         self._code += str(text)
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_line(self, line: Optional[str] = None) -> None:
         """
         Appends a line of code to the generated code and adjust the indent level of the generated code.
 
-        :param line: The line of code (with out LF) that must be appended.
+        :param line: The line of code (without LF) that must be appended.
         """
         if line is None:
             self._write("\n")
             if self.__indent_level > 1:
                 self.__indent_level -= 1
         elif line == '':
             self._write("\n")
@@ -85,55 +85,51 @@
         """
         tmp = self._page_width - ((4 * self.__indent_level) + 2)
         self._write_line('# ' + ('-' * tmp))
 
     # ------------------------------------------------------------------------------------------------------------------
     def is_lob_parameter(self, parameters: Dict[str, Any]) -> bool:
         """
-        Returns True of one of the parameters is a BLOB or CLOB. Otherwise, returns False.
+        Returns Whether one of the parameters is a BLOB or CLOB.
 
         :param parameters: The parameters of a stored routine.
-
-        :rtype: bool
         """
         raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     def write_routine_method(self, routine: Dict[str, Any]) -> str:
         """
         Returns a complete wrapper method.
 
-        :param dict[str,*] routine: The routine metadata.
-
-        :rtype: str
+        :param routine: The routine metadata.
         """
         if self._lob_as_string_flag:
             return self._write_routine_method_without_lob(routine)
         else:
             if self.is_lob_parameter(routine['parameters']):
                 return self._write_routine_method_with_lob(routine)
             else:
                 return self._write_routine_method_without_lob(routine)
 
     # ------------------------------------------------------------------------------------------------------------------
     def __write_docstring_description(self, routine: Dict[str, Any]) -> None:
         """
         Writes the description part of the docstring for the wrapper method of a stored routine.
 
-        :param dict routine: The metadata of the stored routine.
+        :param routine: The metadata of the stored routine.
         """
         if routine['pydoc']['description']:
             self._write_line(routine['pydoc']['description'])
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_docstring_parameters(self, routine: Dict[str, Any]) -> None:
         """
         Writes the parameters part of the docstring for the wrapper method of a stored routine.
 
-        :param dict routine: The metadata of the stored routine.
+        :param routine: The metadata of the stored routine.
         """
         if routine['pydoc']['parameters']:
             self._write_line('')
 
             for param in routine['pydoc']['parameters']:
                 lines = param['description'].split(os.linesep)
                 self._write_line(':param {0} {1}: {2}'.format(param['python_type'],
@@ -159,41 +155,39 @@
             self._write_line(':rtype: {0}'.format(rtype))
 
     # ------------------------------------------------------------------------------------------------------------------
     def __write_docstring(self, routine: Dict[str, Any]) -> None:
         """
         Writes the docstring for the wrapper method of a stored routine.
 
-        :param dict routine: The metadata of the stored routine.
+        :param routine: The metadata of the stored routine.
         """
         self._write_line('"""')
 
         self.__write_docstring_description(routine)
         self._write_docstring_parameters(routine)
         self.__write_docstring_return_type()
 
         self._write_line('"""')
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _get_docstring_return_type(self) -> str:
         """
-        Returns the return type of the wrapper method the be used in the docstring.
-
-        :rtype: str
+        Returns the return type of the wrapper method to be used in the docstring.
         """
+        raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _return_type_hint(self) -> str:
         """
         Returns the return type hint of the wrapper method.
-
-        :rtype: str
         """
+        raise NotImplementedError()
 
     # ------------------------------------------------------------------------------------------------------------------
     @abc.abstractmethod
     def _write_result_handler(self, routine: Dict[str, Any]) -> None:
         """
         Generates code for calling the stored routine in the wrapper method.
         """
@@ -201,15 +195,14 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_routine_method_with_lob(self, routine: Dict[str, Any]) -> str:
         return self._write_routine_method_without_lob(routine)
 
     # ------------------------------------------------------------------------------------------------------------------
     def _write_routine_method_without_lob(self, routine: Dict[str, Any]) -> str:
-
         self._write_line()
         self._write_separator()
         self._write_line('def {0!s}({1!s}) -> {2!s}:'.format(str(routine['routine_name']),
                                                              str(self._get_wrapper_args(routine)),
                                                              str(self._return_type_hint())))
         self.__write_docstring(routine)
         self._write_result_handler(routine)
@@ -218,17 +211,15 @@
 
     # ------------------------------------------------------------------------------------------------------------------
     @staticmethod
     def _get_wrapper_args(routine: Dict[str, Any]) -> str:
         """
         Returns code for the parameters of the wrapper method for the stored routine.
 
-        :param dict[str,*] routine: The routine metadata.
-
-        :rtype: str
+        :param routine: The routine metadata.
         """
         ret = 'self'
 
         for parameter_info in routine['pydoc']['parameters']:
             if ret:
                 ret += ', '
```

