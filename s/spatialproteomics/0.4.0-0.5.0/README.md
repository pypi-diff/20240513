# Comparing `tmp/spatialproteomics-0.4.0.tar.gz` & `tmp/spatialproteomics-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialproteomics-0.4.0.tar", max compression
+gzip compressed data, was "spatialproteomics-0.5.0.tar", max compression
```

## Comparing `spatialproteomics-0.4.0.tar` & `spatialproteomics-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0     1097 2024-05-08 09:00:56.250594 spatialproteomics-0.4.0/LICENSE
--rw-r--r--   0        0        0      964 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1606 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/__init__.py
--rw-r--r--   0        0        0       94 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/base_logger.py
--rw-r--r--   0        0        0     2933 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/constants.py
--rw-r--r--   0        0        0     1877 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/container.py
--rw-r--r--   0        0        0       78 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/ext/__init__.py
--rw-r--r--   0        0        0    17113 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/ext/external.py
--rw-r--r--   0        0        0       69 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/la/__init__.py
--rw-r--r--   0        0        0    26568 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/la/label.py
--rw-r--r--   0        0        0      455 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/la/utils.py
--rw-r--r--   0        0        0      260 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/pl/__init__.py
--rw-r--r--   0        0        0    37508 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/pl/plot.py
--rw-r--r--   0        0        0     5077 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/pl/spectra.py
--rw-r--r--   0        0        0     3787 2024-05-08 09:00:56.354594 spatialproteomics-0.4.0/spatialproteomics/pl/utils.py
--rw-r--r--   0        0        0      568 2024-05-08 09:00:56.358594 spatialproteomics-0.4.0/spatialproteomics/pp/__init__.py
--rw-r--r--   0        0        0     7494 2024-05-08 09:00:56.358594 spatialproteomics-0.4.0/spatialproteomics/pp/intensity.py
--rw-r--r--   0        0        0    40725 2024-05-08 09:00:56.358594 spatialproteomics-0.4.0/spatialproteomics/pp/preprocessing.py
--rw-r--r--   0        0        0     9948 2024-05-08 09:00:56.358594 spatialproteomics-0.4.0/spatialproteomics/pp/utils.py
--rw-r--r--   0        0        0      100 2024-05-08 09:00:56.358594 spatialproteomics-0.4.0/spatialproteomics/tl/__init__.py
--rw-r--r--   0        0        0     6433 2024-05-08 09:00:56.358594 spatialproteomics-0.4.0/spatialproteomics/tl/gaussian.py
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 spatialproteomics-0.4.0/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 spatialproteomics-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-13 11:05:00.246427 spatialproteomics-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1381 2024-05-13 11:05:00.246427 spatialproteomics-0.5.0/README.md
+-rw-r--r--   0        0        0     1080 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1472 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/base_logger.py
+-rw-r--r--   0        0        0     2860 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/constants.py
+-rw-r--r--   0        0        0     1816 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/container.py
+-rw-r--r--   0        0        0       69 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/la/__init__.py
+-rw-r--r--   0        0        0    29344 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/la/label.py
+-rw-r--r--   0        0        0      936 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/la/utils.py
+-rw-r--r--   0        0        0      184 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/pl/__init__.py
+-rw-r--r--   0        0        0    29957 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/pl/plot.py
+-rw-r--r--   0        0        0     8101 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/pl/utils.py
+-rw-r--r--   0        0        0      522 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/pp/__init__.py
+-rw-r--r--   0        0        0     6023 2024-05-13 11:05:00.346428 spatialproteomics-0.5.0/spatialproteomics/pp/intensity.py
+-rw-r--r--   0        0        0    44753 2024-05-13 11:05:00.350428 spatialproteomics-0.5.0/spatialproteomics/pp/preprocessing.py
+-rw-r--r--   0        0        0    12879 2024-05-13 11:05:00.350428 spatialproteomics-0.5.0/spatialproteomics/pp/utils.py
+-rw-r--r--   0        0        0       66 2024-05-13 11:05:00.350428 spatialproteomics-0.5.0/spatialproteomics/tl/__init__.py
+-rw-r--r--   0        0        0    19495 2024-05-13 11:05:00.350428 spatialproteomics-0.5.0/spatialproteomics/tl/tool.py
+-rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 spatialproteomics-0.5.0/setup.py
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 spatialproteomics-0.5.0/PKG-INFO
```

### Comparing `spatialproteomics-0.4.0/LICENSE` & `spatialproteomics-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialproteomics-0.4.0/pyproject.toml` & `spatialproteomics-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "spatialproteomics"
 packages = [
     { include = "spatialproteomics" },
 ]
-version = "0.4.0"
-description = ""
+version = "0.5.0"
+description = "spatialproteomics provides tools for the analysis of highly multiplexed immunofluorescence data"
+readme = "README.md"
 authors = ["Harald Vohringer", "Matthias Meyer-Bender"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 xarray = "^2022.6.0"
 scikit-image = "^0.19.3"
 matplotlib = "^3.5.3"
```

### Comparing `spatialproteomics-0.4.0/spatialproteomics/__init__.py` & `spatialproteomics-0.5.0/spatialproteomics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,53 +23,49 @@
     Purple,
     Red,
     Teal,
     White,
     Yellow,
 )
 from .container import load_image_data
-from .ext import ExternalAccessor
 from .la import LabelAccessor
 from .pl import PlotAccessor
 from .pp import (
     PreprocessingAccessor,
     arcsinh_mean_intensity,
     arcsinh_median_intensity,
     arcsinh_sum_intensity,
     arcsinh_var_intensity,
-    detect_peaks_num,
     is_positive,
     mean_intensity,
     percentage_positive,
     sum_intensity,
 )
-from .tl import TwoComponentGaussianMixture
+from .tl import ToolAccessor
 
 __all__ = [
     "load_image_data",
     "PreprocessingAccessor",
     "LabelAccessor",
     "PlotAccessor",
     "SegmentationAccessor",
-    "ExternalAccessor",
+    "ToolAccessor",
     "Layers",
     "Dims",
     "Features",
     "Props",
     "sum_intensity",
     "mean_intensity",
     "arcsinh_sum_intensity",
     "arcsinh_mean_intensity",
     "arcsinh_var_intensity",
     "arcsinh_median_intensity",
     "merge_segmentation",
-    "detect_peaks_num",
     "percentage_positive",
     "is_positive",
-    "TwoComponentGaussianMixture",
     "Apricot",
     "Beige",
     "Black",
     "Blue",
     "Brown",
     "Cyan",
     "Dims",
```

### Comparing `spatialproteomics-0.4.0/spatialproteomics/constants.py` & `spatialproteomics-0.5.0/spatialproteomics/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,18 @@
 White = "#ffffff"
 Black = "#000000"
 
 
 class Layers(object):
     IMAGE = "_image"
     SEGMENTATION = "_segmentation"
-    COORDINATES = "_coordinates"
-    LABELS = "_labels"
-    DATA = "_data"
-    PLOT = "_plot"
+    PROPERTIES = "_properties"
     OBS = "_obs"
-    NEIGHBORS = "_neighbors"
     INTENSITY = "_intensity"
+    PLOT = "_plot"
 
 
 class Dims(object):
     CHANNELS = "channels"
     X = "x"
     Y = "y"
     RGBA = "rgba"
```

### Comparing `spatialproteomics-0.4.0/spatialproteomics/container.py` & `spatialproteomics-0.5.0/spatialproteomics/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 def load_image_data(
     image: np.ndarray,
     channel_coords: Union[str, List[str]],
     segmentation: Union[None, np.ndarray] = None,
     labels: Union[None, pd.DataFrame] = None,
     cell_col: str = "cell",
     label_col: str = "label",
-    copy_segmentation: bool = False,
     copy_image: bool = False,
 ):
     """Creates a image container.
 
     Creates an Xarray dataset with images, segmentation, and
     coordinate fields.
 
@@ -56,15 +55,15 @@
         dims=[Dims.CHANNELS, Dims.Y, Dims.X],
         name=Layers.IMAGE,
     )
 
     dataset = xr.Dataset(data_vars={Layers.IMAGE: im})
 
     if segmentation is not None:
-        dataset = dataset.pp.add_segmentation(segmentation, copy=copy_segmentation)
+        dataset = dataset.pp.add_segmentation(segmentation)
 
         if labels is not None:
             dataset = dataset.pp.add_labels(labels, cell_col=cell_col, label_col=label_col)
 
     else:
         dataset = xr.Dataset(data_vars={Layers.IMAGE: im})
```

### Comparing `spatialproteomics-0.4.0/spatialproteomics/ext/external.py` & `spatialproteomics-0.5.0/spatialproteomics/tl/tool.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import pandas as pd
 import xarray as xr
 
 from ..constants import Dims, Layers
 from ..pp.utils import handle_disconnected_cells
 
 
-@xr.register_dataset_accessor("ext")
-class ExternalAccessor:
-    """The external accessor enables the application of external tools such as StarDist or Astir"""
+@xr.register_dataset_accessor("tl")
+class ToolAccessor:
+    """The tool accessor enables the application of external tools such as StarDist or Astir."""
 
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
 
     def cellpose(
         self,
         channels: Optional[Union[List[str], str]] = None,
@@ -23,15 +23,15 @@
         channel_settings: list = [0, 0],
         num_iterations: int = 2000,
         cellprob_threshold: float = 0.0,
         flow_threshold: float = 0.4,
         gpu: bool = True,
         model_type: str = "cyto3",
         return_xarray: bool = True,
-        handle_disconnected: str = "keep_largest",
+        handle_disconnected: str = "ignore",
     ):
         """
         Segment cells using Cellpose.
 
         Parameters
         ----------
         channels: List[str], optional
@@ -56,14 +56,18 @@
         xr.Dataset
             Dataset containing original data and segmentation mask.
 
         Notes
         -----
         This method requires the 'cellpose' package to be installed.
         """
+        if isinstance(channels, str):
+            channels = [channels]
+        elif channels is None:
+            channels = self._obj.coords[Dims.CHANNELS].values
 
         if return_xarray:
             # if return_xarray is true, check if a segmentation mask with the key already exists
             assert (
                 key_added not in self._obj
             ), f"A segmentation mask with the key {key_added} already exists. You can either change the key with the key_added parameter, or return the predictions as a numpy array. To do this, set return_xarray to False. Alternatively, you can drop the existing segmentation mask from the object by using pp.drop_layers('{key_added}')."
 
@@ -74,19 +78,14 @@
                 self._obj.coords[Dims.CHANNELS].values
             ), "You are trying to segment only a subset of the available channels. If you want to add the segmentation mask to the xarray object directly, you need to segment either all channels or only one channel. If you want to segment a subset of the channels, you need to return the predictions as a numpy array."
 
         from cellpose import models
 
         model = models.Cellpose(gpu=gpu, model_type=model_type)
 
-        if isinstance(channels, str):
-            channels = [channels]
-        elif channels is None:
-            channels = self._obj.coords[Dims.CHANNELS].values
-
         all_masks = []
         for channel in channels:
             masks_pred, _, _, _ = model.eval(
                 self._obj.pp[channel]._image.values.squeeze(),
                 diameter=diameter,
                 channels=channel_settings,
                 niter=num_iterations,
@@ -216,15 +215,16 @@
     def stardist(
         self,
         scale: float = 3,
         n_tiles: int = 12,
         normalize: bool = True,
         nuclear_channel: str = "DAPI",
         predict_big: bool = False,
-        handle_disconnected: str = "keep_largest",
+        image_key: str = Layers.IMAGE,
+        handle_disconnected: str = "ignore",
         **kwargs,
     ) -> xr.Dataset:
         """
         Apply StarDist algorithm to perform instance segmentation on the nuclear image.
 
         Parameters:
         ----------
@@ -255,15 +255,15 @@
         import csbdeep.utils
         from stardist.models import StarDist2D
 
         if Layers.SEGMENTATION in self._obj:
             raise ValueError("The object already contains a segmentation mask. StarDist will not be executed.")
 
         # getting the nuclear image
-        nuclear_img = self._obj.pp[nuclear_channel].to_array().values.squeeze()
+        nuclear_img = self._obj.pp[nuclear_channel][image_key].values.squeeze()
 
         # normalizing the image
         if normalize:
             nuclear_img = csbdeep.utils.normalize(nuclear_img)
 
         # Load the StarDist model
         model = StarDist2D.from_pretrained("2D_versatile_fluo")
@@ -378,14 +378,45 @@
     def convert_to_anndata(
         self,
         expression_matrix_key: str = Layers.INTENSITY,
         obs_key: str = Layers.OBS,
         additional_layers: Optional[dict] = None,
         additional_uns: Optional[dict] = None,
     ):
+        """
+        Convert the spatialproteomics object to an anndata.AnnData object. The resulting AnnData object does not store the original image or segmentation mask.
+
+        Parameters:
+        ----------
+        expression_matrix_key : str, optional
+            The key of the expression matrix in the spatialproteomics object. Default is Layers.INTENSITY.
+        obs_key : str, optional
+            The key of the observation data in the spatialproteomics object. Default is Layers.OBS.
+        additional_layers : dict, optional
+            Additional layers to include in the anndata.AnnData object. The keys are the names of the layers and the values are the corresponding keys in the spatialproteomics object.
+        additional_uns : dict, optional
+            Additional uns data to include in the anndata.AnnData object. The keys are the names of the uns data and the values are the corresponding keys in the spatialproteomics object.
+
+        Returns:
+        -------
+        adata : anndata.AnnData
+            The converted anndata.AnnData object.
+
+        Raises:
+        ------
+        AssertionError
+            If the expression matrix key or additional layers are not found in the spatialproteomics object.
+
+        Notes:
+        ------
+        - The expression matrix is extracted from the spatialproteomics object using the provided expression matrix key.
+        - If additional layers are specified, they are extracted from the spatialproteomics object and added to the anndata.AnnData object.
+        - If obs_key is present in the spatialproteomics object, it is used to create the obs DataFrame of the anndata.AnnData object.
+        - If additional_uns is specified, the corresponding uns data is extracted from the spatialproteomics object and added to the anndata.AnnData object.
+        """
         import anndata
 
         # checking that the expression matrix key is present in the object
         assert (
             expression_matrix_key in self._obj
         ), f"Expression matrix key {expression_matrix_key} not found in the object. Set the expression matrix key with the expression_matrix_key argument."
 
@@ -408,26 +439,37 @@
                 adata.uns[key] = self._obj.pp.get_layer_as_df(layer)
 
         return adata
 
     def convert_to_spatialdata(
         self, image_key: str = Layers.IMAGE, segmentation_key: str = Layers.SEGMENTATION, **kwargs
     ):
+        """
+        Convert the spatialproteomics object to a spatialdata object.
+
+        Parameters:
+            image_key (str): The key of the image data in the object. Defaults to Layers.IMAGE.
+            segmentation_key (str): The key of the segmentation data in the object. Defaults to Layers.SEGMENTATION.
+            **kwargs: Additional keyword arguments to be passed to the convert_to_anndata method.
+
+        Returns:
+            spatial_data_object (spatialdata.SpatialData): The converted spatialdata object.
+        """
         import spatialdata
 
         markers = self._obj.coords[Dims.CHANNELS].values
         cells = self._obj.coords[Dims.CELLS].values
         image = spatialdata.models.Image2DModel.parse(
             self._obj[image_key].values, transformations=None, dims=("c", "x", "y"), c_coords=markers
         )
         segmentation = spatialdata.models.Labels2DModel.parse(
             self._obj[segmentation_key].values, transformations=None, dims=("x", "y")
         )
 
-        adata = self._obj.ext.convert_to_anndata(**kwargs)
+        adata = self._obj.tl.convert_to_anndata(**kwargs)
 
         # the anndata object within the spatialdata object requires some additional slots, which are created here
         adata.uns["spatialdata_attrs"] = {"region": "segmentation", "region_key": "region", "instance_key": "id"}
 
         obs_df = pd.DataFrame(
             {
                 "id": cells,
```

### Comparing `spatialproteomics-0.4.0/spatialproteomics/la/label.py` & `spatialproteomics-0.5.0/spatialproteomics/la/label.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,111 +12,21 @@
 
 @xr.register_dataset_accessor("la")
 class LabelAccessor:
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
 
     def __contains__(self, key):
-        if Layers.LABELS not in self._obj:
+        if Layers.PROPERTIES not in self._obj:
             return False
 
         label_dict = self._obj.la._label_to_dict(Props.NAME)
         return key in label_dict.keys() or key in label_dict.values()
 
-    def _relabel_dict(self, dictionary: dict):
-        _, fw, _ = relabel_sequential(self._obj.coords[Dims.LABELS].values)
-        return {fw[k]: v for k, v in dictionary.items()}
-
-    def _label_to_dict(self, prop: str, reverse: bool = False, relabel: bool = False) -> dict:
-        """Returns a dictionary that maps each label to a list to their property.
-
-        Parameters
-        ----------
-        prop : str
-            The property to map to the labels.
-        reverse : bool
-            If True, the dictionary will be reversed.
-        relabel : bool
-            Deprecated.
-
-        Returns
-        -------
-        label_dict : dict
-            A dictionary that maps each label to a list to their property.
-        """
-        labels_layer = self._obj[Layers.LABELS]
-        labels = self._obj.coords[Dims.LABELS]
-
-        label_dict = {}
-
-        for label in labels:
-            current_row = labels_layer.loc[label, prop]
-            label_dict[label.values.item()] = current_row.values.item()
-
-        if relabel:
-            return self._obj.la._relabel_dict(label_dict)
-
-        if reverse:
-            label_dict = {v: k for k, v in label_dict.items()}
-
-        return label_dict
-
-    def _cells_to_label(self, relabel: bool = False, include_unlabeled: bool = False):
-        """Returns a dictionary that maps each label to a list of cells."""
-
-        label_dict = {
-            label.item(): self._obj.la._filter_cells_by_label(label.item()) for label in self._obj.coords[Dims.LABELS]
-        }
-
-        if include_unlabeled:
-            label_dict[0] = self._obj.la._filter_cells_by_label(0)
-
-        if relabel:
-            return self._obj.la._relabel_dict(label_dict)
-
-        return label_dict
-
-    def _filter_cells_by_label(self, items: Union[int, List[int]]):
-        """Returns the list of cells with the labels from items."""
-        if type(items) is int:
-            items = [items]
-
-        cells = self._obj[Layers.OBS].loc[:, Features.LABELS].values.copy()
-        cells_bool = np.isin(cells, items)
-        cells_sel = self._obj.coords[Dims.CELLS][cells_bool].values
-
-        return cells_sel
-
-    def _label_name_to_id(self, label):
-        """Given a label name return its id."""
-        label_names_reverse = self._obj.la._label_to_dict(Props.NAME, reverse=True)
-        if label not in label_names_reverse:
-            raise ValueError(f"Cell type {label} not found.")
-
-        return label_names_reverse[label]
-
-    def _filter_by_intensity(
-        self, channel: str, func: Callable, layer_key: str = Layers.INTENSITY, return_int_array: bool = True
-    ):
-        """Returns the list of cells with the labels from items."""
-        cells = self._obj[layer_key].sel({Dims.CHANNELS: channel}).values.copy()
-        cells_bool = func(cells)
-
-        if return_int_array:
-            # turning the boolean array into a numeric array (where 0 is False, 1 is True)
-            return cells_bool.astype(int)
-
-        cells_sel = self._obj.coords[Dims.CELLS][cells_bool].values
-
-        return self._obj.sel({Dims.CELLS: cells_sel})
-
     def __getitem__(self, indices):
-        """
-        Sub selects labels.
-        """
         # type checking
         if isinstance(indices, float):
             raise TypeError("Label indices must be valid integers, str, slices, List[int] or List[str].")
 
         if isinstance(indices, int):
             if indices not in self._obj.coords[Dims.LABELS].values:
                 raise ValueError(f"Label type {indices} not found.")
@@ -129,15 +39,15 @@
             if indices not in label_dict:
                 raise ValueError(f"Label type {indices} not found.")
 
             sel = [label_dict[indices]]
 
         if isinstance(indices, slice):
             l_start = indices.start if indices.start is not None else 1
-            l_stop = indices.stop if indices.stop is not None else self._obj.dims[Dims.LABELS]
+            l_stop = indices.stop if indices.stop is not None else self._obj.sizes[Dims.LABELS]
             sel = [i for i in range(l_start, l_stop)]
 
         if isinstance(indices, (list, tuple)):
             if not all([isinstance(i, (str, int)) for i in indices]):
                 raise TypeError("Label indices must be valid integers, str, slices, List[int] or List[str].")
 
             sel = []
@@ -180,15 +90,15 @@
         -----
         - The function uses 'indices' to specify which labels to deselect.
         - 'indices' can be provided as slices, lists, tuples, or an integer.
         - The function then updates the data object to remove the deselected label indices.
         """
         if isinstance(indices, slice):
             l_start = indices.start if indices.start is not None else 1
-            l_stop = indices.stop if indices.stop is not None else self._obj.dims[Dims.LABELS]
+            l_stop = indices.stop if indices.stop is not None else self._obj.sizes[Dims.LABELS]
             sel = [i for i in range(l_start, l_stop)]
         elif isinstance(indices, list):
             assert all([isinstance(i, (int, str)) for i in indices]), "All label indices must be integers or strings."
             if all([isinstance(i, int) for i in indices]):
                 sel = indices
             else:
                 label_dict = self._obj.la._label_to_dict(Props.NAME, reverse=True)
@@ -211,14 +121,159 @@
             sel = [indices]
 
         inv_sel = [i for i in self._obj.coords[Dims.LABELS] if i not in sel]
 
         cells = self._obj.la._filter_cells_by_label(inv_sel)
         return self._obj.sel({Dims.LABELS: inv_sel, Dims.CELLS: cells})
 
+    def _relabel_dict(self, dictionary: dict):
+        _, fw, _ = relabel_sequential(self._obj.coords[Dims.LABELS].values)
+        return {fw[k]: v for k, v in dictionary.items()}
+
+    def _label_to_dict(self, prop: str, reverse: bool = False, relabel: bool = False) -> dict:
+        """
+        Returns a dictionary that maps each label to a list to their property.
+
+        Parameters
+        ----------
+        prop : str
+            The property to map to the labels.
+        reverse : bool
+            If True, the dictionary will be reversed.
+        relabel : bool
+            Deprecated.
+
+        Returns
+        -------
+        label_dict : dict
+            A dictionary that maps each label to a list to their property.
+        """
+        labels_layer = self._obj[Layers.PROPERTIES]
+        labels = self._obj.coords[Dims.LABELS]
+
+        label_dict = {}
+
+        for label in labels:
+            current_row = labels_layer.loc[label, prop]
+            label_dict[label.values.item()] = current_row.values.item()
+
+        if relabel:
+            return self._obj.la._relabel_dict(label_dict)
+
+        if reverse:
+            label_dict = {v: k for k, v in label_dict.items()}
+
+        return label_dict
+
+    def _cells_to_label(self, relabel: bool = False, include_unlabeled: bool = False) -> dict:
+        """
+        Returns a dictionary that maps each label to a list of cells.
+
+        Parameters
+        ----------
+        relabel : bool, optional
+            If True, relabels the dictionary keys to consecutive integers starting from 1.
+            Default is False.
+        include_unlabeled : bool, optional
+            If True, includes cells that are unlabeled in the dictionary.
+            Default is False.
+
+        Returns
+        -------
+        dict
+            A dictionary that maps each label to a list of cells. The keys are label values,
+            and the values are lists of cell indices.
+        """
+        label_dict = {
+            label.item(): self._obj.la._filter_cells_by_label(label.item()) for label in self._obj.coords[Dims.LABELS]
+        }
+
+        if include_unlabeled:
+            label_dict[0] = self._obj.la._filter_cells_by_label(0)
+
+        if relabel:
+            return self._obj.la._relabel_dict(label_dict)
+
+        return label_dict
+
+    def _filter_cells_by_label(self, items: Union[int, List[int]]):
+        """
+        Filter cells by label.
+
+        Parameters
+        ----------
+        items : int or List[int]
+            The label(s) to filter cells by. If an integer is provided, only cells with that label will be returned.
+            If a list of integers is provided, cells with any of the labels in the list will be returned.
+
+        Returns
+        -------
+        numpy.ndarray
+            An array containing the selected cells.
+        """
+        if type(items) is int:
+            items = [items]
+
+        cells = self._obj[Layers.OBS].loc[:, Features.LABELS].values.copy()
+        cells_bool = np.isin(cells, items)
+        cells_sel = self._obj.coords[Dims.CELLS][cells_bool].values
+
+        return cells_sel
+
+    def _label_name_to_id(self, label):
+        """
+        Convert a label name to its corresponding ID.
+
+        Parameters
+        ----------
+        label : str
+            The name of the label to convert.
+
+        Returns
+        -------
+        int
+            The ID corresponding to the given label name.
+
+        Raises
+        ------
+        ValueError
+            If the given label name is not found in the label names dictionary.
+        """
+        label_names_reverse = self._obj.la._label_to_dict(Props.NAME, reverse=True)
+        if label not in label_names_reverse:
+            raise ValueError(f"Cell type {label} not found.")
+
+        return label_names_reverse[label]
+
+    def _filter_by_intensity(
+        self, channel: str, func: Callable, layer_key: str = Layers.INTENSITY, return_int_array: bool = True
+    ) -> xr.Dataset:
+        """
+        Filter the cells based on intensity values for a specific channel. Useful for binarizing markers.
+
+        Parameters:
+            channel (str): The channel to filter on.
+            func (Callable): A function that takes in intensity values and returns a boolean array indicating which cells to keep.
+            layer_key (str, optional): The key of the layer containing the intensity values. Defaults to Layers.INTENSITY.
+            return_int_array (bool, optional): Whether to return the filtered cells as a numeric array (0 for False, 1 for True). Defaults to True.
+
+        Returns:
+            xarray.Dataset: The filtered cells as a DataArray if return_int_array is False, otherwise a numeric array.
+        """
+        cells = self._obj[layer_key].sel({Dims.CHANNELS: channel}).values.copy()
+        cells_bool = func(cells)
+
+        if return_int_array:
+            # turning the boolean array into a numeric array (where 0 is False, 1 is True)
+            return cells_bool.astype(int)
+
+        cells_sel = self._obj.coords[Dims.CELLS][cells_bool].values
+
+        return self._obj.sel({Dims.CELLS: cells_sel})
+
     def add_label_type(self, name: str, color: str = "w") -> xr.Dataset:
         """
         Add a new label type to the data object.
 
         This method adds a new label type with the specified 'name' and 'color' to the data object.
         The label type is used to identify and categorize cells in the segmentation mask.
 
@@ -249,27 +304,27 @@
 
         if Layers.SEGMENTATION not in self._obj:
             raise ValueError("No segmentation mask found.")
         if Layers.OBS not in self._obj:
             raise ValueError("No observation table found.")
 
         # Assert that label type is not already present
-        if Layers.LABELS in self._obj:
-            if name in self._obj[Layers.LABELS].sel({Dims.PROPS: Props.NAME}):
+        if Layers.PROPERTIES in self._obj:
+            if name in self._obj[Layers.PROPERTIES].sel({Dims.PROPS: Props.NAME}):
                 raise ValueError("Label type already exists.")
 
         array = np.array([name, color]).reshape(1, -1)
 
-        # if label annotations (Layers.LABELS) are not present, create them
-        if Layers.LABELS not in self._obj:
+        # if label properties (Layers.PROPERTIES) are not present, create them
+        if Layers.PROPERTIES not in self._obj:
             da = xr.DataArray(
                 array,
                 coords=[np.array([1]), [Props.NAME, Props.COLOR]],
                 dims=[Dims.LABELS, Dims.PROPS],
-                name=Layers.LABELS,
+                name=Layers.PROPERTIES,
             )
 
             db = xr.DataArray(
                 np.zeros(self._obj.coords[Dims.CELLS].shape[0]).reshape(-1, 1),
                 coords=[self._obj.coords[Dims.CELLS], [Features.LABELS]],
                 dims=[Dims.CELLS, Dims.FEATURES],
                 name=Layers.OBS,
@@ -281,15 +336,15 @@
             da = xr.DataArray(
                 array,
                 coords=[np.array([new_coord]), [Props.NAME, Props.COLOR]],
                 dims=[Dims.LABELS, Dims.PROPS],
             )
 
             da = xr.concat(
-                [self._obj[Layers.LABELS], da],
+                [self._obj[Layers.PROPERTIES], da],
                 dim=Dims.LABELS,
             )
             obj = xr.merge([self._obj, da])
 
         return obj
 
     def remove_label_type(self, cell_type: Union[int, List[int]]) -> xr.Dataset:
@@ -321,18 +376,16 @@
         - It then removes the specified 'cell_type' from the cell type labels, setting their cells to the 'Unlabeled' category.
         """
         if isinstance(cell_type, int):
             cell_type = [cell_type]
 
         if isinstance(cell_type, str):
             cell_type = [self._obj.la._label_name_to_id(cell_type)]
-        # TODO: If list should properly get cell -type
-        # TODO: should call reset label type prior to removing the cell type
 
-        if Layers.LABELS not in self._obj:
+        if Layers.PROPERTIES not in self._obj:
             raise ValueError("No cell type labels found.")
 
         for i in cell_type:
             if i not in self._obj.coords[Dims.LABELS].values:
                 raise ValueError(f"Cell type {i} not found.")
 
         cells_bool = (self._obj[Layers.OBS].sel({Dims.FEATURES: Features.LABELS}) == cell_type).values
@@ -366,16 +419,16 @@
         - The function ensures that 'array' is converted to a NumPy array.
         - It creates a DataArray 'da' with the given 'array' as the property values and unique cell type labels as coords.
         - The DataArray 'da' is then merged into the data object, associating properties with cell type labels.
         - If the label property already exists in the data object, it will be updated with the new property values.
         """
         # checking that we already have properties
         assert (
-            Layers.LABELS in self._obj
-        ), "No label layer found in the data object. Please add labels, e. g. via la.predict_cell_types_argmax() or ext.astir()."
+            Layers.PROPERTIES in self._obj
+        ), "No label layer found in the data object. Please add labels, e. g. via la.predict_cell_types_argmax() or tl.astir()."
         # making sure the property does not exist already
         assert prop not in self._obj.coords[Dims.PROPS].values, f"Property {prop} already exists."
 
         # checking that the length of the array matches the number of labels
         assert len(array) == len(
             self._obj.coords[Dims.LABELS].values
         ), "The length of the array must match the number of labels."
@@ -385,20 +438,20 @@
         if type(array) is list:
             array = np.array(array)
 
         da = xr.DataArray(
             array.reshape(-1, 1),
             coords=[unique_labels.astype(int), [prop]],
             dims=[Dims.LABELS, Dims.PROPS],
-            name=Layers.LABELS,
+            name=Layers.PROPERTIES,
         )
 
-        if Layers.LABELS in self._obj:
+        if Layers.PROPERTIES in self._obj:
             da = xr.concat(
-                [self._obj[Layers.LABELS], da],
+                [self._obj[Layers.PROPERTIES], da],
                 dim=Dims.PROPS,
             )
 
         return xr.merge([da, self._obj])
 
     def set_label_name(self, label, name):
         """
@@ -420,33 +473,35 @@
 
         Notes
         -----
         - The function converts the 'label' from its name to the corresponding ID for internal processing.
         - It updates the name of the cell type label in the data object to the new 'name'.
         """
         # checking that a label layer is already present
-        assert Layers.LABELS in self._obj, "No label layer found in the data object."
+        assert Layers.PROPERTIES in self._obj, "No label layer found in the data object."
         # checking if the old label exists
         assert label in self._obj.la, f"Cell type {label} not found. Existing cell types: {self._obj.la}"
         # checking if the new label already exists
-        assert name not in self._obj[Layers.LABELS].sel({Dims.PROPS: Props.NAME}), f"Label name {name} already exists."
+        assert name not in self._obj[Layers.PROPERTIES].sel(
+            {Dims.PROPS: Props.NAME}
+        ), f"Label name {name} already exists."
 
-        # getting the original labels
-        label_layer = self._obj[Layers.LABELS].copy()
+        # getting the original label properties
+        property_layer = self._obj[Layers.PROPERTIES].copy()
 
         if isinstance(label, str):
             label = self._obj.la._label_name_to_id(label)
 
-        label_layer.loc[label, Props.NAME] = name
+        property_layer.loc[label, Props.NAME] = name
 
-        # removing the old label layer
-        obj = self._obj.pp.drop_layers(Layers.LABELS)
+        # removing the old property layer
+        obj = self._obj.pp.drop_layers(Layers.PROPERTIES)
 
-        # adding the new label layer
-        return xr.merge([label_layer, obj])
+        # adding the new property layer
+        return xr.merge([property_layer, obj])
 
     def set_label_colors(self, labels: Union[str, List[str]], colors: Union[str, List[str]]):
         """
         Set the color of a specific cell type label.
 
         This method sets the 'color' of a specific cell type label identified by the 'label'.
         The 'label' can be either a label ID or the name of the cell type label.
@@ -473,21 +528,21 @@
             colors = [colors]
 
         # checking that there are as many colors as labels
         assert len(labels) == len(colors), "The number of labels and colors must be the same."
 
         # checking that a label layer is already present
         assert (
-            Layers.LABELS in self._obj
-        ), "No label layer found in the data object. Please add labels before setting colors, e. g. by using la.predict_cell_types_argmax() or ext.astir()."
+            Layers.PROPERTIES in self._obj
+        ), "No label layer found in the data object. Please add labels before setting colors, e. g. by using la.predict_cell_types_argmax() or tl.astir()."
 
         # obtaining the current properties
         props_layer = self._obj.coords[Dims.PROPS].values.tolist()
         labels_layer = self._obj.coords[Dims.LABELS].values.tolist()
-        array = self._obj._labels.values.copy()
+        array = self._obj[Layers.PROPERTIES].values.copy()
 
         for label, color in zip(labels, colors):
             # if the label does not exist in the object, a warning is thrown and we continue
             if label not in self._obj.la:
                 logger.warning(f"Label {label} not found in the data object. Skipping.")
                 continue
 
@@ -497,18 +552,18 @@
             # setting the new color for the given label
             array[labels_layer.index(label), props_layer.index(Props.COLOR)] = color
 
         da = xr.DataArray(
             array,
             coords=[labels_layer, props_layer],
             dims=[Dims.LABELS, Dims.PROPS],
-            name=Layers.LABELS,
+            name=Layers.PROPERTIES,
         )
 
-        return xr.merge([self._obj.drop_vars(Layers.LABELS), da])
+        return xr.merge([self._obj.drop_vars(Layers.PROPERTIES), da])
 
     def predict_cell_types_argmax(
         self,
         marker_dict: dict,
         key: str = Layers.INTENSITY,
         overwrite_existing_labels: bool = False,
         cell_col: str = "cell",
@@ -575,23 +630,46 @@
 
         # need to remove the old labels first (if there are old labels)
         obs = obj[Layers.OBS]
         if Features.LABELS in obs.coords[Dims.FEATURES].values:
             # ideally, we should select by Dims.FEATURES here, but that does not work syntactically
             obj[Layers.OBS] = obs.drop_sel(features=Features.LABELS)
             # removing the old colors
-            obj = obj.pp.drop_layers(Layers.LABELS)
+            obj = obj.pp.drop_layers(Layers.PROPERTIES)
 
         # adding the new labels
         return obj.pp.add_labels(celltype_prediction_df)
 
     def add_binarization(
         self, threshold_dict: dict, cell_type: Optional[str] = None, layer_key: str = "_percentage_positive_intensity"
     ):
-        """This method computes the percentage of positive cells for each channel and adds a binary feature for each channel based on the threshold. If a cell_type is specified, the binarization is only applied to this cell type."""
+        """
+        This method computes the percentage of positive cells for each channel and adds a binary feature for each channel based on the threshold.
+        If a cell_type is specified, the binarization is only applied to this cell type.
+
+        Parameters
+        ----------
+        threshold_dict : dict
+            A dictionary mapping channels to threshold values.
+        cell_type : str, optional
+            The specified cell type for which the binarization is applied, by default None.
+        layer_key : str, optional
+            The key for the new binary feature layer, by default "_percentage_positive_intensity".
+
+        Returns
+        -------
+        xr.Dataset
+            A new dataset object with the binary features added.
+
+        Notes
+        -----
+        - If a cell_type is specified, the binarization is only applied to the cells of that specific cell type.
+        - The binary feature is computed by comparing the intensity values of each channel to the threshold value.
+        - The binary feature is added as a new layer to the dataset object.
+        """
         channels = list(threshold_dict.keys())
 
         # checking that the channels are present in the data object
         assert all(
             [channel in self._obj.coords[Dims.CHANNELS].values for channel in channels]
         ), f"One or more channels not found in the data object. Available channels are: {self._obj.coords[Dims.CHANNELS]}"
 
@@ -601,15 +679,14 @@
             obj = self._obj.copy()
         else:
             obj = self._obj.pp.add_quantification(func=percentage_positive, key_added=layer_key)
 
         # if a cell type is specified, we get the and from the cell type and the binarization, which will result in only positive cells of that specific cell type
         # to get this, we first need a binary vector that tells us if a cell is of the specified cell type
         if cell_type is not None:
-            # TODO: verify if this works and add an and gate
             # getting the cell type id
             cell_type_id = obj.la._label_name_to_id(cell_type)
             # getting all of the cells that should have a 1 in the binary vector
             cells_of_specified_cell_type = obj.la[cell_type_id].cells.values
             # creating a boolean mask indicating whether each element of cells is in cells_subset
             ct_mask = np.isin(obj.cells.values, cells_of_specified_cell_type)
             # converting the boolean mask to integers (0 for False, 1 for True)
```

### Comparing `spatialproteomics-0.4.0/spatialproteomics/pl/plot.py` & `spatialproteomics-0.5.0/spatialproteomics/pl/plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,80 @@
-from typing import List, Union
+from typing import List, Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import xarray as xr
-from matplotlib.collections import LineCollection
 from matplotlib.lines import Line2D
 from matplotlib.patches import Patch
 
 from ..base_logger import logger
 from ..constants import Attrs, Dims, Features, Layers, Props
-from .spectra import format_annotation_df, plot_expression_spectra
 from .utils import (
     _autocrop,
     _colorize,
     _get_listed_colormap,
     _label_segmentation_mask,
     _render_labels,
 )
 
 
-def _set_up_subplots(num_plots, ncols=4, width=4, height=3):
-    """Set up subplots for plotting multiple factors."""
-
-    if num_plots == 1:
-        fig, ax = plt.subplots()
-        return fig, ax
-
-    nrows, reminder = divmod(num_plots, ncols)
-
-    if num_plots < ncols:
-        nrows = 1
-        ncols = num_plots
-    else:
-        nrows, reminder = divmod(num_plots, ncols)
-
-        if nrows == 0:
-            nrows = 1
-        if reminder > 0:
-            nrows += 1
-
-    fig, axes = plt.subplots(nrows, ncols, figsize=(width * ncols, height * nrows))
-    _ = [ax.axis("off") for ax in axes.flatten()[num_plots:]]
-    return fig, axes
-
-
 @xr.register_dataset_accessor("pl")
 class PlotAccessor:
     """Adds plotting functions to the image container."""
 
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
 
-    def _graph_overlay(self, ax=None):
-        graph = self._obj.se.get_graph()
-        x = self._obj[Layers.OBS].loc[:, Dims.X].values
-        y = self._obj[Layers.OBS].loc[:, Dims.Y].values
-        ax.triplot(
-            x,
-            y,
-            graph.simplices,
-            color="white",
-        )
-
     def _get_bounds(self):
-        """Returns X/Y bounds of the dataset."""
+        """
+        Get the bounds of the object.
+
+        Returns
+        -------
+        list
+            A list containing the minimum and maximum values for the x and y coordinates.
+        """
         xmin = self._obj.coords[Dims.X].values[0]
         ymin = self._obj.coords[Dims.Y].values[0]
         xmax = self._obj.coords[Dims.X].values[-1]
         ymax = self._obj.coords[Dims.Y].values[-1]
 
         return [xmin, xmax, ymin, ymax]
 
-    def _legend_background(self, **kwargs):
-        """Returns legend handles for the background."""
+    def _create_channel_legend(self, **kwargs):
+        """
+        Create a legend for the channels in the plot layer. Used when rendering intensities.
+
+        Returns:
+            elements (list): A list of Patch objects representing the legend elements.
+        """
+
+        # checking if the plot layer exists
+        assert Layers.PLOT in self._obj, "No plot layer found. Please call pl.colorize() first."
+        # checking if the image colors attribute exists
+        assert (
+            Attrs.IMAGE_COLORS in self._obj[Layers.PLOT].attrs
+        ), "No image colors found. Please call pl.colorize() first."
+
         color_dict = self._obj[Layers.PLOT].attrs[Attrs.IMAGE_COLORS]
 
         # removing unlabeled cells (label = 0)
         color_dict = {k: v for k, v in color_dict.items() if k != 0}
 
         elements = [Patch(facecolor=c, label=ch, **kwargs) for ch, c in color_dict.items()]
         return elements
 
-    def _legend_labels(self):
-        """Returns legend handles for the labels."""
+    def _create_label_legend(self):
+        """
+        Create a legend for the cell type labels.
+
+        Returns:
+            elements (list): A list of Line2D objects representing the legend elements.
+        """
+        # getting colors and names for each cell type label
         color_dict = self._obj.la._label_to_dict(Props.COLOR)
         names_dict = self._obj.la._label_to_dict(Props.NAME)
 
         # removing unlabeled cells (label = 0)
         color_dict = {k: v for k, v in color_dict.items() if k != 0}
         names_dict = {k: v for k, v in names_dict.items() if k != 0}
 
@@ -148,14 +136,18 @@
         merge : True, optional
             Merge the channel dimension. Default is True.
 
         Returns
         -------
         xr.Dataset
             The image container with the colorized image stored in Layers.PLOT.
+
+        Example Usage
+        --------------
+        >>> ds.pp['PAX5', 'CD3'].pl.colorize(['red', 'green']).pl.show()
         """
         # check if a plot already exists
         assert (
             Layers.PLOT not in self._obj
         ), "A plot layer already exists. If you want to plot the channel intensities and a segmentation mask, make sure to call pl.colorize() first, and then pl.render_segmentation() to render the segmentation on top of it. Alternatively, you can call pl.imshow(render_segmentation=True) to achieve the same effect."
 
         if isinstance(colors, str):
@@ -184,106 +176,91 @@
 
         if merge:
             da = da.sum(Dims.CHANNELS, keep_attrs=True)
             da.values[da.values > 1] = 1.0
 
         return xr.merge([self._obj, da])
 
-    def imshow(
+    def show(
         self,
-        legend_background: bool = True,
+        render_image: bool = True,
+        render_segmentation: bool = False,
+        render_labels: bool = False,
+        ax=None,
+        legend_image: bool = True,
         legend_label: bool = True,
-        legend_kwargs: dict = {"framealpha": 1},
         downsample: int = 1,
-        render_intensities: bool = True,
-        render_labels: bool = False,
-        render_segmentation: bool = False,
-        label_kwargs: dict = {},
+        legend_kwargs: dict = {"framealpha": 1},
         segmentation_kwargs: dict = {},
-        ax=None,
-    ):
+        label_kwargs: dict = {},
+    ) -> xr.Dataset:
         """
-        Plots the image.
-
-        Meant to be used in conjunction with plt.colorize and la.render_labels.
-        See examples.
-
-        Parameters
-        ----------
-        legend_background : bool, optional
-            Show the label of the colorized image. Default is False.
-        legend_label : bool, optional
-            Show the labels. Default is False.
-        legend_kwargs : dict, optional
-            Keyword arguments passed to the matplotlib legend function. Default is {"framealpha": 1}.
-        downsample : int, optional
-            Downsample factor for the image. Default is 1 (no downsampling).
-        ax : matplotlib.axes, optional
-            The matplotlib axis to plot on. If not provided, the current axis will be used.
-
-        Returns
-        -------
-        xr.Dataset
-            The updated image container.
+        Display an image with optional rendering elements. Can be used to render intensities, segmentation masks and labels, either individually or all at once.
 
-        Notes
-        -----
-        - The function is used to plot images in conjunction with 'im.colorize' and 'la.render_labels'.
-        - The appearance of the plot and the inclusion of legends can be controlled using the respective parameters.
+        Parameters:
+        - render_image (bool): Whether to render the image with channel intensities. Default is True.
+        - render_segmentation (bool): Whether to render segmentation. Default is False.
+        - render_labels (bool): Whether to render labels. Default is False.
+        - ax: The matplotlib axes to plot on. If None, the current axes will be used.
+        - legend_image (bool): Whether to show the channel legend. Default is True.
+        - legend_label (bool): Whether to show the label legend. Default is True.
+        - downsample (int): Downsample factor for the image. Default is 1 (no downsampling).
+        - legend_kwargs (dict): Keyword arguments for configuring the legend. Default is {"framealpha": 1}.
+        - segmentation_kwargs (dict): Keyword arguments for rendering the segmentation. Default is {}.
+        - label_kwargs (dict): Keyword arguments for rendering the labels. Default is {}.
+
+        Returns:
+        - obj (xr.Dataset): The modified dataset object.
+
+        Raises:
+        - AssertionError: If no rendering element is specified.
+
+        Note:
+        - This method displays an image with optional rendering elements such as intensities, labels, and segmentation.
+        - The `render_intensities`, `render_labels`, and `render_segmentation` parameters control which rendering elements are displayed.
+        - The `ax` parameter allows specifying a specific matplotlib axes to plot on. If None, the current axes will be used.
+        - The `show_channel_legend` and `show_label_legend` parameters control whether to show the channel and label legends, respectively.
+        - The `legend_kwargs`, `segmentation_kwargs`, and `label_kwargs` parameters allow configuring the appearance of the legend, segmentation, and labels, respectively.
         """
         # check that at least one rendering element is specified
         assert any(
-            [render_intensities, render_labels, render_segmentation]
-        ), "No rendering element specified. Please set at least one of 'render_intensities', 'render_labels', or 'render_segmentation' to True."
+            [render_image, render_labels, render_segmentation]
+        ), "No rendering element specified. Please set at least one of 'render_image', 'render_labels', or 'render_segmentation' to True."
 
         # copying the input object to avoid colorizing the original object in place
         obj = self._obj.copy()
-        if Layers.PLOT not in self._obj and render_intensities:
+        if Layers.PLOT not in self._obj and render_image:
             # if there are more than 20 channels, only the first one is plotted
-            if self._obj.dims[Dims.CHANNELS] > 20:
+            if self._obj.sizes[Dims.CHANNELS] > 20:
                 logger.warning(
-                    "More than 20 channels are present in the image. Plotting first channel only. You can subset the channels via pp.[['channel1', 'channel2', ...]] or specify your own color scheme by calling pp.colorize() before calling pl.imshow()l"
+                    "More than 20 channels are present in the image. Plotting first channel only. You can subset the channels via pp.[['channel1', 'channel2', ...]] or specify your own color scheme by calling pp.colorize() before calling pl.show()."
                 )
                 channel = str(self._obj.coords[Dims.CHANNELS].values[0])
                 obj = self._obj.pp[channel].pl.colorize(colors=["white"])
             # if there are less than 20 channels, all are plotted
             else:
                 obj = self._obj.pl.colorize()
 
         if render_labels:
             obj = obj.pl.render_labels(**label_kwargs)
 
         if render_segmentation:
             obj = obj.pl.render_segmentation(**segmentation_kwargs)
 
-        if ax is None:
-            ax = plt.gca()
+        legend_image = legend_image and render_image
+        legend_label = legend_label and render_labels
 
-        bounds = obj.pl._get_bounds()
-
-        ax.imshow(
-            obj[Layers.PLOT].values[::downsample, ::downsample],
-            origin="lower",
-            interpolation="none",
-            extent=bounds,
+        return obj.pl.imshow(
+            legend_image=legend_image,
+            legend_label=legend_label,
+            ax=ax,
+            downsample=downsample,
+            legend_kwargs=legend_kwargs,
         )
 
-        legend = []
-
-        if legend_background and render_intensities:
-            legend += obj.pl._legend_background()
-
-        if legend_label and render_labels:
-            legend += obj.pl._legend_labels()
-
-        if legend_background or legend_label:
-            ax.legend(handles=legend, **legend_kwargs)
-
-        return obj
-
     def annotate(
         self,
         variable: str = "cell",
         layer_key: str = Layers.OBS,
         highlight: list = [],
         text_kwargs: dict = {"color": "w", "fontsize": 12},
         highlight_kwargs: dict = {"color": "w", "fontsize": 16, "fontweight": "bold"},
@@ -337,15 +314,15 @@
             cells = sub.coords[Dims.CELLS]
 
         for cell in cells:
             x = self._obj[Layers.OBS].sel({Dims.CELLS: cell, Dims.FEATURES: Features.X}).values
             y = self._obj[Layers.OBS].sel({Dims.CELLS: cell, Dims.FEATURES: Features.Y}).values
             if variable != "cell":
                 table = self._obj[layer_key]
-                dims = table.dims
+                dims = table.sizes
                 if len(dims) != 2:
                     raise ValueError("Layer does not have the dimension.")
                 if Dims.CELLS not in dims:
                     raise ValueError("Layer does not have a cell dimension.")
 
                 dim = [d for d in dims if d != Dims.CELLS][0]
 
@@ -359,46 +336,40 @@
 
                 ax.text(x, y, s=f"{t:{format_string}}", **text_kwargs)
 
         return self._obj
 
     def render_segmentation(
         self,
-        alpha: float = 0,
-        alpha_boundary: float = 1,
+        alpha: float = 0.0,
+        alpha_boundary: float = 1.0,
         mode: str = "inner",
     ) -> xr.Dataset:
         """
-        Render the segmentation layer of the data object.
-
-        This method renders the segmentation layer of the data object and returns an updated data object
-        with the rendered visualization. The rendered segmentation is represented in RGBA format.
-
-        Parameters
-        ----------
-        alpha : float, optional
-            The alpha value to control the transparency of the rendered segmentation. Default is 0.
-        alpha_boundary : float, optional
-            The alpha value for boundary pixels in the rendered segmentation. Default is 1.
-        mode : str, optional
-            The mode for rendering the segmentation: "inner" for internal region, "boundary" for boundary pixels.
-            Default is "inner".
+        Renders the segmentation mask with optional alpha blending and boundary rendering.
 
-        Returns
-        -------
-        any
-            The updated data object with the rendered segmentation as a new plot layer.
-
-        Notes
-        -----
-        - The function extracts the segmentation layer and information about boundary pixels from the data object.
-        - It applies the specified alpha values and mode to render the segmentation.
-        - The rendered segmentation is represented in RGBA format and added as a new plot layer to the data object.
+        Parameters:
+            alpha (float, optional): The alpha value for blending the segmentation mask with the plot. Default is 0.0.
+            alpha_boundary (float, optional): The alpha value for rendering the boundary of the segmentation mask. Default is 1.0.
+            mode (str, optional): The mode for rendering the segmentation mask. Possible values are "inner" and "outer". Default is "inner".
+
+        Returns:
+            xr.Dataset: The modified xarray Dataset.
+
+        Raises:
+            AssertionError: If no segmentation layer is found in the object.
+
+        Note:
+            - The segmentation mask must be added to the object before calling this method.
+            - The segmentation mask is expected to have a single channel with integer labels.
+            - The rendered segmentation mask will be added as a new layer to the object.
         """
-        assert Layers.SEGMENTATION in self._obj, "Add Segmentation first."
+        assert (
+            Layers.SEGMENTATION in self._obj
+        ), "No segmentation layer found. Please add a segmentation mask before calling this method."
 
         color_dict = {1: "white"}
         cmap = _get_listed_colormap(color_dict)
         segmentation = self._obj[Layers.SEGMENTATION].values
 
         if Layers.PLOT in self._obj:
             attrs = self._obj[Layers.PLOT].attrs
@@ -431,54 +402,42 @@
             dims=[Dims.Y, Dims.X, Dims.RGBA],
             name=Layers.PLOT,
             attrs=attrs,
         )
         return xr.merge([self._obj, da])
 
     def render_labels(
-        self, alpha: float = 1, alpha_boundary: float = 1, mode: str = "inner", override_color: Union[str, None] = None
+        self, alpha: float = 1.0, alpha_boundary: float = 1.0, mode: str = "inner", override_color: Optional[str] = None
     ) -> xr.Dataset:
         """
-        Render the labeled cells in the data object.
-
-        This method renders the labeled cells in the data object based on the label colors and segmentation.
-        The rendered visualization is represented in RGBA format.
-
-        Parameters
-        ----------
-        alpha : float, optional
-            The alpha value to control the transparency of the rendered labels. Default is 0.
-        alpha_boundary : float, optional
-            The alpha value for boundary pixels in the rendered labels. Default is 1.
-        mode : str, optional
-            The mode for rendering the labels: "inner" for internal region, "boundary" for boundary pixels.
-            Default is "inner".
-        override_color : any, optional
-            The color value to override the default label colors. Default is None.
-
-        Returns
-        -------
-        any
-            The updated data object with the rendered labeled cells as a new plot layer.
+        Renders cell type labels on the plot.
 
-        Raises
-        ------
-        AssertionError
-            If the data object does not contain label information. Use 'add_labels' function to add labels first.
-
-        Notes
-        -----
-        - The function retrieves label colors from the data object and applies the specified alpha values and mode.
-        - It renders the labeled cells based on the label colors and the segmentation layer.
-        - The rendered visualization is represented in RGBA format and added as a new plot layer to the data object.
-        - If 'override_color' is provided, all labels will be rendered using the specified color.
+        Parameters:
+            alpha (float, optional): The transparency of the labels. Defaults to 1.0.
+            alpha_boundary (float, optional): The transparency of the label boundaries. Defaults to 1.0.
+            mode (str, optional): The mode of rendering. Can be "inner" or "outer". Defaults to "inner".
+            override_color (str, optional): The color to override the label colors. Defaults to None.
+
+        Returns:
+            xr.Dataset: The modified dataset with rendered labels.
+
+        Raises:
+            AssertionError: If no labels are found in the object.
+
+        Notes:
+            - This method requires labels to be present in the object. Add labels first using `la.predict_cell_types_argmax()` or `tl.astir()`.
+            - The `mode` parameter determines whether the labels are rendered inside or outside the label boundaries.
+            - The `override_color` parameter can be used to override the label colors with a single color.
         """
-        assert Layers.LABELS in self._obj, "Add labels via the add_labels function first."
+        assert (
+            Layers.PROPERTIES in self._obj
+        ), "No labels found in the object. Add labels first, for example by using la.predict_cell_types_argmax() or tl.astir()."
 
         color_dict = self._obj.la._label_to_dict(Props.COLOR, relabel=True)
+
         if override_color is not None:
             color_dict = {k: override_color for k in color_dict.keys()}
 
         cmap = _get_listed_colormap(color_dict)
 
         cells_dict = self._obj.la._cells_to_label(relabel=True)
         segmentation = self._obj[Layers.SEGMENTATION].values
@@ -509,100 +468,176 @@
             dims=[Dims.Y, Dims.X, Dims.RGBA],
             name=Layers.PLOT,
             attrs=attrs,
         )
 
         return xr.merge([self._obj, da])
 
-    def scatter_labels(
+    def imshow(
         self,
-        legend_label: bool = True,
-        size: float = 1,
-        alpha: float = 0.9,
-        zorder=10,
-        ax=None,
-        colorize: bool = True,
+        legend_image: bool = False,
+        legend_label: bool = False,
+        downsample: int = 1,
         legend_kwargs: dict = {"framealpha": 1},
-        scatter_kws: dict = {},
-    ) -> xr.Dataset:
+        ax=None,
+    ):
         """
-        Plots a scatter plot of labels.
+        Plots the image after rendering certain layers.
+        Meant to be used in conjunction with pl.colorize(), pl.render_segmentation and pl.render_label().
+        For a more high level wrapper, please refer to pl.show() instead.
 
         Parameters
         ----------
+        legend_image : bool, optional
+            Show the legendf for the channels. Default is False.
         legend_label : bool, optional
-            Plots the legend of the labels. Default is True.
-        size : float, optional
-            Size of the dots in the scatter plot. Default is 1.
-        alpha : float, optional
-            Alpha value for transparency of the dots in the scatter plot. Default is 0.9.
-        zorder : int, optional
-            The z-order of the scatter plot. Default is 10.
+            Show the labels. Default is False.
+        downsample : int, optional
+            Downsample factor for the image. Default is 1.
+        legend_kwargs : dict, optional
+            Additional keyword arguments for configuring the legend. Default is {"framealpha": 1}.
         ax : matplotlib.axes, optional
             The matplotlib axis to plot on. If not provided, the current axis will be used.
-        colorize : bool, optional
-            Whether to colorize the dots based on label colors. Default is True.
-        legend_kwargs : dict, optional
-            Keyword arguments passed to the matplotlib legend function. Default is {"framealpha": 1}.
-        scatter_kws : dict, optional
-            Additional keyword arguments to be passed to the matplotlib scatter function.
 
         Returns
         -------
         xr.Dataset
             The updated image container.
 
         Notes
         -----
-        - The function plots a scatter plot of labels from the data object.
-        - The size, alpha, and zorder parameters control the appearance of the scatter plot.
-        - You can colorize the dots based on label colors using the 'colorize' parameter.
-        - The legend of the labels can be displayed using the 'legend_label' parameter.
+        - The function is used to plot images in conjunction with 'im.colorize' and 'la.render_label'.
+        - The appearance of the plot and the inclusion of legends can be controlled using the respective parameters.
+        """
+        if Layers.PLOT not in self._obj:
+            logger.warning("No plot defined yet. Plotting the first channel only. Please call pl.colorize() first.")
+            channel = str(self._obj.coords[Dims.CHANNELS].values[0])
+            self._obj = self._obj.pp[channel].pp.colorize(colors=["white"])
+
+        if ax is None:
+            ax = plt.gca()
+
+        bounds = self._obj.pl._get_bounds()
+
+        ax.imshow(
+            self._obj[Layers.PLOT].values[::downsample, ::downsample],
+            origin="lower",
+            interpolation="none",
+            extent=bounds,
+        )
+
+        legend = []
+
+        if legend_image:
+            legend += self._obj.pl._create_channel_legend()
+
+        if legend_label:
+            legend += self._obj.pl._create_label_legend()
+
+        if legend_image or legend_label:
+            ax.legend(handles=legend, **legend_kwargs)
+
+        return self._obj
+
+    def scatter_labels(
+        self,
+        legend: bool = True,
+        size: float = 1.0,
+        alpha: float = 0.9,
+        zorder: int = 10,
+        ax=None,
+        legend_kwargs: dict = {"framealpha": 1},
+        scatter_kwargs: dict = {},
+    ) -> xr.Dataset:
+        """
+        Scatter plot of labeled cells.
+
+        Parameters:
+        -----------
+        legend : bool, optional
+            Whether to show the legend. Default is True.
+        size : float, optional
+            Size of the scatter markers. Default is 1.0.
+        alpha : float, optional
+            Transparency of the scatter markers. Default is 0.9.
+        zorder : int, optional
+            The z-order of the scatter markers. Default is 10.
+        ax : matplotlib.axes.Axes, optional
+            The axes on which to plot the scatter. If not provided, the current axes will be used.
+        legend_kwargs : dict, optional
+            Additional keyword arguments for configuring the legend. Default is {"framealpha": 1}.
+        scatter_kwargs : dict, optional
+            Additional keyword arguments for configuring the scatter plot.
+
+        Returns:
+        --------
+        xr.Dataset
+            The modified spatialproteomics object.
         """
         if ax is None:
             ax = plt.gca()
 
         color_dict = self._obj.la._label_to_dict(Props.COLOR)
         label_dict = self._obj.la._cells_to_label()
 
-        for k, v in label_dict.items():
-            label_subset = self._obj.la[k]
+        for celltype in label_dict.keys():
+            label_subset = self._obj.la[celltype]
             obs_layer = label_subset[Layers.OBS]
             x = obs_layer.loc[:, Features.X]
             y = obs_layer.loc[:, Features.Y]
-            if colorize:
-                ax.scatter(x.values, y.values, s=size, c=color_dict[k], alpha=alpha, zorder=zorder, **scatter_kws)
-            else:
-                ax.scatter(x.values, y.values, s=size, alpha=alpha, zorder=zorder, **scatter_kws)
+            ax.scatter(x.values, y.values, s=size, c=color_dict[celltype], alpha=alpha, zorder=zorder, **scatter_kwargs)
 
         xmin, xmax, ymin, ymax = self._obj.pl._get_bounds()
         ax.set_ylim([ymin, ymax])
         ax.set_xlim([xmin, xmax])
 
-        if legend_label:
-            legend = self._obj.pl._legend_labels()
+        if legend:
+            legend = self._obj.pl._create_label_legend()
             ax.legend(handles=legend, **legend_kwargs).set_zorder(102)
 
         return self._obj
 
     def scatter(
         self,
         feature: str,
+        palette: dict = None,
+        legend: bool = True,
         layer_key: str = Layers.OBS,
-        legend_label: bool = True,
-        size: float = 1,
+        size: float = 1.0,
         alpha: float = 0.9,
-        zorder=10,
+        zorder: int = 10,
         ax=None,
         legend_kwargs: dict = {"framealpha": 1},
         scatter_kws: dict = {},
-        color_scheme: dict = None,
     ) -> xr.Dataset:
         """
-        Plots a scatter plot of an arbitrary element of the _obs-
+        Create a scatter plot of some feature. At the moment, only categorical features are supported.
+
+        Parameters:
+        - feature (str): The feature to be plotted.
+        - palette (dict, optional): A dictionary mapping feature values to colors. If not provided, a default palette will be used.
+        - legend (bool, optional): Whether to show the legend. Default is True.
+        - layer_key (str, optional): The key of the layer to be plotted. Default is Layers.OBS.
+        - size (float, optional): The size of the scatter points. Default is 1.0.
+        - alpha (float, optional): The transparency of the scatter points. Default is 0.9.
+        - zorder (int, optional): The z-order of the scatter points. Default is 10.
+        - ax (object, optional): The matplotlib axes object to plot on. If not provided, the current axes will be used.
+        - legend_kwargs (dict, optional): Additional keyword arguments for configuring the legend. Default is {"framealpha": 1}.
+        - scatter_kws (dict, optional): Additional keyword arguments for configuring the scatter plot. Default is {}.
+
+        Returns:
+        - xr.Dataset: The original data object.
+
+        Raises:
+        - AssertionError: If the layer_key is not found in the data object.
+        - AssertionError: If the feature is not found in the specified layer.
+        - AssertionError: If the X or Y coordinates are not found in the specified layer.
+        - AssertionError: If the number of unique feature values is greater than 10 and no color_scheme is provided.
+        - AssertionError: If not all unique feature values are present in the provided palette.
+
         """
         if ax is None:
             ax = plt.gca()
 
         # check if the layer exists
         assert layer_key in self._obj, f"Layer {layer_key} not found in the data object."
 
@@ -614,41 +649,41 @@
         # check if the layer contains X and Y coordinates
         assert Features.X in layer.coords[Dims.FEATURES], f"Feature {Features.X} not found in the layer {layer_key}."
         assert Features.Y in layer.coords[Dims.FEATURES], f"Feature {Features.Y} not found in the layer {layer_key}."
 
         x = layer.loc[:, Features.X]
         y = layer.loc[:, Features.Y]
 
-        if color_scheme is None:
-            # Default color scheme
+        if palette is None:
+            # Default palette
             unique_values = np.unique(layer.sel(features=feature))
             assert (
                 len(unique_values) <= 10
             ), "Scatter currently only supports categorical features with 10 or fewer unique values. If you want more than 10 features, please provide a color_scheme."
             colors = plt.cm.tab10(np.linspace(0, 1, len(unique_values)))  # Using tab10 colormap for 10 unique colors
             color_dict = {val: color for val, color in zip(unique_values, colors)}
         else:
-            color_dict = color_scheme
-            # check if all unique values are present in the color scheme
+            color_dict = palette
+            # check if all unique values are present in the palette
             assert set(np.unique(layer.sel(features=feature))) <= set(
                 color_dict.keys()
-            ), f"Not all values are present in the color scheme. Make sure the following keys are in your color_scheme: {np.unique(layer.sel(features=feature))}."
+            ), f"Not all values are present in the palette. Make sure the following keys are in your palette: {np.unique(layer.sel(features=feature))}."
 
         # Assigning colors based on feature values
         colors = [color_dict.get(val, "gray") for val in layer.sel(features=feature).values]
 
         ax.scatter(x.values, y.values, color=colors, s=size, alpha=alpha, zorder=zorder, **scatter_kws)
 
         xmin, xmax, ymin, ymax = self._obj.pl._get_bounds()
         ax.set_ylim([ymin, ymax])
         ax.set_xlim([xmin, xmax])
 
         ax.set_aspect("equal")  # Set equal aspect ratio for x and y axes
 
-        if legend_label:
+        if legend:
             # Creating legend labels based on unique feature values
             legend_handles = [
                 plt.Line2D([0], [0], marker="o", color="w", markersize=5, markerfacecolor=color, label=val)
                 for val, color in color_dict.items()
             ]
             ax.legend(handles=legend_handles, **legend_kwargs).set_zorder(102)
 
@@ -677,15 +712,15 @@
             The linewidth of the box. Default is 2.
         ax : matplotlib.axes, optional
             The matplotlib axis to plot on. If not provided, the current axis will be used.
 
         Returns
         -------
         xr.Dataset
-            The updated image container.
+            The updated spatialproteomics object.
 
         Notes
         -----
         - The function adds a rectangular box to the current plot with specified x and y bounds.
         - The box can be customized using the 'color' and 'linewidth' parameters.
         """
 
@@ -696,335 +731,31 @@
         xmin, xmax = xlim
         ymin, ymax = ylim
 
         ax.hlines(xmin=xmin, xmax=xmax, y=ymin, color=color, linewidth=linewidth)
         ax.hlines(xmin=xmin, xmax=xmax, y=ymax, color=color, linewidth=linewidth)
         ax.vlines(ymin=ymin, ymax=ymax, x=xmin, color=color, linewidth=linewidth)
         ax.vlines(ymin=ymin, ymax=ymax, x=xmax, color=color, linewidth=linewidth)
-        return self._obj
-
-    def bar(self, ax=None, bar_kwargs: dict = {}):
-        """
-        Plots a bar plot of present labels.
-
-        Parameters
-        ----------
-        ax : matplotlib.axes, optional
-            The matplotlib axis to plot on. If not provided, the current axis will be used.
-        bar_kwargs : dict, optional
-            Keyword arguments passed to the matplotlib bar function.
-
-        Returns
-        -------
-        xr.Dataset
-            The updated image container.
-
-        Notes
-        -----
-        - The function plots a bar plot of present labels in the data object.
-        - The appearance of the bar plot can be customized using 'bar_kwargs'.
-        """
-        if ax is None:
-            ax = plt.gca()
-
-        color_dict = self._obj.la._label_to_dict(Props.COLOR)
-        names_dict = self._obj.la._label_to_dict(Props.NAME)
-
-        obs_layer = self._obj[Layers.OBS]
-        label_array = obs_layer.loc[:, Features.LABELS].values
-        x, y = np.unique(label_array, return_counts=True)
-        query = ~(x == 0)
-
-        ax.bar(x[query], y[query], color=[color_dict[i] for i in x[query]], **bar_kwargs)
-        ax.set_xticks(x[query])
-        ax.set_xticklabels([names_dict[i] for i in x[query]], rotation=90)
-        ax.set_ylabel("Label Frequency")
-        ax.set_xlabel("Label")
-
-        return self._obj
-
-    def pie(
-        self,
-        wedgeprops={"linewidth": 7, "edgecolor": "white"},
-        circle_radius=0.2,
-        labels=True,
-        ax=None,
-    ):
-        """
-        Plots a pie chart of label frequencies.
-
-        Parameters
-        ----------
-        wedgeprops : dict, optional
-            Keyword arguments passed to the matplotlib pie function for wedge properties.
-        circle_radius : float, optional
-            The radius of the inner circle in the pie chart. Default is 0.2.
-        labels : bool, optional
-            Whether to display labels on the pie chart. Default is True.
-        ax : matplotlib.axes, optional
-            The matplotlib axis to plot on. If not provided, the current axis will be used.
-
-        Returns
-        -------
-        None
-
-        Notes
-        -----
-        - The function plots a pie chart of label frequencies in the data object.
-        - The appearance of the pie chart can be customized using 'wedgeprops' and 'circle_radius'.
-        - Labels on the pie chart can be shown or hidden using the 'labels' parameter.
-        """
-        if ax is None:
-            ax = plt.gca()
-
-        color_dict = self._obj.la._label_to_dict(Props.COLOR)
-        names_dict = self._obj.la._label_to_dict(Props.NAME)
-
-        obs_layer = self._obj[Layers.OBS]
-        label_array = obs_layer.loc[:, Features.LABELS].values
-        x, y = np.unique(label_array, return_counts=True)
-
-        ax.pie(
-            y,
-            labels=[names_dict[i] for i in x] if labels else None,
-            colors=[color_dict[i] for i in x],
-            wedgeprops=wedgeprops,
-        )
-        my_circle = plt.Circle((0, 0), circle_radius, color="white")
-        ax.add_artist(my_circle)
-
-    def spectra(self, cells: Union[List[int], int], layers_key="intensity", ncols=4, width=4, height=3, ax=None):
-        """
-        Plots the spectra of cells.
-
-        Parameters
-        ----------
-        cells : Union[List[int], int]
-            The cell ID(s) whose spectra will be plotted.
-        layers_key : str, optional
-            The key representing the layer in the data object for plotting spectra. Default is "intensity".
-        ax : matplotlib.axes, optional
-            The matplotlib axis to plot on. If not provided, a new figure and axis will be created.
-
-        Returns
-        -------
-        xr.Dataset
-            The selected data array for the plotted cells.
-
-        Notes
-        -----
-        - The function plots the spectra of the specified cell(s) using the 'layers_key' from the data object.
-        """
-        if type(cells) is int:
-            cells = [cells]
-
-        da = self._obj[layers_key].sel({"cells": cells})
-        num_cells = len(cells)
-
-        fig, axes = _set_up_subplots(num_cells, ncols=ncols, width=width, height=height)
-
-        # fig, axes = plt.subplots(1, num_cells, figsize=(4 * num_cells, 3))
-
-        if num_cells > 1:
-            for i, ax in zip(range(da.values.shape[0]), axes.flatten()):
-                ax.bar(np.arange(da.values.shape[1]), da.values[i])
-                ax.set_xticks(np.arange(da.values.shape[1]))
-                ax.set_xticklabels(da.channels.values, rotation=90)
-                ax.set_title(f"Cell {da.cells.values[i]}")
-        else:
-            axes.bar(np.arange(da.values.squeeze().shape[0]), da.values.squeeze())
-            axes.set_xticks(np.arange(da.values.squeeze().shape[0]))
-            axes.set_xticklabels(da.channels.values, rotation=90)
-            axes.set_title(f"Cell {da.cells.values[0]}")
-
-        # if ax is isinstance(ax, np.ndarray):
-        # assert np.prod(ax.shape) >= num_cells, "Must provide at least one axis for each cell to plot."
-
-        return da
-
-    def spectra_with_annotation(
-        self,
-        cells: Union[List[int], None] = None,
-        layers_key="intensity",
-        format_df=None,
-        plot_kwargs: dict = {
-            "width": 12,
-            "height": 2,
-            "hspace": 1.0,
-            "wspace": 0.0001,
-            "xticks": True,
-        },
-    ):
-        """
-        Plots the spectra of cells with annotation.
-
-        Parameters
-        ----------
-        cells : Union[List[int], None], optional
-            The cell ID(s) whose spectra will be plotted. If None, all cells will be plotted.
-        layers_key : str, optional
-            The key representing the layer in the data object for plotting spectra. Default is "intensity".
-        format_df : pd.DataFrame or None, optional
-            A DataFrame containing annotation information for the plotted cells. Default is None (no annotation).
-        plot_kwargs : dict, optional
-            Additional keyword arguments for setting up subplots and plot appearance.
-
-        Returns
-        -------
-        xr.Dataset
-            The image container.
-
-        Notes
-        -----
-        - The function plots the spectra of the specified cell(s) using the 'layers_key' from the data object.
-        - Annotates the spectra using the provided 'format_df' DataFrame.
-        """
-
-        if cells is None:
-            cells = self._obj.coords[Dims.CELLS].values.tolist()
-
-        # da = self._obj.se.quantify_cells(cells)
-        da = self._obj[layers_key].sel({"cells": cells})
-        annot = format_annotation_df(format_df, da)
-
-        plot_expression_spectra(
-            da.values,
-            annot,
-            titles=[f"{i}" for i in da.coords[Dims.CELLS]],
-            **plot_kwargs,
-        )
 
         return self._obj
 
-    def draw_edges(self, color="white", linewidths=0.5, zorder=0, ax=None):
-        """
-        Draws edges connecting neighboring cells.
-
-        Parameters
-        ----------
-        color : str, optional
-            The color of the edges. Default is "white".
-        linewidths : float, optional
-            The linewidth of the edges. Default is 0.5.
-        zorder : int, optional
-            The z-order of the edges in the plot. Default is 0.
-        ax : matplotlib.axes, optional
-            The matplotlib axis to plot on. If not provided, the current axis will be used.
-
-        Returns
-        -------
-        xr.Dataset
-            The updated image container.
+    def autocrop(
+        self, padding: int = 50, downsample: int = 10, key: str = Layers.IMAGE, channel: Optional[str] = None
+    ) -> xr.Dataset:
 
-        Notes
-        -----
-        - The function draws edges connecting neighboring cells in the plot.
-        - The appearance of the edges can be customized using 'color' and 'linewidths'.
         """
-        coords = self._obj[Layers.OBS].loc[:, [Features.X, Features.Y]]
-        neighbors = self._obj[Layers.NEIGHBORS].values.reshape(-1)
-        cell_dim = self._obj.dims[Dims.CELLS]
-        neighbor_dim = self._obj.dims[Dims.NEIGHBORS]
-
-        # set up edgelist
-        origin = coords.values
-        target = coords.sel({Dims.CELLS: neighbors}).values.reshape(cell_dim, neighbor_dim, 2)
-
-        # line segments
-        all_lines = []
-        for k in range(target.shape[1]):
-            lines = [[i, j] for i, j in zip(map(tuple, origin), map(tuple, target[:, k]))]
-            all_lines.extend(lines)
-
-        # Line collection
-        # REFACTOR
-        lc = LineCollection(all_lines, colors=color, linewidths=linewidths, zorder=zorder)
-        if ax is None:
-            ax = plt.gca()
-
-        ax.add_collection(lc)
-        xmin, xmax, ymin, ymax = self._obj.pl._get_bounds()
-        ax.set_ylim([ymin, ymax])
-        ax.set_xlim([xmin, xmax])
-
-        return self._obj
-
-    def channel_histogram(
-        self,
-        intensity_key: str,
-        bins: int = 50,
-        ncols: int = 4,
-        width: float = 4,
-        height: float = 3,
-        log_scale: bool = False,
-        ax=None,
-        **kwargs,
-    ):
-        """
-        Plots histograms of intensity values for each channel.
-
-        Parameters
-        ----------
-        intensity_key : str
-            The key representing the intensity values in the data object.
-        bins : int, optional
-            The number of bins for histogram bins. Default is 50.
-        ncols : int, optional
-            The number of columns for subplot arrangement. Default is 4.
-        width : float, optional
-            The width of the figure. Default is 4.
-        height : float, optional
-            The height of the figure. Default is 3.
-        log_scale : bool, optional
-            Whether to use a logarithmic scale for the y-axis. Default is False.
-        ax : matplotlib.axes, optional
-            The matplotlib axis to plot on. If not provided, subplots will be created.
-        **kwargs : dict, optional
-            Additional keyword arguments passed to the matplotlib hist function.
-
-        Returns
-        -------
-        xr.Dataset
-            The image container.
-
-        Notes
-        -----
-        - The function plots histograms of intensity values for each channel using the 'intensity_key' from the data object.
-        - The histograms are arranged in subplots with 'ncols' columns.
-        - Additional keyword arguments can be passed to customize the appearance of the histograms.
-        """
-        intensities = self._obj[intensity_key]
-        channels = self._obj.coords[Dims.CHANNELS].values
-        num_channels = len(channels)
-
-        # if num_channels > 1 and ax is not None:
-        #     logger.warning("More than one channel. Plotting on first axis.")
-        #     # assert np.prod(ax.shape) >= num_channels, "Must provide at least one axis for each channel to plot."
-        # else:
-        #     if ax is None:
-        #         ax = plt.gca()
-
-        if num_channels > 1:
-
-            fig, axes = _set_up_subplots(num_channels, ncols=ncols, width=width, height=height)
-
-            for ch, ax in zip(channels, axes.flatten()):
-                data = intensities.sel({Dims.CHANNELS: ch}).values
-                ax.hist(data, bins=bins, **kwargs)
-                ax.set_title(ch)
-                if log_scale:
-                    ax.set_yscale("log")
-        else:
-            if ax is None:
-                ax = plt.gca()
-            ch = channels[0]
-            data = intensities.sel({Dims.CHANNELS: ch}).values
-            ax.hist(data, bins=bins, **kwargs)
-            ax.set_title(ch)
-            if log_scale:
-                ax.set_yscale("log")
-
-        return self._obj
+        Crop the image so that the background surrounding the tissue/TMA gets cropped away.
 
-    def autocrop(self, channel=None, downsample=10):
-        slices = _autocrop(self._obj, channel=channel, downsample=downsample)
+        Parameters:
+        - padding (int): The padding to be added around the cropped image in pixels. Default is 50.
+        - downsample (int): The downsampling factor for the image. Default is 10.
+        - key (str): The key of the image to be cropped. Default is Layers.IMAGE.
+        - channel (str, optional): The channel used for cropping. Default is None, which defaults to using the first available channel.
+
+        Returns:
+        - obj.pp (object): The cropped image.
+        """
+        if channel is None:
+            channel = self._obj.coords[Dims.CHANNELS].values.tolist()[0]
+        img = self._obj.pp[channel].pp.downsample(downsample)[key].values.squeeze()
+        slices = _autocrop(img, downsample=downsample, padding=padding)
         return self._obj.pp[slices[0], slices[1]]
```

### Comparing `spatialproteomics-0.4.0/spatialproteomics/pp/__init__.py` & `spatialproteomics-0.5.0/spatialproteomics/pp/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from .intensity import (
     arcsinh_mean_intensity,
     arcsinh_median_intensity,
     arcsinh_sum_intensity,
     arcsinh_var_intensity,
-    detect_peaks_num,
     is_positive,
     mean_intensity,
     percentage_positive,
     sum_intensity,
 )
 from .preprocessing import PreprocessingAccessor
 
@@ -15,11 +14,10 @@
     "PreprocessingAccessor",
     "mean_intensity",
     "sum_intensity",
     "arcsinh_mean_intensity",
     "arcsinh_sum_intensity",
     "arcsinh_var_intensity",
     "arcsinh_median_intensity",
-    "detect_peaks_num",
     "is_positive",
     "percentage_positive",
 ]
```

### Comparing `spatialproteomics-0.4.0/spatialproteomics/pp/preprocessing.py` & `spatialproteomics-0.5.0/spatialproteomics/pp/preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,57 +9,63 @@
 from skimage.morphology import disk
 from skimage.restoration import unsupervised_wiener
 from skimage.segmentation import expand_labels
 
 from ..base_logger import logger
 from ..constants import COLORS, Dims, Features, Labels, Layers, Props
 from ..la.utils import _format_labels
-from .intensity import sum_intensity
+from .intensity import arcsinh_median_intensity
 from .utils import (
+    _get_disconnected_cell,
     _merge_segmentation,
     _normalize,
     _relabel_cells,
     _remove_unlabeled_cells,
     handle_disconnected_cells,
 )
 
 
 @xr.register_dataset_accessor("pp")
 class PreprocessingAccessor:
-    """The image accessor enables fast indexing and preprocesses image.data"""
+    """The image accessor enables fast indexing and preprocessing of the spatialproteomics object."""
 
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
 
     def __getitem__(self, indices) -> xr.Dataset:
-        """Fast subsetting the image container. The following examples show how
+        """
+        Fast subsetting the image container. The following examples show how
         the user can subset the image container:
 
         Subset the image container using x and y coordinates:
-        >> ds.pp[0:50, 0:50]
+        >>> ds.pp[0:50, 0:50]
 
         Subset the image container using x and y coordinates and channels:
-        >> ds.pp['Hoechst', 0:50, 0:50]
+        >>> ds.pp['Hoechst', 0:50, 0:50]
 
         Subset the image container using channels:
-        >> ds.pp['Hoechst']
+        >>> ds.pp['Hoechst']
 
         Multiple channels can be selected by passing a list of channels:
-        >> ds.pp[['Hoechst', 'CD4']]
+        >>> ds.pp[['Hoechst', 'CD4']]
 
-        Parameters:
-        -----------
-        indices: str, slice, list, tuple
+        Parameters
+        ----------
+        indices : str, slice, list, tuple
             The indices to subset the image container.
-        Returns:
-        --------
+
+        Returns
+        -------
         xarray.Dataset
             The subsetted image container.
         """
-        # argument handling
+        # checking if the user provided dict_values or dict_keys and turns them into a list if that is the case
+        if type(indices) is {}.keys().__class__ or type(indices) is {}.values().__class__:
+            indices = list(indices)
+
         if type(indices) is str:
             c_slice = [indices]
             x_slice = slice(None)
             y_slice = slice(None)
         elif type(indices) is slice:
             c_slice = slice(None)
             x_slice = indices
@@ -158,28 +164,25 @@
             # finalise query
             query[Dims.CELLS] = cells
 
         return self._obj.sel(query)
 
     def get_channels(self, channels: Union[List[str], str]) -> xr.Dataset:
         """
-        Returns a single channel as a numpy array.
+        Retrieve the specified channels from the dataset.
 
-        Parameters
-        ----------
-        channels: Union[str, list]
-            The name of the channel or a list of channel names.
+        Parameters:
+        channels (Union[List[str], str]): The channels to retrieve. Can be a single channel name or a list of channel names.
 
-        Returns
-        -------
-        xarray.Dataset
-            The selected channels as a new image container.
+        Returns:
+        xr.Dataset: The dataset containing the specified channels.
         """
         if isinstance(channels, str):
             channels = [channels]
+
         # build query
         query = {Dims.CHANNELS: channels}
 
         return self._obj.sel(query)
 
     def add_channel(self, channels: Union[str, list], array: np.ndarray) -> xr.Dataset:
         """
@@ -222,40 +225,36 @@
 
         da = xr.DataArray(
             array,
             coords=[channels, range(other_x_dim), range(other_y_dim)],
             dims=Dims.IMAGE,
             name=Layers.IMAGE,
         )
-        # im = xr.concat([self._obj[Layers.IMAGE], da], dim=Dims.IMAGE[0])
 
         return xr.merge([self._obj, da])
 
     def add_segmentation(
         self,
         segmentation: np.ndarray,
         mask_growth: int = 0,
         relabel: bool = True,
-        copy: bool = True,
-        handle_disconnected: str = "keep_largest",
+        handle_disconnected: str = "ignore",
     ) -> xr.Dataset:
         """
         Adds a segmentation mask (_segmentation) field to the xarray dataset.
 
         Parameters
         ----------
         segmentation : np.ndarray
             A segmentation mask, i.e., a np.ndarray with image.shape = (x, y),
             that indicates the location of each cell.
         mask_growth : int
             The number of pixels by which the segmentation mask should be grown.
         relabel : bool
             If true the segmentation mask is relabeled to have continuous numbers from 1 to n.
-        copy : bool
-            If true the segmentation mask is copied.
 
         Returns:
         --------
         xr.Dataset
             The amended xarray.
         """
 
@@ -265,17 +264,15 @@
 
         assert (x_dim == self._obj.sizes[Dims.X]) & (
             y_dim == self._obj.sizes[Dims.Y]
         ), "The shape of segmentation mask does not match that of the image."
 
         # checking if there are any disconnected cells in the input
         handle_disconnected_cells(segmentation, mode=handle_disconnected)
-
-        if copy:
-            segmentation = segmentation.copy()
+        segmentation = segmentation.copy()
 
         if relabel:
             segmentation, _ = _relabel_cells(segmentation)
 
         if mask_growth > 0:
             segmentation = expand_labels(segmentation, mask_growth)
 
@@ -295,15 +292,15 @@
 
     def add_observations(
         self,
         properties: Union[str, list, tuple] = ("label", "centroid"),
         return_xarray: bool = False,
     ) -> xr.Dataset:
         """
-        Adds properties derived from the mask to the image container.
+        Adds properties derived from the segmentation mask to the image container.
 
         Parameters
         ----------
         properties : Union[str, list, tuple]
             A list of properties to be added to the image container. See
             skimage.measure.regionprops_table for a list of available properties.
         return_xarray : bool
@@ -429,25 +426,25 @@
             dim=Dims.FEATURES,
         )
 
         return xr.merge([self._obj, da])
 
     def add_quantification(
         self,
-        func=sum_intensity,
+        func=arcsinh_median_intensity,
         key_added: str = Layers.INTENSITY,
         return_xarray=False,
     ) -> xr.Dataset:
         """
         Quantify channel intensities over the segmentation mask.
 
         Parameters
         ----------
         func : Callable, optional
-            The function used for quantification. Default is sum_intensity.
+            The function used for quantification. Default is arcsinh_median_intensity.
         key_added : str, optional
             The key under which the quantification data will be stored in the image container. Default is Layers.INTENSITY.
         return_xarray : bool, optional
             If True, the function returns an xarray.DataArray with the quantification data instead of adding it to the image container.
 
         Returns
         -------
@@ -560,23 +557,23 @@
         if prop == Features.LABELS:
             unique_labels = np.unique(_format_labels(array))
 
         da = xr.DataArray(
             array.reshape(-1, 1),
             coords=[unique_labels.astype(int), [prop]],
             dims=[Dims.LABELS, Dims.PROPS],
-            name=Layers.LABELS,
+            name=Layers.PROPERTIES,
         )
 
         if return_xarray:
             return da
 
-        if Layers.LABELS in self._obj:
+        if Layers.PROPERTIES in self._obj:
             da = xr.concat(
-                [self._obj[Layers.LABELS], da],
+                [self._obj[Layers.PROPERTIES], da],
                 dim=Dims.PROPS,
             )
 
         return xr.merge([da, self._obj])
 
     def add_labels(
         self,
@@ -779,15 +776,16 @@
         return xr.merge([obj, normed])
 
     def filter(self, quantile: float = 0.99, key_added: Optional[str] = None):
         # Pull out the image from its corresponding field (by default "_image")
         image_layer = self._obj[Layers.IMAGE]
         if isinstance(quantile, list):
             quantile = np.array(quantile)
-        # Calulate quat
+
+        # calculate quantile
         lower = np.quantile(image_layer.values.reshape(image_layer.values.shape[0], -1), quantile, axis=1)
         filtered = (image_layer - np.expand_dims(np.diag(lower) if lower.ndim > 1 else lower, (1, 2))).clip(min=0)
 
         if key_added is None:
             obj = self._obj.drop(Layers.IMAGE)
 
         filtered = xr.DataArray(
@@ -814,43 +812,74 @@
             dims=[Dims.CHANNELS, Dims.Y, Dims.X],
             name=Layers.PLOT,
         )
 
         return xr.merge([self._obj, normed])
 
     def downsample(self, rate: int):
+        """
+        Downsamples the image and segmentation mask in the object by a given rate.
+
+        Parameters:
+        - rate (int): The downsampling rate. Only every `rate`-th pixel will be kept.
+
+        Returns:
+        - xr.Dataset: The downsampled object containing the updated image and segmentation mask.
+
+        Raises:
+        - AssertionError: If no image layer is found in the object.
+        - AssertionError: If no segmentation mask is found in the object.
+        """
+        # checking if the object contains an image layer
+        assert Layers.IMAGE in self._obj, "No image layer found in the object."
+        # checking if the object contains a segmentation mask
+        assert Layers.SEGMENTATION in self._obj, "No segmentation mask found in the object."
+
         image_layer = self._obj[Layers.IMAGE]
-        # image_data = image_layer.values[:, ::rate,::rate]
 
         x = self._obj.x.values[::rate]
         y = self._obj.y.values[::rate]
         c = self._obj.channels.values
-        # import pdb;pdb.set_trace()
         img = image_layer.values[:, ::rate, ::rate]
-        # import pdb;pdb.set_trace()
         new_img = xr.DataArray(img, coords=[c, y, x], dims=[Dims.CHANNELS, Dims.Y, Dims.X], name=Layers.IMAGE)
-        # import pdb;pdb.set_trace()
         obj = self._obj.drop(Layers.IMAGE)
-        # import pdb;pdb.set_trace()
 
         if Layers.SEGMENTATION in self._obj:
             seg_layer = self._obj[Layers.SEGMENTATION]
-            # import pdb;pdb.set_trace()
             new_seg = xr.DataArray(
                 seg_layer.values[::rate, ::rate], coords=[y, x], dims=[Dims.Y, Dims.X], name=Layers.SEGMENTATION
             )
-            # import pdb;pdb.set_trace()
             obj = obj.drop(Layers.SEGMENTATION)
 
         obj = obj.drop_dims([Dims.Y, Dims.X])
 
         return xr.merge([obj, new_img, new_seg])
 
     def filter_by_obs(self, col: str, func: Callable):
-        """Returns the list of cells with the labels from items."""
+        """
+        Filter the object by observations based on a given feature and filtering function.
+
+        Parameters:
+            col (str): The name of the feature to filter by.
+            func (Callable): A filtering function that takes in the values of the feature and returns a boolean array.
+
+        Returns:
+            xr.Dataset: The filtered object with the selected cells and updated segmentation mask.
+
+        Raises:
+            AssertionError: If the feature does not exist in the object's observations.
+
+        Notes:
+            - This method filters the object by selecting only the cells that satisfy the filtering condition.
+            - It also updates the segmentation mask to remove cells that are not selected and relabels the remaining cells.
+
+        Example:
+            To filter the object by the feature "area" and keep only the cells with an area greater than 70px:
+            >>> obj = obj.pp.add_observations('area').pp.filter_by_obs('area', lambda x: x > 70)
+        """
         # checking if the feature exists in obs
         assert (
             col in self._obj.coords[Dims.FEATURES].values
         ), f"Feature {col} not found in obs. You can add it with pp.add_observations()."
 
         cells = self._obj[Layers.OBS].sel({Dims.FEATURES: col}).values.copy()
         cells_bool = func(cells)
@@ -878,18 +907,29 @@
 
         # removing the old segmentation
         obj = obj.drop_vars(Layers.SEGMENTATION)
 
         # adding the new filtered and relabeled segmentation
         return xr.merge([obj, da])
 
-    def grow_cells(self, iterations: int = 2, handle_disconnected: str = "keep_largest"):
+    def grow_cells(self, iterations: int = 2, handle_disconnected: str = "ignore") -> xr.Dataset:
         """
-        Grows the cells in the segmentation mask.
+        Grows the segmentation masks by expanding the labels in the object.
+
+        Parameters:
+        - iterations (int): The number of iterations to grow the segmentation masks. Default is 2.
+        - handle_disconnected (str): The mode to handle disconnected segmentation masks. Options are "ignore", "remove", or "fill". Default is "ignore".
+
+        Raises:
+        - ValueError: If the object does not contain a segmentation mask.
+
+        Returns:
+        - obj (xarray.Dataset): The object with the grown segmentation masks and updated observations.
         """
+
         if Layers.SEGMENTATION not in self._obj:
             raise ValueError("The object does not contain a segmentation mask.")
 
         # getting the segmentation mask
         segmentation = self._obj[Layers.SEGMENTATION].values
 
         # growing segmentation masks
@@ -929,19 +969,43 @@
     def merge_segmentation(
         self,
         array: np.ndarray,
         labels: Optional[Union[str, List[str]]] = None,
         threshold: float = 1.0,
         handle_disconnected: str = "relabel",
     ):
-        # array = all of the arrays that will iteratively be merged to the existing segmentation mask
+        """
+        Merge segmentation masks with the existing segmentation mask in the xarray object.
+
+        Parameters:
+            array (np.ndarray): The array containing the segmentation masks to be merged. It can be 2D or 3D.
+            labels (Optional[Union[str, List[str]]]): Optional. The labels corresponding to each segmentation mask in the array.
+                If provided, the number of labels must match the number of arrays.
+            threshold (float): Optional. The threshold value for merging cells. Default is 1.0.
+            handle_disconnected (str): Optional. The method to handle disconnected cells. Default is "relabel".
+
+        Returns:
+            obj (xarray.Dataset): The xarray object with the merged segmentation mask.
+
+        Raises:
+            AssertionError: If no segmentation mask is found in the xarray object.
+            AssertionError: If the input array is not 2D or 3D.
+            AssertionError: If the input array is not of type int.
+            AssertionError: If the shape of the input array does not match the shape of the segmentation mask.
+
+        Notes:
+            - If the input array is 2D, it will be expanded to 3D.
+            - If labels are provided, they need to match the number of arrays.
+            - The merging process starts with merging the biggest cells first, then the smaller ones.
+            - Disconnected cells in the input are handled based on the specified method.
+        """
         # ensuring that a segmentation mask already exists
         assert (
             Layers.SEGMENTATION in self._obj
-        ), "No segmentation mask found in the xarray object. Please add one first using pp.add_segmentation() or ext.stardist()/ext.cellpose()."
+        ), "No segmentation mask found in the xarray object. Please add one first using pp.add_segmentation() or tl.stardist()/tl.cellpose()."
 
         # checking that the array is 2D or 3D
         assert array.ndim in [
             2,
             3,
         ], "The input array must be 2D (if you want to merge one segmentation mask) or 3D (if you want to iteratively merge multiple segmentation masks)."
 
@@ -1042,21 +1106,39 @@
             # creating and adding the new labels
             label_df = pd.DataFrame({"cell": mapping.keys(), "label": mapping.values()})
             obj = obj.pp.add_labels(label_df)
 
         return obj
 
     def get_layer_as_df(self, layer: str = Layers.OBS, celltypes_to_str: bool = True):
-        """This method converts a layer of the image container to a pandas dataframe."""
+        """
+        Returns the specified layer as a pandas DataFrame.
+
+        Parameters:
+            layer (str): The name of the layer to retrieve. Defaults to Layers.OBS.
+            celltypes_to_str (bool): Whether to convert celltype labels to strings. Defaults to True.
+
+        Returns:
+            pandas.DataFrame: The layer data as a DataFrame.
+        """
         data_array = self._obj[layer]
 
         dims = data_array.dims
         coords = data_array.coords
         c1, c2 = coords[dims[0]].values, coords[dims[1]].values
         df = pd.DataFrame(data_array.values, index=c1, columns=c2)
 
         # special case: when exporting obs, we can convert celltypes to strings
         if celltypes_to_str and layer == Layers.OBS and Features.LABELS in df.columns:
             label_dict = self._obj.la._label_to_dict(Props.NAME)
             df[Features.LABELS] = df[Features.LABELS].apply(lambda x: label_dict[x])
 
         return df
+
+    def get_disconnected_cell(self) -> int:
+        """
+        Returns the first disconnected cell from the segmentation layer.
+
+        Returns:
+            ndarray: The first disconnected cell from the segmentation layer.
+        """
+        return _get_disconnected_cell(self._obj[Layers.SEGMENTATION])
```

### Comparing `spatialproteomics-0.4.0/spatialproteomics/pp/utils.py` & `spatialproteomics-0.5.0/spatialproteomics/pp/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,31 @@
+from typing import List, Tuple
+
 import numpy as np
 import scipy.ndimage
-from skimage.measure import regionprops
+from skimage.measure import label, regionprops
 from skimage.segmentation import relabel_sequential
 
 from ..base_logger import logger
 
 
-def merge(images, colors=["C1", "C2", "C3", "C4", "C5"], proj="sum", alpha=0.5):
+def merge(images: List[np.ndarray], proj: str = "sum", alpha: float = 0.5):
+    """
+    Merge multiple images into a single image using different projection methods.
+
+    Parameters:
+    - images (List[np.ndarray]): A list of images to be merged.
+    - proj (str, optional): The projection method to be used. Default is "sum".
+        - "sum": Sum the pixel values of the images.
+        - "blend": Blend the images using alpha blending.
+    - alpha (float, optional): The alpha value used in blending. Default is 0.5.
 
+    Returns:
+    - im_combined (np.ndarray): The merged image.
+    """
     if proj == "sum":
         im_combined = np.sum(np.stack(images, axis=3), axis=3)
         im_combined[im_combined > 1] = 1
     elif proj == "blend":
         im_base = images[0].copy()
         for i in range(1, len(images)):
             alpha_a = images[i][:, :, 3][:, :, np.newaxis]
@@ -23,70 +37,76 @@
                 images[i][:, :, 0:3] * alpha_a + im_base[:, :, 0:3] * alpha_b * (1 - alpha_a)
             ) / alpha_0
             im_base = im_combined
 
     return im_combined
 
 
-def _remove_unlabeled_cells(segmentation: np.ndarray, cells: np.ndarray, copy: bool = True) -> np.ndarray:
-    """Removes all cells from the segmentation that are not in cells."""
-    if copy:
-        segmentation = segmentation.copy()
-    bool_mask = ~np.isin(segmentation, cells)
-    segmentation[bool_mask] = 0
+def _remove_unlabeled_cells(segmentation: np.ndarray, cells: np.ndarray) -> np.ndarray:
+    """
+    Remove unlabeled cells from the segmentation mask.
 
-    return segmentation
+    Parameters:
+    ----------
+    segmentation : np.ndarray
+        The segmentation array representing the labeled cells.
+    cells : np.ndarray
+        The array of cell labels to keep.
 
+    Returns:
+    -------
+    np.ndarray
+        The updated segmentation array with unlabeled cells removed.
+    """
+    segmentation_copy = segmentation.copy()
+    bool_mask = ~np.isin(segmentation_copy, cells)
+    segmentation_copy[bool_mask] = 0
 
-def _relabel_cells(segmentation: np.ndarray):
+    return segmentation_copy
+
+
+def _relabel_cells(segmentation: np.ndarray) -> Tuple[np.ndarray, dict]:
     """
-    Relabels cells in a segmentation array.
+    This method relabels cells in the segmentation array, so that non-consecutive labels are turned into labels from 1 to n again.
 
     Parameters:
     ----------
     segmentation : np.ndarray
         The input segmentation array.
 
     Returns:
     -------
-    tuple[np.ndarray, dict]
+    Tuple[np.ndarray, dict]
         A tuple containing the relabeled segmentation array and a mapping dictionary.
-
-    Notes:
-    ------
-    This method relabels cells in the segmentation array, so that non-consecutive labels are turned into labels from 1 to n again.
-    This is important since CellSeg's mask growing relies on this assumption.
-
-    The mapping dictionary provides a mapping from the original values to the new values.
     """
-    unique_values = np.unique(segmentation)  # Find unique values in the array
-    # num_unique_values = len(unique_values)  # Get the number of unique values
+    # find unique cell IDs
+    unique_values = np.unique(segmentation)
 
-    # Create a mapping from original values to new values
+    # create a mapping from original values to new values
     value_map = {value: i for i, value in enumerate(unique_values)}
 
-    # Map the original array to the new values using the mapping
+    # map the original array to the new values using the mapping
     segmentation_relabeled = np.vectorize(lambda x: value_map[x])(segmentation)
 
     return segmentation_relabeled, value_map
 
 
-def _merge_segmentation(s1, s2, label1=1, label2=2, threshold=1.0):
+def _merge_segmentation(s1: np.ndarray, s2: np.ndarray, label1: int = 1, label2: int = 2, threshold: float = 1.0):
     """
     Merge two segmentation masks based on specified criteria.
 
     Parameters
     ----------
     s1 : numpy.ndarray
         First segmentation mask.
     s2 : numpy.ndarray
         Second segmentation mask.
-    label1 : int, optional
+    label1 : int
         Label for regions from the first mask in the final merged mask. Default is 1.
-    label2 : int, optional
+    label2 : int
         Label for regions from the second mask in the final merged mask. Default is 2.
     threshold : float, optional
         Threshold for area ratio of intersection over union for merging regions.
         Default is 1.0, meaning all regions from the second mask are merged.
 
     Returns
     -------
@@ -132,18 +152,17 @@
 
 def _normalize(
     img: np.ndarray,
     pmin: float = 3.0,
     pmax: float = 99.8,
     eps: float = 1e-20,
     clip: bool = False,
-    name: str = "normed",
 ) -> np.ndarray:
-    """Performs a min max normalisation.
-
+    """
+    Performs a min max normalisation.
     This function was adapted from the csbdeep package.
 
     Parameters
     ----------
     dataarray: xr.DataArray
         A xarray DataArray with an image field.
     pmin: float
@@ -153,55 +172,104 @@
     eps: float
         Epsilon float added to prevent 0 division.
     clip: bool
         Ensures that normed image array contains no values greater than 1.
 
     Returns
     -------
-    xr.DataArray
+    np.ndarray
         A min-max normalized image.
     """
     perc = np.percentile(img, [pmin, pmax], axis=(1, 2)).T
 
     norm = (img - np.expand_dims(perc[:, 0], (1, 2))) / (np.expand_dims(perc[:, 1] - perc[:, 0], (1, 2)) + eps)
 
     if clip:
         norm = np.clip(norm, 0, 1)
 
     return norm
 
 
-def _check_for_disconnected_cells(segmentation: np.ndarray, handle: str = "error"):
+def _check_for_disconnected_cells(segmentation: np.ndarray, handle: str = "error") -> bool:
     """
-    This method checks for disconnected cells in a segmentation mask.
-    It returns True if there are disconnected cells, and False otherwise.
-    handle can be 'error', 'warning', or 'ignore'.
-    """
-    # Label connected components in the entire segmentation mask
-    labeled_mask, num_features = scipy.ndimage.label(segmentation, structure=np.ones((3, 3)))
+    Check for disconnected cells in a segmentation mask.
+
+    Parameters:
+    ----------
+    segmentation : np.ndarray
+        The segmentation mask to check for disconnected cells.
+    handle : str, optional
+        The handling option for disconnected cells. Can be 'error', 'warning', or 'ignore'.
 
-    # Count the number of objects for each cell
-    num_objects_per_cell = np.bincount(labeled_mask[segmentation != 0].ravel())[1:]
+    Returns:
+    -------
+    bool
+        True if there are disconnected cells, False otherwise.
 
-    # Find cells with more than one object
-    cells_with_multiple_objects = np.where(num_objects_per_cell != 1)[0] + 1
+    Raises:
+    ------
+    ValueError
+        If disconnected cells are found and the handle is set to 'error'.
+
+    Warnings:
+    ---------
+    If disconnected cells are found and the handle is set to 'warning'.
 
-    if len(cells_with_multiple_objects) > 0:
+    Notes:
+    ------
+    This method checks for disconnected cells in a segmentation mask. It returns True if there are disconnected cells,
+    and False otherwise. The handle parameter determines how disconnected cells are handled. If handle is set to 'error',
+    a ValueError is raised. If handle is set to 'warning', a warning is logged. If handle is set to 'ignore', the method
+    returns True without raising an error or warning.
+    """
+    relabeled_mask = label(segmentation)
+    num_cells = len(np.unique(segmentation))
+    num_cells_relabeled = len(np.unique(relabeled_mask))
+
+    if num_cells == num_cells_relabeled:
+        return False
+    else:
         if handle == "error":
-            example_cell = cells_with_multiple_objects[0]
-            raise ValueError(f"Found disconnected masks in the segmentation. Example cell: {example_cell}.")
+            raise ValueError(
+                "Found disconnected masks in the segmentation. Use pp.get_disconnected_cell() to get an example of a disconnected cell."
+            )
         elif handle == "warning":
-            logger.warning("Found disconnected masks in the segmentation.")
+            logger.warning(
+                "Found disconnected masks in the segmentation. Use pp.get_disconnected_cell() to to get an example of a disconnected cell."
+            )
         return True
 
-    return False
-
 
 def handle_disconnected_cells(segmentation: np.ndarray, mode: str = "ignore"):
-    """This method handles disconnected cells in a segmentation mask. It can either completely remove any disconnected components, do nothing, only keep the largest or relabel."""
+    """
+    Handle disconnected cells in a segmentation mask.
+
+    Parameters:
+        segmentation (np.ndarray): The input segmentation mask.
+        mode (str, optional): The mode to handle disconnected cells.
+            - "ignore": Do nothing and keep the original segmentation mask.
+            - "remove": Remove disconnected cells from the segmentation mask.
+            - "relabel": Relabel cells to avoid disconnected cells.
+            - "keep_largest": Keep only the largest component of each disconnected cell.
+
+    Returns:
+        np.ndarray: The updated segmentation mask.
+
+    Raises:
+        AssertionError: If the mode is not one of 'ignore', 'remove', 'relabel', 'keep_largest'.
+
+    Notes:
+        - This method checks if there are any disconnected cells in the segmentation mask.
+        - If there are no disconnected cells, it returns the original segmentation mask.
+        - The behavior depends on the chosen mode:
+            - "ignore": Do nothing and return the original segmentation mask.
+            - "remove": Remove disconnected cells by setting their values to 0.
+            - "relabel": Relabel cells to avoid disconnected cells.
+            - "keep_largest": Keep only the largest component of each disconnected cell.
+    """
     assert mode in [
         "ignore",
         "remove",
         "relabel",
         "keep_largest",
     ], f"Could not recognize mode {mode}. Please choose one of 'ignore', 'remove', 'relabel', 'keep_largest'."
 
@@ -255,7 +323,24 @@
                         continue
                     # for any other entity, we give it a new ID
                     max_cell_id += 1
                     segmentation = np.where(new_labels == unique_label, max_cell_id, segmentation)
         logger.warning("Relabeled all cells to avoid disconnected cells.")
 
     return segmentation
+
+
+def _get_disconnected_cell(segmentation: np.ndarray) -> int:
+    """
+    Find and return the first disconnected cell in the given segmentation.
+
+    Parameters:
+    segmentation (np.ndarray): The segmentation array representing the cells.
+
+    Returns:
+    int: The label of the first disconnected cell found, or None if no disconnected cell is found.
+    """
+    for cell in sorted(np.unique(segmentation))[1:]:
+        binary_mask = np.where(segmentation == cell, 1, 0)
+        _, num_features = scipy.ndimage.label(binary_mask)
+        if num_features != 1:
+            return cell
```

