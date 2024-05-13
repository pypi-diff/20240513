# Comparing `tmp/project_arrakis-0.1.2a0-py3-none-any.whl.zip` & `tmp/project_arrakis-0.1.3a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 45447 bytes, number of entries: 21
+Zip file size: 45484 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat      127 b- defN 24-Jan-23 01:40 __init__.py
 -rw-rw-rw-  2.0 fat      109 b- defN 24-Jan-23 01:40 function/__init__.py
 -rw-rw-rw-  2.0 fat    12638 b- defN 24-Mar-16 20:12 function/plots.py
 -rw-rw-rw-  2.0 fat     2034 b- defN 24-Jan-23 01:40 function/timer.py
 -rw-rw-rw-  2.0 fat    11932 b- defN 24-Jan-23 01:40 function/variables.py
 -rw-rw-rw-  2.0 fat       91 b- defN 24-Jan-23 01:40 io/__init__.py
 -rw-rw-rw-  2.0 fat    14881 b- defN 24-May-06 14:50 io/dataio.py
@@ -11,13 +11,13 @@
 -rw-rw-rw-  2.0 fat    34475 b- defN 24-May-07 13:44 streamlines/integration.py
 -rw-rw-rw-  2.0 fat    47345 b- defN 24-Mar-26 00:29 streamlines/interpolation.py
 -rw-rw-rw-  2.0 fat    15615 b- defN 24-Jan-23 01:40 streamlines/search.py
 -rw-rw-rw-  2.0 fat     7539 b- defN 24-May-04 05:02 streamlines/stochastic_model.py
 -rw-rw-rw-  2.0 fat    39741 b- defN 24-May-05 02:24 streamlines/streamlines.py
 -rw-rw-rw-  2.0 fat       89 b- defN 24-Jan-23 01:40 test_cases/__init__.py
 -rw-rw-rw-  2.0 fat    10011 b- defN 24-Mar-23 00:32 test_cases/oblique_shock_data.py
--rw-rw-rw-  2.0 fat     1093 b- defN 24-May-13 11:28 project_arrakis-0.1.2a0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1140 b- defN 24-May-13 11:28 project_arrakis-0.1.2a0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-13 11:28 project_arrakis-0.1.2a0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       44 b- defN 24-May-13 11:28 project_arrakis-0.1.2a0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1685 b- defN 24-May-13 11:28 project_arrakis-0.1.2a0.dist-info/RECORD
-21 files, 225378 bytes uncompressed, 42741 bytes compressed:  81.0%
+-rw-rw-rw-  2.0 fat     1093 b- defN 24-May-13 12:16 project_arrakis-0.1.3a0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1279 b- defN 24-May-13 12:16 project_arrakis-0.1.3a0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-13 12:16 project_arrakis-0.1.3a0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       44 b- defN 24-May-13 12:16 project_arrakis-0.1.3a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1685 b- defN 24-May-13 12:16 project_arrakis-0.1.3a0.dist-info/RECORD
+21 files, 225517 bytes uncompressed, 42778 bytes compressed:  81.0%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: test_cases/__init__.py
 Comment: 
 
 Filename: test_cases/oblique_shock_data.py
 Comment: 
 
-Filename: project_arrakis-0.1.2a0.dist-info/LICENSE
+Filename: project_arrakis-0.1.3a0.dist-info/LICENSE
 Comment: 
 
-Filename: project_arrakis-0.1.2a0.dist-info/METADATA
+Filename: project_arrakis-0.1.3a0.dist-info/METADATA
 Comment: 
 
-Filename: project_arrakis-0.1.2a0.dist-info/WHEEL
+Filename: project_arrakis-0.1.3a0.dist-info/WHEEL
 Comment: 
 
-Filename: project_arrakis-0.1.2a0.dist-info/top_level.txt
+Filename: project_arrakis-0.1.3a0.dist-info/top_level.txt
 Comment: 
 
-Filename: project_arrakis-0.1.2a0.dist-info/RECORD
+Filename: project_arrakis-0.1.3a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `project_arrakis-0.1.2a0.dist-info/LICENSE` & `project_arrakis-0.1.3a0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `project_arrakis-0.1.2a0.dist-info/METADATA` & `project_arrakis-0.1.3a0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: project-arrakis
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: One-way coupled Lagrangian Particle Tracking for CFD simulations. Includes many auxiliary tools.
 Author-email: Dilip Kalagotla <dilipkalagotla@gmail.com>
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: seaborn
+Requires-Dist: tqdm
 
 # project-arrakis
 
 Python based particle tracking algorithms for CFD data
 
 A highly parallelized set of Lagrangian particle tracking (LPT) algorithms based on Python to post-process steady and unsteady CFD data. An advanced programming interface (API) is developed for uncertainty quantification of optical velocimetry data.
```

## Comparing `project_arrakis-0.1.2a0.dist-info/RECORD` & `project_arrakis-0.1.3a0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 streamlines/integration.py,sha256=YZbyGV0-0RHN7lGRujRUquvgTL7KST3KzT_LQa23WY4,34475
 streamlines/interpolation.py,sha256=Imtt-zEx0xNVRqGsvOKp9vDdVsMGKFfO9QfF1ZZWa_0,47345
 streamlines/search.py,sha256=hC_gkCVmb9YAbx7ROFF-TgpKxmdi9HHpK8n1bMuM4mU,15615
 streamlines/stochastic_model.py,sha256=5BCc4sq58X2MT2zbbTipl9imwdYwJu8Zy57aBfqLQaA,7539
 streamlines/streamlines.py,sha256=wyeH3b8ustAw_YoYc1T7e5Zwk92PRnh4zq3PYgFlYVA,39741
 test_cases/__init__.py,sha256=swPcDEehckzkyeI5fY3W1esisEV9qZNw1OaiEiNBu_Q,89
 test_cases/oblique_shock_data.py,sha256=O0Ed55WDdMq2HIUuNf6xE2-rvtEr9VbmUCcawvSHL5o,10011
-project_arrakis-0.1.2a0.dist-info/LICENSE,sha256=457wKUHNWAX0UgtgjB9I4wpQUoS2skQEkLvqMD0R8mk,1093
-project_arrakis-0.1.2a0.dist-info/METADATA,sha256=3pzGsrT4xMWuExhZKgyL5-cyFP9u3yqxgo1h4sp58cg,1140
-project_arrakis-0.1.2a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-project_arrakis-0.1.2a0.dist-info/top_level.txt,sha256=3LCJuCT8Rv02nj80KQw_Ocm-RH8uS7vmsP4xJTebSNI,44
-project_arrakis-0.1.2a0.dist-info/RECORD,,
+project_arrakis-0.1.3a0.dist-info/LICENSE,sha256=457wKUHNWAX0UgtgjB9I4wpQUoS2skQEkLvqMD0R8mk,1093
+project_arrakis-0.1.3a0.dist-info/METADATA,sha256=6KZM6EuwqUuVKKyP_I64B2_nZnMAdIQPGHcB6zeQmSg,1279
+project_arrakis-0.1.3a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+project_arrakis-0.1.3a0.dist-info/top_level.txt,sha256=3LCJuCT8Rv02nj80KQw_Ocm-RH8uS7vmsP4xJTebSNI,44
+project_arrakis-0.1.3a0.dist-info/RECORD,,
```

