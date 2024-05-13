# Comparing `tmp/nonebot_plugin_kurogames-0.1.7.tar.gz` & `tmp/nonebot_plugin_kurogames-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kurogames-0.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_kurogames-0.1.8.tar", max compression
```

## Comparing `nonebot_plugin_kurogames-0.1.7.tar` & `nonebot_plugin_kurogames-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1062 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/LICENSE
--rw-r--r--   0        0        0     3019 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Outputs/rendered_template.html
--rw-r--r--   0        0        0     8272 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/PNSResult.html
--rw-r--r--   0        0        0    36234 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
--rw-r--r--   0        0        0    25514 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
--rw-r--r--   0        0        0    41565 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
--rw-r--r--   0        0        0    36944 2024-05-12 11:54:16.103071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
--rw-r--r--   0        0        0  5682114 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
--rw-r--r--   0        0        0    10716 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/PNS.png
--rw-r--r--   0        0        0    40106 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
--rw-r--r--   0        0        0    39390 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
--rw-r--r--   0        0        0      198 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/kuro_help.py
--rw-r--r--   0        0        0     1798 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/__init__.py
--rw-r--r--   0        0        0      498 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
--rw-r--r--   0        0        0     3386 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_dao.py
--rw-r--r--   0        0        0     3431 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
--rw-r--r--   0        0        0     2826 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
--rw-r--r--   0        0        0     1749 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
--rw-r--r--   0        0        0     2498 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
--rw-r--r--   0        0        0      483 2024-05-12 11:54:16.119071 nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/token_judgement.py
--rw-r--r--   0        0        0      582 2024-05-12 11:54:16.123071 nonebot_plugin_kurogames-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-13 10:30:43.676668 nonebot_plugin_kurogames-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3019 2024-05-13 10:30:43.676668 nonebot_plugin_kurogames-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 10:30:43.676668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Outputs/rendered_template.html
+-rw-r--r--   0        0        0     8272 2024-05-13 10:30:43.676668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/PNSResult.html
+-rw-r--r--   0        0        0    36234 2024-05-13 10:30:43.676668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
+-rw-r--r--   0        0        0    25514 2024-05-13 10:30:43.676668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
+-rw-r--r--   0        0        0    41565 2024-05-13 10:30:43.676668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
+-rw-r--r--   0        0        0    36944 2024-05-13 10:30:43.676668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
+-rw-r--r--   0        0        0  5682114 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
+-rw-r--r--   0        0        0    10716 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/PNS.png
+-rw-r--r--   0        0        0    40106 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
+-rw-r--r--   0        0        0    39390 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
+-rw-r--r--   0        0        0      198 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/kuro_help.py
+-rw-r--r--   0        0        0     1815 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/config.py
+-rw-r--r--   0        0        0      498 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
+-rw-r--r--   0        0        0     3566 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_dao.py
+-rw-r--r--   0        0        0     3431 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
+-rw-r--r--   0        0        0     2826 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
+-rw-r--r--   0        0        0     1749 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
+-rw-r--r--   0        0        0     2498 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
+-rw-r--r--   0        0        0      483 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/token_judgement.py
+-rw-r--r--   0        0        0      582 2024-05-13 10:30:43.692668 nonebot_plugin_kurogames-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_kurogames-0.1.7/LICENSE` & `nonebot_plugin_kurogames-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/README.md` & `nonebot_plugin_kurogames-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/PNSResult.html` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/PNSResult.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/LAMIA.png` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/LAMIA.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/PNS.png` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/PNS.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/__init__.py` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from nonebot import on_command
-from nonebot.plugin import PluginMetadata
-from nonebot.adapters import Event, Message
 from nonebot.params import CommandArg
+from nonebot.plugin import PluginMetadata
+from nonebot.adapters.onebot.v11 import MessageSegment, Message, Bot, MessageEvent
+
+from .Static.kuro_help import kuro_help
 from .handler.pns_handlers.pns_data_handler import pns_data_handler
 from .handler.pns_handlers.pns_login_handler import pns_login_handler, get_kuro_token
-from nonebot.adapters.onebot.v11 import MessageSegment
-from .Static.kuro_help import kuro_help
-
 
 __plugin_meta__ = PluginMetadata(
     name="库洛游戏信息",
     description="一款库洛游戏角色信息插件",
     usage="发送“战双登录”注册，发送“战双”查询战双详情",
     type="application",
     homepage="https://github.com/ConcyWee/nonebot-plugin-kurogames",
@@ -21,22 +20,22 @@
 
 punishing = on_command("pns", aliases={"战双","战双详情"}, priority=5)
 pns_login = on_command("pnslogin", aliases={"战双登陆","战双登录", "库洛登录", "库洛登陆", "鸣潮登录", "鸣潮登陆"}, priority=5)
 pns_help  = on_command("pnshelp", aliases={"战双帮助", "库洛帮助", "鸣潮帮助"}, priority=5)
 
 
 @pns_login.handle()
-async def _(event: Event, arg: Message = CommandArg()):
+async def _(bot:Bot, event: MessageEvent, arg: Message = CommandArg()):
     user_id = event.get_user_id()
     data_content = arg.extract_plain_text()
     result = await pns_login_handler(user_id, data_content)
     await pns_login.finish(result)
 
 @punishing.handle()
-async def _(event: Event):
+async def _(bot: Bot, event: MessageEvent):
     user_id = event.get_user_id()
     data_row = await get_kuro_token(user_id)
     if data_row:
         pic_result = await pns_data_handler(data_row)
         await punishing.finish(MessageSegment.image(pic_result))
     else:
         await punishing.finish("请先输入token")
```

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_dao.py` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_dao.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import sqlite3
 from pathlib import Path
 from contextlib import contextmanager
+from nonebot import get_plugin_config
+from  ..config import Config
 
+plugin_config = get_plugin_config(Config)
 
-KURODIR = Path.cwd() / 'data'
-DATABASE = KURODIR / 'pns.db'
-KURODIR.mkdir(parents=True, exist_ok=True)
+KURO_DIR = plugin_config.KURO_DB_PATH
+if isinstance(KURO_DIR, str):
+    KURO_DIR = Path(KURO_DIR)
+DATABASE = KURO_DIR / 'pns.db'
+
+KURO_DIR.mkdir(parents=True, exist_ok=True)
 
 class UserInfoManagement:
     _initialized = False
     def __init__(self):
         # 初始化数据库连接
         if not self._initialized:
             self.conn = sqlite3.connect(DATABASE)
```

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py` & `nonebot_plugin_kurogames-0.1.8/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.7/pyproject.toml` & `nonebot_plugin_kurogames-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-kurogames"
-version = "0.1.7"
+version = "0.1.8"
 description = "库洛游戏数据详情 谢比螺六~"
 authors = ["ConcyWee <concywee@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
 repository = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
```

### Comparing `nonebot_plugin_kurogames-0.1.7/PKG-INFO` & `nonebot_plugin_kurogames-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-kurogames
-Version: 0.1.7
+Version: 0.1.8
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
-Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.8 Summary:
 åºæ´æ¸¸ææ°æ®è¯¦æ è°¢æ¯èºå­~ Home-page: https://github.com/ConcyWee/
 nonebot-plugin-kurogames License: MIT Author: ConcyWee Author-email:
 concywee@163.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

