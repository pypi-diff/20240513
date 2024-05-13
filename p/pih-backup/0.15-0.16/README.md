# Comparing `tmp/pih-backup-0.15.tar.gz` & `tmp/pih-backup-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-backup-0.15.tar", last modified: Wed Apr 10 22:14:26 2024, max compression
+gzip compressed data, was "pih-backup-0.16.tar", last modified: Mon May 13 02:48:41 2024, max compression
```

## Comparing `pih-backup-0.15.tar` & `pih-backup-0.16.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 22:14:26.356269 pih-backup-0.15/
-drwxrwxrwx   0        0        0        0 2024-04-10 22:14:25.933811 pih-backup-0.15/BackupService/
--rw-rw-rw-   0        0        0      140 2024-02-10 11:56:01.000000 pih-backup-0.15/BackupService/__main__.py
--rw-rw-rw-   0        0        0     5478 2024-04-09 23:53:55.000000 pih-backup-0.15/BackupService/api.py
--rw-rw-rw-   0        0        0     1676 2024-04-10 22:11:16.000000 pih-backup-0.15/BackupService/const.py
--rw-rw-rw-   0        0        0     4870 2024-04-09 23:53:08.000000 pih-backup-0.15/BackupService/service.py
--rw-rw-rw-   0        0        0      269 2024-04-10 22:14:26.325019 pih-backup-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 22:14:26.293771 pih-backup-0.15/pih_backup.egg-info/
--rw-rw-rw-   0        0        0      269 2024-04-10 22:14:25.000000 pih-backup-0.15/pih_backup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-04-10 22:14:25.000000 pih-backup-0.15/pih_backup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 22:14:25.000000 pih-backup-0.15/pih_backup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-10 22:14:25.000000 pih-backup-0.15/pih_backup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 22:14:25.000000 pih-backup-0.15/pih_backup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 22:14:25.000000 pih-backup-0.15/pih_backup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 22:14:26.371893 pih-backup-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 02:48:41.564010 pih-backup-0.16/
+drwxrwxrwx   0        0        0        0 2024-05-13 02:48:41.202563 pih-backup-0.16/BackupService/
+-rw-rw-rw-   0        0        0      140 2024-02-10 11:56:01.000000 pih-backup-0.16/BackupService/__main__.py
+-rw-rw-rw-   0        0        0     5478 2024-04-09 23:53:55.000000 pih-backup-0.16/BackupService/api.py
+-rw-rw-rw-   0        0        0     1676 2024-05-03 03:32:44.000000 pih-backup-0.16/BackupService/const.py
+-rw-rw-rw-   0        0        0     4929 2024-05-03 03:53:43.000000 pih-backup-0.16/BackupService/service.py
+-rw-rw-rw-   0        0        0      269 2024-05-13 02:48:41.532764 pih-backup-0.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 02:48:41.501517 pih-backup-0.16/pih_backup.egg-info/
+-rw-rw-rw-   0        0        0      269 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 02:48:40.000000 pih-backup-0.16/pih_backup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:48:41.579645 pih-backup-0.16/setup.cfg
```

### Comparing `pih-backup-0.15/BackupService/api.py` & `pih-backup-0.16/BackupService/api.py`

 * *Files identical despite different names*

### Comparing `pih-backup-0.15/BackupService/const.py` & `pih-backup-0.16/BackupService/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pih import A
 from pih.collections import RobocopyJobDescription
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Backup"
 
-VERSION: str = "0.15"
+VERSION: str = "0.16"
 
 
 JOB_CONFIG_ALIAS: str = "job_config"
 
 
 class ROBOCOPY:
```

### Comparing `pih-backup-0.15/BackupService/service.py` & `pih-backup-0.16/BackupService/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 
-import ipih
 from pih import A
 from BackupService.api import *
 from BackupService.const import *
 from pih.collections import Result, RobocopyJobStatus
-from pih.tools import ParameterList, nn, escs, e, n, jnl, esc, js
+from pih.tools import ParameterList, e, n, js, nn, ne, nns, jnl, esc, escs
 
 
 from datetime import datetime
 from typing import Any
 import grpc
 
 
@@ -86,15 +85,17 @@
             BackupApi().start_robocopy_job(job_item, force)
         return len(rjl) > 0
 
     def heat_beat_action(current_datetime: datetime) -> None:
         if nn(ROBOCOPY.JOB_MAP):
             rjl: list[RobocopyJobItem] = BackupApi.get_job_list()
             for rji in rjl:
-                if A.D_C.by_secondless_time(current_datetime, rji.start_datetime):
+                if ne(rji.start_cron_string) and A.D_C.now(
+                    nns(rji.start_cron_string), current_datetime
+                ):
                     BackupApi().start_robocopy_job(rji)
 
     def service_call_handler(sc: SC, pl: ParameterList, context) -> Any:
         if sc == SC.heart_beat:
             heat_beat_action(A.D_Ex.parameter_list(pl).get())
             return True
         if sc == SC.robocopy_start_job:
```

