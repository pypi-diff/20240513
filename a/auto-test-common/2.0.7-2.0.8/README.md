# Comparing `tmp/auto-test-common-2.0.7.tar.gz` & `tmp/auto-test-common-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-2.0.7.tar", last modified: Sat May 11 00:58:03 2024, max compression
+gzip compressed data, was "auto-test-common-2.0.8.tar", last modified: Mon May 13 07:43:13 2024, max compression
```

## Comparing `auto-test-common-2.0.7.tar` & `auto-test-common-2.0.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.294419 auto-test-common-2.0.7/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-11 00:58:03.294521 auto-test-common-2.0.7/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.257666 auto-test-common-2.0.7/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-11 00:58:02.000000 auto-test-common-2.0.7/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1821 2024-05-11 00:58:03.000000 auto-test-common-2.0.7/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-05-11 00:58:02.000000 auto-test-common-2.0.7/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-05-11 00:58:02.000000 auto-test-common-2.0.7/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      727 2024-05-11 00:58:02.000000 auto-test-common-2.0.7/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-05-11 00:58:02.000000 auto-test-common-2.0.7/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.258148 auto-test-common-2.0.7/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.7/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.261051 auto-test-common-2.0.7/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.7/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5450 2024-04-24 07:01:06.000000 auto-test-common-2.0.7/common/autotest/assert_function.py
--rw-r--r--   0 edz        (502) staff       (20)    12837 2024-05-10 02:49:12.000000 auto-test-common-2.0.7/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     8348 2024-05-10 01:35:28.000000 auto-test-common-2.0.7/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.7/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.263671 auto-test-common-2.0.7/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.7/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8764 2024-05-11 00:56:55.000000 auto-test-common-2.0.7/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.7/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.7/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.264401 auto-test-common-2.0.7/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.7/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.7/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.268488 auto-test-common-2.0.7/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.7/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.7/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/data/eval_data_handle.py
--rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.7/common/data/faker_handle.py
--rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.7/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.7/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.273318 auto-test-common-2.0.7/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.7/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.7/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.7/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.7/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.7/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.7/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.275865 auto-test-common-2.0.7/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.7/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.7/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.7/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.281818 auto-test-common-2.0.7/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.7/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.7/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.7/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.7/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.7/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.282583 auto-test-common-2.0.7/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.7/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.7/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.285599 auto-test-common-2.0.7/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.7/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.7/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.7/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.7/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.7/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-11 00:58:03.293915 auto-test-common-2.0.7/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.7/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.7/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.7/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.7/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.7/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23509 2024-05-06 01:03:53.000000 auto-test-common-2.0.7/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.7/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.7/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2024-05-11 00:58:03.295084 auto-test-common-2.0.7/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     2101 2024-04-30 05:32:18.000000 auto-test-common-2.0.7/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.688644 auto-test-common-2.0.8/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-13 07:43:13.688822 auto-test-common-2.0.8/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.629199 auto-test-common-2.0.8/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1821 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      727 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-05-13 07:43:13.000000 auto-test-common-2.0.8/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.629737 auto-test-common-2.0.8/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.8/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.633904 auto-test-common-2.0.8/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.8/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5450 2024-04-24 07:01:06.000000 auto-test-common-2.0.8/common/autotest/assert_function.py
+-rw-r--r--   0 edz        (502) staff       (20)    12600 2024-05-11 02:32:19.000000 auto-test-common-2.0.8/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     8348 2024-05-10 01:35:28.000000 auto-test-common-2.0.8/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.636966 auto-test-common-2.0.8/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.8/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8960 2024-05-13 07:43:05.000000 auto-test-common-2.0.8/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.8/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.638411 auto-test-common-2.0.8/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.8/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.8/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.647514 auto-test-common-2.0.8/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.8/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/data/eval_data_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/data/faker_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.8/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.654759 auto-test-common-2.0.8/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.8/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.8/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.8/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1999 2024-05-13 07:18:24.000000 auto-test-common-2.0.8/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.656755 auto-test-common-2.0.8/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.8/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.8/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.8/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.662480 auto-test-common-2.0.8/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.8/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.8/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.8/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.8/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.663900 auto-test-common-2.0.8/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.8/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.8/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.672660 auto-test-common-2.0.8/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.8/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.8/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.8/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.8/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.8/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-13 07:43:13.687842 auto-test-common-2.0.8/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.8/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10707 2024-05-13 07:41:16.000000 auto-test-common-2.0.8/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.8/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.8/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.8/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.8/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23539 2024-05-13 01:17:46.000000 auto-test-common-2.0.8/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.8/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.8/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2024-05-13 07:43:13.689916 auto-test-common-2.0.8/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     2101 2024-04-30 05:32:18.000000 auto-test-common-2.0.8/setup.py
```

### Comparing `auto-test-common-2.0.7/PKG-INFO` & `auto-test-common-2.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.7
+Version: 2.0.8
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.7/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-2.0.8/auto_test_common.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.7
+Version: 2.0.8
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.7/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-2.0.8/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/auto_test_common.egg-info/requires.txt` & `auto-test-common-2.0.8/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/autotest/assert_function.py` & `auto-test-common-2.0.8/common/autotest/assert_function.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/autotest/base_requests.py` & `auto-test-common-2.0.8/common/autotest/base_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             if isinstance(header, str):
                 header = DataProcess.handle_header(header, data)
             elif header is None:
                 header = DataProcess.handle_header(schemal_data['datatype'], data)
             else:
                 header = DataProcess.handle_header(header, data)
         try:
-            if schemal_data['datatype'] == 'json':
+            if schemal_data['datatype'] == 'json' or schemal_data['datatype'] == 'params':
                 if 'body' in schemal_data:
                     schemal_body = ReadFile.get_yaml_ApiSchemal(schemal_key)
                     content = schemal_body['body']
                     if isinstance(content,dict):
                         if 'file' in content:
                             from common.plugin.file_plugin import FilePlugin
                             content = FilePlugin.load_data(content['file'])
@@ -168,22 +168,18 @@
         return res
 
 
     @classmethod
     def handle_body(self, data, format, _replace):
         test_data = data
         try:
-            if format == 'text':
-                test_data = DataProcess.handle_data(variable=data, jsonformat=False, _replace=_replace)
-            elif format == 'json':
+            if format == 'json':
                 test_data = DataProcess.handle_data(variable=data, _replace=_replace)
             elif format == 'None':
                 test_data = data
-            elif format == 'xml':
-                test_data = DataProcess.handle_data(variable=data, jsonformat=False, _replace=_replace)
             else:
                 test_data = DataProcess.handle_data(variable=data, jsonformat=False, _replace=_replace)
             return test_data
         except Exception as e:
             test_data = data
             return test_data
```

### Comparing `auto-test-common-2.0.7/common/autotest/handle_allure.py` & `auto-test-common-2.0.8/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/autotest/handle_assert.py` & `auto-test-common-2.0.8/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/common/api_driver.py` & `auto-test-common-2.0.8/common/common/api_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,18 @@
             from common.data.data_process import DataProcess
             if DataProcess.isNotNull(_data):
                 if header is not None and isinstance(header,dict):
                     if 'Content-Type' in header:
                         if header['Content-Type'].find('x-www-form-urlencoded') >= 0:
                             if isinstance(_data, str):
                                 _temp = json.loads(_data)
-                        _temp = self.dataEncode(_temp)
+                            _temp = self.dataEncode(_temp)
+                        if header['Content-Type'].find('json') >= 0:
+                            if isinstance(_data, str):
+                                _temp = json.loads(_data)
         except Exception as e:
             logger.warning(f'{_data} 转换Json失败')
         return _temp
 
 
     @classmethod
     def getCommontHeader(self, header):
@@ -177,12 +180,12 @@
                             data[key] = (data[key][0], open(all_path, 'rb'), data[key][2])
                         elif data[key].__len__() == 2:
                             all_path = os.sep.join(TEST_FILE_PATH, _path)
                             from common.file.handle_system import adjust_path
                             all_path = adjust_path(all_path)
                             data[key] = (data[key][0], open(all_path, 'rb'))
                 else:
-                    data = data
+                    data[key] = data[key]
         return data
```

### Comparing `auto-test-common-2.0.7/common/common/constant.py` & `auto-test-common-2.0.8/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/common/test.py` & `auto-test-common-2.0.8/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/config/config.py` & `auto-test-common-2.0.8/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/data/data_process.py` & `auto-test-common-2.0.8/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/data/faker_handle.py` & `auto-test-common-2.0.8/common/data/faker_handle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/data/handle_common.py` & `auto-test-common-2.0.8/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/data/template_data.py` & `auto-test-common-2.0.8/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/db/handle_db.py` & `auto-test-common-2.0.8/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/db/handle_db_batch.py` & `auto-test-common-2.0.8/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/db/handle_mongo.py` & `auto-test-common-2.0.8/common/db/handle_mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,30 @@
     def __init__(self, config):
         """初始化连接MongoDb"""
         my_client = MongoClient(config.get("host"), config.get("port"))
         self.my_db = my_client[config.get("dbName")]
         if config.get("dbUsername") is not None:
             self.my_db.authenticate(config.get("dbUsername"), config.get("dbPasswd"))
 
+
     @classmethod
     def mongo_db(self, _key, env: str = Constant.ENV):
         """
         返回MongoDB数据库
         """
         config = MongoDB.get_db_config(_key, env)
-        return MongoDB(config)
+        return MongoDB(config).my_db
 
     @classmethod
     def mongo_collection(self, _key, _collection, env: str = Constant.ENV):
         """
             返回MongoDB集合
         """
         my_db = MongoDB.mongo_db(_key, env)
-        my_col = my_db[_collectin]
+        my_col = my_db[_collection]
         return my_col
 
     @classmethod
     def mongo_find(self, _key, _collection, _query, type: str = "", limit: int = 0, _sort: str = "",
                    env: str = Constant.ENV):
         """
         查询集合中数据
```

### Comparing `auto-test-common-2.0.7/common/db/handle_mysqldb.py` & `auto-test-common-2.0.8/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/db/handle_oracle.py` & `auto-test-common-2.0.8/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/db/handle_sqlserver.py` & `auto-test-common-2.0.8/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/driver/ui_page.py` & `auto-test-common-2.0.8/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/file/ReadFile.py` & `auto-test-common-2.0.8/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/file/handle_excel.py` & `auto-test-common-2.0.8/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/file/handle_file.py` & `auto-test-common-2.0.8/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/file/handle_reques.py` & `auto-test-common-2.0.8/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/file/handle_system.py` & `auto-test-common-2.0.8/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/file/handle_yaml.py` & `auto-test-common-2.0.8/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/mq/handle_rabbit.py` & `auto-test-common-2.0.8/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plat/ATF_platform.py` & `auto-test-common-2.0.8/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plat/jenkin_platform.py` & `auto-test-common-2.0.8/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plat/jira_platform.py` & `auto-test-common-2.0.8/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plat/mysql_platform.py` & `auto-test-common-2.0.8/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plat/service_platform.py` & `auto-test-common-2.0.8/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plugin/allure_plugin.py` & `auto-test-common-2.0.8/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plugin/assert_plugin.py` & `auto-test-common-2.0.8/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plugin/atf_plugin.py` & `auto-test-common-2.0.8/common/plugin/atf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,18 @@
 
 
 
 
 
 
 
+if __name__ == '__main__':
+    results = ATFPlugin.mongo_collection('ndcaps','ndc_sysRoles','sit').find_one()
+    for doc in results:
+        print(doc)
```

### Comparing `auto-test-common-2.0.7/common/plugin/data_bus.py` & `auto-test-common-2.0.8/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plugin/data_plugin.py` & `auto-test-common-2.0.8/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plugin/file_plugin.py` & `auto-test-common-2.0.8/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plugin/hooks_plugin.py` & `auto-test-common-2.0.8/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plugin/pytest_playwright.py` & `auto-test-common-2.0.8/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plugin/pytest_plugin.py` & `auto-test-common-2.0.8/common/plugin/pytest_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             # 关闭json读模式
             f.close()
             logger.info("修改测试报告完成")
 
     @classmethod
     def sendReport(self):
         DataBus.save_init_data()
-        change_allure_title()
+        PytestPlugin.change_allure_title()
         ATFPlugin.sendResult()
 
     @classmethod
     def generated_code(self, _url: str = '', _path: str = TEST_UI_PATH):
         if not DataProcess.isNotNull(_url):
             _url = get_system_key('url')
         test_case_dir = '{}'.format(_path)
@@ -427,15 +427,15 @@
         if DataProcess.isNotNull(_caseNo) and _caseNo.strip() != '00000':
             _title = _caseNo+"【用例编号未关联测试用例】"
             _info = _caseNo + "【用例编号未关联测试用例】"
             _caseTitleList = _caseTitleList + _caseNo.split(';')
         if DataProcess.isNotNull(_caseName):
             _title = _caseName+"【用例名称未关联测试用例】"
             _info = _caseName + "【用例名称未关联测试用例】"
-            _caseTitleList = _caseName.split(';')
+            _caseTitleList = _caseTitleList + _caseName.split(';')
         if DataProcess.isNotNull(_caseTitleList):
             _title = ""
             _info = ""
             print_debug(f"Allure用例名称:{_caseTitleList}")
             for temp in _caseTitleList:
                 info = ServicePlatForm.getCaseInfo(temp)
                 if _title.find(info['summary']+";") < 0:
```

### Comparing `auto-test-common-2.0.7/common/plugin/template_plugin.py` & `auto-test-common-2.0.8/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/common/plugin/yaml_plugin.py` & `auto-test-common-2.0.8/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.7/setup.py` & `auto-test-common-2.0.8/setup.py`

 * *Files identical despite different names*

