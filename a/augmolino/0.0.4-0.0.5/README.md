# Comparing `tmp/augmolino-0.0.4.tar.gz` & `tmp/augmolino-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\augmolino-0.0.4.tar", last modified: Sun May  5 18:19:48 2024, max compression
+gzip compressed data, was "dist\augmolino-0.0.5.tar", last modified: Mon May 13 07:39:05 2024, max compression
```

## Comparing `augmolino-0.0.4.tar` & `augmolino-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 18:19:48.975685 augmolino-0.0.4/
--rw-rw-rw-   0        0        0    35823 2024-05-05 18:07:59.000000 augmolino-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      509 2024-05-05 18:19:48.973682 augmolino-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2024-05-05 18:07:59.000000 augmolino-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 18:19:48.905678 augmolino-0.0.4/augmolino/
--rw-rw-rw-   0        0        0        0 2024-05-05 18:07:59.000000 augmolino-0.0.4/augmolino/__init__.py
--rw-rw-rw-   0        0        0     9860 2024-05-05 18:15:38.000000 augmolino-0.0.4/augmolino/augmentation.py
--rw-rw-rw-   0        0        0     4753 2024-05-05 18:07:59.000000 augmolino-0.0.4/augmolino/augmenter.py
--rw-rw-rw-   0        0        0      747 2024-05-05 18:07:59.000000 augmolino-0.0.4/augmolino/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:19:48.971683 augmolino-0.0.4/augmolino.egg-info/
--rw-rw-rw-   0        0        0      509 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-05 18:19:48.978683 augmolino-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      669 2024-05-05 18:16:36.000000 augmolino-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:19:48.967685 augmolino-0.0.4/tests/
--rw-rw-rw-   0        0        0     4111 2024-05-05 18:07:59.000000 augmolino-0.0.4/tests/test_augmentation.py
--rw-rw-rw-   0        0        0     2643 2024-05-05 18:07:59.000000 augmolino-0.0.4/tests/test_augmenter.py
--rw-rw-rw-   0        0        0      163 2024-05-05 18:12:59.000000 augmolino-0.0.4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:39:05.987160 augmolino-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2024-05-05 18:07:59.000000 augmolino-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      509 2024-05-13 07:39:05.985163 augmolino-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2024-05-05 18:07:59.000000 augmolino-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 07:39:05.943113 augmolino-0.0.5/augmolino/
+-rw-rw-rw-   0        0        0        0 2024-05-05 18:07:59.000000 augmolino-0.0.5/augmolino/__init__.py
+-rw-rw-rw-   0        0        0    10155 2024-05-13 07:20:44.000000 augmolino-0.0.5/augmolino/augmentation.py
+-rw-rw-rw-   0        0        0     4753 2024-05-05 18:07:59.000000 augmolino-0.0.5/augmolino/augmenter.py
+-rw-rw-rw-   0        0        0      747 2024-05-05 18:07:59.000000 augmolino-0.0.5/augmolino/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:39:05.980121 augmolino-0.0.5/augmolino.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-05-13 07:39:05.000000 augmolino-0.0.5/augmolino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-13 07:39:05.000000 augmolino-0.0.5/augmolino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:39:05.000000 augmolino-0.0.5/augmolino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 18:19:48.000000 augmolino-0.0.5/augmolino.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2024-05-13 07:39:05.000000 augmolino-0.0.5/augmolino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 07:39:05.000000 augmolino-0.0.5/augmolino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-13 07:39:05.992163 augmolino-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      669 2024-05-13 07:37:35.000000 augmolino-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:39:05.977118 augmolino-0.0.5/tests/
+-rw-rw-rw-   0        0        0     4099 2024-05-13 07:33:06.000000 augmolino-0.0.5/tests/test_augmentation.py
+-rw-rw-rw-   0        0        0     2643 2024-05-05 18:07:59.000000 augmolino-0.0.5/tests/test_augmenter.py
+-rw-rw-rw-   0        0        0      163 2024-05-05 18:12:59.000000 augmolino-0.0.5/tests/test_utils.py
```

### Comparing `augmolino-0.0.4/LICENSE` & `augmolino-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `augmolino-0.0.4/README.md` & `augmolino-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `augmolino-0.0.4/augmolino/augmentation.py` & `augmolino-0.0.5/augmolino/augmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -257,14 +257,19 @@
 
 class mixAudio(_augmentation):
     """
     Mix two wavefiles at random or specified timestamps.
 
     Parameters
     ----------
+    `f_mix`:
+        Path or str. Sound which should be mixed onto each sound that
+        gets processed by the augmentation. `f_mix` gets set statically
+        and remains in the specific instance of this augmentation. Careful
+        naming is advised.
     `ratio`:
         Float. Ratio by which the sounds are mixed. 
         `0 <= ratio <= 1`, 1 ignores the noise, 0 the main sound. 
         Default is `1`.
     `start_at`:
         Float. Second at which the mixed in sound should be used.
         If unspecified, a random time will be used. Default is `None`.     
@@ -274,25 +279,26 @@
 
     Notes
     -----
     Augmented sound is as long as the original sound of interest, 
     not the mixed-in sound    
     """
 
-    def __init__(self, ratio=0.5, start_at=None, sample_rate=22050):
+    def __init__(self, f_mix, ratio=0.5, start_at=None, sample_rate=22050):
         self.ratio = ratio
         self.start_at = start_at
+        self.f_mix = f_mix
         super().__init__(sample_rate=sample_rate,
                          function=self._mix,
                          ratio=ratio,
                          start_at=start_at)
         self.descriptor = descriptors[__all__[4]]
 
-    def _mix(self, y, f_mix, ratio, start_at):
-        y_mix, _ = lr.load(f_mix, sr=self.sample_rate)
+    def _mix(self, y, ratio, start_at):
+        y_mix, _ = lr.load(self.f_mix, sr=self.sample_rate)
         y_len = len(y)
         y_mix_len = len(y_mix)
         
 
         # use value of center sample as seed
         if start_at == None:
             rd_value = int(1000*y[int(y_len/2)])
```

### Comparing `augmolino-0.0.4/augmolino/augmenter.py` & `augmolino-0.0.5/augmolino/augmenter.py`

 * *Files identical despite different names*

### Comparing `augmolino-0.0.4/augmolino/utils.py` & `augmolino-0.0.5/augmolino/utils.py`

 * *Files identical despite different names*

### Comparing `augmolino-0.0.4/setup.py` & `augmolino-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(name='augmolino',
       packages=['augmolino'],
-      version='0.0.4',
+      version='0.0.5',
       description='augmentation for audio based datasets for machine learning',
       url='https://github.com/jake-is-ESD-protected/augmolino',
       download_url="https://github.com/jake-is-ESD-protected/augmolino/archive/refs/tags/0.0.2.tar.gz",
       author='Jakob Tschavoll',
       author_email='jt@tschavoll.at',
       license='GPL 3.0',
       classifiers=[],
```

### Comparing `augmolino-0.0.4/tests/test_augmentation.py` & `augmolino-0.0.5/tests/test_augmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,23 +140,23 @@
     x = a.run(test_file)
 
 
 def test_mixAudio_class():
     test_f_mix = "tests/sounds/speech.wav"
     test_ratio = 0.5
     test_start_at = 1
-    a = aug.mixAudio(test_ratio, test_start_at)
+    a = aug.mixAudio(test_f_mix, test_ratio, test_start_at)
 
     assert a.descriptor == aug.descriptors[aug.__all__[4]]
     assert a.function == a._mix
     assert len(a.kwargs) == 2
     assert a.tag == "0_5_1"
 
-    x = a.run(test_file, target_path, f_mix=test_f_mix)
-    assert len(a.kwargs) == 3
+    x = a.run(test_file, target_path)
+    assert len(a.kwargs) == 2
 
-    a = aug.mixAudio(test_ratio)
+    a = aug.mixAudio(test_f_mix, test_ratio)
     assert a.tag == "0_5_None"
-    x = a.run(test_file, target_path, f_mix=test_f_mix)
+    x = a.run(test_file, target_path)
 
 
     os.remove(target_path)
```

### Comparing `augmolino-0.0.4/tests/test_augmenter.py` & `augmolino-0.0.5/tests/test_augmenter.py`

 * *Files identical despite different names*

