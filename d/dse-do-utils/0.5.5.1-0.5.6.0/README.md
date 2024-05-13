# Comparing `tmp/dse_do_utils-0.5.5.1.tar.gz` & `tmp/dse_do_utils-0.5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dse_do_utils-0.5.5.1.tar", last modified: Mon Mar  6 22:01:01 2023, max compression
+gzip compressed data, was "dse_do_utils-0.5.6.0.tar", last modified: Mon May 13 16:38:45 2024, max compression
```

## Comparing `dse_do_utils-0.5.5.1.tar` & `dse_do_utils-0.5.6.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 22:01:01.192278 dse_do_utils-0.5.5.1/
--rw-rw-rw-   0        0        0     5912 2023-03-06 22:01:01.191277 dse_do_utils-0.5.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4310 2023-03-04 19:29:45.000000 dse_do_utils-0.5.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-06 22:01:01.172203 dse_do_utils-0.5.5.1/dse_do_utils/
--rw-rw-rw-   0        0        0     4394 2023-03-04 19:29:45.000000 dse_do_utils-0.5.5.1/dse_do_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 22:01:01.191277 dse_do_utils-0.5.5.1/dse_do_utils/core/
--rw-rw-rw-   0        0        0    10840 2023-02-27 03:08:01.000000 dse_do_utils-0.5.5.1/dse_do_utils/core/core01_data_manager.py
--rw-rw-rw-   0        0        0     1278 2023-02-25 18:27:55.000000 dse_do_utils-0.5.5.1/dse_do_utils/core/core01_db_manager.py
--rw-rw-rw-   0        0        0     5736 2023-02-25 18:27:55.000000 dse_do_utils-0.5.5.1/dse_do_utils/core/core01_environment_manager.py
--rw-rw-rw-   0        0        0     9894 2023-02-26 03:49:02.000000 dse_do_utils-0.5.5.1/dse_do_utils/core/core01_optimization_engine.py
--rw-rw-rw-   0        0        0     8594 2023-02-25 23:16:52.000000 dse_do_utils-0.5.5.1/dse_do_utils/core/core02_data_manager.py
--rw-rw-rw-   0        0        0     4748 2023-02-25 23:16:52.000000 dse_do_utils-0.5.5.1/dse_do_utils/core/core02_db_manager.py
--rw-rw-rw-   0        0        0    12856 2023-02-25 23:16:52.000000 dse_do_utils-0.5.5.1/dse_do_utils/core/core02_optimization_engine.py
--rw-rw-rw-   0        0        0     5618 2020-06-23 15:39:06.000000 dse_do_utils-0.5.5.1/dse_do_utils/cpd25utilities.py
--rw-rw-rw-   0        0        0    18372 2022-10-09 18:23:28.000000 dse_do_utils-0.5.5.1/dse_do_utils/datamanager.py
--rw-rw-rw-   0        0        0    12747 2023-03-04 19:29:45.000000 dse_do_utils-0.5.5.1/dse_do_utils/deployeddomodel.py
--rw-rw-rw-   0        0        0    17651 2023-03-04 19:29:45.000000 dse_do_utils-0.5.5.1/dse_do_utils/domodeldeployer.py
--rw-rw-rw-   0        0        0    13695 2021-08-14 22:30:30.000000 dse_do_utils-0.5.5.1/dse_do_utils/domodelexporter.py
--rw-rw-rw-   0        0        0    11462 2022-12-09 04:10:47.000000 dse_do_utils-0.5.5.1/dse_do_utils/mapmanager.py
--rw-rw-rw-   0        0        0    12493 2023-03-04 19:29:45.000000 dse_do_utils-0.5.5.1/dse_do_utils/multiscenariomanager.py
--rw-rw-rw-   0        0        0    19634 2023-03-04 19:29:45.000000 dse_do_utils-0.5.5.1/dse_do_utils/optimizationengine.py
--rw-rw-rw-   0        0        0      650 2021-12-30 17:07:29.000000 dse_do_utils-0.5.5.1/dse_do_utils/plotly_cpd_workaround.py
--rw-rw-rw-   0        0        0     1813 2021-12-30 17:07:29.000000 dse_do_utils-0.5.5.1/dse_do_utils/plotlymanager.py
--rw-rw-rw-   0        0        0   113106 2023-03-04 19:29:45.000000 dse_do_utils-0.5.5.1/dse_do_utils/scenariodbmanager.py
--rw-rw-rw-   0        0        0    63217 2023-02-26 19:58:34.000000 dse_do_utils-0.5.5.1/dse_do_utils/scenariomanager.py
--rw-rw-rw-   0        0        0     8870 2020-06-23 15:39:06.000000 dse_do_utils-0.5.5.1/dse_do_utils/scenariopicker.py
--rw-rw-rw-   0        0        0    21429 2022-12-09 04:10:47.000000 dse_do_utils-0.5.5.1/dse_do_utils/scenariorunner.py
--rw-rw-rw-   0        0        0     2773 2022-10-09 18:23:28.000000 dse_do_utils-0.5.5.1/dse_do_utils/utilities.py
--rw-rw-rw-   0        0        0      414 2023-03-06 21:59:43.000000 dse_do_utils-0.5.5.1/dse_do_utils/version.py
-drwxrwxrwx   0        0        0        0 2023-03-06 22:01:01.185277 dse_do_utils-0.5.5.1/dse_do_utils.egg-info/
--rw-rw-rw-   0        0        0     5912 2023-03-06 22:01:01.000000 dse_do_utils-0.5.5.1/dse_do_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      991 2023-03-06 22:01:01.000000 dse_do_utils-0.5.5.1/dse_do_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 22:01:01.000000 dse_do_utils-0.5.5.1/dse_do_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-06 22:01:01.000000 dse_do_utils-0.5.5.1/dse_do_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-06 22:01:01.192278 dse_do_utils-0.5.5.1/setup.cfg
--rw-rw-rw-   0        0        0     3325 2023-03-06 21:54:56.000000 dse_do_utils-0.5.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:38:45.056211 dse_do_utils-0.5.6.0/
+-rw-rw-rw-   0        0        0     5907 2024-05-13 16:38:45.056211 dse_do_utils-0.5.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4300 2023-03-08 21:45:39.000000 dse_do_utils-0.5.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 16:38:44.980732 dse_do_utils-0.5.6.0/dse_do_utils/
+-rw-rw-rw-   0        0        0     4394 2023-03-04 19:29:45.000000 dse_do_utils-0.5.6.0/dse_do_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:38:45.054218 dse_do_utils-0.5.6.0/dse_do_utils/core/
+-rw-rw-rw-   0        0        0    13543 2024-04-04 21:19:50.000000 dse_do_utils-0.5.6.0/dse_do_utils/core/core01_data_manager.py
+-rw-rw-rw-   0        0        0     1278 2023-02-25 18:27:55.000000 dse_do_utils-0.5.6.0/dse_do_utils/core/core01_db_manager.py
+-rw-rw-rw-   0        0        0     9816 2023-06-16 19:52:29.000000 dse_do_utils-0.5.6.0/dse_do_utils/core/core01_environment_manager.py
+-rw-rw-rw-   0        0        0    10541 2023-06-07 19:11:35.000000 dse_do_utils-0.5.6.0/dse_do_utils/core/core01_optimization_engine.py
+-rw-rw-rw-   0        0        0     9137 2024-04-03 16:15:34.000000 dse_do_utils-0.5.6.0/dse_do_utils/core/core02_data_manager.py
+-rw-rw-rw-   0        0        0     4748 2023-02-25 23:16:52.000000 dse_do_utils-0.5.6.0/dse_do_utils/core/core02_db_manager.py
+-rw-rw-rw-   0        0        0    13787 2024-03-30 03:14:23.000000 dse_do_utils-0.5.6.0/dse_do_utils/core/core02_optimization_engine.py
+-rw-rw-rw-   0        0        0     2357 2024-04-03 15:47:34.000000 dse_do_utils-0.5.6.0/dse_do_utils/core/core02_scenario_runner.py
+-rw-rw-rw-   0        0        0     5618 2020-06-23 15:39:06.000000 dse_do_utils-0.5.6.0/dse_do_utils/cpd25utilities.py
+-rw-rw-rw-   0        0        0    23462 2024-05-07 20:38:09.000000 dse_do_utils-0.5.6.0/dse_do_utils/datamanager.py
+-rw-rw-rw-   0        0        0    20581 2024-05-11 03:30:30.000000 dse_do_utils-0.5.6.0/dse_do_utils/deployeddomodel.py
+-rw-rw-rw-   0        0        0    33976 2024-05-10 23:35:08.000000 dse_do_utils-0.5.6.0/dse_do_utils/domodeldeployer.py
+-rw-rw-rw-   0        0        0    13695 2021-08-14 22:30:30.000000 dse_do_utils-0.5.6.0/dse_do_utils/domodelexporter.py
+-rw-rw-rw-   0        0        0    13642 2023-06-16 00:34:38.000000 dse_do_utils-0.5.6.0/dse_do_utils/mapmanager.py
+-rw-rw-rw-   0        0        0    12493 2023-03-04 19:29:45.000000 dse_do_utils-0.5.6.0/dse_do_utils/multiscenariomanager.py
+-rw-rw-rw-   0        0        0    19796 2023-04-30 16:42:47.000000 dse_do_utils-0.5.6.0/dse_do_utils/optimizationengine.py
+-rw-rw-rw-   0        0        0      650 2021-12-30 17:07:29.000000 dse_do_utils-0.5.6.0/dse_do_utils/plotly_cpd_workaround.py
+-rw-rw-rw-   0        0        0     1898 2023-06-09 02:28:34.000000 dse_do_utils-0.5.6.0/dse_do_utils/plotlymanager.py
+-rw-rw-rw-   0        0        0   113273 2024-04-26 21:08:02.000000 dse_do_utils-0.5.6.0/dse_do_utils/scenariodbmanager.py
+-rw-rw-rw-   0        0        0    63275 2023-05-26 16:04:35.000000 dse_do_utils-0.5.6.0/dse_do_utils/scenariomanager.py
+-rw-rw-rw-   0        0        0     8870 2020-06-23 15:39:06.000000 dse_do_utils-0.5.6.0/dse_do_utils/scenariopicker.py
+-rw-rw-rw-   0        0        0    22450 2024-04-17 23:00:08.000000 dse_do_utils-0.5.6.0/dse_do_utils/scenariorunner.py
+-rw-rw-rw-   0        0        0     4346 2024-04-02 23:24:57.000000 dse_do_utils-0.5.6.0/dse_do_utils/utilities.py
+-rw-rw-rw-   0        0        0      414 2024-05-13 16:34:18.000000 dse_do_utils-0.5.6.0/dse_do_utils/version.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:38:44.997739 dse_do_utils-0.5.6.0/dse_do_utils.egg-info/
+-rw-rw-rw-   0        0        0     5907 2024-05-13 16:38:44.000000 dse_do_utils-0.5.6.0/dse_do_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2024-05-13 16:38:44.000000 dse_do_utils-0.5.6.0/dse_do_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:38:44.000000 dse_do_utils-0.5.6.0/dse_do_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-13 16:38:44.000000 dse_do_utils-0.5.6.0/dse_do_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 16:38:45.056211 dse_do_utils-0.5.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     3330 2023-03-08 21:43:22.000000 dse_do_utils-0.5.6.0/setup.py
```

### Comparing `dse_do_utils-0.5.5.1/PKG-INFO` & `dse_do_utils-0.5.6.0/dse_do_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: dse_do_utils
-Version: 0.5.5.1
-Summary: Decision Optimization utilities for IBM Watson Studio projects
+Name: dse-do-utils
+Version: 0.5.6.0
+Summary: Decision Optimization utilities for IBM Cloud Pak for Data projects
 Home-page: https://github.com/IBM/dse-decision-optimization-utilities
 Author: Victor Terpstra
 Author-email: vterpstra@us.ibm.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/IBM/dse-decision-optimization-utilities
 Project-URL: Documentation, https://ibm.github.io/dse-decision-optimization-utilities/
 Project-URL: IBM Decision Optimization, https://www.ibm.com/analytics/decision-optimization
 Description: # DSE_DO_Utils
-        Decision Optimization utilities for IBM Watson Studio Local and ICPd projects.
+        Decision Optimization utilities for IBM Cloud Pak for Data projects.
         
         [Source (GitHub)](https://github.com/IBM/dse-decision-optimization-utilities)<br>
         [Documentation (GitHubPages)](https://ibm.github.io/dse-decision-optimization-utilities/)
         
         This repository contains the package `dse_do_utils`. This can be installed using pip.
         
         ## Important
@@ -99,12 +99,12 @@
         This package requires:
         1. [decision-optimization-client](https://ibmdecisionoptimization.github.io/decision-optimization-client-doc/). This package provides an interface to the DO scenarios. 
         This package is available in PyPI, however it only runs within CP4D/CP4DaaS.
         2. [docplex](http://ibmdecisionoptimization.github.io/docplex-doc/mp/index.html). This package interfaces with the CPLEX and CP Optimizer optimization engines.
         3. [folium](https://github.com/python-visualization/folium). Map visualization. Only for the MapManager.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation :: Sphinx
 Description-Content-Type: text/markdown
```

### Comparing `dse_do_utils-0.5.5.1/README.md` & `dse_do_utils-0.5.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DSE_DO_Utils
-Decision Optimization utilities for IBM Watson Studio Local and ICPd projects.
+Decision Optimization utilities for IBM Cloud Pak for Data projects.
 
 [Source (GitHub)](https://github.com/IBM/dse-decision-optimization-utilities)<br>
 [Documentation (GitHubPages)](https://ibm.github.io/dse-decision-optimization-utilities/)
 
 This repository contains the package `dse_do_utils`. This can be installed using pip.
 
 ## Important
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/__init__.py` & `dse_do_utils-0.5.6.0/dse_do_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/core/core01_db_manager.py` & `dse_do_utils-0.5.6.0/dse_do_utils/core/core01_db_manager.py`

 * *Files identical despite different names*

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/core/core01_optimization_engine.py` & `dse_do_utils-0.5.6.0/dse_do_utils/core/core01_optimization_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,36 @@
 import pandas as pd
 from docplex.mp.conflict_refiner import ConflictRefiner
 from docplex.mp.solution import SolveSolution
 
 from dse_do_utils import OptimizationEngine
 from dse_do_utils.core.core01_data_manager import Core01DataManager
 from dse_do_utils.datamanager import Outputs
+from typing import TypeVar, Generic
 
+DM = TypeVar('DM', bound='Core01DataManager')
 
-class Core01OptimizationEngine(OptimizationEngine):
-    def __init__(self, data_manager: Core01DataManager, name: str = None, solve_kwargs: Dict = {"log_output": True},
+
+class Core01OptimizationEngine(OptimizationEngine[DM]):
+    """
+    This class supports Python generics to specify the class of the DataManager.
+    This allows an IDE like PyCharm and VSCode to check for methods and attributes
+    and allows more easy navigation (i.e. control-click on name)
+
+    Usage 1 - Define a use-case specific OptimizationEngine class::
+
+        DM = TypeVar('DM', bound='FruitDataManager')
+        class FruitOptimizationEngine(Core01OptimizationEngine[DM]):
+            pass
+
+    Usage 2 - When creating an instance::
+
+        engine = FruitOptimizationEngine[FruitDataManager]
+    """
+    def __init__(self, data_manager: DM, name: str = None, solve_kwargs: Dict = {"log_output": True},
                  export_lp: bool = False, export_sav: bool = False, export_lp_path: str = '',
                  enable_refine_conflict: bool = False):
         super().__init__(data_manager=data_manager, name=name)
         self.solve_kwargs = solve_kwargs
         self.export_lp = export_lp
         self.export_sav = export_sav
         self.export_lp_path = export_lp_path
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/core/core02_data_manager.py` & `dse_do_utils-0.5.6.0/dse_do_utils/core/core02_data_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,26 +82,32 @@
 
     def prep_lex_opti_levels(self):
         """
         Prepare lex_opti_levels
 
         Returns:
             df: lex_opti_levels
+
+        Note (VT_20240403): `isActive` cannot be an optional column: inserting `None` in a PostgressDB reads `False`.
+        Thus applying the fillna in this method won't work after any DB insert/read, which the ScenarioRunner typically does.
+        Not sure if this is a Postgress issue and if and how this can be fixed.
+        For now, assume `isActive` cannot be an optional
+        TODO: move 'isActive' to the value_columns. Not done so far as to avoid any backward compatibility issues.
         """
         input_table_name='LexOptiLevel'
         df = self.inputs.get(input_table_name)
         # Provide default settings when table is missing from inputs:
         if df is None or df.shape[0] == 0:
             df = self.get_default_lex_opti_level_table()
 
         df = self.prepare_df(
             df,
             index_columns=['lexOptiLevelId'],
             value_columns=['priority', 'timeLimit', 'mipGap'], # Note that 'absTol' is not required
-            optional_columns=['relTol', 'absTol', 'isActive'],  #
+            optional_columns=['relTol', 'absTol', 'isActive'],  # TODO: `isActive` should NOT be optional
             dtypes={
                 **self.dtypes,  # later entries will override any entries in in self.dtypes
                 # 'isActive': bool,
                 'priority': int,
                 'timeLimit': int,
                 'mipGap': float,
                 # 'relTol': float,
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/core/core02_db_manager.py` & `dse_do_utils-0.5.6.0/dse_do_utils/core/core02_db_manager.py`

 * *Files identical despite different names*

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/core/core02_optimization_engine.py` & `dse_do_utils-0.5.6.0/dse_do_utils/core/core02_optimization_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright IBM Corp. 2021, 2022
 # IBM Confidential Source Code Materials
 # This Source Code is subject to the license and security terms contained in the License.txt file contained in this source code package.
 
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, TypeVar
 
 import docplex
 import pandas as pd
 from docplex.mp.conflict_refiner import ConflictRefiner
 from docplex.mp.linear import ZeroExpr
 from docplex.mp.solution import SolveSolution
 
@@ -20,21 +20,37 @@
     def __init__(self, mdl):
         self.mdl = mdl
 
     def __call__(self, group):
         return self.mdl.sum(group.expr * group.weight)
 
 
-class Core02OptimizationEngine(Core01OptimizationEngine):
+DM = TypeVar('DM', bound='Core02DataManager')
+
+
+class Core02OptimizationEngine(Core01OptimizationEngine[DM]):
     """Adds Lexicographical Optimization
+
+    How To enable Lexicographical Optimization:
+    1. Add tables `LexOptiLevel` and `LexOptiGoal` to the spreadsheet (if applicable, include in __index__!)
+    2. Subclass the optimization-engine, data-manager and scenario-db-manager from their Core2 classes
+    3. In OptimizationEngine, override the method `lex_get_goal_expr()`
+    4. In DataManager, override abstract methods `get_default_lex_opti_level_table` and `get_default_lex_opti_goal_table`
+    4. In ScenarioDBManager, add the
+        `('LexOptiLevel', Core02LexOptiLevelTable()),
+         ('LexOptiGoal', Core02LexOptiGoalTable()),`
+        to the input_db_tables
     """
 
     def __init__(self, data_manager: Core02DataManager, name: str = None, solve_kwargs: Dict = {"log_output": True},
-                 export_lp: bool = False, export_sav: bool = False, export_lp_path: str = ''):
-        super().__init__(data_manager, name=name, solve_kwargs=solve_kwargs, export_lp=export_lp, export_sav=export_sav, export_lp_path=export_lp_path)
+                 export_lp: bool = False, export_sav: bool = False, export_lp_path: str = '',
+                 enable_refine_conflict: bool = False):
+        super().__init__(data_manager, name=name, solve_kwargs=solve_kwargs,
+                         export_lp=export_lp, export_sav=export_sav, export_lp_path=export_lp_path,
+                         enable_refine_conflict=enable_refine_conflict)
         # self.solver_metrics = None
         self.lex_opti_metrics_list: List[Dict] = []
 
     ####################################################################################
     #  Solve
     ####################################################################################
     def solve(self) -> Optional[SolveSolution]:
@@ -101,14 +117,15 @@
     #     #self.solver_metrics['value'].append(self.mdl.solve_details.status)
     #     self.solver_metrics['value'].append(self.mdl.parameters.mip.tolerances.mipgap.value)
     #     self.solver_metrics['value'].append(self.mdl.number_of_variables)
     #     self.solver_metrics['value'].append(self.mdl.number_of_constraints)
     #     self.solver_metrics['value'].append(self.mdl.parameters.timelimit.value)
 
     def solve_with_lex_goals(self, **kwargs) -> Optional[SolveSolution]:
+        msol = None
         self.dm.logger.debug("Enter")
         levels_df = self.get_lex_optimization_levels()
         self.lex_c = []
         for level in levels_df.itertuples():
             level_id = level.Index
             self.dm.logger.debug(f"Solving level: {level_id}")
 
@@ -160,14 +177,15 @@
 
             self.dm.logger.debug(f"{level_id} level constraint added")
 
         self.mdl.remove_constraints(self.lex_c)
         return msol
 
     def lex_get_goal_expr(self, goal_id):
+        """ABSTRACT method. TO BE OVERRIDDEN!"""
         # if goal_id == 'backlogCost':
         #     return self.backlog_cost
         # elif goal_id == 'unfulfilledDemandCost':
         #     return self.unfulfilled_demand_cost
         # elif goal_id == 'inventoryCost':
         #     return self.inventory_cost
         # elif goal_id == 'productionCost':
@@ -222,15 +240,15 @@
         :return:
         """
         self.dm.logger.info("Start ConflictRefiner.")
         try:
             crefiner = ConflictRefiner()  # Create an instance of the ConflictRefiner
             conflicts = crefiner.refine_conflict(self.mdl, display=True)  # Run the conflict refiner
             # ConflictRefiner.display_conflicts(conflicts) #Display the results
-            conflict_reporting_limit = 10
+            conflict_reporting_limit = 100
             if len(conflicts) > conflict_reporting_limit:
                 self.dm.logger.warning(f"Number of conflicts {len(conflicts)} exceeds reporting limit ({conflict_reporting_limit})")
             i = 0
             for c in conflicts:
                 print(c.element)  # Display conflict result in a little more compact format than ConflictRefiner.display_conflicts
                 i=i+1
                 if i > conflict_reporting_limit:
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/cpd25utilities.py` & `dse_do_utils-0.5.6.0/dse_do_utils/cpd25utilities.py`

 * *Files identical despite different names*

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/datamanager.py` & `dse_do_utils-0.5.6.0/dse_do_utils/datamanager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright IBM All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
 # -----------------------------------------------------------------------------------
 # -----------------------------------------------------------------------------------
 # DataManager
 # -----------------------------------------------------------------------------------
 # -----------------------------------------------------------------------------------
 import types
@@ -173,15 +174,22 @@
             elif param_type == 'bool':
                 # Note that the function `bool()` does not do what you expect!
                 # Note that the type of the raw_param could be a Python bool, string, or Numpy Bool
                 # (see http://joergdietrich.github.io/python-numpy-bool-types.html)
                 # param = (str(raw_param) == 'True')
                 param = (str(raw_param).lower() in ['true', 'yes', 'y', 't', '1', '1.0'])
             elif param_type == 'datetime':
-                param = datetime.strptime(raw_param, value_format)
+                # Make more robust:
+                # 1. Remove any excess quotes if a string (When forcing a value to be a quoted string in Excel)
+                # 2. If it already is a datetime, do not convert (Excel read may return a datetime already)
+                if isinstance(raw_param, datetime):
+                    param = raw_param
+                else:
+                    raw_param = raw_param.strip('"')
+                    param = datetime.strptime(raw_param, value_format)
             else:
                 param = raw_param
         else:
             print(f'Warning: {param_name} not in Parameters. Using default value = {default_value}')
             # If datetime, the default value can be a string
             import six  # For Python 2 and 3 compatibility of testing string instance
             if param_type == 'datetime' and isinstance(default_value, six.string_types):
@@ -343,29 +351,102 @@
     #     """
     #     return pd.concat((
     #         dataframe,
     #         dataframe.apply(
     #             lambda row: pd.Series(func(row, **kwargs), index=column_names), axis=1)), axis=1, sort=False)
 
     @staticmethod
-    def extract_solution(df, extract_dvar_names: List[str] = None, drop_column_names: List[str] = None, drop: bool = True):
+    def extract_solution(df: pd.DataFrame, extract_dvar_names: Optional[List[str] | Dict[str, str]] = None, drop_column_names: List[str] = None,
+                         drop: bool = True, epsilon: float = None, round_decimals: int = None,
+                         solution_column_name_post_fix: str = 'Sol') -> pd.DataFrame:
         """Generalized routine to extract a solution value.
-        Can remove the dvar column from the df to be able to have a clean df for export into scenario."""
+        Can remove the dvar column from the df to be able to have a clean df for export into scenario.
+
+        In some cases, CPLEX extracted values for continuous dvars can have very small values instead of zeros.
+        If epsilon has a value, this method will drop these small values to zero.
+        And it will assume the values need to be positive, so it clips negative values at zero.
+
+        In some case, CPLEX extracted values for integer dvars can have very small values from the rounded integer value.
+        If round_decimals is set to 0, the solution values will be rounded to the nearest integer.
+        Use values larger than zero to round continuous dvars to their required precision.
+
+        Args:
+            df: DataFrame
+            extract_dvar_names: list of column names with CPLEX dvars, or a Dict[str, str]
+                                where the keys are the dvar column names and the values the name of the solution column
+            drop_column_names: columns to be dropped (can be different and in addition to drop)
+            drop: if True drops all columns in extract_dvar_names
+            epsilon (float): if not None, drop values below threshold to zero and clip negative values at zero
+            round_decimals (int): round the solution value by number of decimals. If None, no rounding.
+            If 0, rounding to integer value.
+            solution_column_name_post_fix (str): Postfix for the name of the solution column. Default = 'Sol'
+
+        """
+
+
         if extract_dvar_names is not None:
-            for xDVarName in extract_dvar_names:
+            if isinstance(extract_dvar_names, list):
+                dvar_column_dict = {dvar_name: f'{dvar_name}{solution_column_name_post_fix}' for dvar_name in extract_dvar_names}
+            elif isinstance(extract_dvar_names, dict):
+                dvar_column_dict = extract_dvar_names
+            else:
+                # dvar_column_dict = {}
+                raise TypeError("Input argument 'extract_dvar_names' must be either a List[str] or a Dict[str, str]")
+            for xDVarName, solution_column_name in dvar_column_dict.items():
                 if xDVarName in df.columns:
-                    df[f'{xDVarName}Sol'] = [dvar.solution_value for dvar in df[xDVarName]]
+                    # solution_column_name = f'{xDVarName}Sol'
+                    df[solution_column_name] = [dvar.solution_value for dvar in df[xDVarName]]
                     if drop:
                         df = df.drop([xDVarName], axis=1)
+                    if epsilon is not None:
+                        df.loc[df[solution_column_name] < epsilon, solution_column_name] = 0
+                        df[solution_column_name] = df[solution_column_name].clip(lower=0)
+                    if round_decimals is not None:
+                        df[solution_column_name] = df[solution_column_name].round(round_decimals)
+                        if round_decimals == 0:
+                            df[solution_column_name] = df[solution_column_name].astype(int)
+                else:
+                    # Note (VT_20240401): for backward compatibility reasons, for now, do not throw an exception or print a warning
+                    # print(f"Warning: The column {xDVarName} doesn't exist in the DataFrame. Valid column: {df.columns}")
+                    pass
+
+        # if extract_dvar_names is not None:
+        #     for xDVarName in extract_dvar_names:
+        #         if xDVarName in df.columns:
+        #             solution_column_name = f'{xDVarName}Sol'
+        #             df[solution_column_name] = [dvar.solution_value for dvar in df[xDVarName]]
+        #             if drop:
+        #                 df = df.drop([xDVarName], axis=1)
+        #             if epsilon is not None:
+        #                 df.loc[df[solution_column_name] < epsilon, solution_column_name] = 0
+        #                 df[solution_column_name] = df[solution_column_name].clip(lower=0)
+        #             if round_decimals is not None:
+        #                 df[solution_column_name] = df[solution_column_name].round(round_decimals)
         if drop and drop_column_names is not None:
             for column in drop_column_names:
                 if column in df.columns:
                     df = df.drop([column], axis=1)
         return df
 
+    # def drop_small_epsilon_values(self, df: pd.DataFrame, columns: List[str], epsilon: float = 0.0001) -> pd.DataFrame:
+    #     """Drops small values of extracted CPLEX continuous dvar solutions to zero.
+    #     In some cases, CPLEX extracted values can have very small values instead of zeros.
+    #     This method drops these small values to zero.
+    #     It also assumes the values need to be positive, so it clips all negative values at zero.
+    #     Args:
+    #         df: DataFrame
+    #         columns: List of column names
+    #         epsilon: threshold value
+    #     """
+    #     for col in columns:
+    #         if col in df.columns:
+    #             df.loc[df[col] < epsilon, col] = 0
+    #             df[col] = df[col].clip(lower=0)
+    #     return df
+
     def get_raw_table_by_name(self, table_name: str) -> Optional[pd.DataFrame]:
         """Get the 'raw' (non-indexed) table from inputs or outputs."""
         if self.inputs is not None and table_name in self.inputs:
             df = self.inputs[table_name]
         elif self.outputs is not None and table_name in self.outputs:
             df = self.outputs[table_name]
         else:
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/domodeldeployer.py` & `dse_do_utils-0.5.6.0/dse_do_utils/domodeldeployer.py`

 * *Files 21% similar despite different names*

```diff
@@ -324,15 +324,15 @@
         """Return the meta_props for the creation of the deployment
         Separate method, so can easily be overridden
         """
         meta_props = {
             self.client.deployments.ConfigurationMetaNames.NAME: self.deployment_name,
             self.client.deployments.ConfigurationMetaNames.DESCRIPTION: self.deployment_description,
             self.client.deployments.ConfigurationMetaNames.BATCH: {},
-            self.client.deployments.ConfigurationMetaNames.HARDWARE_SPEC: {'name': 'S', 'nodes': 1}
+            self.client.deployments.ConfigurationMetaNames.HARDWARE_SPEC: {'name': 'S', 'nodes': 2}
         }
         return meta_props
 
     #################################################################################
     def create_package_extension(self, yaml_file_path:str) -> str:
         current_time = time.asctime()
         meta_prop_pkg_ext = {
@@ -368,11 +368,354 @@
         """Get space_id from deployment space name.
         TODO: handle exception if space_name not found.
         """
         spaces = self.client.spaces.get_details()
         return (next(item for item in spaces['resources'] if item['entity']["name"] == space_name)['metadata']['id'])
 
 
+########################################################################################
+# DO Model Deployer for use on a local machine (instead of CP4D)
+########################################################################################
+
+class DOModelDeployerLocal(object):
+    """EXPERIMENTAL
+    Please note this code is experimental. There are a number of aspects HARD-CODED. Please review the source code and override where necessary.
+
+    Deploys a DO Model in WML. For use in CPD 4.0 and SaaS. Retrieves the model from the DO Model Builder.
+
+    Usage::
+
+        md = DOModelDeployer(wml_credentials, space_name,
+                             package_paths, file_paths,
+                             deployment_name, deployment_description)
+        deployment_uid = md.deploy_model()
+        print(deployment_uid)
+
+    """
+    def __init__(self, wml_credentials: Dict, space_name: str,
+                 package_paths: Optional[List[str]] = None,
+                 file_paths: Optional[List[str]] = None,
+                 deployment_name: Optional[str] = 'xxx', deployment_description: Optional[str] = 'xxx',
+                 tmp_dir: Optional[str] = None):
+
+        self.wml_credentials = wml_credentials
+        self.space_name = space_name
+        self.package_paths = (package_paths if package_paths is not None else [])
+        self.file_paths = (file_paths if file_paths is not None else [])
+        self.deployment_name = deployment_name
+        self.deployment_description = deployment_description
+        self.tmp_dir = tmp_dir
+
+        # Initialize clients
+        from ibm_watson_machine_learning import APIClient
+        self.client = APIClient(wml_credentials)
+        space_id = self.guid_from_space_name(space_name)  # TODO: catch error if space_name cannot be found?
+        result = self.client.set.default_space(space_id)
+
+        # State
+        self.model_uid = None
+        self.deployment_uid = None
+
+        # Code templates
+        self.main_header_py = \
+"""
+from docplex.util.environment import get_environment
+from os.path import splitext
+import pandas
+from six import iteritems
+
+def get_all_inputs():
+    '''Utility method to read a list of files and return a tuple with all
+    read data frames.
+    Returns:
+        a map { datasetname: data frame }
+    '''
+    result = {}
+    env = get_environment()
+    for iname in [f for f in os.listdir('.') if splitext(f)[1] == '.csv']:
+        with env.get_input_stream(iname) as in_stream:
+            df = pandas.read_csv(in_stream)
+            datasetname, _ = splitext(iname)
+            result[datasetname] = df
+    return result
+
+def write_all_outputs(outputs):
+    '''Write all dataframes in ``outputs`` as .csv.
+
+    Args:
+        outputs: The map of outputs 'outputname' -> 'output df'
+    '''
+    for (name, df) in iteritems(outputs):
+        csv_file = '%s.csv' % name
+        print(csv_file)
+        with get_environment().get_output_stream(csv_file) as fp:
+            if sys.version_info[0] < 3:
+                fp.write(df.to_csv(index=False, encoding='utf8'))
+            else:
+                fp.write(df.to_csv(index=False).encode(encoding='utf8'))
+    if len(outputs) == 0:
+        print("Warning: no outputs written")
+
+def __iter__(self): return 0
+# Load CSV files into inputs dictionnary
+inputs = get_all_inputs()
+outputs = {}
+
+###########################################################
+# Insert model below
+###########################################################
+"""
+        self.main_footer_py = \
+"""
+###########################################################
+
+# Generate output files
+write_all_outputs(outputs)
+"""
+        self.yaml = \
+"""
+dependencies:
+  - pip:
+    - dse-do-utils
+    - sqlalchemy
+"""
 
+    def guid_from_space_name(self, space_name: str) -> str:
+        """Get space_id from deployment space name.
+        TODO: handle exception if space_name not found.
+        """
+        spaces = self.client.spaces.get_details()
+        return (next(item for item in spaces['resources'] if item['entity']["name"] == space_name)['metadata']['id'])
+
+    def deploy_model(self) -> str:
+        """One call that deploys a model from the Model Builder scenario into WML.
+        Creates a model archive from the extracted model code.
+        Then uploads into WML and creates a deployment.
+
+        Returns:
+            deployment_uid (str): Deployment UID necessary to call the deployment.
+        """
+        if self.tmp_dir is None:
+            with tempfile.TemporaryDirectory() as path:
+                model_archive_file_path = self.create_model_archive(path)
+                yaml_file_path = self.write_yaml_file(os.path.join(path, "main.yml"))
+                deployment_uid = self.deploy_archive(model_archive_file_path, yaml_file_path)
+        else:
+            model_archive_file_path = self.create_model_archive(self.tmp_dir)
+            yaml_file_path = self.write_yaml_file(os.path.join(self.tmp_dir, "main.yml"))
+            deployment_uid = self.deploy_archive(model_archive_file_path, yaml_file_path)
+        return deployment_uid
+
+    ############################################
+    # Create model archive
+    ############################################
+    def create_model_archive(self, path: str):
+        """Creates a model archive on the path:
+        The archive contains one .py file: the do-model surrounded by boilerplate code to process
+        the inputs and outputs dictionaries.
+        Steps:
+        1. Write a file `path/main.py`
+        2. Creates an archive file in path
+        3. Adds the main.py
+        4. Adds packages
+        5. Adds (module) files
+        """
+
+        main_file_path = os.path.join(path, 'main.py')
+        self.write_main_file(main_file_path)
+        file_path = self.create_archive(main_file_path, path)
+        return file_path
+
+    def create_model_directory(self) -> str:
+        """Create a directory 'model' in the default path.
+        Will remove/clear first if exists.
+
+        Return:
+            path
+        """
+        path = 'model'
+        if os.path.isdir(path):
+            shutil.rmtree(path)
+        os.makedirs(path)
+        return path
+
+    def write_main_file(self, file_path: str):
+        """Write the code for the main.py file.
+        Adds the code template header and footer.
+        """
+        with open(file_path, "w") as f:
+            f.write(self.main_header_py)
+            f.write('\n')
+            # f.write(scenario.get_asset_data('model.py').decode('ascii')) # Get from DO Experiment
+            f.write(self.get_model_py())
+            f.write('\n')
+            f.write(self.main_footer_py)
+
+    def get_model_py(self) -> str:
+        """Return the optimization model. Assume the usual inputs and outputs dicts."""
+        model_py = "print('Hello World')"
+        return model_py
+
+    def write_yaml_file(self, file_path: str = './main.yml'):
+        """Write the code for the main.py file.
+        Adds the code template header and footer.
+        """
+        with open(file_path, "w") as f:
+            f.write(self.yaml)
+        return file_path
+
+    def create_archive(self, main_file_path: str, path: str):
+        """Create archive.
+        For now assume one folder `model` with one file `main.py`
+
+        :param main_file_path: file path of main.py file
+        :param path: folder where archive will be written
+        """
+        def reset(tarinfo):
+            tarinfo.uid = tarinfo.gid = 0
+            tarinfo.uname = tarinfo.gname = "root"
+            return tarinfo
+        tar_file_path = os.path.join(path, "model.tar.gz")
+        tar = tarfile.open(tar_file_path, "w:gz")
+        #         tar.add("model/main.py", arcname="main.py", filter=reset)
+        tar.add(main_file_path, arcname="main.py", filter=reset)
+
+        def filter_package(tarinfo):
+            tarinfo.uid = tarinfo.gid = 0
+            tarinfo.uname = tarinfo.gname = "root"
+            if pathlib.Path(tarinfo.name).stem == '__pycache__':
+                return None
+            return tarinfo
+
+        for package_path in self.package_paths:
+            package_name = pathlib.Path(package_path).stem
+            print(f"Including package '{package_name}'")
+            tar.add(package_path, arcname=package_name, filter=filter_package)
+
+        for file_path in self.file_paths:
+            file_name = pathlib.Path(file_path).name
+            print(f"Including file '{file_name}'")
+            tar.add(file_path, arcname=file_name, filter=filter_package)
+
+        tar.close()
+        return tar_file_path
+
+    #########################################################
+    # Deploy model
+    #########################################################
+    def deploy_archive(self, model_archive_file_path, yaml_file_path):
+        print(f"model_archive_file_path={model_archive_file_path}, yaml_file_path={yaml_file_path}")
+        self.model_uid = self.wml_store_model(model_archive_file_path, yaml_file_path)
+        self.deployment_uid = self.wml_create_deployment(self.model_uid)
+        return self.deployment_uid
+
+    def wml_store_model(self, model_archive_file_path, yaml_file_path) -> str:
+        """Stores model in WML
+        Returns:
+            model_uid
+        """
+        yaml_pkg_ext_id = self.create_package_extension(yaml_file_path)  # Rename to `create_yaml_package_extension`
+        pkg_ext_ids=[yaml_pkg_ext_id]
+
+        #Add wheels/zips:
+        for package_zip_filepath in self.package_paths:
+            pkg_ext_ids.append(self.create_zip_package_extension(package_zip_filepath))
+
+        sw_spec_id = self.create_software_specification(pkg_ext_ids)
+        mnist_metadata = self.get_wml_create_store_model_meta_props(sw_spec_id)
+        model_details = self.client.repository.store_model(model=model_archive_file_path,
+                                                           meta_props=mnist_metadata)
+        # model_uid = self.client.repository.get_model_uid(model_details)  # deprecated: use get_model_id
+        model_uid = self.client.repository.get_model_id(model_details)
+        return model_uid
+
+    def create_zip_package_extension(self, package_zip_filepath: str) -> str:
+        """See https://notebooks.githubusercontent.com/view/ipynb?browser=chrome&color_mode=auto&commit=37188b1a8b48be2bef34b35b55f01cba0d29ed19&device=unknown&enc_url=68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f49424d2f776174736f6e2d6d616368696e652d6c6561726e696e672d73616d706c65732f333731383862316138623438626532626566333462333562353566303163626130643239656431392f637064342e302f6e6f7465626f6f6b732f707974686f6e5f73646b2f6465706c6f796d656e74732f637573746f6d5f6c6962726172792f5573652532307363696b69742d6c6561726e253230616e64253230637573746f6d2532306c696272617279253230746f2532307072656469637425323074656d70657261747572652e6970796e62&logged_in=false&nwo=IBM%2Fwatson-machine-learning-samples&path=cpd4.0%2Fnotebooks%2Fpython_sdk%2Fdeployments%2Fcustom_library%2FUse+scikit-learn+and+custom+library+to+predict+temperature.ipynb&platform=android&repository_id=277618282&repository_type=Repository&version=98
+        TYPE can only be 'pip_zip' and package format must be a .zip (See https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/ml-create-custom-software-spec.html?context=cpdaas)
+
+        """
+        package_name = pathlib.Path(package_zip_filepath).stem
+        print(f"Including package '{package_name}'")
+        meta_prop_pkg_extn = {
+            self.client.package_extensions.ConfigurationMetaNames.NAME: package_name,
+            self.client.package_extensions.ConfigurationMetaNames.DESCRIPTION: "Pkg extension for custom lib",
+            self.client.package_extensions.ConfigurationMetaNames.TYPE: "pip_zip"
+        }
+
+        pkg_extn_details = self.client.package_extensions.store(meta_props=meta_prop_pkg_extn, file_path=package_zip_filepath)
+        # print(pkg_extn_details)
+        pkg_extn_uid = self.client.package_extensions.get_uid(pkg_extn_details)
+        #         pkg_extn_url = self.client.package_extensions.get_href(pkg_extn_details)
+        return pkg_extn_uid
+
+    def wml_create_deployment(self, model_uid) -> str:
+        """Create deployment in WML
+        Returns:
+            deployment_uid
+        """
+        meta_props = self.get_wml_create_deployment_meta_props()
+        deployment_details = self.client.deployments.create(model_uid, meta_props=meta_props)
+        deployment_uid = self.client.deployments.get_uid(deployment_details)
+        return deployment_uid
+
+    def get_wml_create_store_model_meta_props(self, sw_spec_id):
+        """Return the meta_props for the store of the model
+        Separate method, so can easily be overridden
+        """
+        mnist_metadata = {
+            self.client.repository.ModelMetaNames.NAME: self.deployment_name,
+            self.client.repository.ModelMetaNames.DESCRIPTION: self.deployment_description,
+            self.client.repository.ModelMetaNames.TYPE: "do-docplex_22.1",
+            self.client.repository.ModelMetaNames.SOFTWARE_SPEC_UID: sw_spec_id
+        }
+        return mnist_metadata
+
+    def get_wml_create_deployment_meta_props(self):
+        """Return the meta_props for the creation of the deployment
+        Separate method, so can easily be overridden
+
+        Note that 1 node is too slow: somehow causes extended running overhead, where the CPLEX model itself can solve quickly
+        Also, 2 nodes still only gives CPLEX one thread.
+        """
+        meta_props = {
+            self.client.deployments.ConfigurationMetaNames.NAME: self.deployment_name,
+            self.client.deployments.ConfigurationMetaNames.DESCRIPTION: self.deployment_description,
+            self.client.deployments.ConfigurationMetaNames.BATCH: {},
+            self.client.deployments.ConfigurationMetaNames.HARDWARE_SPEC: {'name': 'S', 'nodes': 2}  # 1 CPU is very slow
+        }
+        return meta_props
+
+    #################################################################################
+    def create_package_extension(self, yaml_file_path: str) -> str:
+        current_time = time.asctime()
+        meta_prop_pkg_ext = {
+            self.client.package_extensions.ConfigurationMetaNames.NAME: "conda_ext_" + current_time,
+            self.client.package_extensions.ConfigurationMetaNames.DESCRIPTION: "Pkg extension for conda",
+            self.client.package_extensions.ConfigurationMetaNames.TYPE: "conda_yml",
+        }
+
+        # Storing the package and saving it's uid
+        pkg_ext_id = self.client.package_extensions.get_uid(self.client.package_extensions.store(meta_props=meta_prop_pkg_ext,
+                                                                                                 file_path=yaml_file_path))
+        return pkg_ext_id
+
+    def create_software_specification(self, pkg_ext_ids: Optional[List[str]] = None) -> str:
+        """Allow for multiple package_extensions"""
+        pkg_ext_ids = (pkg_ext_ids if pkg_ext_ids is not None else [])
+
+        current_time = time.asctime()
+        # Look for the do_22.1 software specification
+        base_sw_id = self.client.software_specifications.get_uid_by_name("do_22.1")
+
+        # Create a new software specification using the default do_20.1 one as the base for it
+        meta_prop_sw_spec = {
+            self.client.software_specifications.ConfigurationMetaNames.NAME: "do_22.1_ext_"+current_time,
+            self.client.software_specifications.ConfigurationMetaNames.DESCRIPTION: "Software specification for DO example",
+            self.client.software_specifications.ConfigurationMetaNames.BASE_SOFTWARE_SPECIFICATION: {"guid": base_sw_id}
+        }
+        sw_spec_id = self.client.software_specifications.get_uid(self.client.software_specifications.store(meta_props=meta_prop_sw_spec)) # Creating the new software specification
+        for pkg_ext_id in pkg_ext_ids:
+            self.client.software_specifications.add_package_extension(sw_spec_id, pkg_ext_id) # Adding the previously created package extension to it
+        return sw_spec_id
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/domodelexporter.py` & `dse_do_utils-0.5.6.0/dse_do_utils/domodelexporter.py`

 * *Files identical despite different names*

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/mapmanager.py` & `dse_do_utils-0.5.6.0/dse_do_utils/mapmanager.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 # -----------------------------------------------------------------------------------
 # -----------------------------------------------------------------------------------
 # MapManager
 # -----------------------------------------------------------------------------------
 # -----------------------------------------------------------------------------------
 from typing import List, Tuple
 
+from folium import folium, Marker
+from folium.plugins import BeautifyIcon
+
 
 class MapManager(object):
     """Base class for building Folium map visualization.
 
     Currently, the functionality is limited, but may be extended in the future.
 
     Work-around for multi-line in popup:
@@ -274,8 +277,52 @@
         :param rows: list of tuples with name-value pairs
 
         :returns (str): text for a tooltip in table format
         """
         return MapManager.get_html_table(rows)
 
 
+    def add_bar_chart_in_map(self, m, coord,
+                             quantities=None, tooltips=None,
+                             bar_width=20, bar_height_per_unit=1,
+                             border_colors: List = None, background_colors: List = None
+                             ):
+        """Draws a bar chart at the coord. Anchor on the botton-left. Bars expand to the right.
+        Will add as many bars as there are quantities, cycling through pre-defined colors.
+
+        See also:
+        https://stackoverflow.com/questions/60131314/folium-draw-star-marker
+        https://python-visualization.github.io/folium/plugins.html#folium.plugins.BeautifyIcon
+        """
+        # Colors per bar:
+        if tooltips is None:
+            tooltips = []
+        if quantities is None:
+            quantities = []
+        if border_colors is None:
+            import plotly.express as px
+            border_colors=px.colors.qualitative.Dark2  #['green', 'blue', 'red']
+        if background_colors is None:
+            import plotly.express as px
+            background_colors=px.colors.qualitative.Set2  #['lightgreen', 'lightblue', 'lightred']
+
+        bar_anchor_x = 0
+        for i in range(len(quantities)):
+            bar_height = round(quantities[i] * bar_height_per_unit)
+            icon = BeautifyIcon(
+                icon_shape='rectangle-dot',
+                border_color=border_colors[i%len(border_colors)], # cycle back through colors
+                background_color=background_colors[i%len(background_colors)], # cycle back through colors
+                border_width=1,
+                icon_size=[bar_width, bar_height],
+                icon_anchor=[bar_anchor_x, bar_height]
+            )
+            bar_anchor_x -= bar_width
+            # folium.Marker(coord, tooltip=f"demand = {quantities[i]}", icon=icon).add_to(m)
+            if i < len(tooltips):
+                tooltip = tooltips[i]
+            else:
+                tooltip = f"value = {quantities[i]}"
+            Marker(coord, tooltip=tooltip, icon=icon).add_to(m)
+
+
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/multiscenariomanager.py` & `dse_do_utils-0.5.6.0/dse_do_utils/multiscenariomanager.py`

 * *Files identical despite different names*

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/optimizationengine.py` & `dse_do_utils-0.5.6.0/dse_do_utils/optimizationengine.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,22 +28,26 @@
     from .scenariomanager import ScenarioManager
     from .datamanager import DataManager
 except ImportError:
     # import as part of DO Model Builder
     from scenariomanager import ScenarioManager
     from datamanager import DataManager
 
+from typing import TypeVar, Generic
 
-class OptimizationEngine(object):
-    def __init__(self, data_manager: Optional[DataManager] = None, name: str = "MyOptimizationEngine",
+DM = TypeVar('DM', bound='DataManager')
+
+
+class OptimizationEngine(Generic[DM]):
+    def __init__(self, data_manager: Optional[DM] = None, name: str = "MyOptimizationEngine",
                  solve_kwargs = None, export_lp: bool = False, export_sav: bool = False, export_lp_path: str = None, is_cpo_model: bool = False):
         self.is_cpo_model = is_cpo_model
         # self.mdl: Model = Model(name=name)
         self.mdl: Union[Model, cp.CpoModel] = self.create_do_model(name=name, is_cpo_model=is_cpo_model)
-        self.dm = data_manager
+        self.dm: DM = data_manager
         self.solve_kwargs = solve_kwargs  # TODO: use in this.solve()
         self.export_lp = export_lp
         self.export_sav = export_sav  # TODO: add export to sav
         self.export_lp_path = export_lp_path
 
     def create_do_model(self, name: str, is_cpo_model: bool = False, **kwargs) -> Union[Model, cp.CpoModel]:
         """Create a model (.mdl). By default a CPLEX model (mp.Model), or a CP Optimizer model (cp.Model)
@@ -85,43 +89,43 @@
         """Returns pd.Series[BinaryVarType]"""
         return OptimizationEngine.binary_var_series_s(self.mdl, df, **kargs)
         # return pd.Series(self.mdl.binary_var_list(df.index, **kargs), index = df.index)
 
     @staticmethod
     def integer_var_series_s(mdl: docplex.mp.model, df: pd.DataFrame, **kargs) -> pd.Series:
         """Returns pd.Series[IntegerVarType]"""
-        return pd.Series(mdl.integer_var_list(df.index, **kargs), index=df.index)
+        return pd.Series(mdl.integer_var_list(df.index, **kargs), index=df.index, dtype='object')
 
     @staticmethod
     def continuous_var_series_s(mdl: docplex.mp.model, df: pd.DataFrame, **kargs) -> pd.Series:
         """Returns pd.Series[ContinuousVarType]."""
-        return pd.Series(mdl.continuous_var_list(df.index, **kargs), index=df.index)
+        return pd.Series(mdl.continuous_var_list(df.index, **kargs), index=df.index, dtype='object')
 
     @staticmethod
     def binary_var_series_s(mdl: docplex.mp.model, df: pd.DataFrame, **kargs) -> pd.Series:
         """Returns pd.Series[BinaryVarType]"""
-        return pd.Series(mdl.binary_var_list(df.index, **kargs), index=df.index)
+        return pd.Series(mdl.binary_var_list(df.index, **kargs), index=df.index, dtype='object')
 
     def semicontinuous_var_series(self, df, lb, **kargs) -> pd.Series:
         """Returns pd.Series[SemiContinuousVarType]"""
         return self.semicontinuous_var_series_s(self.mdl, df, lb, **kargs)
 
     @staticmethod
     def semicontinuous_var_series_s(mdl: docplex.mp.model, df: pd.DataFrame, lb, **kargs) -> pd.Series:
         """Returns pd.Series[SemiContinuousVarType]."""
-        return pd.Series(mdl.semicontinuous_var_list(df.index, lb, **kargs), index=df.index)
+        return pd.Series(mdl.semicontinuous_var_list(df.index, lb, **kargs), index=df.index, dtype='object')
 
     def semiinteger_var_series(self, df, lb, **kargs) -> pd.Series:
         """Returns pd.Series[SemiIntegerVarType]"""
         return self.semiinteger_var_series_s(self.mdl, df, lb, **kargs)
 
     @staticmethod
     def semiinteger_var_series_s(mdl: docplex.mp.model, df: pd.DataFrame, lb, **kargs) -> pd.Series:
         """Returns pd.Series[SemiIntegerVarType]."""
-        return pd.Series(mdl.semiinteger_var_list(df.index, lb, **kargs), index=df.index)
+        return pd.Series(mdl.semiinteger_var_list(df.index, lb, **kargs), index=df.index, dtype='object')
 
     def solve(self, refine_conflict: bool = False, **kwargs) -> docplex.mp.solution.SolveSolution:
         # TODO: enable export_as_lp_path()?
         # self.export_as_lp_path(lp_file_name=self.mdl.name)
         # TODO: use self.solve_kwargs if **kwargs is empty/None. Or merge them?
         msol = self.mdl.solve(**kwargs)  # log_output=True
         if msol is not None:
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/plotly_cpd_workaround.py` & `dse_do_utils-0.5.6.0/dse_do_utils/plotly_cpd_workaround.py`

 * *Files identical despite different names*

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/plotlymanager.py` & `dse_do_utils-0.5.6.0/dse_do_utils/plotlymanager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright IBM All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
+from typing import Generic, TypeVar
 
 # from typing import List, Dict, Tuple, Optional
 from dse_do_utils.datamanager import DataManager
 
 # import plotly
 # import plotly.graph_objs as go
 
@@ -15,21 +16,22 @@
 #         3. `fig._show()`
 #     """
 #     from IPython.display import display, HTML  # Need to import dynamically. Otherwise problems running locally in pure Python (i.e. without Jupyter)
 #     html = plotly.io.to_html(self)
 #     display(HTML(html))
 # go.Figure._show = _show
 
+DM = TypeVar('DM', bound='DataManager')
 
-class PlotlyManager():
+class PlotlyManager(Generic[DM]):
     """Holds method that create Plotly charts.
     Pass-in the DM as an input in the constructor.
     """
-    def __init__(self, dm:DataManager):
-        self.dm = dm
+    def __init__(self, dm: DM):
+        self.dm: DM = dm
 
     def get_plotly_fig_m(self, id):
         """DEPRECATED. Not used in dse_do_dashboard package.
         On the instance `self`, call the method named by id['index']
         For use with pattern-matching callbacks. Assumes the id['index'] is the name of a method of this class and returns a fig.
         Used in dse_do_dashboard Plotly-Dash dashboards
         """
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/scenariodbmanager.py` & `dse_do_utils-0.5.6.0/dse_do_utils/scenariodbmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1498,41 +1498,43 @@
             print("Delete scenario within a transaction")
             with self.engine.begin() as connection:
                 self._delete_scenario_from_db(scenario_name=scenario_name, connection=connection)
         else:
             self._delete_scenario_from_db(scenario_name=scenario_name, connection=self.engine)
 
     ##########################################################
-    def duplicate_scenario_in_db(self, source_scenario_name: str, target_scenario_name: str):
+    def duplicate_scenario_in_db(self, source_scenario_name: str, target_scenario_name: Optional[str] = None) -> str:
         """Duplicate a scenario. Uses a transaction (when enabled)."""
         if self.enable_transactions:
             print("Duplicate scenario within a transaction")
             with self.engine.begin() as connection:
-                self._duplicate_scenario_in_db(connection, source_scenario_name, target_scenario_name)
+                new_scenario_name = self._duplicate_scenario_in_db(connection, source_scenario_name, target_scenario_name)
         else:
-            self._duplicate_scenario_in_db(self.engine, source_scenario_name, target_scenario_name)
+            new_scenario_name = self._duplicate_scenario_in_db(self.engine, source_scenario_name, target_scenario_name)
+        return new_scenario_name
 
-    def _duplicate_scenario_in_db(self, connection, source_scenario_name: str, target_scenario_name: str = None):
+    def _duplicate_scenario_in_db(self, connection, source_scenario_name: str, target_scenario_name: Optional[str] = None) -> str:
         """Is fully done in DB using SQL in one SQL execute statement
         :param source_scenario_name:
         :param target_scenario_name:
         :param connection:
-        :return:
+        :return: new_scenario_name
         """
         if target_scenario_name is None:
             new_scenario_name = self._find_free_duplicate_scenario_name(source_scenario_name)
         elif self._check_free_scenario_name(target_scenario_name):
             new_scenario_name = target_scenario_name
         else:
             raise ValueError(f"Target name for duplicate scenario '{target_scenario_name}' already exists.")
 
         # inputs, outputs = self.read_scenario_from_db(source_scenario_name)
         # self._replace_scenario_in_db_transaction(scenario_name=new_scenario_name, inputs=inputs, outputs=outputs,
         #                                          bulk=True, connection=connection)
         self._duplicate_scenario_in_db_sql(connection, source_scenario_name, new_scenario_name)
+        return new_scenario_name
 
     def _duplicate_scenario_in_db_sql(self, connection, source_scenario_name: str, target_scenario_name: str = None):
         """
         :param source_scenario_name:
         :param target_scenario_name:
         :param connection:
         :return:
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/scenariomanager.py` & `dse_do_utils-0.5.6.0/dse_do_utils/scenariomanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 import glob
 import pathlib
 import zipfile
 import tempfile
 
 import docplex
 import pandas as pd
-from typing import Sequence, List, Dict, Tuple, Optional
+from typing import Sequence, List, Dict, Tuple, Optional, Union
 
 #  Typing aliases
 from dse_do_utils.utilities import convert_size
+from pathlib import Path
 
 Inputs = Dict[str, pd.DataFrame]
 Outputs = Dict[str, pd.DataFrame]
 InputsOutputs = Tuple[Inputs, Outputs]
 
 # Platform
 # Different platform require different approaches for writing data assets
@@ -78,15 +79,15 @@
         inputs, outputs = sm.load_data_from_excel('MyExcelFile')
         # Do something with the inputs or outputs
         sm.write_data_to_excel('MyExcelFileOutput')
 
     """
 
     def __init__(self, model_name: Optional[str] = None, scenario_name: Optional[str] = None,
-                 local_root: Optional[str] = None, project_id: Optional[str] = None, project_access_token: Optional[str] = None, project=None,
+                 local_root: Optional[Union[str, Path]] = None, project_id: Optional[str] = None, project_access_token: Optional[str] = None, project=None,
                  template_scenario_name: Optional[str] = None, platform: Optional[Platform] = None,
                  inputs: Inputs = None, outputs: Outputs = None,
                  local_relative_data_path: str = 'assets/data_asset', data_directory: str = None):
         """Create a ScenarioManager.
 
         Template_scenario_name: name of a scenario with an (empty but) valid model that has been successfully run at least once.
         When creating a new scenario, will copy the template scenario. This ensures the new scenario can be updated with output generated from running the Jupyter notebook.
@@ -618,15 +619,15 @@
             except PermissionError:
                 excel_file_path_1 = self.get_unique_file_name(excel_file_path_1)
                 writer_1 = pd.ExcelWriter(excel_file_path_1, engine='xlsxwriter')
         else:
             writer_1 = pd.ExcelWriter(excel_file_path_1, engine='xlsxwriter')
 
         ScenarioManager.write_data_to_excel_s(writer_1, inputs=self.inputs, outputs=self.outputs)
-        writer_1.save()
+        writer_1.close()  # .save()
 
         self.add_file_as_data_asset(excel_file_path_1, excel_file_name)
 
         # if self.platform == Platform.CPDaaS:
         #     self.add_data_file_using_project_lib(excel_file_path_1, excel_file_name + '.xlsx')
         # elif self.platform == Platform.CPD40:
         #     self.add_data_file_using_ws_lib(excel_file_path_1, excel_file_name + '.xlsx')
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/scenariopicker.py` & `dse_do_utils-0.5.6.0/dse_do_utils/scenariopicker.py`

 * *Files identical despite different names*

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils/scenariorunner.py` & `dse_do_utils-0.5.6.0/dse_do_utils/scenariorunner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # Copyright IBM All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from dataclasses import dataclass
 
 import pandas as pd
+from dse_do_utils.core.core01_optimization_engine import Core01OptimizationEngine
+
+from dse_do_utils.core.core01_data_manager import Core01DataManager
 
 from dse_do_utils import ScenarioManager, OptimizationEngine
 from dse_do_utils.datamanager import Inputs, Outputs, DataManager
 from dse_do_utils.scenariodbmanager import ScenarioDbManager
 from logging import Logger, getLogger
-from typing import Any, Dict, Optional, Tuple, NamedTuple, Type, List
+from typing import Any, Dict, Optional, Tuple, NamedTuple, Type, List, Union
+
+from dse_do_utils.scenariomanager import Platform
 
 
 @dataclass  # (frozen=True)
 class ScenarioConfig:
     scenario_name: str = 'Scenario_x'
     parameters: Dict = None  # Dict of parameters to override. Uses same names as in Parameters data table.
 
@@ -27,14 +32,15 @@
     write_output_to_excel: bool = False
     enable_data_check: bool = False
     enable_data_check_outputs: bool = False
     data_check_bulk_insert: bool = False  # False implies row-by-row
     log_level: str = 'DEBUG'  # 'DEBUG'
     export_lp: bool = False
     export_sav: bool = False
+    enable_refine_conflict: bool = False
     export_lp_path: str = ''
     do_model_name: str = None
     template_scenario_name: Optional[str] = None  # 'TemplateScenario'
 
 
 class ScenarioGenerator():
     """Generates a variation of a scenario, i.e. `inputs` dataset, driven by a ScenarioConfig.
@@ -51,15 +57,15 @@
                 new_inputs['MyTable2'] = self.generate_my_table2().reset_index()
                 return new_inputs
     """
 
     def __init__(self,
                  inputs: Inputs,
                  scenario_config: ScenarioConfig) -> None:
-        self._logger: Logger = getLogger(self.__class__.__name__)
+        self._logger: Logger = getLogger(__name__)
         self.inputs: Inputs = inputs.copy()  # Only copy of dict
         self.scenario_config: ScenarioConfig = scenario_config
 
     def generate_scenario(self):
         """Generate a variation of the base_inputs. To be overridden.
         This default implementation changes the Parameter table based on the overrides in the ScenarioConfig.parameters.
 
@@ -75,50 +81,61 @@
         new_inputs['Parameter'] = self.get_parameters().reset_index()
         return new_inputs
 
     def get_parameters(self) -> pd.DataFrame:
         """Applies overrides to the Parameter table based on the ScenarioConfig.parameters.
         """
         if self.scenario_config.parameters is None:
-            df = self.inputs['Parameter']
+            if 'Parameter' in self.inputs.keys():
+                df = self.inputs['Parameter']
+            elif 'Parameters' in self.inputs.keys():
+                df = self.inputs['Parameters']
+            else:
+                df = pd.DataFrame(columns=['param', 'value']).set_index('param')
         else:
-            df = self.inputs['Parameter'].copy().set_index(['param'])
+            if 'Parameter' in self.inputs.keys():
+                df = self.inputs['Parameter'].copy().set_index(['param'])
+            elif 'Parameters' in self.inputs.keys():
+                df = self.inputs['Parameters'].copy().set_index(['param'])
+            else:
+                df = pd.DataFrame(columns=['param', 'value']).set_index('param')
             for param, value in self.scenario_config.parameters.items():
                 df.at[param, 'value'] = value
         return df
 
 
 class ScenarioRunner:
     """
     TODO: remove local_root, local_platform, replace by data_directory? (It seems to be working fine though)
     """
     def __init__(self,
                  scenario_db_manager: ScenarioDbManager,
-                 optimization_engine_class: Type[OptimizationEngine],
-                 data_manager_class: Type[DataManager],
+                 optimization_engine_class: Type[Core01OptimizationEngine],
+                 data_manager_class: Type[Core01DataManager],
                  scenario_db_manager_class: Type[ScenarioDbManager],  # For the SQLite data check
                  scenario_generator_class: Optional[Type[ScenarioGenerator]] = None,
                  do_model_name: str = 'my_model',
                  schema: Optional[str] = None,
                  # use_scenario_db: bool = True,
                  local_root: Optional[str] = None,
-                 local_platform: Optional[int] = None,
+                 local_platform: Optional[Union[int, Platform]] = None,
                  data_directory: Optional[str] = None) -> None:
 
         self.scenario_db_manager: ScenarioDbManager = scenario_db_manager
-        self.optimization_engine_class: Type[OptimizationEngine] = optimization_engine_class
-        self.data_manager_class = data_manager_class
+        self.optimization_engine_class: Type[Core01OptimizationEngine] = optimization_engine_class
+        self.data_manager_class: Type[Core01DataManager] = data_manager_class
         self.scenario_db_manager_class = scenario_db_manager_class
         self.scenario_generator_class = scenario_generator_class
 
-        self.optimization_engine: OptimizationEngine = None  # To be set in run.
-        self.data_manager: DataManager = None  # To be set in run.
-        self.sqlite_scenario_db_manager: ScenarioDbManager = None  # To be set in run.
+        self.optimization_engine: Optional[OptimizationEngine] = None  # To be set in run.
+        self.data_manager: Optional[DataManager] = None  # To be set in run.
+        self.sqlite_scenario_db_manager: Optional[ScenarioDbManager] = None  # To be set in run.
 
-        self._logger: Logger = getLogger(self.__class__.__name__)
+        # self._logger: Logger = getLogger(self.__class__.__name__)
+        self._logger: Logger = getLogger(__name__)
         self.schema: Optional[str] = schema
         self.do_model_name: str = do_model_name
         # self.use_scenario_db: bool = use_scenario_db  # TODO: VT20220906: remove, doesn't seem to be used?
         self.local_root: Optional[str] = local_root
         self.local_platform: Optional[int] = local_platform
         self.data_directory: Optional[str] = data_directory
 
@@ -167,15 +184,15 @@
         # elif not excel_file_name and base_inputs:
         #     inputs = base_inputs
         # else:
         #     raise ValueError(
         #         'Either base_inputs or excel_file_name should be provided.')
 
         # Generate scenario
-        self._logger.info(f'Generating scenario {scenario_name}')
+        self._logger.debug(f'Generating scenario {scenario_name}')
         inputs = self.generate_scenario(base_inputs, scenario_config)
 
         # Data check
         if run_config.enable_data_check:
             inputs = self.data_check_inputs(inputs, scenario_name = scenario_config.scenario_name, bulk = run_config.data_check_bulk_insert)
 
         # Pass inputs through scenario DB
@@ -195,26 +212,26 @@
 
         if run_config.insert_in_do:
             self.insert_in_do(inputs, outputs, scenario_config, self.model_name)
 
         if run_config.write_output_to_excel:
             self.write_output_data_to_excel(inputs, outputs, scenario_name)
 
-        self._logger.info(f'Done with {scenario_config.scenario_name}')
+        self._logger.debug(f'Done with {scenario_config.scenario_name}')
 
         return outputs
 
     def create_new_db_schema(self):
         self._logger.info(f'Creating a new schema: {self.schema}')
         self.scenario_db_manager.create_schema()
 
     def _load_base_inputs(self, excel_file_name, base_inputs):
         # Load base inputs
         if excel_file_name and not base_inputs:
-            self._logger.info('Loading data from the excel file')
+            self._logger.info(f'Loading data from the excel file {excel_file_name}')
             inputs = self.load_input_data_from_excel(excel_file_name)
         elif not excel_file_name and base_inputs:
             inputs = base_inputs
         else:
             raise ValueError(
                 'Either base_inputs or excel_file_name should be provided.')
         return inputs
@@ -386,21 +403,22 @@
             inputs=inputs, log_level=run_config.log_level)  # 'DEBUG'
         self.optimization_engine: OptimizationEngine = self.optimization_engine_class(
             data_manager=self.data_manager,
             name=(run_config.do_model_name if run_config.do_model_name is not None else self.do_model_name),
             export_lp=run_config.export_lp,
             export_sav=run_config.export_sav,
             export_lp_path=run_config.export_lp_path,
+            enable_refine_conflict=run_config.enable_refine_conflict
         )
 
         return self.optimization_engine.run()
 
     def insert_outputs_in_db(self, inputs: Inputs, outputs: Outputs, run_config: RunConfig, scenario_name: str):
         self._logger.info('Inserting outputs into the database')
-        if run_config.insert_inputs_in_db:
+        if run_config.insert_outputs_in_db:
             self.scenario_db_manager.update_scenario_output_tables_in_db(scenario_name, outputs)
         else:
             self.scenario_db_manager.replace_scenario_in_db(scenario_name, inputs, outputs)
 
     def insert_in_do(self, inputs, outputs, scenario_config: ScenarioConfig,
                      run_config: RunConfig):
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils.egg-info/PKG-INFO` & `dse_do_utils-0.5.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: dse-do-utils
-Version: 0.5.5.1
-Summary: Decision Optimization utilities for IBM Watson Studio projects
+Name: dse_do_utils
+Version: 0.5.6.0
+Summary: Decision Optimization utilities for IBM Cloud Pak for Data projects
 Home-page: https://github.com/IBM/dse-decision-optimization-utilities
 Author: Victor Terpstra
 Author-email: vterpstra@us.ibm.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/IBM/dse-decision-optimization-utilities
 Project-URL: Documentation, https://ibm.github.io/dse-decision-optimization-utilities/
 Project-URL: IBM Decision Optimization, https://www.ibm.com/analytics/decision-optimization
 Description: # DSE_DO_Utils
-        Decision Optimization utilities for IBM Watson Studio Local and ICPd projects.
+        Decision Optimization utilities for IBM Cloud Pak for Data projects.
         
         [Source (GitHub)](https://github.com/IBM/dse-decision-optimization-utilities)<br>
         [Documentation (GitHubPages)](https://ibm.github.io/dse-decision-optimization-utilities/)
         
         This repository contains the package `dse_do_utils`. This can be installed using pip.
         
         ## Important
@@ -99,12 +99,12 @@
         This package requires:
         1. [decision-optimization-client](https://ibmdecisionoptimization.github.io/decision-optimization-client-doc/). This package provides an interface to the DO scenarios. 
         This package is available in PyPI, however it only runs within CP4D/CP4DaaS.
         2. [docplex](http://ibmdecisionoptimization.github.io/docplex-doc/mp/index.html). This package interfaces with the CPLEX and CP Optimizer optimization engines.
         3. [folium](https://github.com/python-visualization/folium). Map visualization. Only for the MapManager.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation :: Sphinx
 Description-Content-Type: text/markdown
```

### Comparing `dse_do_utils-0.5.5.1/dse_do_utils.egg-info/SOURCES.txt` & `dse_do_utils-0.5.6.0/dse_do_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 dse_do_utils.egg-info/top_level.txt
 dse_do_utils/core/core01_data_manager.py
 dse_do_utils/core/core01_db_manager.py
 dse_do_utils/core/core01_environment_manager.py
 dse_do_utils/core/core01_optimization_engine.py
 dse_do_utils/core/core02_data_manager.py
 dse_do_utils/core/core02_db_manager.py
-dse_do_utils/core/core02_optimization_engine.py
+dse_do_utils/core/core02_optimization_engine.py
+dse_do_utils/core/core02_scenario_runner.py
```

### Comparing `dse_do_utils-0.5.5.1/setup.py` & `dse_do_utils-0.5.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,25 +49,25 @@
 setuptools.setup(
     name="dse_do_utils",
     # version="0.2.2",
     # version=dse_do_utils.__version__,
     version=get_version("dse_do_utils/version.py"),
     author="Victor Terpstra",
     author_email="vterpstra@us.ibm.com",
-    description="Decision Optimization utilities for IBM Watson Studio projects",
+    description="Decision Optimization utilities for IBM Cloud Pak for Data projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IBM/dse-decision-optimization-utilities",
     # packages=setuptools.find_packages(),
     packages=['dse_do_utils', 'dse_do_utils.core'],
 
     classifiers=[
         "Development Status :: 4 - Beta",
         # "Development Status :: 5 - Production/Stable",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Documentation :: Sphinx"
     ],
     project_urls={  # Optional
         'Source': 'https://github.com/IBM/dse-decision-optimization-utilities',
         'Documentation': 'https://ibm.github.io/dse-decision-optimization-utilities/',
```

