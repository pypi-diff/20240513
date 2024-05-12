# Comparing `tmp/eva4-controller-py-0.1.4.tar.gz` & `tmp/eva4-controller-py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva4-controller-py-0.1.4.tar", last modified: Thu Apr 25 22:40:00 2024, max compression
+gzip compressed data, was "eva4-controller-py-0.1.5.tar", last modified: Sun May 12 23:25:52 2024, max compression
```

## Comparing `eva4-controller-py-0.1.4.tar` & `eva4-controller-py-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/
--rw-r--r--   0 divisor   (1000) root         (0)    10644 2023-11-19 23:00:18.000000 eva4-controller-py-0.1.4/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      521 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       46 2022-04-01 21:38:20.000000 eva4-controller-py-0.1.4/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       75 2022-04-01 21:42:50.000000 eva4-controller-py-0.1.4/bin/eva4-svc-controller-py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/eva4_controller_py/
--rw-r--r--   0 divisor   (1000) root         (0)     5826 2024-04-25 22:31:25.000000 eva4-controller-py-0.1.4/eva4_controller_py/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    21104 2024-04-25 22:36:53.000000 eva4-controller-py-0.1.4/eva4_controller_py/macro_api.py
--rw-r--r--   0 divisor   (1000) root         (0)     1307 2024-04-25 22:31:25.000000 eva4-controller-py-0.1.4/eva4_controller_py/macro_builtins.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      521 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      362 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       45 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       19 2024-04-25 22:40:00.000000 eva4-controller-py-0.1.4/eva4_controller_py.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2024-04-25 22:40:00.065114 eva4-controller-py-0.1.4/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)      820 2024-04-25 22:31:25.000000 eva4-controller-py-0.1.4/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-05-12 23:25:52.393508 eva4-controller-py-0.1.5/
+-rw-r--r--   0 divisor   (1000) root         (0)    10644 2023-11-19 23:00:18.000000 eva4-controller-py-0.1.5/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      521 2024-05-12 23:25:52.393508 eva4-controller-py-0.1.5/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       46 2022-04-01 21:38:20.000000 eva4-controller-py-0.1.5/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-05-12 23:25:52.389508 eva4-controller-py-0.1.5/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       75 2022-04-01 21:42:50.000000 eva4-controller-py-0.1.5/bin/eva4-svc-controller-py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-05-12 23:25:52.393508 eva4-controller-py-0.1.5/eva4_controller_py/
+-rw-r--r--   0 divisor   (1000) root         (0)     5916 2024-05-12 23:25:37.000000 eva4-controller-py-0.1.5/eva4_controller_py/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    21664 2024-05-12 23:25:37.000000 eva4-controller-py-0.1.5/eva4_controller_py/macro_api.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1307 2024-05-12 23:25:37.000000 eva4-controller-py-0.1.5/eva4_controller_py/macro_builtins.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-05-12 23:25:52.393508 eva4-controller-py-0.1.5/eva4_controller_py.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      521 2024-05-12 23:25:52.000000 eva4-controller-py-0.1.5/eva4_controller_py.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      362 2024-05-12 23:25:52.000000 eva4-controller-py-0.1.5/eva4_controller_py.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2024-05-12 23:25:52.000000 eva4-controller-py-0.1.5/eva4_controller_py.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       45 2024-05-12 23:25:52.000000 eva4-controller-py-0.1.5/eva4_controller_py.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       19 2024-05-12 23:25:52.000000 eva4-controller-py-0.1.5/eva4_controller_py.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2024-05-12 23:25:52.393508 eva4-controller-py-0.1.5/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)      820 2024-05-12 23:25:37.000000 eva4-controller-py-0.1.5/setup.py
```

### Comparing `eva4-controller-py-0.1.4/LICENSE` & `eva4-controller-py-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eva4-controller-py-0.1.4/PKG-INFO` & `eva4-controller-py-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eva4-controller-py
-Version: 0.1.4
+Version: 0.1.5
 Summary: EVA ICS v4 Python macros controller service
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eva4-controller-py-0.1.4/eva4_controller_py/__init__.py` & `eva4-controller-py-0.1.5/eva4_controller_py/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 from evaics.sdk import Service, Controller, Action, no_rpc_method, ServiceInfo
 from evaics.sdk import OID
 
 from timeouter import Timer
 
 from types import SimpleNamespace
@@ -30,14 +30,15 @@
 bfname = f'{dir_me}/macro_builtins.py'
 d = {}
 with open(bfname) as fh:
     _d.builtins = compile(fh.read(), bfname, 'exec')
 
 
 class Compiler:
+
     def __init__(self):
         self.cache = {}
         self.cache_lock = threading.Lock()
 
     def compile(self, fname):
         mtime = os.path.getmtime(fname)
         with self.cache_lock:
@@ -182,15 +183,16 @@
         '_polldelay': poll_delay,
         'is_shutdown': service.is_shutdown_requested
     }
     _d.env.update(config.get('cvars', {}))
     _d.env.update(macro_api.api_globals)
     macro_api.service = service
     macro_api.locker_svc = config.get('locker_svc')
-    macro_api.mailer_svc = config.get('mailer_svc')
+    macro_api.mailer_svc = config.get('mailer_svc', 'eva.svc.mailer')
+    macro_api.alarm_svc = config.get('alarm_svc', 'eva.alarm.default')
     service.on_rpc_call = handle_rpc
     service.init_rpc(info)
     _d.logger.info(f'dir: {_d.dir_xcpy}, pool_size: {pool_size}')
     service.register_signals()
     service.mark_ready()
     service.wait_core()
     _d.pool.submit(safe_run_system_macro, 'autoexec')
```

### Comparing `eva4-controller-py-0.1.4/eva4_controller_py/macro_api.py` & `eva4-controller-py-0.1.5/eva4_controller_py/macro_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 eva_dir = None
 svc_data_dir = None
 service = None
 
 locker_svc = None
 mailer_svc = None
+alarm_svc = None
 
 g = LocalProxy()
 
 
 def parse_action_payload(payload):
     payload['uuid'] = str(UUID(bytes=payload['uuid']))
     return payload
@@ -120,17 +121,14 @@
 def update_state(oid, state):
     """
     Updates item state
 
     Args:
         oid: item OID
         state: new state (may contain status/value fields)
-
-    Optional:
-        force: force update even if the state is not changed
     """
     if 'status' not in state:
         state['status'] = 1
     oid = OID(oid) if isinstance(oid, str) else oid
     topic = f'{RAW_STATE_TOPIC}{oid.to_path()}'
     bus_publish(topic, state)
 
@@ -349,14 +347,40 @@
                  _target=mailer_svc,
                  subject=subject,
                  text=text,
                  rcp=rcp,
                  i=i)
 
 
+def set_alarm(oid, op, source='lmacro'):
+    """
+    Sets alarm state
+
+    Requires alarm svc to be set in the controller config
+
+    Args:
+        oid: alarm OID
+        op: alarm operation
+    Optional:
+        source: alarm source (default: lmacro)
+
+    Raises:
+        FunctionFailed: failed to set alarm state
+    """
+    if alarm_svc is None:
+        raise MethodNotImplemented('no alarm svc defined')
+    else:
+        rpc_call('alarm.set',
+                 _target=alarm_svc,
+                 i=oid,
+                 op=op,
+                 source=source,
+                 sk='P')
+
+
 def state(oid):
     """
     Gets item state
 
     Args:
         oid: item OID or mask
 
@@ -927,14 +951,15 @@
     'terminate': terminate,
     'kill': kill,
     'run': run,
     'system': _system,
     'ping': ping,
     'time': time.time,
     'mail': mail,
+    'set_alarm': set_alarm,
     'instant': time.perf_counter,
     'date': date,
     'ls': ls,
     'rpc_call': rpc_call,
     'bus_publish': bus_publish,
     'report_accounting_event': report_accounting_event
 }
```

### Comparing `eva4-controller-py-0.1.4/eva4_controller_py/macro_builtins.py` & `eva4-controller-py-0.1.5/eva4_controller_py/macro_builtins.py`

 * *Files identical despite different names*

### Comparing `eva4-controller-py-0.1.4/eva4_controller_py.egg-info/PKG-INFO` & `eva4-controller-py-0.1.5/eva4_controller_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eva4-controller-py
-Version: 0.1.4
+Version: 0.1.5
 Summary: EVA ICS v4 Python macros controller service
 Home-page: https://github.com/eva-ics/eva4
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eva4-controller-py-0.1.4/setup.py` & `eva4-controller-py-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

