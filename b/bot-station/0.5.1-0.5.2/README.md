# Comparing `tmp/bot_station-0.5.1.tar.gz` & `tmp/bot_station-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot_station-0.5.1.tar", last modified: Sun May 12 11:26:29 2024, max compression
+gzip compressed data, was "bot_station-0.5.2.tar", last modified: Mon May 13 20:36:11 2024, max compression
```

## Comparing `bot_station-0.5.1.tar` & `bot_station-0.5.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.921828 bot_station-0.5.1/
--rw-r--r--   0 mmarashan (1826057312) 593637566     1070 2024-05-05 19:58:38.000000 bot_station-0.5.1/LICENSE
--rw-r--r--   0 mmarashan (1826057312) 593637566      755 2024-05-12 11:26:29.921660 bot_station-0.5.1/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566       65 2024-05-12 11:26:11.000000 bot_station-0.5.1/README.md
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.913579 bot_station-0.5.1/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.914356 bot_station-0.5.1/bot_station/api/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.914541 bot_station-0.5.1/bot_station/api/rest/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     7837 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/api/rest/api.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.916075 bot_station-0.5.1/bot_station/api/rest/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      257 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_call_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      331 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      482 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_creation_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      126 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_creation_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      433 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      401 2024-05-08 19:40:03.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_train_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566       90 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/bot_train_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      204 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/api/rest/model/web_app_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.916195 bot_station-0.5.1/bot_station/data/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.916281 bot_station-0.5.1/bot_station/data/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/base/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.916746 bot_station-0.5.1/bot_station/data/base/database/
--rw-r--r--   0 mmarashan (1826057312) 593637566      975 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/base/database/UUID.py
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/base/database/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      428 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/base/database/base_db_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.917165 bot_station-0.5.1/bot_station/data/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1291 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/data/bot/bot_factory_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     8454 2024-05-12 11:00:18.000000 bot_station-0.5.1/bot_station/data/bot/bot_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2169 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot/chat_message_storage_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.917365 bot_station-0.5.1/bot_station/data/bot/mapper/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot/mapper/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      972 2024-05-08 19:40:03.000000 bot_station-0.5.1/bot_station/data/bot/mapper/document_mapper.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.917850 bot_station-0.5.1/bot_station/data/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      124 2024-05-10 19:41:12.000000 bot_station-0.5.1/bot_station/data/bot/model/qdrant_config.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      128 2024-05-10 19:41:18.000000 bot_station-0.5.1/bot_station/data/bot/model/yandex_cloud_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.918213 bot_station-0.5.1/bot_station/data/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566      508 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     3431 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/data/bot_station/bot_registry_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.918406 bot_station-0.5.1/bot_station/data/bot_station/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/data/bot_station/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      853 2024-05-08 19:40:03.000000 bot_station-0.5.1/bot_station/data/bot_station/model/bot_info_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.918678 bot_station-0.5.1/bot_station/di/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/di/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1529 2024-05-10 19:53:19.000000 bot_station-0.5.1/bot_station/di/bot_station_module.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.919009 bot_station-0.5.1/bot_station/domain/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.919440 bot_station-0.5.1/bot_station/domain/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/base/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      605 2024-05-10 20:00:38.000000 bot_station-0.5.1/bot_station/domain/base/const.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/base/utils.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.919879 bot_station-0.5.1/bot_station/domain/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      970 2024-05-12 11:00:18.000000 bot_station-0.5.1/bot_station/domain/bot/bot.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      260 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/domain/bot/bot_factory.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      798 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/chat_message_storage.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.920680 bot_station-0.5.1/bot_station/domain/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      348 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/domain/bot/model/bot_meta_info.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      222 2024-05-08 19:40:03.000000 bot_station-0.5.1/bot_station/domain/bot/model/document.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      254 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/model/lm_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      361 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/model/lm_chat_message.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      379 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot/model/lm_train_data.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.920998 bot_station-0.5.1/bot_station/domain/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/bot_station/domain/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      571 2024-05-10 21:06:41.000000 bot_station-0.5.1/bot_station/domain/bot_station/bot_registry.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2981 2024-05-12 11:02:36.000000 bot_station-0.5.1/bot_station/domain/bot_station/bot_station.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.921456 bot_station-0.5.1/bot_station.egg-info/
--rw-r--r--   0 mmarashan (1826057312) 593637566      755 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566     2295 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/SOURCES.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566        1 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/dependency_links.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566      190 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/requires.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       18 2024-05-12 11:26:29.000000 bot_station-0.5.1/bot_station.egg-info/top_level.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       38 2024-05-12 11:26:29.921863 bot_station-0.5.1/setup.cfg
--rw-r--r--   0 mmarashan (1826057312) 593637566      834 2024-05-08 19:40:03.000000 bot_station-0.5.1/setup.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-12 11:26:29.921290 bot_station-0.5.1/tests/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.1/tests/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     5606 2024-05-12 11:21:25.000000 bot_station-0.5.1/tests/bot_station_api_test.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1426 2024-05-12 11:03:13.000000 bot_station-0.5.1/tests/test_bot_factory.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.198849 bot_station-0.5.2/
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1070 2024-05-05 19:58:38.000000 bot_station-0.5.2/LICENSE
+-rw-r--r--   0 mmarashan (1826057312) 593637566      750 2024-05-13 20:36:11.198642 bot_station-0.5.2/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) 593637566       60 2024-05-13 20:36:00.000000 bot_station-0.5.2/README.md
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.181613 bot_station-0.5.2/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.182342 bot_station-0.5.2/bot_station/api/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.182554 bot_station-0.5.2/bot_station/api/rest/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     7837 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/api/rest/api.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.184364 bot_station-0.5.2/bot_station/api/rest/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      257 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_call_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      331 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      482 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_creation_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      126 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_creation_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      433 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      401 2024-05-08 19:40:03.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_train_dto.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566       90 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_train_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      204 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/web_app_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.184494 bot_station-0.5.2/bot_station/data/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.184584 bot_station-0.5.2/bot_station/data/base/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/base/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.184947 bot_station-0.5.2/bot_station/data/base/database/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      975 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/base/database/UUID.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/base/database/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      428 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/base/database/base_db_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.185487 bot_station-0.5.2/bot_station/data/bot/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1291 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/data/bot/bot_factory_impl.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     8108 2024-05-13 20:34:22.000000 bot_station-0.5.2/bot_station/data/bot/bot_impl.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2169 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot/chat_message_storage_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.185727 bot_station-0.5.2/bot_station/data/bot/mapper/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot/mapper/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      972 2024-05-08 19:40:03.000000 bot_station-0.5.2/bot_station/data/bot/mapper/document_mapper.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.186381 bot_station-0.5.2/bot_station/data/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      124 2024-05-10 19:41:12.000000 bot_station-0.5.2/bot_station/data/bot/model/qdrant_config.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      128 2024-05-10 19:41:18.000000 bot_station-0.5.2/bot_station/data/bot/model/yandex_cloud_config.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.186917 bot_station-0.5.2/bot_station/data/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      508 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     3431 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/data/bot_station/bot_registry_impl.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.187266 bot_station-0.5.2/bot_station/data/bot_station/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot_station/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      853 2024-05-08 19:40:03.000000 bot_station-0.5.2/bot_station/data/bot_station/model/bot_info_dto.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.187624 bot_station-0.5.2/bot_station/di/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/di/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1529 2024-05-10 19:53:19.000000 bot_station-0.5.2/bot_station/di/bot_station_module.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.187876 bot_station-0.5.2/bot_station/domain/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/__init__.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.193861 bot_station-0.5.2/bot_station/domain/base/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/base/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      605 2024-05-10 20:00:38.000000 bot_station-0.5.2/bot_station/domain/base/const.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/base/utils.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.194905 bot_station-0.5.2/bot_station/domain/bot/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      970 2024-05-12 11:00:18.000000 bot_station-0.5.2/bot_station/domain/bot/bot.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      260 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/domain/bot/bot_factory.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      798 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/chat_message_storage.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.196815 bot_station-0.5.2/bot_station/domain/bot/model/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/model/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      348 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/domain/bot/model/bot_meta_info.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      222 2024-05-08 19:40:03.000000 bot_station-0.5.2/bot_station/domain/bot/model/document.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      254 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/model/lm_call_result.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      361 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/model/lm_chat_message.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      379 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/model/lm_train_data.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.197384 bot_station-0.5.2/bot_station/domain/bot_station/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot_station/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566      571 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/domain/bot_station/bot_registry.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2981 2024-05-12 11:02:36.000000 bot_station-0.5.2/bot_station/domain/bot_station/bot_station.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.198396 bot_station-0.5.2/bot_station.egg-info/
+-rw-r--r--   0 mmarashan (1826057312) 593637566      750 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/PKG-INFO
+-rw-r--r--   0 mmarashan (1826057312) 593637566     2295 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/SOURCES.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566        1 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/dependency_links.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566      190 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/requires.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566       18 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/top_level.txt
+-rw-r--r--   0 mmarashan (1826057312) 593637566       38 2024-05-13 20:36:11.198894 bot_station-0.5.2/setup.cfg
+-rw-r--r--   0 mmarashan (1826057312) 593637566      834 2024-05-08 19:40:03.000000 bot_station-0.5.2/setup.py
+drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.198041 bot_station-0.5.2/tests/
+-rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/tests/__init__.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     5606 2024-05-12 11:21:25.000000 bot_station-0.5.2/tests/bot_station_api_test.py
+-rw-r--r--   0 mmarashan (1826057312) 593637566     1426 2024-05-12 11:03:13.000000 bot_station-0.5.2/tests/test_bot_factory.py
```

### Comparing `bot_station-0.5.1/LICENSE` & `bot_station-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/PKG-INFO` & `bot_station-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.5.1
+Version: 0.5.2
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -16,9 +16,9 @@
 Requires-Dist: fastembed==0.2.7
 Requires-Dist: yandexcloud==0.271.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: fastapi==0.110.3
 Requires-Dist: uvicorn==0.29.0
 
-# Bot Station SDK 0.5.1
-What's new: Fix of clear bot after update
+# Bot Station SDK 0.5.2
+What's new: Fix empty docs in prompt
```

### Comparing `bot_station-0.5.1/bot_station/api/rest/api.py` & `bot_station-0.5.2/bot_station/api/rest/api.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/data/base/database/UUID.py` & `bot_station-0.5.2/bot_station/data/base/database/UUID.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/data/bot/bot_factory_impl.py` & `bot_station-0.5.2/bot_station/data/bot/bot_factory_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/data/bot/bot_impl.py` & `bot_station-0.5.2/bot_station/data/bot/bot_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,32 +122,24 @@
 
         # 2. Add context to prompt
         relevant_docs: List[LangchainDocument] = []
         if self.meta.add_external_context_to_prompt:
             relevant_docs = self.knowledge_retriever.get_relevant_documents(
                 query=question.text
             )
-            if len(relevant_docs) > 1:
+            if len(relevant_docs) > 0:
                 reordered_documents: List[LangchainDocument] = list(
                     LongContextReorder().transform_documents(relevant_docs)
                 )
                 prompt_with_question = (
                         prompt_with_question
-                        + "\n\nДля ответа используй только следующие документы:\n"
+                        + "\n\nДля ответа используй только следующие знания:\n"
                 )
                 for d in reordered_documents:
-                    logging.debug(f"Add doc to prompt: {d}")
-                    link = d.metadata.get("link", None)
-                    doc_in_text = {"Tекст": d.page_content}
-                    if link is not None:
-                        doc_in_text["Источник"] = link
-
-                    prompt_with_question = (
-                            prompt_with_question + str(doc_in_text) + "\n"
-                    )
+                    prompt_with_question = prompt_with_question + d.page_content + "\n"
 
         prompt_with_question = (
                 prompt_with_question + "\n\n Сообщение пользователя: " + question.text
         )
 
         logging.debug(f"Running LLM Chain")
```

### Comparing `bot_station-0.5.1/bot_station/data/bot/chat_message_storage_impl.py` & `bot_station-0.5.2/bot_station/data/bot/chat_message_storage_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/data/bot/mapper/document_mapper.py` & `bot_station-0.5.2/bot_station/data/bot/mapper/document_mapper.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/data/bot_station/bot_registry_impl.py` & `bot_station-0.5.2/bot_station/data/bot_station/bot_registry_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/data/bot_station/model/bot_info_dto.py` & `bot_station-0.5.2/bot_station/data/bot_station/model/bot_info_dto.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/di/bot_station_module.py` & `bot_station-0.5.2/bot_station/di/bot_station_module.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/domain/base/const.py` & `bot_station-0.5.2/bot_station/domain/base/const.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/domain/bot/bot.py` & `bot_station-0.5.2/bot_station/domain/bot/bot.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/domain/bot/chat_message_storage.py` & `bot_station-0.5.2/bot_station/domain/bot/chat_message_storage.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/domain/bot_station/bot_registry.py` & `bot_station-0.5.2/bot_station/domain/bot_station/bot_registry.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station/domain/bot_station/bot_station.py` & `bot_station-0.5.2/bot_station/domain/bot_station/bot_station.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/bot_station.egg-info/PKG-INFO` & `bot_station-0.5.2/bot_station.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.5.1
+Version: 0.5.2
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -16,9 +16,9 @@
 Requires-Dist: fastembed==0.2.7
 Requires-Dist: yandexcloud==0.271.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: fastapi==0.110.3
 Requires-Dist: uvicorn==0.29.0
 
-# Bot Station SDK 0.5.1
-What's new: Fix of clear bot after update
+# Bot Station SDK 0.5.2
+What's new: Fix empty docs in prompt
```

### Comparing `bot_station-0.5.1/bot_station.egg-info/SOURCES.txt` & `bot_station-0.5.2/bot_station.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/setup.py` & `bot_station-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/tests/bot_station_api_test.py` & `bot_station-0.5.2/tests/bot_station_api_test.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.1/tests/test_bot_factory.py` & `bot_station-0.5.2/tests/test_bot_factory.py`

 * *Files identical despite different names*

