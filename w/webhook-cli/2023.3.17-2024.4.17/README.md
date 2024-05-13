# Comparing `tmp/webhook_cli-2023.3.17.tar.gz` & `tmp/webhook_cli-2024.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhook_cli-2023.3.17.tar", last modified: Wed Jan 17 14:44:48 2024, max compression
+gzip compressed data, was "webhook_cli-2024.4.17.tar", last modified: Mon May 13 13:19:48 2024, max compression
```

## Comparing `webhook_cli-2023.3.17.tar` & `webhook_cli-2024.4.17.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-01-17 14:44:48.477751 webhook_cli-2023.3.17/
--rw-r--r--   0 nico       (502) staff       (20)     3531 2024-01-17 14:44:48.477342 webhook_cli-2023.3.17/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)     2720 2023-03-15 03:35:11.000000 webhook_cli-2023.3.17/README.md
--rw-r--r--   0 nico       (502) staff       (20)       38 2024-01-17 14:44:48.477875 webhook_cli-2023.3.17/setup.cfg
--rw-r--r--   0 nico       (502) staff       (20)     2114 2024-01-17 14:38:23.000000 webhook_cli-2023.3.17/setup.py
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-01-17 14:44:48.470939 webhook_cli-2023.3.17/test/
--rw-r--r--   0 nico       (502) staff       (20)       54 2023-03-14 07:56:50.000000 webhook_cli-2023.3.17/test/test_cli.py
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-01-17 14:44:48.472929 webhook_cli-2023.3.17/webhook_cli/
--rw-r--r--   0 nico       (502) staff       (20)     1310 2024-01-17 14:39:13.000000 webhook_cli-2023.3.17/webhook_cli/__init__.py
--rw-r--r--   0 nico       (502) staff       (20)      856 2023-03-15 03:14:18.000000 webhook_cli-2023.3.17/webhook_cli/_helper.py
--rwxr-xr-x   0 nico       (502) staff       (20)     3914 2024-01-18 02:00:30.000000 webhook_cli-2023.3.17/webhook_cli/cli.py
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-01-17 14:44:48.476820 webhook_cli-2023.3.17/webhook_cli/ext/
--rw-r--r--   0 nico       (502) staff       (20)        0 2023-03-14 03:40:59.000000 webhook_cli-2023.3.17/webhook_cli/ext/__init__.py
--rw-r--r--   0 nico       (502) staff       (20)    13437 2024-01-18 02:33:44.000000 webhook_cli-2023.3.17/webhook_cli/ext/dingtalk.py
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-01-17 14:44:48.476139 webhook_cli-2023.3.17/webhook_cli.egg-info/
--rw-r--r--   0 nico       (502) staff       (20)     3531 2024-01-17 14:44:48.000000 webhook_cli-2023.3.17/webhook_cli.egg-info/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)      403 2024-01-17 14:44:48.000000 webhook_cli-2023.3.17/webhook_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nico       (502) staff       (20)        1 2024-01-17 14:44:48.000000 webhook_cli-2023.3.17/webhook_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nico       (502) staff       (20)       49 2024-01-17 14:44:48.000000 webhook_cli-2023.3.17/webhook_cli.egg-info/entry_points.txt
--rw-r--r--   0 nico       (502) staff       (20)        1 2023-03-14 08:15:45.000000 webhook_cli-2023.3.17/webhook_cli.egg-info/not-zip-safe
--rw-r--r--   0 nico       (502) staff       (20)       63 2024-01-17 14:44:48.000000 webhook_cli-2023.3.17/webhook_cli.egg-info/requires.txt
--rw-r--r--   0 nico       (502) staff       (20)       12 2024-01-17 14:44:48.000000 webhook_cli-2023.3.17/webhook_cli.egg-info/top_level.txt
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-05-13 13:19:48.044371 webhook_cli-2024.4.17/
+-rw-r--r--   0 nico       (502) staff       (20)     3531 2024-05-13 13:19:48.043888 webhook_cli-2024.4.17/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)     2720 2023-03-15 03:35:11.000000 webhook_cli-2024.4.17/README.md
+-rw-r--r--   0 nico       (502) staff       (20)       38 2024-05-13 13:19:48.044470 webhook_cli-2024.4.17/setup.cfg
+-rw-r--r--   0 nico       (502) staff       (20)     2131 2024-05-13 13:19:35.000000 webhook_cli-2024.4.17/setup.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-05-13 13:19:48.034462 webhook_cli-2024.4.17/test/
+-rw-r--r--   0 nico       (502) staff       (20)       54 2023-03-14 07:56:50.000000 webhook_cli-2024.4.17/test/test_cli.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-05-13 13:19:48.037252 webhook_cli-2024.4.17/webhook_cli/
+-rw-r--r--   0 nico       (502) staff       (20)     1311 2024-05-13 13:06:19.000000 webhook_cli-2024.4.17/webhook_cli/__init__.py
+-rw-r--r--   0 nico       (502) staff       (20)      856 2023-03-15 03:14:18.000000 webhook_cli-2024.4.17/webhook_cli/_helper.py
+-rwxr-xr-x   0 nico       (502) staff       (20)     4049 2024-05-13 13:18:40.000000 webhook_cli-2024.4.17/webhook_cli/cli.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-05-13 13:19:48.042958 webhook_cli-2024.4.17/webhook_cli/ext/
+-rw-r--r--   0 nico       (502) staff       (20)        0 2023-03-14 03:40:59.000000 webhook_cli-2024.4.17/webhook_cli/ext/__init__.py
+-rw-r--r--   0 nico       (502) staff       (20)    15302 2024-05-13 13:12:47.000000 webhook_cli-2024.4.17/webhook_cli/ext/dingtalk.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-05-13 13:19:48.040786 webhook_cli-2024.4.17/webhook_cli.egg-info/
+-rw-r--r--   0 nico       (502) staff       (20)     3531 2024-05-13 13:19:47.000000 webhook_cli-2024.4.17/webhook_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)      403 2024-05-13 13:19:48.000000 webhook_cli-2024.4.17/webhook_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nico       (502) staff       (20)        1 2024-05-13 13:19:48.000000 webhook_cli-2024.4.17/webhook_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nico       (502) staff       (20)       49 2024-05-13 13:19:48.000000 webhook_cli-2024.4.17/webhook_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nico       (502) staff       (20)        1 2023-03-14 08:15:45.000000 webhook_cli-2024.4.17/webhook_cli.egg-info/not-zip-safe
+-rw-r--r--   0 nico       (502) staff       (20)       63 2024-05-13 13:19:48.000000 webhook_cli-2024.4.17/webhook_cli.egg-info/requires.txt
+-rw-r--r--   0 nico       (502) staff       (20)       12 2024-05-13 13:19:48.000000 webhook_cli-2024.4.17/webhook_cli.egg-info/top_level.txt
```

### Comparing `webhook_cli-2023.3.17/PKG-INFO` & `webhook_cli-2024.4.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhook_cli
-Version: 2023.3.17
+Version: 2024.4.17
 Summary: webhook通知命令行工具
 Home-page: https://git.minieye.tech/nico/wehook-cli
 Author: Nico Ning
 Author-email: ningrong@minieye.cc
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `webhook_cli-2023.3.17/README.md` & `webhook_cli-2024.4.17/README.md`

 * *Files identical despite different names*

### Comparing `webhook_cli-2023.3.17/setup.py` & `webhook_cli-2024.4.17/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+## coding: utf-8
 #! python3
 import io
 import re
 import sys
 import os.path
 from setuptools import setup, find_packages
```

### Comparing `webhook_cli-2023.3.17/webhook_cli/__init__.py` & `webhook_cli-2024.4.17/webhook_cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     webhook-cli msg.json
     webhook-cli --url
 
     :copyright: © 2023 by the NicoNing.
     :license: GPL, see LICENSE for more details.
 """
 
-__version__ = '2023.3.17'
+__version__ = '2024.4.17'
 
 long_usage = f"""
     
     webhook命令行工具 ({__version__})
 
 eg:
   [0] webhook --init_config        ; 初始化配置模板 
@@ -34,7 +34,8 @@
   [1] --webhook_url 
   [2] 当前进程，使用环境变量指定的配置文件(ENV.$WEBHOOK_CONFIG) 
   [4] 当前工作目录下的 config.toml  
   [5] Ubuntu系统全局默认：$HOME/.config/webhook_cli/config.toml 
 
 ## 可选参数:   
 """
+
```

### Comparing `webhook_cli-2023.3.17/webhook_cli/_helper.py` & `webhook_cli-2024.4.17/webhook_cli/_helper.py`

 * *Files identical despite different names*

### Comparing `webhook_cli-2023.3.17/webhook_cli/cli.py` & `webhook_cli-2024.4.17/webhook_cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     --version           ; 获取版本号
     --config            ; 显示默认的配置文件， 及其内容
     """
     PROG = "webhook"
     if sys.argv[0].startswith("."):
         PROG = sys.argv[0]
     tip_help = f"如需帮助，请运行: {PROG} --help"
-    tip_usage = webhook_cli.long_usage
+    tip_usage = webhook_cli.long_usage + os.linesep + os.path.abspath(__file__) + os.linesep
+    # tip_usage = webhook_cli.long_usage + os.linesep * 2 + WebhookDingTalk.desc
     sys_parser = argparse.ArgumentParser(usage=tip_usage, prog=PROG)
     sys_parser.add_argument("-v", "--version", help="显示版本号", action="store_true")
     sys_parser.add_argument("-d", "--dry_run", help="不运行，只打印调试参数", action="store_true")
     sys_parser.add_argument("-i", "--init_config", help="生成默认配置(./config.toml)", action="store_true")
     sys_parser.add_argument("-c", "--check_config", help="检查当前的配置", action="store_true")
     sys_parser.add_argument("--webhook_url", help="如果设定，将覆盖默认配置的webhook_url", default="")
     sys_parser.add_argument("--file", help="必须是可读的文本文件，支持markdown文件(.md);\n"
```

### Comparing `webhook_cli-2023.3.17/webhook_cli/ext/dingtalk.py` & `webhook_cli-2024.4.17/webhook_cli/ext/dingtalk.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,130 +20,175 @@
 from webhook_cli._helper import env, env_bool, BColors
 
 
 class WebhookDingTalk():
     cfg_dir = os.environ.get("HOME", os.getcwd())
     cfg_system = os.path.join(cfg_dir, ".config/webhook_cli/config.toml")
     cfg_default = os.path.join(os.getcwd(), "config.toml")
-    cfg_custom = ""
-    desc = "[配置优先级]：${config} >  ENV.$WEBHOOK_CONFIG   > config.toml > $HOME/.config/webhook_cli/config.toml"
+    cfg_custom = ""  # ; 选填
+    CfgOptions = None  # ; 选填
+    WEBHOOK_API = "https://oapi.dingtalk.com/robot/send"
+    ENV_DEFAULT = "WEBHOOK_CONFIG"
+
+
+    @classmethod
+    @property
+    def desc(cls):
+        return f"[Webhook-cli.SDK配置优先级]：" \
+               f"\r\n【0】. $CfgOptions: 自定义的配置键表(Dict) " \
+               f"\r\n【1】. $cfg_custom: 自定义的配置文件 " \
+               f"\r\n【2】. $ENV.{cls.ENV_DEFAULT}: 自定义的通过环境变量指定的配置文件路径" \
+               f"\r\n【3】. $cfg_default: 默认当前工作路径的配置文件(config.toml)" \
+               f"\r\n【4】. $cfg_system:  默认系统的全局配置文件($HOME/.config/webhook_cli/config.toml)"
 
     _options_sample_ = dict(
         app_type="dingtalk",
-        app_desc="\n钉钉群机器人配置模板（可设置为 ENV.$WEBHOOK_CONFIG , 支持toml/json）："
+        app_desc="\n钉钉群机器人配置说明【（】可设置为 ENV.$WEBHOOK_CONFIG , 支持toml/json）："
                  "\n 0. webhook_url 必要的配置项, 其它均为可选；"
                  "\n 1. 以`x`前缀的配置项, 是内置的控制项；"
                  "\n 2. 以`_`前缀的配置项, 是开发调试参数, 不建议稳定版本使用；"
                  "\n 3. 以`#`前缀或后缀的配置项, 可视为注释，可忽略；"
                  "\n 4. 其它参数与 app_type (默认为'dingtalk')相关, 不一而论。"
                  "\n\n",
         keyword="webhook通知的关键词",
         webhook_url="https://oapi.dingtalk.com/robot/send?access_token=${}",
         at_mobiles=["${手机号码1}", "${手机号码2}"],
         at_mobiles_global=[],
         x_cached_msg_dir="./_.webhook-cached",
         x_cached_msg_always=False,
         x_cached_msg_if_failed=True,
     )
+
     _options_sample_["_ENV_PARAM_REFER_MAP_"] = dict(
         WEBHOOK_URL="自定义url",
         WEBHOOK_CONFIG="自定义配置文件",
     )
 
-
     @classmethod
     def get_config_file(cls, nullable=True):
-        if cls.cfg_custom:
-            if not os.path.isfile(cls.cfg_custom):
-                print(f"[配置文件不存在] 请检查路径 {cls.cfg_custom} (cwd: {os.getcwd()})")
-                if not nullable:
-                    raise FileNotFoundError(cls.cfg_custom)
-                else:
-                    return None
+        is_exist, fp, msg = cls._get_config_file(nullable)
+        if not is_exist:
+            print(msg)
+            print(cls.desc)
+            if not nullable:
+                raise FileNotFoundError(msg)
+        return fp
+
+    @classmethod
+    def _get_config_file(cls, nullable=True):
+        ##; 肮脏的逻辑，但是这样才比较符合用户直觉。
+        ##; 如果已配置，必须有效; 如果未配置，则按预设权重查找配置文件;
+        ##return: is_exist, fp, msg 
+        if os.path.isfile(cls.cfg_custom):
+            msg = f"[自定义配置] 加载成功: {cls.cfg_custom} "
+            return True, cls.cfg_custom, msg
+        elif cls.cfg_custom:
+            msg = f"[自定义配置] 无法加载: {cls.cfg_custom} (abs: {os.path.abspath(cls.cfg_custom)})"
+            if not nullable:
+                raise FileNotFoundError(msg)
             else:
-                print(f"[自定义配置] {cls.cfg_custom} ")
-                return cls.cfg_custom
+                return False, cls.cfg_custom, msg
 
-        config_file = env("WEBHOOK_CONFIG", cls.cfg_default)
-        if os.path.exists(config_file):
-            print(f"[使用配置] {config_file} ")
-            return config_file
+        if cls.ENV_DEFAULT:
+            config_file = env(cls.ENV_DEFAULT, cls.cfg_default)
+        else:
+            config_file = cls.cfg_default
+
+        if os.path.isfile(config_file):
+            msg = f"[默认配置] 加载成功(ENV.${cls.ENV_DEFAULT}): {config_file} "
+            return True, config_file, msg
         elif config_file != cls.cfg_default:
-            print(f"[配置无效] 找不到此文件( ENV.$WEBHOOK_CONFIG  ): {config_file} ")
+            msg = f"[默认配置] 无法加载(ENV.${cls.ENV_DEFAULT}): {config_file} "
             if not nullable:
                 raise FileNotFoundError(config_file)
+            return False, config_file, msg
+
         elif os.path.exists(cls.cfg_system):
-            print(f"[系统配置] {cls.cfg_system} ")
-            return cls.cfg_system
+            msg = f"[系统配置] 加载成功: {cls.cfg_system} "
+            return True, cls.cfg_system, msg
 
-        print(f"[配置失效] webhook_cli 找不到配置文件 !!!")
+        msg = f"[配置失效] webhook_cli 找不到配置文件 !!!"
         if not nullable:
             print(cls.desc)
             raise FileNotFoundError(cls.cfg_default)
 
+        return False, config_file, msg
+
 
     @classmethod
     def get_config_options(cls, stdout=False, **kwargs):
         if stdout:
-            print(cls.desc)
             print(f"[系统配置]:{cls.cfg_system}  ({os.path.exists(cls.cfg_system)})")
             print(f"[缺省配置]:{cls.cfg_default} ({os.path.exists(cls.cfg_default)})", )
 
-        fp = cls.get_config_file(nullable=True)
-        if fp is None:
-            return kwargs
-
-        if fp.endswith(".json") or fp.endswith(".json5"):
-            with open(fp, "r") as fr:
-                data = json5.load(fr)  # type:dict
-                data.update(kwargs)
+        is_exist, fp, msg = cls._get_config_file(nullable=True)
+        if isinstance(cls.CfgOptions, dict):
+            kws = dict(cls.CfgOptions, **kwargs)
         else:
-            with open(fp, "r") as fr:
-                data = rtoml.load(fr)
-                data.update(kwargs)
+            kws = kwargs
+        if is_exist:
+            if fp.endswith(".json") or fp.endswith(".json5"):
+                with open(fp, "r") as fr:
+                    data = json5.load(fr)  # type:dict
+                    data.update(kws)
+            else:
+                with open(fp, "r") as fr:
+                    data = rtoml.load(fr)
+                    data.update(kws)
+            kws = data
+        elif stdout:
+            print(msg)
+
         if stdout:
-            text = rtoml.dumps(data, pretty=True)
+            text = rtoml.dumps(kws, pretty=True)
             print("\n" + "##" * 20 + BColors.OK)
             print(text)
             print(BColors.ENDC + "##" * 20 + "\n")
-        webhook_url = data.get("webhook_url")
+
+        access_token = kws.get("access_token")
+        if access_token:
+            webhook_url = f"{cls.WEBHOOK_API}?access_token={access_token}"
+            webhook_url = kws.setdefault("webhook_url", webhook_url)
+        else:
+            webhook_url = kws.get("webhook_url", "")
         if not webhook_url:
-            print(f"[当前配置] {fp}\n")
-            print("[该配置无效] 必须提供有效的$webhook_url")
-            cls.set_config_sample(output_file="")
-        return data
+            print(f"[当前配置] {fp}")
+            print("[配置无效] 未提供有效的$webhook_url")
+            cls.set_config_sample(output_file=fp)
+        return kws
 
 
     @classmethod
     def set_config_sample(cls, output_file: (str, bool) = cfg_default, **kwargs):
         output_rel = os.path.relpath(output_file, os.getcwd())
         print("\n" + "##" * 20)
         print(f"## 生成参考配置: {output_rel} " + BColors.OK)
         options = cls._options_sample_
+        options.update(kwargs)
         text = rtoml.dumps(options, pretty=True)
         print(text)
         print(BColors.ENDC + "##" * 20 + "\n")
         if output_file and isinstance(output_file, str):
             if os.path.exists(output_file):
                 print(f"[配置文件已存在] {output_file}")
                 print(f"[建议] 如果要覆盖配置, 先备份再删除, 然后重试。")
             else:
                 with safely_open(output_file, "w") as fo:
                     fo.write(text)
                 print(f"[配置文件已保存] {output_rel}")
         return options
 
     @classmethod
-    def _send_data(cls, msgtype: str, msgdata: dict, is_at_all=False, **kwargs):
+    def _send_data(cls, msgtype: str, msgdata: dict, is_at_all=False, params=None, headers=None, **kwargs):
         options = cls.get_config_options(**kwargs)
         at_mobiles = options.get("at_mobiles", [])
         at_mobiles_g = options.get("at_mobiles_global", [])
         at_mobiles.extend(at_mobiles_g)
 
-        webhook_url = options.get("webhook_url")
+        webhook_url = options.get("webhook_url", cls.WEBHOOK_API)
         keyword = options.get("keyword", "")
 
         data = dict(
             msgtype=msgtype,
             at=dict(
                 atMobiles=at_mobiles,
                 isAtAll=is_at_all,
@@ -153,15 +198,15 @@
         data[msgtype] = msgdata
         if not webhook_url:
             print("[通知失败] invalid $webhook_url")
             pprint(msgdata, indent=2)
             return -1, data
 
         now = datetime.datetime.now()
-        resp = requests.post(webhook_url, json=data)
+        resp = requests.post(webhook_url, json=data, params=params, headers=headers)
         if resp.status_code == 200:
             print(f"[发送通知] {keyword} {msgtype} at_mobiles:{at_mobiles}")
             resp_data = resp.json()  # type:dict
             print("[response]", resp_data)
             errcode = resp_data.get("errcode")
             data = OrderedDict(
                 webhook="dingtalk",
```

### Comparing `webhook_cli-2023.3.17/webhook_cli.egg-info/PKG-INFO` & `webhook_cli-2024.4.17/webhook_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhook-cli
-Version: 2023.3.17
+Version: 2024.4.17
 Summary: webhook通知命令行工具
 Home-page: https://git.minieye.tech/nico/wehook-cli
 Author: Nico Ning
 Author-email: ningrong@minieye.cc
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

