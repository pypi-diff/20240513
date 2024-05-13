# Comparing `tmp/hscloud-0.0.0.4.tar.gz` & `tmp/hscloud-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.0.4.tar", last modified: Sat May 11 11:09:49 2024, max compression
+gzip compressed data, was "hscloud-0.0.0.5.tar", last modified: Mon May 13 02:00:01 2024, max compression
```

## Comparing `hscloud-0.0.0.4.tar` & `hscloud-0.0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 11:09:49.512112 hscloud-0.0.0.4/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.4/LICENSE
--rw-rw-rw-   0        0        0      432 2024-05-11 11:09:49.510113 hscloud-0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 11:09:49.491114 hscloud-0.0.0.4/hscloud/
--rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.4/hscloud/__init__.py
--rw-rw-rw-   0        0        0     3653 2024-05-09 07:55:39.000000 hscloud-0.0.0.4/hscloud/helpers.py
--rw-rw-rw-   0        0        0     1052 2024-05-11 11:09:24.000000 hscloud-0.0.0.4/hscloud/hscloud.py
-drwxrwxrwx   0        0        0        0 2024-05-11 11:09:49.509113 hscloud-0.0.0.4/hscloud.egg-info/
--rw-rw-rw-   0        0        0      432 2024-05-11 11:09:49.000000 hscloud-0.0.0.4/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-11 11:09:49.000000 hscloud-0.0.0.4/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 11:09:49.000000 hscloud-0.0.0.4/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-11 11:09:49.000000 hscloud-0.0.0.4/hscloud.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-11 11:09:49.000000 hscloud-0.0.0.4/hscloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-11 11:09:49.000000 hscloud-0.0.0.4/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 11:09:49.512112 hscloud-0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      887 2024-05-11 11:07:26.000000 hscloud-0.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:00:01.459643 hscloud-0.0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      432 2024-05-13 02:00:01.457642 hscloud-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 02:00:01.440642 hscloud-0.0.0.5/hscloud/
+-rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.5/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     3653 2024-05-09 07:55:39.000000 hscloud-0.0.0.5/hscloud/helpers.py
+-rw-rw-rw-   0        0        0      953 2024-05-13 01:58:22.000000 hscloud-0.0.0.5/hscloud/hscloud.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:00:01.455642 hscloud-0.0.0.5/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      432 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:00:01.459643 hscloud-0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      887 2024-05-13 01:58:47.000000 hscloud-0.0.0.5/setup.py
```

### Comparing `hscloud-0.0.0.4/README.md` & `hscloud-0.0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.0.4/hscloud/helpers.py` & `hscloud-0.0.0.5/hscloud/helpers.py`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.0.4/hscloud/hscloud.py` & `hscloud-0.0.0.5/hscloud/hscloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,13 +20,9 @@
 
     def get_devices(self) -> tuple:
         return Helpers.devices(self.endpoint, self.access_token)
 
     def get_status(self, devicesn) -> tuple:
         return Helpers.status(self.endpoint, self.access_token, devicesn)
 
-    def update_status(self, devicesn, **kwargs) -> bool:
-        response = Helpers.update(self.endpoint, self.access_token, devicesn, **kwargs)
-        if response[0] == 0:
-            return True
-        else:
-            return False
+    def update_status(self, devicesn, **kwargs) -> tuple:
+        return Helpers.update(self.endpoint, self.access_token, devicesn, **kwargs)
```

### Comparing `hscloud-0.0.0.4/setup.py` & `hscloud-0.0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'hscloud',
     packages = ['hscloud'],
     include_package_data=True,
-    version = '0.0.0.4',
+    version = '0.0.0.5',
     license='MIT',
     description = 'Library to login to Dreo cloud and get device info.',
     author = 'Kane Wang',
     author_email = 'app@hesung.com',
     url = 'https://github.com/dreo-team/hscloud',
     download_url = 'https://github.com/dreo-team/hscloud/dist/hscloud-0.0.11.tar.gz',
     install_requires=[
```

