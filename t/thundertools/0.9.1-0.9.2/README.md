# Comparing `tmp/thundertools-0.9.1-py3-none-any.whl.zip` & `tmp/thundertools-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 13326 bytes, number of entries: 19
+Zip file size: 13361 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx      552 b- defN 24-Mar-13 10:26 thunder/__init__.py
 -rw-rw-r--  2.0 unx      735 b- defN 23-Nov-01 15:58 thunder/boolpicker.py
 -rw-rw-r--  2.0 unx     1823 b- defN 24-Mar-14 08:47 thunder/citer.py
 -rw-rw-r--  2.0 unx     1876 b- defN 23-Nov-01 15:58 thunder/enumpicker.py
 -rw-rw-r--  2.0 unx     7136 b- defN 23-Nov-01 15:58 thunder/export_conda.py
 -rw-rw-r--  2.0 unx     3190 b- defN 23-Nov-01 15:58 thunder/fancylogger.py
 -rw-rw-r--  2.0 unx     2513 b- defN 23-Nov-01 15:58 thunder/filepicker.py
 -rw-rw-r--  2.0 unx      727 b- defN 23-Nov-01 15:58 thunder/numberpicker.py
--rw-rw-r--  2.0 unx     2545 b- defN 24-Mar-13 10:26 thunder/profiler.py
+-rw-rw-r--  2.0 unx     2699 b- defN 24-May-13 13:11 thunder/profiler.py
 -rw-rw-r--  2.0 unx     1507 b- defN 23-Nov-01 19:53 thunder/repr_dict.py
 -rw-rw-r--  2.0 unx      372 b- defN 23-Nov-01 15:58 thunder/stringpicker.py
 -rw-rw-r--  2.0 unx     2435 b- defN 23-Nov-01 15:58 thunder/thunder_credentials.py
 -rw-rw-r--  2.0 unx     1033 b- defN 24-Mar-08 08:05 thunder/tools.py
--rw-rw-r--  2.0 unx       22 b- defN 24-Mar-14 08:49 thunder/version.py
+-rw-rw-r--  2.0 unx       22 b- defN 24-May-13 13:08 thunder/version.py
 -rw-rw-r--  2.0 unx     1751 b- defN 24-Mar-08 07:42 thunder/zipit.py
--rw-rw-r--  2.0 unx      553 b- defN 24-Mar-14 08:49 thundertools-0.9.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-14 08:49 thundertools-0.9.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Mar-14 08:49 thundertools-0.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1473 b- defN 24-Mar-14 08:49 thundertools-0.9.1.dist-info/RECORD
-19 files, 30343 bytes uncompressed, 10948 bytes compressed:  63.9%
+-rw-rw-r--  2.0 unx      553 b- defN 24-May-13 13:11 thundertools-0.9.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-13 13:11 thundertools-0.9.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-May-13 13:11 thundertools-0.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1473 b- defN 24-May-13 13:11 thundertools-0.9.2.dist-info/RECORD
+19 files, 30497 bytes uncompressed, 10983 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: thunder/version.py
 Comment: 
 
 Filename: thunder/zipit.py
 Comment: 
 
-Filename: thundertools-0.9.1.dist-info/METADATA
+Filename: thundertools-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: thundertools-0.9.1.dist-info/WHEEL
+Filename: thundertools-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: thundertools-0.9.1.dist-info/top_level.txt
+Filename: thundertools-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: thundertools-0.9.1.dist-info/RECORD
+Filename: thundertools-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## thunder/profiler.py

```diff
@@ -2,18 +2,19 @@
 from time import time
 from typing import Dict, DefaultDict, Callable, Optional
 import atexit
 import functools
 
 
 class Profiler:
-    def __init__(self, auto_report: bool = True) -> None:
+    def __init__(self, auto_report: bool = True, ignore_duplicate: bool = False) -> None:
         self.profiles: DefaultDict[str, Dict[str, float]] = defaultdict(lambda: {'count': 0, 'total_time': 0})
         self.active_profiles: Dict[str, float] = {}
-        self.auto_report = auto_report
+        self.auto_report: bool = auto_report
+        self.ignore_duplicate: bool = ignore_duplicate
         if self.auto_report:
             atexit.register(self.report)
 
     def __enter__(self) -> 'Profiler':
         self.start('_global')
         return self
 
@@ -27,14 +28,16 @@
         hours, remainder = divmod(duration_seconds, 3600)
         minutes, seconds = divmod(remainder, 60)
         milliseconds = (duration_seconds % 1) * 1000
         return f"{int(hours):02d}h {int(minutes):02d}m {int(seconds):02d}s {int(milliseconds):03d}ms"
 
     def start(self, name: str) -> None:
         if name in self.active_profiles:
+            if self.ignore_duplicate:
+                return
             raise ValueError(f"Profile '{name}' is already running.")
         self.active_profiles[name] = time()
 
     def stop(self, name: str) -> None:
         start_time = self.active_profiles.pop(name, None)
         if start_time is None:
             raise ValueError(f"Profile '{name}' has not been started.")
```

## thunder/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.9.1'
+__version__ = '0.9.2'
```

## Comparing `thundertools-0.9.1.dist-info/METADATA` & `thundertools-0.9.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thundertools
-Version: 0.9.1
+Version: 0.9.2
 Summary: Different tools for working in Python
 Home-page: https://github.com/ArnoDeDonder/ThunderTools
 Author: Arno De Donder
 Author-email: arno.dedonder@hotmail.com
 License: MIT
 Keywords: python,tools,utility,shell,terminal,scripts,linux,tqdm,zip
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: colorama ~=0.4.6
-Requires-Dist: setuptools ~=65.6.3
-Requires-Dist: pyyaml ==6.0.1
+Requires-Dist: colorama >=0.4.6
+Requires-Dist: setuptools >=65.6.3
+Requires-Dist: pyyaml >=6.0.1
```

## Comparing `thundertools-0.9.1.dist-info/RECORD` & `thundertools-0.9.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 thunder/boolpicker.py,sha256=JMlWpBF6BCmF3qIGzi78rVAe42zpI-xBsDK8P8EL7ac,735
 thunder/citer.py,sha256=21p4I6mEdOu3YkVpMHJfDmAWv8llvlzUWrtQud9fCCc,1823
 thunder/enumpicker.py,sha256=P0pyDR2PDR5O37gB4HvwBB3MymnzFqy2q5FwMDHuT58,1876
 thunder/export_conda.py,sha256=x8rcuBt0u0IHYPT-BpSj7AX5tyD407cxmzzO-vDK86U,7136
 thunder/fancylogger.py,sha256=-Cyy2EX_8A6cNNzP4MV4a0B1dL-0bcXHsEJc_-Zx2nQ,3190
 thunder/filepicker.py,sha256=BjM8tjGBaTEEg9UQ3aQZmwC8QZ6sGPp2UNjHF4OZ-9Q,2513
 thunder/numberpicker.py,sha256=pI3qdyGvDFeKmIRL9CUEgse3MUkQHQXsbm14NFnWWO4,727
-thunder/profiler.py,sha256=C_0D1FFAjTCrgo-ocWhSGrM1NcwbtLaPYBAomBwsXX8,2545
+thunder/profiler.py,sha256=OzKHUORICJN4W5CIS9ujJ9bxsfNGkBnmn3i11EBfSt4,2699
 thunder/repr_dict.py,sha256=bmbjo7UoLRwwk__MvP9sICPYTPXAyEaQ8gvY8k3tFf0,1507
 thunder/stringpicker.py,sha256=QWeO4xXkYF6lVv9wCX_FTXCdFqIY79JnplO3y_vHUas,372
 thunder/thunder_credentials.py,sha256=27cY6RomDo2uahKOLSt9H5Z6W7Qh_ku2O1Wjy-ZQYTw,2435
 thunder/tools.py,sha256=j1NzvV63rZQZssGWY9N0GntDCMPNxumklVyrES5f6zc,1033
-thunder/version.py,sha256=pF8TnH2QJF8nfDmcD7oPTrAOnioy05dV4YmYDzkT5Es,22
+thunder/version.py,sha256=HSMl6bLm3r1Ias1jHIPpJeQ0IYNuuSdlT38MTb79ewM,22
 thunder/zipit.py,sha256=-4qUzN00HKB-FEwv8OZA8rCXs9kVsi15BzpuRuQSlHA,1751
-thundertools-0.9.1.dist-info/METADATA,sha256=de-WKvUcV04pVFyk2ZeTc_Dsv5BiBkfzG_YxDfz9AWE,553
-thundertools-0.9.1.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-thundertools-0.9.1.dist-info/top_level.txt,sha256=H3Kmgbx7mW8sBDn18vcmMUqB_NO4MO0EddocH6RLuMM,8
-thundertools-0.9.1.dist-info/RECORD,,
+thundertools-0.9.2.dist-info/METADATA,sha256=HAj16NGQhwJP6C54H8AFnH0AoaTdHey22iPGkRAaiBE,553
+thundertools-0.9.2.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+thundertools-0.9.2.dist-info/top_level.txt,sha256=H3Kmgbx7mW8sBDn18vcmMUqB_NO4MO0EddocH6RLuMM,8
+thundertools-0.9.2.dist-info/RECORD,,
```

