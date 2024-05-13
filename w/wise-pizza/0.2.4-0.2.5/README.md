# Comparing `tmp/wise-pizza-0.2.4.tar.gz` & `tmp/wise-pizza-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.2.4.tar", last modified: Wed Mar  6 13:59:12 2024, max compression
+gzip compressed data, was "wise-pizza-0.2.5.tar", last modified: Mon May 13 16:03:35 2024, max compression
```

## Comparing `wise-pizza-0.2.4.tar` & `wise-pizza-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-03-06 13:59:12.937899 wise-pizza-0.2.4/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8093 2024-03-06 13:59:12.937255 wise-pizza-0.2.4/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7149 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/README.md
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2024-03-06 13:59:12.937974 wise-pizza-0.2.4/setup.cfg
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1415 2024-03-06 13:58:00.000000 wise-pizza-0.2.4/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-03-06 13:59:12.911912 wise-pizza-0.2.4/tests/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8631 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/tests/test_fit.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-03-06 13:59:12.923040 wise-pizza-0.2.4/wise_pizza/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      142 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/__init__.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1731 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/cluster.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    23275 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/explain.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7431 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/find_alpha.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9193 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/make_matrix.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    12888 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/plotting.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    13312 2024-03-06 13:42:32.000000 wise-pizza-0.2.4/wise_pizza/plotting_time.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3788 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/preselect.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      329 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/run_streamlit_app_entry_point.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      553 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/segment_data.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    17460 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/slicer.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7503 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/slicer_facades.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      983 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/slicer_plotting.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4435 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/solver.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    12152 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/streamlit_app.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3700 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/time.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3228 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/transform.py
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11210 2024-03-06 13:27:20.000000 wise-pizza-0.2.4/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-03-06 13:59:12.936435 wise-pizza-0.2.4/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8093 2024-03-06 13:59:12.000000 wise-pizza-0.2.4/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      721 2024-03-06 13:59:12.000000 wise-pizza-0.2.4/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2024-03-06 13:59:12.000000 wise-pizza-0.2.4/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       91 2024-03-06 13:59:12.000000 wise-pizza-0.2.4/wise_pizza.egg-info/entry_points.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      150 2024-03-06 13:59:12.000000 wise-pizza-0.2.4/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2024-03-06 13:59:12.000000 wise-pizza-0.2.4/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:35.012511 wise-pizza-0.2.5/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    10832 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8093 2024-05-13 16:03:35.011797 wise-pizza-0.2.5/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7149 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/README.md
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      220 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2024-05-13 16:03:35.012586 wise-pizza-0.2.5/setup.cfg
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1415 2024-05-13 16:01:29.000000 wise-pizza-0.2.5/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:34.985835 wise-pizza-0.2.5/tests/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9754 2024-05-13 15:24:20.000000 wise-pizza-0.2.5/tests/test_fit.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:34.994538 wise-pizza-0.2.5/wise_pizza/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      142 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/__init__.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3869 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/cluster.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    23347 2024-05-13 15:23:28.000000 wise-pizza-0.2.5/wise_pizza/explain.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     9193 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/make_matrix.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    12938 2024-05-13 14:44:18.000000 wise-pizza-0.2.5/wise_pizza/plotting.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    13313 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/plotting_time.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3788 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/preselect.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      329 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/run_streamlit_app_entry_point.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      553 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/segment_data.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    17785 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/slicer.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7503 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/slicer_facades.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      983 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/slicer_plotting.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:35.010944 wise-pizza-0.2.5/wise_pizza/solve/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/__init__.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     7430 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/find_alpha.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     1080 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/fitter.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     4435 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/solver.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     6415 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/tree.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      697 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/solve/weighted_quantiles.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    12152 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/streamlit_app.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3700 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/time.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     3554 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/transform.py
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)    11210 2024-05-13 14:29:38.000000 wise-pizza-0.2.5/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2024-05-13 16:03:35.008402 wise-pizza-0.2.5/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     8093 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      853 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       91 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/entry_points.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      150 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2024-05-13 16:03:34.000000 wise-pizza-0.2.5/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.2.4/LICENSE` & `wise-pizza-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/PKG-INFO` & `wise-pizza-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,15 +18,15 @@
 Requires-Dist: pytest
 Requires-Dist: plotly
 Requires-Dist: scikit_learn
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: tqdm
 Requires-Dist: cloudpickle
 Requires-Dist: pivottablejs
-Requires-Dist: streamlit==1.28.0
+Requires-Dist: streamlit==1.32.0
 Provides-Extra: test
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 <img src="https://github.com/transferwise/wise-pizza/blob/main/docs/Wise_Logo.png?raw=True" width=10% height=10%>
```

### Comparing `wise-pizza-0.2.4/README.md` & `wise-pizza-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/setup.py` & `wise-pizza-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.2.4",
+    version="0.2.5",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
@@ -25,15 +25,15 @@
         "pytest",
         "plotly",
         "scikit_learn",
         "scipy>=1.8.0",
         "tqdm",
         "cloudpickle",
         "pivottablejs",
-        "streamlit==1.28.0"
+        "streamlit==1.32.0"
     ],
     extras_require={
         "test": [
             "flake8",
             "pytest",
             "pytest-cov"
         ],
```

### Comparing `wise-pizza-0.2.4/tests/test_fit.py` & `wise-pizza-0.2.5/tests/test_fit.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from wise_pizza.explain import (
     explain_changes_in_average,
     explain_changes_in_totals,
     explain_levels,
     explain_timeseries,
 )
 from wise_pizza.segment_data import SegmentData
-from wise_pizza.solver import solve_lasso, solve_lp
+from wise_pizza.solve.solver import solve_lasso, solve_lp
 from wise_pizza.time import create_time_basis
 from wise_pizza.plotting_time import plot_time
 
 np.random.seed(42)
 
 dims = [
     "TYPE",
@@ -29,26 +29,27 @@
 totals = "VOLUME"
 size = "TRANSACTION_COUNT"
 
 # possible values for explain methods
 # Too long, delete some values for quick starts, e.g. by deleting the parameters in nan_percent, size_one_percent
 deltas_test_values = [
     ("totals", "split_fits", "force_dim", "extra_dim"),  # how
-    ("lp", "lasso"),  # solver
+    ("lp", "lasso", "tree"),  # solver
     (True,),  # plot_is_static
     (explain_changes_in_average, explain_changes_in_totals),  # function
     (0.0, 90.0),  # nan_percent
     (0.0, 90.0),  # size_one_percent
+    (True, False),  # cluster_values
 ]
 # possible variants for explain methods
 deltas_test_cases = list(itertools.product(*deltas_test_values))
 
 # possible values for explain_levels
 levels_test_values = [
-    ("lp", "lasso"),  # solver
+    ("lp", "lasso", "tree"),  # solver
     (0.0, 90.0),  # nan_percent
     (0.0, 90.0),  # size_one_percent
 ]
 
 # possible variants for explain_levels
 levels_test_cases = list(itertools.product(*levels_test_values))
 
@@ -132,46 +133,79 @@
     for s in sf.segments:
         print(s)
     print(sf.summary())
     print(sf.relevant_cluster_names)
     print("yay!")
 
 
-@pytest.mark.parametrize("nan_percent", [0.0, 1.0])
-def test_synthetic_template(nan_percent: float):
-    all_data = synthetic_data(init_len=1000)
+@pytest.mark.parametrize("nan_percent, clustering", [[0.0, False], [1.0, False]])
+def test_synthetic_template(nan_percent: float, clustering: bool):
+    all_data = synthetic_data(init_len=10000, dim_values=5)
     data = all_data.data
 
     data.loc[(data["dim0"] == 0) & (data["dim1"] == 1), "totals"] += 100
     data.loc[(data["dim1"] == 0) & (data["dim2"] == 1), "totals"] += 300
 
     if nan_percent > 0:
         data = values_to_nan(data, nan_percent)
     sf = explain_levels(
         data,
         dims=all_data.dimensions,
         total_name=all_data.segment_total,
         size_name=all_data.segment_size,
         max_depth=2,
-        min_segments=5,
+        max_segments=5,
         verbose=1,
         solver="lp",
+        cluster_values=clustering,
     )
     print("***")
     for s in sf.segments:
         print(s)
 
     assert abs(sf.segments[0]["coef"] - 300) < 2
     assert abs(sf.segments[1]["coef"] - 100) < 2
 
     # sf.plot()
     print("yay!")
 
 
 @pytest.mark.parametrize("nan_percent", [0.0, 1.0])
+def test_synthetic_template_tree(nan_percent: float):
+    all_data = synthetic_data(init_len=1000)
+    data = all_data.data
+
+    data.loc[(data["dim0"] == 0) & (data["dim1"] == 1), "totals"] += 200
+    data.loc[(data["dim1"] == 0) & (data["dim2"] == 1), "totals"] += 300
+
+    if nan_percent > 0:
+        data = values_to_nan(data, nan_percent)
+    sf = explain_levels(
+        data,
+        dims=all_data.dimensions,
+        total_name=all_data.segment_total,
+        size_name=all_data.segment_size,
+        max_depth=2,
+        min_segments=5,
+        verbose=1,
+        solver="tree",
+    )
+    print("***")
+    for s in sf.segments:
+        print(s)
+
+    # TODO: insert approppriate asserts
+    # assert abs(sf.segments[0]["coef"] - 300) < 2
+    # assert abs(sf.segments[1]["coef"] - 100) < 2
+
+    # sf.plot()
+    print("yay!")
+
+
+@pytest.mark.parametrize("nan_percent", [0.0, 1.0])
 def test_synthetic_ts_template(nan_percent: float):
     all_data = synthetic_ts_data(init_len=10000)
 
     # Add some big trends to the data
     # TODO: insert trend break patterns too
     months = np.array(sorted(all_data.data[all_data.time_col].unique()))
     basis = create_time_basis(months, baseline_dims=1)
@@ -189,15 +223,15 @@
     sf = explain_timeseries(
         df,
         dims=all_data.dimensions,
         total_name=all_data.segment_total,
         time_name=all_data.time_col,
         size_name=all_data.segment_size,
         max_depth=2,
-        min_segments=5,
+        max_segments=5,
         verbose=True,
     )
     print("***")
     for s in sf.segments:
         print(s)
 
     plot_time(sf)
@@ -206,24 +240,25 @@
     assert abs(sf.segments[1]["coef"] - 100) < 2
 
     # sf.plot()
     print("yay!")
 
 
 @pytest.mark.parametrize(
-    "how, solver, plot_is_static, function, nan_percent, size_one_percent",
+    "how, solver, plot_is_static, function, nan_percent, size_one_percent, cluster_values",
     deltas_test_cases,
 )
 def test_deltas(
     how: str,
     solver: str,
     plot_is_static: bool,
     function: Callable,
     nan_percent: float,
     size_one_percent: float,
+    cluster_values: bool,
 ):
     all_data = monthly_driver_data()
     df = all_data.data
 
     months = sorted(df.COHORT_MONTH.unique())
 
     data = df[df.COHORT_MONTH == months[-1]]
@@ -238,16 +273,17 @@
         pre_data,
         data,
         all_data.dimensions,
         all_data.segment_total,
         all_data.segment_size,
         how=how,
         max_depth=1,
-        min_segments=10,
+        max_segments=10,
         solver=solver,
+        cluster_values=cluster_values
     )
     # sf.plot(plot_is_static=plot_is_static)
     print("yay!")
 
 
 @pytest.mark.parametrize("solver, nan_percent, size_one_percent", levels_test_cases)
 def test_explain_levels(solver: str, nan_percent: float, size_one_percent: float):
@@ -262,15 +298,15 @@
 
     sf = explain_levels(
         df=data,
         dims=all_data.dimensions,
         total_name=all_data.segment_total,
         size_name=all_data.segment_size,
         max_depth=1,
-        min_segments=10,
+        max_segments=10,
         solver=solver,
     )
     print(sf.summary())
     print("yay!")
 
 
 def test_solve_lasso():
```

### Comparing `wise-pizza-0.2.4/wise_pizza/explain.py` & `wise-pizza-0.2.5/wise_pizza/explain.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 def explain_changes_in_average(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     dims: List[str],
     total_name: str,
     size_name: str,
-    min_segments: int = 5,
-    max_segments: Optional[int] = None,
+    min_segments: Optional[int] = None,
+    max_segments: int = 5,
     min_depth: int = 1,
     max_depth: int = 2,
     solver: str = "lasso",
     how: str = "totals",
     force_add_up: bool = False,
     constrain_signs: bool = True,
     cluster_values: bool = False,
@@ -119,16 +119,16 @@
 
 def explain_changes_in_totals(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     dims: List[str],
     total_name: str,
     size_name: str,
-    min_segments: int = 5,
-    max_segments: Optional[int] = None,
+    min_segments: Optional[int] = None,
+    max_segments: int = 5,
     min_depth: int = 1,
     max_depth: int = 2,
     solver: str = "lasso",
     how: str = "totals",
     force_add_up: bool = False,
     constrain_signs: bool = True,
     cluster_values: bool = False,
@@ -220,15 +220,14 @@
         sp = SlicerPair(sf_size, sf_avg)
         sp.plot = lambda plot_is_static=False, width=2000, height=500, cluster_key_width=180, cluster_value_width=318, return_fig=False: plot_split_segments(
             sp.s1,
             sp.s2,
             plot_is_static=plot_is_static,
             width=width,
             height=height,
-            cluster_values=cluster_values,
             cluster_key_width=cluster_key_width,
             cluster_value_width=cluster_value_width,
             return_fig=return_fig,
         )
         return sp
 
     else:
@@ -254,30 +253,29 @@
         sf.post_total = df2[total_name].sum()
 
         sf.plot = lambda plot_is_static=False, width=1000, height=1000, cluster_key_width=180, cluster_value_width=318, return_fig=False: plot_waterfall(
             sf,
             plot_is_static=plot_is_static,
             width=width,
             height=height,
-            cluster_values=cluster_values,
             cluster_key_width=cluster_key_width,
             cluster_value_width=cluster_value_width,
             return_fig=return_fig,
         )
         sf.task = "changes in totals"
         return sf
 
 
 def explain_levels(
     df: pd.DataFrame,
     dims: List[str],
     total_name: str,
     size_name: Optional[str] = None,
-    min_segments: int = 10,
-    max_segments: int = None,
+    min_segments: int = None,
+    max_segments: int = 10,
     min_depth: int = 1,
     max_depth: int = 2,
     solver="lasso",
     verbose=0,
     force_add_up: bool = False,
     constrain_signs: bool = True,
     cluster_values: bool = False,
@@ -337,34 +335,34 @@
     sf.reg.intercept_ = average
     sf.plot = lambda plot_is_static=False, width=2000, height=500, return_fig=False, cluster_key_width=180, cluster_value_width=318: plot_segments(
         sf,
         plot_is_static=plot_is_static,
         width=width,
         height=height,
         return_fig=return_fig,
-        cluster_values=cluster_values,
         cluster_key_width=cluster_key_width,
         cluster_value_width=cluster_value_width,
     )
     sf.task = "levels"
     return sf
 
 
 def explain_timeseries(
     df: pd.DataFrame,
     dims: List[str],
     total_name: str,
     time_name: str,
     size_name: Optional[str] = None,
-    min_segments: int = 5,
-    max_segments: int = None,
+    min_segments: int = None,
+    max_segments: int = 5,
     min_depth: int = 1,
     max_depth: int = 2,
     solver: str = "omp",
     verbose: bool = False,
+    constrain_signs: bool = False,
     cluster_values: bool = False,
     time_basis: Optional[pd.DataFrame] = None,
     fit_log_space: bool = False,
     fit_sizes: Optional[bool] = None,
     log_space_weight_sc: float = 0.5,
 ):
     df = copy.copy(df)
@@ -384,15 +382,18 @@
             raise ValueError("fit_sizes should be None or False if size_name is None")
         fit_sizes = False
     else:
         if fit_sizes is None:
             fit_sizes = True
 
     if fit_log_space:
-        tf = LogTransform(offset=1, weight_pow_sc=log_space_weight_sc)
+        tf = LogTransform(
+            offset=1,
+            weight_pow_sc=log_space_weight_sc,
+        )
     else:
         tf = IdentityTransform()
 
     size_name_orig = size_name + "_orig"
     total_name_orig = total_name + "_orig"
 
     df2 = df.rename(columns={size_name: size_name_orig, total_name: total_name_orig})
@@ -411,14 +412,15 @@
             size_name=size_name,
             min_segments=min_segments,
             max_segments=max_segments,
             min_depth=min_depth,
             max_depth=max_depth,
             solver=solver,
             verbose=verbose,
+            constrain_signs=constrain_signs,
             cluster_values=cluster_values,
             time_basis=time_basis,
         )
         return TransformedSliceFinder(sf_totals, transformer=tf)
 
     this_w = np.ones_like(df2[size_name_orig].values)
     these_totals = df2[size_name_orig].values
@@ -437,14 +439,15 @@
         time_name=time_name,
         min_segments=min_segments,
         max_segments=max_segments,
         min_depth=min_depth,
         max_depth=max_depth,
         solver=solver,
         verbose=verbose,
+        constrain_signs=constrain_signs,
         cluster_values=cluster_values,
         time_basis=time_basis,
     )
 
     sf1 = TransformedSliceFinder(sf_wgt, transformer=tf)
 
     # Replace actual weights with fitted ones, for consistent extrapolation
@@ -473,14 +476,15 @@
         size_name=size_name,
         min_segments=min_segments,
         max_segments=max_segments,
         min_depth=min_depth,
         max_depth=max_depth,
         solver=solver,
         verbose=verbose,
+        constrain_signs=constrain_signs,
         cluster_values=cluster_values,
         time_basis=time_basis,
     )
 
     assert almost_equals(t, sf_totals.actual_totals)
     assert almost_equals(w, sf_totals.weights)
 
@@ -509,16 +513,16 @@
 
 def _explain_timeseries(
     df: pd.DataFrame,
     dims: List[str],
     total_name: str,
     time_name: str,
     size_name: Optional[str] = None,
-    min_segments: int = 5,
-    max_segments: int = None,
+    min_segments: int = None,
+    max_segments: int = 5,
     min_depth: int = 1,
     max_depth: int = 2,
     solver: str = "omp",
     verbose: bool = False,
     force_add_up: bool = False,
     constrain_signs: bool = False,
     cluster_values: bool = False,
```

### Comparing `wise-pizza-0.2.4/wise_pizza/find_alpha.py` & `wise-pizza-0.2.5/wise_pizza/solve/find_alpha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pandas as pd
 from scipy.sparse import vstack, csr_array, issparse
-from scipy.linalg import svd, expm
+from scipy.linalg import svd
 
-from wise_pizza.solver import solve_lasso, solve_lp, solve_omp
+from wise_pizza.solve.solver import solve_lasso, solve_lp, solve_omp
 
 
 def find_alpha(
     X,
     y_,
     max_nonzeros=None,
     min_nonzeros=None,
@@ -118,15 +118,15 @@
     if use_proj:
         mat = small_mat
         y = small_y
     else:
         mat = X
         y = y_
 
-    if solver=="omp":
+    if solver == "omp":
         reg, nonzeros = solve_omp(mat.toarray(), y, min_nonzeros)
         return reg, nonzeros
 
     alpha = 2 * max(y)
     nonzeros = []
     iter = 0
 
@@ -139,17 +139,14 @@
         d = (err1 * err1).sum() - (err2 * err2).sum() - yerr
         if verbose is not None:
             print("errors", sqerr1, sqerr2)
 
     if verbose:
         print_errors(np.zeros(X.shape[1]))
 
-
-
-
     while len(nonzeros) < min_nonzeros:
         alpha /= 2
         reg = solve(
             mat,
             y,
             alpha,
             constrain_signs=constrain_signs,
```

### Comparing `wise-pizza-0.2.4/wise_pizza/make_matrix.py` & `wise-pizza-0.2.5/wise_pizza/make_matrix.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/wise_pizza/plotting.py` & `wise-pizza-0.2.5/wise_pizza/plotting.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 def plot_split_segments(
     sf_size: "SliceFinder",
     sf_avg: "SliceFinder",
     plot_is_static: bool = False,
     width: int = 2000,
     height: int = 500,
-    cluster_values: bool = False,
     cluster_key_width: int = 180,
     cluster_value_width: int = 318,
     return_fig: bool = False,
 ):
     """
     Plot split segments for explain_changes: split_fits
     @param sf_size: SliceFinder from sizes
@@ -109,15 +108,15 @@
         row=2,
         annotation_text="Global average",
     )
 
     for i in range(1, 3):
         fig.update_yaxes(autorange="reversed", row=i)
 
-    if cluster_values:
+    if sf_size.relevant_cluster_names:
         data_dict = sf_size.relevant_cluster_names
         keys = list(data_dict.keys())
         values = list(data_dict.values())
         key_column_width = cluster_key_width  # Adjust the multiplier as needed
         value_column_width = cluster_value_width  # Adjust the multiplier as needed
 
         # Create a table trace with specified column widths
@@ -135,15 +134,15 @@
         # Create a figure
         fig2 = go.Figure(data=[table_trace], layout=layout)
 
     if plot_is_static:
         # Convert the figure to a static image
         image_bytes = to_image(fig, format="png", scale=2)
 
-        if cluster_values:
+        if sf_size.relevant_cluster_names:
             display(
                 Image(
                     image_bytes,
                     height=height + len(size_data.index) * 30,
                     width=width + len(size_data.index) * 30,
                 )
             )
@@ -154,30 +153,29 @@
             return Image(
                 image_bytes,
                 height=height + len(size_data.index) * 30,
                 width=width + len(size_data.index) * 30,
             )
     else:
         if return_fig:
-            if cluster_values:
+            if sf_size.relevant_cluster_names:
                 return [fig, fig2]
             else:
                 return fig
         fig.show()
-        if cluster_values:
+        if sf_size.relevant_cluster_names:
             fig2.show()
 
 
 def plot_segments(
     sf: "SliceFinder",
     plot_is_static: bool = False,
     width: int = 2000,
     height: int = 500,
     return_fig: bool = False,
-    cluster_values: bool = False,
     cluster_key_width: int = 180,
     cluster_value_width: int = 318,
 ):
     """
     Plot segments for explain_levels
     @param sf: SliceFinder
     @param plot_is_static: static (True) or dynamic (False) plotly result
@@ -240,15 +238,15 @@
         line_width=3,
         line_dash="dash",
         line_color="red",
         col=2,
         annotation_text="Global average",
     )
 
-    if cluster_values:
+    if sf.relevant_cluster_names:
         data_dict = sf.relevant_cluster_names
         keys = list(data_dict.keys())
         values = list(data_dict.values())
         key_column_width = cluster_key_width  # Adjust the multiplier as needed
         value_column_width = cluster_value_width  # Adjust the multiplier as needed
 
         # Create a table trace with specified column widths
@@ -267,15 +265,15 @@
         fig2 = go.Figure(data=[table_trace], layout=layout)
 
     if plot_is_static:
         # Convert the figure to a static image
         image_bytes = to_image(fig, format="png", scale=2)
 
         # Display the static image in the Jupyter notebook
-        if cluster_values:
+        if sf.relevant_cluster_names:
             image_bytes2 = to_image(fig2, format="png", scale=2)
             display(
                 Image(
                     image_bytes,
                     height=height + len(sf.segment_labels) * 30,
                     width=width + len(sf.segment_labels) * 30,
                 )
@@ -285,21 +283,21 @@
             return Image(
                 image_bytes,
                 height=height + len(sf.segment_labels) * 30,
                 width=width + len(sf.segment_labels) * 30,
             )
     else:
         if return_fig:
-            if cluster_values:
+            if sf.relevant_cluster_names:
                 return [fig, fig2]
             else:
                 return fig
         else:
             fig.show()
-            if cluster_values:
+            if sf.relevant_cluster_names:
                 fig2.show()
 
 
 def waterfall_args(sf: "SliceFinder"):
     """
     Waterfall plot arguments
     @param sf: SliceFinder
@@ -356,15 +354,14 @@
 
 
 def plot_waterfall(
     sf: "SliceFinder",
     plot_is_static: bool = False,
     width: int = 1000,
     height: int = 1000,
-    cluster_values: bool = False,
     cluster_key_width: int = 180,
     cluster_value_width: int = 318,
     return_fig: bool = False,
 ):
     """
     Plot waterfall and Bar for explain_changes
     @param sf: SliceFinder
@@ -383,15 +380,15 @@
 
     fig.update_layout(
         title="Segments contributing most to the change",
         #         showlegend = True,
         **waterfall_layout_args(sf, width, height),
     )
 
-    if cluster_values:
+    if sf.relevant_cluster_names:
         data_dict = sf.relevant_cluster_names
         keys = list(data_dict.keys())
         values = list(data_dict.values())
         key_column_width = cluster_key_width  # Adjust the multiplier as needed
         value_column_width = cluster_value_width  # Adjust the multiplier as needed
 
         # Create a table trace with specified column widths
@@ -408,22 +405,22 @@
 
         # Create a figure
         fig2 = go.Figure(data=[table_trace], layout=layout)
 
     if plot_is_static:
         # Convert the figure to a static image
         image_bytes = to_image(fig, format="png", scale=2)
-        if cluster_values:
+        if sf.relevant_cluster_names:
             display(Image(image_bytes, height=height, width=width))
             fig2.show()
         else:
             # Display the static image in the Jupyter notebook
             display(Image(image_bytes, width=width, height=height))
     else:
         if return_fig:
-            if cluster_values:
+            if sf.relevant_cluster_names:
                 return [fig, fig2]
             else:
                 return fig
         fig.show()
-        if cluster_values:
+        if sf.relevant_cluster_names:
             fig2.show()
```

### Comparing `wise-pizza-0.2.4/wise_pizza/plotting_time.py` & `wise-pizza-0.2.5/wise_pizza/plotting_time.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -427,8 +427,8 @@
                     marker=dict(color="#ff685f"),
                     showlegend=showlegend and col == col_nums[0],
                 ),
                 row=row_num,
                 col=col,
             )
 
-    return min_impact, max_impact
+    return min_impact, max_impact
```

### Comparing `wise-pizza-0.2.4/wise_pizza/preselect.py` & `wise-pizza-0.2.5/wise_pizza/preselect.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/wise_pizza/segment_data.py` & `wise-pizza-0.2.5/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/wise_pizza/slicer.py` & `wise-pizza-0.2.5/wise_pizza/slicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from typing import Optional, Union, List, Dict, Sequence
 from collections import defaultdict
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csc_matrix, diags
 
-from wise_pizza.find_alpha import clean_up_min_max, find_alpha
+from wise_pizza.solve.find_alpha import clean_up_min_max, find_alpha
 from wise_pizza.make_matrix import sparse_dummy_matrix
-from wise_pizza.cluster import guided_kmeans
+from wise_pizza.cluster import make_clusters
 from wise_pizza.preselect import HeuristicSelector
 from wise_pizza.time import extend_dataframe
 from wise_pizza.slicer_facades import SliceFinderPredictFacade
+from wise_pizza.solve.tree import tree_solver
+from wise_pizza.solve.solver import solve_lasso
 
 
 def _summary(obj) -> str:
     out = {"task": obj.task, "segments": obj.segments}
     return json.dumps(out)
 
 
@@ -111,44 +113,50 @@
         Function to fit slicer and find segments
         @param dim_df: Dataset with dimensions
         @param totals: Column with totals
         @param weights: Column with sizes
         @param min_segments: Minimum number of segments to find
         @param max_segments: Maximum number of segments to find, defaults to min_segments
         @param min_depth: Minimum number of dimension to constrain in segment definition
-        @param max_depth: Maximum number of dimension to constrain in segment definition
-        @param solver: If this equals to "lp" uses the LP solver, else uses the (recommended) Lasso solver
+        @param max_depth: Maximum number of dimensions to constrain in segment definition; also max depth pf tree in tree solver
+        @param solver: Valid values are "lasso" (default), "tree" (for non-overlapping segments), "omp", or "lp"
         @param verbose: If set to a truish value, lots of debug info is printed to console
         @param force_dim: To add dim
         @param force_add_up: To force add up
         @param constrain_signs: To constrain signs
         @param cluster_values In addition to single-value slices, consider slices that consist of a
         group of segments from the same dimension with similar naive averages
 
         """
+
+        assert solver.lower() in ["lasso", "tree", "omp", "lp"]
         min_segments, max_segments = clean_up_min_max(min_segments, max_segments)
         if verbose is not None:
             self.verbose = verbose
 
         totals = np.array(totals).astype(np.float64)
 
         if weights is None:
             weights = np.ones_like(totals)
         else:
             weights = np.array(weights).astype(np.float64)
 
         assert min(weights) >= 0
         assert np.sum(np.abs(totals[weights == 0])) == 0
 
+        # Cast all dimension values to strings
+        dim_df = dim_df.astype(str)
+
         dims = list(dim_df.columns)
         # sort the dataframe by dimension values,
         # making sure the other vectors stay aligned
         dim_df = dim_df.reset_index(drop=True)
         dim_df["totals"] = totals
         dim_df["weights"] = weights
+
         if time_col is not None:
             dim_df["__time"] = time_col
             dim_df = pd.merge(dim_df, time_basis, left_on="__time", right_index=True)
             sort_dims = dims + ["__time"]
         else:
             sort_dims = dims
 
@@ -172,78 +180,82 @@
         self.weights = dim_df["weights"].values
         self.totals = dim_df["totals"].values
 
         # While we still have weights and totals as part of the dataframe, let's produce clusters
         # of dimension values with similar outcomes
         clusters = defaultdict(list)
         self.cluster_names = {}
-        if cluster_values:
-            for dim in dims:
-                if (
-                    len(dim_df[dim].unique()) >= 6
-                ):  # otherwise what's the point in clustering?
-                    grouped_df = (
-                        dim_df[[dim, "totals", "weights"]]
-                        .groupby(dim, as_index=False)
-                        .sum()
-                    )
-                    grouped_df["avg"] = grouped_df["totals"] / grouped_df["weights"]
-                    grouped_df["cluster"], _ = guided_kmeans(grouped_df["avg"])
-                    pre_clusters = (
-                        grouped_df[["cluster", dim]]
-                        .groupby("cluster")
-                        .agg({dim: lambda x: "@@".join(x)})
-                        .values
-                    )
-                    # filter out clusters with only one element
-                    these_clusters = [c for c in pre_clusters.reshape(-1) if "@@" in c]
-                    # create short cluster names
-                    for i, c in enumerate(these_clusters):
-                        self.cluster_names[f"{dim}_cluster_{i+1}"] = c
+
+        if solver == "tree":
+            if cluster_values:
+                warnings.warn(
+                    "Ignoring cluster_values argument as tree solver makes its own clusters"
+                )
+            self.X, self.col_defs, self.cluster_names = tree_solver(
+                dim_df=dim_df,
+                dims=dims,
+                time_basis=self.time_basis,
+                num_leaves=max_segments,
+                max_depth=max_depth,
+            )
+            self.nonzeros = np.array(range(self.X.shape[1]))
+            Xw = csc_matrix(diags(self.weights) @ self.X)
+            self.reg = solve_lasso(
+                Xw.toarray(),
+                self.totals,
+                alpha=1e-5,
+                verbose=self.verbose,
+                fit_intercept=False,
+            )
+            print("")
+        else:
+            if cluster_values:
+                self.cluster_names = make_clusters(dim_df, dims)
+                for dim in dims:
                     clusters[dim] = [
                         c for c in self.cluster_names.keys() if c.startswith(dim)
                     ]
 
-        dim_df = dim_df[dims]  # if time_col is None else dims + ["__time"]]
-        self.dim_df = dim_df
-
-        # lazy calculation of the dummy matrix (calculation can be very slow)
-        if (
-            list(dim_df.columns) != self.dims
-            or max_depth != self.max_depth
-            or self.X is not None
-            and len(dim_df) != self.X.shape[1]
-        ):
-            self.X, self.col_defs = self._init_mat(
-                dim_df,
-                min_depth,
-                max_depth,
-                force_dim=force_dim,
-                clusters=clusters,
-                time_basis=self.time_basis,
+            dim_df = dim_df[dims]  # if time_col is None else dims + ["__time"]]
+            self.dim_df = dim_df
+            # lazy calculation of the dummy matrix (calculation can be very slow)
+            if (
+                list(dim_df.columns) != self.dims
+                or max_depth != self.max_depth
+                or self.X is not None
+                and len(dim_df) != self.X.shape[1]
+            ):
+                self.X, self.col_defs = self._init_mat(
+                    dim_df,
+                    min_depth,
+                    max_depth,
+                    force_dim=force_dim,
+                    clusters=clusters,
+                    time_basis=self.time_basis,
+                )
+                assert len(self.col_defs) == self.X.shape[1]
+                self.min_depth = min_depth
+                self.max_depth = max_depth
+                self.dims = list(dim_df.columns)
+
+            Xw = csc_matrix(diags(self.weights) @ self.X)
+
+            if self.verbose:
+                print("Starting solve!")
+            self.reg, self.nonzeros = find_alpha(
+                Xw,
+                self.totals,
+                max_nonzeros=max_segments,
+                solver=solver,
+                min_nonzeros=min_segments,
+                verbose=self.verbose,
+                adding_up_regularizer=force_add_up,
+                constrain_signs=constrain_signs,
             )
-            assert len(self.col_defs) == self.X.shape[1]
-            self.min_depth = min_depth
-            self.max_depth = max_depth
-            self.dims = list(dim_df.columns)
 
-        Xw = csc_matrix(diags(self.weights) @ self.X)
-
-        if self.verbose:
-            print("Starting solve!")
-        self.reg, self.nonzeros = find_alpha(
-            Xw,
-            self.totals,
-            max_nonzeros=max_segments,
-            solver=solver,
-            min_nonzeros=min_segments,
-            verbose=self.verbose,
-            adding_up_regularizer=force_add_up,
-            constrain_signs=constrain_signs,
-        )
         if self.verbose:
             print("Solver done!!")
 
         self.segments = [
             {"segment": self.col_defs[i], "index": int(i)} for i in self.nonzeros
         ]
 
@@ -272,15 +284,16 @@
                 dummy = this_vec
 
             this_wgts = self.weights * dummy
             wgt = this_wgts.sum()
             # assert wgt == wgts[i]
             s["orig_i"] = i
             s["coef"] = self.reg.coef_[i]
-            s["impact"] = np.abs(s["coef"]) * (np.abs(this_vec) * self.weights).sum()
+            # TODO: does not taking the abs of coef here break time series?
+            s["impact"] = s["coef"] * (np.abs(this_vec) * self.weights).sum()
             s["avg_impact"] = s["impact"] / sum(self.weights)
             s["total"] = (self.totals * dummy).sum()
             s["seg_size"] = wgt
             s["naive_avg"] = s["total"] / wgt
 
         if time_basis is not None:  # it's a time series product
             # Do we need this bit at all?
```

### Comparing `wise-pizza-0.2.4/wise_pizza/slicer_facades.py` & `wise-pizza-0.2.5/wise_pizza/slicer_facades.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/wise_pizza/slicer_plotting.py` & `wise-pizza-0.2.5/wise_pizza/slicer_plotting.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/wise_pizza/solver.py` & `wise-pizza-0.2.5/wise_pizza/solve/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/wise_pizza/streamlit_app.py` & `wise-pizza-0.2.5/wise_pizza/streamlit_app.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/wise_pizza/time.py` & `wise-pizza-0.2.5/wise_pizza/time.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/wise_pizza/transform.py` & `wise-pizza-0.2.5/wise_pizza/transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self, t_total: np.ndarray, t_w: np.ndarray
     ) -> Tuple[np.ndarray, np.ndarray]:
         t_mean = t_total / t_w
         mean = self.inverse_transform_mean(t_mean)
         w = self.inverse_transform_weight(t_w, t_mean)
         return mean * w, w
 
-    def test_transforms(self, total, weights, eps=1e-6):
+    def test_transforms(self, total, weights, eps=1e-4):
         mean = total / weights
         t_mean = self.transform_mean(mean)
         assert almost_equals(mean, self.inverse_transform_mean(t_mean), eps)
 
         t_w = self.transform_weight(weights, mean)
         re_w = self.inverse_transform_weight(t_w, t_mean)
         assert almost_equals(weights, re_w, eps)
@@ -67,27 +67,36 @@
 
     def inverse_transform_weight(self, w: np.ndarray, x: np.ndarray) -> np.ndarray:
         return w
 
 
 class LogTransform(TransformWithWeights):
     def __init__(
-        self, offset: float, weight_pow_sc: float = 0.1, max_inverse: float = 1e6
+        self, offset: float, weight_pow_sc: float = 0.1, cap_inverse: bool = True
     ):
         self.offset = offset
         self.weight_pow_sc = weight_pow_sc
-        self.max_inverse = max_inverse
+        self.cap_inverse = cap_inverse
+        if cap_inverse:
+            self.max_inverse = 0.0
+        else:
+            self.max_inverse = None
 
     def transform_mean(self, x: np.ndarray) -> np.ndarray:
+        if self.cap_inverse:
+            self.max_inverse = np.maximum(self.max_inverse, 2 * x.max())
         return np.log(self.offset + x)
 
     def inverse_transform_mean(self, x: np.ndarray) -> np.ndarray:
-        return np.maximum(
-            0.0, np.exp(np.minimum(x, np.log(self.max_inverse))) - self.offset
-        )
+        if self.cap_inverse:
+            return np.maximum(
+                0.0, np.exp(np.minimum(x, np.log(self.max_inverse))) - self.offset
+            )
+        else:
+            return np.maximum(0.0, np.exp(x) - self.offset)
 
     def transform_weight(self, w: np.ndarray, mean: np.ndarray) -> np.ndarray:
         # pure math would give weight_pow_sc = 1, but then
         # there's too much information from actuals being leaked into the weights,
         # so the
         return w * np.power(self.offset + mean, self.weight_pow_sc)
```

### Comparing `wise-pizza-0.2.4/wise_pizza/utils.py` & `wise-pizza-0.2.5/wise_pizza/utils.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.2.4/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.2.5/wise_pizza.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,15 +18,15 @@
 Requires-Dist: pytest
 Requires-Dist: plotly
 Requires-Dist: scikit_learn
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: tqdm
 Requires-Dist: cloudpickle
 Requires-Dist: pivottablejs
-Requires-Dist: streamlit==1.28.0
+Requires-Dist: streamlit==1.32.0
 Provides-Extra: test
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 <img src="https://github.com/transferwise/wise-pizza/blob/main/docs/Wise_Logo.png?raw=True" width=10% height=10%>
```

### Comparing `wise-pizza-0.2.4/wise_pizza.egg-info/SOURCES.txt` & `wise-pizza-0.2.5/wise_pizza.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 README.md
 pyproject.toml
 setup.py
 tests/test_fit.py
 wise_pizza/__init__.py
 wise_pizza/cluster.py
 wise_pizza/explain.py
-wise_pizza/find_alpha.py
 wise_pizza/make_matrix.py
 wise_pizza/plotting.py
 wise_pizza/plotting_time.py
 wise_pizza/preselect.py
 wise_pizza/run_streamlit_app_entry_point.py
 wise_pizza/segment_data.py
 wise_pizza/slicer.py
 wise_pizza/slicer_facades.py
 wise_pizza/slicer_plotting.py
-wise_pizza/solver.py
 wise_pizza/streamlit_app.py
 wise_pizza/time.py
 wise_pizza/transform.py
 wise_pizza/utils.py
 wise_pizza.egg-info/PKG-INFO
 wise_pizza.egg-info/SOURCES.txt
 wise_pizza.egg-info/dependency_links.txt
 wise_pizza.egg-info/entry_points.txt
 wise_pizza.egg-info/requires.txt
-wise_pizza.egg-info/top_level.txt
+wise_pizza.egg-info/top_level.txt
+wise_pizza/solve/__init__.py
+wise_pizza/solve/find_alpha.py
+wise_pizza/solve/fitter.py
+wise_pizza/solve/solver.py
+wise_pizza/solve/tree.py
+wise_pizza/solve/weighted_quantiles.py
```

