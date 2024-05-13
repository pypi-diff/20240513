# Comparing `tmp/middleware-help-python-0.1.2.tar.gz` & `tmp/middleware-help-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-help-python-0.1.2.tar", last modified: Sat May 11 01:01:08 2024, max compression
+gzip compressed data, was "middleware-help-python-0.1.3.tar", last modified: Mon May 13 08:11:31 2024, max compression
```

## Comparing `middleware-help-python-0.1.2.tar` & `middleware-help-python-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 01:01:08.765142 middleware-help-python-0.1.2/
--rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      543 2024-05-11 01:01:08.763158 middleware-help-python-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 01:01:08.762176 middleware-help-python-0.1.2/middleware_help_python.egg-info/
--rw-rw-rw-   0        0        0      543 2024-05-11 01:01:08.000000 middleware-help-python-0.1.2/middleware_help_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-05-11 01:01:08.000000 middleware-help-python-0.1.2/middleware_help_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 01:01:08.000000 middleware-help-python-0.1.2/middleware_help_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-11 01:01:08.000000 middleware-help-python-0.1.2/middleware_help_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-11 01:01:08.000000 middleware-help-python-0.1.2/middleware_help_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-11 01:01:08.760153 middleware-help-python-0.1.2/middleware_helper/
--rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.1.2/middleware_helper/__init__.py
--rw-rw-rw-   0        0        0      530 2024-05-10 10:22:25.000000 middleware-help-python-0.1.2/middleware_helper/libs.py
--rw-rw-rw-   0        0        0     5144 2024-05-11 01:00:25.000000 middleware-help-python-0.1.2/middleware_helper/mysql.py
--rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.1.2/middleware_helper/network.py
--rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.1.2/middleware_helper/redis.py
--rw-rw-rw-   0        0        0       42 2024-05-11 01:01:08.765142 middleware-help-python-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-05-11 01:01:05.000000 middleware-help-python-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:11:31.867924 middleware-help-python-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      543 2024-05-13 08:11:31.865925 middleware-help-python-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 08:11:31.863932 middleware-help-python-0.1.3/middleware_help_python.egg-info/
+-rw-rw-rw-   0        0        0      543 2024-05-13 08:11:31.000000 middleware-help-python-0.1.3/middleware_help_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-13 08:11:31.000000 middleware-help-python-0.1.3/middleware_help_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:11:31.000000 middleware-help-python-0.1.3/middleware_help_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-13 08:11:31.000000 middleware-help-python-0.1.3/middleware_help_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-13 08:11:31.000000 middleware-help-python-0.1.3/middleware_help_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:11:31.861938 middleware-help-python-0.1.3/middleware_helper/
+-rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.1.3/middleware_helper/__init__.py
+-rw-rw-rw-   0        0        0      530 2024-05-10 10:22:25.000000 middleware-help-python-0.1.3/middleware_helper/libs.py
+-rw-rw-rw-   0        0        0     5194 2024-05-13 08:10:57.000000 middleware-help-python-0.1.3/middleware_helper/mysql.py
+-rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.1.3/middleware_helper/network.py
+-rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.1.3/middleware_helper/redis.py
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:11:31.867924 middleware-help-python-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2024-05-13 08:11:16.000000 middleware-help-python-0.1.3/setup.py
```

### Comparing `middleware-help-python-0.1.2/LICENSE` & `middleware-help-python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.1.2/PKG-INFO` & `middleware-help-python-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.1.2/middleware_help_python.egg-info/PKG-INFO` & `middleware-help-python-0.1.3/middleware_help_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.1.2/middleware_helper/libs.py` & `middleware-help-python-0.1.3/middleware_helper/libs.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.1.2/middleware_helper/mysql.py` & `middleware-help-python-0.1.3/middleware_helper/mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,11 +123,11 @@
             else:
                 value = str(value)
             value_list.append(value)
         field_str = "(" + ", ".join(field_list) + ")"
         value_str = "(" + ", ".join(value_list) + ")"
         return field_str, value_str
 
-    def insert_order_sql(self, data_info: dict, table_name: str) -> list:
+    def insert_order_sql(self, data_info: dict, table_name: str, is_need_close: bool) -> list:
         field_str, value_str = self.convert_key_value_str(**data_info)
         sql = "insert into " + "`{}` {} values {};".format(table_name, field_str, value_str)
-        return self.execute_sql(sql=sql, action="insert")
+        return self.execute_sql(sql=sql, action="insert", is_need_close=is_need_close)
```

### Comparing `middleware-help-python-0.1.2/middleware_helper/network.py` & `middleware-help-python-0.1.3/middleware_helper/network.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.1.2/middleware_helper/redis.py` & `middleware-help-python-0.1.3/middleware_helper/redis.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.1.2/setup.py` & `middleware-help-python-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='middleware-help-python',
-    version='0.1.2',
+    version='0.1.3',
     description='This is my middleware help package',
     long_description='This is my middleware help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/middleware-help-python',
     packages=find_packages(),
     install_requires=[
```

