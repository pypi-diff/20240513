# Comparing `tmp/sentry-stack-dingding-1.0.4.tar.gz` & `tmp/sentry-stack-dingding-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentry-stack-dingding-1.0.4.tar", last modified: Mon May 13 04:32:53 2024, max compression
+gzip compressed data, was "dist/sentry-stack-dingding-1.0.5.tar", last modified: Mon May 13 05:05:36 2024, max compression
```

## Comparing `sentry-stack-dingding-1.0.4.tar` & `sentry-stack-dingding-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       38 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/setup.cfg
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1044 2024-05-13 04:26:29.000000 sentry-stack-dingding-1.0.4/setup.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      774 2024-05-13 03:32:44.000000 sentry-stack-dingding-1.0.4/README.md
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/PKG-INFO
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/src/
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/src/sentry_stack_dingding.egg-info/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      453 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/src/sentry_stack_dingding.egg-info/SOURCES.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       16 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/src/sentry_stack_dingding.egg-info/top_level.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/src/sentry_stack_dingding.egg-info/dependency_links.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/src/sentry_stack_dingding.egg-info/PKG-INFO
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       74 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/src/sentry_stack_dingding.egg-info/entry_points.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.4/src/sentry_stack_dingding.egg-info/not-zip-safe
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       23 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/src/sentry_stack_dingding.egg-info/requires.txt
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 04:32:53.000000 sentry-stack-dingding-1.0.4/src/sentry_dingding/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     2637 2024-05-13 04:32:03.000000 sentry-stack-dingding-1.0.4/src/sentry_dingding/plugin.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       34 2024-05-13 04:32:49.000000 sentry-stack-dingding-1.0.4/src/sentry_dingding/__init__.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      320 2024-05-13 02:34:05.000000 sentry-stack-dingding-1.0.4/src/sentry_dingding/forms.py
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       38 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/setup.cfg
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1044 2024-05-13 04:26:29.000000 sentry-stack-dingding-1.0.5/setup.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      774 2024-05-13 03:32:44.000000 sentry-stack-dingding-1.0.5/README.md
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/PKG-INFO
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/src/
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/src/sentry_stack_dingding.egg-info/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      453 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/src/sentry_stack_dingding.egg-info/SOURCES.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       16 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/src/sentry_stack_dingding.egg-info/top_level.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/src/sentry_stack_dingding.egg-info/dependency_links.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/src/sentry_stack_dingding.egg-info/PKG-INFO
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       74 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/src/sentry_stack_dingding.egg-info/entry_points.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.5/src/sentry_stack_dingding.egg-info/not-zip-safe
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       23 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/src/sentry_stack_dingding.egg-info/requires.txt
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 05:05:36.000000 sentry-stack-dingding-1.0.5/src/sentry_dingding/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     2826 2024-05-13 05:05:21.000000 sentry-stack-dingding-1.0.5/src/sentry_dingding/plugin.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       34 2024-05-13 05:05:33.000000 sentry-stack-dingding-1.0.5/src/sentry_dingding/__init__.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      320 2024-05-13 02:34:05.000000 sentry-stack-dingding-1.0.5/src/sentry_dingding/forms.py
```

### Comparing `sentry-stack-dingding-1.0.4/setup.py` & `sentry-stack-dingding-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `sentry-stack-dingding-1.0.4/README.md` & `sentry-stack-dingding-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sentry-stack-dingding-1.0.4/PKG-INFO` & `sentry-stack-dingding-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-stack-dingding
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Sentry extension which send errors stats to DingDing
 Home-page: https://github.com/wilsonloo/sentry-stack-dingding.git
 Author: wilson-loo
 Author-email: 614231319@qq.com
 License: MIT
 Description: # Sentry-DingDing
```

### Comparing `sentry-stack-dingding-1.0.4/src/sentry_stack_dingding.egg-info/PKG-INFO` & `sentry-stack-dingding-1.0.5/src/sentry_stack_dingding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-stack-dingding
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Sentry extension which send errors stats to DingDing
 Home-page: https://github.com/wilsonloo/sentry-stack-dingding.git
 Author: wilson-loo
 Author-email: 614231319@qq.com
 License: MIT
 Description: # Sentry-DingDing
```

### Comparing `sentry-stack-dingding-1.0.4/src/sentry_dingding/plugin.py` & `sentry-stack-dingding-1.0.5/src/sentry_dingding/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,17 +52,23 @@
 
         access_token = self.get_option('access_token', group.project)
         send_url = DingTalk_API.format(token=access_token)
         title = u'【%s】的项目异常' % event.project.slug
 
         # splice stack
         stackDeep=self.get_option('stack_deep', group.project)
-        stack = ""
-        if event.frames and len(event.frames) > 0:
-            stack = event.frames[:stackDeep]
+        if event.data:
+            if event.data["frames"]:
+                stack = event.data["frames"]
+            if event.data["stack"]:
+                stack = event.data["stack"]
+
+        if stack:
+        # if event.frames and len(event.frames) > 0:
+        #     stack = event.frames[:stackDeep]
             stack = json.dumps(stack, indent=2)
         
         data = {
             "msgtype": "markdown",
             "markdown": {
                 "title": title,
                 "text": u"#### {title} \n\n > {message} \n\n {stack} \n\n [详细信息]({url})".format(
```

