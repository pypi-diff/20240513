# Comparing `tmp/antakia_core-0.4.4.tar.gz` & `tmp/antakia_core-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antakia_core-0.4.4.tar", max compression
+gzip compressed data, was "antakia_core-0.4.5.tar", max compression
```

## Comparing `antakia_core-0.4.4.tar` & `antakia_core-0.4.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1497 2024-03-19 14:18:22.609303 antakia_core-0.4.4/LICENSE
--rw-r--r--   0        0        0       54 2024-03-19 14:18:22.609385 antakia_core-0.4.4/README.md
--rw-r--r--   0        0        0      758 2024-04-29 14:00:54.227196 antakia_core-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      110 2024-03-19 14:18:22.610283 antakia_core-0.4.4/src/antakia_core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610377 antakia_core-0.4.4/src/antakia_core/compute/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610480 antakia_core-0.4.4/src/antakia_core/compute/dim_reduction/__init__.py
--rw-r--r--   0        0        0     7261 2024-04-23 14:56:02.573651 antakia_core-0.4.4/src/antakia_core/compute/dim_reduction/dim_reduc_method.py
--rw-r--r--   0        0        0     7926 2024-04-25 14:03:01.843934 antakia_core-0.4.4/src/antakia_core/compute/dim_reduction/dim_reduction.py
--rw-r--r--   0        0        0       75 2024-03-22 17:21:14.615326 antakia_core-0.4.4/src/antakia_core/compute/dim_reduction/pacmap_progress/__init__.py
--rw-r--r--   0        0        0    40149 2024-03-22 17:21:15.061170 antakia_core-0.4.4/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610898 antakia_core-0.4.4/src/antakia_core/compute/model_subtitution/__init__.py
--rw-r--r--   0        0        0      840 2024-03-21 16:04:55.999992 antakia_core-0.4.4/src/antakia_core/compute/model_subtitution/classification_models.py
--rw-r--r--   0        0        0     3733 2024-04-23 14:51:04.769035 antakia_core-0.4.4/src/antakia_core/compute/model_subtitution/model_class.py
--rw-r--r--   0        0        0     8139 2024-04-23 14:51:04.885872 antakia_core-0.4.4/src/antakia_core/compute/model_subtitution/model_interface.py
--rw-r--r--   0        0        0     1842 2024-03-19 14:18:22.611366 antakia_core-0.4.4/src/antakia_core/compute/model_subtitution/regression_models.py
--rw-r--r--   0        0        0     1785 2024-04-23 14:50:36.703592 antakia_core-0.4.4/src/antakia_core/compute/skope_rule/skope_rule.py
--rw-r--r--   0        0        0      192 2024-03-19 14:18:22.611682 antakia_core-0.4.4/src/antakia_core/data_handler/__init__.py
--rw-r--r--   0        0        0     3969 2024-04-23 14:51:04.148770 antakia_core-0.4.4/src/antakia_core/data_handler/projected_values.py
--rw-r--r--   0        0        0       98 2024-03-19 14:18:22.611895 antakia_core-0.4.4/src/antakia_core/data_handler/region.py
--rw-r--r--   0        0        0     9794 2024-04-29 13:44:05.319988 antakia_core-0.4.4/src/antakia_core/data_handler/region_.py
--rw-r--r--   0        0        0    10674 2024-04-23 14:50:36.705105 antakia_core-0.4.4/src/antakia_core/data_handler/region_set.py
--rw-r--r--   0        0        0    10089 2024-04-23 14:50:36.705350 antakia_core-0.4.4/src/antakia_core/data_handler/rule.py
--rw-r--r--   0        0        0     4434 2024-04-23 14:50:36.706070 antakia_core-0.4.4/src/antakia_core/data_handler/rules.py
--rw-r--r--   0        0        0      190 2024-03-19 14:18:22.612650 antakia_core-0.4.4/src/antakia_core/explanation/__init__.py
--rw-r--r--   0        0        0     2129 2024-03-29 12:59:56.497027 antakia_core-0.4.4/src/antakia_core/explanation/explanation_method.py
--rw-r--r--   0        0        0     4778 2024-04-23 09:45:08.541634 antakia_core-0.4.4/src/antakia_core/explanation/explanations.py
--rw-r--r--   0        0        0      307 2024-03-19 14:18:22.612977 antakia_core-0.4.4/src/antakia_core/utils/__init__.py
--rw-r--r--   0        0        0     2031 2024-04-23 14:51:04.685563 antakia_core-0.4.4/src/antakia_core/utils/correlation_coef.py
--rw-r--r--   0        0        0     1302 2024-03-29 13:06:13.987832 antakia_core-0.4.4/src/antakia_core/utils/long_task.py
--rw-r--r--   0        0        0      561 2024-04-23 14:51:04.692721 antakia_core-0.4.4/src/antakia_core/utils/splittable_callback.py
--rw-r--r--   0        0        0     4576 2024-04-23 09:45:08.541955 antakia_core-0.4.4/src/antakia_core/utils/utils.py
--rw-r--r--   0        0        0    12510 2024-04-23 09:45:08.542559 antakia_core-0.4.4/src/antakia_core/utils/variable.py
--rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 antakia_core-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-03-19 14:18:22.609303 antakia_core-0.4.5/LICENSE
+-rw-r--r--   0        0        0       54 2024-03-19 14:18:22.609385 antakia_core-0.4.5/README.md
+-rw-r--r--   0        0        0      758 2024-05-13 10:17:54.476144 antakia_core-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-03-19 14:18:22.610283 antakia_core-0.4.5/src/antakia_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610377 antakia_core-0.4.5/src/antakia_core/compute/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610480 antakia_core-0.4.5/src/antakia_core/compute/dim_reduction/__init__.py
+-rw-r--r--   0        0        0     7236 2024-05-13 10:01:30.845481 antakia_core-0.4.5/src/antakia_core/compute/dim_reduction/dim_reduc_method.py
+-rw-r--r--   0        0        0     7926 2024-04-25 14:03:01.843934 antakia_core-0.4.5/src/antakia_core/compute/dim_reduction/dim_reduction.py
+-rw-r--r--   0        0        0       75 2024-03-22 17:21:14.615326 antakia_core-0.4.5/src/antakia_core/compute/dim_reduction/pacmap_progress/__init__.py
+-rw-r--r--   0        0        0    40149 2024-03-22 17:21:15.061170 antakia_core-0.4.5/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610898 antakia_core-0.4.5/src/antakia_core/compute/model_subtitution/__init__.py
+-rw-r--r--   0        0        0      840 2024-03-21 16:04:55.999992 antakia_core-0.4.5/src/antakia_core/compute/model_subtitution/classification_models.py
+-rw-r--r--   0        0        0     3733 2024-04-23 14:51:04.769035 antakia_core-0.4.5/src/antakia_core/compute/model_subtitution/model_class.py
+-rw-r--r--   0        0        0     8139 2024-04-23 14:51:04.885872 antakia_core-0.4.5/src/antakia_core/compute/model_subtitution/model_interface.py
+-rw-r--r--   0        0        0     1842 2024-03-19 14:18:22.611366 antakia_core-0.4.5/src/antakia_core/compute/model_subtitution/regression_models.py
+-rw-r--r--   0        0        0     1785 2024-04-23 14:50:36.703592 antakia_core-0.4.5/src/antakia_core/compute/skope_rule/skope_rule.py
+-rw-r--r--   0        0        0      192 2024-03-19 14:18:22.611682 antakia_core-0.4.5/src/antakia_core/data_handler/__init__.py
+-rw-r--r--   0        0        0     3969 2024-04-23 14:51:04.148770 antakia_core-0.4.5/src/antakia_core/data_handler/projected_values.py
+-rw-r--r--   0        0        0       98 2024-03-19 14:18:22.611895 antakia_core-0.4.5/src/antakia_core/data_handler/region.py
+-rw-r--r--   0        0        0     9794 2024-05-13 10:05:59.839054 antakia_core-0.4.5/src/antakia_core/data_handler/region_.py
+-rw-r--r--   0        0        0    10674 2024-04-23 14:50:36.705105 antakia_core-0.4.5/src/antakia_core/data_handler/region_set.py
+-rw-r--r--   0        0        0    10089 2024-04-23 14:50:36.705350 antakia_core-0.4.5/src/antakia_core/data_handler/rule.py
+-rw-r--r--   0        0        0     4434 2024-04-23 14:50:36.706070 antakia_core-0.4.5/src/antakia_core/data_handler/rules.py
+-rw-r--r--   0        0        0      190 2024-03-19 14:18:22.612650 antakia_core-0.4.5/src/antakia_core/explanation/__init__.py
+-rw-r--r--   0        0        0     2129 2024-03-29 12:59:56.497027 antakia_core-0.4.5/src/antakia_core/explanation/explanation_method.py
+-rw-r--r--   0        0        0     4778 2024-04-23 09:45:08.541634 antakia_core-0.4.5/src/antakia_core/explanation/explanations.py
+-rw-r--r--   0        0        0      307 2024-03-19 14:18:22.612977 antakia_core-0.4.5/src/antakia_core/utils/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-23 14:51:04.685563 antakia_core-0.4.5/src/antakia_core/utils/correlation_coef.py
+-rw-r--r--   0        0        0     1302 2024-03-29 13:06:13.987832 antakia_core-0.4.5/src/antakia_core/utils/long_task.py
+-rw-r--r--   0        0        0      561 2024-04-23 14:51:04.692721 antakia_core-0.4.5/src/antakia_core/utils/splittable_callback.py
+-rw-r--r--   0        0        0     4576 2024-04-23 09:45:08.541955 antakia_core-0.4.5/src/antakia_core/utils/utils.py
+-rw-r--r--   0        0        0    12510 2024-04-23 09:45:08.542559 antakia_core-0.4.5/src/antakia_core/utils/variable.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 antakia_core-0.4.5/PKG-INFO
```

### Comparing `antakia_core-0.4.4/LICENSE` & `antakia_core-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/pyproject.toml` & `antakia_core-0.4.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antakia-core"
-version = "0.4.4"
+version = "0.4.5"
 description = "Core modules for AntakIA"
 authors = ["Pierre Hulot <pierre@ai-vidence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 pandas = "^2.2.0"
```

### Comparing `antakia_core-0.4.4/src/antakia_core/compute/dim_reduction/dim_reduc_method.py` & `antakia_core-0.4.5/src/antakia_core/compute/dim_reduction/dim_reduc_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,20 +136,20 @@
         if fit_sample_num is None or fit_sample_num > self.X.shape[0]:
             fit_sample_num = self.X.shape[0]
         self.publish_progress(0)
         kwargs['n_components'] = self.get_dimension()
         param = self.default_parameters.copy()
         param.update(kwargs)
         dim_red_model = self.dimreduc_model(**param)
-        if hasattr(dim_red_model, 'fit'):
-            fitted_model = dim_red_model.fit(self.X.sample(n=fit_sample_num))
+        if hasattr(dim_red_model, 'fit_transform'):
+            X_red = dim_red_model.fit_transform(self.X)
+        elif hasattr(dim_red_model, 'fit'):
+            fitted_model = dim_red_model.fit(self.X)
             if hasattr(fitted_model, 'transform'):
                 X_red = fitted_model.transform(self.X)
-        elif hasattr(dim_red_model, 'fit_transform'):
-            X_red = dim_red_model.fit_transform(self.X)
         else:
             raise AttributeError(
                 "No fit method implemented for dimensionality reduction method"
             )
         X_red = pd.DataFrame(X_red)
         self.publish_progress(100)
         return X_red
```

### Comparing `antakia_core-0.4.4/src/antakia_core/compute/dim_reduction/dim_reduction.py` & `antakia_core-0.4.5/src/antakia_core/compute/dim_reduction/dim_reduction.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py` & `antakia_core-0.4.5/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/compute/model_subtitution/classification_models.py` & `antakia_core-0.4.5/src/antakia_core/compute/model_subtitution/classification_models.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/compute/model_subtitution/model_class.py` & `antakia_core-0.4.5/src/antakia_core/compute/model_subtitution/model_class.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/compute/model_subtitution/model_interface.py` & `antakia_core-0.4.5/src/antakia_core/compute/model_subtitution/model_interface.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/compute/model_subtitution/regression_models.py` & `antakia_core-0.4.5/src/antakia_core/compute/model_subtitution/regression_models.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/compute/skope_rule/skope_rule.py` & `antakia_core-0.4.5/src/antakia_core/compute/skope_rule/skope_rule.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/data_handler/projected_values.py` & `antakia_core-0.4.5/src/antakia_core/data_handler/projected_values.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/data_handler/region_.py` & `antakia_core-0.4.5/src/antakia_core/data_handler/region_.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/data_handler/region_set.py` & `antakia_core-0.4.5/src/antakia_core/data_handler/region_set.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/data_handler/rule.py` & `antakia_core-0.4.5/src/antakia_core/data_handler/rule.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/data_handler/rules.py` & `antakia_core-0.4.5/src/antakia_core/data_handler/rules.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/explanation/explanation_method.py` & `antakia_core-0.4.5/src/antakia_core/explanation/explanation_method.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/explanation/explanations.py` & `antakia_core-0.4.5/src/antakia_core/explanation/explanations.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/utils/correlation_coef.py` & `antakia_core-0.4.5/src/antakia_core/utils/correlation_coef.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/utils/long_task.py` & `antakia_core-0.4.5/src/antakia_core/utils/long_task.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/utils/splittable_callback.py` & `antakia_core-0.4.5/src/antakia_core/utils/splittable_callback.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/utils/utils.py` & `antakia_core-0.4.5/src/antakia_core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/src/antakia_core/utils/variable.py` & `antakia_core-0.4.5/src/antakia_core/utils/variable.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.4.4/PKG-INFO` & `antakia_core-0.4.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antakia-core
-Version: 0.4.4
+Version: 0.4.5
 Summary: Core modules for AntakIA
 Author: Pierre Hulot
 Author-email: pierre@ai-vidence.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

