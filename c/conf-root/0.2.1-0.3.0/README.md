# Comparing `tmp/conf_root-0.2.1.tar.gz` & `tmp/conf_root-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_root-0.2.1.tar", last modified: Mon Apr 29 07:50:18 2024, max compression
+gzip compressed data, was "conf_root-0.3.0.tar", last modified: Mon May 13 13:00:36 2024, max compression
```

## Comparing `conf_root-0.2.1.tar` & `conf_root-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:50:18.085878 conf_root-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 07:50:11.000000 conf_root-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-29 07:50:18.085878 conf_root-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-29 07:50:11.000000 conf_root-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:50:18.081878 conf_root-0.2.1/conf_root/
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-29 07:50:11.000000 conf_root-0.2.1/conf_root/ArgparseConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-29 07:50:11.000000 conf_root-0.2.1/conf_root/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:50:18.085878 conf_root-0.2.1/conf_root/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-29 07:50:11.000000 conf_root-0.2.1/conf_root/agents/BasicAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 07:50:11.000000 conf_root-0.2.1/conf_root/agents/JsonAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-29 07:50:11.000000 conf_root-0.2.1/conf_root/agents/YamlAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-29 07:50:11.000000 conf_root-0.2.1/conf_root/conf_root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:50:18.085878 conf_root-0.2.1/conf_root.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-29 07:50:18.000000 conf_root-0.2.1/conf_root.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-29 07:50:18.000000 conf_root-0.2.1/conf_root.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:50:18.000000 conf_root-0.2.1/conf_root.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 07:50:18.000000 conf_root-0.2.1/conf_root.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 07:50:18.000000 conf_root-0.2.1/conf_root.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:50:18.085878 conf_root-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-29 07:50:11.000000 conf_root-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:50:18.085878 conf_root-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-29 07:50:11.000000 conf_root-0.2.1/tests/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-29 07:50:11.000000 conf_root-0.2.1/tests/test_json_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-29 07:50:11.000000 conf_root-0.2.1/tests/test_nested_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-29 07:50:11.000000 conf_root-0.2.1/tests/test_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-29 07:50:11.000000 conf_root-0.2.1/tests/test_yaml_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.587498 conf_root-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 13:00:32.000000 conf_root-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-13 13:00:36.587498 conf_root-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-13 13:00:32.000000 conf_root-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.583497 conf_root-0.3.0/conf_root/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/ConfRoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.583497 conf_root-0.3.0/conf_root/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/agents/BasicAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/agents/JsonAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/agents/RuamelYamlAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-13 13:00:32.000000 conf_root-0.3.0/conf_root/agents/YamlAgent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.587498 conf_root-0.3.0/conf_root.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 13:00:36.000000 conf_root-0.3.0/conf_root.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:00:36.587498 conf_root-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-13 13:00:32.000000 conf_root-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:00:36.587498 conf_root-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_json_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_nested_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_ruamel_yaml_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-13 13:00:32.000000 conf_root-0.3.0/tests/test_yaml_agent.py
```

### Comparing `conf_root-0.2.1/LICENSE` & `conf_root-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conf_root-0.2.1/conf_root/agents/JsonAgent.py` & `conf_root-0.3.0/conf_root/agents/JsonAgent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,39 @@
+import os
+
+from conf_root.Configuration import Configuration
 from conf_root.agents.BasicAgent import BasicAgent
 import json
 
 
 class JsonAgent(BasicAgent):
     default_extension = 'json'
 
-    def create(self, cls):
-        # 将dataclass默认值转换为dict，便于序列化
-        default_dict = self.dataclass_default_dict(cls)
+    def exist(self, configuration: Configuration) -> bool:
+        return self.get_configuration_location(configuration).exists()
+
+    def create(self, configuration: Configuration):
+        super().create(configuration)
+        location = self.get_configuration_location(configuration)
+        # 将默认值转换为dict，便于序列化
+        default_dict = configuration.defaults
 
         # 将dict转换为YAML并写入文件
         if len(default_dict.keys()) > 0:
-            with open(self.location, "w") as file:
+            with open(location, "w") as file:
                 json.dump(default_dict, file)
 
-    def load(self, cls, obj):
-        with open(self.location, encoding='utf-8') as file:
+    def load(self, configuration):
+        super().load(configuration)
+        location = self.get_configuration_location(configuration)
+        with open(location, encoding='utf-8') as file:
             data = json.load(file)
-
         # 将dict展开为对象。
-        self.dict_to_dataclass(data, cls, obj)
-
-    def save(self, obj):
-        data_dict = self.dataclass_to_dict(obj)
+        return data
 
+    def save(self, configuration, obj):
+        super().save(configuration, obj)
+        location = self.get_configuration_location(configuration)
+        data_dict = configuration.obj2data(obj)
         # 将dict转换为YAML并写入文件
-        with open(self.location, "w") as file:
+        with open(location, "w") as file:
             json.dump(data_dict, file)
```

### Comparing `conf_root-0.2.1/setup.py` & `conf_root-0.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="conf_root",  # 包名
-    version="0.2.1",  # 版本号
+    version="0.3.0",  # 版本号
     install_requires=[
-        "PyYAML"
+        "ruamel.yaml"
     ],
     author="ciaranchen",
     author_email="ciaranchen@qq.com",
     description="基于dataclass的符合逻辑的配置取用方式。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ciaranchen/conf_root",
```

### Comparing `conf_root-0.2.1/tests/test_argparse.py` & `conf_root-0.3.0/tests/test_argparse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import argparse
 import os
 import unittest
 import yaml
-from conf_root import configuration, ArgparseConfiguration
+from conf_root import ConfRoot
 
 
 class TestArgparse(unittest.TestCase):
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
-        self.location = 'argsparse.yaml'
+        self.location = 'argparse.yml'
 
     def tearDown(self):
         # 这个方法将在每个测试方法结束后运行
         # 使用os.remove删除在测试中创建的文件
         try:
             os.remove(self.location)
         except FileNotFoundError:
             pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
 
     def test_with_default_value(self):
         parser = argparse.ArgumentParser(description="Test with default value")
         parser.add_argument("--arg1", default=10, type=int, help="Number 1")
         parser.add_argument("--arg2", default=20, type=int, help="Number 2")
-        ac = ArgparseConfiguration.from_argparse(parser)
-        ArgsClass = configuration(self.location)(ac.dataclass)
+        ArgsClass = ConfRoot().from_argparse(parser, self.location)
 
         args_namespace = parser.parse_args(['--arg2', '30'])
         args_dataclass = ArgsClass(**vars(args_namespace))
 
         self.assertEqual(args_dataclass.arg1, 10)
         self.assertEqual(args_dataclass.arg2, 30)
 
@@ -39,20 +38,19 @@
         self.assertEqual(data['arg2'], 20)
 
     def test_without_default_value(self):
         parser = argparse.ArgumentParser(description="Test without default value")
         parser.add_argument("--default_value", default=40, type=int)
         parser.add_argument("--arg1", type=int)
         parser.add_argument("--arg2", type=int)
+        ArgsClass = ConfRoot().from_argparse(parser)
 
-        ac = ArgparseConfiguration.from_argparse(parser)
-        ArgsClass = configuration(self.location)(ac.dataclass)
         args_namespace = parser.parse_args(['--arg2', '30'])
-
         args_dataclass = ArgsClass(**vars(args_namespace))
+
         self.assertIsNone(args_dataclass.arg1)
         self.assertEqual(args_dataclass.arg2, 30)
         self.assertEqual(args_dataclass.default_value, 40)
 
         # 注意，因为dataclass中non-default的定义需在default的变量前，所以在ArgsClass的定义中会对他们进行排序。
         args_dataclass2 = ArgsClass(12, 13)
         self.assertEqual(args_dataclass2.default_value, 40)
@@ -69,17 +67,15 @@
 
     def test_action(self):
         parser = argparse.ArgumentParser(description="Test action")
         parser.add_argument("--verbose", action="store_true", help="Enable verbose mode")
         parser.add_argument('--foo', action='store_const', const=42)
         parser.add_argument("--items", nargs='+', type=str, help="List of items")
         parser.add_argument('--count', '-c', action='count', default=0)
-
-        ac = ArgparseConfiguration.from_argparse(parser)
-        ArgsClass = configuration(self.location)(ac.dataclass)
+        ArgsClass = ConfRoot().from_argparse(parser)
         args_dataclass = ArgsClass()
 
         self.assertFalse(hasattr(args_dataclass, 'items'))
         self.assertFalse(hasattr(args_dataclass, 'help'))
         self.assertFalse(hasattr(args_dataclass, 'count'))
         self.assertTrue(args_dataclass.verbose)
         self.assertEqual(args_dataclass.foo, 42)
```

### Comparing `conf_root-0.2.1/tests/test_json_agent.py` & `conf_root-0.3.0/tests/test_nested_dataclass.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,85 @@
 import os
 import unittest
-from dataclasses import dataclass
+from dataclasses import dataclass, field as dataclass_field
 
-from conf_root import configuration, JsonAgent
+from conf_root import ConfRoot
+
+
+@ConfRoot(agent=None).wrap()
+@dataclass
+class NestedConfig:
+    config1: str = 'nest_config1'
+    config2: str = 'nest_config2'
 
 
 @dataclass
 class AppConfig:
-    not_default: str
-    database_host: str = 'localhost'
-    database_port: int = 5432
+    nc_defined: NestedConfig
+    nc_default: NestedConfig = dataclass_field(default_factory=NestedConfig)
 
 
 class TestConfig(unittest.TestCase):
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
-        self.location = 'settings.json'
+        self.location = 'nested_config.yml'
 
     def tearDown(self):
         # 这个方法将在每个测试方法结束后运行
         # 使用os.remove删除在测试中创建的文件
         try:
             os.remove(self.location)
         except FileNotFoundError:
             pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
 
     def test_create(self):
-        DecoratedConfig = configuration(self.location, agent=JsonAgent)(AppConfig)
-        app_config = DecoratedConfig('admin')
-        self.assertEqual(app_config.database_host, 'localhost')
-        self.assertEqual(app_config.database_port, 5432)
-        self.assertEqual(app_config.not_default, 'admin')
-
+        DecoratedConfig = ConfRoot().wrap(self.location)(AppConfig)
+        app_config = DecoratedConfig(NestedConfig(config1='defined1', config2='defined2'))
+        self.assertEqual(app_config.nc_default.config1, 'nest_config1')
+        self.assertEqual(app_config.nc_default.config2, 'nest_config2')
+
+        self.assertEqual(app_config.nc_defined.config1, 'defined1')
+        self.assertEqual(app_config.nc_defined.config2, 'defined2')
+        # print(app_config.__CONF_ROOT__.defaults)
         # 外部修改配置文件后读取，结果应为配置文件内的设置。
         # 打开文件，读取内容
         self.assertTrue(os.path.exists(self.location))
         with open(self.location, 'r') as file:
             content = file.read()
-        self.assertTrue('localhost' in content)
-        self.assertTrue('5432' in content)
-        # admin 因为非默认配置，不在配置文件中。
-        self.assertFalse('admin' in content)
+        self.assertTrue('nest_config1' in content)
+        self.assertTrue('nest_config2' in content)
+        # defined 因为非默认配置，不在配置文件中。
+        self.assertFalse('defined1' in content)
+        self.assertFalse('defined2' in content)
 
     def test_load(self):
-        content = """{"database_host": "127.0.0.1", "database_port": 5432}"""
+        content = """nc_default:
+    config1: default_load1
+nc_defined:
+    config1: load1
+    config2: load2"""
+
         # 将处理后的内容写回文件（可以先备份原文件）
         with open(self.location, 'w') as file:
             file.write(content)
 
-        DecoratedConfig = configuration(self.location, agent=JsonAgent)(AppConfig)
-        app_config = DecoratedConfig('admin')
-        self.assertEqual(app_config.database_host, '127.0.0.1')
-        self.assertEqual(app_config.database_port, 5432)
+        DecoratedConfig = ConfRoot().wrap(self.location)(AppConfig)
+        app_config = DecoratedConfig(NestedConfig(config1='defined1', config2='defined2'))
+        self.assertEqual(app_config.nc_default.config1, 'default_load1')
+        self.assertEqual(app_config.nc_default.config2, 'nest_config2')
+
+        self.assertEqual(app_config.nc_defined.config1, 'load1')
+        self.assertEqual(app_config.nc_defined.config2, 'load2')
 
     def test_save(self):
-        DecoratedConfig = configuration(self.location, agent=JsonAgent)(AppConfig)
-        app_config = DecoratedConfig('admin')
-        app_config.database_host = '192.168.1.1'
-        app_config.database_port = 3309
+        DecoratedConfig = ConfRoot().wrap(self.location)(AppConfig)
+        app_config = DecoratedConfig(NestedConfig(config1='defined1', config2='defined2'))
+        app_config.nc_default.config1 = 'save_default'
+        app_config.nc_defined.config1 = 'save_defined'
         app_config.save()
 
         # 外部修改配置文件后读取，结果应为配置文件内的设置。
         # 打开文件，读取内容
-        self.assertTrue(os.path.exists(self.location))
         with open(self.location, 'r') as file:
             content = file.read()
-        self.assertTrue('192.168.1.1' in content)
-        self.assertTrue('3309' in content)
-        self.assertTrue('admin' in content)
+        self.assertTrue('save_default' in content)
+        self.assertTrue('save_defined' in content)
```

### Comparing `conf_root-0.2.1/tests/test_normal.py` & `conf_root-0.3.0/tests/test_normal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 import os.path
 import unittest
 from dataclasses import dataclass
 
-from conf_root import configuration
+from conf_root import ConfRoot
 from conf_root.agents.JsonAgent import JsonAgent
 
 
-class MyTestCase(unittest.TestCase):
+class TestWrap(unittest.TestCase):
 
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
-        self.default_yaml_location = 'config.yml'
-        self.default_json_location = 'config.json'
+        self.yaml_location = 'config.yml'
+        self.json_location = 'config.json'
 
     def tearDown(self):
         # 使用os.remove删除在测试中创建的文件
         try:
-            os.remove(self.default_yaml_location)
+            os.remove(self.yaml_location)
         except FileNotFoundError:
             pass
 
         try:
-            os.remove(self.default_json_location)
+            os.remove(self.json_location)
         except FileNotFoundError:
             pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
 
+    def replace_text(self, filename, origin_text, replace_text):
+        with open(filename, 'r') as file:
+            content = file.read()
+        content = content.replace(origin_text, replace_text)
+        with open(filename, 'w') as file:
+            file.write(content)
+
     def test_default_yaml_configuration(self):
         # 测试直接使用configuration而不带参数的情况。
-        @configuration
+        @ConfRoot().wrap('config')
         @dataclass
         class AppConfig:
             something: int = 42
 
         app_config = AppConfig()
-        self.assertTrue(os.path.exists(self.default_yaml_location))
-        with open(self.default_yaml_location, 'r') as file:
+        self.assertTrue(os.path.exists(self.yaml_location))
+        with open(self.yaml_location, 'r') as file:
             content = file.read()
         self.assertTrue('42' in content)
+        self.replace_text(self.yaml_location, '42', '43')
+        app_config2 = AppConfig()
+        self.assertEqual(app_config2.something, 43)
 
     def test_default_json_configuration(self):
-        @configuration(agent=JsonAgent)
+        @ConfRoot(agent=JsonAgent).wrap('config')
         @dataclass
         class AppConfig:
             something: int = 42
 
         app_config = AppConfig()
-        self.assertTrue(os.path.exists(self.default_json_location))
-        with open(self.default_json_location, 'r') as file:
+        self.assertTrue(os.path.exists(self.json_location))
+        with open(self.json_location, 'r') as file:
             content = file.read()
         self.assertTrue('42' in content)
+        self.replace_text(self.json_location, '42', '43')
+        app_config2 = AppConfig()
+        self.assertEqual(app_config2.something, 43)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `conf_root-0.2.1/tests/test_yaml_agent.py` & `conf_root-0.3.0/tests/test_json_agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import os
 import unittest
 from dataclasses import dataclass
 
-from conf_root import configuration
+from conf_root import ConfRoot, JsonAgent
 
 
-@dataclass
-class AppConfig:
-    not_default: str
-    database_host: str = 'localhost'
-    database_port: int = 5432
-
-
-class TestConfig(unittest.TestCase):
+class TestJsonConfig(unittest.TestCase):
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
-        self.location = 'settings.yaml'
+        self.location = 'settings.json'
 
     def tearDown(self):
         # 这个方法将在每个测试方法结束后运行
         # 使用os.remove删除在测试中创建的文件
         try:
             os.remove(self.location)
         except FileNotFoundError:
             pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
 
     def test_create(self):
-        DecoratedConfig = configuration(self.location)(AppConfig)
-        app_config = DecoratedConfig('admin')
+        @ConfRoot(agent=JsonAgent).wrap(self.location)
+        @dataclass
+        class AppConfig:
+            not_default: str
+            database_host: str = 'localhost'
+            database_port: int = 5432
+
+        app_config = AppConfig('admin')
         self.assertEqual(app_config.database_host, 'localhost')
         self.assertEqual(app_config.database_port, 5432)
         self.assertEqual(app_config.not_default, 'admin')
 
         # 外部修改配置文件后读取，结果应为配置文件内的设置。
         # 打开文件，读取内容
         self.assertTrue(os.path.exists(self.location))
@@ -39,29 +38,39 @@
             content = file.read()
         self.assertTrue('localhost' in content)
         self.assertTrue('5432' in content)
         # admin 因为非默认配置，不在配置文件中。
         self.assertFalse('admin' in content)
 
     def test_load(self):
-        content = """database_host: 127.0.0.1
-database_port: 5432
-"""
+        @ConfRoot(agent=JsonAgent).wrap(self.location)
+        @dataclass
+        class AppConfig:
+            not_default: str
+            database_host: str = 'localhost'
+            database_port: int = 5432
+
+        content = """{"database_host": "127.0.0.1", "database_port": 5432}"""
         # 将处理后的内容写回文件（可以先备份原文件）
         with open(self.location, 'w') as file:
             file.write(content)
 
-        DecoratedConfig = configuration(self.location)(AppConfig)
-        app_config = DecoratedConfig('admin')
+        app_config = AppConfig('admin')
         self.assertEqual(app_config.database_host, '127.0.0.1')
         self.assertEqual(app_config.database_port, 5432)
 
     def test_save(self):
-        DecoratedConfig = configuration(self.location)(AppConfig)
-        app_config = DecoratedConfig('admin')
+        @ConfRoot(agent=JsonAgent).wrap(self.location)
+        @dataclass
+        class AppConfig:
+            not_default: str
+            database_host: str = 'localhost'
+            database_port: int = 5432
+
+        app_config = AppConfig('admin')
         app_config.database_host = '192.168.1.1'
         app_config.database_port = 3309
         app_config.save()
 
         # 外部修改配置文件后读取，结果应为配置文件内的设置。
         # 打开文件，读取内容
         self.assertTrue(os.path.exists(self.location))
```

