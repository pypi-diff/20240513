# Comparing `tmp/sentry-stack-dingding-1.0.1.tar.gz` & `tmp/sentry-stack-dingding-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentry-stack-dingding-1.0.1.tar", last modified: Mon May 13 02:44:04 2024, max compression
+gzip compressed data, was "dist/sentry-stack-dingding-1.0.2.tar", last modified: Mon May 13 03:35:14 2024, max compression
```

## Comparing `sentry-stack-dingding-1.0.1.tar` & `sentry-stack-dingding-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       38 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/setup.cfg
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      996 2024-05-13 02:31:23.000000 sentry-stack-dingding-1.0.1/setup.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      478 2024-05-13 02:40:13.000000 sentry-stack-dingding-1.0.1/README.md
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1149 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/PKG-INFO
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/sentry_stack_dingding.egg-info/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      453 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/sentry_stack_dingding.egg-info/SOURCES.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       16 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/sentry_stack_dingding.egg-info/top_level.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/sentry_stack_dingding.egg-info/dependency_links.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1149 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/sentry_stack_dingding.egg-info/PKG-INFO
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       74 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/sentry_stack_dingding.egg-info/entry_points.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/sentry_stack_dingding.egg-info/not-zip-safe
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       23 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/sentry_stack_dingding.egg-info/requires.txt
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 02:44:04.000000 sentry-stack-dingding-1.0.1/src/sentry_dingding/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     2373 2024-05-13 02:38:02.000000 sentry-stack-dingding-1.0.1/src/sentry_dingding/plugin.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       35 2024-05-11 10:39:38.000000 sentry-stack-dingding-1.0.1/src/sentry_dingding/__init__.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      320 2024-05-13 02:34:05.000000 sentry-stack-dingding-1.0.1/src/sentry_dingding/forms.py
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       38 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/setup.cfg
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      996 2024-05-13 03:33:44.000000 sentry-stack-dingding-1.0.2/setup.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      774 2024-05-13 03:32:44.000000 sentry-stack-dingding-1.0.2/README.md
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/PKG-INFO
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      453 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/SOURCES.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       16 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/top_level.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/dependency_links.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/PKG-INFO
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       74 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/entry_points.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/not-zip-safe
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       23 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/requires.txt
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.2/src/sentry_dingding/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     2631 2024-05-13 03:26:25.000000 sentry-stack-dingding-1.0.2/src/sentry_dingding/plugin.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       35 2024-05-13 03:34:24.000000 sentry-stack-dingding-1.0.2/src/sentry_dingding/__init__.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      320 2024-05-13 02:34:05.000000 sentry-stack-dingding-1.0.2/src/sentry_dingding/forms.py
```

### Comparing `sentry-stack-dingding-1.0.1/setup.py` & `sentry-stack-dingding-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="sentry-stack-dingding",
-    version='1.0.1',
+    version='1.0.2',
     author='wilson-loo',
     author_email='614231319@qq.com',
     url='https://github.com/wilsonloo/sentry-stack-dingding.git',
     description='A Sentry extension which send errors stats to DingDing',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

### Comparing `sentry-stack-dingding-1.0.1/PKG-INFO` & `sentry-stack-dingding-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-stack-dingding
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Sentry extension which send errors stats to DingDing
 Home-page: https://github.com/wilsonloo/sentry-stack-dingding.git
 Author: wilson-loo
 Author-email: 614231319@qq.com
 License: MIT
 Description: # Sentry-DingDing
         
@@ -19,22 +19,35 @@
         'Event' object has no attribute 'id' 
         ```
         
         * feature-2:
         add stack preview in dingding
         
         ## 安装
-        
+        * requirement.txt 方式:
+        ```
+            sentry-stack-dingding
         ```
-        # requirement.txt
         
-        sentry-stack-dingding
+        * sentry/enhance-image.sh 方式
+        ```sh
+            # 在sentry/enhance-image.sh 添加 pip install sentry-stack-dingding
+            # 然后 sudo ./install.sh
         ```
         
-        docker-compose 安装的直接改成这个插件包就好了，如果帮你解决了问题，麻烦给个小星星.
+        * docker-compose 方式：直接改成这个插件包就好了
+        
+        如果帮你解决了问题，麻烦给个小星星.
+        
+        ## 构建
+        ```sh
+        python3 setup.py sdist bdist_wheel
+        twine upload --repository testpypi dist/*
+        twine upload --repository pypi dist/*
+        ```
         
         
 Keywords: sentry stack dingding
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `sentry-stack-dingding-1.0.1/src/sentry_stack_dingding.egg-info/PKG-INFO` & `sentry-stack-dingding-1.0.2/src/sentry_stack_dingding.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-stack-dingding
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Sentry extension which send errors stats to DingDing
 Home-page: https://github.com/wilsonloo/sentry-stack-dingding.git
 Author: wilson-loo
 Author-email: 614231319@qq.com
 License: MIT
 Description: # Sentry-DingDing
         
@@ -19,22 +19,35 @@
         'Event' object has no attribute 'id' 
         ```
         
         * feature-2:
         add stack preview in dingding
         
         ## 安装
-        
+        * requirement.txt 方式:
+        ```
+            sentry-stack-dingding
         ```
-        # requirement.txt
         
-        sentry-stack-dingding
+        * sentry/enhance-image.sh 方式
+        ```sh
+            # 在sentry/enhance-image.sh 添加 pip install sentry-stack-dingding
+            # 然后 sudo ./install.sh
         ```
         
-        docker-compose 安装的直接改成这个插件包就好了，如果帮你解决了问题，麻烦给个小星星.
+        * docker-compose 方式：直接改成这个插件包就好了
+        
+        如果帮你解决了问题，麻烦给个小星星.
+        
+        ## 构建
+        ```sh
+        python3 setup.py sdist bdist_wheel
+        twine upload --repository testpypi dist/*
+        twine upload --repository pypi dist/*
+        ```
         
         
 Keywords: sentry stack dingding
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `sentry-stack-dingding-1.0.1/src/sentry_dingding/plugin.py` & `sentry-stack-dingding-1.0.2/src/sentry_dingding/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,22 +50,29 @@
         if group.is_ignored():
             return
 
         access_token = self.get_option('access_token', group.project)
         send_url = DingTalk_API.format(token=access_token)
         title = u'【%s】的项目异常' % event.project.slug
 
+        # splice stack
+        stackDeep=self.get_option('stack_deep', group.project)
+        stack=event.stack or ""
+        stack_lines = stack.split('\n')
+        selected_stack_lines = stack_lines[:stackDeep]
+        stack = '\n'.join(selected_stack_lines)
+        
         data = {
             "msgtype": "markdown",
             "markdown": {
                 "title": title,
                 "text": u"#### {title} \n\n > {message} \n\n {stack} \n\n [详细信息]({url})".format(
                     title=title,
                     message=event.message or event.title,
-                    stack=event.stack or "",
+                    stack=stack,
                     url=u"{}events/{}/".format(group.get_absolute_url(), event.event_id),
                 )
             }
         }
         requests.post(
             url=send_url,
             headers={"Content-Type": "application/json"},
```

