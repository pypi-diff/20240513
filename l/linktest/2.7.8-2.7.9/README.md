# Comparing `tmp/linktest-2.7.8.tar.gz` & `tmp/linktest-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.7.8.tar", last modified: Sun May 12 07:37:59 2024, max compression
+gzip compressed data, was "linktest-2.7.9.tar", last modified: Mon May 13 05:54:22 2024, max compression
```

## Comparing `linktest-2.7.8.tar` & `linktest-2.7.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-12 07:37:59.593367 linktest-2.7.8/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-12 07:37:59.593102 linktest-2.7.8/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-12 07:37:59.590228 linktest-2.7.8/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-12 07:02:10.000000 linktest-2.7.8/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-12 07:32:42.000000 linktest-2.7.8/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38108 2024-05-12 06:57:42.000000 linktest-2.7.8/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102469 2024-05-12 06:48:37.000000 linktest-2.7.8/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-12 07:02:16.000000 linktest-2.7.8/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-12 07:37:59.592711 linktest-2.7.8/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-12 07:37:59.593421 linktest-2.7.8/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-12 07:37:54.000000 linktest-2.7.8/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-13 05:54:22.311805 linktest-2.7.9/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-13 05:54:22.311226 linktest-2.7.9/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-13 05:54:22.306775 linktest-2.7.9/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-12 15:05:15.000000 linktest-2.7.9/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-12 14:47:28.000000 linktest-2.7.9/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38132 2024-05-12 15:03:30.000000 linktest-2.7.9/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102112 2024-05-12 14:11:01.000000 linktest-2.7.9/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-12 15:05:20.000000 linktest-2.7.9/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-12 14:00:45.000000 linktest-2.7.9/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-13 05:54:22.310367 linktest-2.7.9/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-13 05:54:21.000000 linktest-2.7.9/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-13 05:54:22.311943 linktest-2.7.9/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-13 05:54:16.000000 linktest-2.7.9/setup.py
```

### Comparing `linktest-2.7.8/linktest/appium_utils.py` & `linktest-2.7.9/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/auto_generate_testcase_list.py` & `linktest-2.7.9/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.7.9/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/base_testcase.py` & `linktest-2.7.9/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/clean_data.py` & `linktest-2.7.9/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/conver_xml_into_db.py` & `linktest-2.7.9/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/database_helper.py` & `linktest-2.7.9/linktest/database_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,19 +41,24 @@
                screenshot_list_for_db,
                testcase_start_time)
 
         print("-------- executed done insert_tc_sql: %s" % insert_tc_sql)
         cousor.execute(insert_tc_sql)
     except BaseException:
         traceback.print_exc()
-        print(traceback.format_exc())
     finally:
-        conn.commit()
-        cousor.close()
-        conn.close()
+        try:
+            if 'conn' in locals() and conn is not None:
+                conn.commit()
+            if 'cursor' in locals() and cursor is not None:
+                cursor.close()
+            if 'conn' in locals() and conn is not None:
+                conn.close()
+        except BaseException as e:
+            traceback.print_exc()
 
 
 def insert_execution_summary_log(execution_id,
                                  environment=None,
                                  os=None,
                                  automation_framework_version=None,
                                  total_execution_time=None,
@@ -82,24 +87,28 @@
                total_testcases_count,
                pass_testcases_count,
                fail_testcases_count,
                rerun_flag,
                socket.getfqdn()
                )
 
-        # print("insert_execution_summary_sql: %s" % insert_execution_summary_sql)
         print("======== saved execution summary into database ========")
         cousor.execute(insert_execution_summary_sql)
     except BaseException:
         traceback.print_exc()
-        print(traceback.format_exc())
     finally:
-        conn.commit()
-        cousor.close()
-        conn.close()
+        try:
+            if 'conn' in locals() and conn is not None:
+                conn.commit()
+            if 'cursor' in locals() and cursor is not None:
+                cursor.close()
+            if 'conn' in locals() and conn is not None:
+                conn.close()
+        except BaseException as e:
+            traceback.print_exc()
 
 
 def save_execution_log(passed_testcases, failed_testcases, output_folder, project_name, jenkins_job_name="", rerun_flag=False):
     try:
         conn = pymysql.connect(user='root', password='password', database='testdb')
         cursor = conn.cursor()
 
@@ -138,17 +147,21 @@
                            testcase.packages,
                            jenkins_job_name,
                            testcase.rerun_tag,
                            conn.escape_string(error_message) if error_message else "",
                            screenshot_list_for_db,
                            testcase.testcase_start_time)
 
-            # print("-------- executed done insert_tc_sql: %s" % insert_tc_sql)
             cursor.execute(insert_tc_sql)
         print("-------- saved execution details into database --------")
     except BaseException:
         traceback.print_exc()
-        print(traceback.format_exc())
     finally:
-        conn.commit()
-        cursor.close()
-        conn.close()
+        try:
+            if 'conn' in locals() and conn is not None:
+                conn.commit()
+            if 'cursor' in locals() and cursor is not None:
+                cursor.close()
+            if 'conn' in locals() and conn is not None:
+                conn.close()
+        except BaseException as e:
+            traceback.print_exc()
```

### Comparing `linktest-2.7.8/linktest/date_utilities.py` & `linktest-2.7.9/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/doctor.py` & `linktest-2.7.9/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/framework_log.py` & `linktest-2.7.9/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/generate_html_log.py` & `linktest-2.7.9/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/get_adb_devices.py` & `linktest-2.7.9/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/get_ios_devices_list.py` & `linktest-2.7.9/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/get_platform_info.py` & `linktest-2.7.9/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/get_project_info.py` & `linktest-2.7.9/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/html_report.py` & `linktest-2.7.9/linktest/html_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
                             </tr>
                             <tr>
                                 <th>OS</th>
                                 <td align='center'>%s</td>
                             </tr>
                             <tr>
                                 <th>Framework</th>
-                                <td align='center'><a target="_blank" href="https://plugins.jetbrains.com/plugin/21600-linktest/versions">linktest %s</a></td>
+                                <td align='center'><a target="_blank" style="color: #3366C5;" href="https://plugins.jetbrains.com/plugin/21600-linktest/versions">linktest %s</a></td>
                             </tr>
                         </table>
                     </td>
                 </tr>
             </table>
             """ % (
                 start_time.strftime("%Y-%m-%d %H:%M:%S"),
```

### Comparing `linktest-2.7.8/linktest/logged_requests.py` & `linktest-2.7.9/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/main.py` & `linktest-2.7.9/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1991,72 +1991,70 @@
                                                  begin_time
                                                  )
                 print("generate xml report done...")
         except BaseException:
             traceback.print_exc()
             with open(output_folder + "error_log.txt", "w") as file_obj:
                 file_obj.write(traceback.format_exc())
-        finally:
-            try:
-                rerun_flag = getattr(settings, "RERUN_FLAG", False)
 
-                if getattr(settings, "SAVE_LOG_TO_DB", False):
-                    from . import database_helper
+        try:
+            rerun_flag = getattr(settings, "RERUN_FLAG", False)
 
-                    database_helper.save_execution_log(passed_testcases=TestCaseExecutor.passed_testcases,
-                                                       failed_testcases=TestCaseExecutor.failed_testcases,
-                                                       output_folder=output_folder,
-                                                       project_name=project_info.project_name,
-                                                       jenkins_job_name=TestCaseExecutor.jenkins_job_name,
-                                                       rerun_flag=rerun_flag
-                                                       )
-            except BaseException:
-                traceback.print_exc()
-            finally:
-                try:
-                    html_report.Reporter(output_folder,
-                                         TestCaseExecutor.passed_testcases,
-                                         TestCaseExecutor.failed_testcases,
-                                         TestCaseExecutor.error_testcases,
-                                         begin_time,
-                                         PLATFORM_INFO,
-                                         len(BaseTestCase.GlobalDataList) > 0,
-                                         True)
-                except BaseException:
-                    traceback.print_exc()
+            if getattr(settings, "SAVE_LOG_TO_DB", False):
+                from . import database_helper
 
-            print(
-                "=*=*=" * 20 + os.linesep + "Execution has been completed. For further details, please refer to the accompanying HTML report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html" + os.linesep)
+                database_helper.save_execution_log(passed_testcases=TestCaseExecutor.passed_testcases,
+                                                   failed_testcases=TestCaseExecutor.failed_testcases,
+                                                   output_folder=output_folder,
+                                                   project_name=project_info.project_name,
+                                                   jenkins_job_name=TestCaseExecutor.jenkins_job_name,
+                                                   rerun_flag=rerun_flag)
+        except BaseException:
+            traceback.print_exc()
 
-            # save the execution summary into DB (environment, total_execution_time,
-            try:
-                import linktest
-                from . import database_helper
+        try:
+            html_report.Reporter(output_folder,
+                                 TestCaseExecutor.passed_testcases,
+                                 TestCaseExecutor.failed_testcases,
+                                 TestCaseExecutor.error_testcases,
+                                 begin_time,
+                                 PLATFORM_INFO,
+                                 len(BaseTestCase.GlobalDataList) > 0,
+                                 True)
+        except BaseException:
+            traceback.print_exc()
+
+        print(
+            "=*=*=" * 20 + os.linesep + "Execution has been completed. For further details, please refer to the accompanying HTML report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html" + os.linesep)
 
-                if getattr(settings, "SAVE_LOG_TO_DB", False):
-                    end_time = datetime.datetime.now()
-                    execution_time = end_time - begin_time
-
-                    database_helper.insert_execution_summary_log(
-                        execution_id=output_folder.split(os.sep + "output" + os.sep)[1],
-                        environment=settings.ENVIRONMENT,
-                        os=PLATFORM_INFO,
-                        automation_framework_version=linktest.__version__,
-                        total_execution_time=execution_time,
-                        jenkins_job_name=None,
-                        project_name=project_info.project_name,
-                        total_testcases_count=total_testcases_count,
-                        pass_testcases_count=len(TestCaseExecutor.passed_testcases),
-                        fail_testcases_count=total_testcases_count - len(TestCaseExecutor.passed_testcases),
-                        rerun_flag=1 if rerun_flag else 0
-                    )
-            except BaseException:
-                traceback.print_exc()
-            finally:
-                pass
+        # save the execution summary into DB (environment, total_execution_time,
+        try:
+            import linktest
+            from . import database_helper
+
+            if getattr(settings, "SAVE_LOG_TO_DB", False):
+                end_time = datetime.datetime.now()
+                execution_time = end_time - begin_time
+
+                database_helper.insert_execution_summary_log(
+                    execution_id=output_folder.split(os.sep + "output" + os.sep)[1],
+                    environment=settings.ENVIRONMENT,
+                    os=PLATFORM_INFO,
+                    automation_framework_version=linktest.__version__,
+                    total_execution_time=execution_time,
+                    jenkins_job_name=None,
+                    project_name=project_info.project_name,
+                    total_testcases_count=total_testcases_count,
+                    pass_testcases_count=len(TestCaseExecutor.passed_testcases),
+                    fail_testcases_count=total_testcases_count - len(TestCaseExecutor.passed_testcases),
+                    rerun_flag=1 if rerun_flag else 0
+                )
+        except BaseException:
+            traceback.print_exc()
+        
 
         # 如果最后执行完所有的testcase 并且GlobalDataList 不为空，则自动保存GlobalDataList
         if len(BaseTestCase.GlobalDataList) > 0:
             file_path = os.path.join(output_folder, "global_data_list.py")
             try:
                 with open(file_path, "w", encoding='utf-8') as f:
                     f.write("global_data_list = " + json.dumps(BaseTestCase.GlobalDataList, indent=4, ensure_ascii=False))
```

### Comparing `linktest-2.7.8/linktest/memory_usage.py` & `linktest-2.7.9/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/re_func.py` & `linktest-2.7.9/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/run.py` & `linktest-2.7.9/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/run_testcase_thread.py` & `linktest-2.7.9/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/scp_report_to_specified_path.py` & `linktest-2.7.9/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/selenium_helper.py` & `linktest-2.7.9/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/timeout_thread.py` & `linktest-2.7.9/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/ui_testcase.py` & `linktest-2.7.9/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/update_config.py` & `linktest-2.7.9/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/webdriver_wrapper.py` & `linktest-2.7.9/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/webdriver_wrapper_chrome.py` & `linktest-2.7.9/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/webdriver_wrapper_edge.py` & `linktest-2.7.9/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/webdriver_wrapper_firefox.py` & `linktest-2.7.9/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/webdriver_wrapper_ie.py` & `linktest-2.7.9/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/webdriver_wrapper_safari.py` & `linktest-2.7.9/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest/xml_report.py` & `linktest-2.7.9/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.8/linktest.egg-info/SOURCES.txt` & `linktest-2.7.9/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

