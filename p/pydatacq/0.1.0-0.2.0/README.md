# Comparing `tmp/pydatacq-0.1.0.tar.gz` & `tmp/pydatacq-0.2.0.tar.gz`

## Comparing `pydatacq-0.1.0.tar` & `pydatacq-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0  4487098 2020-02-02 00:00:00.000000 pydatacq-0.1.0/resources/fft.mp4
--rw-r--r--   0        0        0  3412266 2020-02-02 00:00:00.000000 pydatacq-0.1.0/resources/fm_sine.mp4
--rw-r--r--   0        0        0  2480308 2020-02-02 00:00:00.000000 pydatacq-0.1.0/resources/thd.mp4
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/demo_fm_sine.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/fft.py
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/fft_calculations.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/live_fm_sine.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/live_sds.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/live_window.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/matplotlib_rc.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/osc.py
--rw-r--r--   0        0        0    17793 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/sds.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/siglent.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/examples/thd.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/pydatacq/__init__.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 pydatacq-0.1.0/src/pydatacq/live_data.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pydatacq-0.1.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pydatacq-0.1.0/LICENSE
--rw-r--r--   0        0        0    13862 2020-02-02 00:00:00.000000 pydatacq-0.1.0/README.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 pydatacq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    14366 2020-02-02 00:00:00.000000 pydatacq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0  4487098 2020-02-02 00:00:00.000000 pydatacq-0.2.0/resources/fft.mp4
+-rw-r--r--   0        0        0  3412266 2020-02-02 00:00:00.000000 pydatacq-0.2.0/resources/fm_sine.mp4
+-rw-r--r--   0        0        0  2480308 2020-02-02 00:00:00.000000 pydatacq-0.2.0/resources/thd.mp4
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/demo_fm_sine.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/fft.py
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/fft_calculations.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/live_fm_sine.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/matplotlib_rc.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/osc.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/examples/thd.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/__init__.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/live_data.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/live_sds.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/live_window.py
+-rw-r--r--   0        0        0    17738 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/sds.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pydatacq-0.2.0/src/pydatacq/siglent.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pydatacq-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pydatacq-0.2.0/LICENSE
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 pydatacq-0.2.0/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pydatacq-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14431 2020-02-02 00:00:00.000000 pydatacq-0.2.0/PKG-INFO
```

### Comparing `pydatacq-0.1.0/resources/fft.mp4` & `pydatacq-0.2.0/resources/fft.mp4`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/resources/fm_sine.mp4` & `pydatacq-0.2.0/resources/fm_sine.mp4`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/resources/thd.mp4` & `pydatacq-0.2.0/resources/thd.mp4`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/src/examples/demo_fm_sine.py` & `pydatacq-0.2.0/src/examples/demo_fm_sine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import matplotlib.pyplot as plt
 import numpy as np
+from pydatacq import LiveWindow
 
 from live_fm_sine import LiveFMSine
-from live_window import LiveWindow
 
 plt.rcParams['toolbar'] = 'None'
 
 
 # 
 async def process(data):
     '''
```

### Comparing `pydatacq-0.1.0/src/examples/fft.py` & `pydatacq-0.2.0/src/examples/fft.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 import builtins
 import asyncio
 
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import quantiphy as q
+from pydatacq import SDS, LiveSDS, LiveWindow
 
-from sds import SDS
 import fft_calculations
 from fft_calculations import fft
-from live_sds import LiveSDS
-from live_window import LiveWindow
 import matplotlib_rc
 
 live_sds = None
 
 parser = argparse.ArgumentParser(description='Display FFT for a channel on Siglent oscilloscope.',
                                  formatter_class=argparse.ArgumentDefaultsHelpFormatter)
```

### Comparing `pydatacq-0.1.0/src/examples/fft_calculations.py` & `pydatacq-0.2.0/src/examples/fft_calculations.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/src/examples/live_fm_sine.py` & `pydatacq-0.2.0/src/examples/live_fm_sine.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/src/examples/live_sds.py` & `pydatacq-0.2.0/src/pydatacq/live_sds.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from sds import SDS
-from pydatacq import LiveData
+from .sds import SDS
+from .live_data import LiveData
 
 
 #
 class LiveSDS(LiveData):
     '''
     Produces live data from an Siglent SDS1202X-E oscilloscope. This
     live data is produced asynchronously and can be processed in a
```

### Comparing `pydatacq-0.1.0/src/examples/live_window.py` & `pydatacq-0.2.0/src/pydatacq/live_window.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/src/examples/matplotlib_rc.py` & `pydatacq-0.2.0/src/examples/matplotlib_rc.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/src/examples/osc.py` & `pydatacq-0.2.0/src/examples/osc.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 import argparse
 import uvloop
 
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import quantiphy as q
+from pydatacq import SDS, LiveSDS, LiveWindow
 
-from sds import SDS
 import fft_calculations
 from fft_calculations import V_to_Vrms, Vrms_to_dBVrms, fft, thd
-from live_sds import LiveSDS
-from live_window import LiveWindow
 import matplotlib_rc
 
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 live_sds = None
```

### Comparing `pydatacq-0.1.0/src/examples/sds.py` & `pydatacq-0.2.0/src/pydatacq/sds.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from time import time, asctime
 
 import numpy as np
 from scipy.fft import rfft, rfftfreq
 from scipy.signal.windows import flattop
 import quantiphy as q
 
-from siglent import Siglent
+from .siglent import Siglent
 
 
 CH = ['C1','C2']
 
 ### Timebase lookup
 tbase_lookup = np.array([200e-12,
                 500e-12,
@@ -168,26 +168,25 @@
         response = await self.async_query(cmd)
         timebase = float(response[5:-2])
 
         T = timebase * self.divisions()
         wait = T * 4
         now = time()
 
-        if True:
-            if self._wavetime is not None:
-                # decide how long ago it was the last waveform
-                # was acquired. Wait more until it was 'wait'
-                # seconds ago to let the oscilloscope acquire
-                # a new waveform.
-                passed = now - self._wavetime
-                if passed < wait:
-                    sleep = wait - passed
-                    print(f'{asctime()}: sleep {sleep}')
-                    await asyncio.sleep(sleep)
-            self._wavetime = now
+        if self._wavetime is not None:
+            # decide how long ago it was the last waveform
+            # was acquired. Wait more until it was 'wait'
+            # seconds ago to let the oscilloscope acquire
+            # a new waveform.
+            passed = now - self._wavetime
+            if passed < wait:
+                sleep = wait - passed
+#                    print(f'{asctime()}: sleep {sleep}')
+                await asyncio.sleep(sleep)
+        self._wavetime = now
 
         # Get wave
         wave = await self.async_query_rawwave(channel)
         w = np.frombuffer(wave,dtype=np.int8)
         w = np.where(w>127, w-256, w)
 
         # Get VDIV
```

### Comparing `pydatacq-0.1.0/src/examples/siglent.py` & `pydatacq-0.2.0/src/pydatacq/siglent.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/src/examples/thd.py` & `pydatacq-0.2.0/src/examples/thd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import argparse
 import asyncio
 
 import numpy as np
 import matplotlib.pyplot as plt
 import quantiphy as q
+from pydatacq import SDS, LiveSDS, LiveWindow
 
-from sds import SDS
 from fft_calculations import V_to_Vrms, Vrms_to_dBVrms, fft, thd
-from live_sds import LiveSDS
-from live_window import LiveWindow
 import matplotlib_rc
 
 parser = argparse.ArgumentParser(description='Display FFT and calculate THD for a channel on Siglent SDS1202X-E oscilloscope.',
                                  formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
 parser.add_argument('-C',dest='channel',required=True,type=int,help='channel to display',choices=[1,2])
 parser.add_argument('-f0',default='1k',metavar='FREQ',help='fundamental frequency (in Hz)')
```

### Comparing `pydatacq-0.1.0/src/pydatacq/live_data.py` & `pydatacq-0.2.0/src/pydatacq/live_data.py`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/LICENSE` & `pydatacq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatacq-0.1.0/README.md` & `pydatacq-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pydatacq - Asynchronous Data Acquisition
 
 With pydatacq you can collect data from a series of instruments. The drivers for specific instruments can be injected into the library. A driver for the SDS series of oscilloscopes from Siglent are included.
 
 Data is acquired in an asynchronous way. Data collection is not blocking. So several instruments can be sampled at the same time, as well as calcuulation, display, storing etc of the sampled data.
 
-Some demo progams (fft,thd,oscilloscope) are included in the package as well.
+Some demo progams (fft,thd,oscilloscope) are available in the src/examples folder.
 
 Short screen captures of sampling data and displaying them in a matplotlib window are present in the /resources folder.
 
 
 
 ## Classes
```

### Comparing `pydatacq-0.1.0/pyproject.toml` & `pydatacq-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydatacq"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="kvdijken", email="sla_nippers_0x@icloud.com" },
 ]
 dependencies = ["numpy","scipy","uvloop","matplotlib","quantiphy"]
 
 description = "A package for asynchronous data acquisition"
 readme = "README.md"
@@ -17,7 +17,9 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
 
+[project.urls]
+Homepage = "https://github.com/kvdijken/pydatacq"
```

### Comparing `pydatacq-0.1.0/PKG-INFO` & `pydatacq-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.3
 Name: pydatacq
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for asynchronous data acquisition
+Project-URL: Homepage, https://github.com/kvdijken/pydatacq
 Author-email: kvdijken <sla_nippers_0x@icloud.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: matplotlib
@@ -17,15 +18,15 @@
 
 # pydatacq - Asynchronous Data Acquisition
 
 With pydatacq you can collect data from a series of instruments. The drivers for specific instruments can be injected into the library. A driver for the SDS series of oscilloscopes from Siglent are included.
 
 Data is acquired in an asynchronous way. Data collection is not blocking. So several instruments can be sampled at the same time, as well as calcuulation, display, storing etc of the sampled data.
 
-Some demo progams (fft,thd,oscilloscope) are included in the package as well.
+Some demo progams (fft,thd,oscilloscope) are available in the src/examples folder.
 
 Short screen captures of sampling data and displaying them in a matplotlib window are present in the /resources folder.
 
 
 
 ## Classes
```

