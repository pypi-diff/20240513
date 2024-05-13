# Comparing `tmp/asmu-0.0.1a8.tar.gz` & `tmp/asmu-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmu-0.0.1a8.tar", last modified: Sat May  4 15:55:33 2024, max compression
+gzip compressed data, was "asmu-0.0.1a9.tar", last modified: Mon May 13 16:15:47 2024, max compression
```

## Comparing `asmu-0.0.1a8.tar` & `asmu-0.0.1a9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 15:55:33.343035 asmu-0.0.1a8/
--rw-rw-rw-   0 root         (0) root         (0)    35148 2024-05-04 15:55:19.000000 asmu-0.0.1a8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      846 2024-05-04 15:55:33.342034 asmu-0.0.1a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-05-04 15:55:19.000000 asmu-0.0.1a8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 15:55:33.341035 asmu-0.0.1a8/asmu/
--rw-rw-rw-   0 root         (0) root         (0)      551 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/afile.py
--rw-rw-rw-   0 root         (0) root         (0)     2925 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)     3207 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/asetup.py
--rw-rw-rw-   0 root         (0) root         (0)     7136 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/generator.py
--rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/io.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2024-05-04 15:55:19.000000 asmu-0.0.1a8/asmu/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 15:55:33.342034 asmu-0.0.1a8/asmu.egg-info/
--rw-r--r--   0 root         (0) root         (0)      846 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      276 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-04 15:55:33.000000 asmu-0.0.1a8/asmu.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      739 2024-05-04 15:55:19.000000 asmu-0.0.1a8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-04 15:55:33.343035 asmu-0.0.1a8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:15:47.518345 asmu-0.0.1a9/
+-rw-rw-rw-   0 root         (0) root         (0)    35148 2024-05-13 16:15:33.000000 asmu-0.0.1a9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      846 2024-05-13 16:15:47.518345 asmu-0.0.1a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-05-13 16:15:33.000000 asmu-0.0.1a9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:15:47.516345 asmu-0.0.1a9/asmu/
+-rw-rw-rw-   0 root         (0) root         (0)      551 2024-05-13 16:15:33.000000 asmu-0.0.1a9/asmu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2024-05-13 16:15:33.000000 asmu-0.0.1a9/asmu/afile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2961 2024-05-13 16:15:33.000000 asmu-0.0.1a9/asmu/analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3207 2024-05-13 16:15:33.000000 asmu-0.0.1a9/asmu/asetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     7136 2024-05-13 16:15:33.000000 asmu-0.0.1a9/asmu/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-13 16:15:33.000000 asmu-0.0.1a9/asmu/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2024-05-13 16:15:33.000000 asmu-0.0.1a9/asmu/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:15:47.517345 asmu-0.0.1a9/asmu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      846 2024-05-13 16:15:47.000000 asmu-0.0.1a9/asmu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      276 2024-05-13 16:15:47.000000 asmu-0.0.1a9/asmu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 16:15:47.000000 asmu-0.0.1a9/asmu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 16:15:47.000000 asmu-0.0.1a9/asmu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-13 16:15:47.000000 asmu-0.0.1a9/asmu.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      739 2024-05-13 16:15:33.000000 asmu-0.0.1a9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 16:15:47.518345 asmu-0.0.1a9/setup.cfg
```

### Comparing `asmu-0.0.1a8/LICENSE` & `asmu-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a8/asmu/__init__.py` & `asmu-0.0.1a9/asmu/__init__.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a8/asmu/afile.py` & `asmu-0.0.1a9/asmu/afile.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a8/asmu/analyzer.py` & `asmu-0.0.1a9/asmu/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,56 +31,56 @@
                 except queue.Empty:
                     pass
             # flush the remaining queue ater stream is closed
             while not self._q.empty():
                 self._process_queue()
         threading.Thread(target=runner, args=(self, stream, )).start()
 
-
-    def _get_fft(self) -> np.ndarray:
-        raise NotImplementedError() # TODO: Move this to helper function
-        return np.fft.rfft(self._q.get()*self._w, axis=0, norm="forward")*2/np.mean(self._w)
-    
 class Recorder(Analyzer):
     def __init__(self, signal, queuesize=10):
         """_summary_
 
         Args:
             signal (_type_): _description_
             queuesize (int, optional): _description_. Defaults to 10.
         """
         self._signal = signal
         super().__init__(queuesize)
         
     def _process_queue(self):
         self._signal.write(self._q.get(timeout=0.2))
 
-class calSPL(Analyzer):
-    def __init__(self, queuesize: int=10):
+class calcPa(Analyzer):
+    def __init__(self, blocksize, queuesize: int=10):
         self._uks = []
         self._ks = []
+        self._w = np.hanning(blocksize)
         super().__init__(queuesize)
 
     def _process_queue(self):
         ukm = self._get_fft()
 
         kmax = np.argmax(np.abs(ukm))
         self._uks.append(np.abs(ukm[kmax]))
         self._ks.append(kmax)
 
-    def get_cSPL(self, spl):
+    def _get_fft(self) -> np.ndarray:
+        # TODO: Move this to helper function
+        return np.fft.rfft(self._q.get(timeout=0.2)*self._w[:, None], axis=0, norm="forward")*2/np.mean(self._w)
+
+    def get_cPa(self, spl):
         self.reset()
 
         p0 = 2e-5                           # [Pa]Rms
         p = p0 * 10 ** (spl / 20)           # [Pa]Rms
         pcal = p * np.sqrt(2)               # [Pa]
 
         return pcal/np.mean(self._uks[2:]) # dont use the first three measurements
 
-    def get_kSPL(self):
+    def get_kPa(self):
         return round(np.mean(self._ks))
     
 def get_corrs_sampleshifts(indata: np.ndarray, refdata: np.ndarray, burstLength: int) -> tuple[np.ndarray, np.ndarray]:
     corrs = []
     sampleshifts = []
     n = int(np.size(refdata))
     for cidx in range(np.ma.size(indata, axis=1)):
```

### Comparing `asmu-0.0.1a8/asmu/asetup.py` & `asmu-0.0.1a9/asmu/asetup.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a8/asmu/generator.py` & `asmu-0.0.1a9/asmu/generator.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a8/asmu/io.py` & `asmu-0.0.1a9/asmu/io.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a8/asmu/view.py` & `asmu-0.0.1a9/asmu/view.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a8/pyproject.toml` & `asmu-0.0.1a9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asmu"
-version = "v0.0.1a8"
+version = "v0.0.1a9"
 authors = [
     {name = "felhub", email = "felhub@net4us.at"},
 ]
 description = "Acoustic Signal Measurement Utilities"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

