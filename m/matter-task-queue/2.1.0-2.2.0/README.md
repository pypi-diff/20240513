# Comparing `tmp/matter_task_queue-2.1.0-py3-none-any.whl.zip` & `tmp/matter_task_queue-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8837 bytes, number of entries: 10
+Zip file size: 8753 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_task_queue/__about__.py
 -rw-r--r--  2.0 unx      327 b- defN 20-Feb-02 00:00 matter_task_queue/__init__.py
 -rw-r--r--  2.0 unx     1228 b- defN 20-Feb-02 00:00 matter_task_queue/base_task.py
 -rw-r--r--  2.0 unx     4032 b- defN 20-Feb-02 00:00 matter_task_queue/celery_config.py
 -rw-r--r--  2.0 unx     1020 b- defN 20-Feb-02 00:00 matter_task_queue/config.py
--rw-r--r--  2.0 unx     3232 b- defN 20-Feb-02 00:00 matter_task_queue/utils.py
-?rw-r--r--  2.0 unx     4808 b- defN 20-Feb-02 00:00 matter_task_queue-2.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_task_queue-2.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_task_queue-2.1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      859 b- defN 20-Feb-02 00:00 matter_task_queue-2.1.0.dist-info/RECORD
-10 files, 16795 bytes uncompressed, 7361 bytes compressed:  56.2%
+-rw-r--r--  2.0 unx     2861 b- defN 20-Feb-02 00:00 matter_task_queue/utils.py
+?rw-r--r--  2.0 unx     4808 b- defN 20-Feb-02 00:00 matter_task_queue-2.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_task_queue-2.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_task_queue-2.2.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      859 b- defN 20-Feb-02 00:00 matter_task_queue-2.2.0.dist-info/RECORD
+10 files, 16424 bytes uncompressed, 7277 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: matter_task_queue/config.py
 Comment: 
 
 Filename: matter_task_queue/utils.py
 Comment: 
 
-Filename: matter_task_queue-2.1.0.dist-info/METADATA
+Filename: matter_task_queue-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: matter_task_queue-2.1.0.dist-info/WHEEL
+Filename: matter_task_queue-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: matter_task_queue-2.1.0.dist-info/licenses/LICENSE
+Filename: matter_task_queue-2.2.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_task_queue-2.1.0.dist-info/RECORD
+Filename: matter_task_queue-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_task_queue/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "2.1.0"
+__version__ = "2.2.0"
```

## matter_task_queue/utils.py

```diff
@@ -1,14 +1,15 @@
-import warnings
-import logging
 import asyncio
+import logging
+import warnings
+
 from celery import current_app as current_celery_app
-from celery.signals import worker_process_init, worker_process_shutdown
+
+from .celery_config import CELERY_BEAT_CONFIG, build_celery_config
 from .config import Config
-from .celery_config import build_celery_config, CELERY_BEAT_CONFIG
 
 warnings.filterwarnings("ignore", "SelectableGroups dict interface")
 
 
 try:
     loop = asyncio.get_running_loop()
 except RuntimeError:
@@ -62,31 +63,20 @@
         resp = loop.run_until_complete(func(*args, **kwargs))
     finally:
         asyncio.set_event_loop(None)
     return resp
 
 
 def create_celery(
-    task_module_paths: [str],
+    task_module_paths: list[str],
     celery_beat_schedule: dict = None,
     create_dead_letter_queue=True,
 ):
+    # TODO pass celery app as an argument
+    # see "Breaking the chain" in https://docs.celeryq.dev/en/stable/userguide/application.html#id4
     celery_app = current_celery_app
     celery_app.conf.update(build_celery_config(create_dead_letter_queue))
     celery_app.conf.update(CELERY_BEAT_CONFIG)
     celery_app.conf.update(beat_schedule=celery_beat_schedule)
     celery_app.autodiscover_tasks(task_module_paths)
 
     return celery_app
-
-
-@worker_process_init.connect()
-def worker_process_init(**kwargs):
-    logging.info("Worker Process Initialization started...")
-    # Optional Process Init Code
-    logging.info("Done Worker Process Initialization.")
-
-
-@worker_process_shutdown.connect()
-def worker_process_shutdown(**kwargs):
-    logging.info(f"Worker process [{kwargs['pid']}] shutdown... -> Exit Code: [{kwargs['exitcode']}]")
-    logging.info("Done worker process shutdown.")
```

## Comparing `matter_task_queue-2.1.0.dist-info/METADATA` & `matter_task_queue-2.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: matter-task-queue
-Version: 2.1.0
+Version: 2.2.0
 Summary: A template for new Matter's library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-task-queue#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-task-queue/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-task-queue
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
```

## Comparing `matter_task_queue-2.1.0.dist-info/licenses/LICENSE` & `matter_task_queue-2.2.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_task_queue-2.1.0.dist-info/RECORD` & `matter_task_queue-2.2.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-matter_task_queue/__about__.py,sha256=XL173fqhULxoUHjZEFhlqdi_Iw0cCjggqFhXkmgKiHU,134
+matter_task_queue/__about__.py,sha256=RInFV5fKDrs42qPhdwM9B3N6AVLR-6hYuR5l0YIXn14,134
 matter_task_queue/__init__.py,sha256=ZFkdbgwBSqy_H99nGWgV3FPvA4_qn3SjQ0jFyBDa7q0,327
 matter_task_queue/base_task.py,sha256=6J-CkaNo3PoERYwfcq2N6WKvUkm7eE1ZtGqqv9ms7nk,1228
 matter_task_queue/celery_config.py,sha256=-K8F3uI3HzFH6WHGsZZo5hW4nUBdtnXZwgv6rGH1QTs,4032
 matter_task_queue/config.py,sha256=Nj86ToyMgHBjUcxnoBiEIsLNw2zDCZydN5bqFa354Gg,1020
-matter_task_queue/utils.py,sha256=V5vlCW39lRJvorJka7kAAt2IRSebgmAGVXydOYHwdQ0,3232
-matter_task_queue-2.1.0.dist-info/METADATA,sha256=r1NG_brbEt9JCty1zjb-Z1HIz4ycv3Qc5uTXnIdS9wQ,4808
-matter_task_queue-2.1.0.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-matter_task_queue-2.1.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_task_queue-2.1.0.dist-info/RECORD,,
+matter_task_queue/utils.py,sha256=n20xaGEDOLjUX0M2FYeo9_VnIVCfuRJohB_lQjRHie8,2861
+matter_task_queue-2.2.0.dist-info/METADATA,sha256=N6V21RQGOJyCyYevjH05TIB-DB33mhc4wWG-AE_jHk8,4808
+matter_task_queue-2.2.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+matter_task_queue-2.2.0.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_task_queue-2.2.0.dist-info/RECORD,,
```

