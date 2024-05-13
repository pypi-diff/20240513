# Comparing `tmp/opsys-spectrometer-0.0.2.tar.gz` & `tmp/opsys-spectrometer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Z:\opt\atlassian\pipelines\agent\build\dist\.tmp-1cnagpra\opsys-spectrometer-0.0.2.tar", last modified: Sun May 12 10:43:30 2024, max compression
+gzip compressed data, was "Z:\opt\atlassian\pipelines\agent\build\dist\.tmp-7izfmrqb\opsys-spectrometer-0.0.3.tar", last modified: Mon May 13 13:18:49 2024, max compression
```

## Comparing `opsys-spectrometer-0.0.2.tar` & `opsys-spectrometer-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      376 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1834 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/
--rw-rw-rw-   0        0        0      118 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/__init__.py
--rw-rw-rw-   0        0        0   392192 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/avaspecx64.dll
--rw-rw-rw-   0        0        0      551 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/spectrometer_abstract.py
--rw-rw-rw-   0        0        0     4603 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/opsys_spectrometer/spectrometer_controller.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/
--rw-rw-rw-   0        0        0      376 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-12 10:43:29.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      610 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1095 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:43:30.000000 opsys-spectrometer-0.0.2/test/
--rw-rw-rw-   0        0        0       78 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/test/__init__.py
--rw-rw-rw-   0        0        0     2686 2024-05-12 10:43:12.000000 opsys-spectrometer-0.0.2/test/test_spectrometer.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-05-13 13:18:23.000000 opsys-spectrometer-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      376 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1834 2024-05-13 13:18:23.000000 opsys-spectrometer-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/opsys_spectrometer/
+-rw-rw-rw-   0        0        0      118 2024-05-13 13:18:23.000000 opsys-spectrometer-0.0.3/opsys_spectrometer/__init__.py
+-rw-rw-rw-   0        0        0   392192 2024-05-13 13:18:24.000000 opsys-spectrometer-0.0.3/opsys_spectrometer/avaspecx64.dll
+-rw-rw-rw-   0        0        0      551 2024-05-13 13:18:23.000000 opsys-spectrometer-0.0.3/opsys_spectrometer/spectrometer_abstract.py
+-rw-rw-rw-   0        0        0     4682 2024-05-13 13:18:23.000000 opsys-spectrometer-0.0.3/opsys_spectrometer/spectrometer_controller.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/opsys_spectrometer.egg-info/
+-rw-rw-rw-   0        0        0      376 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/opsys_spectrometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/opsys_spectrometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/opsys_spectrometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-13 13:18:48.000000 opsys-spectrometer-0.0.3/opsys_spectrometer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      610 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/opsys_spectrometer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/opsys_spectrometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2024-05-13 13:18:23.000000 opsys-spectrometer-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:18:49.000000 opsys-spectrometer-0.0.3/test/
+-rw-rw-rw-   0        0        0       78 2024-05-13 13:18:23.000000 opsys-spectrometer-0.0.3/test/__init__.py
+-rw-rw-rw-   0        0        0     2686 2024-05-13 13:18:23.000000 opsys-spectrometer-0.0.3/test/test_spectrometer.py
```

### Comparing `opsys-spectrometer-0.0.2/LICENSE` & `opsys-spectrometer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opsys-spectrometer-0.0.2/README.md` & `opsys-spectrometer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `opsys-spectrometer-0.0.2/opsys_spectrometer/avaspecx64.dll` & `opsys-spectrometer-0.0.3/opsys_spectrometer/avaspecx64.dll`

 * *Files identical despite different names*

### Comparing `opsys-spectrometer-0.0.2/opsys_spectrometer/spectrometer_abstract.py` & `opsys-spectrometer-0.0.3/opsys_spectrometer/spectrometer_abstract.py`

 * *Files identical despite different names*

### Comparing `opsys-spectrometer-0.0.2/opsys_spectrometer/spectrometer_controller.py` & `opsys-spectrometer-0.0.3/opsys_spectrometer/spectrometer_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,16 @@
     def get_peak_value(self):
         """
         Get max measured value
 
         Returns:
             float: max measured value
         """
-        peak = max(self.data)
+        peak_index = max(self.data)
+        peak = self.get_lambda()[np.where(self.data==peak_index)[0][0]]
             
         return round(peak, 3)
     
     def get_fwhm(self):
         """
         Get Full Width at Half Max value,
         for given x and y values
```

### Comparing `opsys-spectrometer-0.0.2/opsys_spectrometer.egg-info/requires.txt` & `opsys-spectrometer-0.0.3/opsys_spectrometer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `opsys-spectrometer-0.0.2/setup.py` & `opsys-spectrometer-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     if fname.exists():
         with open(fname, 'r') as f:
             targets = f.read().splitlines()
     return targets
 
 
 setuptools.setup(name='opsys-spectrometer',
-                 version='0.0.2',
+                 version='0.0.3',
                  description='python package for wavelength measuring devices',
                  url='https://bitbucket.org/opsys_tech/opsys-spectrometer/src/master/',
                  download_url='https://bitbucket.org/opsys_tech/opsys-spectrometer/src/master/',
                  author='dmitry.borovensky',
                  install_requires=get_install_requirements(),
                  author_email='dmitry.borovensky@opsys-tech.com',
                  packages=setuptools.find_packages(),
```

### Comparing `opsys-spectrometer-0.0.2/test/test_spectrometer.py` & `opsys-spectrometer-0.0.3/test/test_spectrometer.py`

 * *Files identical despite different names*

