# Comparing `tmp/gbfs-0.1.1.tar.gz` & `tmp/gbfs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbfs-0.1.1.tar", max compression
+gzip compressed data, was "gbfs-0.2.0.tar", max compression
```

## Comparing `gbfs-0.1.1.tar` & `gbfs-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0     1068 2024-03-19 09:08:51.147748 gbfs-0.1.1/LICENSE
--rw-r--r--   0        0        0     2806 2024-03-19 09:08:51.147748 gbfs-0.1.1/README.md
--rw-r--r--   0        0        0       36 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/__init__.py
--rw-r--r--   0        0        0       25 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/algorithms/__init__.py
--rw-r--r--   0        0        0     5151 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/algorithms/base.py
--rw-r--r--   0        0        0     3174 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/algorithms/gbafs.py
--rw-r--r--   0        0        0        0 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/feature_selection/__init__.py
--rw-r--r--   0        0        0     2476 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/feature_selection/clustering.py
--rw-r--r--   0        0        0     4215 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/feature_selection/feature_space.py
--rw-r--r--   0        0        0      932 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/feature_selection/knee_locator.py
--rw-r--r--   0        0        0     2014 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/feature_selection/mss.py
--rw-r--r--   0        0        0      556 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/models/data_view.py
--rw-r--r--   0        0        0      690 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/models/dim_reducer.py
--rw-r--r--   0        0        0        0 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/utils/__init__.py
--rw-r--r--   0        0        0     5366 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/utils/data_processor.py
--rw-r--r--   0        0        0     1853 2024-03-19 09:08:51.151749 gbfs-0.1.1/gbfs/utils/distance.py
--rw-r--r--   0        0        0     1375 2024-03-19 09:08:51.151749 gbfs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4116 1970-01-01 00:00:00.000000 gbfs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-13 05:54:46.050883 gbfs-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3126 2024-05-13 05:54:46.050883 gbfs-0.2.0/README.md
+-rw-r--r--   0        0        0       98 2024-05-13 05:54:46.050883 gbfs-0.2.0/gbfs/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-13 05:54:46.050883 gbfs-0.2.0/gbfs/algorithms/__init__.py
+-rw-r--r--   0        0        0     4812 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/algorithms/base.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/algorithms/gb_afs/__init__.py
+-rw-r--r--   0        0        0     3531 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/algorithms/gb_afs/gbafs.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/algorithms/gb_bc_fs/__init__.py
+-rw-r--r--   0        0        0     6506 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/algorithms/gb_bc_fs/gbbcfs.py
+-rw-r--r--   0        0        0    19361 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/algorithms/gb_bc_fs/heuristic.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/feature_selection/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/feature_selection/clustering.py
+-rw-r--r--   0        0        0     4376 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/feature_selection/feature_space.py
+-rw-r--r--   0        0        0      932 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/feature_selection/knee_locator.py
+-rw-r--r--   0        0        0     2014 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/feature_selection/mss.py
+-rw-r--r--   0        0        0      556 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/models/data_view.py
+-rw-r--r--   0        0        0      690 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/models/dim_reducer.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/utils/__init__.py
+-rw-r--r--   0        0        0     5169 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/utils/data_processor.py
+-rw-r--r--   0        0        0     1853 2024-05-13 05:54:46.054883 gbfs-0.2.0/gbfs/utils/distance.py
+-rw-r--r--   0        0        0     1392 2024-05-13 05:54:46.054883 gbfs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4474 1970-01-01 00:00:00.000000 gbfs-0.2.0/PKG-INFO
```

### Comparing `gbfs-0.1.1/LICENSE` & `gbfs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gbfs-0.1.1/README.md` & `gbfs-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 ## GB-FS
 
 **gbfs** is a comprehensive repository dedicated to advancing Graph-Based Feature Selection methodologies in machine learning. Our project houses two significant contributions to the field: GB-AFS and GB-BC-FS, each developed to address the intricate challenges of feature selection with graph-based solutions.
 
 [![Downloads](https://static.pepy.tech/badge/gbfs)](https://pepy.tech/project/gbfs) [![Downloads](https://static.pepy.tech/badge/gbfs/month)](https://pepy.tech/project/gbfs)
+[![ci Status](https://github.com/davidlevinwork/gbfs/actions/workflows/ci.yml/badge.svg)](https://github.com/davidlevinwork/gbfs/actions/workflows/ci.yml)
+[![Tests Status](https://github.com/davidlevinwork/gbfs/actions/workflows/tests.yml/badge.svg)](https://github.com/davidlevinwork/gbfs/actions/workflows/tests.yml)
+
 
 ## Table of contents
 - [Our Contributions](#our-contributions)
 - [Installation](#installation)
 - [Usage](#usage)
   - [GB-AFS](#GB-AFS)
     - [Initialization](#Initialization)
```

### Comparing `gbfs-0.1.1/gbfs/algorithms/base.py` & `gbfs-0.2.0/gbfs/algorithms/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from abc import ABC, abstractmethod
 from typing import Optional
 
 import numpy as np
 
 from gbfs.feature_selection.clustering import Clustering
 from gbfs.feature_selection.feature_space import FeatureSpace
 from gbfs.feature_selection.knee_locator import KneesLocator
 from gbfs.models.dim_reducer import DimReducerProtocol
 from gbfs.utils.data_processor import DataProcessor
 
 
-class FeatureSelectorBase:
+class FeatureSelectorBase(ABC):
     """
     Base class for feature selection using dimensionality reduction, separability metrics,
     and clustering to identify the most significant features in a dataset.
 
     The class processes the input dataset, evaluates feature space using the specified
     dimensionality reduction model and separability metric, performs clustering to find
     optimal feature subsets, and uses a knee detection method to select the number of
@@ -35,34 +36,27 @@
         self.dataset_path = dataset_path
         self.label_column = label_column
         self.dim_reducer_model = dim_reducer_model
         self.separability_metric = separability_metric
 
         self.__process_data()
 
+    @abstractmethod
     def select_features(self) -> Optional[list]:
         """
-        Executes the feature selection process by creating the feature space, evaluating clustering,
-        finding the knee point, and finally selecting the features based on the clustering results.
-
-        :return: A list of selected feature indices or None if no features are selected.
+        Abstract method to execute the feature selection process.
         """
-        self._create_feature_space()
-        self._evaluate_clustering()
-        self._find_knee_point()
-        self._find_features()
-
-        return self.selected_features.tolist()
 
     def __process_data(self):
         """
         Processes the input dataset to prepare it for the feature selection process.
         """
         processor = DataProcessor(
-            dataset_path=self.dataset_path, label_column=self.label_column
+            dataset_path=self.dataset_path,
+            label_column=self.label_column,
         )
         self.data = processor.run()
 
     def _create_feature_space(self):
         """
         Creates the feature space using the provided dimensionality reduction model and separability metric.
         """
@@ -109,15 +103,15 @@
         return self._knee_locator.knee
 
     @property
     def norm_knee(self) -> Optional[int]:
         return self._knee_locator.norm_knee
 
     @property
-    def mss_knee(self) -> Optional[float]:
+    def mss(self) -> Optional[float]:
         return self._mss_knee
 
     @property
     def knee_y(self) -> int | float | None:
         return self._knee_locator.knee_y
 
     @property
```

### Comparing `gbfs-0.1.1/gbfs/algorithms/gbafs.py` & `gbfs-0.2.0/gbfs/algorithms/gb_afs/gbafs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from typing import Optional
+
 import matplotlib.pyplot as plt
 import seaborn as sns
 
+from gbfs.algorithms.base import FeatureSelectorBase
 from gbfs.models.dim_reducer import DimReducerProtocol
 
-from .base import FeatureSelectorBase
-
 
 class GBAFS(FeatureSelectorBase):
     """
     Implements the Graph-Based Automatic Feature Selection (GB-AFS algorithm).
 
     GB-AFS is a novel graph-based filter method fpr automatic feature selection for multi-class classification tasks.
     The method determines the minimum combination of features required to sustain prediction performance ; It does not
@@ -33,21 +34,27 @@
         super().__init__(
             dataset_path=dataset_path,
             separability_metric=separability_metric,
             dim_reducer_model=dim_reducer_model,
             label_column=label_column,
         )
 
-    def select_features(self):
+    def select_features(self) -> Optional[list]:
         """
-        Executes the feature selection process inherited from FeatureSelectorBase.
+        Executes the feature selection process by creating the feature space, evaluating clustering,
+        finding the knee point, and finally selecting the features based on the clustering results.
 
-        :return: A list of selected feature indices.
+        :return: A list of selected feature indices or None if no features are selected.
         """
-        return super().select_features()
+        self._create_feature_space()
+        self._evaluate_clustering()
+        self._find_knee_point()
+        self._find_features()
+
+        return self.selected_features.tolist()
 
     def plot_feature_space(self):
         """
         Visualizes the feature space using a scatter plot and highlights the selected features.
 
         Centroids of selected features are marked distinctly to distinguish them from
         the rest of the features in the feature space. The color intensity in the scatter plot
```

### Comparing `gbfs-0.1.1/gbfs/feature_selection/clustering.py` & `gbfs-0.2.0/gbfs/feature_selection/clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import numpy as np
 from sklearn_extra.cluster import KMedoids
+from tqdm import tqdm
 
 from gbfs.feature_selection.mss import calc_mss_value
 from gbfs.models.data_view import DataProps, FeaturesGraph
 
+STAGE_NAME = 'Clustering Evaluation Using MSS'
+
 
 class Clustering:
     """
     The Clustering class is designed to perform clustering on a reduced feature space
     to evaluate the clustering performance using different metrics.
 
     :param data_props: DataProps instance containing the dataset.
@@ -25,15 +28,15 @@
         calculates the MSS (Mean Simplified Silhouette) for each clustering outcome to assess the clustering quality.
 
         :return: A list of dictionaries, each containing the number of clusters ('k'), the MSS value ('mss'),
                  and the KMedoids clustering result ('kmedoids') for that number of clusters. Each KMedoids result
                  includes the cluster labels, indices of the medoids, and the locations of the medoids.
         """
         results = []
-        for k in range(2, self.features_len):
+        for k in tqdm(range(2, self.features_len), desc=STAGE_NAME):
             kmedoids = self._run_kmedoids(
                 data=self.feature_space.reduced_sep_matrix, k=k
             )
             mss = calc_mss_value(
                 space=self.feature_space.reduced_sep_matrix, clustering=kmedoids
             )
             results.append({'k': k, 'mss': mss, 'kmedoids': kmedoids})
```

### Comparing `gbfs-0.1.1/gbfs/feature_selection/feature_space.py` & `gbfs-0.2.0/gbfs/feature_selection/feature_space.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from itertools import combinations
 
 import numpy as np
+from tqdm import tqdm
 
 from gbfs.models.data_view import DataView, FeaturesGraph
 from gbfs.models.dim_reducer import DimReducerProtocol
 from gbfs.utils.distance import get_distance
 
+STAGE_NAME = 'Separability-Based Feature Space'
+
 
 class FeatureSpace:
     """
     The FeatureSpace class is responsible for computing a separability matrix for feature selection.
 
     :param data: DataView instance containing the dataset.
     :param separability_metric: The metric used to compute separability between features.
@@ -51,15 +54,19 @@
         :return: Numpy ndarray representing the separability matrix.
         """
         label_combinations = list(combinations(np.unique(self.data.norm_data.y), 2))
         num_features = len(self.data.data_props.features)
         num_label_combinations = len(label_combinations)
         separation_matrix = np.zeros((num_features, num_label_combinations))
 
-        for i, feature in enumerate(self.data.data_props.features):
+        for i, feature in tqdm(
+            enumerate(self.data.data_props.features),
+            total=num_features,
+            desc=STAGE_NAME,
+        ):
             for j, labels in enumerate(label_combinations):
                 label_1_values = self._extract_feature_values_for_class(
                     feature_name=feature, class_name=labels[0]
                 )
                 label_2_values = self._extract_feature_values_for_class(
                     feature_name=feature, class_name=labels[1]
                 )
```

### Comparing `gbfs-0.1.1/gbfs/feature_selection/knee_locator.py` & `gbfs-0.2.0/gbfs/feature_selection/knee_locator.py`

 * *Files identical despite different names*

### Comparing `gbfs-0.1.1/gbfs/feature_selection/mss.py` & `gbfs-0.2.0/gbfs/feature_selection/mss.py`

 * *Files identical despite different names*

### Comparing `gbfs-0.1.1/gbfs/models/data_view.py` & `gbfs-0.2.0/gbfs/models/data_view.py`

 * *Files identical despite different names*

### Comparing `gbfs-0.1.1/gbfs/models/dim_reducer.py` & `gbfs-0.2.0/gbfs/models/dim_reducer.py`

 * *Files identical despite different names*

### Comparing `gbfs-0.1.1/gbfs/utils/data_processor.py` & `gbfs-0.2.0/gbfs/utils/data_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional
+from typing import Dict
 
 import pandas as pd
 from sklearn.preprocessing import MinMaxScaler
 
 from gbfs.models.data_view import DataCollection, DataProps, DataView
 
 EPSILON = 1e-10
@@ -15,41 +15,42 @@
     and constructs DataView objects that encapsulate the dataset and its properties.
 
     This class is essential for preparing data before applying feature selection, ensuring
     that the data is in a suitable format and scale for analysis.
 
     :param dataset_path: Path to the dataset file (CSV format expected).
     :param label_column: Name of the column in the dataset that serves as the label. Defaults to 'class'.
-    :param cost_column: Optional; name of the column that indicates the cost associated with each feature.
-                        If not provided, all features are assumed to have equal cost.
     """
 
     def __init__(
         self,
         dataset_path: str,
         label_column: str = 'class',
-        cost_column: Optional[str] = None,
     ):
         self.dataset_path = dataset_path
         self.label_column = label_column
-        self.cost_column = cost_column
 
     def run(self) -> DataView:
         """
         Executes the data processing steps: loading the dataset, normalizing the feature values,
         and creating a DataView object containing the processed data along with its properties.
 
         :return: DataView object encapsulating the original and normalized datasets,
                  along with metadata about the dataset's properties.
         """
-        data = pd.read_csv(self.dataset_path)
-        norm_data = self._normalize_data(data)
+        data = pd.read_csv(self.dataset_path, header=0)
+        feature_costs = self._extract_and_remove_costs(data=data)
+        norm_data = self._normalize_data(data=data)
 
-        data_collections = self._create_data_collections(data, norm_data)
-        data_props = self._compute_data_properties(data_collections['original'])
+        data_collections = self._create_data_collections(
+            original_data=data, normalized_data=norm_data
+        )
+        data_props = self._compute_data_properties(
+            data=data_collections['original'], feature_costs=feature_costs
+        )
 
         return DataView(
             data=data_collections['original'],
             norm_data=data_collections['normalized'],
             data_props=data_props,
         )
 
@@ -88,45 +89,46 @@
             'normalized': DataCollection(
                 x=normalized_data.drop(self.label_column, axis=1),
                 y=pd.DataFrame(normalized_data[self.label_column]),
                 x_y=normalized_data,
             ),
         }
 
-    def _compute_data_properties(self, data: DataCollection) -> DataProps:
+    def _compute_data_properties(
+        self, data: DataCollection, feature_costs: Dict[str, float]
+    ) -> DataProps:
         """
         Computes and encapsulates the dataset's properties, such as the number of features,
         the number of labels, and optionally the cost associated with each feature.
 
         :param data: A DataCollection instance of the dataset.
         :return: A DataProps instance containing the dataset's properties.
         """
         labels = data.y[self.label_column].unique()
         features = data.x.columns
-        feature_costs = self._compute_feature_costs(data.x)
 
         return DataProps(
             labels=labels,
             n_labels=len(labels),
             features=features,
             n_features=len(features),
             feature_costs=feature_costs,
         )
 
-    def _compute_feature_costs(self, features: pd.DataFrame) -> Dict[str, float]:
+    @staticmethod
+    def _extract_and_remove_costs(data: pd.DataFrame) -> Dict[str, float]:
         """
-        Computes the cost associated with each feature, based on the values in the cost column,
-        if such a column is specified. Otherwise, it defaults to a cost of 1.0 for all features.
+        Extracts costs from the first row below the column names and removes this row from the DataFrame.
+        Assumes the first row below the column names contains the cost for each feature.
 
-        :param features: A pandas DataFrame of the features from the dataset.
+        :param data: DataFrame from which costs are extracted.
         :return: A dictionary mapping each feature name to its associated cost.
         """
-        if self.cost_column:
-            try:
-                costs = features[self.cost_column].fillna(EPSILON).tolist()
-                return dict(zip(features.columns, costs))
-            except KeyError:
-                raise KeyError(
-                    f"Cost column '{self.cost_column}' does not exist in the data."
-                )
-        else:
-            return {feature: 1.0 for feature in features.columns}
+        try:
+            costs = data.iloc[0].fillna(1.0).to_dict()
+            data.drop(data.index[0], inplace=True)
+        except IndexError:
+            raise ValueError('Data is empty or the cost row does not exist.')
+        except Exception as e:
+            raise RuntimeError(f'An error occurred: {e!s}')
+
+        return costs
```

### Comparing `gbfs-0.1.1/gbfs/utils/distance.py` & `gbfs-0.2.0/gbfs/utils/distance.py`

 * *Files identical despite different names*

### Comparing `gbfs-0.1.1/pyproject.toml` & `gbfs-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gbfs"
-version = "0.1.1"
+version = "0.2.0"
 description = "Graph-Based Feature-Selection Algorithms"
 license = "MIT"
 readme = "README.md"
 authors = ["David Levin <davidlevin40@gmail.com>"]
 keywords = [
     "feature-selection",
     "automatic-feature-selection",
@@ -27,14 +27,15 @@
 python = "^3.10"
 pandas = "^2.2.1"
 matplotlib = "^3.8.3"
 scikit-learn = "^1.4.1.post1"
 scikit-learn-extra = "^0.3.0"
 kneed = "^0.8.5"
 seaborn = "^0.13.2"
+tqdm = "^4.66.4"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = {extras = ["imaging"], version = "^9.5.13"}
```

### Comparing `gbfs-0.1.1/PKG-INFO` & `gbfs-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbfs
-Version: 0.1.1
+Version: 0.2.0
 Summary: Graph-Based Feature-Selection Algorithms
 Home-page: https://github.com/davidlevinwork/gbfs/
 License: MIT
 Keywords: feature-selection,automatic-feature-selection,clustering,dimensionality-reduction
 Author: David Levin
 Author-email: davidlevin40@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -20,23 +20,27 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: kneed (>=0.8.5,<0.9.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: scikit-learn-extra (>=0.3.0,<0.4.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Project-URL: Documentation, https://davidlevinwork.github.io/gbfs/
 Project-URL: Repository, https://github.com/davidlevinwork/gbfs/
 Description-Content-Type: text/markdown
 
 ## GB-FS
 
 **gbfs** is a comprehensive repository dedicated to advancing Graph-Based Feature Selection methodologies in machine learning. Our project houses two significant contributions to the field: GB-AFS and GB-BC-FS, each developed to address the intricate challenges of feature selection with graph-based solutions.
 
 [![Downloads](https://static.pepy.tech/badge/gbfs)](https://pepy.tech/project/gbfs) [![Downloads](https://static.pepy.tech/badge/gbfs/month)](https://pepy.tech/project/gbfs)
+[![ci Status](https://github.com/davidlevinwork/gbfs/actions/workflows/ci.yml/badge.svg)](https://github.com/davidlevinwork/gbfs/actions/workflows/ci.yml)
+[![Tests Status](https://github.com/davidlevinwork/gbfs/actions/workflows/tests.yml/badge.svg)](https://github.com/davidlevinwork/gbfs/actions/workflows/tests.yml)
+
 
 ## Table of contents
 - [Our Contributions](#our-contributions)
 - [Installation](#installation)
 - [Usage](#usage)
   - [GB-AFS](#GB-AFS)
     - [Initialization](#Initialization)
```

