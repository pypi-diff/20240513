# Comparing `tmp/data_watchtower-0.0.3.tar.gz` & `tmp/data_watchtower-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_watchtower-0.0.3.tar", last modified: Mon May  6 08:22:17 2024, max compression
+gzip compressed data, was "data_watchtower-0.0.4.tar", max compression
```

## Comparing `data_watchtower-0.0.3.tar` & `data_watchtower-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.255872 data_watchtower-0.0.3/
--rw-rw-rw-   0        0        0     1090 2024-05-01 02:10:55.000000 data_watchtower-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      504 2024-05-06 08:22:17.254844 data_watchtower-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2435 2024-05-03 13:56:51.000000 data_watchtower-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.232454 data_watchtower-0.0.3/data_watchtower/
--rw-rw-rw-   0        0        0      270 2024-05-05 08:41:55.000000 data_watchtower-0.0.3/data_watchtower/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.240245 data_watchtower-0.0.3/data_watchtower/api/
--rw-rw-rw-   0        0        0       48 2024-05-03 02:34:32.000000 data_watchtower-0.0.3/data_watchtower/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.243364 data_watchtower-0.0.3/data_watchtower/api/handlers/
--rw-rw-rw-   0        0        0       48 2024-05-03 03:21:05.000000 data_watchtower-0.0.3/data_watchtower/api/handlers/__init__.py
--rw-rw-rw-   0        0        0      845 2024-05-05 04:43:17.000000 data_watchtower-0.0.3/data_watchtower/api/handlers/base.py
--rw-rw-rw-   0        0        0      553 2024-05-03 12:39:06.000000 data_watchtower-0.0.3/data_watchtower/api/handlers/watchtower.py
--rw-rw-rw-   0        0        0      835 2024-05-05 04:40:00.000000 data_watchtower-0.0.3/data_watchtower/api/server.py
--rw-rw-rw-   0        0        0      291 2024-05-05 06:57:58.000000 data_watchtower-0.0.3/data_watchtower/api/url.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.248064 data_watchtower-0.0.3/data_watchtower/core/
--rw-rw-rw-   0        0        0       48 2024-04-26 07:27:27.000000 data_watchtower-0.0.3/data_watchtower/core/__init__.py
--rw-rw-rw-   0        0        0     2809 2024-05-05 04:36:42.000000 data_watchtower-0.0.3/data_watchtower/core/base.py
--rw-rw-rw-   0        0        0     1138 2024-05-03 09:14:39.000000 data_watchtower-0.0.3/data_watchtower/core/data_loaders.py
--rw-rw-rw-   0        0        0     1546 2024-05-03 04:45:13.000000 data_watchtower-0.0.3/data_watchtower/core/macro.py
--rw-rw-rw-   0        0        0    10439 2024-04-28 03:18:50.000000 data_watchtower-0.0.3/data_watchtower/core/validators.py
--rw-rw-rw-   0        0        0     5861 2024-05-03 12:39:06.000000 data_watchtower-0.0.3/data_watchtower/core/watchtower.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.251181 data_watchtower-0.0.3/data_watchtower/model/
--rw-rw-rw-   0        0        0       48 2024-04-26 07:38:23.000000 data_watchtower-0.0.3/data_watchtower/model/__init__.py
--rw-rw-rw-   0        0        0     2528 2024-05-03 15:15:42.000000 data_watchtower-0.0.3/data_watchtower/model/models.py
--rw-rw-rw-   0        0        0     8448 2024-05-03 15:15:42.000000 data_watchtower-0.0.3/data_watchtower/model/services.py
--rw-rw-rw-   0        0        0     5473 2024-05-03 12:33:46.000000 data_watchtower-0.0.3/data_watchtower/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.253258 data_watchtower-0.0.3/data_watchtower.egg-info/
--rw-rw-rw-   0        0        0      504 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      806 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 08:22:17.255872 data_watchtower-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      795 2024-05-06 08:21:51.000000 data_watchtower-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.252218 data_watchtower-0.0.3/tests/
--rw-rw-rw-   0        0        0     7055 2024-05-05 04:20:24.000000 data_watchtower-0.0.3/tests/test_validator.py
+-rw-r--r--   0        0        0      266 2024-05-13 01:50:29.799456 data_watchtower-0.0.4/data_watchtower/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-03 02:34:32.713935 data_watchtower-0.0.4/data_watchtower/api/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-03 03:21:05.216750 data_watchtower-0.0.4/data_watchtower/api/handlers/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-12 13:13:02.383972 data_watchtower-0.0.4/data_watchtower/api/handlers/base.py
+-rw-r--r--   0        0        0      691 2024-05-11 03:09:37.211029 data_watchtower-0.0.4/data_watchtower/api/handlers/data_loader.py
+-rw-r--r--   0        0        0     1587 2024-05-12 13:37:42.277012 data_watchtower-0.0.4/data_watchtower/api/handlers/watchtower.py
+-rw-r--r--   0        0        0      884 2024-05-11 09:19:04.404088 data_watchtower-0.0.4/data_watchtower/api/server.py
+-rw-r--r--   0        0        0      388 2024-05-11 06:04:24.353601 data_watchtower-0.0.4/data_watchtower/api/url.py
+-rw-r--r--   0        0        0       48 2024-04-26 07:27:27.399876 data_watchtower-0.0.4/data_watchtower/core/__init__.py
+-rw-r--r--   0        0        0     4739 2024-05-12 01:33:43.657801 data_watchtower-0.0.4/data_watchtower/core/base.py
+-rw-r--r--   0        0        0      976 2024-05-07 10:18:14.933640 data_watchtower-0.0.4/data_watchtower/core/data_loaders.py
+-rw-r--r--   0        0        0     1556 2024-05-10 10:48:00.694726 data_watchtower-0.0.4/data_watchtower/core/macro.py
+-rw-r--r--   0        0        0    10439 2024-04-28 03:18:50.489993 data_watchtower-0.0.4/data_watchtower/core/validators.py
+-rw-r--r--   0        0        0     5982 2024-05-08 02:01:24.145907 data_watchtower-0.0.4/data_watchtower/core/watchtower.py
+-rw-r--r--   0        0        0       48 2024-04-26 07:38:23.540515 data_watchtower-0.0.4/data_watchtower/model/__init__.py
+-rw-r--r--   0        0        0     2595 2024-05-12 03:39:26.344155 data_watchtower-0.0.4/data_watchtower/model/models.py
+-rw-r--r--   0        0        0     8716 2024-05-12 03:39:50.329215 data_watchtower-0.0.4/data_watchtower/model/services.py
+-rw-r--r--   0        0        0     6630 2024-05-12 13:37:11.773450 data_watchtower-0.0.4/data_watchtower/utils.py
+-rw-r--r--   0        0        0     1090 2024-05-01 02:10:55.882035 data_watchtower-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1164 2024-05-13 01:50:02.047916 data_watchtower-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2435 2024-05-03 13:56:51.909708 data_watchtower-0.0.4/README.md
+-rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 data_watchtower-0.0.4/PKG-INFO
```

### Comparing `data_watchtower-0.0.3/LICENSE` & `data_watchtower-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.3/README.md` & `data_watchtower-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.3/data_watchtower/api/server.py` & `data_watchtower-0.0.4/data_watchtower/api/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 define("db_url", default=default_db_url, help="db url")
 
 
 def make_app():
     database = DbServices(options.db_url)
     app = tornado.web.Application(
         URLS,
-        database=database
+        database=database,
+        debug=True,
+        autoreload=False,
     )
     return app
 
 
 async def main():
     options.parse_command_line()
     app = make_app()
```

### Comparing `data_watchtower-0.0.3/data_watchtower/core/macro.py` & `data_watchtower-0.0.4/data_watchtower/core/macro.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,12 +32,12 @@
     'yesterday:2': {
         'impl': lambda: (datetime.datetime.now() - datetime.timedelta(days=1)).strftime("%Y%m%d"),
         'description': "昨天的日期.格式:yyyy-mm-dd",
     },
 
 }
 try:
-    custom_macro = load_object('macros:DEFAULT_MACRO_CONFIG')
+    custom_macro = load_object('dw_custom.macros:DEFAULT_MACRO_CONFIG')
     DEFAULT_MACRO_CONFIG.update(custom_macro)
     logger.info('custom macros loaded. count:%s' % len(custom_macro))
 except (ModuleNotFoundError, NameError):
     pass
```

### Comparing `data_watchtower-0.0.3/data_watchtower/core/validators.py` & `data_watchtower-0.0.4/data_watchtower/core/validators.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.3/data_watchtower/core/watchtower.py` & `data_watchtower-0.0.4/data_watchtower/core/watchtower.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,29 +25,32 @@
         self._data_loader = data_loader  # 原本的loader,参数可能包含宏
         self._data_loader_meta = data_loader.to_dict()  # 原本的loader,参数可能包含宏
         self._validators = []
         self._validators_meta = []
         self.name = name
         self.metrics = {}
         custom_macro_map = custom_macro_map or {}
-        self.custom_macro_map = custom_macro_map
         self.macro_map = copy.deepcopy(DEFAULT_MACRO_CONFIG)
         self.macro_map.update(custom_macro_map)
         self.macro_template = MacroTemplate(self.macro_map)
         self.extra = extra
 
         self.validator_success_method = validator_success_method
         if success_method is None:
             if len(self.macro_template.get_used_macro_maps([name])) > 0:
                 self.success_method = 'all'
             else:
                 self.success_method = 'last'
         else:
             self.success_method = success_method
 
+    def set_custom_macro(self, **custom_macro_map):
+        self.macro_map.update(custom_macro_map)
+        self.macro_template.macro_config.update(custom_macro_map)
+
     @classmethod
     def from_dict(cls, data):
         data_loader = spawn_data_loader_from_dict(data.get('data_loader', {}))
         validator_success_method = data.get('validator_success_method', 'all')
         inst = cls(
             name=data['name'], data_loader=data_loader,
             validator_success_method=validator_success_method,
```

### Comparing `data_watchtower-0.0.3/data_watchtower/model/models.py` & `data_watchtower-0.0.4/data_watchtower/model/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def to_dict(self, fields_from_query=None):
         return model_to_dict(self, fields_from_query=fields_from_query)
 
     class Meta:
         database = database_proxy
 
 
-class ValidationDetail(BaseModel):
+class ValidationDetailModel(BaseModel):
     id = AutoField(primary_key=True)
     wt_name = CharField(max_length=128, index=True)
     name = CharField(max_length=128)
     success = BooleanField()
     run_time = DateTimeField()
     metrics = TextField()
     params = TextField(null=True)
@@ -35,19 +35,20 @@
     update_time = DateTimeField(default=datetime.datetime.now)
     create_time = DateTimeField(default=datetime.datetime.now)
 
     class Meta:
         table_name = 'dw_validation_detail'
 
 
-class Watchtower(BaseModel):
+class WatchtowerModel(BaseModel):
     name = CharField(max_length=128, primary_key=True)  # wt_name
     success = BooleanField(null=True)  # success
     run_time = DateTimeField(null=True)  # 最后一次运行的时间
     data_loader = TextField()
+    schedule = CharField(max_length=64, null=True)
     # validators = TextField()
     success_method = CharField(max_length=64)
     validator_success_method = CharField(max_length=64, default='all', help_text='option: any, all')
     update_time = DateTimeField(default=datetime.datetime.now)
     create_time = DateTimeField(default=datetime.datetime.now)
 
     class Meta:
@@ -58,15 +59,15 @@
         if 'data_loader' in result:
             result['data_loader'] = json_loads(result['data_loader'])
         if 'validators' in result:
             result['validators'] = json_loads(result['validators'])
         return result
 
 
-class ValidatorRelation(BaseModel):
+class ValidatorRelationModel(BaseModel):
     id = AutoField(primary_key=True)
     wt_name = CharField(max_length=128, index=True)
     validator = CharField(index=True)
     params = TextField(null=True)
     update_time = DateTimeField(default=datetime.datetime.now)
     create_time = DateTimeField(default=datetime.datetime.now)
```

### Comparing `data_watchtower-0.0.3/data_watchtower/model/services.py` & `data_watchtower-0.0.4/data_watchtower/model/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import logging
 import datetime
 import shortuuid
 from peewee import fn, JOIN
 from peewee import IntegrityError
-from playhouse.db_url import connect
-from data_watchtower.model.models import ValidationDetail, Watchtower, database_proxy, ValidatorRelation
-from data_watchtower.utils import json_dumps, json_loads
+from data_watchtower.model.models import ValidationDetailModel, WatchtowerModel, database_proxy, ValidatorRelationModel
+from data_watchtower.utils import json_dumps, json_loads, connect_db_from_url
 
 logger = logging.getLogger(__name__)
 
 
 class DbServices(object):
     def __init__(self, connection):
         """
         可以使用db_url进行数据库连接. 用法: https://docs.peewee-orm.com/en/latest/peewee/playhouse.html#db-url
         或者直接使用peewee的Database对象
         :param connection:
             str: eg: sqlite:///data.db mysql://user:passwd@ip:port/my_db
             other: eg. MySQLDatabase, PostgresqlDatabase ...
         """
         if isinstance(connection, str):
-            self.database = connect(url=connection)
+            self.database = connect_db_from_url(url=connection)
         else:
             self.database = connection
         database_proxy.initialize(self.database)
 
     def create_tables(self):
-        models = [Watchtower, ValidationDetail, ValidatorRelation]
+        models = [WatchtowerModel, ValidationDetailModel, ValidatorRelationModel]
         with self.database:
             for model in models:
                 if not self.database.table_exists(model):
                     self.database.create_tables([model])
 
     def get_watchtower(self, name):
-        model = Watchtower.get(Watchtower.name == name).get()
+        model = WatchtowerModel.get(WatchtowerModel.name == name).get()
         item = model.to_dict()
         if item is not None:
             item['data_loader'] = json_loads(item['data_loader'])
             # item['validators'] = json_loads(item['validators'])
-        validators = ValidatorRelation.select().where(ValidatorRelation.wt_name == name)
+        validators = ValidatorRelationModel.select().where(ValidatorRelationModel.wt_name == name)
         item['validators'] = []
         for validator_item in validators:
             validator = dict(
                 params=json_loads(validator_item.params),
                 __class__=validator_item.validator,
             )
             item['validators'].append(validator)
@@ -52,77 +51,78 @@
 
     def get_watchtowers(self):
         """
         获取所有的watchtower
         :return:
         """
         result = []
-        query = Watchtower.select(
-            Watchtower.name,
-            Watchtower.success,
-            Watchtower.run_time,
-            Watchtower.data_loader,
-            Watchtower.success_method,
-            Watchtower.validator_success_method,
+        query = WatchtowerModel.select(
+            WatchtowerModel.name,
+            WatchtowerModel.success,
+            WatchtowerModel.schedule,
+            WatchtowerModel.run_time,
+            WatchtowerModel.data_loader,
+            WatchtowerModel.success_method,
+            WatchtowerModel.validator_success_method,
         )
         for item in query:
             result.append(item.to_dict(fields_from_query=query))
         return result
 
     def add_watchtower(self, watchtower):
         update_time = datetime.datetime.now()
         try:
             with self.database.atomic():
                 item = watchtower.to_dict()
                 item['create_time'] = update_time
                 item['update_time'] = update_time
-                wt = Watchtower(**item)
+                wt = WatchtowerModel(**item)
                 wt.save(force_insert=True)
                 validators = []
                 for validator_item in watchtower.get_validator_meta():
-                    inst = ValidatorRelation(
+                    inst = ValidatorRelationModel(
                         wt_name=watchtower.name,
                         validator=validator_item['__class__'],
                         params=json_dumps(validator_item['params']),
                     )
                     validators.append(inst)
-                ValidatorRelation.bulk_create(validators, batch_size=100)
+                ValidatorRelationModel.bulk_create(validators, batch_size=100)
         except IntegrityError as e:
             logger.warning('add watchtower error!. msg:%s' % str(e))
             return
 
     def update_watchtower(self, wt_name, **item):
         if len(item) == 0:
             return 0
         update_time = datetime.datetime.now()
         with self.database.atomic():
-            wt = Watchtower.select().where(Watchtower.name == wt_name).get()
+            wt = WatchtowerModel.select().where(WatchtowerModel.name == wt_name).get()
             if wt:
                 if 'validators' in item:
                     validators = []
                     for validator_item in wt.get_validator_meta():
-                        inst = ValidatorRelation(
+                        inst = ValidatorRelationModel(
                             wt_name=wt.name,
                             validator=validator_item['__class__'],
                             params=json_dumps(validator_item['params']),
                         )
                         validators.append(inst)
-                    ValidatorRelation.bulk_create(validators, batch_size=100)
+                    ValidatorRelationModel.bulk_create(validators, batch_size=100)
                 if 'data_loader' in item:
                     wt.validators = json_dumps(item.pop('data_loader'))
                 for k, v in item.items():
                     setattr(wt, k, v)
                 wt.update_time = update_time
                 return wt.save()
             else:
                 return 0
 
     def delete_watchtower(self, watchtower):
         with self.database.atomic():
-            wt = Watchtower.select().where(Watchtower.name == watchtower.wt_name).get()
+            wt = WatchtowerModel.select().where(WatchtowerModel.name == watchtower.wt_name).get()
             if wt:
                 return wt.delete_instance()
             else:
                 return 0
 
     def save_result(self, watchtower, result):
         update_time = datetime.datetime.now()
@@ -156,23 +156,24 @@
                 run_type=2,
                 update_time=update_time,
                 create_time=update_time,
 
             )
             records.append(row)
         with self.database.atomic():
-            ValidationDetail.insert_many(records).execute()
+            ValidationDetailModel.insert_many(records).execute()
+        self.update_watchtower_success_status(watchtower)
         return
 
     def compute_watchtower_success_status(self, watchtower):
         wt_name = watchtower.name
         success_method = watchtower.validator_success_method
         if success_method == 'all':
-            DetailAlias = ValidationDetail.alias()
-            DetailAliasBase = ValidationDetail.alias('base')
+            DetailAlias = ValidationDetailModel.alias()
+            DetailAliasBase = ValidationDetailModel.alias('base')
             join_query = DetailAlias.select(
                 DetailAlias.name,
                 fn.MAX(DetailAlias.run_time).alias('run_time')
             ).where(
                 (DetailAlias.wt_name == wt_name) & (DetailAlias.run_type == 1)
             ).group_by(DetailAlias.name).alias('join_query')
             predicate = ((DetailAliasBase.name == join_query.c.name) &
@@ -182,17 +183,17 @@
                 DetailAliasBase.run_id
             ).join(
                 join_query, JOIN.INNER, on=predicate
             ).where(cond)
             return not query.exists()
         elif success_method == 'last':
             query = (
-                ValidationDetail.select(ValidationDetail.success)
-                .where((ValidationDetail.wt_name == wt_name) & (ValidationDetail.run_type == 1))
-                .order_by(ValidationDetail.run_time.desc())
+                ValidationDetailModel.select(ValidationDetailModel.success)
+                .where((ValidationDetailModel.wt_name == wt_name) & (ValidationDetailModel.run_type == 1))
+                .order_by(ValidationDetailModel.run_time.desc())
                 .limit(1)
             )
             item = query.get()
             if item:
                 return True
             else:
                 return item.success
@@ -201,13 +202,13 @@
 
     def update_watchtower_success_status(self, watchtower):
         run_time = datetime.datetime.now()
         success = self.compute_watchtower_success_status(watchtower)
         self.update_watchtower(watchtower.name, success=success, run_time=run_time)
 
     def add_validator_to_watchtower(self, wt_name, validator, params):
-        inst = ValidatorRelation(
+        inst = ValidatorRelationModel(
             wt_name=wt_name,
             validator=validator,
             params=params,
         )
         return inst.save(force_insert=True)
```

### Comparing `data_watchtower-0.0.3/data_watchtower/utils.py` & `data_watchtower-0.0.4/data_watchtower/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+import inspect
 import re
 import json
 import copy
 import importlib
+from pkgutil import iter_modules
 from string import Template
 
 from attrs import asdict
+from playhouse.db_url import connect
+
+
+def connect_db_from_url(url, **connect_params):
+    return connect(url, unquote_password=True, **connect_params)
 
 
 def load_object(path):
     if not isinstance(path, str):
         if callable(path):
             return path
         else:
@@ -176,27 +183,53 @@
 
     if isinstance(obj, str):
         return obj
     return json.dumps(obj, default=_default_encoder, ensure_ascii=True)
 
 
 def json_loads(data):
-    if isinstance(data, str):
+    if not data:
+        return None
+    if isinstance(data, (str, bytes)):
         return json.loads(data)
     else:
         return data
 
 
-def dump_macro_map(macro_map):
-    """
-    把模板转换成字符串
-    :param macro_map:
-    :return:
-    """
+def walk_modules(path):
+    mods = []
+    mod = importlib.import_module(path)
+    mods.append(mod)
+    if hasattr(mod, '__path__'):
+        for _, sub_path, is_pkg in iter_modules(mod.__path__):
+            full_path = path + '.' + sub_path
+            if is_pkg:
+                mods += walk_modules(full_path)
+            else:
+                sub_mod = importlib.import_module(full_path)
+                mods.append(sub_mod)
+    return mods
+
+
+def load_subclasses(root_modules, base_class):
+    result = []
+    for root_module in root_modules:
+        for m in walk_modules(root_module):
+            for obj in vars(m).values():
+                if inspect.isclass(obj) and issubclass(obj, base_class) and obj.__module__ == m.__name__:
+                    result.append(obj)
+    return result
+
 
+def get_subclasses(cls):
+    subclasses = []
+    for subclass in cls.__subclasses__():
+        subclasses.append(subclass)
+        subclasses.extend(get_subclasses(subclass))
+    return subclasses
     pass
 
 
 def f2():
     return 1
```

