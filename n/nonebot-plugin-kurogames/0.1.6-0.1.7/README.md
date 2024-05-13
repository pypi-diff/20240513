# Comparing `tmp/nonebot_plugin_kurogames-0.1.6.tar.gz` & `tmp/nonebot_plugin_kurogames-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kurogames-0.1.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_kurogames-0.1.7.tar", max compression
```

## Comparing `nonebot_plugin_kurogames-0.1.6.tar` & `nonebot_plugin_kurogames-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1062 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/LICENSE
--rw-r--r--   0        0        0     3019 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Outputs/rendered_template.html
--rw-r--r--   0        0        0     8272 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/PNSResult.html
--rw-r--r--   0        0        0    36234 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
--rw-r--r--   0        0        0    25514 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
--rw-r--r--   0        0        0    41565 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
--rw-r--r--   0        0        0    36944 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
--rw-r--r--   0        0        0  5682114 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
--rw-r--r--   0        0        0    10716 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/PNS.png
--rw-r--r--   0        0        0    40106 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
--rw-r--r--   0        0        0    39390 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
--rw-r--r--   0        0        0      198 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/kuro_help.py
--rw-r--r--   0        0        0     1758 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/__init__.py
--rw-r--r--   0        0        0      498 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
--rw-r--r--   0        0        0     3279 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_dao.py
--rw-r--r--   0        0        0     2982 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
--rw-r--r--   0        0        0     3059 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
--rw-r--r--   0        0        0     1725 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
--rw-r--r--   0        0        0     2498 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
--rw-r--r--   0        0        0      483 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/token_judgement.py
--rw-r--r--   0        0        0      582 2024-05-12 03:59:34.284203 nonebot_plugin_kurogames-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3019 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Outputs/rendered_template.html
+-rw-r--r--   0        0        0     8272 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/PNSResult.html
+-rw-r--r--   0        0        0    36234 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
+-rw-r--r--   0        0        0    25514 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
+-rw-r--r--   0        0        0    41565 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
+-rw-r--r--   0        0        0    36944 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
+-rw-r--r--   0        0        0  5682114 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
+-rw-r--r--   0        0        0    10716 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/PNS.png
+-rw-r--r--   0        0        0    40106 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
+-rw-r--r--   0        0        0    39390 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
+-rw-r--r--   0        0        0      198 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/kuro_help.py
+-rw-r--r--   0        0        0     1798 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
+-rw-r--r--   0        0        0     3386 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_dao.py
+-rw-r--r--   0        0        0     3431 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
+-rw-r--r--   0        0        0     2826 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
+-rw-r--r--   0        0        0     1749 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
+-rw-r--r--   0        0        0     2498 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
+-rw-r--r--   0        0        0      483 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/token_judgement.py
+-rw-r--r--   0        0        0      582 2024-05-12 11:54:16.123071 nonebot_plugin_kurogames-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.7/PKG-INFO
```

### Comparing `nonebot_plugin_kurogames-0.1.6/LICENSE` & `nonebot_plugin_kurogames-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/README.md` & `nonebot_plugin_kurogames-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/PNSResult.html` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/PNSResult.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/LAMIA.png` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/LAMIA.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/PNS.png` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/PNS.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/__init__.py` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 __plugin_meta__ = PluginMetadata(
     name="库洛游戏信息",
     description="一款库洛游戏角色信息插件",
     usage="发送“战双登录”注册，发送“战双”查询战双详情",
     type="application",
     homepage="https://github.com/ConcyWee/nonebot-plugin-kurogames",
     config=None,
-    supported_adapters=None
+    supported_adapters={"nonebot.adapters.onebot.v11"},
 )
 
 
 punishing = on_command("pns", aliases={"战双","战双详情"}, priority=5)
 pns_login = on_command("pnslogin", aliases={"战双登陆","战双登录", "库洛登录", "库洛登陆", "鸣潮登录", "鸣潮登陆"}, priority=5)
 pns_help  = on_command("pnshelp", aliases={"战双帮助", "库洛帮助", "鸣潮帮助"}, priority=5)
 
 
 @pns_login.handle()
 async def _(event: Event, arg: Message = CommandArg()):
     user_id = event.get_user_id()
     data_content = arg.extract_plain_text()
-    result = pns_login_handler(user_id, data_content)
+    result = await pns_login_handler(user_id, data_content)
     await pns_login.finish(result)
 
 @punishing.handle()
 async def _(event: Event):
     user_id = event.get_user_id()
-    data_row = get_kuro_token(user_id)
+    data_row = await get_kuro_token(user_id)
     if data_row:
         pic_result = await pns_data_handler(data_row)
         await punishing.finish(MessageSegment.image(pic_result))
     else:
         await punishing.finish("请先输入token")
 
 @pns_help.handle()
```

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_dao.py` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_dao.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import sqlite3
+from pathlib import Path
 from contextlib import contextmanager
 
-DATABASE = './pns.db'
+
+KURODIR = Path.cwd() / 'data'
+DATABASE = KURODIR / 'pns.db'
+KURODIR.mkdir(parents=True, exist_ok=True)
 
 class UserInfoManagement:
     _initialized = False
     def __init__(self):
         # 初始化数据库连接
         if not self._initialized:
             self.conn = sqlite3.connect(DATABASE)
```

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,89 +19,67 @@
         'sec-fetch-mode': 'cors',
         'sec-fetch-dest': 'empty',
         'accept-encoding': 'gzip, deflate, br, zstd',
         'accept-language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
         'user-agent': 'okhttp/3.10.0',
     }
 
-def getPunishingResource(token):
+async def get_punishing_resource(token):
     REFRESH_URL = 'https://api.kurobbs.com/gamer/widget/game2/refresh'
     header_data['token'] = token
     form_data = {
         'gameId': 2,
         'type': 2,
     }
+    return await do_fetch(REFRESH_URL, header_data, form_data)
 
-    try:
-        result = do_fetch(REFRESH_URL, header_data, form_data)
-    except Exception as e:
-        raise e
-    return result
-
-def get_punishing_account_info(token):
+async def get_punishing_account_info(token):
     PNS_INFO_URL = 'https://api.kurobbs.com/gamer/role/list'
     header_data['token'] = token
     form_data = {
         'gameId': 2,
     }
+    return await do_fetch(PNS_INFO_URL, header_data, form_data)
 
-    try:
-        result = do_fetch(PNS_INFO_URL, header_data, form_data)
-    except Exception as e:
-        raise e
-    return result
-
-def get_mc_account_info(token):
+async def get_mc_account_info(token):
 
     MC_INFO_URL = 'https://api.kurobbs.com/gamer/role/list'
     header_data['token'] = token
     form_data = {
         'gameId': 3,
     }
 
-    try:
-        result = do_fetch(MC_INFO_URL, header_data, form_data)
-    except Exception as e:
-        raise e
-    return result
+    return await do_fetch(MC_INFO_URL, header_data, form_data)
 
-def get_monthly_resource(roleId, token):
+async def get_monthly_resource(roleId, token):
     MONTHLY_RESOURCE_URL = 'https://api.kurobbs.com/gamer/resource/month'
     header_data['token'] = token
     form_data = {
         'roleId': roleId,
     }
-    try:
-        result = do_fetch(MONTHLY_RESOURCE_URL, header_data, form_data)
-    except Exception as e:
-        raise e
-    return result
+    return await do_fetch(MONTHLY_RESOURCE_URL, header_data, form_data)
 
-def get_pns_game_account(roleId, serverId, token):
+async def get_pns_game_account(roleId, serverId, token):
     GAME_ACCOUNT_URL = 'https://api.kurobbs.com/gamer/roleBox/gameAccount'
     header_data['token'] = token
     form_data = {
         'gameId' : 2,
         'roleId' : roleId,
         'serverId' : serverId,
     }
-    try:
-        result = do_fetch(GAME_ACCOUNT_URL, header_data, form_data)
-    except Exception as e:
-        raise e
-    return result
-
-def do_fetch(url, header, data):
-    try:
-        response = httpx.post(url, headers=header, data=data)
-        if not (response.status_code == 200):
-            raise Exception('fetch error: ', response.status_code, response.reason_phrase)
-        else:
-            rsp = response.json()
+    return await do_fetch(GAME_ACCOUNT_URL, header_data, form_data)
 
-            if rsp.get('code') == 200:
-                result = rsp
+async def do_fetch(url, header, data):
+    async with httpx.AsyncClient() as client:
+        try:
+            response = await client.post(url, headers=header, data=data)
+            if not (response.status_code == 200):
+                raise Exception('fetch error: ', response.status_code, response.reason_phrase)
             else:
-                raise Exception('api error:', rsp)
-    except Exception as e:
-        raise Exception('fetch error: '+ str(e))
-    return result
+                rsp = response.json()
+
+                if rsp.get('code') == 200:
+                    return rsp
+                else:
+                    raise Exception('api error:', rsp)
+        except Exception as e:
+            raise Exception('fetch error: '+ str(e))
```

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 from ..pns_dao import UserInfoManagement
 from ..token_judgement import token_judgement
 from .pns_detail_handler import get_punishing_account_info, get_mc_account_info
 
 manager = UserInfoManagement()
-def pns_login_handler(user_id, data_content):
+async def pns_login_handler(user_id, data_content):
 
     if data_content == "":
         return("请输入战双token, 如：/战双登录 your_token")
     if token_judgement(data_content) != "success":
         return(token_judgement(data_content))
 
-    pns_info  = get_punishing_account_info(json.loads(data_content)["data"]["token"])
-    mc_info   = get_mc_account_info(json.loads(data_content)["data"]["token"])
+    pns_info  = await get_punishing_account_info(json.loads(data_content)["data"]["token"])
+    mc_info   = await get_mc_account_info(json.loads(data_content)["data"]["token"])
 
     pns_id    = None if (not pns_info["data"])  else pns_info["data"][0]["roleId"]
     mc_id     = None if (not mc_info["data"])   else mc_info ["data"][0]["roleId"]
 
     if pns_id or mc_id:
         server_id = pns_info["data"][0]["serverId"]  if (pns_info["data"])  else mc_info["data"]["serverId"] if (mc_info["data"]) else None
         data = {
@@ -36,10 +36,10 @@
             try:
                 manager._insert_data(user_id, data)
             except Exception as e:
                 return("插入数据失败: " + str(e))
         return("token保存成功！")
     return("该账号暂未绑定任何游戏")
 
-def get_kuro_token(qq_id):
+async def get_kuro_token(qq_id):
     result = manager._get_data(qq_id)
     return result
```

### Comparing `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py` & `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.6/pyproject.toml` & `nonebot_plugin_kurogames-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-kurogames"
-version = "0.1.6"
+version = "0.1.7"
 description = "库洛游戏数据详情 谢比螺六~"
 authors = ["ConcyWee <concywee@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
 repository = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
```

### Comparing `nonebot_plugin_kurogames-0.1.6/PKG-INFO` & `nonebot_plugin_kurogames-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-kurogames
-Version: 0.1.6
+Version: 0.1.7
 Summary: 库洛游戏数据详情 谢比螺六~
 Home-page: https://github.com/ConcyWee/nonebot-plugin-kurogames
 License: MIT
 Author: ConcyWee
 Author-email: concywee@163.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.7 Summary:
 åºæ´æ¸¸ææ°æ®è¯¦æ è°¢æ¯èºå­~ Home-page: https://github.com/ConcyWee/
 nonebot-plugin-kurogames License: MIT Author: ConcyWee Author-email:
 concywee@163.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

