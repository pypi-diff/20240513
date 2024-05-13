# Comparing `tmp/bevfs-1.0.0.tar.gz` & `tmp/bevfs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bevfs-1.0.0.tar", last modified: Mon May 13 20:30:33 2024, max compression
+gzip compressed data, was "dist/bevfs-1.0.1.tar", last modified: Mon May 13 20:59:34 2024, max compression
```

## Comparing `bevfs-1.0.0.tar` & `bevfs-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mohammedbilalshakeel   (503) staff       (20)        0 2024-05-13 20:30:33.850722 bevfs-1.0.0/
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)     2495 2024-05-13 20:30:33.850474 bevfs-1.0.0/PKG-INFO
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)     1791 2024-05-13 18:54:57.000000 bevfs-1.0.0/README.md
-drwxr-xr-x   0 mohammedbilalshakeel   (503) staff       (20)        0 2024-05-13 20:30:33.847733 bevfs-1.0.0/bevfs/
--rwxrwxrwx   0 mohammedbilalshakeel   (503) staff       (20)       34 2024-05-13 20:28:12.000000 bevfs-1.0.0/bevfs/__init__.py
--rwxrwxrwx   0 mohammedbilalshakeel   (503) staff       (20)    37801 2024-05-13 20:28:02.000000 bevfs-1.0.0/bevfs/bevfs.py
-drwxr-xr-x   0 mohammedbilalshakeel   (503) staff       (20)        0 2024-05-13 20:30:33.849371 bevfs-1.0.0/bevfs.egg-info/
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)     2495 2024-05-13 20:30:33.000000 bevfs-1.0.0/bevfs.egg-info/PKG-INFO
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)      208 2024-05-13 20:30:33.000000 bevfs-1.0.0/bevfs.egg-info/SOURCES.txt
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)        1 2024-05-13 20:30:33.000000 bevfs-1.0.0/bevfs.egg-info/dependency_links.txt
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)       49 2024-05-13 20:30:33.000000 bevfs-1.0.0/bevfs.egg-info/requires.txt
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)        6 2024-05-13 20:30:33.000000 bevfs-1.0.0/bevfs.egg-info/top_level.txt
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)       38 2024-05-13 20:30:33.850819 bevfs-1.0.0/setup.cfg
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)      967 2024-05-13 20:29:03.000000 bevfs-1.0.0/setup.py
-drwxr-xr-x   0 mohammedbilalshakeel   (503) staff       (20)        0 2024-05-13 20:30:33.849693 bevfs-1.0.0/test/
--rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)      114 2024-05-13 19:56:12.000000 bevfs-1.0.0/test/test.py
+drwxr-xr-x   0 mohammedbilalshakeel   (503) staff       (20)        0 2024-05-13 20:59:34.556908 bevfs-1.0.1/
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)     2699 2024-05-13 20:59:34.556642 bevfs-1.0.1/PKG-INFO
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)     1947 2024-05-13 20:57:37.000000 bevfs-1.0.1/README.md
+drwxr-xr-x   0 mohammedbilalshakeel   (503) staff       (20)        0 2024-05-13 20:59:34.554618 bevfs-1.0.1/bevfs/
+-rwxrwxrwx   0 mohammedbilalshakeel   (503) staff       (20)       34 2024-05-13 20:28:12.000000 bevfs-1.0.1/bevfs/__init__.py
+-rwxrwxrwx   0 mohammedbilalshakeel   (503) staff       (20)    37799 2024-05-13 20:56:02.000000 bevfs-1.0.1/bevfs/bevfs.py
+drwxr-xr-x   0 mohammedbilalshakeel   (503) staff       (20)        0 2024-05-13 20:59:34.556066 bevfs-1.0.1/bevfs.egg-info/
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)     2699 2024-05-13 20:59:34.000000 bevfs-1.0.1/bevfs.egg-info/PKG-INFO
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)      208 2024-05-13 20:59:34.000000 bevfs-1.0.1/bevfs.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)        1 2024-05-13 20:59:34.000000 bevfs-1.0.1/bevfs.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)       49 2024-05-13 20:59:34.000000 bevfs-1.0.1/bevfs.egg-info/requires.txt
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)        6 2024-05-13 20:59:34.000000 bevfs-1.0.1/bevfs.egg-info/top_level.txt
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)       38 2024-05-13 20:59:34.557424 bevfs-1.0.1/setup.cfg
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)      967 2024-05-13 20:58:53.000000 bevfs-1.0.1/setup.py
+drwxr-xr-x   0 mohammedbilalshakeel   (503) staff       (20)        0 2024-05-13 20:59:34.556306 bevfs-1.0.1/test/
+-rw-r--r--   0 mohammedbilalshakeel   (503) staff       (20)      114 2024-05-13 19:56:12.000000 bevfs-1.0.1/test/test.py
```

### Comparing `bevfs-1.0.0/PKG-INFO` & `bevfs-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: bevfs
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for feature selection in high dimensional data.
 Home-page: https://github.com/Bilal39/Bird-Eye-View/tree/main
 Author: Mohammed Bilal Shakeel
 Author-email: mohammedbilalshakeel@gmail.com
 License: UNKNOWN
 Description: # Bird-Eye-View
-        The Bird's Eye View (BEV) technique is a cutting-edge approach for feature selection, particularly effective in dealing with high-dimensional data. The method's core objective is to identify and eliminate irrelevant features that could hinder machine learning models' accuracy. Removing unimportant features contributes significantly to the models' optimal fit and improve predictive power. The BEV approach has been extensively evaluated against other advanced feature selection methods, with consistently superior results in terms of model accuracy and selected numbers of features. The BEV methodology employs a combination of modern techniques, including evolutionary algorithms, Markov chain, reinforcement learning, and genetic algorithms, that synergistically improve its effectiveness. 
+        The Bird's Eye View (BEV) technique is a cutting-edge approach for feature selection (FS), particularly effective in dealing with high-dimensional data. The method's core objective is to identify and eliminate irrelevant features that could hinder machine learning models' accuracy. Removing unimportant features contributes significantly to the models' optimal fit and improve predictive power. The BEV approach has been extensively evaluated against other advanced feature selection methods, with consistently superior results in terms of model accuracy and selected numbers of features. The BEV methodology employs a combination of modern techniques, including evolutionary algorithms, Markov chain, reinforcement learning, and genetic algorithms, that synergistically improve its effectiveness. 
         
         # Requirements
         The following libraries are required to use the BEV methodology
         * scikit_learn
         * pandas
         * numpy
         * matplotlib
         
-        # Instructions to use BEV
+        # Instructions to use BEVFS
         
-        *	Import bev_algorithm function from bev.
+        *	Import bevfs_algorithm function from bevfs.
         *	Specify the full data file path.
         *	It will start feature selection process.
-        *	Upon completion of the feature selection process, the selected feature files will be automatically saved in the "best features" folder, located in the root directory of the project.
+        *	Upon completion of the feature selection process, the selected feature file will be automatically saved in the "best features" folder, located in the root directory of the project.
         *	The detailed statistics for each selected features file, including the experiment number, stage number, accuracy, and number of features, will be embedded in the data file name.
         
+        # Example
+        from bevfs import bevfs_algorithm
+        
+        bevfs_algorithm("/data.txt") # It should be comma seperated file.
+        
         # Data preparation Guidance
         *	The data must be in CSV format.
+        *	There should be one header row.
         *	The output column should be placed as the first column (i.e., zero index) in the file.
         *	There can be any number of input columns as needed.
         
         It is recommended to perform some basic data exploration and cleaning to ensure the data is accurate, consistent, and free from errors.
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bevfs-1.0.0/README.md` & `bevfs-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 # Bird-Eye-View
-The Bird's Eye View (BEV) technique is a cutting-edge approach for feature selection, particularly effective in dealing with high-dimensional data. The method's core objective is to identify and eliminate irrelevant features that could hinder machine learning models' accuracy. Removing unimportant features contributes significantly to the models' optimal fit and improve predictive power. The BEV approach has been extensively evaluated against other advanced feature selection methods, with consistently superior results in terms of model accuracy and selected numbers of features. The BEV methodology employs a combination of modern techniques, including evolutionary algorithms, Markov chain, reinforcement learning, and genetic algorithms, that synergistically improve its effectiveness. 
+The Bird's Eye View (BEV) technique is a cutting-edge approach for feature selection (FS), particularly effective in dealing with high-dimensional data. The method's core objective is to identify and eliminate irrelevant features that could hinder machine learning models' accuracy. Removing unimportant features contributes significantly to the models' optimal fit and improve predictive power. The BEV approach has been extensively evaluated against other advanced feature selection methods, with consistently superior results in terms of model accuracy and selected numbers of features. The BEV methodology employs a combination of modern techniques, including evolutionary algorithms, Markov chain, reinforcement learning, and genetic algorithms, that synergistically improve its effectiveness. 
 
 # Requirements
 The following libraries are required to use the BEV methodology
 * scikit_learn
 * pandas
 * numpy
 * matplotlib
 
-# Instructions to use BEV
+# Instructions to use BEVFS
 
-*	Import bev_algorithm function from bev.
+*	Import bevfs_algorithm function from bevfs.
 *	Specify the full data file path.
 *	It will start feature selection process.
-*	Upon completion of the feature selection process, the selected feature files will be automatically saved in the "best features" folder, located in the root directory of the project.
+*	Upon completion of the feature selection process, the selected feature file will be automatically saved in the "best features" folder, located in the root directory of the project.
 *	The detailed statistics for each selected features file, including the experiment number, stage number, accuracy, and number of features, will be embedded in the data file name.
 
+# Example
+from bevfs import bevfs_algorithm
+
+bevfs_algorithm("/data.txt") # It should be comma seperated file.
+
 # Data preparation Guidance
 *	The data must be in CSV format.
+*	There should be one header row.
 *	The output column should be placed as the first column (i.e., zero index) in the file.
 *	There can be any number of input columns as needed.
 
 It is recommended to perform some basic data exploration and cleaning to ensure the data is accurate, consistent, and free from errors.
```

### Comparing `bevfs-1.0.0/bevfs/bevfs.py` & `bevfs-1.0.1/bevfs/bevfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,15 +808,15 @@
             print("\nThe Best accuracy in each stage = \n", top_acc_all_stages)
             print("\nSelected features for corresponding best accuracies = \n",
                   number_of_feat_all_stages)
             end_time = time.time()
             elapsed_time = end_time - start_time
 
             print("\nTotal Time in minutes = ", elapsed_time/60)
-            print("\nThe best subset of features have been saved to 'best features' folder = ")
+            print("\nThe best subset of features have been saved to 'best features' folder ")
             print("\n------------------------------------------------------------------------")
             print("------------------------------ E N D -----------------------------------")
             print("------------------------------------------------------------------------")
 
         except IndexError:
             # After every experiment, accuracies and nbr of features are stored in global dictionaries
             top_acc_all_experiments["Experiment_Number_{}".format(
```

### Comparing `bevfs-1.0.0/bevfs.egg-info/PKG-INFO` & `bevfs-1.0.1/bevfs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: bevfs
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for feature selection in high dimensional data.
 Home-page: https://github.com/Bilal39/Bird-Eye-View/tree/main
 Author: Mohammed Bilal Shakeel
 Author-email: mohammedbilalshakeel@gmail.com
 License: UNKNOWN
 Description: # Bird-Eye-View
-        The Bird's Eye View (BEV) technique is a cutting-edge approach for feature selection, particularly effective in dealing with high-dimensional data. The method's core objective is to identify and eliminate irrelevant features that could hinder machine learning models' accuracy. Removing unimportant features contributes significantly to the models' optimal fit and improve predictive power. The BEV approach has been extensively evaluated against other advanced feature selection methods, with consistently superior results in terms of model accuracy and selected numbers of features. The BEV methodology employs a combination of modern techniques, including evolutionary algorithms, Markov chain, reinforcement learning, and genetic algorithms, that synergistically improve its effectiveness. 
+        The Bird's Eye View (BEV) technique is a cutting-edge approach for feature selection (FS), particularly effective in dealing with high-dimensional data. The method's core objective is to identify and eliminate irrelevant features that could hinder machine learning models' accuracy. Removing unimportant features contributes significantly to the models' optimal fit and improve predictive power. The BEV approach has been extensively evaluated against other advanced feature selection methods, with consistently superior results in terms of model accuracy and selected numbers of features. The BEV methodology employs a combination of modern techniques, including evolutionary algorithms, Markov chain, reinforcement learning, and genetic algorithms, that synergistically improve its effectiveness. 
         
         # Requirements
         The following libraries are required to use the BEV methodology
         * scikit_learn
         * pandas
         * numpy
         * matplotlib
         
-        # Instructions to use BEV
+        # Instructions to use BEVFS
         
-        *	Import bev_algorithm function from bev.
+        *	Import bevfs_algorithm function from bevfs.
         *	Specify the full data file path.
         *	It will start feature selection process.
-        *	Upon completion of the feature selection process, the selected feature files will be automatically saved in the "best features" folder, located in the root directory of the project.
+        *	Upon completion of the feature selection process, the selected feature file will be automatically saved in the "best features" folder, located in the root directory of the project.
         *	The detailed statistics for each selected features file, including the experiment number, stage number, accuracy, and number of features, will be embedded in the data file name.
         
+        # Example
+        from bevfs import bevfs_algorithm
+        
+        bevfs_algorithm("/data.txt") # It should be comma seperated file.
+        
         # Data preparation Guidance
         *	The data must be in CSV format.
+        *	There should be one header row.
         *	The output column should be placed as the first column (i.e., zero index) in the file.
         *	There can be any number of input columns as needed.
         
         It is recommended to perform some basic data exploration and cleaning to ensure the data is accurate, consistent, and free from errors.
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bevfs-1.0.0/setup.py` & `bevfs-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='bevfs',
-    version='1.0.0',
+    version='1.0.1',
     author='Mohammed Bilal Shakeel',
     author_email='mohammedbilalshakeel@gmail.com',
     description='A package for feature selection in high dimensional data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Bilal39/Bird-Eye-View/tree/main',
     packages=find_packages(),  # Automatically discover and include all packages
```

