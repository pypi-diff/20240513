# Comparing `tmp/ctrip-app-ui-0.4.1.tar.gz` & `tmp/ctrip-app-ui-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.4.1.tar", last modified: Sun May 12 15:53:34 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.4.2.tar", last modified: Sun May 12 18:04:19 2024, max compression
```

## Comparing `ctrip-app-ui-0.4.1.tar` & `ctrip-app-ui-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 15:53:34.943981 ctrip-app-ui-0.4.1/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.1/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-12 15:53:34.941986 ctrip-app-ui-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 15:53:34.929021 ctrip-app-ui-0.4.1/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.1/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.1/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.1/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.1/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.1/capp_ui/dir.py
--rw-rw-rw-   0        0        0    63998 2024-05-12 15:52:49.000000 ctrip-app-ui-0.4.1/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.1/capp_ui/fee.py
--rw-rw-rw-   0        0        0     3859 2024-05-11 16:34:35.000000 ctrip-app-ui-0.4.1/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24704 2024-05-11 03:15:13.000000 ctrip-app-ui-0.4.1/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.1/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.1/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.1/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.1/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:53:34.940989 ctrip-app-ui-0.4.1/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-12 15:53:34.000000 ctrip-app-ui-0.4.1/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-12 15:53:34.000000 ctrip-app-ui-0.4.1/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 15:53:34.000000 ctrip-app-ui-0.4.1/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-12 15:53:34.000000 ctrip-app-ui-0.4.1/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-12 15:53:34.000000 ctrip-app-ui-0.4.1/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 15:53:34.943981 ctrip-app-ui-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1103 2024-05-12 15:53:28.000000 ctrip-app-ui-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:04:19.722674 ctrip-app-ui-0.4.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-12 18:04:19.720684 ctrip-app-ui-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 18:04:19.709686 ctrip-app-ui-0.4.2/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.2/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.2/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.2/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.2/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.2/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    64496 2024-05-12 18:03:38.000000 ctrip-app-ui-0.4.2/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.2/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     3859 2024-05-11 16:34:35.000000 ctrip-app-ui-0.4.2/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24664 2024-05-12 17:54:06.000000 ctrip-app-ui-0.4.2/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.2/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.2/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.2/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.2/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:04:19.719659 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-12 18:04:19.000000 ctrip-app-ui-0.4.2/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 18:04:19.722674 ctrip-app-ui-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2024-05-12 18:04:14.000000 ctrip-app-ui-0.4.2/setup.py
```

### Comparing `ctrip-app-ui-0.4.1/LICENSE` & `ctrip-app-ui-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/config.py` & `ctrip-app-ui-0.4.2/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/date_extend.py` & `ctrip-app-ui-0.4.2/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/device.py` & `ctrip-app-ui-0.4.2/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/dir.py` & `ctrip-app-ui-0.4.2/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/domain_service.py` & `ctrip-app-ui-0.4.2/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1160,30 +1160,39 @@
     # @SleepWait(wait_time=1)
     def select_more_payment(self) -> bool:
         """
         当【同意并支付】后，特殊情况下，会出现支付小弹框，这个时候需要先判断是否存在小框，如果存在，则切换到通用支付选择界面
         """
         flag = False
         try:
-            more_payment = self.device.get_po(type="android.widget.TextView", name="android.widget.TextView",
+            more_payment = self.device.get_po(type="android.view.ViewGroup", name="更多付款方式",
                                               text="更多付款方式")
             if more_payment.exists() is True:
                 more_payment.click()
-                logger.warning("小弹框选择【更多付款方式】.")
+                logger.warning("小弹框选择【更多付款方式】")
                 flag = True
         except (PocoNoSuchNodeException, Exception):
             try:
-                more_payment = self.device.get_po(type="android.view.ViewGroup", name="更多付款方式",
-                                                  text="更多付款方式")
-                if more_payment.exists() is True:
-                    more_payment.click()
-                    logger.warning("小弹框选择【更多付款方式】.")
-                    flag = True
-            except (PocoNoSuchNodeException, Exception):
-                logger.info("没有出现支付小弹框，请在通用支付选择界面操作.")
+                file_name = join_path([get_images_dir(), "更多付款方式.png"])
+                if is_exists(file_name):
+                    pos = self.device.exists(self.device.get_cv_template(file_name))
+                    if pos:
+                        self.device.touch(v=pos)
+                        logger.warning("小弹框选择【更多付款方式】")
+                        flag = True
+            except (Exception,):
+                try:
+                    more_payment = self.device.get_po(type="android.widget.TextView", name="android.widget.TextView",
+                                                      text="更多付款方式")
+                    if more_payment.exists() is True:
+                        more_payment.click()
+                        logger.warning("小弹框选择【更多付款方式】")
+                        flag = True
+                except (PocoNoSuchNodeException, Exception):
+                    logger.info("没有出现支付小弹框，请在通用支付选择界面操作.")
         return flag
 
     def __get_wallet_element(self) -> UIObjectProxy:
         return self.device.get_po(
             type="android.widget.TextView", name="android.widget.TextView", textMatches=r'^钱包.*'
         )
```

### Comparing `ctrip-app-ui-0.4.1/capp_ui/fee.py` & `ctrip-app-ui-0.4.2/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/libs.py` & `ctrip-app-ui-0.4.2/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.4.2/capp_ui/mobile_terminals.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import subprocess
 import typing as t
 from poco.proxy import UIObjectProxy
 # from airtest.cli.parser import cli_setup
 from airtest.utils.transform import TargetPos
 
 from poco.drivers.android.uiautomation import AndroidUiautomationPoco
-from airtest.core.api import auto_setup, device, Template, touch, find_all, connect_device
+from airtest.core.api import auto_setup, device, Template, touch, find_all, connect_device, exists
 
 from capp_ui.device import cli_setup
 from capp_ui.dir import get_project_path
 from capp_ui.libs import airtest_exception_format, logger
 
 iOS_PLATFORM = "iOS"
 DEFAULT_PLATFORM = "Android"  # Android、Windows、iOS
@@ -379,32 +379,31 @@
             # 你可以在每次查找目标失败时，指定一个回调函数
             # def notfound():
             #     print("No target found")
             # self.device.wait(Template(r"tpl1607510661400.png"), intervalfunc=notfound)
             result = self.dev.wait(v=v, timeout=timeout, interval=interval, intervalfunc=intervalfunc)
         return result or None
 
-    @airtest_exception_format
-    def exists(self, v: Template) -> t.Any:
+    def exists(self, v: Template) -> bool:
         """ "
         检查设备上是否存在给定目标
         v Template: 要检查的目标
         return: 如果未找到目标，则返回False，否则返回目标的坐标
         platform: Android, iOS, Windows
         """
-        result = None
+        result = False
         if self.platform in (DEFAULT_PLATFORM, WINDOWS_PLATFORM, iOS_PLATFORM):
             # if self.device.exists(Template(r"tpl1606822430589.png")):
             #    self.device.touch(Template(r"tpl1606822430589.png"))
             # 因为 exists() 会返回坐标，我们可以直接点击坐标来减少一次图像查找
             # pos = self.device.exists(Template(r"tpl1606822430589.png"))
             # if pos:
             #    self.device.touch(pos)
-            result = self.dev.exists(v=v)
-        return result or None
+            result = exists(v=v)
+        return result
 
     @airtest_exception_format
     def find_all(self, v: Template) -> t.List:
         """
         在设备屏幕上查找所有出现的目标并返回其坐标列表
         v Template: 寻找目标
         return list:  [{‘result’: (x, y), ‘rectangle’: ( (left_top, left_bottom, right_bottom, right_top) ), ‘
```

### Comparing `ctrip-app-ui-0.4.1/capp_ui/platforms.py` & `ctrip-app-ui-0.4.2/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/test.py` & `ctrip-app-ui-0.4.2/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/utils.py` & `ctrip-app-ui-0.4.2/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/capp_ui/validators.py` & `ctrip-app-ui-0.4.2/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.1/setup.py` & `ctrip-app-ui-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.4.1'
+    version='0.4.2'
             '',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
```

