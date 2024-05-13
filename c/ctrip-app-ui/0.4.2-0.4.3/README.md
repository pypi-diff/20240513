# Comparing `tmp/ctrip-app-ui-0.4.2.tar.gz` & `tmp/ctrip-app-ui-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.4.2.tar", last modified: Sun May 12 18:04:19 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.4.3.tar", last modified: Mon May 13 17:24:35 2024, max compression
```

## Comparing `ctrip-app-ui-0.4.2.tar` & `ctrip-app-ui-0.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 18:04:19.722674 ctrip-app-ui-0.4.2/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-12 18:04:19.720684 ctrip-app-ui-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 18:04:19.709686 ctrip-app-ui-0.4.2/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.2/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.2/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.2/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.2/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.2/capp_ui/dir.py
--rw-rw-rw-   0        0        0    64496 2024-05-12 18:03:38.000000 ctrip-app-ui-0.4.2/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.2/capp_ui/fee.py
--rw-rw-rw-   0        0        0     3859 2024-05-11 16:34:35.000000 ctrip-app-ui-0.4.2/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24664 2024-05-12 17:54:06.000000 ctrip-app-ui-0.4.2/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.2/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.2/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.2/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.2/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-12 18:04:19.719659 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 18:04:19.722674 ctrip-app-ui-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1103 2024-05-12 18:04:14.000000 ctrip-app-ui-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:24:35.406988 ctrip-app-ui-0.4.3/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-13 17:24:35.404992 ctrip-app-ui-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 17:24:35.390032 ctrip-app-ui-0.4.3/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.3/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.3/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.3/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.3/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.3/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    64892 2024-05-13 17:22:07.000000 ctrip-app-ui-0.4.3/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.3/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     3859 2024-05-11 16:34:35.000000 ctrip-app-ui-0.4.3/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.4.3/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.3/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.3/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.3/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.3/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:24:35.403995 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 17:24:35.000000 ctrip-app-ui-0.4.3/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 17:24:35.407987 ctrip-app-ui-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-13 17:24:26.000000 ctrip-app-ui-0.4.3/setup.py
```

### Comparing `ctrip-app-ui-0.4.2/LICENSE` & `ctrip-app-ui-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/config.py` & `ctrip-app-ui-0.4.3/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/date_extend.py` & `ctrip-app-ui-0.4.3/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/device.py` & `ctrip-app-ui-0.4.3/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/dir.py` & `ctrip-app-ui-0.4.3/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/domain_service.py` & `ctrip-app-ui-0.4.3/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import time
 import typing as t
 from decimal import Decimal
 from poco.proxy import UIObjectProxy
 from poco.exceptions import PocoNoSuchNodeException, PocoTargetTimeout
 
 from capp_ui.platforms import PlatformService
-from capp_ui.mobile_terminals import stop_app
 from capp_ui.utils import get_ui_object_proxy_attr
 from capp_ui.config import ctrip_soft_keyboard_position
+from capp_ui.mobile_terminals import stop_app, PocoProxy
 from capp_ui.date_extend import is_later_than_current_time
 from capp_ui.dir import get_images_dir, is_exists, join_path
 from capp_ui.date_extend import get_trip_year_month_day, get_datetime_area, is_public_holiday
 from capp_ui.libs import SleepWait, LoopFindElement, LoopFindElementSubmit, logger, LoopClickElement
 
 
 class CtripAppService(object):
@@ -32,27 +32,37 @@
     """
     IMAGE_DIR = get_images_dir()
 
     def __init__(self, device_id: str, port: int = 0, enable_debug: bool = False, platform: str = "Android",
                  app_name: str = None, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.app_name = app_name or "ctrip.android.view"
+        self.poco = None
         self.device = PlatformService(device_id=device_id, enable_debug=enable_debug, platform=platform,
                                       port=port).device
 
     def start(self) -> None:
         self.device.start_app(self.app_name)
+        time.sleep(1.0)
+        poco_poxy = PocoProxy()
+        self.device.poco = poco_poxy.poco
+        self.device.get_po = poco_poxy.get_po
+        self.device.get_po_extend = poco_poxy.get_po_extend
 
     def stop(self) -> None:
         stop_app(self.app_name, device_id=self.device.device_id)
 
-    @LoopFindElementSubmit(loop=1, action="重启应用")
     def restart(self):
         stop_app(self.app_name, device_id=self.device.device_id)
+        time.sleep(1.0)
         self.device.start_app(self.app_name)
+        poco_poxy = PocoProxy()
+        self.device.poco = poco_poxy.poco
+        self.device.get_po = poco_poxy.get_po
+        self.device.get_po_extend = poco_poxy.get_po_extend
 
     def hide_navigation_bar(self):
         """如果导航栏已打开，需要隐藏，导航栏很影响元素定位"""
         try:
             navigation_bar = self.device.get_po(
                 type="android.widget.ImageView", name="com.android.systemui:id/hide", desc="隐藏"
             )
```

### Comparing `ctrip-app-ui-0.4.2/capp_ui/fee.py` & `ctrip-app-ui-0.4.3/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/libs.py` & `ctrip-app-ui-0.4.3/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.4.3/capp_ui/mobile_terminals.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,17 +96,15 @@
         self.platform = platform
         self.device_id = device_id
         self.port = port
         self.device_conn = device_conn
         self.enable_debug = enable_debug
         self.__init_device()
         self.dev = device()
-        self.poco = AndroidUiautomationPoco(
-            use_airtest_input=True, screenshot_each_action=False, force_restart=True
-        )
+        self.poco = None
 
     def __init_device(self) -> None:
         if not cli_setup():
             project_root = get_project_path()
             airtest.utils.compat.DEFAULT_LOG_DIR = "logs"
             airtest.core.settings.Settings.DEBUG = self.enable_debug
             airtest.core.settings.Settings.LOG_FILE = "{}.log".format(self.device_id)
@@ -458,14 +456,63 @@
         if self.platform in (DEFAULT_PLATFORM, WINDOWS_PLATFORM, iOS_PLATFORM):
             # self.device.set_clipboard("content")
             # will paste "content" to the device
             # self.device.paste()
             result = self.dev.paste(*args, **kwargs)
         return result or None
 
+    @airtest_exception_format
+    def hide_keyword(self, file_name: str) -> None:
+        temp = self.get_cv_template(file_name=file_name)
+        hide_icon = self.find_all(v=temp)
+        if len(hide_icon) > 0:
+            logger.info("目前检测到键盘已打开，需要隐藏键盘，再做后续操作...")
+            self.touch(v=temp)
+        else:
+            hw_keyword = self.poco(type="android.widget.ImageView", name="com.android.systemui:id/back", desc="返回")
+            if isinstance(hw_keyword, UIObjectProxy) and hw_keyword.exists():
+                logger.info("目前检测到HW键盘已经打开，需要隐藏键盘，再做后续操作...")
+                hw_keyword.click()
+            else:
+                lg_keyword = self.poco(type="com.lge.ime.humaninterface.inputview.layout.HIGColoredEnterKey",
+                                       name="完成")
+                if isinstance(lg_keyword, UIObjectProxy) and lg_keyword.exists():
+                    logger.info("目前检测到LG键盘已经打开，需要隐藏键盘，再做后续操作...")
+                    lg_keyword.click()
+                else:
+                    logger.info("键盘已经隐藏，无需处理键盘...")
+
+    # 获取元素在屏幕上的绝对坐标
+    def get_abs_position(self, element: UIObjectProxy) -> t.Tuple:
+        screen_width, screen_height = get_screen_size_via_adb(device_id=self.device_id)
+        relative_position = element.get_position()
+        absolute_x = int(relative_position[0] * screen_width)
+        absolute_y = int(relative_position[1] * screen_height)
+        return absolute_x, absolute_y
+
+    # 快捷滑屏
+    def quick_slide_screen(self, duration: float = 0.5):
+        # 获取屏幕尺寸
+        screen_width, screen_height = get_screen_size_via_adb(device_id=self.device_id)
+        # 定义起始点和终止点坐标
+        start_x = screen_width // 2  # 屏幕中心点的横坐标
+        start_y = screen_height // 2  # 屏幕中心点的纵坐标
+        end_x = start_x  # 横坐标保持不变
+        end_y = screen_height // 4  # 终止点纵坐标为屏幕顶部 1/4 处
+        # 执行滑动操作
+        self.swipe((start_x, start_y), (end_x, end_y), duration=duration)
+
+
+class PocoProxy(object):
+
+    def __init__(self):
+        self.poco = AndroidUiautomationPoco(
+            use_airtest_input=True, screenshot_each_action=False, force_restart=True
+        )
+
     def get_po(self, type: str, name: str = '', text: str = '', desc: str = '', textMatches: str = '') -> UIObjectProxy:
         kwargs = dict()
         if type:
             kwargs["type"] = type
         if name:
             kwargs["name"] = name
         if text:
@@ -518,48 +565,7 @@
             zOrders = i.attr("zOrders")
             touchable_raw = i.attr("touchable")
             # pprint(get_ui_object_proxy_attr(ui_object_proxy=i))
             if zOrders.get("global") == global_num and zOrders.get("local") == local_num and touchable_raw == touchable:
                 # pprint(get_ui_object_proxy_attr(ui_object_proxy=i))
                 po_list.append(i)
         return po_list
-
-    @airtest_exception_format
-    def hide_keyword(self, file_name: str) -> None:
-        temp = self.get_cv_template(file_name=file_name)
-        hide_icon = self.find_all(v=temp)
-        if len(hide_icon) > 0:
-            logger.info("目前检测到键盘已打开，需要隐藏键盘，再做后续操作...")
-            self.touch(v=temp)
-        else:
-            hw_keyword = self.poco(type="android.widget.ImageView", name="com.android.systemui:id/back", desc="返回")
-            if hw_keyword.exists():
-                logger.info("目前检测到HW键盘已经打开，需要隐藏键盘，再做后续操作...")
-                hw_keyword.click()
-            else:
-                lg_keyword = self.poco(type="com.lge.ime.humaninterface.inputview.layout.HIGColoredEnterKey",
-                                       name="完成")
-                if lg_keyword.exists():
-                    logger.info("目前检测到LG键盘已经打开，需要隐藏键盘，再做后续操作...")
-                    lg_keyword.click()
-                else:
-                    logger.info("键盘已经隐藏，无需处理键盘...")
-
-    # 获取元素在屏幕上的绝对坐标
-    def get_abs_position(self, element: AndroidUiautomationPoco) -> t.Tuple:
-        screen_width, screen_height = get_screen_size_via_adb(device_id=self.device_id)
-        relative_position = element.get_position()
-        absolute_x = int(relative_position[0] * screen_width)
-        absolute_y = int(relative_position[1] * screen_height)
-        return absolute_x, absolute_y
-
-    # 快捷滑屏
-    def quick_slide_screen(self, duration: float = 0.5):
-        # 获取屏幕尺寸
-        screen_width, screen_height = get_screen_size_via_adb(device_id=self.device_id)
-        # 定义起始点和终止点坐标
-        start_x = screen_width // 2  # 屏幕中心点的横坐标
-        start_y = screen_height // 2  # 屏幕中心点的纵坐标
-        end_x = start_x  # 横坐标保持不变
-        end_y = screen_height // 4  # 终止点纵坐标为屏幕顶部 1/4 处
-        # 执行滑动操作
-        self.swipe((start_x, start_y), (end_x, end_y), duration=duration)
```

### Comparing `ctrip-app-ui-0.4.2/capp_ui/platforms.py` & `ctrip-app-ui-0.4.3/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/test.py` & `ctrip-app-ui-0.4.3/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/utils.py` & `ctrip-app-ui-0.4.3/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/capp_ui/validators.py` & `ctrip-app-ui-0.4.3/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.2/setup.py` & `ctrip-app-ui-0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.4.2'
-            '',
+    version='0.4.3',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

