# Comparing `tmp/auterion-cli-1.7.0.tar.gz` & `tmp/auterion-cli-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.7.0.tar", last modified: Fri Apr 12 09:33:54 2024, max compression
+gzip compressed data, was "auterion-cli-1.7.1.tar", last modified: Mon May 13 12:55:41 2024, max compression
```

## Comparing `auterion-cli-1.7.0.tar` & `auterion-cli-1.7.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 09:33:53.000000 auterion-cli-1.7.0/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.624145 auterion-cli-1.7.0/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.624145 auterion-cli-1.7.0/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_inspect_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9751 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4407 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 12:55:40.000000 auterion-cli-1.7.1/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.562714 auterion-cli-1.7.1/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 12:55:41.000000 auterion-cli-1.7.1/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.562714 auterion-cli-1.7.1/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.562714 auterion-cli-1.7.1/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_inspect_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11456 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4407 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:55:41.566714 auterion-cli-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-13 12:55:31.000000 auterion-cli-1.7.1/setup.py
```

### Comparing `auterion-cli-1.7.0/README.md` & `auterion-cli-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.7.1/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_command.py` & `auterion-cli-1.7.1/auterioncli/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-1.json` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-1.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-2.json` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-2.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_inspect_command.py` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_inspect_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/slimify.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.7.1/auterioncli/commands/app_sdk/update.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #! /usr/bin/env python3
 import argparse
 import os
+import signal
 import sys
 
 import requests
 import time
 import enum
 from datetime import datetime
 try:
@@ -38,14 +39,44 @@
             # The version route is not implemented in v1.0
             return "v1.0"
         else:
             return None
     except:
         return None
 
+def cancel_update(url):
+    print("Cancelling update...")
+    try:
+        response = requests.post(f"{url}/rollback")
+        if response.status_code == 200:
+            print("Update cancellation requested...")
+        elif response.status_code == 404:
+            print("Cancellation endpoint not found for your current AOS version: update will proceed on the connected device.")
+            sys.exit(0)
+        else:
+            print(f"Cancel request received response: {response}")
+            sys.exit(0)
+    except Exception as e:
+        print(f"Failed to send cancel update request: {e}")
+        sys.exit(0)
+
+    is_final_state = False
+    while(not is_final_state):
+        is_final_state, code, _, _ = get_device_status(url, verbose=False)
+        time.sleep(0.1)
+
+    if code == ExitCode.CANCELLED:
+        print("Update cancelled successfully")
+    elif code == ExitCode.SUCCESS:
+        print("Update completed succesfully before cancellation triggered")
+    else:
+        print(f"Update finished with code: {code}. Exiting.")
+
+    sys.exit(0)
+
 def refresh_progress_bar(monitor):
     if monitor.finished:
         return
     if monitor.last_bytes_read is None:
         monitor.progress_bar.update(monitor.bytes_read)
     else:
         monitor.progress_bar.update(monitor.bytes_read-monitor.last_bytes_read)
@@ -53,21 +84,29 @@
     percentage = float(monitor.last_bytes_read) / float(monitor.total_size)
     if percentage > 1.0:
         monitor.finished = True
         monitor.progress_bar.close()
         print("Waiting for the device to complete the installation")
 
 def upload_artifact(url, file_path, cookies, extra_headers):
-    e = MultipartEncoder(fields={'file': (None, open(file_path,"rb"), 'application/octet-stream')})
+    filename = os.path.basename(file_path) or "unknown.auterionos"
+    e = MultipartEncoder(fields={'file': (filename, open(file_path,"rb"), 'application/octet-stream')})
     m = MultipartEncoderMonitor(e, refresh_progress_bar)
     m.last_bytes_read = None
     m.total_size = os.path.getsize(file_path)
     m.progress_bar = tqdm(desc="Uploading artifact", unit_scale=True, total=m.total_size)
     m.finished = False
     try:
+        if not extra_headers:
+            extra_headers = {}
+        extra_headers['Content-Type'] = m.content_type
+
+        # Request update cancellation on user interrupt 
+        signal.signal(signal.SIGINT, lambda signal, frame: cancel_update(url))
+        
         response = requests.post("{}/update".format(url), data=m, cookies=cookies, headers=extra_headers)
         if 400 <= response.status_code < 500:
             print("Not authenticated to perform this action", file=sys.stderr)
             print("Log into the device with 'auterion device login' first.", file=sys.stderr)
             exit(1)
         if response:
             data = response.json()
@@ -105,15 +144,51 @@
         try:
             if requests.get("{}/v1.0/ping".format(url)):
                 return True
         except:
             return False
     return False
 
-def get_device_status(url, reboot_counter=0, last_status=None):
+def print_device_status(status):
+    if status == "INSTALLING":
+        print("Waiting for the device to complete the installation")
+    elif status == "INSTALLED":
+        print("Waiting for the device to reboot")
+    elif status == "REBOOTING":
+        print("Device is rebooting")
+    elif status == "REBOOTED":
+        print("Device rebooted")
+    elif status == "VERIFICATION":
+        print("Update verification")
+    elif status == "FMU_UPDATE":
+        print("Update FMU")
+    elif status == "FMU_UPDATE_SUCCEED":
+        print("FMU updated successfully")
+    elif status == "CUSTOM_APP_INSTALL":
+        print("Installing custom apps")
+    elif status == "FMU_UPDATE_FAILED":
+        print("FMU update failed")
+    elif status == "REPARTITIONING":
+        print("Device is being repartitioned")
+    elif status == "SUCCEED":
+        print("The device has been updated successfully")
+    elif status == "APP_INSTALL_SUCCEED":
+        print("Application has been installed successfully")
+    elif status == "APP_INSTALL_FAILED":
+        print("Application installation failed.")
+    elif status == "FAILED":
+        print("Update verification failed. The system has been rollbacked")
+    elif status == "NEED_POWER_CYCLE":
+        print("The device has been updated successfully, you need to powercycle your drone to complete the update.")
+    elif status == "CANCELLED":
+        print("Update has been cancelled")
+    elif status == "INVALID_ARTIFACT":
+        print("Update has been cancelled: Artifact is invalid")
+
+def get_device_status(url, reboot_counter=0, last_status=None, verbose=True):
     status = None
     try:
         response = requests.get("{}/status".format(url), timeout=1)
 
         if response.status_code == 404:
             return False, ExitCode.REQUEST_API_VERSION, None, reboot_counter
 
@@ -131,56 +206,33 @@
     # if status == "UPLOADING":
     #     # We do nothing
     code = None
     if last_status != status:
         if last_status == "REBOOTING":
             # Force to request the API
             return False, ExitCode.REQUEST_API_VERSION, None, reboot_counter
-        if status == "INSTALLING":
-            print("Waiting for the device to complete the installation")
-        elif status == "INSTALLED":
-            print("Waiting for the device to reboot")
-        elif status == "REBOOTING":
-            print("Device is rebooting")
-        elif status == "REBOOTED":
-            print("Device rebooted")
-        elif status == "VERIFICATION":
-            print("Update verification")
-        elif status == "FMU_UPDATE":
-            print("Update FMU")
-        elif status == "FMU_UPDATE_SUCCEED":
-            print("FMU updated successfully")
-        elif status == "CUSTOM_APP_INSTALL":
-            print("Installing custom apps")
         elif status == "FMU_UPDATE_FAILED":
-            print("FMU update failed")
             code = ExitCode.FMU_UPDATE_FAILED
-        elif status == "REPARTITIONING":
-            print("Device is being repartitioned")
         elif status == "SUCCEED":
-            print("The device has been updated successfully")
             code = ExitCode.SUCCESS
         elif status == "APP_INSTALL_SUCCEED":
-            print("Application has been installed successfully")
             code = ExitCode.SUCCESS
         elif status == "APP_INSTALL_FAILED":
-            print("Application installation failed.")
             code = ExitCode.UPDATE_FAILED
         elif status == "FAILED":
-            print("Update verification failed. The system has been rollbacked")
             code = ExitCode.UPDATE_FAILED
         elif status == "NEED_POWER_CYCLE":
-            print("The device has been updated successfully, you need to powercycle your drone to complete the update.")
             code = ExitCode.SUCCESS
         elif status == "CANCELLED":
-            print("Update has been cancelled")
             code = ExitCode.CANCELLED
         elif status == "INVALID_ARTIFACT":
-            print("Update has been cancelled: Artifact is invalid")
             code = ExitCode.INVALID_ARTIFACT
+        if verbose:
+            print_device_status(status)
+
     return code != None, code, status, reboot_counter
 
 def update_failed(message, url):
     _, code, _, _ = get_device_status(url)
     print(message)
     if code == None:
         code = ExitCode.UPDATE_FAILED
```

### Comparing `auterion-cli-1.7.0/auterioncli/commands/container_command.py` & `auterion-cli-1.7.1/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/device_command.py` & `auterion-cli-1.7.1/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/info_command.py` & `auterion-cli-1.7.1/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/report_command.py` & `auterion-cli-1.7.1/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/commands/utils.py` & `auterion-cli-1.7.1/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/main.py` & `auterion-cli-1.7.1/auterioncli/main.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/auterioncli/meta_util.py` & `auterion-cli-1.7.1/auterioncli/meta_util.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.7.0/setup.py` & `auterion-cli-1.7.1/setup.py`

 * *Files identical despite different names*

