# Comparing `tmp/sparse-lmm-0.6.tar.gz` & `tmp/sparse-lmm-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse-lmm-0.6.tar", last modified: Tue Jan  9 04:25:59 2024, max compression
+gzip compressed data, was "sparse-lmm-0.7.tar", last modified: Sun May 12 23:49:28 2024, max compression
```

## Comparing `sparse-lmm-0.6.tar` & `sparse-lmm-0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-01-09 04:25:59.879008 sparse-lmm-0.6/
--rw-rw-r--   0 techt     (1000) techt     (1000)        8 2024-01-02 05:58:54.000000 sparse-lmm-0.6/.gitignore
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-01-09 04:25:59.875008 sparse-lmm-0.6/.idea/
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-01-09 04:25:59.875008 sparse-lmm-0.6/.idea/inspectionProfiles/
--rw-rw-r--   0 techt     (1000) techt     (1000)      174 2023-10-13 15:02:00.000000 sparse-lmm-0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)      177 2023-10-13 15:02:00.000000 sparse-lmm-0.6/.idea/misc.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)      300 2023-10-13 15:10:13.000000 sparse-lmm-0.6/.idea/modules.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)      441 2023-10-13 20:23:31.000000 sparse-lmm-0.6/.idea/sparse-lmm.iml
--rw-rw-r--   0 techt     (1000) techt     (1000)      180 2023-10-13 15:02:00.000000 sparse-lmm-0.6/.idea/vcs.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)    13382 2024-01-09 04:25:52.000000 sparse-lmm-0.6/.idea/workspace.xml
--rw-rw-r--   0 techt     (1000) techt     (1000)     1071 2023-09-18 00:20:17.000000 sparse-lmm-0.6/LICENSE.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-01-09 04:25:59.879008 sparse-lmm-0.6/PKG-INFO
--rw-rw-r--   0 techt     (1000) techt     (1000)        0 2023-09-18 03:45:22.000000 sparse-lmm-0.6/README.md
--rw-rw-r--   0 techt     (1000) techt     (1000)    39332 2023-09-17 23:16:18.000000 sparse-lmm-0.6/combined_plots.png
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-01-09 04:25:59.879008 sparse-lmm-0.6/dist/
--rw-rw-r--   0 techt     (1000) techt     (1000)    43128 2023-10-13 20:31:30.000000 sparse-lmm-0.6/dist/sparse-lmm-0.4.tar.gz
--rw-rw-r--   0 techt     (1000) techt     (1000)     7102 2023-10-13 20:31:30.000000 sparse-lmm-0.6/dist/sparse_lmm-0.4-py3-none-any.whl
--rw-rw-r--   0 techt     (1000) techt     (1000)       38 2024-01-09 04:25:59.879008 sparse-lmm-0.6/setup.cfg
--rw-rw-r--   0 techt     (1000) techt     (1000)      576 2024-01-09 04:25:36.000000 sparse-lmm-0.6/setup.py
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-01-09 04:25:59.879008 sparse-lmm-0.6/sparse_lmm/
--rw-rw-r--   0 techt     (1000) techt     (1000)     8752 2024-01-09 04:24:54.000000 sparse-lmm-0.6/sparse_lmm/VariableSelection.py
--rw-rw-r--   0 techt     (1000) techt     (1000)     8341 2024-01-02 05:12:00.000000 sparse-lmm-0.6/sparse_lmm/VariableSelection_new.py
--rw-rw-r--   0 techt     (1000) techt     (1000)      236 2023-09-18 04:02:20.000000 sparse-lmm-0.6/sparse_lmm/__init__.py
--rw-rw-r--   0 techt     (1000) techt     (1000)    37017 2024-01-02 03:51:59.000000 sparse-lmm-0.6/sparse_lmm/combined_plots.png
--rwxrwxr-x   0 techt     (1000) techt     (1000)     5011 2023-09-14 18:54:06.000000 sparse-lmm-0.6/sparse_lmm/helpingMethods.py
-drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-01-09 04:25:59.879008 sparse-lmm-0.6/sparse_lmm.egg-info/
--rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-01-09 04:25:59.000000 sparse-lmm-0.6/sparse_lmm.egg-info/PKG-INFO
--rw-rw-r--   0 techt     (1000) techt     (1000)      586 2024-01-09 04:25:59.000000 sparse-lmm-0.6/sparse_lmm.egg-info/SOURCES.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)        1 2024-01-09 04:25:59.000000 sparse-lmm-0.6/sparse_lmm.egg-info/dependency_links.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)       12 2024-01-09 04:25:59.000000 sparse-lmm-0.6/sparse_lmm.egg-info/requires.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)       11 2024-01-09 04:25:59.000000 sparse-lmm-0.6/sparse_lmm.egg-info/top_level.txt
--rw-rw-r--   0 techt     (1000) techt     (1000)     1734 2023-10-13 01:48:51.000000 sparse-lmm-0.6/test.py
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/
+-rw-rw-r--   0 techt     (1000) techt     (1000)        8 2024-01-02 05:58:54.000000 sparse-lmm-0.7/.gitignore
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/.idea/
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/.idea/inspectionProfiles/
+-rw-rw-r--   0 techt     (1000) techt     (1000)      174 2023-10-13 15:02:00.000000 sparse-lmm-0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      177 2023-10-13 15:02:00.000000 sparse-lmm-0.7/.idea/misc.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      300 2023-10-13 15:10:13.000000 sparse-lmm-0.7/.idea/modules.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      441 2023-10-13 20:23:31.000000 sparse-lmm-0.7/.idea/sparse-lmm.iml
+-rw-rw-r--   0 techt     (1000) techt     (1000)      180 2023-10-13 15:02:00.000000 sparse-lmm-0.7/.idea/vcs.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)    13922 2024-05-12 23:48:49.000000 sparse-lmm-0.7/.idea/workspace.xml
+-rw-rw-r--   0 techt     (1000) techt     (1000)     1071 2023-09-18 00:20:17.000000 sparse-lmm-0.7/LICENSE.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-12 23:49:28.138434 sparse-lmm-0.7/PKG-INFO
+-rw-rw-r--   0 techt     (1000) techt     (1000)        0 2023-09-18 03:45:22.000000 sparse-lmm-0.7/README.md
+-rw-rw-r--   0 techt     (1000) techt     (1000)    39332 2023-09-17 23:16:18.000000 sparse-lmm-0.7/combined_plots.png
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/dist/
+-rw-rw-r--   0 techt     (1000) techt     (1000)    43128 2023-10-13 20:31:30.000000 sparse-lmm-0.7/dist/sparse-lmm-0.4.tar.gz
+-rw-rw-r--   0 techt     (1000) techt     (1000)     7102 2023-10-13 20:31:30.000000 sparse-lmm-0.7/dist/sparse_lmm-0.4-py3-none-any.whl
+-rw-rw-r--   0 techt     (1000) techt     (1000)       38 2024-05-12 23:49:28.138434 sparse-lmm-0.7/setup.cfg
+-rw-rw-r--   0 techt     (1000) techt     (1000)      576 2024-05-12 23:49:14.000000 sparse-lmm-0.7/setup.py
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/sparse_lmm/
+-rw-rw-r--   0 techt     (1000) techt     (1000)     9874 2024-05-12 23:29:04.000000 sparse-lmm-0.7/sparse_lmm/VariableSelection.py
+-rw-rw-r--   0 techt     (1000) techt     (1000)     8341 2024-01-02 05:12:00.000000 sparse-lmm-0.7/sparse_lmm/VariableSelection_new.py
+-rw-rw-r--   0 techt     (1000) techt     (1000)      236 2023-09-18 04:02:20.000000 sparse-lmm-0.7/sparse_lmm/__init__.py
+-rw-rw-r--   0 techt     (1000) techt     (1000)    37017 2024-01-02 03:51:59.000000 sparse-lmm-0.7/sparse_lmm/combined_plots.png
+-rwxrwxr-x   0 techt     (1000) techt     (1000)     5011 2023-09-14 18:54:06.000000 sparse-lmm-0.7/sparse_lmm/helpingMethods.py
+drwxrwxr-x   0 techt     (1000) techt     (1000)        0 2024-05-12 23:49:28.138434 sparse-lmm-0.7/sparse_lmm.egg-info/
+-rw-rw-r--   0 techt     (1000) techt     (1000)      410 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/PKG-INFO
+-rw-rw-r--   0 techt     (1000) techt     (1000)      586 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/SOURCES.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)        1 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/dependency_links.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)       12 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/requires.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)       11 2024-05-12 23:49:28.000000 sparse-lmm-0.7/sparse_lmm.egg-info/top_level.txt
+-rw-rw-r--   0 techt     (1000) techt     (1000)     1734 2023-10-13 01:48:51.000000 sparse-lmm-0.7/test.py
```

### Comparing `sparse-lmm-0.6/.idea/workspace.xml` & `sparse-lmm-0.7/.idea/workspace.xml`

 * *Files 6% similar despite different names*

#### Comparing `sparse-lmm-0.6/.idea/workspace.xml` & `sparse-lmm-0.7/.idea/workspace.xml`

```diff
@@ -2,27 +2,25 @@
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="a73f1000-df80-42b0-bbec-78717e3dffc9" name="Changes" comment="only rotate x; remove intercept x0">
       <change beforePath="$PROJECT_DIR$/.idea/workspace.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/workspace.xml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/setup.py" beforeDir="false" afterPath="$PROJECT_DIR$/setup.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/sparse_lmm.egg-info/PKG-INFO" beforeDir="false" afterPath="$PROJECT_DIR$/sparse_lmm.egg-info/PKG-INFO" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/sparse_lmm.egg-info/SOURCES.txt" beforeDir="false" afterPath="$PROJECT_DIR$/sparse_lmm.egg-info/SOURCES.txt" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/sparse_lmm/VariableSelection.py" beforeDir="false" afterPath="$PROJECT_DIR$/sparse_lmm/VariableSelection.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
       <list>
+        <option value="Jupyter Notebook"/>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
@@ -36,21 +34,21 @@
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "SHARE_PROJECT_CONFIGURATION_FILES": "true",
     "WebServerToolWindowFactoryState": "false",
-    "last_opened_file_path": "/home/techt/Desktop/model/sparse-lmm/sparse_lmm/VariableSelection_new.py",
+    "last_opened_file_path": "/home/techt/Desktop/model/sparse-lmm/t1.py",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "settings.editor.selected.configurable": "web.server",
-    "two.files.diff.last.used.file": "/home/techt/Desktop/model/sparse-lmm/sparse_lmm/VariableSelection_new.py",
+    "two.files.diff.last.used.file": "/home/techt/Desktop/model/sparse-lmm/t1.py",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/precision_lasso"/>
     </key>
@@ -229,15 +227,23 @@
       <workItem from="1704167271390" duration="109000"/>
       <workItem from="1704167384890" duration="2571000"/>
       <workItem from="1704309568439" duration="599000"/>
       <workItem from="1704394975741" duration="1203000"/>
       <workItem from="1704470301522" duration="598000"/>
       <workItem from="1704555791237" duration="1855000"/>
       <workItem from="1704651860725" duration="910000"/>
-      <workItem from="1704728143675" duration="4875000"/>
+      <workItem from="1704728143675" duration="5645000"/>
+      <workItem from="1704830174041" duration="628000"/>
+      <workItem from="1704920402164" duration="619000"/>
+      <workItem from="1705458945901" duration="11000"/>
+      <workItem from="1705614736560" duration="316000"/>
+      <workItem from="1706066522765" duration="2781000"/>
+      <workItem from="1711508793025" duration="1057000"/>
+      <workItem from="1711761443949" duration="581000"/>
+      <workItem from="1715282022782" duration="7663000"/>
     </task>
     <task id="LOCAL-00001" summary="update">
       <created>1704167599803</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1704167599803</updated>
@@ -245,15 +251,22 @@
     <task id="LOCAL-00002" summary="only rotate x; remove intercept x0">
       <created>1704175197733</created>
       <option name="number" value="00002"/>
       <option name="presentableId" value="LOCAL-00002"/>
       <option name="project" value="LOCAL"/>
       <updated>1704175197733</updated>
     </task>
-    <option name="localTasksCounter" value="3"/>
+    <task id="LOCAL-00003" summary="only rotate x; remove intercept x0">
+      <created>1705614771590</created>
+      <option name="number" value="00003"/>
+      <option name="presentableId" value="LOCAL-00003"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1705614771590</updated>
+    </task>
+    <option name="localTasksCounter" value="4"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.History.Properties">
     <option name="COLUMN_ID_ORDER">
@@ -262,13 +275,24 @@
         <option value="Default.Author"/>
         <option value="Default.Date"/>
         <option value="Default.Subject"/>
         <option value="Space.CommitStatus"/>
       </list>
     </option>
   </component>
+  <component name="Vcs.Log.Tabs.Properties">
+    <option name="TAB_STATES">
+      <map>
+        <entry key="MAIN">
+          <value>
+            <State/>
+          </value>
+        </entry>
+      </map>
+    </option>
+  </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="update"/>
     <MESSAGE value="only rotate x; remove intercept x0"/>
     <option name="LAST_COMMIT_MESSAGE" value="only rotate x; remove intercept x0"/>
   </component>
 </project>
```

### Comparing `sparse-lmm-0.6/LICENSE.txt` & `sparse-lmm-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.6/combined_plots.png` & `sparse-lmm-0.7/combined_plots.png`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.6/dist/sparse-lmm-0.4.tar.gz` & `sparse-lmm-0.7/dist/sparse-lmm-0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.6/dist/sparse_lmm-0.4-py3-none-any.whl` & `sparse-lmm-0.7/dist/sparse_lmm-0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.6/setup.py` & `sparse-lmm-0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sparse-lmm',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     install_requires=['scipy', 'numpy'
                       ],
     author='Haohan Wang',
     author_email='haohanw@illinois.edu',
     description='An implementation of Linear Mixed Model, a statistical model that promotes sparse variable selection '
                 'in the presence of correlated and linearly dependent variables. ',
```

### Comparing `sparse-lmm-0.6/sparse_lmm/VariableSelection.py` & `sparse-lmm-0.7/sparse_lmm/VariableSelection_new.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import scipy.optimize as opt
 import numpy.linalg as linalg
 
 import time
 
-from .helpingMethods import *
+from helpingMethods import *
 from sklearn.linear_model import Lasso
 
 class VariableSelection:
-    def __init__(self, modified=True, lamda=0.1, numintervals=100, ldeltamin=-5, ldeltamax=5, scale=0, alpha=0.05, fdr=False,
+    def __init__(self, lamda, numintervals=100, ldeltamin=-5, ldeltamax=5, scale=0, alpha=0.05, fdr=False,
                  acceleration=True,
                  quiet=True):
         self.numintervals = numintervals
         self.ldeltamin = ldeltamin
         self.ldeltamax = ldeltamax
         self.scale = scale
         self.alpha = alpha
-        self.modified = modified  # Only rotate X, and apply Lasso instead of hypothesis test
-        self.lamda = lamda  # Regularization coeffecient for Lasso.
+        self.lamda = lamda  # A important parameter. Regularization coeffecient for Lasso.
         self.fdr = fdr
         self.ldelta0 = None
         self.quiet = quiet
         self.acceleration = acceleration
         self.K = None
 
     def estimateDelta(self, y):
@@ -53,41 +52,38 @@
 
         if y.ndim == 1:
             y = np.reshape(y, (n_s, 1))
 
         self.y = y
         self.S, self.U, ldelta0= self.train_nullmodel(self.y, self.K)
 
+        # if self.ldelta0 is None:
+        #     self.ldelta0 = ldelta0
         self.ldelta0 = ldelta0
 
-        if not self.modified:
-            X0 = np.ones(len(self.y)).reshape(len(self.y), 1)
+        # X0 = np.ones(len(self.y)).reshape(len(self.y), 1)
 
         delta0 = np.exp(self.ldelta0)
         Sdi = 1. / (self.S + delta0)
         Sdi_sqrt = np.sqrt(Sdi)
         SUX = np.dot(self.U.T, X)
         SUX = SUX * np.tile(Sdi_sqrt, (n_f, 1)).T
-        if not self.modified:
-            SUy = np.dot(self.U.T, self.y)
-            SUy = SUy * Sdi_sqrt.reshape((n_s, 1))
+        # SUy = np.dot(self.U.T, self.y)
+        # SUy = SUy * Sdi_sqrt.reshape((n_s, 1))
 
         self.SUX = SUX
-        if not self.modified:
-            self.SUy = SUy
-            SUX0 = np.dot(self.U.T, X0)
-            self.SUX0 = SUX0 * np.tile(Sdi_sqrt, (1, 1)).T
-            self.X0 = X0
-            self.neg_log_p, self.beta = self.hypothesisTest(self.SUX, self.SUy, X, self.SUX0, self.X0)
-        else:
-            print(f'alpha for Lasso: {self.lamda}')
-            lasso = Lasso(alpha=self.lamda)
-            lasso.fit(self.SUX, self.y)
-            self.beta = lasso.coef_
-            self.neg_log_p = None
+        # self.SUy = SUy
+        # SUX0 = np.dot(self.U.T, X0)
+        # self.SUX0 = SUX0 * np.tile(Sdi_sqrt, (1, 1)).T
+        # self.X0 = X0
+        # self.neg_log_p, self.beta = self.hypothesisTest(self.SUX, self.SUy, X, self.SUX0, self.X0)
+        print(f'alpha for Lasso: {self.lamda}')
+        lasso = Lasso(alpha=self.lamda)
+        lasso.fit(self.SUX, self.y)
+        self.beta = lasso.coef_
 
 
     def fit_detail(self, X, y):
         [n_s, n_f] = X.shape
         if self.K is None:
             self.K = np.dot(X, X.T)
 
@@ -150,22 +146,14 @@
         threshold = 1e-8
         n = len(tmp)
         for i in range(n):
             if tmp[i] < (i+1)*self.alpha/n:
                 threshold = tmp[i]
         self.neg_log_p[self.neg_log_p<-np.log(threshold)] = 0
 
-    def getNegLogP(self):
-        if self.neg_log_p is None:
-            return None
-        if not self.fdr:
-            return self.neg_log_p
-        else:
-            self.fdrControl()
-            return self.neg_log_p
 
     def hypothesisTest(self, UX, Uy, X, UX0, X0):
         [m, n] = X.shape
         p = []
         betas = []
         for i in range(n):
             if UX0 is not None:
```

### Comparing `sparse-lmm-0.6/sparse_lmm/VariableSelection_new.py` & `sparse-lmm-0.7/sparse_lmm/VariableSelection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import scipy.optimize as opt
 import numpy.linalg as linalg
 
 import time
 
-from helpingMethods import *
+from .helpingMethods import *
 from sklearn.linear_model import Lasso
 
 class VariableSelection:
-    def __init__(self, lamda, numintervals=100, ldeltamin=-5, ldeltamax=5, scale=0, alpha=0.05, fdr=False,
+    def __init__(self, modified=True, fit_intercept=False, lamda=0.1, numintervals=100, ldeltamin=-5, ldeltamax=5, scale=0, alpha=0.05, fdr=False,
                  acceleration=True,
                  quiet=True):
         self.numintervals = numintervals
         self.ldeltamin = ldeltamin
         self.ldeltamax = ldeltamax
         self.scale = scale
         self.alpha = alpha
-        self.lamda = lamda  # A important parameter. Regularization coeffecient for Lasso.
+        self.modified = modified  # Only rotate X, and apply Lasso instead of hypothesis test
+        self.fit_intercept = fit_intercept
+        self.lamda = lamda  # Regularization coeffecient for Lasso.
         self.fdr = fdr
         self.ldelta0 = None
         self.quiet = quiet
         self.acceleration = acceleration
         self.K = None
 
     def estimateDelta(self, y):
@@ -52,38 +54,40 @@
 
         if y.ndim == 1:
             y = np.reshape(y, (n_s, 1))
 
         self.y = y
         self.S, self.U, ldelta0= self.train_nullmodel(self.y, self.K)
 
-        # if self.ldelta0 is None:
-        #     self.ldelta0 = ldelta0
         self.ldelta0 = ldelta0
 
-        # X0 = np.ones(len(self.y)).reshape(len(self.y), 1)
+        if not self.modified:
+            X0 = np.ones(len(self.y)).reshape(len(self.y), 1)
 
         delta0 = np.exp(self.ldelta0)
         Sdi = 1. / (self.S + delta0)
         Sdi_sqrt = np.sqrt(Sdi)
         SUX = np.dot(self.U.T, X)
         SUX = SUX * np.tile(Sdi_sqrt, (n_f, 1)).T
-        # SUy = np.dot(self.U.T, self.y)
-        # SUy = SUy * Sdi_sqrt.reshape((n_s, 1))
+        if not self.modified:
+            SUy = np.dot(self.U.T, self.y)
+            SUy = SUy * Sdi_sqrt.reshape((n_s, 1))
 
         self.SUX = SUX
-        # self.SUy = SUy
-        # SUX0 = np.dot(self.U.T, X0)
-        # self.SUX0 = SUX0 * np.tile(Sdi_sqrt, (1, 1)).T
-        # self.X0 = X0
-        # self.neg_log_p, self.beta = self.hypothesisTest(self.SUX, self.SUy, X, self.SUX0, self.X0)
-        print(f'alpha for Lasso: {self.lamda}')
-        lasso = Lasso(alpha=self.lamda)
-        lasso.fit(self.SUX, self.y)
-        self.beta = lasso.coef_
+        if not self.modified:
+            self.SUy = SUy
+            SUX0 = np.dot(self.U.T, X0)
+            self.SUX0 = SUX0 * np.tile(Sdi_sqrt, (1, 1)).T
+            self.X0 = X0
+            self.neg_log_p, self.beta = self.hypothesisTest(self.SUX, self.SUy, X, self.SUX0, self.X0)
+        else:
+            lasso = Lasso(alpha=self.lamda, fit_intercept=self.fit_intercept)
+            lasso.fit(self.SUX, self.y)
+            self.beta = lasso.coef_
+            self.neg_log_p = None
 
 
     def fit_detail(self, X, y):
         [n_s, n_f] = X.shape
         if self.K is None:
             self.K = np.dot(X, X.T)
 
@@ -146,14 +150,22 @@
         threshold = 1e-8
         n = len(tmp)
         for i in range(n):
             if tmp[i] < (i+1)*self.alpha/n:
                 threshold = tmp[i]
         self.neg_log_p[self.neg_log_p<-np.log(threshold)] = 0
 
+    def getNegLogP(self):
+        if self.neg_log_p is None:
+            return None
+        if not self.fdr:
+            return self.neg_log_p
+        else:
+            self.fdrControl()
+            return self.neg_log_p
 
     def hypothesisTest(self, UX, Uy, X, UX0, X0):
         [m, n] = X.shape
         p = []
         betas = []
         for i in range(n):
             if UX0 is not None:
@@ -206,14 +218,40 @@
                                                               (ldeltagrid[i - 1], ldeltagrid[i], ldeltagrid[i + 1]),
                                                               full_output=True)
                 if nllopt < nllmin:
                     nllmin = nllopt
                     ldeltaopt_glob = ldeltaopt
         return S, U, ldeltaopt_glob
 
+    def predict(self, X_new):
+        if X_new.ndim == 1:
+            X_new = X_new.reshape(1, -1)
+
+        # Check if necessary parameters are initialized
+        if self.K is None or self.U is None or self.S is None:
+            raise ValueError("Model has not been properly initialized with training data.")
+
+        # Project the new data using the U matrix derived from training
+        U_new = np.dot(X_new, self.U)
+
+        # Scale the transformed data by the diagonal matrix Sdi_sqrt derived from training
+        delta0_new = np.exp(self.ldelta0)
+        Sdi_new = 1. / (self.S + delta0_new)
+        Sdi_sqrt_new = np.sqrt(Sdi_new)
+        SUX_new = U_new * np.tile(Sdi_sqrt_new, (X_new.shape[1], 1)).T
+
+        # Multiply the transformed data by beta coefficients to get predictions
+        # Ensure beta is reshaped appropriately for matrix multiplication
+        if self.beta.ndim == 1:
+            self.beta = self.beta.reshape(-1, 1)
+
+        y_pred = np.dot(SUX_new, self.beta)
+
+        return y_pred.flatten()  # Flatten in case the output is a single sample
+
     def getBeta(self):
         return self.beta
 
 if __name__ == '__main__':
 
     from matplotlib import pyplot as plt
```

### Comparing `sparse-lmm-0.6/sparse_lmm/combined_plots.png` & `sparse-lmm-0.7/sparse_lmm/combined_plots.png`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.6/sparse_lmm/helpingMethods.py` & `sparse-lmm-0.7/sparse_lmm/helpingMethods.py`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.6/sparse_lmm.egg-info/SOURCES.txt` & `sparse-lmm-0.7/sparse_lmm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparse-lmm-0.6/test.py` & `sparse-lmm-0.7/test.py`

 * *Files identical despite different names*

