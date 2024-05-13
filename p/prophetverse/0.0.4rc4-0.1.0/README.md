# Comparing `tmp/prophetverse-0.0.4rc4.tar.gz` & `tmp/prophetverse-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophetverse-0.0.4rc4.tar", max compression
+gzip compressed data, was "prophetverse-0.1.0.tar", max compression
```

## Comparing `prophetverse-0.0.4rc4.tar` & `prophetverse-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0    11357 2024-05-10 22:07:53.041764 prophetverse-0.0.4rc4/LICENSE
--rw-r--r--   0        0        0     3328 2024-05-10 22:07:53.041764 prophetverse-0.0.4rc4/README.md
--rw-r--r--   0        0        0      672 2024-05-10 22:08:01.549936 prophetverse-0.0.4rc4/pyproject.toml
--rw-r--r--   0        0        0       61 2024-05-10 22:07:53.057764 prophetverse-0.0.4rc4/src/prophetverse/__init__.py
--rw-r--r--   0        0        0     8336 2024-05-10 22:07:53.057764 prophetverse-0.0.4rc4/src/prophetverse/effects.py
--rw-r--r--   0        0        0     6688 2024-05-10 22:07:53.057764 prophetverse-0.0.4rc4/src/prophetverse/engine.py
--rw-r--r--   0        0        0       59 2024-05-10 22:07:53.057764 prophetverse-0.0.4rc4/src/prophetverse/logger.py
--rw-r--r--   0        0        0     4032 2024-05-10 22:07:53.057764 prophetverse-0.0.4rc4/src/prophetverse/models.py
--rw-r--r--   0        0        0       77 2024-05-10 22:07:53.057764 prophetverse-0.0.4rc4/src/prophetverse/sktime/__init__.py
--rw-r--r--   0        0        0     4701 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/sktime/_expand_column_per_level.py
--rw-r--r--   0        0        0    14213 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/sktime/base.py
--rw-r--r--   0        0        0    15371 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/sktime/multivariate.py
--rw-r--r--   0        0        0     2054 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/sktime/seasonality.py
--rw-r--r--   0        0        0    10052 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/sktime/univariate.py
--rw-r--r--   0        0        0       25 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/trend/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/trend/base.py
--rw-r--r--   0        0        0    16632 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/trend/piecewise.py
--rw-r--r--   0        0        0       77 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/utils/__init__.py
--rw-r--r--   0        0        0     4309 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/utils/frame_to_array.py
--rw-r--r--   0        0        0      988 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/utils/multiindex.py
--rw-r--r--   0        0        0      802 2024-05-10 22:07:53.061764 prophetverse-0.0.4rc4/src/prophetverse/utils/regex.py
--rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 prophetverse-0.0.4rc4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 00:11:34.893268 prophetverse-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4550 2024-05-13 00:11:34.893268 prophetverse-0.1.0/README.md
+-rw-r--r--   0        0        0      669 2024-05-13 00:11:44.161242 prophetverse-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/distributions.py
+-rw-r--r--   0        0        0     8336 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/effects.py
+-rw-r--r--   0        0        0     6688 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/engine.py
+-rw-r--r--   0        0        0       59 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/logger.py
+-rw-r--r--   0        0        0     7009 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/models.py
+-rw-r--r--   0        0        0       72 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/__init__.py
+-rw-r--r--   0        0        0     4701 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/_expand_column_per_level.py
+-rw-r--r--   0        0        0    14213 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/base.py
+-rw-r--r--   0        0        0    15371 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/multivariate.py
+-rw-r--r--   0        0        0     2054 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/seasonality.py
+-rw-r--r--   0        0        0    19480 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/sktime/univariate.py
+-rw-r--r--   0        0        0       25 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/trend/__init__.py
+-rw-r--r--   0        0        0     2863 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/trend/base.py
+-rw-r--r--   0        0        0     1139 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/trend/flat.py
+-rw-r--r--   0        0        0    16632 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/trend/piecewise.py
+-rw-r--r--   0        0        0       77 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/utils/__init__.py
+-rw-r--r--   0        0        0     4309 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/utils/frame_to_array.py
+-rw-r--r--   0        0        0      988 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/utils/multiindex.py
+-rw-r--r--   0        0        0      802 2024-05-13 00:11:34.917268 prophetverse-0.1.0/src/prophetverse/utils/regex.py
+-rw-r--r--   0        0        0     5093 1970-01-01 00:00:00.000000 prophetverse-0.1.0/PKG-INFO
```

### Comparing `prophetverse-0.0.4rc4/LICENSE` & `prophetverse-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/pyproject.toml` & `prophetverse-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prophetverse"
-version = "0.0.4-rc4"
+version = "0.1.0"
 description = ""
 authors = ["Felipe Angelim <felipeangelim@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "prophetverse", from="src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
@@ -21,10 +21,11 @@
 mkdocs = "^1.5.3"
 mkdocstrings-python = "^1.9.0"
 mkdocs-jupyter = "^0.24.6"
 pymdown-extensions = "^10.7.1"
 mkdocs-material = "^9.5.14"
 pytest-cov = "^5.0.0"
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/effects.py` & `prophetverse-0.1.0/src/prophetverse/effects.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/engine.py` & `prophetverse-0.1.0/src/prophetverse/engine.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/sktime/_expand_column_per_level.py` & `prophetverse-0.1.0/src/prophetverse/sktime/_expand_column_per_level.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/sktime/base.py` & `prophetverse-0.1.0/src/prophetverse/sktime/base.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/sktime/multivariate.py` & `prophetverse-0.1.0/src/prophetverse/sktime/multivariate.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/sktime/seasonality.py` & `prophetverse-0.1.0/src/prophetverse/sktime/seasonality.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/trend/base.py` & `prophetverse-0.1.0/src/prophetverse/trend/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,7 +90,11 @@
         """
         
         t_days = convert_index_to_days_since_epoch(idx)
         return (t_days) / self.t_scale - self.t_start
 
     def __call__(self, **kwargs):
         return self.compute_trend(**kwargs)
+
+        
+        
+
```

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/trend/piecewise.py` & `prophetverse-0.1.0/src/prophetverse/trend/piecewise.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/utils/frame_to_array.py` & `prophetverse-0.1.0/src/prophetverse/utils/frame_to_array.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/utils/multiindex.py` & `prophetverse-0.1.0/src/prophetverse/utils/multiindex.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/src/prophetverse/utils/regex.py` & `prophetverse-0.1.0/src/prophetverse/utils/regex.py`

 * *Files identical despite different names*

### Comparing `prophetverse-0.0.4rc4/PKG-INFO` & `prophetverse-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,27 @@
-Metadata-Version: 2.1
-Name: prophetverse
-Version: 0.0.4rc4
-Summary: 
-Author: Felipe Angelim
-Author-email: felipeangelim@gmail.com
-Requires-Python: >=3.9,<3.13
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: numpyro (>=0.13.2)
-Requires-Dist: optax (>=0.2)
-Requires-Dist: sktime (>=0.21)
-Description-Content-Type: text/markdown
-
 # Prophetverse
 
 <p align="center">
 <img src="docs/static/logo-removebg.png" width="200">
 
 </p>
 
 [![PyPI version](https://badge.fury.io/py/prophetverse.svg)](https://badge.fury.io/py/prophetverse)
 [![codecov](https://codecov.io/gh/felipeangelimvieira/prophetverse/graph/badge.svg?token=O37PGJI3ZX)](https://codecov.io/gh/felipeangelimvieira/prophetverse)
 
 
-This library was created to make a numpyro-based Prophet model for timeseries forecasting, allowing the user to provide custom priors for specific groups of exogenous variables. In addition, it offers a multivariate implementation for hierarchical forecasting, with potentially shared coefficients between timeseries. All implementations (hierarchical and univariate) are based on sktime interface.
+This library was created to provide new versions of the Prophet model for timeseries forecasting. Implemented with numpyro, it allows to provide custom priors for specific groups of exogenous variables, and also offers a multivariate implementation for hierarchical forecasting, with potentially shared coefficients between timeseries. All implementations are based on sktime interface.
 
-The idea was not to fully reproduce Prophet, but to provide an extension with some extra features.
 
 ### Features
 
 ✅ Univariate and multivariate forecasting
 
+✅ Gamma-likelihood and Negative Binomial likelihood for count data
+
 ✅ Custom prior distributions for exogenous variables
 
 ✅ Non-linear effects for exogenous variables (one may create custom effects inheriting AbstractEffect class)
 
 ✅ Shared coefficients between timeseries (multi-variate model)
 
 ✅ Sktime interface
@@ -57,34 +41,42 @@
 
 Or with poetry:
 
 ```bash
 poetry add prophetverse
 ```
 
-
 ## Differences between this Prophet and the original one
 
 The main differences with the original Prophet model are:
 
-1. The logistic version of the trend. In the original paper, the logistic growth is:
+### Logistic trend
 
-```math
-trend = \frac{C}{1 + \exp(-k(t - m))}
-```
+In this implementation, the capacity is modeled as a random variable and is assumed to be constant. In the original model, it was necessary to pass the capacity as a hyperparameter, but we often don't know the maximum value. One example is forecasting the number of new users of a product. We may not know surely what the maximum number of new users is, and may be particularly interested in it.
 
-where $C$ is the capacity, $k$ is the growth rate and $m$ is the timeoffset. In this implementation, we implement a similar and equivalent model, but with a different parameterization:
+### Gamma and Negative Binomial likelihoods
 
-```math
-trend = \frac{C}{1 + \exp(-(kt + m'))}
-```
+The original model only supports Gaussian likelihood. This implementation supports Gamma and Negative Binomial likelihoods, which are useful for count data. 
+
+### Custom priors
+
+Users can set different prior distributions for the model parameters and define custom relationships between the exogenous variables and their effects on the mean. For example, one may want to force a positive effect of a variable on the mean, and use a HalfNormal prior for the coefficient and a `prophetverse.effects.LinearEffect` for the effect (see examples for more details).
+
+I believe this is one of the most important features of this library. It opens the door to a lot of applications, such as Marketing Mix Modeling, which has the objective of understanding the effect of different marketing channels on sales. A saturating effect, such as a Hill Function, can be used to model the diminishing returns of a given channel.
+
+### Changepoints
+
+The changepoint interval is used instead of the changepoint number. Motivation: as the time series evolve, a given changepoint number may have different meanings. For example, a changepoint number of 10 may be too much for a series with 100 observations but too little for a series with 1000 observations. The changepoint interval may avoid this problem and avoid the need of tuning this hyperparameter frequently.
+
+### Scaling
+
+The time series is scaled internally as it is in the original model to provide more stable hyperparameters. However, exogenous variables must be scaled by the user. For that, you can use sktime's transformers and pass them to the `feature_transformer` argument of the model. 
+
+### Seasonality
 
-which are equivalent. The priors for those parameters $k$ and $m'$ are chosen in a data driven way, so that they match the maximum and minimum value of the series.
+The Fourier terms for seasonality must be passed as exogenous variables in the `feature_transformer` argument, see [FourierFeatures](https://www.sktime.net/en/stable/api_reference/auto_generated/sktime.transformations.series.fourier.FourierFeatures.html) for a ready-to-use transformer. Also, check the examples in this documentation.
 
-2. The capacity is also modelled as a random variable, and it's assumed constant. The user can pass the capacity prior as a parameter.
-3. One can set different prior distributions for the parameters of the model. The parameters also may be different for different groups of variables, which allows to force positive coefficients for some groups and not for others (with HalfNormal prior, for example).
-4. Changepoint interval is used instead of changepoint number. Motivation: as the timeseries evolve, a given changepoint number may have different meanings. For example, a changepoint number of 10 may be too much for a series with 100 observations, but too little for a series with 1000 observations. The changepoint interval may avoid this problem.
-5. The exogenous variable inputs are not scaled. They should be scaled prior to the model fitting, with sktime transfomers for example.
-6. The fourier terms for seasonality must be passed as exogenous variables in `feature_transformer` argument.
+### Multivariate model
 
-For the hierarchical model, the forecast is done in a bottom-up fashion. All series parameters are infered simultaneously, and a multivariate normal likelihood is used (LKJ prior for the correlation matrix). In the future, forecasts with OLS reconciliation may be implemented.
+For the hierarchical model, the forecast is done in a bottom-up fashion. All series parameters are inferred simultaneously, and a multivariate normal likelihood is used (with LKJ prior for the correlation matrix). In the future, forecasts with OLS reconciliation may be implemented.
 
+This model is also useful if you want to share coefficients of exogenous variables between time series. For example, if you have a dataset with multiple time series of sales of different products, you may want to share the effect of a given marketing channel between them. This is also possible with this implementation.
```

