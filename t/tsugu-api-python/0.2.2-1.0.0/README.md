# Comparing `tmp/tsugu-api-python-0.2.2.tar.gz` & `tmp/tsugu-api-python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-0.2.2.tar", last modified: Sun May 12 05:09:54 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.0.0.tar", last modified: Mon May 13 01:41:07 2024, max compression
```

## Comparing `tsugu-api-python-0.2.2.tar` & `tsugu-api-python-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.969159 tsugu-api-python-0.2.2/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.969159 tsugu-api-python-0.2.2/tsugu_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v1/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v1/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v1/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api/v2/_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api_async/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v1/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v1/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v1/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api_async/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-12 05:09:46.000000 tsugu-api-python-0.2.2/tsugu_api_async/v2/_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:09:54.973159 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-12 05:09:54.000000 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-12 05:09:54.000000 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 05:09:54.000000 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 05:09:54.000000 tsugu-api-python-0.2.2/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-13 01:40:59.000000 tsugu-api-python-1.0.0/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:41:07.560061 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-13 01:41:07.000000 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-13 01:41:07.000000 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 01:41:07.000000 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 01:41:07.000000 tsugu-api-python-1.0.0/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-0.2.2/LICENSE` & `tsugu-api-python-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.2/PKG-INFO` & `tsugu-api-python-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 0.2.2
+Version: 1.0.0
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -15,19 +15,15 @@
         _✨ Python 编写的 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 相关各种功能 API 调用库  ✨_
         
         </div>
         
         <p align="center">
         
         <a href="https://github.com/Yamamoto-2/tsugu-bangdream-bot">
-          <img src="https://img.shields.io/badge/tsugu bangdream bot-v1 api-FFEE88" alt="license">
-        </a>
-        
-        <a href="https://github.com/Yamamoto-2/tsugu-bangdream-bot">
-          <img src="https://img.shields.io/badge/tsugu bangdream bot-v2 api-FFEE88" alt="license">
+          <img src="https://img.shields.io/badge/tsugu bangdream bot-api-FFEE88" alt="license">
         </a>
         
         <a href="https://github.com/WindowsSov8forUs/tsugu-api-python">
           <img src="https://img.shields.io/github/v/release/WindowsSov8forUs/tsugu-api-python" alt="Latest Release Version">
         </a>
         
         <a href="https://github.com/WindowsSov8forUs/tsugu-api-python/blob/main/LICENSE">
@@ -50,71 +46,65 @@
         
         ### 目前已有的功能
         
         > 所有方法都同时拥有异步与同步版本。
         
         #### Tsugu 后端功能
         
-        > **`None`** 表示该功能没有相应的方法。
-        
-        |功能描述|v1 方法名称|v2 方法名称|
-        |:------|:----------|:---------|
-        |获取卡面图片|`get_card_illustration`|`card_illustration`|
-        |获取玩家状态信息|`search_player`|`player`|
-        |模拟指定卡池抽卡结果|`gacha_simulate`|`gacha_simulate`|
-        |查询指定卡池信息|`search_gacha`|`gacha`|
-        |查询符合条件的活动信息|`search_event`|`event`|
-        |查询符合条件的歌曲信息|`search_song`|`song`|
-        |查询歌曲分数表|`song_meta`|`song_meta`|
-        |查询符合条件的角色信息|`search_character`|`character`|
-        |查询指定歌曲指定难度的谱面|`song_chart`|`chart`|
-        |查询指定活动的全部档位预测线|`ycx_all`|`ycx_all`|
-        |查询指定活动的指定档位预测线|`ycx`|`ycx`|
-        |查询指定活动指定档位相关的历史预测线|`lsycx`|`lsycx`|
-        |获取指定车牌列表的图片形式|`room_list`|**`None`**|
-        |查询符合条件的卡牌|`search_card`|`card`|
-        |从后端获取最近的车牌信息列表|`station_query_all_room`|**`None`**|
-        |提交车牌信息到后端|`station_submit_room_number`|**`None`**|
-        |获取最近的车牌信息数据|**`None`**|`ycm`|
-        
-        > 部分功能类似的方法在 `v1` 和 `v2` 中调用方式并不相同。
+        |功能描述|方法名称|
+        |:------|:----------|
+        |获取活动试炼舞台信息|`event_stage`|
+        |模拟指定卡池抽卡结果|`gacha_simulate`|
+        |获取卡面图片|`get_card_illustration`|
+        |查询指定活动指定档位相关的历史预测线|`lsycx`|
+        |获取指定车牌列表的图片形式|`room_list`|
+        |查询符合条件的卡牌|`search_card`|
+        |查询符合条件的角色信息|`search_character`|
+        |查询符合条件的活动信息|`search_event`|
+        |查询指定卡池信息|`search_gacha`|
+        |获取玩家状态信息|`search_player`|
+        |查询符合条件的歌曲信息|`search_song`|
+        |查询指定歌曲指定难度的谱面|`song_chart`|
+        |查询歌曲分数表|`song_meta`|
+        |查询指定活动的指定档位预测线|`ycx`|
+        |查询指定活动的全部档位预测线|`ycx_all`|
+        |提交车牌信息到后端|`station_submit_room_number`|
+        |从后端获取最近的车牌信息列表|`station_query_all_room`|
         
-        #### 用户数据后端功能 (仅 `v1` )
+        #### 用户数据后端功能
         
-        |功能描述|v1 方法名称|
+        |功能描述|方法名称|
         |:------|:----------|
-        获取用户数据|`get_user_data`|
-        发送绑定用户请求|`bind_player_request`|
-        验证绑定用户请求|`bind_player_verification`|
-        设置是否转发指定用户的车牌|`set_car_forwarding`|
-        设置指定用户的默认服务器列表|`set_default_server`|
-        设置指定用户的主服务器模式|`set_server_mode`|
+        |获取用户数据|`get_user_data`|
+        |修改用户数据|`change_user_data`|
+        |发送绑定用户请求|`bind_player_request`|
+        |验证绑定用户请求|`bind_player_verification`|
         
         > 以上功能都可使用本地用户数据库代替，本 API 不提供相关的配置方法。
         
-        #### 车站功能 (仅 `v1` )
+        #### 车站功能
         
-        |功能描述|v1 方法名称|
+        |功能描述|方法名称|
         |:------|:----------|
         |提交车牌信息到车站|`submit_room_number`|
         
         
         ## 快速使用
         
-        以下将以获取歌曲 **EXIST** (id=325) 和卡面 **羽沢 つぐみ - Precious birthday！** (id=1672) 的信息为例。
+        以下将以获取歌曲 **EXIST** (id=325) 的信息为例。
         
         使用以下指令安装本模块：
         ```bash
         $ pip3 install tsugu-api-python
         ```
         
-        首先是使用如下代码，通过 `v1` 版本获取指定歌曲信息图片：
+        使用如下代码，获取指定歌曲信息图片：
         
         ```python
-        from tsugu_api.v1 import search_song
+        from tsugu_api import search_song
         
         def main() -> None:
             result = search_song([3, 0], "EXIST") # 这里也可以传入 "325" ，具体取决于用户输入信息
         
         main()
         ```
         
@@ -122,47 +112,14 @@
         
         获取到的 `result` 将是一个 `_Response` 对象，当获取到准确的信息时， `result` 的值如下：
         
         ```python
         [
             {
                 "type": "base64",
-                "string": ... # 图片的 Base64 字符串
-            }
-        ]
-        ```
-        
-        若传入的查询参数不合法或查询过程中出错，获取到的 `result` 的值如下：
-        
-        ```python
-        [
-            {
-                "type": "string",
-                "string": ... # 错误信息
-            }
-        ]
-        ```
-        
-        然后是使用如下代码，通过 `v2` 版本获取指定卡牌信息图片：
-        
-        ```python
-        from tsugu_api.v2 import card
-        
-        def main() -> None:
-            result = card("1672", [3, 0]) # 这里也可以传入其他字符串 ，结果将变为一个符合参数的卡牌列表图片
-        
-        main()
-        ```
-        
-        获取到的 `result` 将是一个 `_Response` 对象，当获取到准确的信息时， `result` 的值如下：
-        
-        ```python
-        [
-            {
-                "type": "base64",
                 "string": ... # 图片的 Base64 字符串
             }
         ]
         ```
         
         若传入的查询参数不合法或查询过程中出错，获取到的 `result` 的值如下：
```

#### html2text {}

```diff
@@ -1,79 +1,62 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.2 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.0 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
-      _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
+          _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
 ## è¯´æ è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [TsuguBanGDreamBot](https://
 github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file)
 ç¸å³åç§åè½ API çåºï¼åæ¬ç»å¤§é¨å Tsugu
 æä¾çåè½ãä½¿ç¨æ¬ API
 åºæä¾çæ¹æ³å¯ä»¥å®ç°ç»å¤§é¨ååè½ï¼èæ­é [bestdori-api]
 (https://github.com/WindowsSov8forUs/bestdori-api)
 å¯ä»¥å®ç°ç¨æ·ç»å®ç­å¶ä»åè½ã > è¯¥ API
 åºåæ¶æä¾äºå¼æ­¥ä¸åæ­¥çæ¬ï¼å¯èªè¡éæ©ä½¿ç¨ã >
 ä¸åæ°æ®è·åç­æä½éè¿éç½®çåç«¯æå¡å¨è¿è¡ï¼è¯¥ API
 åºåªæä¾åç«¯æéçè°ç¨åè½ãè¥éè¦ä½¿ç¨æ¬å°æ°æ®åºï¼è¯·èªè¡æä½ã
 ### ç®åå·²æçåè½ > æææ¹æ³é½åæ¶æ¥æå¼æ­¥ä¸åæ­¥çæ¬ã
-#### Tsugu åç«¯åè½ > **`None`** è¡¨ç¤ºè¯¥åè½æ²¡æç¸åºçæ¹æ³ã
-|åè½æè¿°|v1 æ¹æ³åç§°|v2 æ¹æ³åç§°| |:------|:----------|:---------
-| |è·åå¡é¢å¾ç|`get_card_illustration`|`card_illustration`|
-|è·åç©å®¶ç¶æä¿¡æ¯|`search_player`|`player`|
-|æ¨¡ææå®å¡æ± æ½å¡ç»æ|`gacha_simulate`|`gacha_simulate`|
-|æ¥è¯¢æå®å¡æ± ä¿¡æ¯|`search_gacha`|`gacha`|
-|æ¥è¯¢ç¬¦åæ¡ä»¶çæ´»å¨ä¿¡æ¯|`search_event`|`event`|
-|æ¥è¯¢ç¬¦åæ¡ä»¶çæ­æ²ä¿¡æ¯|`search_song`|`song`|
-|æ¥è¯¢æ­æ²åæ°è¡¨|`song_meta`|`song_meta`|
-|æ¥è¯¢ç¬¦åæ¡ä»¶çè§è²ä¿¡æ¯|`search_character`|`character`|
-|æ¥è¯¢æå®æ­æ²æå®é¾åº¦çè°±é¢|`song_chart`|`chart`|
-|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`|`ycx_all`|
-|æ¥è¯¢æå®æ´»å¨çæå®æ¡£ä½é¢æµçº¿|`ycx`|`ycx`|
-|æ¥è¯¢æå®æ´»å¨æå®æ¡£ä½ç¸å³çåå²é¢æµçº¿|`lsycx`|`lsycx`|
-|è·åæå®è½¦çåè¡¨çå¾çå½¢å¼|`room_list`|**`None`**|
-|æ¥è¯¢ç¬¦åæ¡ä»¶çå¡ç|`search_card`|`card`|
-|ä»åç«¯è·åæè¿çè½¦çä¿¡æ¯åè¡¨|`station_query_all_room`|**`None`**|
-|æäº¤è½¦çä¿¡æ¯å°åç«¯|`station_submit_room_number`|**`None`**|
-|è·åæè¿çè½¦çä¿¡æ¯æ°æ®|**`None`**|`ycm`| >
-é¨ååè½ç±»ä¼¼çæ¹æ³å¨ `v1` å `v2` ä¸­è°ç¨æ¹å¼å¹¶ä¸ç¸åã
-#### ç¨æ·æ°æ®åç«¯åè½ (ä» `v1` ) |åè½æè¿°|v1 æ¹æ³åç§°| |:----
---|:----------| è·åç¨æ·æ°æ®|`get_user_data`|
-åéç»å®ç¨æ·è¯·æ±|`bind_player_request`|
-éªè¯ç»å®ç¨æ·è¯·æ±|`bind_player_verification`|
-è®¾ç½®æ¯å¦è½¬åæå®ç¨æ·çè½¦ç|`set_car_forwarding`|
-è®¾ç½®æå®ç¨æ·çé»è®¤æå¡å¨åè¡¨|`set_default_server`|
-è®¾ç½®æå®ç¨æ·çä¸»æå¡å¨æ¨¡å¼|`set_server_mode`| >
+#### Tsugu åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+| |è·åæ´»å¨è¯ç¼èå°ä¿¡æ¯|`event_stage`|
+|æ¨¡ææå®å¡æ± æ½å¡ç»æ|`gacha_simulate`|
+|è·åå¡é¢å¾ç|`get_card_illustration`|
+|æ¥è¯¢æå®æ´»å¨æå®æ¡£ä½ç¸å³çåå²é¢æµçº¿|`lsycx`|
+|è·åæå®è½¦çåè¡¨çå¾çå½¢å¼|`room_list`|
+|æ¥è¯¢ç¬¦åæ¡ä»¶çå¡ç|`search_card`|
+|æ¥è¯¢ç¬¦åæ¡ä»¶çè§è²ä¿¡æ¯|`search_character`|
+|æ¥è¯¢ç¬¦åæ¡ä»¶çæ´»å¨ä¿¡æ¯|`search_event`|
+|æ¥è¯¢æå®å¡æ± ä¿¡æ¯|`search_gacha`|
+|è·åç©å®¶ç¶æä¿¡æ¯|`search_player`|
+|æ¥è¯¢ç¬¦åæ¡ä»¶çæ­æ²ä¿¡æ¯|`search_song`|
+|æ¥è¯¢æå®æ­æ²æå®é¾åº¦çè°±é¢|`song_chart`|
+|æ¥è¯¢æ­æ²åæ°è¡¨|`song_meta`|
+|æ¥è¯¢æå®æ´»å¨çæå®æ¡£ä½é¢æµçº¿|`ycx`|
+|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`|
+|æäº¤è½¦çä¿¡æ¯å°åç«¯|`station_submit_room_number`|
+|ä»åç«¯è·åæè¿çè½¦çä¿¡æ¯åè¡¨|`station_query_all_room`| ####
+ç¨æ·æ°æ®åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+| |è·åç¨æ·æ°æ®|`get_user_data`| |ä¿®æ¹ç¨æ·æ°æ®|`change_user_data`|
+|åéç»å®ç¨æ·è¯·æ±|`bind_player_request`|
+|éªè¯ç»å®ç¨æ·è¯·æ±|`bind_player_verification`| >
 ä»¥ä¸åè½é½å¯ä½¿ç¨æ¬å°ç¨æ·æ°æ®åºä»£æ¿ï¼æ¬ API
-ä¸æä¾ç¸å³çéç½®æ¹æ³ã #### è½¦ç«åè½ (ä» `v1` )
-|åè½æè¿°|v1 æ¹æ³åç§°| |:------|:----------
-| |æäº¤è½¦çä¿¡æ¯å°è½¦ç«|`submit_room_number`| ## å¿«éä½¿ç¨
-ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) åå¡é¢ **ç¾½æ²¢ ã¤ãã¿ -
-Precious birthdayï¼** (id=1672) çä¿¡æ¯ä¸ºä¾ã
+ä¸æä¾ç¸å³çéç½®æ¹æ³ã #### è½¦ç«åè½ |åè½æè¿°|æ¹æ³åç§°|
+|:------|:----------| |æäº¤è½¦çä¿¡æ¯å°è½¦ç«|`submit_room_number`| ##
+å¿«éä½¿ç¨ ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) çä¿¡æ¯ä¸ºä¾ã
 ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install tsugu-api-python
-``` é¦åæ¯ä½¿ç¨å¦ä¸ä»£ç ï¼éè¿ `v1`
-çæ¬è·åæå®æ­æ²ä¿¡æ¯å¾çï¼ ```python from tsugu_api.v1 import
-search_song def main() -> None: result = search_song([3, 0], "EXIST") #
-è¿éä¹å¯ä»¥ä¼ å¥ "325" ï¼å·ä½åå³äºç¨æ·è¾å¥ä¿¡æ¯ main() ``` > `
-[3, 0]` æä»£ç¨æ·çé»è®¤æå¡å¨åè¡¨ï¼å¯ä»éè¿ `get_user_data()`
-æ¹æ³è·åçè¿åå¼ä¸­è·åã è·åå°ç `result` å°æ¯ä¸ä¸ª
-`_Response` å¯¹è±¡ï¼å½è·åå°åç¡®çä¿¡æ¯æ¶ï¼ `result` çå¼å¦ä¸ï¼
-```python [ { "type": "base64", "string": ... # å¾çç Base64 å­ç¬¦ä¸² } ]
-``` è¥ä¼ å¥çæ¥è¯¢åæ°ä¸åæ³ææ¥è¯¢è¿ç¨ä¸­åºéï¼è·åå°ç
-`result` çå¼å¦ä¸ï¼ ```python [ { "type": "string", "string": ... #
-éè¯¯ä¿¡æ¯ } ] ``` ç¶åæ¯ä½¿ç¨å¦ä¸ä»£ç ï¼éè¿ `v2`
-çæ¬è·åæå®å¡çä¿¡æ¯å¾çï¼ ```python from tsugu_api.v2 import card
-def main() -> None: result = card("1672", [3, 0]) #
-è¿éä¹å¯ä»¥ä¼ å¥å¶ä»å­ç¬¦ä¸²
-ï¼ç»æå°åä¸ºä¸ä¸ªç¬¦ååæ°çå¡çåè¡¨å¾ç main() ```
-è·åå°ç `result` å°æ¯ä¸ä¸ª `_Response`
-å¯¹è±¡ï¼å½è·åå°åç¡®çä¿¡æ¯æ¶ï¼ `result` çå¼å¦ä¸ï¼ ```python
-[ { "type": "base64", "string": ... # å¾çç Base64 å­ç¬¦ä¸² } ] ```
+``` ä½¿ç¨å¦ä¸ä»£ç ï¼è·åæå®æ­æ²ä¿¡æ¯å¾çï¼ ```python from
+tsugu_api import search_song def main() -> None: result = search_song([3, 0],
+"EXIST") # è¿éä¹å¯ä»¥ä¼ å¥ "325" ï¼å·ä½åå³äºç¨æ·è¾å¥ä¿¡æ¯
+main() ``` > `[3, 0]` æä»£ç¨æ·çé»è®¤æå¡å¨åè¡¨ï¼å¯ä»éè¿
+`get_user_data()` æ¹æ³è·åçè¿åå¼ä¸­è·åã è·åå°ç `result`
+å°æ¯ä¸ä¸ª `_Response` å¯¹è±¡ï¼å½è·åå°åç¡®çä¿¡æ¯æ¶ï¼ `result`
+çå¼å¦ä¸ï¼ ```python [ { "type": "base64", "string": ... # å¾çç
+Base64 å­ç¬¦ä¸² } ] ```
 è¥ä¼ å¥çæ¥è¯¢åæ°ä¸åæ³ææ¥è¯¢è¿ç¨ä¸­åºéï¼è·åå°ç
 `result` çå¼å¦ä¸ï¼ ```python [ { "type": "string", "string": ... #
 éè¯¯ä¿¡æ¯ } ] ``` > å¼æ­¥çæ¬çè°ç¨æ¹å¼ç¸åï¼åªæ¯å°
 `tsugu_api` æ¹ä¸º `tsugu_api_async` å³å¯ã Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown
```

### Comparing `tsugu-api-python-0.2.2/README.md` & `tsugu-api-python-1.0.0/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,170 +1,142 @@
-<div align="center">
-
-![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/blob/main/logo.png)
-
-# tsugu-api-python
-
-_✨ Python 编写的 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 相关各种功能 API 调用库  ✨_
-
-</div>
-
-<p align="center">
-
-<a href="https://github.com/Yamamoto-2/tsugu-bangdream-bot">
-  <img src="https://img.shields.io/badge/tsugu bangdream bot-v1 api-FFEE88" alt="license">
-</a>
-
-<a href="https://github.com/Yamamoto-2/tsugu-bangdream-bot">
-  <img src="https://img.shields.io/badge/tsugu bangdream bot-v2 api-FFEE88" alt="license">
-</a>
-
-<a href="https://github.com/WindowsSov8forUs/tsugu-api-python">
-  <img src="https://img.shields.io/github/v/release/WindowsSov8forUs/tsugu-api-python" alt="Latest Release Version">
-</a>
-
-<a href="https://github.com/WindowsSov8forUs/tsugu-api-python/blob/main/LICENSE">
-  <img src="https://img.shields.io/github/license/WindowsSov8forUs/tsugu-api-python" alt="License">
-</a>
-
-<a href="https://www.python.org/downloads/">
-  <img src="https://img.shields.io/pypi/pyversions/tsugu-api-python" alt="Python Version">
-</a>
-
-</p>
-
-## 说明
-
-这是一个用 Python 编写的调用 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 相关各种功能 API 的库，包括绝大部分 Tsugu 提供的功能。使用本 API 库提供的方法可以实现绝大部分功能，而搭配 [bestdori-api](https://github.com/WindowsSov8forUs/bestdori-api) 可以实现用户绑定等其他功能。
-
-> 该 API 库同时提供了异步与同步版本，可自行选择使用。
-
-> 一切数据获取等操作通过配置的后端服务器进行，该 API 库只提供前端所需的调用功能。若需要使用本地数据库，请自行操作。
-
-### 目前已有的功能
-
-> 所有方法都同时拥有异步与同步版本。
-
-#### Tsugu 后端功能
-
-> **`None`** 表示该功能没有相应的方法。
-
-|功能描述|v1 方法名称|v2 方法名称|
-|:------|:----------|:---------|
-|获取卡面图片|`get_card_illustration`|`card_illustration`|
-|获取玩家状态信息|`search_player`|`player`|
-|模拟指定卡池抽卡结果|`gacha_simulate`|`gacha_simulate`|
-|查询指定卡池信息|`search_gacha`|`gacha`|
-|查询符合条件的活动信息|`search_event`|`event`|
-|查询符合条件的歌曲信息|`search_song`|`song`|
-|查询歌曲分数表|`song_meta`|`song_meta`|
-|查询符合条件的角色信息|`search_character`|`character`|
-|查询指定歌曲指定难度的谱面|`song_chart`|`chart`|
-|查询指定活动的全部档位预测线|`ycx_all`|`ycx_all`|
-|查询指定活动的指定档位预测线|`ycx`|`ycx`|
-|查询指定活动指定档位相关的历史预测线|`lsycx`|`lsycx`|
-|获取指定车牌列表的图片形式|`room_list`|**`None`**|
-|查询符合条件的卡牌|`search_card`|`card`|
-|从后端获取最近的车牌信息列表|`station_query_all_room`|**`None`**|
-|提交车牌信息到后端|`station_submit_room_number`|**`None`**|
-|获取最近的车牌信息数据|**`None`**|`ycm`|
-
-> 部分功能类似的方法在 `v1` 和 `v2` 中调用方式并不相同。
-
-#### 用户数据后端功能 (仅 `v1` )
-
-|功能描述|v1 方法名称|
-|:------|:----------|
-获取用户数据|`get_user_data`|
-发送绑定用户请求|`bind_player_request`|
-验证绑定用户请求|`bind_player_verification`|
-设置是否转发指定用户的车牌|`set_car_forwarding`|
-设置指定用户的默认服务器列表|`set_default_server`|
-设置指定用户的主服务器模式|`set_server_mode`|
-
-> 以上功能都可使用本地用户数据库代替，本 API 不提供相关的配置方法。
-
-#### 车站功能 (仅 `v1` )
-
-|功能描述|v1 方法名称|
-|:------|:----------|
-|提交车牌信息到车站|`submit_room_number`|
-
-
-## 快速使用
-
-以下将以获取歌曲 **EXIST** (id=325) 和卡面 **羽沢 つぐみ - Precious birthday！** (id=1672) 的信息为例。
-
-使用以下指令安装本模块：
-```bash
-$ pip3 install tsugu-api-python
-```
-
-首先是使用如下代码，通过 `v1` 版本获取指定歌曲信息图片：
-
-```python
-from tsugu_api.v1 import search_song
-
-def main() -> None:
-    result = search_song([3, 0], "EXIST") # 这里也可以传入 "325" ，具体取决于用户输入信息
-
-main()
-```
-
-> `[3, 0]` 指代用户的默认服务器列表，可从通过 `get_user_data()` 方法获取的返回值中获取。
-
-获取到的 `result` 将是一个 `_Response` 对象，当获取到准确的信息时， `result` 的值如下：
-
-```python
-[
-    {
-        "type": "base64",
-        "string": ... # 图片的 Base64 字符串
-    }
-]
-```
-
-若传入的查询参数不合法或查询过程中出错，获取到的 `result` 的值如下：
-
-```python
-[
-    {
-        "type": "string",
-        "string": ... # 错误信息
-    }
-]
-```
-
-然后是使用如下代码，通过 `v2` 版本获取指定卡牌信息图片：
-
-```python
-from tsugu_api.v2 import card
-
-def main() -> None:
-    result = card("1672", [3, 0]) # 这里也可以传入其他字符串 ，结果将变为一个符合参数的卡牌列表图片
-
-main()
-```
-
-获取到的 `result` 将是一个 `_Response` 对象，当获取到准确的信息时， `result` 的值如下：
-
-```python
-[
-    {
-        "type": "base64",
-        "string": ... # 图片的 Base64 字符串
-    }
-]
-```
-
-若传入的查询参数不合法或查询过程中出错，获取到的 `result` 的值如下：
-
-```python
-[
-    {
-        "type": "string",
-        "string": ... # 错误信息
-    }
-]
-```
-
-> 异步版本的调用方式相同，只是将 `tsugu_api` 改为 `tsugu_api_async` 即可。
+Metadata-Version: 2.1
+Name: tsugu-api-python
+Version: 1.0.0
+Summary: Tsugu BanGDream Bot 的功能 API 统合包
+Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
+Author: WindowsSov8
+Author-email: qwertyuiop2333@hotmail.com
+License: MIT
+Description: <div align="center">
+        
+        ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/blob/main/logo.png)
+        
+        # tsugu-api-python
+        
+        _✨ Python 编写的 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 相关各种功能 API 调用库  ✨_
+        
+        </div>
+        
+        <p align="center">
+        
+        <a href="https://github.com/Yamamoto-2/tsugu-bangdream-bot">
+          <img src="https://img.shields.io/badge/tsugu bangdream bot-api-FFEE88" alt="license">
+        </a>
+        
+        <a href="https://github.com/WindowsSov8forUs/tsugu-api-python">
+          <img src="https://img.shields.io/github/v/release/WindowsSov8forUs/tsugu-api-python" alt="Latest Release Version">
+        </a>
+        
+        <a href="https://github.com/WindowsSov8forUs/tsugu-api-python/blob/main/LICENSE">
+          <img src="https://img.shields.io/github/license/WindowsSov8forUs/tsugu-api-python" alt="License">
+        </a>
+        
+        <a href="https://www.python.org/downloads/">
+          <img src="https://img.shields.io/pypi/pyversions/tsugu-api-python" alt="Python Version">
+        </a>
+        
+        </p>
+        
+        ## 说明
+        
+        这是一个用 Python 编写的调用 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 相关各种功能 API 的库，包括绝大部分 Tsugu 提供的功能。使用本 API 库提供的方法可以实现绝大部分功能，而搭配 [bestdori-api](https://github.com/WindowsSov8forUs/bestdori-api) 可以实现用户绑定等其他功能。
+        
+        > 该 API 库同时提供了异步与同步版本，可自行选择使用。
+        
+        > 一切数据获取等操作通过配置的后端服务器进行，该 API 库只提供前端所需的调用功能。若需要使用本地数据库，请自行操作。
+        
+        ### 目前已有的功能
+        
+        > 所有方法都同时拥有异步与同步版本。
+        
+        #### Tsugu 后端功能
+        
+        |功能描述|方法名称|
+        |:------|:----------|
+        |获取活动试炼舞台信息|`event_stage`|
+        |模拟指定卡池抽卡结果|`gacha_simulate`|
+        |获取卡面图片|`get_card_illustration`|
+        |查询指定活动指定档位相关的历史预测线|`lsycx`|
+        |获取指定车牌列表的图片形式|`room_list`|
+        |查询符合条件的卡牌|`search_card`|
+        |查询符合条件的角色信息|`search_character`|
+        |查询符合条件的活动信息|`search_event`|
+        |查询指定卡池信息|`search_gacha`|
+        |获取玩家状态信息|`search_player`|
+        |查询符合条件的歌曲信息|`search_song`|
+        |查询指定歌曲指定难度的谱面|`song_chart`|
+        |查询歌曲分数表|`song_meta`|
+        |查询指定活动的指定档位预测线|`ycx`|
+        |查询指定活动的全部档位预测线|`ycx_all`|
+        |提交车牌信息到后端|`station_submit_room_number`|
+        |从后端获取最近的车牌信息列表|`station_query_all_room`|
+        
+        #### 用户数据后端功能
+        
+        |功能描述|方法名称|
+        |:------|:----------|
+        |获取用户数据|`get_user_data`|
+        |修改用户数据|`change_user_data`|
+        |发送绑定用户请求|`bind_player_request`|
+        |验证绑定用户请求|`bind_player_verification`|
+        
+        > 以上功能都可使用本地用户数据库代替，本 API 不提供相关的配置方法。
+        
+        #### 车站功能
+        
+        |功能描述|方法名称|
+        |:------|:----------|
+        |提交车牌信息到车站|`submit_room_number`|
+        
+        
+        ## 快速使用
+        
+        以下将以获取歌曲 **EXIST** (id=325) 的信息为例。
+        
+        使用以下指令安装本模块：
+        ```bash
+        $ pip3 install tsugu-api-python
+        ```
+        
+        使用如下代码，获取指定歌曲信息图片：
+        
+        ```python
+        from tsugu_api import search_song
+        
+        def main() -> None:
+            result = search_song([3, 0], "EXIST") # 这里也可以传入 "325" ，具体取决于用户输入信息
+        
+        main()
+        ```
+        
+        > `[3, 0]` 指代用户的默认服务器列表，可从通过 `get_user_data()` 方法获取的返回值中获取。
+        
+        获取到的 `result` 将是一个 `_Response` 对象，当获取到准确的信息时， `result` 的值如下：
+        
+        ```python
+        [
+            {
+                "type": "base64",
+                "string": ... # 图片的 Base64 字符串
+            }
+        ]
+        ```
+        
+        若传入的查询参数不合法或查询过程中出错，获取到的 `result` 的值如下：
+        
+        ```python
+        [
+            {
+                "type": "string",
+                "string": ... # 错误信息
+            }
+        ]
+        ```
+        
+        > 异步版本的调用方式相同，只是将 `tsugu_api` 改为 `tsugu_api_async` 即可。
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,72 +1,62 @@
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.0.0 Summary: Tsugu
+BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
+WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
+qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
-      _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
+          _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
 ## è¯´æ è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [TsuguBanGDreamBot](https://
 github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file)
 ç¸å³åç§åè½ API çåºï¼åæ¬ç»å¤§é¨å Tsugu
 æä¾çåè½ãä½¿ç¨æ¬ API
 åºæä¾çæ¹æ³å¯ä»¥å®ç°ç»å¤§é¨ååè½ï¼èæ­é [bestdori-api]
 (https://github.com/WindowsSov8forUs/bestdori-api)
 å¯ä»¥å®ç°ç¨æ·ç»å®ç­å¶ä»åè½ã > è¯¥ API
 åºåæ¶æä¾äºå¼æ­¥ä¸åæ­¥çæ¬ï¼å¯èªè¡éæ©ä½¿ç¨ã >
 ä¸åæ°æ®è·åç­æä½éè¿éç½®çåç«¯æå¡å¨è¿è¡ï¼è¯¥ API
 åºåªæä¾åç«¯æéçè°ç¨åè½ãè¥éè¦ä½¿ç¨æ¬å°æ°æ®åºï¼è¯·èªè¡æä½ã
 ### ç®åå·²æçåè½ > æææ¹æ³é½åæ¶æ¥æå¼æ­¥ä¸åæ­¥çæ¬ã
-#### Tsugu åç«¯åè½ > **`None`** è¡¨ç¤ºè¯¥åè½æ²¡æç¸åºçæ¹æ³ã
-|åè½æè¿°|v1 æ¹æ³åç§°|v2 æ¹æ³åç§°| |:------|:----------|:---------
-| |è·åå¡é¢å¾ç|`get_card_illustration`|`card_illustration`|
-|è·åç©å®¶ç¶æä¿¡æ¯|`search_player`|`player`|
-|æ¨¡ææå®å¡æ± æ½å¡ç»æ|`gacha_simulate`|`gacha_simulate`|
-|æ¥è¯¢æå®å¡æ± ä¿¡æ¯|`search_gacha`|`gacha`|
-|æ¥è¯¢ç¬¦åæ¡ä»¶çæ´»å¨ä¿¡æ¯|`search_event`|`event`|
-|æ¥è¯¢ç¬¦åæ¡ä»¶çæ­æ²ä¿¡æ¯|`search_song`|`song`|
-|æ¥è¯¢æ­æ²åæ°è¡¨|`song_meta`|`song_meta`|
-|æ¥è¯¢ç¬¦åæ¡ä»¶çè§è²ä¿¡æ¯|`search_character`|`character`|
-|æ¥è¯¢æå®æ­æ²æå®é¾åº¦çè°±é¢|`song_chart`|`chart`|
-|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`|`ycx_all`|
-|æ¥è¯¢æå®æ´»å¨çæå®æ¡£ä½é¢æµçº¿|`ycx`|`ycx`|
-|æ¥è¯¢æå®æ´»å¨æå®æ¡£ä½ç¸å³çåå²é¢æµçº¿|`lsycx`|`lsycx`|
-|è·åæå®è½¦çåè¡¨çå¾çå½¢å¼|`room_list`|**`None`**|
-|æ¥è¯¢ç¬¦åæ¡ä»¶çå¡ç|`search_card`|`card`|
-|ä»åç«¯è·åæè¿çè½¦çä¿¡æ¯åè¡¨|`station_query_all_room`|**`None`**|
-|æäº¤è½¦çä¿¡æ¯å°åç«¯|`station_submit_room_number`|**`None`**|
-|è·åæè¿çè½¦çä¿¡æ¯æ°æ®|**`None`**|`ycm`| >
-é¨ååè½ç±»ä¼¼çæ¹æ³å¨ `v1` å `v2` ä¸­è°ç¨æ¹å¼å¹¶ä¸ç¸åã
-#### ç¨æ·æ°æ®åç«¯åè½ (ä» `v1` ) |åè½æè¿°|v1 æ¹æ³åç§°| |:----
---|:----------| è·åç¨æ·æ°æ®|`get_user_data`|
-åéç»å®ç¨æ·è¯·æ±|`bind_player_request`|
-éªè¯ç»å®ç¨æ·è¯·æ±|`bind_player_verification`|
-è®¾ç½®æ¯å¦è½¬åæå®ç¨æ·çè½¦ç|`set_car_forwarding`|
-è®¾ç½®æå®ç¨æ·çé»è®¤æå¡å¨åè¡¨|`set_default_server`|
-è®¾ç½®æå®ç¨æ·çä¸»æå¡å¨æ¨¡å¼|`set_server_mode`| >
+#### Tsugu åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+| |è·åæ´»å¨è¯ç¼èå°ä¿¡æ¯|`event_stage`|
+|æ¨¡ææå®å¡æ± æ½å¡ç»æ|`gacha_simulate`|
+|è·åå¡é¢å¾ç|`get_card_illustration`|
+|æ¥è¯¢æå®æ´»å¨æå®æ¡£ä½ç¸å³çåå²é¢æµçº¿|`lsycx`|
+|è·åæå®è½¦çåè¡¨çå¾çå½¢å¼|`room_list`|
+|æ¥è¯¢ç¬¦åæ¡ä»¶çå¡ç|`search_card`|
+|æ¥è¯¢ç¬¦åæ¡ä»¶çè§è²ä¿¡æ¯|`search_character`|
+|æ¥è¯¢ç¬¦åæ¡ä»¶çæ´»å¨ä¿¡æ¯|`search_event`|
+|æ¥è¯¢æå®å¡æ± ä¿¡æ¯|`search_gacha`|
+|è·åç©å®¶ç¶æä¿¡æ¯|`search_player`|
+|æ¥è¯¢ç¬¦åæ¡ä»¶çæ­æ²ä¿¡æ¯|`search_song`|
+|æ¥è¯¢æå®æ­æ²æå®é¾åº¦çè°±é¢|`song_chart`|
+|æ¥è¯¢æ­æ²åæ°è¡¨|`song_meta`|
+|æ¥è¯¢æå®æ´»å¨çæå®æ¡£ä½é¢æµçº¿|`ycx`|
+|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`|
+|æäº¤è½¦çä¿¡æ¯å°åç«¯|`station_submit_room_number`|
+|ä»åç«¯è·åæè¿çè½¦çä¿¡æ¯åè¡¨|`station_query_all_room`| ####
+ç¨æ·æ°æ®åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+| |è·åç¨æ·æ°æ®|`get_user_data`| |ä¿®æ¹ç¨æ·æ°æ®|`change_user_data`|
+|åéç»å®ç¨æ·è¯·æ±|`bind_player_request`|
+|éªè¯ç»å®ç¨æ·è¯·æ±|`bind_player_verification`| >
 ä»¥ä¸åè½é½å¯ä½¿ç¨æ¬å°ç¨æ·æ°æ®åºä»£æ¿ï¼æ¬ API
-ä¸æä¾ç¸å³çéç½®æ¹æ³ã #### è½¦ç«åè½ (ä» `v1` )
-|åè½æè¿°|v1 æ¹æ³åç§°| |:------|:----------
-| |æäº¤è½¦çä¿¡æ¯å°è½¦ç«|`submit_room_number`| ## å¿«éä½¿ç¨
-ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) åå¡é¢ **ç¾½æ²¢ ã¤ãã¿ -
-Precious birthdayï¼** (id=1672) çä¿¡æ¯ä¸ºä¾ã
+ä¸æä¾ç¸å³çéç½®æ¹æ³ã #### è½¦ç«åè½ |åè½æè¿°|æ¹æ³åç§°|
+|:------|:----------| |æäº¤è½¦çä¿¡æ¯å°è½¦ç«|`submit_room_number`| ##
+å¿«éä½¿ç¨ ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) çä¿¡æ¯ä¸ºä¾ã
 ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install tsugu-api-python
-``` é¦åæ¯ä½¿ç¨å¦ä¸ä»£ç ï¼éè¿ `v1`
-çæ¬è·åæå®æ­æ²ä¿¡æ¯å¾çï¼ ```python from tsugu_api.v1 import
-search_song def main() -> None: result = search_song([3, 0], "EXIST") #
-è¿éä¹å¯ä»¥ä¼ å¥ "325" ï¼å·ä½åå³äºç¨æ·è¾å¥ä¿¡æ¯ main() ``` > `
-[3, 0]` æä»£ç¨æ·çé»è®¤æå¡å¨åè¡¨ï¼å¯ä»éè¿ `get_user_data()`
-æ¹æ³è·åçè¿åå¼ä¸­è·åã è·åå°ç `result` å°æ¯ä¸ä¸ª
-`_Response` å¯¹è±¡ï¼å½è·åå°åç¡®çä¿¡æ¯æ¶ï¼ `result` çå¼å¦ä¸ï¼
-```python [ { "type": "base64", "string": ... # å¾çç Base64 å­ç¬¦ä¸² } ]
-``` è¥ä¼ å¥çæ¥è¯¢åæ°ä¸åæ³ææ¥è¯¢è¿ç¨ä¸­åºéï¼è·åå°ç
-`result` çå¼å¦ä¸ï¼ ```python [ { "type": "string", "string": ... #
-éè¯¯ä¿¡æ¯ } ] ``` ç¶åæ¯ä½¿ç¨å¦ä¸ä»£ç ï¼éè¿ `v2`
-çæ¬è·åæå®å¡çä¿¡æ¯å¾çï¼ ```python from tsugu_api.v2 import card
-def main() -> None: result = card("1672", [3, 0]) #
-è¿éä¹å¯ä»¥ä¼ å¥å¶ä»å­ç¬¦ä¸²
-ï¼ç»æå°åä¸ºä¸ä¸ªç¬¦ååæ°çå¡çåè¡¨å¾ç main() ```
-è·åå°ç `result` å°æ¯ä¸ä¸ª `_Response`
-å¯¹è±¡ï¼å½è·åå°åç¡®çä¿¡æ¯æ¶ï¼ `result` çå¼å¦ä¸ï¼ ```python
-[ { "type": "base64", "string": ... # å¾çç Base64 å­ç¬¦ä¸² } ] ```
+``` ä½¿ç¨å¦ä¸ä»£ç ï¼è·åæå®æ­æ²ä¿¡æ¯å¾çï¼ ```python from
+tsugu_api import search_song def main() -> None: result = search_song([3, 0],
+"EXIST") # è¿éä¹å¯ä»¥ä¼ å¥ "325" ï¼å·ä½åå³äºç¨æ·è¾å¥ä¿¡æ¯
+main() ``` > `[3, 0]` æä»£ç¨æ·çé»è®¤æå¡å¨åè¡¨ï¼å¯ä»éè¿
+`get_user_data()` æ¹æ³è·åçè¿åå¼ä¸­è·åã è·åå°ç `result`
+å°æ¯ä¸ä¸ª `_Response` å¯¹è±¡ï¼å½è·åå°åç¡®çä¿¡æ¯æ¶ï¼ `result`
+çå¼å¦ä¸ï¼ ```python [ { "type": "base64", "string": ... # å¾çç
+Base64 å­ç¬¦ä¸² } ] ```
 è¥ä¼ å¥çæ¥è¯¢åæ°ä¸åæ³ææ¥è¯¢è¿ç¨ä¸­åºéï¼è·åå°ç
 `result` çå¼å¦ä¸ï¼ ```python [ { "type": "string", "string": ... #
 éè¯¯ä¿¡æ¯ } ] ``` > å¼æ­¥çæ¬çè°ç¨æ¹å¼ç¸åï¼åªæ¯å°
-`tsugu_api` æ¹ä¸º `tsugu_api_async` å³å¯ã
+`tsugu_api` æ¹ä¸º `tsugu_api_async` å³å¯ã Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Requires-Python:
+>=3.8 Description-Content-Type: text/markdown
```

### Comparing `tsugu-api-python-0.2.2/setup.py` & `tsugu-api-python-1.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='0.2.2',
+    version='1.0.0',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-0.2.2/tsugu_api/_network.py` & `tsugu-api-python-1.0.0/tsugu_api/_network.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,106 @@
 '''`tsugu_api._network`
 
 向 Tsugu 后端发送请求相关模块'''
 from json import dumps
 from typing import Any, Literal, Optional, cast
 
-from httpx import Response, Request, Client
+from httpx import Client, Request, Response, HTTPStatusError
 
 from . import settings
 
 # 向后端发送 API 请求类
 class Api:
     '''向后端发送 API 请求类
 
     参数:
         url (str): 请求的 URL 地址
     '''
     url: str
     '''请求的 API 地址'''
     proxy: bool
     '''是否使用代理服务器'''
-    params: Optional[dict[str, Any]]
-    '''请求的参数'''
-    data: Optional[dict[str, Any]]
-    '''请求的数据'''
     # 初始化
     def __init__(
         self,
         url: str,
-        proxy: bool,
-        *,
-        params: Optional[dict[str, Any]]=None,
-        data: Optional[dict[str, Any]]=None
+        proxy: bool
     ) -> None:
         '''初始化'''
         self.url = url
         self.proxy = proxy
-        self.params = params
-        self.data = data
         return
     
     # 请求发送
     def _request(
         self,
         method: Literal['get', 'post'],
+        *,
+        params: Optional[dict[str, Any]]=None,
+        data: Optional[dict[str, Any]]=None
     ) -> Response:
         '''请求发送
 
         参数:
             method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
+            params (Optional[dict[str, Any]]): 请求的参数
+            data (Optional[dict[str, Any]]): 请求的数据
 
         返回:
             Response: 收到的响应
         '''
         # 构建请求头
         if method == 'post':
             headers = {'Content-Type': 'application/json'}
         else:
             headers = None
         
         # 构建一个请求体
         request = Request(
             method,
             self.url,
-            params=self.params,
-            data=cast(dict, dumps(self.data)) if self.data is not None else self.data,
+            params=params,
+            data=cast(dict, dumps(data)) if data is not None else data,
             headers=headers
         )
+        print(data)
         # 构建代理服务器字典
         if self.proxy:
             proxies = settings._get_proxy()
         else:
             proxies = None
         
         # 发送请求并获取响应
         with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
             response = client.send(request)
         
         # 处理接收到的响应
-        response.raise_for_status()
+        try:
+            response.raise_for_status()
+        except HTTPStatusError as exception:
+            if exception.response.status_code == 400:
+                return response
+            else:
+                raise exception
         return response
     
-    def post(self) -> Response:
+    def post(self, data: Optional[dict[str, Any]]=None) -> Response:
         '''发送 POST 请求
 
+        参数:
+            data (Optional[dict[str, Any]]): 请求的数据
+
         返回:
             Response: 收到的响应
         '''
-        return self._request('post')
+        return self._request('post', data=data)
     
-    def get(self) -> Response:
+    def get(self, params: Optional[dict[str, Any]]=None) -> Response:
         '''发送 GET 请求
 
+        参数:
+            params (Optional[dict[str, Any]]): 请求的参数
+
         返回:
             Response: 收到的响应
         '''
-        return self._request('get')
+        return self._request('get', params=params)
```

### Comparing `tsugu-api-python-0.2.2/tsugu_api/settings.py` & `tsugu-api-python-1.0.0/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.2/tsugu_api/utils.py` & `tsugu-api-python-1.0.0/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.2/tsugu_api/v1/_bandoristation.py` & `tsugu-api-python-1.0.0/tsugu_api/_bandoristation.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,12 +24,11 @@
         'source': source,
         'token': token
     }
     
     # 发送请求
     response = Api(
         BANDORI_STATION_URL,
-        proxy=settings.backend_proxy,
-        params=params
-    ).get().json()
+        proxy=settings.backend_proxy
+    ).get(params).json()
     if response['status'] == 'failure':
         raise RoomSubmitFailure(response['response'])
```

### Comparing `tsugu-api-python-0.2.2/tsugu_api/v1/_tsugu.py` & `tsugu-api-python-1.0.0/tsugu_api/_tsugu.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-from time import time
 from typing import Optional
 
 from tsugu_api import settings
 from tsugu_api._network import Api
 from tsugu_api._typing import (
+    _Room,
     _Server,
-    _CarData,
     _Response,
-    _Difficulty,
-    _QueryResult,
-    _SubmitResult
+    _DifficultyText
 )
 
-def get_card_illustration(card_id: int) -> _Response:
-    '''获取卡面
+def event_stage(server: _Server, event_id: Optional[int] = None, meta: bool = False) -> _Response:
+    '''查询团队 LIVE 佳节活动舞台数据
 
     参数:
-        card_id (int): 卡片 ID
+        server (_Server): 服务器
+        event_id (int): 活动 ID
+        meta (bool): 是否携带歌曲分数表
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/getCardIllustration'
+    url = settings.backend_url + '/eventStage'
     
     # 构建数据
     data = {
-        'cardId': card_id
+        'server': server,
+        'meta': meta,
+        'compress': settings.compress
     }
+    if event_id:
+        data['eventId'] = event_id
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
 def gacha_simulate(server_mode: _Server, times: Optional[int] = None, gacha_id: Optional[int] = None) -> _Response:
     '''模拟抽卡
 
     参数:
         server_mode (_Server): 服务器模式
         times (int): 抽卡次数
@@ -61,445 +63,368 @@
         data['times'] = times
     if gacha_id:
         data['gachaId'] = gacha_id
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
-
-def search_player(player_id: int, server: _Server) -> _Response:
-    '''查询玩家状态
-
-    参数:
-        player_id (int): 玩家 ID
-        server (_Server): 服务器
-
-    返回:
-        _Response: 响应信息
-    '''
-    
-    # 构建 URL
-    url = settings.backend_url + '/searchPlayer'
-    
-    # 构建数据
-    data = {
-        'playerId': player_id,
-        'server': server,
-        'useEasyBG': settings.use_easy_bg,
-        'compress': settings.compress
-    }
-    
-    # 发送请求
-    return Api(
-        url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def search_gacha(default_servers: list[_Server], gacha_id: int) -> _Response:
-    '''查询卡池
+def get_card_illustration(card_id: int) -> _Response:
+    '''获取卡面
 
     参数:
-        default_servers (list[_Server]): 默认服务器
-        gacha_id (int): 卡池 ID
+        card_id (int): 卡片 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchGacha'
+    url = settings.backend_url + '/getCardIllustration'
     
     # 构建数据
     data = {
-        'default_servers': default_servers,
-        'gachaId': gacha_id,
-        'useEasyBG': settings.use_easy_bg,
-        'compress': settings.compress
+        'cardId': str(card_id)
     }
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def search_event(default_servers: list[_Server], text: str) -> _Response:
-    '''查询活动
+def lsycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
+    '''查询历史排行榜预测线
 
     参数:
-        default_servers (list[_Server]): 默认服务器
-        text (str): 查询参数
+        server (_Server): 服务器
+        tier (int): 排行榜挡位
+        event_id (int): 活动 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchEvent'
+    url = settings.backend_url + '/lsycx'
     
     # 构建数据
     data = {
-        'default_servers': default_servers,
-        'text': text,
-        'useEasyBG': settings.use_easy_bg,
+        'server': server,
+        'tier': tier,
         'compress': settings.compress
     }
+    if event_id:
+        data['eventId'] = event_id
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def event_stage(server: _Server, meta: bool = False, event_id: Optional[int] = None) -> _Response:
-    '''查询团队 LIVE 佳节活动舞台数据
+def room_list(room_list: list[_Room]) -> _Response:
+    '''绘制车牌绘图
 
     参数:
-        server (_Server): 服务器
-        meta (bool): 是否携带歌曲分数表
-        event_id (int): 活动 ID
+        room_list (list[_CarData]): 车牌信息列表
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/eventStage'
+    url = settings.backend_url + '/roomList'
     
     # 构建数据
     data = {
-        'server': server,
-        'meta': meta,
+        'roomList': room_list,
         'compress': settings.compress
     }
-    if event_id:
-        data['eventId'] = event_id
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def search_song(default_servers: list[_Server], text: str) -> _Response:
-    '''查询歌曲
+def search_card(default_servers: list[_Server], text: str) -> _Response:
+    '''查询卡片
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchSong'
+    url = settings.backend_url + '/searchCard'
     
     # 构建数据
     data = {
         'default_servers': default_servers,
         'text': text,
         'useEasyBG': settings.use_easy_bg,
         'compress': settings.compress
     }
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def song_meta(default_servers: list[_Server], server: _Server) -> _Response:
-    '''查询歌曲分数表
+def search_character(default_servers: list[_Server], text: str) -> _Response:
+    '''查询角色
 
     参数:
         default_servers (list[_Server]): 默认服务器
-        server (_Server): 主服务器
+        text (str): 查询参数
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/songMeta'
+    url = settings.backend_url + '/searchCharacter'
     
     # 构建数据
     data = {
         'default_servers': default_servers,
-        'server': server,
+        'text': text,
         'compress': settings.compress
     }
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def search_character(default_servers: list[_Server], text: str) -> _Response:
-    '''查询角色
+def search_event(default_servers: list[_Server], text: str) -> _Response:
+    '''查询活动
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchCharacter'
+    url = settings.backend_url + '/searchEvent'
     
     # 构建数据
     data = {
         'default_servers': default_servers,
         'text': text,
+        'useEasyBG': settings.use_easy_bg,
         'compress': settings.compress
     }
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def song_chart(default_servers: list[_Server], song_id: int, difficulty_text: _Difficulty) -> _Response:
-    '''查询歌曲谱面
+def search_gacha(default_servers: list[_Server], gacha_id: int) -> _Response:
+    '''查询卡池
 
     参数:
         default_servers (list[_Server]): 默认服务器
-        song_id (int): 歌曲 ID
-        difficulty_text (_Difficulty): 谱面难度
+        gacha_id (int): 卡池 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/songChart'
+    url = settings.backend_url + '/searchGacha'
     
     # 构建数据
     data = {
         'default_servers': default_servers,
-        'songId': song_id,
-        'difficultyText': difficulty_text,
+        'gachaId': gacha_id,
+        'useEasyBG': settings.use_easy_bg,
         'compress': settings.compress
     }
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def ycx_all(server: _Server, event_id: Optional[int] = None) -> _Response:
-    '''查询全挡位预测线
+def search_player(player_id: int, server: _Server) -> _Response:
+    '''查询玩家状态
 
     参数:
+        player_id (int): 玩家 ID
         server (_Server): 服务器
-        event_id (int): 活动 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/ycxAll'
+    url = settings.backend_url + '/searchPlayer'
     
     # 构建数据
     data = {
+        'playerId': player_id,
         'server': server,
+        'useEasyBG': settings.use_easy_bg,
         'compress': settings.compress
     }
-    if event_id:
-        data['eventId'] = event_id
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def ycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
-    '''查询排行榜预测线
+def search_song(default_servers: list[_Server], text: str) -> _Response:
+    '''查询歌曲
 
     参数:
-        server (_Server): 服务器
-        tier (int): 排行榜挡位
-        event_id (int): 活动 ID
+        default_servers (list[_Server]): 默认服务器
+        text (str): 查询参数
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/ycx'
+    url = settings.backend_url + '/searchSong'
     
     # 构建数据
     data = {
-        'server': server,
-        'tier': tier,
+        'default_servers': default_servers,
+        'text': text,
         'compress': settings.compress
     }
-    if event_id:
-        data['eventId'] = event_id
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def lsycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
-    '''查询历史排行榜预测线
+def song_chart(default_servers: list[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
+    '''查询歌曲谱面
 
     参数:
-        server (_Server): 服务器
-        tier (int): 排行榜挡位
-        event_id (int): 活动 ID
+        default_servers (list[_Server]): 默认服务器
+        song_id (int): 歌曲 ID
+        difficulty_text (_Difficulty): 谱面难度
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/lsycx'
+    url = settings.backend_url + '/songChart'
     
     # 构建数据
     data = {
-        'server': server,
-        'tier': tier,
+        'default_servers': default_servers,
+        'songId': song_id,
+        'difficultyText': difficulty_text,
         'compress': settings.compress
     }
-    if event_id:
-        data['eventId'] = event_id
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def room_list(room_list: list[_CarData]) -> _Response:
-    '''绘制车牌绘图
+def song_meta(default_servers: list[_Server], server: _Server) -> _Response:
+    '''查询歌曲分数表
 
     参数:
-        room_list (list[_CarData]): 车牌信息列表
+        default_servers (list[_Server]): 默认服务器
+        server (_Server): 主服务器
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/roomList'
+    url = settings.backend_url + '/songMeta'
     
     # 构建数据
     data = {
-        'roomList': room_list,
+        'default_servers': default_servers,
+        'server': server,
         'compress': settings.compress
     }
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
 
-def search_card(default_servers: list[_Server], text: str) -> _Response:
-    '''查询卡片
+def ycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
+    '''查询排行榜预测线
 
     参数:
-        default_servers (list[_Server]): 默认服务器
-        text (str): 查询参数
+        server (_Server): 服务器
+        tier (int): 排行榜挡位
+        event_id (int): 活动 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchCard'
+    url = settings.backend_url + '/ycx'
     
     # 构建数据
     data = {
-        'default_servers': default_servers,
-        'text': text,
-        'useEasyBG': settings.use_easy_bg,
+        'server': server,
+        'tier': tier,
         'compress': settings.compress
     }
-    
-    # 发送请求
-    return Api(
-        url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
-
-def station_query_all_room() -> _QueryResult:
-    '''查询最近车站车牌
-
-    返回:
-        _QueryResult: 响应信息
-    '''
-    
-    # 构建 URL
-    url = settings.backend_url + '/station/queryAllRoom'
+    if event_id:
+        data['eventId'] = event_id
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
-    ).get().json()
+    ).post(data).json()
 
-def station_submit_room_number(
-    number: int,
-    raw_message: str,
-    platform: str,
-    user_id: str,
-    user_name: str
-) -> _SubmitResult:
-    '''提交车牌号
+def ycx_all(server: _Server, event_id: Optional[int] = None) -> _Response:
+    '''查询全挡位预测线
 
     参数:
-        number (int): 车牌号
-        raw_message (str): 原始消息
-        platform (str): 平台
-        user_id (str): 用户 ID
-        user_name (str): 用户名
+        server (_Server): 服务器
+        event_id (int): 活动 ID
 
     返回:
-        _SubmitResult: 响应信息
+        _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/station/submitRoomNumber'
+    url = settings.backend_url + '/ycxAll'
     
     # 构建数据
     data = {
-        'number': number,
-        'raw_message': raw_message,
-        'platform': platform,
-        'user_id': user_id,
-        'user_name': user_name,
-        'time': int(time())
+        'server': server,
+        'compress': settings.compress
     }
+    if event_id:
+        data['eventId'] = event_id
     
     # 发送请求
     return Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post().json()
+        proxy=settings.backend_proxy
+    ).post(data).json()
```

### Comparing `tsugu-api-python-0.2.2/tsugu_api_async/_network.py` & `tsugu-api-python-1.0.0/tsugu_api_async/_network.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''`tsugu_api_async._network`
 
 向 Tsugu 后端发送请求相关模块'''
 from json import dumps
 from typing import Any, Literal, Optional, cast
 
 from aiohttp import ClientSession
-from httpx import Request, AsyncClient
+from httpx import Request, Response, AsyncClient, HTTPStatusError
 
 from . import settings
 from ._typing import _ApiResponse
 
 # 向后端发送 API 请求类
 class Api:
     '''向后端发送 API 请求类
@@ -17,43 +17,39 @@
     参数:
         url (str): 请求的 URL 地址
     '''
     url: str
     '''请求的 API 地址'''
     proxy: bool
     '''是否使用代理服务器'''
-    params: Optional[dict[str, Any]]
-    '''请求的参数'''
-    data: Optional[dict[str, Any]]
-    '''请求的数据'''
     # 初始化
     def __init__(
         self,
         url: str,
-        proxy: bool,
-        *,
-        params: Optional[dict[str, Any]]=None,
-        data: Optional[dict[str, Any]]=None
+        proxy: bool
     ) -> None:
         '''初始化'''
         self.url = url
         self.proxy = proxy
-        self.params = params
-        self.data = data
         return
     
     # 请求发送
     async def _request(
         self,
         method: Literal['get', 'post'],
+        *,
+        params: Optional[dict[str, Any]]=None,
+        data: Optional[dict[str, Any]]=None
     ) -> _ApiResponse:
         '''请求发送
 
         参数:
             method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
+            params (Optional[dict[str, Any]]): 请求的参数
+            data (Optional[dict[str, Any]]): 请求的数据
 
         返回:
             Response: 收到的响应
         '''
         # 构建请求头
         if method == 'post':
             headers = {'Content-Type': 'application/json'}
@@ -69,43 +65,61 @@
         # 发送请求并获取响应
         if settings.client == settings.Client.HTTPX:
             async with AsyncClient(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
                 # 构建一个请求体
                 request = Request(
                     method,
                     self.url,
-                    params=self.params,
-                    data=cast(dict, dumps(self.data)) if self.data is not None else self.data,
+                    params=params,
+                    data=cast(dict, dumps(data)) if data is not None else data,
                     headers=headers
                 )
                 
                 response = await client.send(request)
         else:
             async with ClientSession() as session:
                 response = await session.request(
                     method,
                     self.url,
-                    params=self.params,
-                    data=cast(dict, dumps(self.data)) if self.data is not None else self.data,
+                    params=params,
+                    data=cast(dict, dumps(data)) if data is not None else data,
                     headers=headers,
-                    proxy=settings.proxy if len(settings.proxy) > 0 else None,
+                    proxy=settings.proxy if len(settings.proxy) > 0 and self.proxy else None,
                 )
         
         # 处理接收到的响应
-        response.raise_for_status()
+        if isinstance(response, Response):
+            try:
+                response.raise_for_status()
+            except HTTPStatusError as exception:
+                if exception.response.status_code == 400:
+                    return response
+                else:
+                    raise exception
+        else:
+            if response.status == 400:
+                return response
+            else:
+                response.raise_for_status()
         return response
     
-    async def post(self) -> _ApiResponse:
+    async def post(self, data: Optional[dict[str, Any]]=None) -> _ApiResponse:
         '''发送 POST 请求
 
+        参数:
+            data (Optional[dict[str, Any]]): 请求的数据
+
         返回:
             _ApiResponse: 收到的响应
         '''
-        return await self._request('post')
+        return await self._request('post', data=data)
     
-    async def get(self) -> _ApiResponse:
+    async def get(self, params: Optional[dict[str, Any]]=None) -> _ApiResponse:
         '''发送 GET 请求
 
+        参数:
+            params (Optional[dict[str, Any]]): 请求的参数
+
         返回:
             _ApiResponse: 收到的响应
         '''
-        return await self._request('get')
+        return await self._request('get', params=params)
```

### Comparing `tsugu-api-python-0.2.2/tsugu_api_async/_typing.py` & `tsugu-api-python-1.0.0/tsugu_api_async/_typing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-`tsugu_api_async._typing`
+`tsugu_api._typing`
 
 定义了一些类型别名
 '''
 
 from typing import (
     Union,
     Literal,
@@ -13,85 +13,117 @@
 )
 
 from httpx import Response
 from aiohttp import ClientResponse
 
 _ApiResponse: TypeAlias = Union[Response, ClientResponse]
 
-_Server: TypeAlias = Literal[0, 1, 2, 3, 4]
+_ServerId: TypeAlias = Literal[0, 1, 2, 3, 4]
 '''
 服务器 ID
 
 值:
     0: 日服
     1: 国际服
     2: 台服
     3: 国服
     4: 韩服
 '''
+_ServerName: TypeAlias = Literal['jp', 'en', 'tw', 'cn', 'kr']
+'''
+服务器名
+
+值:
+    'jp': 日服
+    'en': 国际服
+    'tw': 台服
+    'cn': 国服
+    'kr': 韩服
+'''
+_Server: TypeAlias = Union[_ServerId, _ServerName]
+'''服务器'''
 
 class _Data(TypedDict):
     '''API 单个响应数据'''
     type: Literal['string', 'base64']
     string: str
 
 _Response: TypeAlias = list[_Data]
 
-class _CarData(TypedDict):
-    '''车牌数据'''
-    number: int
-    rawMessage: str
-    source: str
-    userId: int
-    time: int
-    avanter: str
-    userName: str
+_DifficultyText: TypeAlias = Literal['easy', 'normal', 'hard', 'expert', 'special']
+'''难度名'''
+
+class _Player(TypedDict):
+    id: int
+    server: _Server
 
 _Status: TypeAlias = Literal['success', 'failure']
 '''响应状态'''
 
-class _Result(TypedDict):
-    '''响应结果'''
+class _SubmitResponse(TypedDict):
+    '''`/station/submitRoomNumber` 响应结果'''
     status: _Status
     data: str
 
-class _QueryResult(TypedDict):
-    '''`/station/queryAllRoom` 响应结果'''
-    status: _Status
-    data: Union[str, list[_CarData]]
+class _Room(TypedDict):
+    '''房间数据'''
+    number: int
+    rawMessage: str
+    source: str
+    userId: str
+    time: int
+    player: _Player
+    avanter: NotRequired[str]
+    userName: NotRequired[str]
 
-class _SubmitResult(TypedDict):
-    '''`submit_room_number` 响应结果'''
+class _QueryResponse(TypedDict):
+    '''`/station/queryAllRoom` 响应结果'''
     status: _Status
-    data: Union[str, list[_CarData]]
+    data: Union[str, list[_Room]]
 
-class _ServerData(TypedDict):
+class _TsuguUserServer(TypedDict):
     '''服务器数据'''
     playerId: int
-    bindingStatus: int
+    bindingStatus: Literal[0, 1, 2]
+    verifyCode: NotRequired[int]
 
-class _UserData(TypedDict):
+class _TsuguUser(TypedDict):
     '''用户数据'''
-    _id: NotRequired[str]
     user_id: str
     platform: str
     server_mode: _Server
     default_server: list[_Server]
     car: bool
-    server_list: list[_ServerData]
+    server_list: list[_TsuguUserServer]
 
-class _UserDataResult(TypedDict):
-    '''`get_user_data` 响应结果'''
+class _UserDataResponse(TypedDict):
+    '''`/user/getUserData` 响应结果'''
     status: _Status
-    data: Union[str, _UserData]
+    data: Union[str, _TsuguUser]
+
+class _Update(TypedDict):
+    '''更新数据'''
+    user_id: NotRequired[str]
+    platform: NotRequired[str]
+    server_mode: NotRequired[_ServerId]
+    default_server: NotRequired[list[_ServerId]]
+    car: NotRequired[bool]
+    server_list: NotRequired[list[_TsuguUserServer]]
+
+class _UpdateResponse(TypedDict):
+    '''`/user/changeUserData` 响应结果'''
+    status: _Status
+    data: NotRequired[str]
 
 class _VerifyCode(TypedDict):
     '''验证码'''
     verifyCode: int
 
 class _BindResponse(TypedDict):
-    '''绑定响应'''
+    '''`/user/bindPlayerRequest` 绑定响应'''
     status: _Status
     data: Union[str, _VerifyCode]
 
-_Difficulty: TypeAlias = Literal['easy', 'normal', 'hard', 'expert', 'special']
-'''难度名'''
+class _VerificationResponse(TypedDict):
+    '''`/user/bindPlayerVerification` 响应结果'''
+    status: _Status
+    data: str
```

### Comparing `tsugu-api-python-0.2.2/tsugu_api_async/settings.py` & `tsugu-api-python-1.0.0/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.2/tsugu_api_async/utils.py` & `tsugu-api-python-1.0.0/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.2.2/tsugu_api_async/v1/_bandoristation.py` & `tsugu-api-python-1.0.0/tsugu_api_async/_bandoristation.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,13 @@
         'source': source,
         'token': token
     }
     
     # 发送请求
     response = await Api(
             BANDORI_STATION_URL,
-            proxy=settings.backend_proxy,
-            params=params
-    ).get()
+            proxy=settings.backend_proxy
+    ).get(params)
     if isinstance(response, Response): response = response.json()
     else: response = await response.json()
     if response['status'] == 'failure':
         raise RoomSubmitFailure(response['response'])
```

### Comparing `tsugu-api-python-0.2.2/tsugu_api_async/v1/_tsugu.py` & `tsugu-api-python-1.0.0/tsugu_api_async/_tsugu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-from time import time
 from typing import Optional
 
 from httpx import Response
 
 from tsugu_api_async import settings
 from tsugu_api_async._network import Api
 from tsugu_api_async._typing import (
+    _Room,
     _Server,
-    _CarData,
     _Response,
-    _Difficulty,
-    _QueryResult,
-    _SubmitResult
+    _DifficultyText
 )
 
-async def get_card_illustration(card_id: int) -> _Response:
-    '''获取卡面
+async def event_stage(server: _Server, event_id: Optional[int] = None, meta: bool = False) -> _Response:
+    '''查询团队 LIVE 佳节活动舞台数据
 
     参数:
-        platform (str): 平台名称
-        user_id (str): 用户 ID
+        server (_Server): 服务器
+        event_id (int): 活动 ID
+        meta (bool): 是否携带歌曲分数表
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/getCardIllustration'
+    url = settings.backend_url + '/eventStage'
     
     # 构建数据
     data = {
-        'cardId': card_id
+        'server': server,
+        'meta': meta,
+        'compress': settings.compress
     }
+    if event_id:
+        data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def gacha_simulate(server_mode: _Server, times: Optional[int] = None, gacha_id: Optional[int] = None) -> _Response:
     '''模拟抽卡
 
     参数:
@@ -66,477 +67,396 @@
         data['times'] = times
     if gacha_id:
         data['gachaId'] = gacha_id
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
-    if isinstance(response, Response): return response.json()
-    return await response.json()
-
-async def search_player(player_id: int, server: _Server) -> _Response:
-    '''查询玩家状态
-
-    参数:
-        player_id (int): 玩家 ID
-        server (_Server): 服务器
-
-    返回:
-        _Response: 响应信息
-    '''
-    
-    # 构建 URL
-    url = settings.backend_url + '/searchPlayer'
-    
-    # 构建数据
-    data = {
-        'playerId': player_id,
-        'server': server,
-        'useEasyBG': settings.use_easy_bg,
-        'compress': settings.compress
-    }
-    
-    # 发送请求
-    response = await Api(
-        url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_gacha(default_servers: list[_Server], gacha_id: int) -> _Response:
-    '''查询卡池
+async def get_card_illustration(card_id: int) -> _Response:
+    '''获取卡面
 
     参数:
-        default_servers (list[_Server]): 默认服务器
-        gacha_id (int): 卡池 ID
+        card_id (int): 卡片 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchGacha'
+    url = settings.backend_url + '/getCardIllustration'
     
     # 构建数据
     data = {
-        'default_servers': default_servers,
-        'gachaId': gacha_id,
-        'useEasyBG': settings.use_easy_bg,
-        'compress': settings.compress
+        'cardId': str(card_id)
     }
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_event(default_servers: list[_Server], text: str) -> _Response:
-    '''查询活动
+async def lsycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
+    '''查询历史排行榜预测线
 
     参数:
-        default_servers (list[_Server]): 默认服务器
-        text (str): 查询参数
+        server (_Server): 服务器
+        tier (int): 排行榜挡位
+        event_id (int): 活动 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchEvent'
+    url = settings.backend_url + '/lsycx'
     
     # 构建数据
     data = {
-        'default_servers': default_servers,
-        'text': text,
-        'useEasyBG': settings.use_easy_bg,
+        'server': server,
+        'tier': tier,
         'compress': settings.compress
     }
+    if event_id:
+        data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def event_stage(server: _Server, meta: bool = False, event_id: Optional[int] = None) -> _Response:
-    '''查询团队 LIVE 佳节活动舞台数据
+async def room_list(room_list: list[_Room]) -> _Response:
+    '''绘制车牌绘图
 
     参数:
-        server (_Server): 服务器
-        meta (bool): 是否携带歌曲分数表
-        event_id (int): 活动 ID
+        room_list (list[_CarData]): 车牌信息列表
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/eventStage'
+    url = settings.backend_url + '/roomList'
     
     # 构建数据
     data = {
-        'server': server,
-        'meta': meta,
+        'roomList': room_list,
         'compress': settings.compress
     }
-    if event_id:
-        data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_song(default_servers: list[_Server], text: str) -> _Response:
-    '''查询歌曲
+async def search_card(default_servers: list[_Server], text: str) -> _Response:
+    '''查询卡片
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchSong'
+    url = settings.backend_url + '/searchCard'
     
     # 构建数据
     data = {
         'default_servers': default_servers,
         'text': text,
         'useEasyBG': settings.use_easy_bg,
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def song_meta(default_servers: list[_Server], server: _Server) -> _Response:
-    '''查询歌曲分数表
+async def search_character(default_servers: list[_Server], text: str) -> _Response:
+    '''查询角色
 
     参数:
         default_servers (list[_Server]): 默认服务器
-        server (_Server): 主服务器
+        text (str): 查询参数
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/songMeta'
+    url = settings.backend_url + '/searchCharacter'
     
     # 构建数据
     data = {
         'default_servers': default_servers,
-        'server': server,
+        'text': text,
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_character(default_servers: list[_Server], text: str) -> _Response:
-    '''查询角色
+async def search_event(default_servers: list[_Server], text: str) -> _Response:
+    '''查询活动
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchCharacter'
+    url = settings.backend_url + '/searchEvent'
     
     # 构建数据
     data = {
         'default_servers': default_servers,
         'text': text,
+        'useEasyBG': settings.use_easy_bg,
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def song_chart(default_servers: list[_Server], song_id: int, difficulty_text: _Difficulty) -> _Response:
-    '''查询歌曲谱面
+async def search_gacha(default_servers: list[_Server], gacha_id: int) -> _Response:
+    '''查询卡池
 
     参数:
         default_servers (list[_Server]): 默认服务器
-        song_id (int): 歌曲 ID
-        difficulty_text (_Difficulty): 谱面难度
+        gacha_id (int): 卡池 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/songChart'
+    url = settings.backend_url + '/searchGacha'
     
     # 构建数据
     data = {
         'default_servers': default_servers,
-        'songId': song_id,
-        'difficultyText': difficulty_text,
+        'gachaId': gacha_id,
+        'useEasyBG': settings.use_easy_bg,
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def ycx_all(server: _Server, event_id: Optional[int] = None) -> _Response:
-    '''查询全挡位预测线
+async def search_player(player_id: int, server: _Server) -> _Response:
+    '''查询玩家状态
 
     参数:
+        player_id (int): 玩家 ID
         server (_Server): 服务器
-        event_id (int): 活动 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/ycxAll'
+    url = settings.backend_url + '/searchPlayer'
     
     # 构建数据
     data = {
+        'playerId': player_id,
         'server': server,
+        'useEasyBG': settings.use_easy_bg,
         'compress': settings.compress
     }
-    if event_id:
-        data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def ycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
-    '''查询排行榜预测线
+async def search_song(default_servers: list[_Server], text: str) -> _Response:
+    '''查询歌曲
 
     参数:
-        server (_Server): 服务器
-        tier (int): 排行榜挡位
-        event_id (int): 活动 ID
+        default_servers (list[_Server]): 默认服务器
+        text (str): 查询参数
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/ycx'
+    url = settings.backend_url + '/searchSong'
     
     # 构建数据
     data = {
-        'server': server,
-        'tier': tier,
+        'default_servers': default_servers,
+        'text': text,
         'compress': settings.compress
     }
-    if event_id:
-        data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def lsycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
-    '''查询历史排行榜预测线
+async def song_chart(default_servers: list[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
+    '''查询歌曲谱面
 
     参数:
-        server (_Server): 服务器
-        tier (int): 排行榜挡位
-        event_id (int): 活动 ID
+        default_servers (list[_Server]): 默认服务器
+        song_id (int): 歌曲 ID
+        difficulty_text (_Difficulty): 谱面难度
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/lsycx'
+    url = settings.backend_url + '/songChart'
     
     # 构建数据
     data = {
-        'server': server,
-        'tier': tier,
+        'default_servers': default_servers,
+        'songId': song_id,
+        'difficultyText': difficulty_text,
         'compress': settings.compress
     }
-    if event_id:
-        data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def room_list(room_list: list[_CarData]) -> _Response:
-    '''绘制车牌绘图
+async def song_meta(default_servers: list[_Server], server: _Server) -> _Response:
+    '''查询歌曲分数表
 
     参数:
-        room_list (list[_CarData]): 车牌信息列表
+        default_servers (list[_Server]): 默认服务器
+        server (_Server): 主服务器
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/roomList'
+    url = settings.backend_url + '/songMeta'
     
     # 构建数据
     data = {
-        'roomList': room_list,
+        'default_servers': default_servers,
+        'server': server,
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_card(default_servers: list[_Server], text: str) -> _Response:
-    '''查询卡片
+async def ycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
+    '''查询排行榜预测线
 
     参数:
-        default_servers (list[_Server]): 默认服务器
-        text (str): 查询参数
+        server (_Server): 服务器
+        tier (int): 排行榜挡位
+        event_id (int): 活动 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/searchCard'
+    url = settings.backend_url + '/ycx'
     
     # 构建数据
     data = {
-        'default_servers': default_servers,
-        'text': text,
-        'useEasyBG': settings.use_easy_bg,
+        'server': server,
+        'tier': tier,
         'compress': settings.compress
     }
+    if event_id:
+        data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def station_query_all_room() -> _QueryResult:
-    '''查询最近车站车牌
-
-    返回:
-        _QueryResult: 响应信息
-    '''
-    
-    # 构建 URL
-    url = settings.backend_url + '/station/queryAllRoom'
-    
-    # 发送请求
-    return await (
-        await Api(
-            url,
-            proxy=settings.backend_proxy
-        ).get()
-    ).json()
-
-async def station_submit_room_number(
-    number: int,
-    raw_message: str,
-    platform: str,
-    user_id: str,
-    user_name: str
-) -> _SubmitResult:
-    '''提交车牌号
+async def ycx_all(server: _Server, event_id: Optional[int] = None) -> _Response:
+    '''查询全挡位预测线
 
     参数:
-        number (int): 车牌号
-        raw_message (str): 原始消息
-        platform (str): 平台
-        user_id (str): 用户 ID
-        user_name (str): 用户名
+        server (_Server): 服务器
+        event_id (int): 活动 ID
 
     返回:
-        _SubmitResult: 响应信息
+        _Response: 响应信息
     '''
     
     # 构建 URL
-    url = settings.backend_url + '/station/submitRoomNumber'
+    url = settings.backend_url + '/ycxAll'
     
     # 构建数据
     data = {
-        'number': number,
-        'raw_message': raw_message,
-        'platform': platform,
-        'user_id': user_id,
-        'user_name': user_name,
-        'time': int(time())
+        'server': server,
+        'compress': settings.compress
     }
+    if event_id:
+        data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
-        proxy=settings.backend_proxy,
-        data=data
-    ).post()
+        proxy=settings.backend_proxy
+    ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
```

