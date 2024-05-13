# Comparing `tmp/pyfemtet-0.4.1.tar.gz` & `tmp/pyfemtet-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfemtet-0.4.1.tar", max compression
+gzip compressed data, was "pyfemtet-0.4.2.tar", max compression
```

## Comparing `pyfemtet-0.4.1.tar` & `pyfemtet-0.4.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1485 2024-04-10 06:20:51.769757 pyfemtet-0.4.1/LICENSE
--rw-r--r--   0        0        0      387 2024-04-10 06:20:51.769757 pyfemtet-0.4.1/README.md
--rw-r--r--   0        0        0   170268 2024-04-10 06:20:51.769757 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.femprj
--rw-r--r--   0        0        0   226626 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.prt
--rw-r--r--   0        0        0     3064 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.py
--rw-r--r--   0        0        0    83094 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.SLDPRT
--rw-r--r--   0        0        0   155307 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.femprj
--rw-r--r--   0        0        0     3901 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.py
--rw-r--r--   0        0        0   268761 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/gau_ex08_parametric.femprj
--rw-r--r--   0        0        0     2013 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/gau_ex08_parametric.py
--rw-r--r--   0        0        0   126336 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/her_ex40_parametric.femprj
--rw-r--r--   0        0        0     5172 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/her_ex40_parametric.py
--rw-r--r--   0        0        0     2401 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/wat_ex14_parallel_parametric.py
--rw-r--r--   0        0        0   172895 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/wat_ex14_parametric.femprj
--rw-r--r--   0        0        0     2289 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/wat_ex14_parametric.py
--rw-r--r--   0        0        0       21 2024-04-10 06:21:06.921794 pyfemtet-0.4.1/pyfemtet/__init__.py
--rw-r--r--   0        0        0     1386 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/core.py
--rw-r--r--   0        0        0    16177 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/dispatch_extensions.py
--rw-r--r--   0        0        0     2507 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/logger.py
--rw-r--r--   0        0        0      596 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/__init__.py
--rw-r--r--   0        0        0    20602 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/_femopt.py
--rw-r--r--   0        0        0    24331 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/_femopt_core.py
--rw-r--r--   0        0        0      480 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/interface/__init__.py
--rw-r--r--   0        0        0     2079 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/interface/_base.py
--rw-r--r--   0        0        0    24428 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/interface/_femtet.py
--rw-r--r--   0        0        0       83 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/interface/_femtet_with_nx/__init__.py
--rw-r--r--   0        0        0     4192 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/interface/_femtet_with_nx/_interface.py
--rw-r--r--   0        0        0     2856 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/interface/_femtet_with_nx/update_model.py
--rw-r--r--   0        0        0     6515 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/interface/_femtet_with_sldworks.py
--rw-r--r--   0        0        0      191 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/opt/__init__.py
--rw-r--r--   0        0        0     7101 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/opt/_base.py
--rw-r--r--   0        0        0     9506 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/opt/_optuna.py
--rw-r--r--   0        0        0      193 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/visualization/__init__.py
--rw-r--r--   0        0        0     5306 2024-04-10 06:20:51.773758 pyfemtet-0.4.1/pyfemtet/opt/visualization/_graphs.py
--rw-r--r--   0        0        0    42104 2024-04-10 06:20:51.777758 pyfemtet-0.4.1/pyfemtet/opt/visualization/_monitor.py
--rw-r--r--   0        0        0     1314 2024-04-10 06:21:06.921794 pyfemtet-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 pyfemtet-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1485 2024-05-13 11:07:43.197936 pyfemtet-0.4.2/LICENSE
+-rw-r--r--   0        0        0      483 2024-05-13 11:07:43.197936 pyfemtet-0.4.2/README.md
+-rw-r--r--   0        0        0   170268 2024-05-13 11:07:43.293937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.femprj
+-rw-r--r--   0        0        0   226626 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.prt
+-rw-r--r--   0        0        0     3980 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.py
+-rw-r--r--   0        0        0    83094 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.SLDPRT
+-rw-r--r--   0        0        0   155307 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.femprj
+-rw-r--r--   0        0        0     4182 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.py
+-rw-r--r--   0        0        0   268761 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/gau_ex08_parametric.femprj
+-rw-r--r--   0        0        0     1799 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/gau_ex08_parametric.py
+-rw-r--r--   0        0        0   126336 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/her_ex40_parametric.femprj
+-rw-r--r--   0        0        0     5144 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/her_ex40_parametric.py
+-rw-r--r--   0        0        0     2148 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parallel_parametric.py
+-rw-r--r--   0        0        0   172895 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parametric.femprj
+-rw-r--r--   0        0        0     2052 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parametric.py
+-rw-r--r--   0        0        0       21 2024-05-13 11:07:55.278068 pyfemtet-0.4.2/pyfemtet/__init__.py
+-rw-r--r--   0        0        0     1386 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/core.py
+-rw-r--r--   0        0        0    16177 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/dispatch_extensions.py
+-rw-r--r--   0        0        0     2507 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/logger.py
+-rw-r--r--   0        0        0      596 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/__init__.py
+-rw-r--r--   0        0        0    20602 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/_femopt.py
+-rw-r--r--   0        0        0    24361 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/_femopt_core.py
+-rw-r--r--   0        0        0      480 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/__init__.py
+-rw-r--r--   0        0        0     2079 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_base.py
+-rw-r--r--   0        0        0    24439 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet.py
+-rw-r--r--   0        0        0       83 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/__init__.py
+-rw-r--r--   0        0        0     4192 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/_interface.py
+-rw-r--r--   0        0        0     2856 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/update_model.py
+-rw-r--r--   0        0        0     6515 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_sldworks.py
+-rw-r--r--   0        0        0      191 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/opt/__init__.py
+-rw-r--r--   0        0        0     7101 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/opt/_base.py
+-rw-r--r--   0        0        0     9996 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/opt/_optuna.py
+-rw-r--r--   0        0        0      193 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/visualization/__init__.py
+-rw-r--r--   0        0        0     5306 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/visualization/_graphs.py
+-rw-r--r--   0        0        0    42104 2024-05-13 11:07:43.297937 pyfemtet-0.4.2/pyfemtet/opt/visualization/_monitor.py
+-rw-r--r--   0        0        0     1360 2024-05-13 11:07:55.278068 pyfemtet-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 pyfemtet-0.4.2/PKG-INFO
```

### Comparing `pyfemtet-0.4.1/LICENSE` & `pyfemtet-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.femprj` & `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.prt` & `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/NX_ex01/NX_ex01.prt`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.SLDPRT` & `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.SLDPRT`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.femprj` & `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/Sldworks_ex01/Sldworks_ex01.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/gau_ex08_parametric.femprj` & `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/gau_ex08_parametric.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/her_ex40_parametric.femprj` & `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/her_ex40_parametric.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/FemtetPJTSample/wat_ex14_parametric.femprj` & `pyfemtet-0.4.2/pyfemtet/FemtetPJTSample/wat_ex14_parametric.femprj`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/core.py` & `pyfemtet-0.4.2/pyfemtet/core.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/dispatch_extensions.py` & `pyfemtet-0.4.2/pyfemtet/dispatch_extensions.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/logger.py` & `pyfemtet-0.4.2/pyfemtet/logger.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/__init__.py` & `pyfemtet-0.4.2/pyfemtet/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/_femopt.py` & `pyfemtet-0.4.2/pyfemtet/opt/_femopt.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/_femopt_core.py` & `pyfemtet-0.4.2/pyfemtet/opt/_femopt_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,14 @@
     """
 
     HEADER_ROW = 2
     ENCODING = 'cp932'
     prm_names = []
     obj_names = []
     cns_names = []
-    local_data = pd.DataFrame()
     is_restart = False
     is_processing = False
     _future = None
     _actor_data = None
 
     def __init__(
             self,
@@ -393,14 +392,17 @@
         # 引数の処理
         self.path = history_path  # .csv
         self.prm_names = prm_names
         self.obj_names = obj_names
         self.cns_names = cns_names
         self.additional_metadata = additional_metadata or ''
 
+        # 初期化
+        self.local_data = pd.DataFrame()
+
         # 最適化実行中かどうか
         self.is_processing = client is not None
 
         # 最適化実行中の process monitor である場合
         if self.is_processing:
 
             # actor の生成
```

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/interface/_base.py` & `pyfemtet-0.4.2/pyfemtet/opt/interface/_base.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/interface/_femtet.py` & `pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                 while psutil.pid_exists(pid):
                     if time() - start > 30:  # 30 秒経っても存在するのは何かおかしい
                         os.kill(pid, signal.SIGKILL)
                         break
                     sleep(1)
                 sleep(1)
 
-            except AttributeError:  # already dead
+            except (AttributeError, OSError):  # already dead
                 pass
         # CoUninitialize()  # Win32 exception occurred releasing IUnknown at 0x0000022427692748
 
     def _connect_new_femtet(self):
         logger.info('└ Try to launch and connect new Femtet process.')
 
         self.Femtet, self.femtet_pid = launch_and_dispatch_femtet(strictly_pid_specify=self.strictly_pid_specify)
```

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/interface/_femtet_with_nx/_interface.py` & `pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/_interface.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/interface/_femtet_with_nx/update_model.py` & `pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_nx/update_model.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/interface/_femtet_with_sldworks.py` & `pyfemtet-0.4.2/pyfemtet/opt/interface/_femtet_with_sldworks.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/opt/_base.py` & `pyfemtet-0.4.2/pyfemtet/opt/opt/_base.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/opt/_optuna.py` & `pyfemtet-0.4.2/pyfemtet/opt/opt/_optuna.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,20 @@
             if len(self.study.trials) == 0:  # リスタートでなければ
                 # ユーザーの指定した初期値
                 params = self.get_parameter('dict')
                 self.study.enqueue_trial(params, user_attrs={"message": "initial"})
 
                 # add_initial_parameter で追加された初期値
                 for prm, prm_set_name in self.additional_initial_parameter:
+                    if type(prm) is dict:
+                        assert prm.keys() == params.keys(), '設定されたパラメータ名と add_init_parameter で追加されたパラメータ名が一致しません。'
+                    else:
+                        assert len(prm) == len(params.keys()), '設定されたパラメータ数と add_init_parameter で追加されたパラメータ数が一致しません。'
+                        prm = dict(zip(params.keys(), prm))
+
                     self.study.enqueue_trial(
                         prm,
                         user_attrs={"message": prm_set_name}
                     )
 
                 # add_init で指定された方法による初期値
                 if 'LHS' in self.additional_initial_methods:
```

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/visualization/_graphs.py` & `pyfemtet-0.4.2/pyfemtet/opt/visualization/_graphs.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyfemtet/opt/visualization/_monitor.py` & `pyfemtet-0.4.2/pyfemtet/opt/visualization/_monitor.py`

 * *Files identical despite different names*

### Comparing `pyfemtet-0.4.1/pyproject.toml` & `pyfemtet-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfemtet"
-version = "0.4.1"  # ignored by versioning plugin
+version = "0.4.2"  # ignored by versioning plugin
 description = "Design parameter optimization using Femtet."
 authors = ["kazuma.naito <kazuma.naito@murata.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/pyfemtet/pyfemtet"
 
 [tool.poetry.dependencies]
@@ -32,14 +32,16 @@
 sphinx = "==7.2.6"
 myst-parser = "==2.0.0"
 sphinx-rtd-theme = "==2.0.0"
 sphinx-autobuild = "==2021.3.14"
 pytest = "^7.4.3"
 sphinx-design = "^0.5.0"
 bokeh = "^3.3.3"
+pytest-dashboard = "*"
+sphinx-intl = "^2.2.0"
 
 [tool.poetry.scripts]
 opt-show = "pyfemtet.opt.visualization:entry_point"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     'ignore::DeprecationWarning',
```

### Comparing `pyfemtet-0.4.1/PKG-INFO` & `pyfemtet-0.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfemtet
-Version: 0.4.1
+Version: 0.4.2
 Summary: Design parameter optimization using Femtet.
 Home-page: https://github.com/pyfemtet/pyfemtet
 License: BSD-3-Clause
 Author: kazuma.naito
 Author-email: kazuma.naito@murata.com
 Requires-Python: >=3.9.3,<3.13
 Classifier: License :: OSI Approved :: BSD License
@@ -31,15 +31,16 @@
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/pyfemtet/pyfemtet
 Description-Content-Type: text/markdown
 
 PyFemtet is the extension package for Femtet with Python.
 
 - Femtet Website: https://www.muratasoftware.com/
-- Documentation: https://pyfemtet.github.io/pyfemtet/
+- Documentation (English): https://pyfemtet.readthedocs.io/en/stable/
+- ドキュメント（日本語）: https://pyfemtet.readthedocs.io/jp/stable/
 - Source code: https://github.com/pyfemtet/pyfemtet
 - Bug reports: https://github.com/pyfemtet/pyfemtet/issues
 
 
 It provides:
 
 - single and multi objective parameter optimization
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

