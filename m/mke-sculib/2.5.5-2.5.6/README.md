# Comparing `tmp/mke_sculib-2.5.5.tar.gz` & `tmp/mke_sculib-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.5.5.tar", last modified: Sat May 11 20:05:13 2024, max compression
+gzip compressed data, was "mke_sculib-2.5.6.tar", last modified: Mon May 13 18:06:44 2024, max compression
```

## Comparing `mke_sculib-2.5.5.tar` & `mke_sculib-2.5.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 20:05:13.733485 mke_sculib-2.5.5/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.5/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-11 20:05:13.733485 mke_sculib-2.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.5/README.rst
--rw-rw-rw-   0        0        0     1017 2024-05-11 20:05:13.734470 mke_sculib-2.5.5/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 20:05:13.706471 mke_sculib-2.5.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-11 20:05:13.726389 mke_sculib-2.5.5/src/mke_sculib/
--rw-rw-rw-   0        0        0     1216 2024-05-11 20:04:31.000000 mke_sculib-2.5.5/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.5/src/mke_sculib/acu.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.5/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.5/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.5/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.5/src/mke_sculib/js_helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.5/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0   106616 2024-05-11 19:38:17.000000 mke_sculib-2.5.5/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.5.5/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.5/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-11 20:05:13.731475 mke_sculib-2.5.5/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-11 20:05:13.000000 mke_sculib-2.5.5/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2024-05-11 20:05:13.000000 mke_sculib-2.5.5/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 20:05:13.000000 mke_sculib-2.5.5/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-11 20:05:13.000000 mke_sculib-2.5.5/src/mke_sculib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-11 20:05:13.000000 mke_sculib-2.5.5/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-11 20:05:13.732474 mke_sculib-2.5.5/tests/
--rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.5/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.5/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:06:44.068924 mke_sculib-2.5.6/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.6/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-13 18:06:44.069924 mke_sculib-2.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.6/README.rst
+-rw-rw-rw-   0        0        0     1017 2024-05-13 18:06:44.070923 mke_sculib-2.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:06:44.038047 mke_sculib-2.5.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 18:06:44.049695 mke_sculib-2.5.6/src/mke_sculib/
+-rw-rw-rw-   0        0        0     1216 2024-05-13 18:05:40.000000 mke_sculib-2.5.6/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.6/src/mke_sculib/acu.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.6/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.6/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.6/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.6/src/mke_sculib/js_helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.6/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0   106870 2024-05-13 18:04:43.000000 mke_sculib-2.5.6/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.5.6/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.6/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:06:44.061919 mke_sculib-2.5.6/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-13 18:06:43.000000 mke_sculib-2.5.6/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2024-05-13 18:06:43.000000 mke_sculib-2.5.6/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:06:43.000000 mke_sculib-2.5.6/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-13 18:06:43.000000 mke_sculib-2.5.6/src/mke_sculib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 18:06:43.000000 mke_sculib-2.5.6/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 18:06:44.068924 mke_sculib-2.5.6/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.6/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.6/tests/test_scu.py
```

### Comparing `mke_sculib-2.5.5/LICENSE` & `mke_sculib-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/PKG-INFO` & `mke_sculib-2.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.5.5
+Version: 2.5.6
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.5/README.rst` & `mke_sculib-2.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/setup.cfg` & `mke_sculib-2.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/src/mke_sculib/__init__.py` & `mke_sculib-2.5.6/src/mke_sculib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.5.5'
+__version__ = '2.5.6'
 
 from mke_sculib.scu import scu as scu_api, plot_tt, print_color, colors
 from mke_sculib.sim import scu_sim
 from mke_sculib.stellarium_api import stellarium_api as stellar_api
 from mke_sculib.sim import plot_motion_pyplot as plot_motion
 from mke_sculib.helpers import get_utcnow, make_zulustr, parse_zulutime
```

### Comparing `mke_sculib-2.5.5/src/mke_sculib/acu.py` & `mke_sculib-2.5.6/src/mke_sculib/acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.5.6/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.5.6/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/src/mke_sculib/helpers.py` & `mke_sculib-2.5.6/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/src/mke_sculib/js_helpers.py` & `mke_sculib-2.5.6/src/mke_sculib/js_helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.5.6/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/src/mke_sculib/scu.py` & `mke_sculib-2.5.6/src/mke_sculib/scu.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,19 +208,20 @@
         
         def statusupdate():
             
             with ws_sync_connect(f'ws://{self.parent.ip}:{self.parent.port}/wsstatus') as ws:
                 ws.send(json.dumps(self.channels))
                 while True:
                     data = json.loads(ws.recv())
-                    self.t_last_remote = Time(data['timestamp'])
                     self.t_last_local = Time.now()
                     self.tickcount += 1
                     self.data = {k:v[0] for k, v in data['fields'].items()}
-                    
+                    # data['timestamp'] is the local NTP timestamp of the windows system, not the actual PTP time
+                    self.t_last_remote = Time(self.data.get('acu.time.external_ptp', data['timestamp']))
+
         self.thread = threading.Thread(target=statusupdate)
         self.thread.daemon = True
         self.thread.start()
         if self.verb: log('--> datasteam started...', color=colors.OKGREEN)
         return self.thread
     
 
@@ -559,15 +560,17 @@
                     r.raise_for_status()
                     return json.loads(txt)
                     
             return await asyncio.gather(*(get(d, p) for d, p in zip(devices, params)))
 
     def get_errors(self, warnings=True):
         if warnings:
-            return {k:v for k, v in self.getc(as_dict=True).items() if ('warn' in k.lower() or 'err' in k.lower()) and v}
+            fun = lambda k, v: ('warn' in k.lower() or 'err' in k.lower()) and v and 'not_used' not in k and 'limit' not in k and 'stowpins' not in k and v
+            return {k:v for k, v in self.getc(as_dict=True).items() if fun(k, v)}
+
         return {k:v for k, v in self.getc(as_dict=True).items() if 'err' in k.lower() and v}
     
     def scu_get_concurrent(self, devices, params):
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(self.scu_get_async(devices, params))
```

### Comparing `mke_sculib-2.5.5/src/mke_sculib/sim.py` & `mke_sculib-2.5.6/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.5.6/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.5.6/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.5.5
+Version: 2.5.6
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.5/src/mke_sculib.egg-info/SOURCES.txt` & `mke_sculib-2.5.6/src/mke_sculib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/tests/test_acu_sim.py` & `mke_sculib-2.5.6/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.5/tests/test_scu.py` & `mke_sculib-2.5.6/tests/test_scu.py`

 * *Files identical despite different names*

