# Comparing `tmp/sparse-lmm-0.7.tar.gz` & `tmp/sparse-lmm-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse-lmm-0.7.tar", last modified: Sun May 12 23:49:28 2024, max compression
+gzip compressed data, was "sparse-lmm-0.8.tar", last modified: Mon May 13 00:56:48 2024, max compression
```

## Comparing `sparse-lmm-0.7.tar` & `sparse-lmm-0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/
--rw-rw-r--   0 techt     (1000) techt     (1000)        8 2024-01-02 05:58:54.000000 sparse-lmm-0.7/.gitignore
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/.idea/
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/.idea/inspectionProfiles/
--rw-rw-r--   0 techt     (1000) techt     (1000)      174 2023-10-13 15:02:00.000000 sparse-lmm-0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)      177 2023-10-13 15:02:00.000000 sparse-lmm-0.7/.idea/misc.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)      300 2023-10-13 15:10:13.000000 sparse-lmm-0.7/.idea/modules.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)      441 2023-10-13 20:23:31.000000 sparse-lmm-0.7/.idea/sparse-lmm.iml
--rw-rw-r--   0 techt     (1000) techt     (1000)      180 2023-10-13 15:02:00.000000 sparse-lmm-0.7/.idea/vcs.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)    13922 2024-05-12 23:48:49.000000 sparse-lmm-0.7/.idea/workspace.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)     1071 2023-09-18 00:20:17.000000 sparse-lmm-0.7/LICENSE.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-12 23:49:28.138434 sparse-lmm-0.7/PKG-INFO
--rw-rw-r--   0 techt     (1000) techt     (1000)        0 2023-09-18 03:45:22.000000 sparse-lmm-0.7/README.md
--rw-rw-r--   0 techt     (1000) techt     (1000)    39332 2023-09-17 23:16:18.000000 sparse-lmm-0.7/combined_plots.png
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/dist/
--rw-rw-r--   0 techt     (1000) techt     (1000)    43128 2023-10-13 20:31:30.000000 sparse-lmm-0.7/dist/sparse-lmm-0.4.tar.gz
--rw-rw-r--   0 techt     (1000) techt     (1000)     7102 2023-10-13 20:31:30.000000 sparse-lmm-0.7/dist/sparse_lmm-0.4-py3-none-any.whl
--rw-rw-r--   0 techt     (1000) techt     (1000)       38 2024-05-12 23:49:28.138434 sparse-lmm-0.7/setup.cfg
--rw-rw-r--   0 techt     (1000) techt     (1000)      576 2024-05-12 23:49:14.000000 sparse-lmm-0.7/setup.py
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/sparse_lmm/
--rw-rw-r--   0 techt     (1000) techt     (1000)     9874 2024-05-12 23:29:04.000000 sparse-lmm-0.7/sparse_lmm/VariableSelection.py
--rw-rw-r--   0 techt     (1000) techt     (1000)     8341 2024-01-02 05:12:00.000000 sparse-lmm-0.7/sparse_lmm/VariableSelection_new.py
--rw-rw-r--   0 techt     (1000) techt     (1000)      236 2023-09-18 04:02:20.000000 sparse-lmm-0.7/sparse_lmm/__init__.py
--rw-rw-r--   0 techt     (1000) techt     (1000)    37017 2024-01-02 03:51:59.000000 sparse-lmm-0.7/sparse_lmm/combined_plots.png
--rwxrwxr-x   0 techt     (1000) techt     (1000)     5011 2023-09-14 18:54:06.000000 sparse-lmm-0.7/sparse_lmm/helpingMethods.py
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/sparse_lmm.egg-info/
--rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/PKG-INFO
--rw-rw-r--   0 techt     (1000) techt     (1000)      586 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/SOURCES.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)        1 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/dependency_links.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)       12 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/requires.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)       11 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/top_level.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)     1734 2023-10-13 01:48:51.000000 sparse-lmm-0.7/test.py
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/
+-rw-rw-r--   0 techt     (1000) techt     (1000)        8 2024-01-02 05:58:54.000000 sparse-lmm-0.8/.gitignore
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/.idea/
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/.idea/inspectionProfiles/
+-rw-rw-r--   0 techt     (1000) techt     (1000)      174 2023-10-13 15:02:00.000000 sparse-lmm-0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      177 2023-10-13 15:02:00.000000 sparse-lmm-0.8/.idea/misc.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      300 2023-10-13 15:10:13.000000 sparse-lmm-0.8/.idea/modules.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      441 2023-10-13 20:23:31.000000 sparse-lmm-0.8/.idea/sparse-lmm.iml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      180 2023-10-13 15:02:00.000000 sparse-lmm-0.8/.idea/vcs.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)    14213 2024-05-13 00:56:07.000000 sparse-lmm-0.8/.idea/workspace.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)     1071 2023-09-18 00:20:17.000000 sparse-lmm-0.8/LICENSE.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-13 00:56:48.031495 sparse-lmm-0.8/PKG-INFO
+-rw-rw-r--   0 techt     (1000) techt     (1000)        0 2023-09-18 03:45:22.000000 sparse-lmm-0.8/README.md
+-rw-rw-r--   0 techt     (1000) techt     (1000)    39332 2023-09-17 23:16:18.000000 sparse-lmm-0.8/combined_plots.png
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/dist/
+-rw-rw-r--   0 techt     (1000) techt     (1000)    43128 2023-10-13 20:31:30.000000 sparse-lmm-0.8/dist/sparse-lmm-0.4.tar.gz
+-rw-rw-r--   0 techt     (1000) techt     (1000)     7102 2023-10-13 20:31:30.000000 sparse-lmm-0.8/dist/sparse_lmm-0.4-py3-none-any.whl
+-rw-rw-r--   0 techt     (1000) techt     (1000)       38 2024-05-13 00:56:48.031495 sparse-lmm-0.8/setup.cfg
+-rw-rw-r--   0 techt     (1000) techt     (1000)      576 2024-05-13 00:54:10.000000 sparse-lmm-0.8/setup.py
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/sparse_lmm/
+-rw-rw-r--   0 techt     (1000) techt     (1000)     9815 2024-05-13 00:53:56.000000 sparse-lmm-0.8/sparse_lmm/VariableSelection.py
+-rw-rw-r--   0 techt     (1000) techt     (1000)     8341 2024-01-02 05:12:00.000000 sparse-lmm-0.8/sparse_lmm/VariableSelection_new.py
+-rw-rw-r--   0 techt     (1000) techt     (1000)      236 2023-09-18 04:02:20.000000 sparse-lmm-0.8/sparse_lmm/__init__.py
+-rw-rw-r--   0 techt     (1000) techt     (1000)    37017 2024-01-02 03:51:59.000000 sparse-lmm-0.8/sparse_lmm/combined_plots.png
+-rwxrwxr-x   0 techt     (1000) techt     (1000)     5011 2023-09-14 18:54:06.000000 sparse-lmm-0.8/sparse_lmm/helpingMethods.py
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-13 00:56:48.031495 sparse-lmm-0.8/sparse_lmm.egg-info/
+-rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-13 00:56:47.000000 sparse-lmm-0.8/sparse_lmm.egg-info/PKG-INFO
+-rw-rw-r--   0 techt     (1000) techt     (1000)      586 2024-05-13 00:56:48.000000 sparse-lmm-0.8/sparse_lmm.egg-info/SOURCES.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)        1 2024-05-13 00:56:47.000000 sparse-lmm-0.8/sparse_lmm.egg-info/dependency_links.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)       12 2024-05-13 00:56:47.000000 sparse-lmm-0.8/sparse_lmm.egg-info/requires.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)       11 2024-05-13 00:56:47.000000 sparse-lmm-0.8/sparse_lmm.egg-info/top_level.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)     1734 2023-10-13 01:48:51.000000 sparse-lmm-0.8/test.py
```

### Comparing `sparse-lmm-0.7/.idea/workspace.xml` & `sparse-lmm-0.8/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `sparse-lmm-0.7/.idea/workspace.xml` & `sparse-lmm-0.8/.idea/workspace.xml`

```diff
@@ -2,14 +2,16 @@
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="a73f1000-df80-42b0-bbec-78717e3dffc9" name="Changes" comment="only rotate x; remove intercept x0">
       <change beforePath="$PROJECT_DIR$/.idea/workspace.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/workspace.xml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/setup.py" beforeDir="false" afterPath="$PROJECT_DIR$/setup.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/sparse_lmm.egg-info/PKG-INFO" beforeDir="false" afterPath="$PROJECT_DIR$/sparse_lmm.egg-info/PKG-INFO" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/sparse_lmm/VariableSelection.py" beforeDir="false" afterPath="$PROJECT_DIR$/sparse_lmm/VariableSelection.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -34,21 +36,21 @@
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "SHARE_PROJECT_CONFIGURATION_FILES": "true",
     "WebServerToolWindowFactoryState": "false",
-    "last_opened_file_path": "/home/techt/Desktop/model/sparse-lmm/t1.py",
+    "last_opened_file_path": "/home/techt/Desktop/model/sparse-lmm/try1.py",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "settings.editor.selected.configurable": "web.server",
-    "two.files.diff.last.used.file": "/home/techt/Desktop/model/sparse-lmm/t1.py",
+    "two.files.diff.last.used.file": "/home/techt/Desktop/model/sparse-lmm/try1.py",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/precision_lasso"/>
     </key>
@@ -235,15 +237,15 @@
       <workItem from="1704830174041" duration="628000"/>
       <workItem from="1704920402164" duration="619000"/>
       <workItem from="1705458945901" duration="11000"/>
       <workItem from="1705614736560" duration="316000"/>
       <workItem from="1706066522765" duration="2781000"/>
       <workItem from="1711508793025" duration="1057000"/>
       <workItem from="1711761443949" duration="581000"/>
-      <workItem from="1715282022782" duration="7663000"/>
+      <workItem from="1715282022782" duration="10098000"/>
     </task>
     <task id="LOCAL-00001" summary="update">
       <created>1704167599803</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1704167599803</updated>
```

### Comparing `sparse-lmm-0.7/LICENSE.txt` & `sparse-lmm-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.7/combined_plots.png` & `sparse-lmm-0.8/combined_plots.png`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.7/dist/sparse-lmm-0.4.tar.gz` & `sparse-lmm-0.8/dist/sparse-lmm-0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.7/dist/sparse_lmm-0.4-py3-none-any.whl` & `sparse-lmm-0.8/dist/sparse_lmm-0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.7/setup.py` & `sparse-lmm-0.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sparse-lmm',
-    version='0.7',
+    version='0.8',
     packages=find_packages(),
     install_requires=['scipy', 'numpy'
                       ],
     author='Haohan Wang',
     author_email='haohanw@illinois.edu',
     description='An implementation of Linear Mixed Model, a statistical model that promotes sparse variable selection '
                 'in the presence of correlated and linearly dependent variables. ',
```

### Comparing `sparse-lmm-0.7/sparse_lmm/VariableSelection.py` & `sparse-lmm-0.8/sparse_lmm/VariableSelection.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 
 import time
 
 from .helpingMethods import *
 from sklearn.linear_model import Lasso
 
 class VariableSelection:
-    def __init__(self, modified=True, fit_intercept=False, lamda=0.1, numintervals=100, ldeltamin=-5, ldeltamax=5, scale=0, alpha=0.05, fdr=False,
+    def __init__(self, modified=True, lamda=0.1, numintervals=100, ldeltamin=-5, ldeltamax=5, scale=0, alpha=0.05, fdr=False,
                  acceleration=True,
                  quiet=True):
         self.numintervals = numintervals
         self.ldeltamin = ldeltamin
         self.ldeltamax = ldeltamax
         self.scale = scale
         self.alpha = alpha
         self.modified = modified  # Only rotate X, and apply Lasso instead of hypothesis test
-        self.fit_intercept = fit_intercept
         self.lamda = lamda  # Regularization coeffecient for Lasso.
         self.fdr = fdr
         self.ldelta0 = None
         self.quiet = quiet
         self.acceleration = acceleration
         self.K = None
 
@@ -76,17 +75,17 @@
         if not self.modified:
             self.SUy = SUy
             SUX0 = np.dot(self.U.T, X0)
             self.SUX0 = SUX0 * np.tile(Sdi_sqrt, (1, 1)).T
             self.X0 = X0
             self.neg_log_p, self.beta = self.hypothesisTest(self.SUX, self.SUy, X, self.SUX0, self.X0)
         else:
-            lasso = Lasso(alpha=self.lamda, fit_intercept=self.fit_intercept)
-            lasso.fit(self.SUX, self.y)
-            self.beta = lasso.coef_
+            self.lasso = Lasso(alpha=self.lamda)
+            self.lasso.fit(self.SUX, self.y)
+            self.beta = self.lasso.coef_
             self.neg_log_p = None
 
 
     def fit_detail(self, X, y):
         [n_s, n_f] = X.shape
         if self.K is None:
             self.K = np.dot(X, X.T)
@@ -240,15 +239,15 @@
         SUX_new = U_new * np.tile(Sdi_sqrt_new, (X_new.shape[1], 1)).T
 
         # Multiply the transformed data by beta coefficients to get predictions
         # Ensure beta is reshaped appropriately for matrix multiplication
         if self.beta.ndim == 1:
             self.beta = self.beta.reshape(-1, 1)
 
-        y_pred = np.dot(SUX_new, self.beta)
+        y_pred = np.dot(SUX_new, self.beta) + self.lasso.intercept_
 
         return y_pred.flatten()  # Flatten in case the output is a single sample
 
     def getBeta(self):
         return self.beta
 
 if __name__ == '__main__':
```

### Comparing `sparse-lmm-0.7/sparse_lmm/VariableSelection_new.py` & `sparse-lmm-0.8/sparse_lmm/VariableSelection_new.py`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.7/sparse_lmm/combined_plots.png` & `sparse-lmm-0.8/sparse_lmm/combined_plots.png`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.7/sparse_lmm/helpingMethods.py` & `sparse-lmm-0.8/sparse_lmm/helpingMethods.py`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.7/sparse_lmm.egg-info/SOURCES.txt` & `sparse-lmm-0.8/sparse_lmm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.7/test.py` & `sparse-lmm-0.8/test.py`

 * *Files identical despite different names*

