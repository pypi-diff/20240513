# Comparing `tmp/zjbbintest-2.4.tar.gz` & `tmp/zjbbintest-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zjbbintest-2.4.tar", last modified: Fri May 10 11:48:16 2024, max compression
+gzip compressed data, was "dist/zjbbintest-2.5.tar", last modified: Mon May 13 13:39:38 2024, max compression
```

## Comparing `zjbbintest-2.4.tar` & `zjbbintest-2.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:48:16.040704 zjbbintest-2.4/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-10 11:48:16.040534 zjbbintest-2.4/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      514 2024-05-07 11:52:14.000000 zjbbintest-2.4/README.md
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-10 11:48:16.040751 zjbbintest-2.4/setup.cfg
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      603 2024-05-10 11:48:12.000000 zjbbintest-2.4/setup.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:48:16.035426 zjbbintest-2.4/zjbbintest/
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:48:16.036645 zjbbintest-2.4/zjbbintest/Actuator/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-2.4/zjbbintest/Actuator/__init__.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:48:16.036881 zjbbintest-2.4/zjbbintest/Actuator/bin_test_case/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:16.000000 zjbbintest-2.4/zjbbintest/Actuator/bin_test_case/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    13665 2024-05-10 11:48:06.000000 zjbbintest-2.4/zjbbintest/Actuator/bin_test_case/bin_test_case.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:48:16.037142 zjbbintest-2.4/zjbbintest/Actuator/bin_test_exception/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:22.000000 zjbbintest-2.4/zjbbintest/Actuator/bin_test_exception/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-2.4/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:48:16.039109 zjbbintest-2.4/zjbbintest/Actuator/utils/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-2.4/zjbbintest/Actuator/utils/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      973 2024-05-10 09:44:52.000000 zjbbintest-2.4/zjbbintest/Actuator/utils/action_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6643 2024-05-10 09:44:52.000000 zjbbintest-2.4/zjbbintest/Actuator/utils/assert_execution.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3733 2024-05-08 06:54:26.000000 zjbbintest-2.4/zjbbintest/Actuator/utils/format_check.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-2.4/zjbbintest/Actuator/utils/processing_path.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     7608 2024-05-10 09:44:52.000000 zjbbintest-2.4/zjbbintest/Actuator/utils/requestor.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)    12193 2024-05-10 09:44:52.000000 zjbbintest-2.4/zjbbintest/Actuator/utils/string_dynamic_run.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:48:16.039611 zjbbintest-2.4/zjbbintest/Analysis/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 14:37:18.000000 zjbbintest-2.4/zjbbintest/Analysis/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     2596 2024-05-09 12:16:14.000000 zjbbintest-2.4/zjbbintest/Analysis/har2json.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3188 2024-05-10 11:05:40.000000 zjbbintest-2.4/zjbbintest/Analysis/replace_values.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:48:16.040217 zjbbintest-2.4/zjbbintest/Template/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 05:24:09.000000 zjbbintest-2.4/zjbbintest/Template/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1255 2024-05-10 08:40:52.000000 zjbbintest-2.4/zjbbintest/Template/bintest_template.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1172 2024-05-07 09:08:55.000000 zjbbintest-2.4/zjbbintest/Template/report_template.html
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:50:15.000000 zjbbintest-2.4/zjbbintest/__init__.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     9805 2024-05-08 12:19:43.000000 zjbbintest-2.4/zjbbintest/bintest.py
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      501 2024-04-23 04:49:02.000000 zjbbintest-2.4/zjbbintest/bintest_data.py
-drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-10 11:48:16.036501 zjbbintest-2.4/zjbbintest.egg-info/
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-10 11:48:16.000000 zjbbintest-2.4/zjbbintest.egg-info/PKG-INFO
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1019 2024-05-10 11:48:16.000000 zjbbintest-2.4/zjbbintest.egg-info/SOURCES.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-10 11:48:16.000000 zjbbintest-2.4/zjbbintest.egg-info/dependency_links.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)      720 2024-05-10 11:48:16.000000 zjbbintest-2.4/zjbbintest.egg-info/requires.txt
--rw-r--r--   0 zhangjiabin01   (501) staff       (20)       11 2024-05-10 11:48:16.000000 zjbbintest-2.4/zjbbintest.egg-info/top_level.txt
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-13 13:39:38.104562 zjbbintest-2.5/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-13 13:39:38.104430 zjbbintest-2.5/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      514 2024-05-07 11:52:14.000000 zjbbintest-2.5/README.md
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       38 2024-05-13 13:39:38.104601 zjbbintest-2.5/setup.cfg
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      603 2024-05-13 13:39:36.000000 zjbbintest-2.5/setup.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-13 13:39:38.099207 zjbbintest-2.5/zjbbintest/
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-13 13:39:38.100325 zjbbintest-2.5/zjbbintest/Actuator/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:19:26.000000 zjbbintest-2.5/zjbbintest/Actuator/__init__.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-13 13:39:38.100544 zjbbintest-2.5/zjbbintest/Actuator/bin_test_case/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:16.000000 zjbbintest-2.5/zjbbintest/Actuator/bin_test_case/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    13665 2024-05-10 11:48:06.000000 zjbbintest-2.5/zjbbintest/Actuator/bin_test_case/bin_test_case.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-13 13:39:38.101197 zjbbintest-2.5/zjbbintest/Actuator/bin_test_exception/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:51:22.000000 zjbbintest-2.5/zjbbintest/Actuator/bin_test_exception/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3663 2024-04-30 03:43:11.000000 zjbbintest-2.5/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-13 13:39:38.103171 zjbbintest-2.5/zjbbintest/Actuator/utils/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-04-16 03:21:41.000000 zjbbintest-2.5/zjbbintest/Actuator/utils/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      973 2024-05-10 09:44:52.000000 zjbbintest-2.5/zjbbintest/Actuator/utils/action_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     6407 2024-05-11 07:03:52.000000 zjbbintest-2.5/zjbbintest/Actuator/utils/assert_execution.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     3734 2024-05-12 15:28:29.000000 zjbbintest-2.5/zjbbintest/Actuator/utils/format_check.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1110 2024-04-22 09:45:48.000000 zjbbintest-2.5/zjbbintest/Actuator/utils/processing_path.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     7611 2024-05-11 07:15:47.000000 zjbbintest-2.5/zjbbintest/Actuator/utils/requestor.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    12193 2024-05-10 09:44:52.000000 zjbbintest-2.5/zjbbintest/Actuator/utils/string_dynamic_run.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-13 13:39:38.103586 zjbbintest-2.5/zjbbintest/Analysis/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 14:37:18.000000 zjbbintest-2.5/zjbbintest/Analysis/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    11073 2024-05-13 13:38:33.000000 zjbbintest-2.5/zjbbintest/Analysis/har2json.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    11276 2024-05-13 13:34:08.000000 zjbbintest-2.5/zjbbintest/Analysis/replace_values.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-13 13:39:38.104116 zjbbintest-2.5/zjbbintest/Template/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 05:24:09.000000 zjbbintest-2.5/zjbbintest/Template/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1255 2024-05-10 08:40:52.000000 zjbbintest-2.5/zjbbintest/Template/bintest_template.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1172 2024-05-07 09:08:55.000000 zjbbintest-2.5/zjbbintest/Template/report_template.html
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        0 2024-05-08 06:50:15.000000 zjbbintest-2.5/zjbbintest/__init__.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)    12463 2024-05-13 13:31:46.000000 zjbbintest-2.5/zjbbintest/bintest.py
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      501 2024-04-23 04:49:02.000000 zjbbintest-2.5/zjbbintest/bintest_data.py
+drwxr-xr-x   0 zhangjiabin01   (501) staff       (20)        0 2024-05-13 13:39:38.100201 zjbbintest-2.5/zjbbintest.egg-info/
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      208 2024-05-13 13:39:38.000000 zjbbintest-2.5/zjbbintest.egg-info/PKG-INFO
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)     1019 2024-05-13 13:39:38.000000 zjbbintest-2.5/zjbbintest.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)        1 2024-05-13 13:39:38.000000 zjbbintest-2.5/zjbbintest.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)      720 2024-05-13 13:39:38.000000 zjbbintest-2.5/zjbbintest.egg-info/requires.txt
+-rw-r--r--   0 zhangjiabin01   (501) staff       (20)       11 2024-05-13 13:39:38.000000 zjbbintest-2.5/zjbbintest.egg-info/top_level.txt
```

### Comparing `zjbbintest-2.4/README.md` & `zjbbintest-2.5/README.md`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.4/setup.py` & `zjbbintest-2.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     for line in file:
         dependencies.append(line.strip())
 
 print(dependencies)
 
 setup(
     name='zjbbintest',
-    version='2.4',
+    version='2.5',
     author="zhangjiabin01",
     author_email="zhangjiabin01@baidu.com",
     description="bintest自动化框架",
     packages=find_packages(),
     package_data={
             'zjbbintest': ['Template/*'],  # 包含my_package中的templates文件夹下的所有文件
         },
```

### Comparing `zjbbintest-2.4/zjbbintest/Actuator/bin_test_case/bin_test_case.py` & `zjbbintest-2.5/zjbbintest/Actuator/bin_test_case/bin_test_case.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.4/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py` & `zjbbintest-2.5/zjbbintest/Actuator/bin_test_exception/bin_test_exception.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.4/zjbbintest/Actuator/utils/action_execution.py` & `zjbbintest-2.5/zjbbintest/Actuator/utils/action_execution.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.4/zjbbintest/Actuator/utils/assert_execution.py` & `zjbbintest-2.5/zjbbintest/Actuator/utils/assert_execution.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,36 +89,30 @@
         :param case_var_dict:
         :param req_dict:
         :param resp_dict:
         :return:
         """
         self.expect_data, _ = StringDynamicRun(self.expect_data, case_var_dict, req_dict, resp_dict).run()
         self.actual_data, _ = StringDynamicRun(self.actual_data, case_var_dict, req_dict, resp_dict).run()
-        if self.expect_data is None:
-            raise BTAssertDictFormatException(self, "expect")
-        if self.assert_name is None:
-            raise BTAssertDictFormatException(self, "operator")
-        if self.actual_data is None:
-            raise BTAssertDictFormatException(self, "actual")
 
     @staticmethod
     def create_obj_by_dict(assert_dict):
         """
         根据断言字典创建断言对象
         :param assert_dict:
         :return:
         """
         assert_name = assert_dict.get("operator")
         expect_data = assert_dict.get("expect")
         actual_data = assert_dict.get("actual")
-        if expect_data is None:
+        if expect_data is None or expect_data == "":
             raise BTAssertDictFormatException(assert_dict, "expect")
-        if assert_name is None:
+        if assert_name is None or assert_name == "":
             raise BTAssertDictFormatException(assert_dict, "operator")
-        if actual_data is None:
+        if actual_data is None or actual_data == "":
             raise BTAssertDictFormatException(assert_dict, "actual")
         return AssertExecutor(expect_data, actual_data, assert_name)
 
 
 class BatchAssertExecutor:
     """
     批量断言执行器
```

### Comparing `zjbbintest-2.4/zjbbintest/Actuator/utils/format_check.py` & `zjbbintest-2.5/zjbbintest/Actuator/utils/format_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                                          "OPTIONS", "PATCH", "CONNECT", "TRACE",
                                          "get", "post", "put", "delete", "head",
                                          "options", "patch", "connect", "trace"]
                             },
                             "headers": {
                                 "type": "object"
                             },
-                            "param": {
+                            "params": {
                                 "type": "object"
                             },
                             "body": {
                                 "type": "object"
                             }
                         },
                         "required": ["url", "path", "method"]
```

### Comparing `zjbbintest-2.4/zjbbintest/Actuator/utils/processing_path.py` & `zjbbintest-2.5/zjbbintest/Actuator/utils/processing_path.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.4/zjbbintest/Actuator/utils/requestor.py` & `zjbbintest-2.5/zjbbintest/Actuator/utils/requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,17 +181,17 @@
             self.content = json.loads(self.content)
             self.text = json.loads(self.text)
         except Exception as e:
             print(f"解析响应内容失败，原因：{e}")
             pass
         return {
             "status_code": self.status_code,
-            "text": self.text,
-            "content": self.content,
-            "response_headers": self.response_headers
+            "text": self.text
+            # "content": self.content,
+            # "response_headers": self.response_headers
         }
 
 
 def convert_to_str(dictionary):
     """
     将字典中的key和value都转化为字符串
     :param dictionary:
```

### Comparing `zjbbintest-2.4/zjbbintest/Actuator/utils/string_dynamic_run.py` & `zjbbintest-2.5/zjbbintest/Actuator/utils/string_dynamic_run.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.4/zjbbintest/Template/bintest_template.py` & `zjbbintest-2.5/zjbbintest/Template/bintest_template.py`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.4/zjbbintest/Template/report_template.html` & `zjbbintest-2.5/zjbbintest/Template/report_template.html`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.4/zjbbintest/bintest.py` & `zjbbintest-2.5/zjbbintest/bintest.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,21 +9,27 @@
 from datetime import datetime
 import json
 import os
 from functools import wraps
 from inspect import getmembers, isfunction
 
 from zjbbintest.Actuator.bin_test_case.bin_test_case import BinTestCase
-from zjbbintest.Actuator.bin_test_exception.bin_test_exception import BTFuncFormatCheckException, BTAssertFormatCheckException, \
+from zjbbintest.Actuator.bin_test_exception.bin_test_exception import BTFuncFormatCheckException, \
+    BTAssertFormatCheckException, \
     BTActionFormatCheckException, BTCaseNotLoadException
 from zjbbintest.Actuator.utils.processing_path import get_json_files_in_directories
+from zjbbintest.Analysis.har2json import save_json, have_easy_har, analysis_har_list, \
+    parse_har_list
+from zjbbintest.Analysis.replace_values import get_req_bt_str_map, get_resp_bt_str_map, save_conf_var, \
+    get_conf_bt_str_map, case_json_replace_bintest_var
 from zjbbintest.Template.bintest_template import render_report
 from zjbbintest.bintest_data import BinTestData
 import logging
 
+
 # config_dict = {}
 # func_dict = {}
 # assert_dict = {}
 # action_dict = {}
 # run_case_list = []
 # case_load_flag = False
 
@@ -257,7 +263,69 @@
             case_res = bin_case.run()
             case_res_list.append(case_res)
         # 生成测试报告
         render_report(case_res_list, now_time, report_path)
     else:
         raise BTCaseNotLoadException()
 
+
+def rebuild(har_file_path, conf_ini_file_path, case_dir_path=''):
+    """
+    根据har_file_path重建case，将其放在case_dir_path目录下
+    case_dir_path目录下，应该存放三个文件
+    1 替换后的case的json形式 xxx_case.json
+    2 变量的bt_str映射关系 xxx_bt_str.json
+    3 提取的请求和响应信息 xxx_req_resp.json
+    :param har_file_path:
+    :param conf_ini_file_path
+    :param case_dir_path:
+    :return: 
+    """
+    # 判断har_file_path是否存在
+    if not os.path.exists(har_file_path):
+        raise FileNotFoundError(f"har文件 {har_file_path} 不存在。")
+    if not os.path.exists(conf_ini_file_path):
+        raise FileNotFoundError(f"配置文件 {conf_ini_file_path} 不存在。")
+    # 获取文件名
+    file_name = os.path.basename(har_file_path)
+    # 获取路径
+    dir_name = os.path.dirname(har_file_path)
+    # 获取基础名（不含后缀）
+    base_name, _ = os.path.splitext(file_name)
+
+    easy_har_list = have_easy_har(har_file_path)
+    case_json = analysis_har_list(easy_har_list)
+    req_dict, resp_dict = parse_har_list(easy_har_list)
+    conf_dict = save_conf_var(conf_ini_file_path)
+    req_bt_str_map = get_req_bt_str_map(req_dict)
+    resp_bt_str_map = get_resp_bt_str_map(resp_dict)
+    conf_bt_str_map = get_conf_bt_str_map(conf_dict)
+    new_case_json = case_json_replace_bintest_var(case_json, conf_bt_str_map, req_bt_str_map, resp_bt_str_map)
+    req_resp_json = {}
+    for req_key, req in req_dict.items():
+        req_resp_json[req_key] = {
+            'request': req,
+            'response': resp_dict.get(req_key)
+        }
+    bt_str_map_json = {
+        'conf': conf_bt_str_map,
+        'req': req_bt_str_map,
+        'resp': resp_bt_str_map
+    }
+    if not case_dir_path:
+        # 如果case_dir_path为空，则放在当前目录下的case目录下
+        case_dir_path = dir_name + f'/{base_name}'
+    case_full_path = case_dir_path + f'/{base_name}_case.json'
+    bt_str_map_full_path = case_dir_path + f'/{base_name}_bt_str.json'
+    req_resp_full_path = case_dir_path + f'/{base_name}_req_resp.json'
+    # 创建case_dir_path目录
+    if not os.path.exists(case_dir_path):
+        os.makedirs(case_dir_path)
+    # 保存
+    save_json(new_case_json, case_full_path)
+    save_json(bt_str_map_json, bt_str_map_full_path)
+    save_json(req_resp_json, req_resp_full_path)
+
+
+
+
+
```

### Comparing `zjbbintest-2.4/zjbbintest.egg-info/SOURCES.txt` & `zjbbintest-2.5/zjbbintest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zjbbintest-2.4/zjbbintest.egg-info/requires.txt` & `zjbbintest-2.5/zjbbintest.egg-info/requires.txt`

 * *Files identical despite different names*

