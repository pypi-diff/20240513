# Comparing `tmp/data_watchtower-0.0.4.tar.gz` & `tmp/data_watchtower-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_watchtower-0.0.4.tar", max compression
+gzip compressed data, was "data_watchtower-0.0.5.tar", max compression
```

## Comparing `data_watchtower-0.0.4.tar` & `data_watchtower-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      266 2024-05-13 01:50:29.799456 data_watchtower-0.0.4/data_watchtower/__init__.py
--rw-r--r--   0        0        0       48 2024-05-03 02:34:32.713935 data_watchtower-0.0.4/data_watchtower/api/__init__.py
--rw-r--r--   0        0        0       48 2024-05-03 03:21:05.216750 data_watchtower-0.0.4/data_watchtower/api/handlers/__init__.py
--rw-r--r--   0        0        0     2172 2024-05-12 13:13:02.383972 data_watchtower-0.0.4/data_watchtower/api/handlers/base.py
--rw-r--r--   0        0        0      691 2024-05-11 03:09:37.211029 data_watchtower-0.0.4/data_watchtower/api/handlers/data_loader.py
--rw-r--r--   0        0        0     1587 2024-05-12 13:37:42.277012 data_watchtower-0.0.4/data_watchtower/api/handlers/watchtower.py
--rw-r--r--   0        0        0      884 2024-05-11 09:19:04.404088 data_watchtower-0.0.4/data_watchtower/api/server.py
--rw-r--r--   0        0        0      388 2024-05-11 06:04:24.353601 data_watchtower-0.0.4/data_watchtower/api/url.py
--rw-r--r--   0        0        0       48 2024-04-26 07:27:27.399876 data_watchtower-0.0.4/data_watchtower/core/__init__.py
--rw-r--r--   0        0        0     4739 2024-05-12 01:33:43.657801 data_watchtower-0.0.4/data_watchtower/core/base.py
--rw-r--r--   0        0        0      976 2024-05-07 10:18:14.933640 data_watchtower-0.0.4/data_watchtower/core/data_loaders.py
--rw-r--r--   0        0        0     1556 2024-05-10 10:48:00.694726 data_watchtower-0.0.4/data_watchtower/core/macro.py
--rw-r--r--   0        0        0    10439 2024-04-28 03:18:50.489993 data_watchtower-0.0.4/data_watchtower/core/validators.py
--rw-r--r--   0        0        0     5982 2024-05-08 02:01:24.145907 data_watchtower-0.0.4/data_watchtower/core/watchtower.py
--rw-r--r--   0        0        0       48 2024-04-26 07:38:23.540515 data_watchtower-0.0.4/data_watchtower/model/__init__.py
--rw-r--r--   0        0        0     2595 2024-05-12 03:39:26.344155 data_watchtower-0.0.4/data_watchtower/model/models.py
--rw-r--r--   0        0        0     8716 2024-05-12 03:39:50.329215 data_watchtower-0.0.4/data_watchtower/model/services.py
--rw-r--r--   0        0        0     6630 2024-05-12 13:37:11.773450 data_watchtower-0.0.4/data_watchtower/utils.py
--rw-r--r--   0        0        0     1090 2024-05-01 02:10:55.882035 data_watchtower-0.0.4/LICENSE
--rw-r--r--   0        0        0     1164 2024-05-13 01:50:02.047916 data_watchtower-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2435 2024-05-03 13:56:51.909708 data_watchtower-0.0.4/README.md
--rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 data_watchtower-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      266 2024-05-13 14:25:00.117332 data_watchtower-0.0.5/data_watchtower/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-03 02:34:32.713935 data_watchtower-0.0.5/data_watchtower/api/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-03 03:21:05.216750 data_watchtower-0.0.5/data_watchtower/api/handlers/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-12 13:13:02.383972 data_watchtower-0.0.5/data_watchtower/api/handlers/base.py
+-rw-r--r--   0        0        0      693 2024-05-13 12:45:28.715213 data_watchtower-0.0.5/data_watchtower/api/handlers/data_loader.py
+-rw-r--r--   0        0        0     2741 2024-05-13 12:33:44.805863 data_watchtower-0.0.5/data_watchtower/api/handlers/watchtower.py
+-rw-r--r--   0        0        0      884 2024-05-11 09:19:04.404088 data_watchtower-0.0.5/data_watchtower/api/server.py
+-rw-r--r--   0        0        0      388 2024-05-11 06:04:24.353601 data_watchtower-0.0.5/data_watchtower/api/url.py
+-rw-r--r--   0        0        0       48 2024-04-26 07:27:27.399876 data_watchtower-0.0.5/data_watchtower/core/__init__.py
+-rw-r--r--   0        0        0     4739 2024-05-12 01:33:43.657801 data_watchtower-0.0.5/data_watchtower/core/base.py
+-rw-r--r--   0        0        0      976 2024-05-07 10:18:14.933640 data_watchtower-0.0.5/data_watchtower/core/data_loaders.py
+-rw-r--r--   0        0        0     1556 2024-05-10 10:48:00.694726 data_watchtower-0.0.5/data_watchtower/core/macro.py
+-rw-r--r--   0        0        0    10439 2024-04-28 03:18:50.489993 data_watchtower-0.0.5/data_watchtower/core/validators.py
+-rw-r--r--   0        0        0     6019 2024-05-13 12:21:15.499719 data_watchtower-0.0.5/data_watchtower/core/watchtower.py
+-rw-r--r--   0        0        0       48 2024-04-26 07:38:23.540515 data_watchtower-0.0.5/data_watchtower/model/__init__.py
+-rw-r--r--   0        0        0     2388 2024-05-13 12:08:17.428027 data_watchtower-0.0.5/data_watchtower/model/models.py
+-rw-r--r--   0        0        0     8693 2024-05-13 14:13:24.312996 data_watchtower-0.0.5/data_watchtower/model/services.py
+-rw-r--r--   0        0        0     6630 2024-05-12 13:37:11.773450 data_watchtower-0.0.5/data_watchtower/utils.py
+-rw-r--r--   0        0        0     1090 2024-05-01 02:10:55.882035 data_watchtower-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1345 2024-05-13 14:25:09.347785 data_watchtower-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2435 2024-05-03 13:56:51.909708 data_watchtower-0.0.5/README.md
+-rw-r--r--   0        0        0     3900 1970-01-01 00:00:00.000000 data_watchtower-0.0.5/PKG-INFO
```

### Comparing `data_watchtower-0.0.4/data_watchtower/api/handlers/base.py` & `data_watchtower-0.0.5/data_watchtower/api/handlers/base.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.4/data_watchtower/api/handlers/data_loader.py` & `data_watchtower-0.0.5/data_watchtower/api/handlers/data_loader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
         result = dict(
             records=data
         )
         self.json(result)
         return
 
     def post(self):
-        return self.get()
+        return self.get()
```

### Comparing `data_watchtower-0.0.4/data_watchtower/api/server.py` & `data_watchtower-0.0.5/data_watchtower/api/server.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.4/data_watchtower/core/base.py` & `data_watchtower-0.0.5/data_watchtower/core/base.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.4/data_watchtower/core/data_loaders.py` & `data_watchtower-0.0.5/data_watchtower/core/data_loaders.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.4/data_watchtower/core/macro.py` & `data_watchtower-0.0.5/data_watchtower/core/macro.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.4/data_watchtower/core/validators.py` & `data_watchtower-0.0.5/data_watchtower/core/validators.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.4/data_watchtower/core/watchtower.py` & `data_watchtower-0.0.5/data_watchtower/core/watchtower.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,71 +5,78 @@
 
 from data_watchtower.utils import (spawn_data_loader_from_dict, spawn_validator_from_dict,
                                    get_string_values, MacroTemplate, json_loads, json_dumps)
 from data_watchtower.core.macro import DEFAULT_MACRO_CONFIG
 
 
 class Watchtower(object):
-
-    def __init__(self, name, data_loader, **params):
+    def __init__(self, name, data_loader, custom_macro_map=None, **params):
         """
 
         :param name:
         :param data_loader:
-        :param params:
+        :param params: schedule, validator_success_method, success_method
         """
-        custom_macro_map = params.get('custom_macro_map')  # 只是运行的时候使用,不会保存
-        validator_success_method = params.get('validator_success_method', 'all')
-        success_method = params.get('success_method', None)
-        extra = params.get('extra', {})
+        custom_macro_map = custom_macro_map or {}  # 只是运行的时候使用,不会保存
         self.params = params
         self._data_loader = data_loader  # 原本的loader,参数可能包含宏
         self._data_loader_meta = data_loader.to_dict()  # 原本的loader,参数可能包含宏
         self._validators = []
         self._validators_meta = []
         self.name = name
         self.metrics = {}
-        custom_macro_map = custom_macro_map or {}
         self.macro_map = copy.deepcopy(DEFAULT_MACRO_CONFIG)
         self.macro_map.update(custom_macro_map)
         self.macro_template = MacroTemplate(self.macro_map)
-        self.extra = extra
-
-        self.validator_success_method = validator_success_method
+        # 回填默认值
+        self.params['schedule'] = self.schedule
+        self.params['validator_success_method'] = self.validator_success_method
+        self.params['success_method'] = self.success_method
+
+    @property
+    def schedule(self):
+        return self.params.get('schedule')
+
+    @property
+    def validator_success_method(self):
+        return self.params.get('validator_success_method', 'all')
+
+    @property
+    def success_method(self):
+        success_method = self.params.get('success_method')
         if success_method is None:
-            if len(self.macro_template.get_used_macro_maps([name])) > 0:
-                self.success_method = 'all'
+            if len(self.macro_template.get_used_macro_maps([self.name])) > 0:
+                return 'all'
             else:
-                self.success_method = 'last'
+                return 'last'
         else:
-            self.success_method = success_method
+            return success_method
 
     def set_custom_macro(self, **custom_macro_map):
         self.macro_map.update(custom_macro_map)
         self.macro_template.macro_config.update(custom_macro_map)
 
     @classmethod
     def from_dict(cls, data):
         data_loader = spawn_data_loader_from_dict(data.get('data_loader', {}))
-        validator_success_method = data.get('validator_success_method', 'all')
-        inst = cls(
-            name=data['name'], data_loader=data_loader,
-            validator_success_method=validator_success_method,
-        )
+        params = data.get('params', {})
+        inst = cls(name=data['name'], data_loader=data_loader, **params)
         for validator in data.get('validators', []):
             inst.add_validator(spawn_validator_from_dict(validator))
         return inst
 
     def to_dict(self):
+        params = {
+
+        }
         result = dict(
             name=self.name,
             data_loader=json_dumps(self.get_loader_meta()),
             validators=json_dumps(self.get_validator_meta()),
-            validator_success_method=self.validator_success_method,
-            success_method=self.success_method,
+            params=json_dumps(self.params),
         )
         return result
 
     def add_validator(self, validator):
         item = validator.to_dict()
         self._validators_meta.append(item)
 
@@ -143,15 +150,14 @@
             name=wt_name,
             success=success,
             run_time=run_time,
             macro_maps=macro_maps,
             metrics=self.metrics,
             validators_result=validators_result,
         )
-        result.update(self.extra)
         return result
 
     @classmethod
     def module_path(cls):
         return "%s:%s" % (cls.__module__, cls.__name__)
```

### Comparing `data_watchtower-0.0.4/data_watchtower/model/models.py` & `data_watchtower-0.0.5/data_watchtower/model/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,18 +40,15 @@
 
 
 class WatchtowerModel(BaseModel):
     name = CharField(max_length=128, primary_key=True)  # wt_name
     success = BooleanField(null=True)  # success
     run_time = DateTimeField(null=True)  # 最后一次运行的时间
     data_loader = TextField()
-    schedule = CharField(max_length=64, null=True)
-    # validators = TextField()
-    success_method = CharField(max_length=64)
-    validator_success_method = CharField(max_length=64, default='all', help_text='option: any, all')
+    params = TextField()
     update_time = DateTimeField(default=datetime.datetime.now)
     create_time = DateTimeField(default=datetime.datetime.now)
 
     class Meta:
         table_name = 'dw_watchtower'
 
     def to_dict(self, fields_from_query=None):
```

### Comparing `data_watchtower-0.0.4/data_watchtower/model/services.py` & `data_watchtower-0.0.5/data_watchtower/model/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
             for model in models:
                 if not self.database.table_exists(model):
                     self.database.create_tables([model])
 
     def get_watchtower(self, name):
         model = WatchtowerModel.get(WatchtowerModel.name == name).get()
         item = model.to_dict()
+        item['params'] = json_loads(item['params'])
         if item is not None:
             item['data_loader'] = json_loads(item['data_loader'])
-            # item['validators'] = json_loads(item['validators'])
         validators = ValidatorRelationModel.select().where(ValidatorRelationModel.wt_name == name)
         item['validators'] = []
         for validator_item in validators:
             validator = dict(
                 params=json_loads(validator_item.params),
                 __class__=validator_item.validator,
             )
@@ -54,22 +54,22 @@
         获取所有的watchtower
         :return:
         """
         result = []
         query = WatchtowerModel.select(
             WatchtowerModel.name,
             WatchtowerModel.success,
-            WatchtowerModel.schedule,
             WatchtowerModel.run_time,
             WatchtowerModel.data_loader,
-            WatchtowerModel.success_method,
-            WatchtowerModel.validator_success_method,
+            WatchtowerModel.params,
         )
         for item in query:
-            result.append(item.to_dict(fields_from_query=query))
+            row = item.to_dict(fields_from_query=query)
+            row['params'] = json_loads(row['params'])
+            result.append(row)
         return result
 
     def add_watchtower(self, watchtower):
         update_time = datetime.datetime.now()
         try:
             with self.database.atomic():
                 item = watchtower.to_dict()
@@ -86,33 +86,33 @@
                     )
                     validators.append(inst)
                 ValidatorRelationModel.bulk_create(validators, batch_size=100)
         except IntegrityError as e:
             logger.warning('add watchtower error!. msg:%s' % str(e))
             return
 
-    def update_watchtower(self, wt_name, **item):
+    def update_watchtower(self, name, **item):
         if len(item) == 0:
             return 0
         update_time = datetime.datetime.now()
         with self.database.atomic():
-            wt = WatchtowerModel.select().where(WatchtowerModel.name == wt_name).get()
+            wt = WatchtowerModel.select().where(WatchtowerModel.name == name).get()
             if wt:
-                if 'validators' in item:
-                    validators = []
-                    for validator_item in wt.get_validator_meta():
-                        inst = ValidatorRelationModel(
-                            wt_name=wt.name,
-                            validator=validator_item['__class__'],
-                            params=json_dumps(validator_item['params']),
-                        )
-                        validators.append(inst)
-                    ValidatorRelationModel.bulk_create(validators, batch_size=100)
+                # if 'validators' in item:
+                #     validators = []
+                #     for validator_item in wt.get_validator_meta():
+                #         inst = ValidatorRelationModel(
+                #             wt_name=wt.name,
+                #             validator=validator_item['__class__'],
+                #             params=json_dumps(validator_item['params']),
+                #         )
+                #         validators.append(inst)
+                #     ValidatorRelationModel.bulk_create(validators, batch_size=100)
                 if 'data_loader' in item:
-                    wt.validators = json_dumps(item.pop('data_loader'))
+                    wt.data_loader = json_dumps(item.pop('data_loader'))
                 for k, v in item.items():
                     setattr(wt, k, v)
                 wt.update_time = update_time
                 return wt.save()
             else:
                 return 0
```

### Comparing `data_watchtower-0.0.4/data_watchtower/utils.py` & `data_watchtower-0.0.5/data_watchtower/utils.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.4/LICENSE` & `data_watchtower-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.4/pyproject.toml` & `data_watchtower-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 package-mode = true
 name = "data-watchtower"
-version = "0.0.4"
+version = "0.0.5"
 description = "Data quality inspection tool. Identify issues before your CTO detects them!"
 authors = ["acracker <acracker@163.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/acracker/data_watchtower"
 
 
@@ -14,20 +14,27 @@
 attrs = "^23.2.0"
 peewee = "^3.17.3"
 shortuuid = "^1.0.13"
 tornado = [
     { version = "^6.2", python = "<3.8" },
     { version = "^6.4", python = ">=3.8" }
 ]
-pandas = "^1.3.0"
+pandas = [
+    { version = "^1.3.0", python = "<3.10" },
+    { version = "^2.1.0", python = ">=3.10" }
+]
+
 polars = [
     { version = "0.18.4", python = "<3.8" },
     { version = "^0.20.23", python = ">=3.8" }
 ]
-pyarrow = "^12.0.1"
+pyarrow = [
+    { version = "^12.0.1", python = "<3.8" },
+    { version = "^16.0.0", python = ">=3.8" }
+]
 connectorx = [
     { version = "0.3.1", python = "<3.8" },
     { version = "^0.3.2", python = ">=3.8" }
 ]
 apischema = "^0.18.1"
```

### Comparing `data_watchtower-0.0.4/README.md` & `data_watchtower-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.4/PKG-INFO` & `data_watchtower-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-watchtower
-Version: 0.0.4
+Version: 0.0.5
 Summary: Data quality inspection tool. Identify issues before your CTO detects them!
 Home-page: https://github.com/acracker/data_watchtower
 License: MIT
 Author: acracker
 Author-email: acracker@163.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,19 +14,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: apischema (>=0.18.1,<0.19.0)
 Requires-Dist: attrs (>=23.2.0,<24.0.0)
 Requires-Dist: connectorx (==0.3.1) ; python_version < "3.8"
 Requires-Dist: connectorx (>=0.3.2,<0.4.0) ; python_version >= "3.8"
-Requires-Dist: pandas (>=1.3.0,<2.0.0)
+Requires-Dist: pandas (>=1.3.0,<2.0.0) ; python_version < "3.10"
+Requires-Dist: pandas (>=2.1.0,<3.0.0) ; python_version >= "3.10"
 Requires-Dist: peewee (>=3.17.3,<4.0.0)
 Requires-Dist: polars (==0.18.4) ; python_version < "3.8"
 Requires-Dist: polars (>=0.20.23,<0.21.0) ; python_version >= "3.8"
-Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: pyarrow (>=12.0.1,<13.0.0) ; python_version < "3.8"
+Requires-Dist: pyarrow (>=16.0.0,<17.0.0) ; python_version >= "3.8"
 Requires-Dist: shortuuid (>=1.0.13,<2.0.0)
 Requires-Dist: tornado (>=6.2,<7.0) ; python_version < "3.8"
 Requires-Dist: tornado (>=6.4,<7.0) ; python_version >= "3.8"
 Project-URL: Repository, https://github.com/acracker/data_watchtower
 Description-Content-Type: text/markdown
 
 # data_watchtower
```

