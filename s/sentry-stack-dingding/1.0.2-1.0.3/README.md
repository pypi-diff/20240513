# Comparing `tmp/sentry-stack-dingding-1.0.2.tar.gz` & `tmp/sentry-stack-dingding-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentry-stack-dingding-1.0.2.tar", last modified: Mon May 13 03:35:14 2024, max compression
+gzip compressed data, was "dist/sentry-stack-dingding-1.0.3.tar", last modified: Mon May 13 04:26:33 2024, max compression
```

## Comparing `sentry-stack-dingding-1.0.2.tar` & `sentry-stack-dingding-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       38 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/setup.cfg
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      996 2024-05-13 03:33:44.000000 sentry-stack-dingding-1.0.2/setup.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      774 2024-05-13 03:32:44.000000 sentry-stack-dingding-1.0.2/README.md
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/PKG-INFO
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      453 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/SOURCES.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       16 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/top_level.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/dependency_links.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/PKG-INFO
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       74 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/entry_points.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/not-zip-safe
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       23 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/requires.txt
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_dingding/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     2631 2024-05-13 03:26:25.000000 sentry-stack-dingding-1.0.2/src/sentry_dingding/plugin.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       35 2024-05-13 03:34:24.000000 sentry-stack-dingding-1.0.2/src/sentry_dingding/__init__.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      320 2024-05-13 02:34:05.000000 sentry-stack-dingding-1.0.2/src/sentry_dingding/forms.py
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       38 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/setup.cfg
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1044 2024-05-13 04:26:29.000000 sentry-stack-dingding-1.0.3/setup.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      774 2024-05-13 03:32:44.000000 sentry-stack-dingding-1.0.3/README.md
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/PKG-INFO
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/src/
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/src/sentry_stack_dingding.egg-info/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      453 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/src/sentry_stack_dingding.egg-info/SOURCES.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       16 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/src/sentry_stack_dingding.egg-info/top_level.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/src/sentry_stack_dingding.egg-info/dependency_links.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/src/sentry_stack_dingding.egg-info/PKG-INFO
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       74 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/src/sentry_stack_dingding.egg-info/entry_points.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.3/src/sentry_stack_dingding.egg-info/not-zip-safe
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       23 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/src/sentry_stack_dingding.egg-info/requires.txt
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 04:26:33.000000 sentry-stack-dingding-1.0.3/src/sentry_dingding/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     2650 2024-05-13 04:25:48.000000 sentry-stack-dingding-1.0.3/src/sentry_dingding/plugin.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       35 2024-05-13 04:25:55.000000 sentry-stack-dingding-1.0.3/src/sentry_dingding/__init__.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      320 2024-05-13 02:34:05.000000 sentry-stack-dingding-1.0.3/src/sentry_dingding/forms.py
```

### Comparing `sentry-stack-dingding-1.0.2/setup.py` & `sentry-stack-dingding-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
+from src import sentry_dingding
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="sentry-stack-dingding",
-    version='1.0.2',
+    version=sentry_dingding.VERSION,
     author='wilson-loo',
     author_email='614231319@qq.com',
     url='https://github.com/wilsonloo/sentry-stack-dingding.git',
     description='A Sentry extension which send errors stats to DingDing',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

### Comparing `sentry-stack-dingding-1.0.2/README.md` & `sentry-stack-dingding-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sentry-stack-dingding-1.0.2/PKG-INFO` & `sentry-stack-dingding-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-stack-dingding
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Sentry extension which send errors stats to DingDing
 Home-page: https://github.com/wilsonloo/sentry-stack-dingding.git
 Author: wilson-loo
 Author-email: 614231319@qq.com
 License: MIT
 Description: # Sentry-DingDing
```

### Comparing `sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/PKG-INFO` & `sentry-stack-dingding-1.0.3/src/sentry_stack_dingding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-stack-dingding
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Sentry extension which send errors stats to DingDing
 Home-page: https://github.com/wilsonloo/sentry-stack-dingding.git
 Author: wilson-loo
 Author-email: 614231319@qq.com
 License: MIT
 Description: # Sentry-DingDing
```

### Comparing `sentry-stack-dingding-1.0.2/src/sentry_dingding/plugin.py` & `sentry-stack-dingding-1.0.3/src/sentry_dingding/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class DingDingPlugin(NotificationPlugin):
     """
     Sentry plugin to send error counts to DingDing.
     """
     author = 'wilson-loo'
     author_url = 'https://github.com/wilsonloo/sentry-stack-dingding'
     version = sentry_dingding.VERSION
-    description = 'Send error counts to DingDing.'
+    description = 'Send error counts to DingDing with stack preview'
     resource_links = [
         ('Source', 'https://github.com/wilsonloo/sentry-stack-dingding.git'),
         ('Bug Tracker', 'https://github.com/wilsonloo/sentry-stack-dingding.git/issues'),
         ('README', 'https://github.com/wilsonloo/sentry-stack-dingding.git/blob/master/README.md'),
     ]
 
     slug = 'DingDing'
@@ -52,15 +52,15 @@
 
         access_token = self.get_option('access_token', group.project)
         send_url = DingTalk_API.format(token=access_token)
         title = u'【%s】的项目异常' % event.project.slug
 
         # splice stack
         stackDeep=self.get_option('stack_deep', group.project)
-        stack=event.stack or ""
+        stack=event.frames or ""
         stack_lines = stack.split('\n')
         selected_stack_lines = stack_lines[:stackDeep]
         stack = '\n'.join(selected_stack_lines)
         
         data = {
             "msgtype": "markdown",
             "markdown": {
```

