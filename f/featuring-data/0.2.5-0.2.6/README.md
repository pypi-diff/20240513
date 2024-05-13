# Comparing `tmp/featuring_data-0.2.5.tar.gz` & `tmp/featuring_data-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featuring_data-0.2.5.tar", last modified: Thu May  2 19:57:20 2024, max compression
+gzip compressed data, was "featuring_data-0.2.6.tar", last modified: Mon May 13 03:10:55 2024, max compression
```

## Comparing `featuring_data-0.2.5.tar` & `featuring_data-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 19:57:20.084800 featuring_data-0.2.5/
--rw-r--r--   0 dancapellupo   (501) staff       (20)     1079 2024-02-15 19:01:48.000000 featuring_data-0.2.5/LICENSE
--rw-r--r--   0 dancapellupo   (501) staff       (20)     8655 2024-05-02 19:57:20.084567 featuring_data-0.2.5/PKG-INFO
--rw-r--r--   0 dancapellupo   (501) staff       (20)     7788 2024-05-02 13:39:18.000000 featuring_data-0.2.5/README.md
--rw-r--r--   0 dancapellupo   (501) staff       (20)      865 2024-05-02 19:54:50.000000 featuring_data-0.2.5/pyproject.toml
--rw-r--r--   0 dancapellupo   (501) staff       (20)       38 2024-05-02 19:57:20.084850 featuring_data-0.2.5/setup.cfg
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 19:57:20.077135 featuring_data-0.2.5/src/
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 19:57:20.084306 featuring_data-0.2.5/src/featuring_data.egg-info/
--rw-r--r--   0 dancapellupo   (501) staff       (20)     8655 2024-05-02 19:57:20.000000 featuring_data-0.2.5/src/featuring_data.egg-info/PKG-INFO
--rw-r--r--   0 dancapellupo   (501) staff       (20)      824 2024-05-02 19:57:20.000000 featuring_data-0.2.5/src/featuring_data.egg-info/SOURCES.txt
--rw-r--r--   0 dancapellupo   (501) staff       (20)        1 2024-05-02 19:57:20.000000 featuring_data-0.2.5/src/featuring_data.egg-info/dependency_links.txt
--rw-r--r--   0 dancapellupo   (501) staff       (20)      135 2024-05-02 19:57:20.000000 featuring_data-0.2.5/src/featuring_data.egg-info/requires.txt
--rw-r--r--   0 dancapellupo   (501) staff       (20)       14 2024-05-02 19:57:20.000000 featuring_data-0.2.5/src/featuring_data.egg-info/top_level.txt
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 19:57:20.078589 featuring_data-0.2.5/src/featuringdata/
--rw-r--r--   0 dancapellupo   (501) staff       (20)        0 2024-02-19 19:41:13.000000 featuring_data-0.2.5/src/featuringdata/__init__.py
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 19:57:20.080744 featuring_data-0.2.5/src/featuringdata/featureSelector/
--rw-r--r--   0 dancapellupo   (501) staff       (20)       79 2024-03-26 00:18:12.000000 featuring_data-0.2.5/src/featuringdata/featureSelector/__init__.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)      819 2024-03-15 01:12:03.000000 featuring_data-0.2.5/src/featuringdata/featureSelector/_create_pdf_report.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    25391 2024-04-26 03:01:02.000000 featuring_data-0.2.5/src/featuringdata/featureSelector/_features_select.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)     4018 2024-03-18 02:12:33.000000 featuring_data-0.2.5/src/featuringdata/featureSelector/_generate_plots.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    13670 2024-04-19 04:06:25.000000 featuring_data-0.2.5/src/featuringdata/featureSelector/_recursive_fit.py
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-02 19:57:20.083849 featuring_data-0.2.5/src/featuringdata/featuresEDA/
--rw-r--r--   0 dancapellupo   (501) staff       (20)       68 2024-02-19 23:39:34.000000 featuring_data-0.2.5/src/featuringdata/featuresEDA/__init__.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    17018 2024-04-26 21:01:09.000000 featuring_data-0.2.5/src/featuringdata/featuresEDA/_correlation.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    21188 2024-04-26 21:05:20.000000 featuring_data-0.2.5/src/featuringdata/featuresEDA/_create_pdf_report.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    22295 2024-04-28 02:43:24.000000 featuring_data-0.2.5/src/featuringdata/featuresEDA/_features_eda.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)    13544 2024-05-02 17:42:10.000000 featuring_data-0.2.5/src/featuringdata/featuresEDA/_generate_plots.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)     6793 2024-04-22 02:30:06.000000 featuring_data-0.2.5/src/featuringdata/featuresEDA/_initial_eda_functions.py
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-13 03:10:55.045459 featuring_data-0.2.6/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     1079 2024-02-15 19:01:48.000000 featuring_data-0.2.6/LICENSE
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    12106 2024-05-13 03:10:55.045235 featuring_data-0.2.6/PKG-INFO
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    11239 2024-05-13 02:21:39.000000 featuring_data-0.2.6/README.md
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      865 2024-05-13 03:10:25.000000 featuring_data-0.2.6/pyproject.toml
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       38 2024-05-13 03:10:55.047028 featuring_data-0.2.6/setup.cfg
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-13 03:10:55.038678 featuring_data-0.2.6/src/
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-13 03:10:55.044809 featuring_data-0.2.6/src/featuring_data.egg-info/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    12106 2024-05-13 03:10:55.000000 featuring_data-0.2.6/src/featuring_data.egg-info/PKG-INFO
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      824 2024-05-13 03:10:55.000000 featuring_data-0.2.6/src/featuring_data.egg-info/SOURCES.txt
+-rw-r--r--   0 dancapellupo   (501) staff       (20)        1 2024-05-13 03:10:55.000000 featuring_data-0.2.6/src/featuring_data.egg-info/dependency_links.txt
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      135 2024-05-13 03:10:55.000000 featuring_data-0.2.6/src/featuring_data.egg-info/requires.txt
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       14 2024-05-13 03:10:55.000000 featuring_data-0.2.6/src/featuring_data.egg-info/top_level.txt
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-13 03:10:55.040176 featuring_data-0.2.6/src/featuringdata/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)        0 2024-02-19 19:41:13.000000 featuring_data-0.2.6/src/featuringdata/__init__.py
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-13 03:10:55.041717 featuring_data-0.2.6/src/featuringdata/featureSelector/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       79 2024-03-26 00:18:12.000000 featuring_data-0.2.6/src/featuringdata/featureSelector/__init__.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      934 2024-05-08 22:32:57.000000 featuring_data-0.2.6/src/featuringdata/featureSelector/_create_pdf_report.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    30353 2024-05-09 01:54:02.000000 featuring_data-0.2.6/src/featuringdata/featureSelector/_features_select.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     4488 2024-05-08 15:32:51.000000 featuring_data-0.2.6/src/featuringdata/featureSelector/_generate_plots.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    14569 2024-05-09 03:03:21.000000 featuring_data-0.2.6/src/featuringdata/featureSelector/_recursive_fit.py
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-05-13 03:10:55.044198 featuring_data-0.2.6/src/featuringdata/featuresEDA/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       68 2024-02-19 23:39:34.000000 featuring_data-0.2.6/src/featuringdata/featuresEDA/__init__.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    17018 2024-04-26 21:01:09.000000 featuring_data-0.2.6/src/featuringdata/featuresEDA/_correlation.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    21188 2024-04-26 21:05:20.000000 featuring_data-0.2.6/src/featuringdata/featuresEDA/_create_pdf_report.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    22424 2024-05-09 17:45:05.000000 featuring_data-0.2.6/src/featuringdata/featuresEDA/_features_eda.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    14919 2024-05-09 18:11:39.000000 featuring_data-0.2.6/src/featuringdata/featuresEDA/_generate_plots.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     6793 2024-04-22 02:30:06.000000 featuring_data-0.2.6/src/featuringdata/featuresEDA/_initial_eda_functions.py
```

### Comparing `featuring_data-0.2.5/LICENSE` & `featuring_data-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `featuring_data-0.2.5/PKG-INFO` & `featuring_data-0.2.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,79 @@
-Metadata-Version: 2.1
-Name: featuring-data
-Version: 0.2.5
-Summary: This package is designed to help anyone with a new dataset get started with EDA quickly.
-Author-email: "Daniel M. Capellupo" <daniel@dmcdatascience.com>
-Project-URL: Homepage, https://github.com/dancapellupo/featuring-data
-Project-URL: Issues, https://github.com/dancapellupo/featuring-data/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.22.0
-Requires-Dist: pandas>=1.4.0
-Requires-Dist: matplotlib>=3.6.0
-Requires-Dist: seaborn>=0.13.0
-Requires-Dist: scipy>=1.7.3
-Requires-Dist: scikit-learn>=1.0.2
-Requires-Dist: xgboost>=1.6.0
-Requires-Dist: fpdf>=1.7.2
-Requires-Dist: tqdm>=4.40.0
 
+<img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/featuring-data-logo-md.png"><br>
+
+-------------------------------------------------------------------------------
 
 # Featuring Data: Exploratory Data Analysis (EDA) and Feature Selection
 
+[![PyPI Version](https://img.shields.io/pypi/v/featuring-data
+)](https://pypi.org/project/featuring-data/)
+
 Featuring Data is a Python library that builds on the well-known Pandas,
 matplotlib, and scikit-learn libraries to provide an easy starting point for
 EDA and feature selection on any structured dataset that is in the form of a
 Pandas dataframe.
 
 The two main parts of this library are the `FeaturesEDA` and the
 `FeatureSelector` classes. Both classes provide easy options to create EDA
 plots and a full PDF report in two lines of code.
 
 ## Installation and Dependencies
 
-The Featuring Data library requires Python 3+, numpy , Pandas , matplotlib ,
-seaborn, and scikit-learn.
+The Featuring Data library requires Python>=3.8, numpy, pandas, matplotlib,
+seaborn, scikit-learn, and xgboost.
 
 The latest stable release (and required dependencies) can be installed from
 PyPI:
 
-[code here]
+```
+pip install featuring-data
+```
+
+## Why Install this Package?
+
+How many times do you have a new dataset - maybe someone sends you a new
+Excel or CSV file - and you just want to do a quick EDA and get a quick
+sense of the dataset before proceeding?
+
+Do you find that your Jupyter notebook gets very long and very messy, very
+quickly, when going through the different columns of a pandas dataframe,
+creating plots, identifying how many unique values a particular column has,
+etc.?
+
+This package allows you to do this fast, so you quickly have a strong
+starting point for further exploration.
+
+Plus, you get
+[a nicely formatted PDF](https://github.com/dancapellupo/featuring-data/blob/4b57e045df68efe75b4a3b9116a32dfd2cd7ef59/examples/Housing_Ames_EDA_Report_20240512_220339.pdf),
+with all the usual, important details of a dataset layed out, for future
+reference as you continue to work with a dataset.
+
+Another bonus is that in creating this package, I have carefully researched
+different methods and metrics. So, you won't be getting just the usual
+Pearson correlation metrics or standard scatterplots.
+
+Beyond EDA, there is a function to aid in feature selection. Going beyond
+some of the usual feature selection techniques, this function performs an
+iterative xgboost training, starting with all features and removing the
+least "important" feature one-by-one. A nicely formatted PDF with different
+plots helps visualize what is going on during the training and can help
+uncover which features are driving the results.
+
+## Get Started Quickly
+
+After installing the package, open
+[this Jupyter notebook](https://github.com/dancapellupo/featuring-data/blob/6efc4b54c65f8a2f38b498a01f569ad25bf2eb23/examples/featuring_data_regression_example.ipynb)
+for a regression example or
+[this Jupyter notebook](https://github.com/dancapellupo/featuring-data/blob/6efc4b54c65f8a2f38b498a01f569ad25bf2eb23/examples/featuring_data_classification_example.ipynb)
+for a classification example, and run with the provided dataset (or read in
+your own CSV or pandas dataframe).
+
+[This PDF](https://github.com/dancapellupo/featuring-data/blob/4b57e045df68efe75b4a3b9116a32dfd2cd7ef59/examples/Housing_Ames_EDA_Report_20240512_220339.pdf)
+shows an example output of the `FeaturesEDA` functionality.
 
 ## FeaturesEDA: A comprehensive EDA in two lines of code
 
 This class implements Exploratory Data Analysis (EDA) on an input dataset.
 
 ```python
 eda = FeaturesEDA(report_prefix='Housing_Ames', target_col="SalePrice", cols_to_drop=["Id"])
@@ -57,15 +85,15 @@
 report is generated and saved in your current working directory - for easy
 reference or sharing results with team members and even stakeholders.
 
 ```python
 eda.master_columns_df.head(5)
 ```
 
-![Housing Ames 'master_columns_df' dataframe](/tmp/housing_ames_master_columns_df_head5.png)
+<img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/housing_ames_master_columns_df_head5.png" alt="Housing Ames 'master_columns_df' dataframe"><br>
 *This is a truncated example of the main dataframe output of the EDA class,
 showing each column from the training dataset in the left-most column (the
 index of this dataframe), the number of Nulls in that column, the type of data
 in that column, the number of unique values, and information about correlation
 between each column of the dataset and the target column.*
 
 The functions within this class perform the following tasks:
@@ -109,20 +137,23 @@
     features.
 - EDA Plots
   - For every feature, a plot of that feature versus the target variable
     is generated.
   - The code automatically selects the type of plot based on the number
     of unique values of that feature. For up to 10 unique values in a
     numeric feature, and for all categorical features, a box plot with a
-    swarm plot is generated. If there are more than 1,000 data points,
-    then only a random selection of 1,000 points are plotted on the
-    swarm plot (but the box plot is calculated based on all points).
-  - For typical numeric features, a standard scatter plot is generated.
+    scatter density plot (the points are artificially spread for visual
+    purposes) overplotted is generated.
+  - For typical numeric features, a scatter density plot is generated. A color
+    scale indicates how many overlapping points there are in a given location.
+
+|   |   |
+|---|---|
+| <img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/housing_ames_GrLivArea_vs_SalePrice.png" alt="Example visualization of continuous variable."> | <img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/housing_ames_ExterQual_vs_SalePrice.png" alt="Example visualization of discrete variable."> |
 
-![Example visualizations of continuous and discrete variables](/tmp/housing_ames_example_feature_plots.png)
 *An example plot of a numeric/continuous variable versus a continuous target
 (left; the sale price of a house in Ames), and a discrete/categorical variable
 versus the same continuous target (right).*
 
 ## FeatureSelector: Feature selection by recursive model training
 
 This class implements an iterative machine learning model training
@@ -163,12 +194,24 @@
         random splits of the data.
     - The following information is kept from every iteration:
         - the feature importance values of every feature at every iteration
         - performance metrics on both the training and validation set
         - the number of features
         - the features removed at the end of each iteration
 
-![](/tmp/housing_ames_num_features_vs_MAE.png)
+<img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/housing_ames_num_features_vs_MAE.png" width=500><br>
 *This plot shows that as the number of features is reduced, the model
-performance stay fairly constant, until you go down to about 20 features
+performance stays fairly constant, until you go down to about 20 features
 (out of ~100 original features). The two colors represent two different
 train/validation data splits.*
+
+## Credits
+
+[1] Inspiration for the density scatterplots comes primarily from this
+[StackOverflow post](https://stackoverflow.com/a/64105308).
+
+[2] The example data set for regression comes from this
+[Kaggle competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data).
+
+[3] The example data set for classification comes from this
+[Kaggle competition](https://www.kaggle.com/competitions/titanic/data).
+
```

### Comparing `featuring_data-0.2.5/pyproject.toml` & `featuring_data-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "featuring-data"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
     { name="Daniel M. Capellupo", email="daniel@dmcdatascience.com" },
 ]
 description = "This package is designed to help anyone with a new dataset get started with EDA quickly."
 readme = "README.md"
 dependencies = [
   "numpy>=1.22.0",
```

### Comparing `featuring_data-0.2.5/src/featuring_data.egg-info/PKG-INFO` & `featuring_data-0.2.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featuring-data
-Version: 0.2.5
+Version: 0.2.6
 Summary: This package is designed to help anyone with a new dataset get started with EDA quickly.
 Author-email: "Daniel M. Capellupo" <daniel@dmcdatascience.com>
 Project-URL: Homepage, https://github.com/dancapellupo/featuring-data
 Project-URL: Issues, https://github.com/dancapellupo/featuring-data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,34 +18,85 @@
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: scikit-learn>=1.0.2
 Requires-Dist: xgboost>=1.6.0
 Requires-Dist: fpdf>=1.7.2
 Requires-Dist: tqdm>=4.40.0
 
 
+<img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/featuring-data-logo-md.png"><br>
+
+-------------------------------------------------------------------------------
+
 # Featuring Data: Exploratory Data Analysis (EDA) and Feature Selection
 
+[![PyPI Version](https://img.shields.io/pypi/v/featuring-data
+)](https://pypi.org/project/featuring-data/)
+
 Featuring Data is a Python library that builds on the well-known Pandas,
 matplotlib, and scikit-learn libraries to provide an easy starting point for
 EDA and feature selection on any structured dataset that is in the form of a
 Pandas dataframe.
 
 The two main parts of this library are the `FeaturesEDA` and the
 `FeatureSelector` classes. Both classes provide easy options to create EDA
 plots and a full PDF report in two lines of code.
 
 ## Installation and Dependencies
 
-The Featuring Data library requires Python 3+, numpy , Pandas , matplotlib ,
-seaborn, and scikit-learn.
+The Featuring Data library requires Python>=3.8, numpy, pandas, matplotlib,
+seaborn, scikit-learn, and xgboost.
 
 The latest stable release (and required dependencies) can be installed from
 PyPI:
 
-[code here]
+```
+pip install featuring-data
+```
+
+## Why Install this Package?
+
+How many times do you have a new dataset - maybe someone sends you a new
+Excel or CSV file - and you just want to do a quick EDA and get a quick
+sense of the dataset before proceeding?
+
+Do you find that your Jupyter notebook gets very long and very messy, very
+quickly, when going through the different columns of a pandas dataframe,
+creating plots, identifying how many unique values a particular column has,
+etc.?
+
+This package allows you to do this fast, so you quickly have a strong
+starting point for further exploration.
+
+Plus, you get
+[a nicely formatted PDF](https://github.com/dancapellupo/featuring-data/blob/4b57e045df68efe75b4a3b9116a32dfd2cd7ef59/examples/Housing_Ames_EDA_Report_20240512_220339.pdf),
+with all the usual, important details of a dataset layed out, for future
+reference as you continue to work with a dataset.
+
+Another bonus is that in creating this package, I have carefully researched
+different methods and metrics. So, you won't be getting just the usual
+Pearson correlation metrics or standard scatterplots.
+
+Beyond EDA, there is a function to aid in feature selection. Going beyond
+some of the usual feature selection techniques, this function performs an
+iterative xgboost training, starting with all features and removing the
+least "important" feature one-by-one. A nicely formatted PDF with different
+plots helps visualize what is going on during the training and can help
+uncover which features are driving the results.
+
+## Get Started Quickly
+
+After installing the package, open
+[this Jupyter notebook](https://github.com/dancapellupo/featuring-data/blob/6efc4b54c65f8a2f38b498a01f569ad25bf2eb23/examples/featuring_data_regression_example.ipynb)
+for a regression example or
+[this Jupyter notebook](https://github.com/dancapellupo/featuring-data/blob/6efc4b54c65f8a2f38b498a01f569ad25bf2eb23/examples/featuring_data_classification_example.ipynb)
+for a classification example, and run with the provided dataset (or read in
+your own CSV or pandas dataframe).
+
+[This PDF](https://github.com/dancapellupo/featuring-data/blob/4b57e045df68efe75b4a3b9116a32dfd2cd7ef59/examples/Housing_Ames_EDA_Report_20240512_220339.pdf)
+shows an example output of the `FeaturesEDA` functionality.
 
 ## FeaturesEDA: A comprehensive EDA in two lines of code
 
 This class implements Exploratory Data Analysis (EDA) on an input dataset.
 
 ```python
 eda = FeaturesEDA(report_prefix='Housing_Ames', target_col="SalePrice", cols_to_drop=["Id"])
@@ -57,15 +108,15 @@
 report is generated and saved in your current working directory - for easy
 reference or sharing results with team members and even stakeholders.
 
 ```python
 eda.master_columns_df.head(5)
 ```
 
-![Housing Ames 'master_columns_df' dataframe](/tmp/housing_ames_master_columns_df_head5.png)
+<img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/housing_ames_master_columns_df_head5.png" alt="Housing Ames 'master_columns_df' dataframe"><br>
 *This is a truncated example of the main dataframe output of the EDA class,
 showing each column from the training dataset in the left-most column (the
 index of this dataframe), the number of Nulls in that column, the type of data
 in that column, the number of unique values, and information about correlation
 between each column of the dataset and the target column.*
 
 The functions within this class perform the following tasks:
@@ -109,20 +160,23 @@
     features.
 - EDA Plots
   - For every feature, a plot of that feature versus the target variable
     is generated.
   - The code automatically selects the type of plot based on the number
     of unique values of that feature. For up to 10 unique values in a
     numeric feature, and for all categorical features, a box plot with a
-    swarm plot is generated. If there are more than 1,000 data points,
-    then only a random selection of 1,000 points are plotted on the
-    swarm plot (but the box plot is calculated based on all points).
-  - For typical numeric features, a standard scatter plot is generated.
+    scatter density plot (the points are artificially spread for visual
+    purposes) overplotted is generated.
+  - For typical numeric features, a scatter density plot is generated. A color
+    scale indicates how many overlapping points there are in a given location.
+
+|   |   |
+|---|---|
+| <img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/housing_ames_GrLivArea_vs_SalePrice.png" alt="Example visualization of continuous variable."> | <img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/housing_ames_ExterQual_vs_SalePrice.png" alt="Example visualization of discrete variable."> |
 
-![Example visualizations of continuous and discrete variables](/tmp/housing_ames_example_feature_plots.png)
 *An example plot of a numeric/continuous variable versus a continuous target
 (left; the sale price of a house in Ames), and a discrete/categorical variable
 versus the same continuous target (right).*
 
 ## FeatureSelector: Feature selection by recursive model training
 
 This class implements an iterative machine learning model training
@@ -163,12 +217,24 @@
         random splits of the data.
     - The following information is kept from every iteration:
         - the feature importance values of every feature at every iteration
         - performance metrics on both the training and validation set
         - the number of features
         - the features removed at the end of each iteration
 
-![](/tmp/housing_ames_num_features_vs_MAE.png)
+<img src="https://raw.githubusercontent.com/dancapellupo/featuring-data/main/tmp/housing_ames_num_features_vs_MAE.png" width=500><br>
 *This plot shows that as the number of features is reduced, the model
-performance stay fairly constant, until you go down to about 20 features
+performance stays fairly constant, until you go down to about 20 features
 (out of ~100 original features). The two colors represent two different
 train/validation data splits.*
+
+## Credits
+
+[1] Inspiration for the density scatterplots comes primarily from this
+[StackOverflow post](https://stackoverflow.com/a/64105308).
+
+[2] The example data set for regression comes from this
+[Kaggle competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data).
+
+[3] The example data set for classification comes from this
+[Kaggle competition](https://www.kaggle.com/competitions/titanic/data).
+
```

### Comparing `featuring_data-0.2.5/src/featuring_data.egg-info/SOURCES.txt` & `featuring_data-0.2.6/src/featuring_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featuring_data-0.2.5/src/featuringdata/featureSelector/_create_pdf_report.py` & `featuring_data-0.2.6/src/featuringdata/featureSelector/_create_pdf_report.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 
 def initialize_pdf_doc():
     pdf = FPDF()
 
     pdf.add_page()
     pdf.set_font('Arial', 'B', 16)
     pdf.cell(w=0, h=10, txt="Feature Selection with Recursive Model Training", ln=1)
-    pdf.ln(2)
+    pdf.ln(6)
 
     return pdf
 
 
-def add_text_pdf(pdf, txt, bold=False, fontsize=12):
-    style = 'B' if bold else ''
+def add_text_pdf(pdf, txt, style='', fontsize=12, new_page=False, space_below=7):
+
+    if new_page:
+        pdf.add_page()
+
+    # style = 'B' if bold else ''
     pdf.set_font('Arial', style, fontsize)
 
     pdf.write(5, txt)
 
-    pdf.ln(7)
-
+    if space_below > 0:
+        pdf.ln(space_below)
+    
     return pdf
 
 
 def add_plot_pdf(pdf, file_path, new_page=True):
 
     if new_page:
         pdf.add_page()
```

### Comparing `featuring_data-0.2.5/src/featuringdata/featureSelector/_features_select.py` & `featuring_data-0.2.6/src/featuringdata/featureSelector/_features_select.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from ._create_pdf_report import (
     initialize_pdf_doc,
     add_text_pdf,
     add_plot_pdf,
     save_pdf_doc
 )
 
-from ._recursive_fit import recursive_fit, calc_model_metric
+from ._recursive_fit import recursive_fit, calc_model_metric, get_metric_names, round_to_n_sigfig
 
-from ._generate_plots import plot_inline_scatter, plot_xy, plot_horizontal_line, plot_vertical_line, save_fig, plot_xy_splitaxis
+from ._generate_plots import plot_inline_scatter, plot_xy, convert_title_to_filename, plot_horizontal_line, plot_vertical_line, save_fig, plot_xy_splitaxis
 
 
 class FeatureSelector:
     """
     This class implements an iterative machine learning model training
     (currently using the xgboost algorithm) to help with feature selection and
     understanding the importance of the input features.
@@ -260,20 +260,22 @@
         training_results_df, self.hyperparams_df, self.feature_importance_dict_list = recursive_fit(
             X_train_comb, y_train_comb, X_test_comb, y_test_comb, target_log=self.target_log,
             target_type=self.target_type, parameter_dict=self.parameter_dict)
 
         # --------------------------------------------------------------------
         # Identify Best Results
 
+        primary_metric, secondary_metric = get_metric_names(target_type=self.target_type)
+
         # TODO: Identify best run based on metric out to certain number [3?] of decimal points
-        best_result_ind_1 = np.argmin(training_results_df["RMSE_test_1"].values)
-        best_result_ind_2 = np.argmin(training_results_df["RMSE_test_2"].values)
+        best_result_ind_1 = np.argmin(training_results_df[f"{primary_metric}_test_1"].values)
+        best_result_ind_2 = np.argmin(training_results_df[f"{primary_metric}_test_2"].values)
 
-        best_result_1 = training_results_df["RMSE_test_1"].values[best_result_ind_1]
-        best_result_2 = training_results_df["RMSE_test_2"].values[best_result_ind_2]
+        best_result_1 = training_results_df[f"{primary_metric}_test_1"].values[best_result_ind_1]
+        best_result_2 = training_results_df[f"{primary_metric}_test_2"].values[best_result_ind_2]
 
         print('Best results: (1) {} [{}], (2) {} [{}]\n'.format(
             best_result_1, best_result_ind_1, best_result_2, best_result_ind_2))
 
         if best_result_1 < best_result_2:
             data_ind = 0
             best_ind = best_result_ind_1
@@ -301,84 +303,148 @@
         else:
             xgb_reg = XGBClassifier(n_estimators=1000, early_stopping_rounds=20, random_state=42, **hyperparams_dict)
         xgb_reg.fit(X_train_best, y_train_comb[data_ind], eval_set=[(X_test_best, y_test_comb[data_ind])], verbose=True)
 
         y_test_pred = xgb_reg.predict(X_test_best)
         
         if self.target_log:
-            mae_final = calc_model_metric(np.expm1(y_test_comb[data_ind]), np.expm1(y_test_pred),
+            sec_metric_final = calc_model_metric(np.expm1(y_test_comb[data_ind]), np.expm1(y_test_pred),
                                           target_type=self.target_type, metric_type='easy')
         else:
-            mae_final = calc_model_metric(y_test_comb[data_ind], y_test_pred, target_type=self.target_type,
+            sec_metric_final = calc_model_metric(y_test_comb[data_ind], y_test_pred, target_type=self.target_type,
                                           metric_type='easy')
-        print('\nFinal MAE: {}\n'.format(mae_final))
+        print(f'\nFinal {secondary_metric}: {sec_metric_final:.3f}\n')
 
         # --------------------
         # Save results to CSV:
         training_results_df.to_csv('{}_training_results_full_{}.csv'.format(self.report_prefix, timestamp))
         self.hyperparams_df.to_csv('{}_best_hyperparameters_{}.csv'.format(self.report_prefix, timestamp))
 
         # --------------------------------------------------------------------
         # Generating PDF Document and Plots:
         self.pdf = initialize_pdf_doc()
 
         # --------------------------------------------------------------------
-        # PLOT #1 - Plot of model metric vs iteration
+        # PLOTS #1 and #2 - Plot of model metric vs iteration
 
         # First look for large gaps along x-axis:
         num_features_start = training_results_df["num_features_{}".format(data_ind+1)].iloc[0]
         gap_loc = np.where(
             np.diff(training_results_df["num_features_{}".format(data_ind+1)].values)[0:5] < -0.2*num_features_start)[0]
         start_ii = gap_loc[-1] + 1 if gap_loc.size > 0 else 0
 
-        # Creat the plot:
-        f, ax = plot_inline_scatter(training_results_df.iloc[start_ii:], x_col="num_features_{}".format(1),
-                                    y_col="MAE_test_{}".format(1), outfile=False)
-        best_mae = training_results_df["MAE_test_{}".format(data_ind+1)].iloc[best_ind]
-        plot_inline_scatter(training_results_df.iloc[start_ii:], f=f, ax=ax, x_col="num_features_{}".format(2),
-                                    y_col="MAE_test_{}".format(2), xlabel='Number of Features in Iteration',
-                                    ylabel='Mean Average Error (MAE) for Val Set',
-                                    hline=best_mae,
-                                    vline=training_results_df["num_features_{}".format(data_ind+1)].iloc[best_ind],
-                                    overplot=True, outfile=True, plots_folder=plots_folder, title='num_features_vs_MAE')
-        # ax = plot_horizontal_line(ax, y_loc=best_mae)
-        # ax = plot_vertical_line(ax, x_loc=training_results_df["num_features_{}".format(data_ind+1)].iloc[best_ind])
-        # save_fig(f, ax, plots_folder=plots_folder, title='num_features_vs_MAE')
+        # ---
+        # PLOT #1 - Primary metric used in xgboost training:
 
-        # plot_xy_splitaxis(x=training_results_df["num_features_1"].values, y=training_results_df["MAE_test_1"].values,
-        #                   plots_folder=plots_folder, title='num_features_vs_MAE')
+        # Create the plots:
+        f, ax = plot_inline_scatter(training_results_df.iloc[start_ii:], x_col=f"num_features_{1}",
+                                    y_col=f"{primary_metric}_test_{1}", leg_label=f'Data Split {1}', outfile=False)
+        best_prim_metric = training_results_df[f"{primary_metric}_test_{data_ind+1}"].iloc[best_ind]
+        if primary_metric == 'RMSE':
+            ylabel = 'RMSE for Val Set'
+        else:
+            ylabel = 'Logloss for Val Set'
+        plot_inline_scatter(training_results_df.iloc[start_ii:], f=f, ax=ax, x_col=f"num_features_{2}",
+                            y_col=f"{primary_metric}_test_{2}", leg_label=f'Data Split {2}',
+                            xlabel='Number of Features in Iteration', ylabel=ylabel, hline=best_prim_metric,
+                            vline=training_results_df[f"num_features_{data_ind+1}"].iloc[best_ind],
+                            reverse_x=True, overplot=True, outfile=True, plots_folder=plots_folder,
+                            title=f'num_features_vs_{primary_metric}')
 
         # Add plot and informative text to PDF:
-        self.pdf = add_text_pdf(self.pdf, txt="Recursive Training Results", bold=True)
-        self.pdf = add_plot_pdf(self.pdf, file_path=plots_folder+'/num_features_vs_MAE'+'.png', new_page=False)
+        self.pdf = add_text_pdf(self.pdf, txt="Recursive Training Results", style='B', space_below=10)
+        self.pdf = add_plot_pdf(self.pdf, file_path=plots_folder+f'/num_features_vs_{primary_metric}'+'.png',
+                                new_page=False)
         if start_ii > 0:
-            out_txt = ("Note: The point from the first iteration with {} features and an MAE of {} was removed from "
-                       "this plot.").format(num_features_start,
-                                            training_results_df["MAE_test_{}".format(data_ind+1)].iloc[0])
+            out_txt = (f"Note: The point from the first iteration with {num_features_start} features and a "
+                       f"{primary_metric} of {training_results_df[f'{primary_metric}_test_{data_ind+1}'].iloc[0]} was "
+                       f"removed from this plot.")
             self.pdf = add_text_pdf(self.pdf, txt=out_txt)
             out_txt = ("Normally, the way this recursive model training works is that it removes the feature with the "
                        "lowest importance at each iteration. However, if there are multiple features that have exactly "
                        "zero importance, then all of those zero importance features are removed at once.")
             self.pdf = add_text_pdf(self.pdf, txt=out_txt)
         out_txt = ("The above plot has our model metric on the y-axis, and the number of features for each model "
                    "training iteration on the x-axis. In other words, each dot here represents an iteration of the "
                    "recursive model training.")
         self.pdf = add_text_pdf(self.pdf, txt=out_txt)
-        out_txt = ("As the number of features is reduced, eventually the model will start to perform much more poorly. "
-                   "The vertical line is the location with the best value of the evaluation metric, which is an MAE of "
-                   "{}), compared to the starting MAE of {}.").format(
-            best_mae, training_results_df["MAE_test_{}".format(data_ind+1)].iloc[0])
-        self.pdf = add_text_pdf(self.pdf, txt=out_txt)
-        out_txt = ("The model training started with {} features (after one-hot encoding any categorical "
-                   "features), and achieved the best model training results with {} features.").format(
-            num_features_start, training_results_df["num_features_{}".format(data_ind+1)].iloc[best_ind])
+        out_txt = "As the number of features is reduced, eventually the model will start to perform much more poorly."
         self.pdf = add_text_pdf(self.pdf, txt=out_txt)
+        # TODO: Put metric values in boldface:
+        out_txt = (f"This plot shows the primary metric that was used in model training, which is {primary_metric}. "
+                   f"The vertical line is the location with the best value of this metric, which is a {primary_metric} "
+                   f"of ")
+        self.pdf = add_text_pdf(self.pdf, txt=out_txt, space_below=0)
+        self.pdf = add_text_pdf(self.pdf, style='B', txt=f"{best_prim_metric}", space_below=0)
+        self.pdf = add_text_pdf(self.pdf, txt=f", compared to the starting {primary_metric} of ", space_below=0)
+        self.pdf = add_text_pdf(self.pdf, style='B', space_below=0,
+                                txt=f"{training_results_df[f'{primary_metric}_test_{data_ind+1}'].iloc[0]}")
+        self.pdf = add_text_pdf(self.pdf, txt=f".")
+        # DONE: Make italic:
+        out_txt = f"Note that lower values of {primary_metric} indicate better model performance."
+        self.pdf = add_text_pdf(self.pdf, style='I', txt=out_txt)
+        out_txt = (f"The model training started with {num_features_start} features (after one-hot encoding any "
+                   f"categorical features), and achieved the best model training results with ")
+        self.pdf = add_text_pdf(self.pdf, txt=out_txt, space_below=0)
+        self.pdf = add_text_pdf(
+            self.pdf, txt=f"{training_results_df['num_features_{}'.format(data_ind+1)].iloc[best_ind]} features",
+            style='B', space_below=0)
+        self.pdf = add_text_pdf(self.pdf, txt=f".")
+        # TODO: Add baseline for logloss - random assignment based on fraction with each label
         # TODO: Assess how low, in terms of number of features, one could go without drastically decreasing the
         #  performance
-        # TODO: Print MAE compared to range of y_val values
+        # TODO: Print MAE compared to range of y_val valuee
+        
+        # ---
+        # PLOT #2 - Secondary evaluation metric:
+
+        if secondary_metric == 'MAE':
+            best_sec_metric_ind = np.argmin(training_results_df[f"{secondary_metric}_test_{data_ind+1}"].values)
+        else:
+            best_sec_metric_ind = np.argmax(training_results_df[f"{secondary_metric}_test_{data_ind+1}"].values)
+        best_sec_metric = training_results_df[f"{secondary_metric}_test_{data_ind+1}"].iloc[best_sec_metric_ind]
+
+        f, ax = plot_inline_scatter(training_results_df.iloc[start_ii:], x_col=f"num_features_{1}",
+                                    y_col=f"{secondary_metric}_test_{1}", leg_label=f'Data Split {1}', outfile=False)
+        if secondary_metric == 'MAE':
+            ylabel = 'Mean Average Error (MAE) for Val Set'
+        else:
+            ylabel = 'Cohen-Kappa for Val Set'
+        plot_inline_scatter(training_results_df.iloc[start_ii:], f=f, ax=ax, x_col=f"num_features_{2}",
+                            y_col=f"{secondary_metric}_test_{2}", leg_label=f'Data Split {2}',
+                            xlabel='Number of Features in Iteration', ylabel=ylabel, hline=best_sec_metric,
+                            vline=training_results_df[f"num_features_{data_ind+1}"].iloc[best_sec_metric_ind],
+                            reverse_x=True, overplot=True, outfile=True, plots_folder=plots_folder,
+                            title=f'num_features_vs_{secondary_metric}')
+        
+        self.pdf = add_plot_pdf(self.pdf, file_path=plots_folder+f'/num_features_vs_{secondary_metric}'+'.png',
+                                new_page=True)
+        out_txt = f"This plot is the same as the previous page, except with the secondary metric, {secondary_metric}."
+        self.pdf = add_text_pdf(self.pdf, txt=out_txt)
+        out_txt = "It is therefore possible that the 'best' iteration will be different in this plot."
+        self.pdf = add_text_pdf(self.pdf, style='I', txt=out_txt)
+        self.pdf = add_text_pdf(self.pdf, txt=f"The best value of {secondary_metric} is ", space_below=0)
+        self.pdf = add_text_pdf(self.pdf, style='B', txt=f"{best_sec_metric:,}", space_below=0)
+        self.pdf = add_text_pdf(self.pdf, txt=f", compared to the starting value of ", space_below=0)
+        self.pdf = add_text_pdf(self.pdf, style='B', space_below=0,
+                                txt=f"{training_results_df[f'{secondary_metric}_test_{data_ind+1}'].iloc[0]:,}")
+        if self.target_type == 'regression':
+            out_txt = f" (the average {self.target_col} is {round_to_n_sigfig(data_df[self.target_col].mean(), 5):,})"
+            self.pdf = add_text_pdf(self.pdf, txt=out_txt, space_below=0)
+        self.pdf = add_text_pdf(self.pdf, txt=f".")
+        if secondary_metric == 'CohKap':
+            out_txt = (f"Note that with the Cohen-Kappa score, the possible range is 0 to 1, with 0 meaning that the "
+                       f"model has no predictive power and 1 is the best it could be.")
+            self.pdf = add_text_pdf(self.pdf, style='I', txt=out_txt)
+        self.pdf = add_text_pdf(
+            self.pdf, txt="With this metric, the best model training result occurred with ", space_below=0)
+        self.pdf = add_text_pdf(
+            self.pdf, txt=f"{training_results_df['num_features_{}'.format(data_ind+1)].iloc[best_ind]} features",
+            style='B', space_below=0)
+        self.pdf = add_text_pdf(self.pdf, txt=f".")
 
         # ----------------------------------------------
         # Collect and examine feature importance values:
         self.feat_import_bycol_df = pd.DataFrame(columns=["max_feat_imp", "best_feat_imp", "num_iters"])
         for col in self.feature_importance_dict_list[data_ind].keys():
             feat_import_vals = self.feature_importance_dict_list[data_ind][col]
             best_feat_imp = feat_import_vals[best_ind] if best_ind < len(feat_import_vals) else np.nan
@@ -387,14 +453,17 @@
         self.feat_import_bycol_df["num_iters"] = self.feat_import_bycol_df["num_iters"].astype(int)
         self.feat_import_bycol_df = self.feat_import_bycol_df.sort_values(by=["max_feat_imp"], ascending=False)
 
         # --------------------------------------------------------------------
         # PLOT #2 - Generate plots showing how the feature importance of the
         #  top features changes depending on the number of total features used
 
+        self.pdf = add_text_pdf(self.pdf, txt="Exploring Feature Importance during Iterative Training", style='B',
+                                new_page=True, space_below=10)
+
         num_features = training_results_df["num_features_{}".format(data_ind+1)].values
         # Set the number of features to show on each plot:
         num_feat_per_plot = 5
         # Set the total number of features to plot:
         tot_feat_to_plot = min(20, len(self.feat_import_bycol_df) - len(self.feat_import_bycol_df) % num_feat_per_plot)
         # Each loop corresponds to one plot:
         for jj in range(0, tot_feat_to_plot, num_feat_per_plot):
@@ -409,53 +478,58 @@
                 x = num_features[start_ii:num_iters]
                 y = self.feature_importance_dict_list[data_ind][col][start_ii:]
 
                 print(jj, jjj, col)
 
                 # If this is the first feature for this plot panel:
                 if jjj == 0:
-                    f, ax = plot_xy(x, y, xlabel='num_features_{}'.format(data_ind+1), ylabel='feature importance',
-                                    leg_label=col, overplot=False, outfile=False)
+                    f, ax = plot_xy(x, y, xlabel='Number of Features (Data Split {})'.format(data_ind+1),
+                                    ylabel='Feature Importance', overplot=False, outfile=False, markersize=5, label=col)
                 elif jjj < num_feat_per_plot-1:
-                    f, ax = plot_xy(x, y, f=f, ax=ax, leg_label=col, overplot=True, outfile=False)
+                    f, ax = plot_xy(x, y, f=f, ax=ax, overplot=True, outfile=False, markersize=5, label=col)
                 # If this is the last feature for this plot panel, save the
                 #  plot to disk:
                 else:
-                    plot_xy(x, y, f=f, ax=ax, leg_label=col, overplot=True, outfile=True, plots_folder=plots_folder,
-                            title='feature_importance_vs_number_features_{}'.format(jj))
+                    plot_xy(x, y, f=f, ax=ax, overplot=True, outfile=True, plots_folder=plots_folder, reverse_x=True,
+                            title='feature_importance_vs_number_features_{}'.format(jj), markersize=5, label=col)
 
             # Create a new PDF page for every 2 plots:
-            new_page = True if (jj % 2) == 0 else False
+            new_page = True if (jj != 0) and ((jj % 2) == 0) else False
             self.pdf = add_plot_pdf(
                 self.pdf, file_path=plots_folder+'/feature_importance_vs_number_features_{}'.format(jj)+'.png',
                 new_page=new_page)
 
         # --------------------------------------------------------------------
         # PLOT #3 - Generate plot of feature importance versus correlation
         #  with target variable
 
         cols_best_iter = self.feat_import_bycol_df.dropna().index
         # This plot can only be generated if a dataframe with feature
         #  correlations is passed to the function:
         if master_columns_df is not None:
+            self.pdf = add_text_pdf(
+                self.pdf, txt="Exploring Feature Importance Compared to Individual Feature Correlations", style='B',
+                new_page=True, space_below=10)
+            plot_title = 'Target Correlation vs Feature Importance'
+
             # Get a list of features that are both numeric and are part of the
             #  "best" training iteration:
             numeric_df = master_columns_df.loc[master_columns_df["Column Type"] == 'numeric']
             if len(numeric_df) > 0:
                 numeric_best_feat = set(cols_best_iter).intersection(set(numeric_df.index))
                 print('Number of numeric features in best iteration: {}'.format(len(numeric_best_feat)))
 
                 x, y = [], []
                 for feat in numeric_best_feat:
                     x.append(numeric_df.loc[feat, "Random Forest"])
                     y.append(self.feat_import_bycol_df.loc[feat, "best_feat_imp"])
 
                 f, ax = plot_xy(x, y, xlabel='RF Correlation between Feature and Target', ylabel='Feature Importance',
-                                leg_label='Numeric Feature', overplot=False, outfile=False, plots_folder=plots_folder,
-                                title='target_correlation_vs_feature_importance')
+                                overplot=False, outfile=False, plots_folder=plots_folder, title=plot_title,
+                                markersize=5, label='Numeric Feature')
 
             non_numeric_df = master_columns_df.loc[master_columns_df["Column Type"] == 'non-numeric']
             if len(non_numeric_df) > 0:
                 feat_import_bycol_df_best = self.feat_import_bycol_df.dropna()
                 # non_numeric_best_feat = set(cols_best_iter).difference()
 
                 x, y = [], []
@@ -471,19 +545,19 @@
                         feat_df = feat_import_bycol_df_best.loc[
                             feat_import_bycol_df_best.index.str.startswith(feat + '_')]
                         if len(feat_df) > 0:
                             x.append(non_numeric_df.loc[feat, "RF_norm"])
                             y.append(feat_df["best_feat_imp"].sum())
 
                 print('Number of non-numeric features in best iteration: {}'.format(len(y)))
-                plot_xy(x, y, f=f, ax=ax, leg_label='Non-Numeric Feature', overplot=True, outfile=True,
-                        plots_folder=plots_folder, title='target_correlation_vs_feature_importance')
-
-            self.pdf = add_plot_pdf(self.pdf, file_path=plots_folder+'/target_correlation_vs_feature_importance'+'.png',
-                                    new_page=True)
+                plot_xy(x, y, f=f, ax=ax, overplot=True, outfile=True, plots_folder=plots_folder, title=plot_title,
+                        markersize=5, label='Non-Numeric Feature')
+            
+            self.pdf = add_plot_pdf(self.pdf, file_path=plots_folder+'/'+convert_title_to_filename(plot_title)+'.png',
+                                    new_page=False)
 
         # Save PDF document to current working directory
         save_pdf_doc(self.pdf, custom_filename=self.report_prefix, timestamp=timestamp)
 
         return training_results_df
 
     def rerun_plots(self):
```

### Comparing `featuring_data-0.2.5/src/featuringdata/featureSelector/_generate_plots.py` & `featuring_data-0.2.6/src/featuringdata/featureSelector/_generate_plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 
+def convert_title_to_filename(title):
+    return title.lower().replace(' ', '_')
+
+
 def plot_inline_scatter(data_df, x_col, y_col, f=None, ax=None, xlabel=None, ylabel=None, title='', overplot=False,
-                        hline=None, vline=None, outfile=True, plots_folder='./'):
+                        leg_label='', hline=None, vline=None, reverse_x=False, outfile=True, plots_folder='./'):
 
     if not overplot:
-        sns.set_theme(style="whitegrid")
+        sns.set_theme(style="ticks", font_scale=1.2)
         f, ax = plt.subplots(figsize=(9, 6))
         ax.set_title(title)
 
-    sns.scatterplot(data_df, x=x_col, y=y_col, size=3, legend=False)
+    # sns.scatterplot(data_df, x=x_col, y=y_col, size=3, legend=False)
+    plt.plot(data_df[x_col], data_df[y_col], 'o', markersize=6, label=leg_label)
 
     if xlabel is not None:
         plt.xlabel(xlabel)
     if ylabel is not None:
         plt.ylabel(ylabel)
 
     if (hline is not None) or (vline is not None):
@@ -24,47 +29,54 @@
 
         if hline is not None:
             ax.hlines(hline, xmin, xmax, color='black', linestyles=':')
 
         if vline is not None:
             ax.vlines(vline, ymin, ymax, color='black', linestyles=':')
 
-        ax.set_xlim(xmin, xmax)
+        ax.set_xlim(xmax, xmin) if reverse_x else ax.set_xlim(xmin, xmax)
         ax.set_ylim(ymin, ymax)
 
     if outfile:
+        if leg_label != '':
+            plt.legend()
+        plt.grid()
         plt.savefig('{}/{}.png'.format(plots_folder, title), bbox_inches='tight')
         # *** Close for now ***
         # plt.close(f)
     else:
         return f, ax
 
 
-def plot_xy(x, y, f=None, ax=None, xlabel=None, ylabel=None, leg_label='', title='', overplot=False, outfile=True,
-            plots_folder='./'):
+def plot_xy(x, y, f=None, ax=None, xlabel=None, ylabel=None, title='', reverse_x=False, overplot=False, outfile=True,
+            plots_folder='./', **kwargs):
 
     if not overplot:
-        sns.set_theme(style="whitegrid")
+        sns.set_theme(style="ticks", font_scale=1.1)
         f, ax = plt.subplots(figsize=(9, 6))
         ax.set_title(title)
 
     # sns.lineplot(x=x, y=y, size=3, legend='auto')
     # sns.scatterplot(x=x, y=y, size=3, label=leg_label)
-    plt.plot(x, y, 'o', markersize=3, label=leg_label)
+    plt.plot(x, y, 'o', **kwargs)
 
     if xlabel is not None:
         plt.xlabel(xlabel)
     if ylabel is not None:
         plt.ylabel(ylabel)
 
     plt.legend()
 
     if outfile:
-        # TODO Take title, lowercase and replace spaces with underscores
-        plt.savefig('{}/{}.png'.format(plots_folder, title), bbox_inches='tight')
+        if reverse_x:
+            xmin, xmax = ax.get_xlim()
+            ax.set_xlim(xmax, xmin)
+        plt.grid()
+        # DONE Take title, lowercase and replace spaces with underscores
+        plt.savefig('{}/{}.png'.format(plots_folder, convert_title_to_filename(title)), bbox_inches='tight')
         plt.close(f)
     else:
         return f, ax
 
 
 def plot_horizontal_line(ax, y_loc):
     ax.hlines(y_loc, 0, 1, transform=ax.get_yaxis_transform(), color='black', linestyles=':')
```

### Comparing `featuring_data-0.2.5/src/featuringdata/featureSelector/_recursive_fit.py` & `featuring_data-0.2.6/src/featuringdata/featureSelector/_recursive_fit.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,25 @@
     log_loss,
     cohen_kappa_score,
 )
 
 from xgboost.sklearn import XGBRegressor, XGBClassifier
 
 
+def get_metric_names(target_type='regression'):
+    if target_type == 'regression':
+        primary_metric = 'RMSE'
+        secondary_metric = 'MAE'
+    else:
+        primary_metric = 'logloss'
+        secondary_metric = 'CohKap'
+
+    return primary_metric, secondary_metric
+
+
 def round_to_n_sigfig(x, n=3):
     """
     Round a number to 'n' significant digits.
 
     Parameters
     ----------
     x : int or float
@@ -141,17 +152,18 @@
     feature_columns.append(feature_columns_full.copy())
     feature_columns.append(feature_columns_full.copy())
 
     num_columns_orig = len(feature_columns_full)
     print('Starting number of feature columns: {}\n'.format(num_columns_orig))
 
     # Set-up training results dataframe:
-    training_results_cols_prefix = ["RMSE_train_", "RMSE_test_", "MAE_test_", "num_features_", "feature_list_",
-                                    "feat_high_import_name_", "feat_high_import_val_",
-                                    "features_to_remove_"]
+    primary_metric, secondary_metric = get_metric_names(target_type)
+    training_results_cols_prefix = [
+        f"{primary_metric}_train_", f"{primary_metric}_test_", f"{secondary_metric}_test_", "num_features_",
+        "feature_list_", "feat_high_import_name_", "feat_high_import_val_", "features_to_remove_"]
     training_results_cols = []
     for ii in range(1, len(X_train_comb)+1):
         training_results_cols.extend([x + str(ii) for x in training_results_cols_prefix])
     training_results_df = pd.DataFrame(columns=training_results_cols)
 
     # Set-up dataframe to store results of hyperparameter search:
     hyperparams_list = list(parameter_dict.keys())
@@ -298,17 +310,25 @@
                 col_to_drop = feature_columns[data_jj][min_feat_import_ind]
                 feature_columns[data_jj].remove(col_to_drop)
 
             # Save to dataframe the name(s) of the dropped column(s):
             out_row.append(col_to_drop)
 
         training_results_df.loc[jj] = out_row
-        print('Iter', jj, training_results_df.loc[jj, "num_features_1"], training_results_df.loc[jj, "RMSE_test_1"],
-              training_results_df.loc[jj, "feat_high_import_name_1"],
-              training_results_df.loc[jj, "feat_high_import_val_1"])
+        if jj == 0:
+            print(f'         NumFeats(1) {primary_metric}(1)   TopFeat(1) TopFeatImp(1)'
+                  f'  NumFeats(2) {primary_metric}(2)   TopFeat(2) TopFeatImp(2)')
+        print(f'Iter {jj:4} : {training_results_df.loc[jj, "num_features_1"]:5}  '
+              f'{training_results_df.loc[jj, f"{primary_metric}_test_1"]:.5f} '
+              f'{training_results_df.loc[jj, "feat_high_import_name_1"]:>20} '
+              f'{training_results_df.loc[jj, "feat_high_import_val_1"]:.2f}  :  '
+              f'{training_results_df.loc[jj, "num_features_2"]:5} '
+              f'{training_results_df.loc[jj, f"{primary_metric}_test_2"]:.5f}  '
+              f'{training_results_df.loc[jj, "feat_high_import_name_2"]:>20} '
+              f'{training_results_df.loc[jj, "feat_high_import_val_2"]:.2f}')
 
         # Stop running the iterative training once all features have been
         #  removed from at least one of the data splits:
         if len(feature_columns[0]) == 0 or len(feature_columns[1]) == 0:
             break
 
     print()
```

### Comparing `featuring_data-0.2.5/src/featuringdata/featuresEDA/_correlation.py` & `featuring_data-0.2.6/src/featuringdata/featuresEDA/_correlation.py`

 * *Files identical despite different names*

### Comparing `featuring_data-0.2.5/src/featuringdata/featuresEDA/_create_pdf_report.py` & `featuring_data-0.2.6/src/featuringdata/featuresEDA/_create_pdf_report.py`

 * *Files identical despite different names*

### Comparing `featuring_data-0.2.5/src/featuringdata/featuresEDA/_features_eda.py` & `featuring_data-0.2.6/src/featuringdata/featuresEDA/_features_eda.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         self.target_col = target_col
         self.cols_to_drop = cols_to_drop
         self.numeric_uniq_vals_thresh = numeric_uniq_vals_thresh
         self.nonnumeric_uniq_vals_thresh = nonnumeric_uniq_vals_thresh
 
         self.pdf = None
         self.null_count_by_row_series = None
-        # TODO: Combine unique values and corr info into one DF
+        self.master_columns_df = pd.DataFrame()
         self.numeric_cols = None
         self.non_numeric_cols = None
         self.numeric_collinear_df = pd.DataFrame()
 
     def run_initial_eda(self, data_df, output=True):
         """
         Run an initial exploratory data analysis (EDA) on a given dataset.
@@ -291,15 +291,15 @@
                                                 target_num_uniq)
 
         # Save PDF document to current working directory:
         if output:
             custom_filename = self.report_prefix + '_Initial'
             save_pdf_doc(self.pdf, custom_filename=custom_filename, timestamp=timestamp)
 
-    def run_full_eda(self, data_df, run_collinear=True, generate_plots=True):
+    def run_full_eda(self, data_df, run_collinear=True, generate_plots=True, plot_style='scatterdense'):
         """
         Run a comprehensive exploratory data analysis (EDA) on a given dataset.
 
         This function runs the following steps:
         - The initial EDA -- see "run_initial_eda"
         - Feature correlations analysis
         - EDA Plots
@@ -434,15 +434,16 @@
                 columns_list_ordered = self.master_columns_df.loc[
                     self.master_columns_df["Column Type"] == 'numeric'].sort_values(
                         by=["Random Forest"], ascending=False).index.to_list()
 
                 # Generate plots of numeric features, and save them to the
                 # timestamped directory defined above:
                 plot_feature_values(data_df, columns_list_ordered, self.master_columns_df, target_col=self.target_col,
-                                    numeric=True, target_type=self.target_type, plots_folder=plots_folder)
+                                    numeric=True, plot_style=plot_style, target_type=self.target_type,
+                                    plots_folder=plots_folder)
 
                 # Add the plots to the PDF:
                 self.pdf = section_of_plots(self.pdf, columns_list_ordered, target_col=self.target_col, numeric=True,
                                             plots_folder=plots_folder)
 
             # ----------------------------------
             # Generate plots of non-numeric features
@@ -453,15 +454,16 @@
                 columns_list_ordered = self.master_columns_df.loc[
                     self.master_columns_df["Column Type"] == 'non-numeric'].sort_values(
                         by=["RF_norm"], ascending=False).index.to_list()
 
                 # Generate plots of non-numeric features, and save them to the
                 # timestamped directory defined above:
                 plot_feature_values(data_df, columns_list_ordered, self.master_columns_df, target_col=self.target_col,
-                                    numeric=False, target_type=self.target_type, plots_folder=plots_folder)
+                                    numeric=False, plot_style=plot_style, target_type=self.target_type,
+                                    plots_folder=plots_folder)
                 
                 # Add the plots to the PDF:
                 self.pdf = section_of_plots(self.pdf, columns_list_ordered, target_col=self.target_col, numeric=False,
                                             plots_folder=plots_folder)
 
         print('\n--- Files Output ---')
         # Save PDF document to current working directory:
```

### Comparing `featuring_data-0.2.5/src/featuringdata/featuresEDA/_generate_plots.py` & `featuring_data-0.2.6/src/featuringdata/featuresEDA/_generate_plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 
-import time
 from tqdm.auto import tqdm
 
+import math
 import numpy as np
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.offsetbox import AnchoredText
 import seaborn as sns
 from scipy.interpolate import interpn
 from scipy.stats import gaussian_kde
+from sklearn.preprocessing import MinMaxScaler
 
 
 def plot_ecdf(data_col, data_label='', xlabel='Data Values', filename='ecdf', overplot=False, outfile=True,
               plots_folder='./'):
 
     if not overplot:
         sns.set_theme(style="whitegrid")
@@ -90,27 +91,30 @@
         xy = np.vstack([x, y])
         z = gaussian_kde(xy)(xy)
 
     # Sort the points by density, so that the densest points are plotted last
     if sort:
         idx = z.argsort()
         x, y, z = x[idx], y[idx], z[idx]
-
+    
+    # z = MinMaxScaler(feature_range=(0, 1)).fit_transform(z.reshape(-1, 1))
+    z /= 10**(math.floor(math.log10(abs(z.max()))))
+    
     plt.scatter(x, y, c=z, **kwargs)
     plt.colorbar()
 
     # norm = mpl.colors.Normalize(vmin=np.min(z), vmax=np.max(z))
     # cbar = fig.colorbar(mpl.cm.ScalarMappable(norm=norm), ax=ax, cmap='viridis')
     # cbar.ax.set_ylabel('Density')
 
     return ax
 
 
 def plot_feature_values(data_df, columns_list, correlation_df, target_col, numeric=True, target_type='regression',
-                        catplot_style='scatterdense', plots_folder='./plots'):
+                        plot_style='scatterdense', plots_folder='./plots'):
     """
     Generate EDA plots that show each feature versus the target variable.
 
     The code automatically adjusts based on certain properties of the feature:
     - For categorical features, as well as numeric features with up to 10
       unique values, a box plot with a swarm plot is generated. If there are
       more than 1,000 data points, then only a random selection of 1,000
@@ -135,14 +139,17 @@
         '_correlation.calc_nonnumeric_features_target_corr'.
 
     target_col : str
 
     numeric : bool
 
     catplot_style : str
+        The options are:
+        - 'scatterdense' for density scatterplots with the matplotlib viridis color palette
+        - 'swarm' or 'strip' for default seaborn colors and style
 
     plots_folder : str
 
     Returns
     -------
     r2 : float
         The theoretical maximum R^2 for the given number of unique values.
@@ -150,15 +157,15 @@
 
     # backend_ = mpl.get_backend()
     # print('*** {} ***'.format(backend_))
     # mpl.use("Agg")
     # print('*** {} ***'.format(mpl.get_backend()))
 
     # Set box plot display parameters:
-    if catplot_style != 'scatterdense':
+    if plot_style != 'scatterdense':
         box_params = {'whis': [0, 100], 'width': 0.6}
     else:
         box_params = {'whis': [0, 100], 'width': 0.6, 'fill': False, 'color': 'black'}
 
     set_ylim = False
     if target_type == 'regression':
         # Check for strong outliers in target column:
@@ -210,24 +217,24 @@
                     sns.boxplot(data_df_col_notnull, x=column, y=target_col, order=xaxis_order, **box_params)
 
                 else:
                     # Standard Box Plot
                     sns.boxplot(data_df_col_notnull, x=column, y=target_col, **box_params)  # hue="method", palette="vlag"
 
                 # Add in points to show each observation
-                if (catplot_style != 'scatterdense') and (len(data_df_col_notnull) > 1000):
+                if (plot_style != 'scatterdense') and (len(data_df_col_notnull) > 1000):
                     data_df_col_notnull = data_df_col_notnull.sample(n=1000, replace=False)
 
-                if catplot_style == 'swarm':
+                if plot_style in ('swarm', 'seaborn'):
                     sns.swarmplot(data_df_col_notnull, x=column, y=target_col, size=2, color=".3", warn_thresh=0.4)
 
-                elif catplot_style == 'strip':
+                elif plot_style == 'strip':
                     sns.stripplot(data_df_col_notnull, x=column, y=target_col, jitter=0.25, size=2, color=".3")
 
-                elif catplot_style == 'scatterdense':
+                elif plot_style == 'scatterdense':
                     x_all, y_all = np.array([]), np.array([])
 
                     for cat in ax.get_xticklabels():
                         # print(cat, cat.get_text(), cat.get_position(), cat.get_position()[0])
 
                         try:
                             data_df_cat = data_df_col_notnull.loc[
@@ -240,15 +247,21 @@
                             np.random.normal(scale=0.06, size=len(data_df_cat)))  # 0.005
                         y = data_df_cat[target_col].values
                         x_all, y_all = np.append(x_all, x), np.append(y_all, y)
 
                     ax = plot_scatter_density(x_all, y_all, fig=f, ax=ax, bins=100, s=3, cmap='viridis')
                 
             else:
-                sns.histplot(data_df_col_notnull, x=column, hue=target_col, discrete=True, shrink=0.6, multiple="dodge")  # "stack"
+                if plot_style == 'seaborn':
+                    sns.histplot(data_df_col_notnull, x=column, hue=target_col, discrete=True, shrink=0.6,
+                                 multiple="dodge")  # "stack"
+                else:
+                    with sns.color_palette('viridis'):
+                        sns.histplot(data_df_col_notnull, x=column, hue=target_col, discrete=True, shrink=0.6,
+                                     multiple="dodge")  # "stack"
                 ax.set_xticks(data_df_col_notnull[column].unique())
 
             if (not numeric) and num_uniq >= 10:
                 plt.xticks(rotation=45)
                 plt.grid(axis='x')
 
             plt.grid(axis='y')
@@ -263,49 +276,60 @@
             if xx.size > 0:
                 data_df_col_notnull = data_df_col_notnull.drop(xx)
 
                 anc = AnchoredText('Not Shown: {} Outliers'.format(xx.size), loc="upper left", frameon=False)
                 ax.add_artist(anc)
 
             if target_type == 'regression':
-                # sns.scatterplot(train_data_mod, x=column, y=target_col, hue="OverallQual")
-                # sns.scatterplot(data_df, x=column, y=target_col, size=2, legend=False)
+                if plot_style == 'seaborn':
+                    sns.scatterplot(data_df_col_notnull, x=column, y=target_col, size=2, legend=False)
 
-                ax = plot_scatter_density(data_df_col_notnull[column].values, data_df_col_notnull[target_col].values,
-                                        fig=f, ax=ax, bins=100, s=3, cmap='viridis')
+                else:
+                    ax = plot_scatter_density(data_df_col_notnull[column].values, data_df_col_notnull[target_col].values,
+                                            fig=f, ax=ax, bins=100, s=3, cmap='viridis')
 
-                # plt.hist2d(data_df_col_notnull[column], data_df_col_notnull[target_col], bins=(100, 100),
-                #            cmap='viridis', cmin=1)  # BuPu
-                # plt.colorbar()
+                    # plt.hist2d(data_df_col_notnull[column], data_df_col_notnull[target_col], bins=(100, 100),
+                    #            cmap='viridis', cmin=1)  # BuPu
+                    # plt.colorbar()
 
-                # ax.scatter(x, y, c=z, s=100, edgecolor='')
-                # ax.scatter(x, y, c=z, s=50)
+                    # ax.scatter(x, y, c=z, s=100, edgecolor='')
+                    # ax.scatter(x, y, c=z, s=50)
             
             else:
                 sns.boxplot(data_df_col_notnull, x=column, y=target_col, orient='y', **box_params)
 
-                x_all, y_all = np.array([]), np.array([])
+                if (plot_style != 'scatterdense') and (len(data_df_col_notnull) > 1000):
+                    data_df_col_notnull = data_df_col_notnull.sample(n=1000, replace=False)
+
+                if plot_style in ('swarm', 'seaborn'):
+                    sns.swarmplot(data_df_col_notnull, x=column, y=target_col, orient='y', size=2, color=".3", warn_thresh=0.4)
+
+                elif plot_style == 'strip':
+                    sns.stripplot(data_df_col_notnull, x=column, y=target_col, orient='y', jitter=0.25, size=2, color=".3")
+                
+                elif plot_style == 'scatterdense':
+                    x_all, y_all = np.array([]), np.array([])
+
+                    for cat in ax.get_yticklabels():
+                        # print(cat, cat.get_text(), cat.get_position(), cat.get_position()[0])
 
-                for cat in ax.get_yticklabels():
-                    # print(cat, cat.get_text(), cat.get_position(), cat.get_position()[0])
+                        try:
+                            data_df_cat = data_df_col_notnull.loc[
+                                (data_df_col_notnull[target_col] == cat.get_text()) | (
+                                            data_df_col_notnull[target_col] == float(cat.get_text()))]
+                        except ValueError:
+                            data_df_cat = data_df_col_notnull.loc[data_df_col_notnull[target_col] == cat.get_text()]
+                        # print(len(data_df_cat))
 
-                    try:
-                        data_df_cat = data_df_col_notnull.loc[
-                            (data_df_col_notnull[target_col] == cat.get_text()) | (
-                                        data_df_col_notnull[target_col] == float(cat.get_text()))]
-                    except ValueError:
-                        data_df_cat = data_df_col_notnull.loc[data_df_col_notnull[target_col] == cat.get_text()]
-                    # print(len(data_df_cat))
-
-                    y = (np.zeros(len(data_df_cat)) + cat.get_position()[1] +
-                        np.random.normal(scale=0.06, size=len(data_df_cat)))
-                    x = data_df_cat[column].values
-                    x_all, y_all = np.append(x_all, x), np.append(y_all, y)
+                        y = (np.zeros(len(data_df_cat)) + cat.get_position()[1] +
+                            np.random.normal(scale=0.06, size=len(data_df_cat)))
+                        x = data_df_cat[column].values
+                        x_all, y_all = np.append(x_all, x), np.append(y_all, y)
 
-                ax = plot_scatter_density(x_all, y_all, fig=f, ax=ax, bins=100, s=3, cmap='viridis')
+                    ax = plot_scatter_density(x_all, y_all, fig=f, ax=ax, bins=100, s=3, cmap='viridis')
 
             plt.grid()
 
             plt.xlabel(column)
             plt.ylabel(target_col)
 
         if set_ylim:
```

### Comparing `featuring_data-0.2.5/src/featuringdata/featuresEDA/_initial_eda_functions.py` & `featuring_data-0.2.6/src/featuringdata/featuresEDA/_initial_eda_functions.py`

 * *Files identical despite different names*

