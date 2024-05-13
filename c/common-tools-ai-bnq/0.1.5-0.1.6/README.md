# Comparing `tmp/common-tools-ai-bnq-0.1.5.tar.gz` & `tmp/common-tools-ai-bnq-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.1.5.tar", last modified: Fri May 10 08:16:10 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.1.6.tar", last modified: Mon May 13 11:49:13 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.1.5.tar` & `common-tools-ai-bnq-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:16:10.110012 common-tools-ai-bnq-0.1.5/
--rw-rw-rw-   0        0        0     2511 2024-05-10 08:16:10.110012 common-tools-ai-bnq-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2024-05-10 08:15:54.000000 common-tools-ai-bnq-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 08:16:10.089810 common-tools-ai-bnq-0.1.5/bnq_py_core/
--rw-rw-rw-   0        0        0      356 2024-04-24 02:52:35.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/cos_connect.py
--rw-rw-rw-   0        0        0     4616 2024-05-10 08:10:48.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     1995 2024-05-10 08:10:10.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.5/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:16:10.109019 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0     2511 2024-05-10 08:16:09.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-05-10 08:16:10.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:16:09.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-05-10 08:16:09.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-10 08:16:09.000000 common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:16:10.111013 common-tools-ai-bnq-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-10 08:16:06.000000 common-tools-ai-bnq-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:49:13.476247 common-tools-ai-bnq-0.1.6/
+-rw-rw-rw-   0        0        0     2531 2024-05-13 11:49:13.475247 common-tools-ai-bnq-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2024-05-10 08:15:54.000000 common-tools-ai-bnq-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 11:49:13.441858 common-tools-ai-bnq-0.1.6/bnq_py_core/
+-rw-rw-rw-   0        0        0      356 2024-04-24 02:52:35.000000 common-tools-ai-bnq-0.1.6/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.1.6/bnq_py_core/cos_connect.py
+-rw-rw-rw-   0        0        0     5125 2024-05-13 11:28:10.000000 common-tools-ai-bnq-0.1.6/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.1.6/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     2076 2024-05-13 11:48:35.000000 common-tools-ai-bnq-0.1.6/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.6/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:49:13.474254 common-tools-ai-bnq-0.1.6/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0     2531 2024-05-13 11:49:13.000000 common-tools-ai-bnq-0.1.6/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2024-05-13 11:49:13.000000 common-tools-ai-bnq-0.1.6/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 11:49:13.000000 common-tools-ai-bnq-0.1.6/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-05-13 11:49:13.000000 common-tools-ai-bnq-0.1.6/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 11:49:13.000000 common-tools-ai-bnq-0.1.6/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 11:49:13.476247 common-tools-ai-bnq-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      856 2024-05-13 11:47:43.000000 common-tools-ai-bnq-0.1.6/setup.py
```

### Comparing `common-tools-ai-bnq-0.1.5/PKG-INFO` & `common-tools-ai-bnq-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.5
+Version: 0.1.6
 Summary: Common tools of AI module for BNQ
+Home-page: UNKNOWN
 Author: BNQ
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
     python setup.py sdist bdist_wheel
     twine upload dist/*
```

### Comparing `common-tools-ai-bnq-0.1.5/README.md` & `common-tools-ai-bnq-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.5/bnq_py_core/cos_connect.py` & `common-tools-ai-bnq-0.1.6/bnq_py_core/cos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.5/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.1.6/bnq_py_core/logger_record.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 # @File:logger_record.py
 
 import logging
 import logging.config
 import logging.handlers
 import os
 import pathlib
+import sys
 import time
 
 from structlog import configure, processors, stdlib
+from termcolor import colored
 
 
 class LoggingRecord(object):
     """日志记录类，用于记录运行中的信息
 
     """
     __instance = None  # 单例
@@ -54,45 +56,56 @@
         log_filename = os.path.join(self.log_record_path, self.__filename)
         logging.config.dictConfig({
             "version": 1,
             "disable_existing_loggers": False,
             "formatters": {
                 "default": {
                     "format": '%(asctime)s - %(levelname)s - %(name)s - %(message)s'
+                },
+                "console": {
+                    "format": colored(f'[%(asctime)s][%(levelname)1.1s][%(process)d][%(name)s]', 'green') + colored(
+                        f'(%(filename)s %(lineno)d)', 'yellow') + ': %(message)s'
                 }
             },
             "handlers": {
+                "console_handler": {
+                    "class": "logging.StreamHandler",
+                    "level": self.level,
+                    "formatter": "console",
+                    "stream": sys.stdout
+                },
                 "file_handler": {
                     "level": self.level,
                     "formatter": "default",
                     "class": "concurrent_log_handler.ConcurrentRotatingFileHandler",
                     "filename": log_filename,
                     "maxBytes": self.max_bytes,
                     "backupCount": self.backup_count,
                     "encoding": "UTF-8"
                 },
             },
             "loggers": {
                 "": {
-                    "handlers": ["file_handler"],
+                    "handlers": ["file_handler", "console_handler"],
                     "level": self.level
                 }
             }
         })
         configure(
             context_class=dict,
             logger_factory=stdlib.LoggerFactory(),
             wrapper_class=stdlib.BoundLogger,
             processors=[
                 stdlib.filter_by_level,
                 stdlib.PositionalArgumentsFormatter(),
                 processors.StackInfoRenderer(),
                 processors.format_exc_info,
                 processors.UnicodeDecoder(),
-                stdlib.render_to_log_kwargs]
+                stdlib.render_to_log_kwargs
+            ]
         )
         self.logger = logging.getLogger("BNQ-AI")
         self.logger.level = self.level
 
     def debug(self, record_info):
         """debug级别的日志记录
 
@@ -136,21 +149,19 @@
         self.logger.warning(warning_info)
 
     def exception(self, exception_info):
         self.logger.exception(exception_info)
 
 
 if __name__ == "__main__":
-    import os
 
-    og_record_path = os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "log")
+    # og_record_path = os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "log")
 
-    testLog = LoggingRecord(log_level=logging.DEBUG, log_dir=og_record_path)
+    testLog = LoggingRecord(log_level=logging.DEBUG)
     for i in range(10):
-        print(i, 'i')
         print(testLog, "testLog")
         testLog.debug(i)
         testLog.info("中文测试")
         testLog.error(i)
         testLog.warning(i)
         testLog.exception(i)
         # time.sleep(3)
```

### Comparing `common-tools-ai-bnq-0.1.5/bnq_py_core/nacos_connect.py` & `common-tools-ai-bnq-0.1.6/bnq_py_core/nacos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.5/bnq_py_core/read_conf_from_ini.py` & `common-tools-ai-bnq-0.1.6/bnq_py_core/read_conf_from_ini.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # @time:2024/3/27 17:44
 # Author:Zhang HongTao
 # @File:read_conf_from_ini.py
 
 
+import ast
 import configparser
 import os
-import ast
 
 
 class GetConfInfo:
     """获取配置文件中的信息
     """
     __instance = None
 
@@ -23,14 +23,15 @@
         """
         if not cls.__instance:
             cls.__instance = super(GetConfInfo, cls).__new__(cls, *args, **kwargs)
         return cls.__instance
 
     def __init__(self):
         self.conf = configparser.RawConfigParser()
+        path_file = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
         self.conf_path = os.path.join(os.getcwd(), "config", "conf.ini")
         self.conf.read(self.conf_path)
         log_env_path = os.path.join(path_file, 'logenv')
         self.field = self.get_field(log_env_path)
 
     @staticmethod
     def get_field(log_env_path):
```

### Comparing `common-tools-ai-bnq-0.1.5/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.1.6/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.5/common_tools_ai_bnq.egg-info/PKG-INFO` & `common-tools-ai-bnq-0.1.6/common_tools_ai_bnq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.1.5
+Version: 0.1.6
 Summary: Common tools of AI module for BNQ
+Home-page: UNKNOWN
 Author: BNQ
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
     python setup.py sdist bdist_wheel
     twine upload dist/*
```

### Comparing `common-tools-ai-bnq-0.1.5/setup.py` & `common-tools-ai-bnq-0.1.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.22',
         'nacos-sdk-python==0.1.12',
         'PyYAML==6.0.1',
         'cos-python-sdk-v5==1.9.28',
+        'termcolor==2.4.0'
     ],
     # 其他元数据，如作者、描述等
     author='BNQ',
     description='Common tools of AI module for BNQ',
     long_description=long_description,
     long_description_content_type="text/markdown",  # 指明内容类型为markdown
 )
```

