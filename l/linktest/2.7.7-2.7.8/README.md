# Comparing `tmp/linktest-2.7.7.tar.gz` & `tmp/linktest-2.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.7.7.tar", last modified: Sat May 11 14:51:50 2024, max compression
+gzip compressed data, was "linktest-2.7.8.tar", last modified: Sun May 12 07:37:59 2024, max compression
```

## Comparing `linktest-2.7.7.tar` & `linktest-2.7.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-11 14:51:50.131667 linktest-2.7.7/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-11 14:51:50.131429 linktest-2.7.7/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-11 14:51:50.129233 linktest-2.7.7/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-11 14:26:27.000000 linktest-2.7.7/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-11 14:27:40.000000 linktest-2.7.7/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-10 09:40:20.000000 linktest-2.7.7/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    37992 2024-05-11 14:45:31.000000 linktest-2.7.7/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102849 2024-05-11 08:42:16.000000 linktest-2.7.7/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-10 09:36:35.000000 linktest-2.7.7/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-11 14:26:34.000000 linktest-2.7.7/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-10 09:10:39.000000 linktest-2.7.7/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-11 14:51:50.131032 linktest-2.7.7/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-11 14:51:49.000000 linktest-2.7.7/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-11 14:51:50.131722 linktest-2.7.7/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-11 14:51:43.000000 linktest-2.7.7/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-12 07:37:59.593367 linktest-2.7.8/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-12 07:37:59.593102 linktest-2.7.8/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-12 07:37:59.590228 linktest-2.7.8/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-12 07:02:10.000000 linktest-2.7.8/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-12 07:32:42.000000 linktest-2.7.8/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38108 2024-05-12 06:57:42.000000 linktest-2.7.8/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102469 2024-05-12 06:48:37.000000 linktest-2.7.8/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-12 07:02:16.000000 linktest-2.7.8/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-12 05:43:01.000000 linktest-2.7.8/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-12 07:37:59.592711 linktest-2.7.8/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-12 07:37:59.000000 linktest-2.7.8/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-12 07:37:59.593421 linktest-2.7.8/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-12 07:37:54.000000 linktest-2.7.8/setup.py
```

### Comparing `linktest-2.7.7/linktest/appium_utils.py` & `linktest-2.7.8/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/auto_generate_testcase_list.py` & `linktest-2.7.8/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.7.8/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/base_testcase.py` & `linktest-2.7.8/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/clean_data.py` & `linktest-2.7.8/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/conver_xml_into_db.py` & `linktest-2.7.8/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/database_helper.py` & `linktest-2.7.8/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/date_utilities.py` & `linktest-2.7.8/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/doctor.py` & `linktest-2.7.8/linktest/doctor.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,15 @@
 #  23. AUTO_DOWNLOAD_CHROMEDRIVER (default value is False)
 #  24. ALWAYS_GENERATE_CURL (default value is False)
 #  25. AUTO_SCREENSHOT_ON_ACTION(default value is False)
 
 import logging
 
 # ------ testcase's log setting ------
-- LOG_FORMAT = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
 - LOG_LEVEL = logging.DEBUG # default value is DEBUG
-- LOG_TO_FILE = True # default value is True
 - LOG_TO_CONSOLE = True # default value is True
 
 
 class Environment(object):
     UAT = "uat"
     QA = "qa"
     LIVE = "www"
```

### Comparing `linktest-2.7.7/linktest/framework_log.py` & `linktest-2.7.8/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/generate_html_log.py` & `linktest-2.7.8/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/get_adb_devices.py` & `linktest-2.7.8/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/get_ios_devices_list.py` & `linktest-2.7.8/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/get_platform_info.py` & `linktest-2.7.8/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/get_project_info.py` & `linktest-2.7.8/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/html_report.py` & `linktest-2.7.8/linktest/html_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,16 @@
                                     // 添加到数组中
                                     selectedFailedCaseNames.push(textAfterSlash);
                                 }
                             }
                         }
                     });
                     
+                    selectedFailedCaseNames = Array.from(new Set(selectedFailedCaseNames));
+                    
                     // Join the array into a single string with commas separating the values
                     const textToCopy = selectedFailedCaseNames.join(' ');
                     
                     // Using the Clipboard API to copy text
                     navigator.clipboard.writeText(textToCopy).then(function() {
                         // Success action, e.g., showing a message
                         document.getElementById('copy_status_info').textContent = 'Copied!';
@@ -555,15 +557,15 @@
                                 failed_testcase.log_file_path.replace("test.log", "test.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
                     elif failed_testcase.rerun_tag == 1:
                         try:
                             report_file_handler.write(
-                                "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='left' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> &nbsp; [TXT </font> </a>" %
+                                "&nbsp; &nbsp; <strong style='color: darkorange; '>rerun Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='left' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> &nbsp; [TXT </font> </a>" %
                                 failed_testcase.log_file_path)
                             report_file_handler.write(
                                 " | &nbsp; <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> HTML]</font> </a>" %
                                 failed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
                         except BaseException:
                             print(traceback.format_exc())
```

### Comparing `linktest-2.7.7/linktest/logged_requests.py` & `linktest-2.7.8/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/main.py` & `linktest-2.7.8/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     - DEFAULT_BROWSER_NAME (default browser name for UI test cases; default value is "chrome")
     - HEAD_LESS (default value is False; runs the browser in headless mode)
     - WEBDRIVER_IMPLICIT_WAIT (default value is 10 seconds; maximum time the WebDriver should wait for an element to be present before throwing an exception)
     - LOG_TO_CONSOLE (default value is True; always logs to the console)
     - ALWAYS_GENERATE_CURL (default value is False; always generates cURL commands)
 
     # ------ Configuration Related to the TestCase's Log ------
-    - LOG_FORMAT = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
     - LOG_LEVEL = logging.DEBUG # default value is DEBUG
     - LOG_TO_CONSOLE = True # default value is True, Always log to file
 
 2. settings/testcase_tags.py
     - The Tags class is used to define all test case tags.
     - Assign a tag to each test case (tags can be any non-blank string; you can create tags based on your specific needs, such as "smoke", "nightly", "regression", "p1", "ignore", etc.)
     - Note: If a test case's tag contains "ignore", it will only be added to the ignore_testcase_list, even if its tag attribute contains other tag names (e.g. tag = "nightly, smoke, ignore")
@@ -385,37 +384,19 @@
 import time
 
 try:
     import settings
 except BaseException:
     raise ("No settings module found ....")
 
-try:
-    from settings import RERUN_FLAG
-except ImportError:
-    settings.RERUN_FLAG = False
-
-try:
-    from settings import QUEUE_SIZE
-except ImportError:
-    settings.QUEUE_SIZE = 1
-
-try:
-    from settings import LOG_FORMAT
-except ImportError:
-    settings.LOG_FORMAT = '%(asctime)s %(levelname)s %(filename)s %(lineno)d: %(message)s'
-
-
 # set Default time_zone = 'Asia/Shanghai'
-if hasattr(settings, "TIME_ZONE"):
-    if settings.TIME_ZONE:
-        os.environ['TZ'] = '%s' % settings.TIME_ZONE
+if getattr(settings, "TIME_ZONE", False):
+    os.environ['TZ'] = '%s' % settings.TIME_ZONE
 else:
     os.environ['TZ'] = 'Asia/Shanghai'
-    # os.environ['TZ'] = 'US/Central'
 
 if hasattr(time, 'tzset'):
     # https://docs.python.org/3/library/time.html#time.tzset
     # Availability: Unix
     time.tzset()
 
 import re
@@ -469,34 +450,30 @@
 from . import base_testcase
 from . import ui_testcase
 from . import ios_testcase
 from . import get_platform_info
 from . import appium_utils
 from . import android_testcase
 from . import api_testcase
-# from .scp_report_to_specified_path import scp_report_to_specified_path
 from .base_testcase import BaseTestCase
 from .get_adb_devices import get_adb_devices
 from .xml_report import convert_to_seconds
 
 from urllib.error import URLError
 
 PLATFORM_INFO = get_platform_info.get_platform_info()
 DEFAULT_SLEEP_TIME_FOR_MOBILE_TESTCASE = 2
 REAL_DEVICE = android_testcase.AndroidTestCase.REAL_DEVICE
 VIRTUAL_DEVICE = android_testcase.AndroidTestCase.VIRTUAL_DEVICE
 
 ####### testcase log settings start #######
 # Default values
-default_log_format = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
-default_level = logging.DEBUG
-
+log_format = '%(asctime)s %(levelname)s %(filename)s %(lineno)d: %(message)s'
 # Read from settings
-log_format = getattr(settings, 'LOG_FORMAT', default_log_format)
-level = getattr(settings, 'LOG_LEVEL', default_level)
+log_level = getattr(settings, 'LOG_LEVEL', logging.DEBUG)
 
 ####### testcase log settings end #######
 
 
 class TestCaseExecutor(threading.Thread):
     failed_testcases = []
     passed_testcases = []
@@ -514,17 +491,16 @@
         threading.Thread.__init__(self)
         self.output_folder = output_folder
         self.begin_time = begin_time
         self.queue = testcase_queue
         self.total_testcases_count = total_testcases_count
         TestCaseExecutor.testcase_queue = self.queue
 
-        if hasattr(settings, "RERUN_FLAG"):
-            if settings.RERUN_FLAG:
-                TestCaseExecutor.rerun_testcase_queue = collections.deque()
+        if getattr(settings, "RERUN_FLAG", False):
+            TestCaseExecutor.rerun_testcase_queue = collections.deque()
 
     def create_logger(self, logger_ref, testcase_full_folder, logger_name):
         # Initialize handlers list
         handlers = []
 
         with TestCaseExecutor.create_log_lock:
             importlib.reload(logging)
@@ -540,15 +516,15 @@
             # Add StreamHandler if LOG_TO_CONSOLE is set to True in settings
             if getattr(settings, 'LOG_TO_CONSOLE', True):
                 handlers.append(logging.StreamHandler(sys.stdout))
 
             # Define basic configuration
             logging.basicConfig(
                 # Define logging level
-                level=level,
+                level=log_level,
                 # Declare the object we created to format the log messages
                 format=log_format,
                 # Declare handlers
                 handlers=handlers
             )
 
             logger = logging.getLogger(logger_ref)
@@ -1241,15 +1217,15 @@
                             TestCaseExecutor.jenkins_job_name = \
                                 project_info.project_path.split(os.sep + "jenkins" + os.sep + "workspace" + os.sep)[
                                     1].split(os.sep)[0]
 
                 try:
                     print(" - (Passed:%s | Failed:%s | Remaining:%s | Total:%s) - Testcase execution for '%s' has completed." % (
                             len(TestCaseExecutor.passed_testcases),
-                            len(TestCaseExecutor.failed_testcases),
+                            int(len(TestCaseExecutor.failed_testcases)/2) if getattr(settings, "RERUN_FLAG", False) else len(TestCaseExecutor.failed_testcases),
                             len(TestCaseExecutor.testcase_queue),
                             self.total_testcases_count,
                             testcase.__name__))
 
                 except BaseException:
                     pass
 
@@ -1984,25 +1960,26 @@
         for testcase_executor in testcase_executor_list:
             time.sleep(0.5)
             testcase_executor.start()
 
         for testcase_executor in testcase_executor_list:
             testcase_executor.join()
 
-        print(os.linesep + "****************** TestCases Passed: %s, TestCases Failed: %s, Total TestCases Executed: %s ******************" % (
-                len(TestCaseExecutor.passed_testcases),len(TestCaseExecutor.failed_testcases), total_testcases_count))
-
+        final_failed_testcase_list = []
         if len(TestCaseExecutor.failed_testcases) > 0:
-            failed_testcase_name_list = "%s" % os.linesep
-
             for tc in TestCaseExecutor.failed_testcases:
-                failed_testcase_name_list += tc.__class__.__name__ + os.linesep
+                final_failed_testcase_list.append(max(set(tc.packages.split(",")), key=len) + os.sep + tc.__class__.__name__)
+                
+            # remove duplicate testcases in failed_testcase_name_list
+            final_failed_testcase_list = list(set(final_failed_testcase_list))
 
-            print("Failed TestCase List:")
-            print(failed_testcase_name_list)
+        print(os.linesep + "****************** TestCases Passed: %s, TestCases Failed: %s, Total TestCases Executed: %s ******************" % (
+                len(TestCaseExecutor.passed_testcases),len(final_failed_testcase_list), total_testcases_count))
+        print("Failed TestCase List:")
+        print(final_failed_testcase_list)
 
         if not settings.DEBUG_RUN:
             close_browsers_and_webdrivers()
         else:
             clean_appium_env()
 
 
@@ -2044,15 +2021,15 @@
                                          PLATFORM_INFO,
                                          len(BaseTestCase.GlobalDataList) > 0,
                                          True)
                 except BaseException:
                     traceback.print_exc()
 
             print(
-                "=*=*=" * 20 + os.linesep + "Execution has been completed. For further details, please refer to the accompanying HTML report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
+                "=*=*=" * 20 + os.linesep + "Execution has been completed. For further details, please refer to the accompanying HTML report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html" + os.linesep)
 
             # save the execution summary into DB (environment, total_execution_time,
             try:
                 import linktest
                 from . import database_helper
 
                 if getattr(settings, "SAVE_LOG_TO_DB", False):
@@ -2080,16 +2057,16 @@
         # 如果最后执行完所有的testcase 并且GlobalDataList 不为空，则自动保存GlobalDataList
         if len(BaseTestCase.GlobalDataList) > 0:
             file_path = os.path.join(output_folder, "global_data_list.py")
             try:
                 with open(file_path, "w", encoding='utf-8') as f:
                     f.write("global_data_list = " + json.dumps(BaseTestCase.GlobalDataList, indent=4, ensure_ascii=False))
 
-                print("Global Data List File Path:")
-                print(file_path)
+                # print("Global Data List File Path:")
+                # print(file_path)
             except OSError as e:
                 print("Error writing global_data_list to file:")
                 print(str(e))
             except Exception as e:
                 print("An unexpected error occurred:")
                 print(str(e))
```

### Comparing `linktest-2.7.7/linktest/memory_usage.py` & `linktest-2.7.8/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/re_func.py` & `linktest-2.7.8/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/run.py` & `linktest-2.7.8/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/run_testcase_thread.py` & `linktest-2.7.8/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/scp_report_to_specified_path.py` & `linktest-2.7.8/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/selenium_helper.py` & `linktest-2.7.8/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/timeout_thread.py` & `linktest-2.7.8/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/ui_testcase.py` & `linktest-2.7.8/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/update_config.py` & `linktest-2.7.8/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/webdriver_wrapper.py` & `linktest-2.7.8/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/webdriver_wrapper_chrome.py` & `linktest-2.7.8/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/webdriver_wrapper_edge.py` & `linktest-2.7.8/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/webdriver_wrapper_firefox.py` & `linktest-2.7.8/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/webdriver_wrapper_ie.py` & `linktest-2.7.8/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/webdriver_wrapper_safari.py` & `linktest-2.7.8/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest/xml_report.py` & `linktest-2.7.8/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.7/linktest.egg-info/SOURCES.txt` & `linktest-2.7.8/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

