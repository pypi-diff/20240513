# Comparing `tmp/taskflows-0.4.3-py3-none-any.whl.zip` & `tmp/taskflows-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23801 bytes, number of entries: 16
+Zip file size: 23894 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx       87 b- defN 24-Feb-15 20:59 taskflows/__init__.py
--rw-rw-r--  2.0 unx    10110 b- defN 24-May-02 17:22 taskflows/admin.py
+-rw-rw-r--  2.0 unx    10229 b- defN 24-May-07 20:34 taskflows/admin.py
 -rw-rw-r--  2.0 unx     3444 b- defN 24-May-01 00:36 taskflows/db.py
 -rw-rw-r--  2.0 unx     8937 b- defN 24-Mar-05 14:35 taskflows/tasks.py
 -rw-rw-r--  2.0 unx      564 b- defN 24-Feb-12 20:43 taskflows/utils.py
 -rwxrwxr-x  2.0 unx      587 b- defN 24-May-02 17:22 taskflows/service/__init__.py
 -rwxrwxr-x  2.0 unx     1286 b- defN 24-Feb-29 14:30 taskflows/service/commands.py
 -rwxrwxr-x  2.0 unx     1586 b- defN 24-Feb-12 20:43 taskflows/service/constraints.py
 -rw-rw-r--  2.0 unx    18204 b- defN 24-Apr-22 18:48 taskflows/service/docker.py
 -rwxrwxr-x  2.0 unx     2234 b- defN 24-Feb-12 20:43 taskflows/service/schedule.py
--rwxrwxr-x  2.0 unx    18155 b- defN 24-Apr-29 23:57 taskflows/service/service.py
--rw-rw-r--  2.0 unx     4093 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx      111 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1294 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/RECORD
-16 files, 70794 bytes uncompressed, 21679 bytes compressed:  69.4%
+-rwxrwxr-x  2.0 unx    18155 b- defN 24-May-07 19:56 taskflows/service/service.py
+-rw-rw-r--  2.0 unx     4293 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      111 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1294 b- defN 24-May-13 18:06 taskflows-0.4.4.dist-info/RECORD
+16 files, 71113 bytes uncompressed, 21772 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: taskflows/service/schedule.py
 Comment: 
 
 Filename: taskflows/service/service.py
 Comment: 
 
-Filename: taskflows-0.4.3.dist-info/METADATA
+Filename: taskflows-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: taskflows-0.4.3.dist-info/WHEEL
+Filename: taskflows-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: taskflows-0.4.3.dist-info/entry_points.txt
+Filename: taskflows-0.4.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: taskflows-0.4.3.dist-info/top_level.txt
+Filename: taskflows-0.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: taskflows-0.4.3.dist-info/RECORD
+Filename: taskflows-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## taskflows/admin.py

```diff
@@ -1,13 +1,14 @@
 import re
 import subprocess
 from functools import lru_cache
 from itertools import cycle
 from pprint import pformat, pprint
 from typing import Optional, Tuple
+from collections import defaultdict
 
 import click
 import sqlalchemy as sa
 from click.core import Group
 from dynamic_imports import import_module
 from rich import box
 from rich.console import Console
@@ -283,24 +284,25 @@
     remove_service(service)
     click.echo(click.style("Done!", fg="green"))
 
 
 @cli.command
 @click.argument("service", required=False)
 def show(service: str):
-    services = []
+    files = defaultdict(list)
+    for f in systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}*.service"):
+        files[f.stem].append(f)
+    for f in systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}*.timer"):
+        files[f.stem].append(f)
     if service:
-        if not service.startswith(_SYSTEMD_FILE_PREFIX):
-            service = _SYSTEMD_FILE_PREFIX+service
-        if not service.endswith('.service'):
-            service += '.service'
-        services = [service]
-    else:
-        services = list(systemd_dir.glob('*.service'))
-    services = "\n\n".join([s.read_text() for s in services])
+        files = {k: v for k, v in files.items() if service in k}
+    services = []
+    for srvs in files.values():
+        services.append('\n'.join([s.read_text() for s in srvs]))
+    services = "\n\n".join(services)
     click.echo(click.style(services, fg="cyan"))
 
 
 def table_column_colors():
     colors_gen = cycle(["orange3", "green", "cyan", "magenta", "dodger_blue1", "red"])
 
     @lru_cache
```

## Comparing `taskflows-0.4.3.dist-info/METADATA` & `taskflows-0.4.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 Metadata-Version: 2.1
 Name: taskflows
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python task management, scheduling, alerts.
 Author-email: Dan Kelleher <kelleherjdan@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: sqlalchemy >=2.0.0
 Requires-Dist: pydantic >=2.0.0
 Requires-Dist: tqdm
 Requires-Dist: click
-Requires-Dist: python-dotenv
 Requires-Dist: rich
 Requires-Dist: dynamic-imports >=1.0.0
 Requires-Dist: alert-msgs >=0.5.0
 Requires-Dist: quicklogs >=1.1.0
 Requires-Dist: func-timeout >=4.0.0
-Requires-Dist: docker
-Requires-Dist: dbus-python
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-asyncio ; extra == 'dev'
 Requires-Dist: psycopg[binary] ; extra == 'dev'
+Provides-Extra: service
+Requires-Dist: python-dotenv ; extra == 'service'
+Requires-Dist: docker ; extra == 'service'
+Requires-Dist: dbus-python ; extra == 'service'
 
 
 # Task Management, Scheduling, and Alerting.
 
 Admin commands are accessed via the `taskflows` command line tool. See `taskflows --help` for complete usage.  
 
 ### Setup
+For task decorators:
 ```bash
-sudo apt install libdbus-glib-1-dev
-loginctl enable-linger
 pip install taskflows
 ``` 
+For additional service/scheduling functionality:
+```bash
+sudo apt install libdbus-glib-1-dev
+loginctl enable-linger
+pip install taskflows[service]
+```
 
 Task execution metadata is stored in SQLite (default) or Postgresql. To use a personal database, set environment variable `TASKFLOWS_DB_URL` to your database URL. If using Postgresql, TASKFLOWS_DB_SCHEMA may also be set to use a custom schema (default schema is *taskflows*).   
 
 ### Create Tasks
 Turn any function (optionally async) into a task that logs metadata to the database and sends alerts, allows retries, etc..
 ```python
 alerts=[
```

## Comparing `taskflows-0.4.3.dist-info/RECORD` & `taskflows-0.4.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 taskflows/__init__.py,sha256=oW-FCpGdoTfDXFNZ7hlNV2lzLUzQoKSPTP2TfvDIPPk,87
-taskflows/admin.py,sha256=1errDFcld0SB3Um1KIHKjRPYhYP_ZXoTcrCczZE9Uko,10110
+taskflows/admin.py,sha256=dXtzOrR4zFdFdpjHlZS3Gb8_HWS_Lo2CxAIKIZn38vU,10229
 taskflows/db.py,sha256=aOoWhuy1__7YobfP0bB1x-sTFEjoSM06Kdw1m6--GWc,3444
 taskflows/tasks.py,sha256=aXQxLu6_JItg5iqQpZDDYLaJKIvbI5B17_rLWQGWJFk,8937
 taskflows/utils.py,sha256=TahZKvotnW_us79SXYkjrjXoa464MwHFe6uo5SR0XuI,564
 taskflows/service/__init__.py,sha256=Epl-nKhfYN7Qn69PBBH8mvxXgYVJBywvIAcIFUK8Su8,587
 taskflows/service/commands.py,sha256=t_ITtM5l5_Dtpx70p6uKBaWGixGkNZCYm13zXBlQkQw,1286
 taskflows/service/constraints.py,sha256=2N5eSAJjUg2twxmVjs3GWaqmppc-DW0dZ5MlMRqcmNw,1586
 taskflows/service/docker.py,sha256=w2VFWPCcAd5hLqkOamfdJuPagT_qeB4tBqVoFnGw5Rc,18204
 taskflows/service/schedule.py,sha256=84B5phVhjSoj-UTtmqHmVwKTHYVjjfuryYW3p4yuJco,2234
 taskflows/service/service.py,sha256=_tKef13I2Ge3qPF3WgJprVFAaxDxnPciCC6fMPuo2iY,18155
-taskflows-0.4.3.dist-info/METADATA,sha256=c44Ca9B-QAZjeC741_0-L7Zqduff0b8oENKKvfQpUmU,4093
-taskflows-0.4.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-taskflows-0.4.3.dist-info/entry_points.txt,sha256=84ElXyA0XQ3cRfNIL-woPCmCkGk9-OV4YarSW0i-88Y,111
-taskflows-0.4.3.dist-info/top_level.txt,sha256=CipuamG5azL_xisU7bxm8aEd18vy0JSHVWx4WzswtqQ,10
-taskflows-0.4.3.dist-info/RECORD,,
+taskflows-0.4.4.dist-info/METADATA,sha256=wH6QlfidgfcQ-2XEz2aYyGGMSKCUX48TTdeiB0C9xO0,4293
+taskflows-0.4.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+taskflows-0.4.4.dist-info/entry_points.txt,sha256=84ElXyA0XQ3cRfNIL-woPCmCkGk9-OV4YarSW0i-88Y,111
+taskflows-0.4.4.dist-info/top_level.txt,sha256=CipuamG5azL_xisU7bxm8aEd18vy0JSHVWx4WzswtqQ,10
+taskflows-0.4.4.dist-info/RECORD,,
```

