# Comparing `tmp/eddymotion-0.1.3.tar.gz` & `tmp/eddymotion-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eddymotion-0.1.3.tar", last modified: Sat Apr 10 10:51:52 2021, max compression
+gzip compressed data, was "dist/eddymotion-0.1.4.tar", last modified: Mon Apr 12 11:22:53 2021, max compression
```

## Comparing `eddymotion-0.1.3.tar` & `eddymotion-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 oesteban   (502) staff       (20)        0 2021-04-10 10:51:52.064643 eddymotion-0.1.3/
--rw-r--r--   0 oesteban   (502) staff       (20)        0 2021-03-10 08:06:25.000000 eddymotion-0.1.3/CHANGES.rst
--rw-r--r--   0 oesteban   (502) staff       (20)    22408 2021-03-10 08:06:25.000000 eddymotion-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 oesteban   (502) staff       (20)    11346 2021-03-10 08:06:25.000000 eddymotion-0.1.3/LICENSE
--rw-r--r--   0 oesteban   (502) staff       (20)      171 2021-04-08 21:01:54.000000 eddymotion-0.1.3/MANIFEST.in
--rw-r--r--   0 oesteban   (502) staff       (20)     2250 2021-03-10 08:06:25.000000 eddymotion-0.1.3/Makefile
--rw-r--r--   0 oesteban   (502) staff       (20)     1107 2021-04-10 10:51:52.065092 eddymotion-0.1.3/PKG-INFO
--rw-r--r--   0 oesteban   (502) staff       (20)      213 2021-04-08 20:24:47.000000 eddymotion-0.1.3/README.md
-drwxr-xr-x   0 oesteban   (502) staff       (20)        0 2021-04-10 10:51:52.058144 eddymotion-0.1.3/eddymotion/
--rw-r--r--   0 oesteban   (502) staff       (20)      337 2021-04-08 20:53:16.000000 eddymotion-0.1.3/eddymotion/__init__.py
--rw-r--r--   0 oesteban   (502) staff       (20)       85 2021-04-10 10:51:51.000000 eddymotion-0.1.3/eddymotion/_version.py
-drwxr-xr-x   0 oesteban   (502) staff       (20)        0 2021-04-10 10:51:52.063750 eddymotion-0.1.3/eddymotion/config/
--rw-r--r--   0 oesteban   (502) staff       (20)      959 2021-04-08 20:24:47.000000 eddymotion-0.1.3/eddymotion/config/dwi-to-b0_level1.json
--rw-r--r--   0 oesteban   (502) staff       (20)      954 2021-04-08 20:24:47.000000 eddymotion-0.1.3/eddymotion/config/dwi-to-dwi_level1.json
--rw-r--r--   0 oesteban   (502) staff       (20)     7999 2021-04-10 10:51:00.000000 eddymotion-0.1.3/eddymotion/dmri.py
--rw-r--r--   0 oesteban   (502) staff       (20)     7258 2021-04-08 20:39:44.000000 eddymotion-0.1.3/eddymotion/estimator.py
--rw-r--r--   0 oesteban   (502) staff       (20)     6611 2021-04-10 10:51:00.000000 eddymotion-0.1.3/eddymotion/model.py
--rw-r--r--   0 oesteban   (502) staff       (20)     1020 2021-04-10 10:51:00.000000 eddymotion-0.1.3/eddymotion/viz.py
-drwxr-xr-x   0 oesteban   (502) staff       (20)        0 2021-04-10 10:51:52.062250 eddymotion-0.1.3/eddymotion.egg-info/
--rw-r--r--   0 oesteban   (502) staff       (20)     1107 2021-04-10 10:51:51.000000 eddymotion-0.1.3/eddymotion.egg-info/PKG-INFO
--rw-r--r--   0 oesteban   (502) staff       (20)      506 2021-04-10 10:51:51.000000 eddymotion-0.1.3/eddymotion.egg-info/SOURCES.txt
--rw-r--r--   0 oesteban   (502) staff       (20)        1 2021-04-10 10:51:51.000000 eddymotion-0.1.3/eddymotion.egg-info/dependency_links.txt
--rw-r--r--   0 oesteban   (502) staff       (20)      834 2021-04-10 10:51:51.000000 eddymotion-0.1.3/eddymotion.egg-info/requires.txt
--rw-r--r--   0 oesteban   (502) staff       (20)       11 2021-04-10 10:51:51.000000 eddymotion-0.1.3/eddymotion.egg-info/top_level.txt
--rw-r--r--   0 oesteban   (502) staff       (20)        1 2021-04-09 14:12:40.000000 eddymotion-0.1.3/eddymotion.egg-info/zip-safe
--rw-r--r--   0 oesteban   (502) staff       (20)      327 2021-04-08 20:39:09.000000 eddymotion-0.1.3/pyproject.toml
--rw-r--r--   0 oesteban   (502) staff       (20)     1996 2021-04-10 10:51:52.068863 eddymotion-0.1.3/setup.cfg
--rw-r--r--   0 oesteban   (502) staff       (20)      636 2021-04-08 20:37:47.000000 eddymotion-0.1.3/setup.py
+drwxr-xr-x   0 oesteban   (502) staff       (20)        0 2021-04-12 11:22:53.372631 eddymotion-0.1.4/
+drwxr-xr-x   0 oesteban   (502) staff       (20)        0 2021-04-12 11:22:53.363684 eddymotion-0.1.4/.maint/
+-rw-r--r--   0 oesteban   (502) staff       (20)      192 2021-04-12 11:15:43.000000 eddymotion-0.1.4/.maint/contributors.json
+-rw-r--r--   0 oesteban   (502) staff       (20)      654 2021-04-12 11:15:43.000000 eddymotion-0.1.4/.maint/developers.json
+-rw-r--r--   0 oesteban   (502) staff       (20)       44 2021-04-12 11:15:43.000000 eddymotion-0.1.4/.maint/former.json
+-rw-r--r--   0 oesteban   (502) staff       (20)     1815 2021-04-12 11:15:43.000000 eddymotion-0.1.4/.maint/paper_author_list.py
+-rw-r--r--   0 oesteban   (502) staff       (20)     1226 2021-04-12 11:15:43.000000 eddymotion-0.1.4/.maint/update_changes.sh
+-rwxr-xr-x   0 oesteban   (502) staff       (20)     4558 2021-04-12 11:15:43.000000 eddymotion-0.1.4/.maint/update_zenodo.py
+-rw-r--r--   0 oesteban   (502) staff       (20)      426 2021-04-12 11:20:16.000000 eddymotion-0.1.4/CHANGES.rst
+-rw-r--r--   0 oesteban   (502) staff       (20)    22408 2021-03-10 08:06:25.000000 eddymotion-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 oesteban   (502) staff       (20)    11346 2021-03-10 08:06:25.000000 eddymotion-0.1.4/LICENSE
+-rw-r--r--   0 oesteban   (502) staff       (20)      171 2021-04-08 21:01:54.000000 eddymotion-0.1.4/MANIFEST.in
+-rw-r--r--   0 oesteban   (502) staff       (20)     2250 2021-03-10 08:06:25.000000 eddymotion-0.1.4/Makefile
+-rw-r--r--   0 oesteban   (502) staff       (20)     1107 2021-04-12 11:22:53.372857 eddymotion-0.1.4/PKG-INFO
+-rw-r--r--   0 oesteban   (502) staff       (20)      213 2021-04-08 20:24:47.000000 eddymotion-0.1.4/README.md
+drwxr-xr-x   0 oesteban   (502) staff       (20)        0 2021-04-12 11:22:53.367314 eddymotion-0.1.4/eddymotion/
+-rw-r--r--   0 oesteban   (502) staff       (20)      337 2021-04-08 20:53:16.000000 eddymotion-0.1.4/eddymotion/__init__.py
+-rw-r--r--   0 oesteban   (502) staff       (20)       85 2021-04-12 11:22:52.000000 eddymotion-0.1.4/eddymotion/_version.py
+drwxr-xr-x   0 oesteban   (502) staff       (20)        0 2021-04-12 11:22:53.372088 eddymotion-0.1.4/eddymotion/config/
+-rw-r--r--   0 oesteban   (502) staff       (20)      959 2021-04-08 20:24:47.000000 eddymotion-0.1.4/eddymotion/config/dwi-to-b0_level1.json
+-rw-r--r--   0 oesteban   (502) staff       (20)      954 2021-04-08 20:24:47.000000 eddymotion-0.1.4/eddymotion/config/dwi-to-dwi_level1.json
+-rw-r--r--   0 oesteban   (502) staff       (20)     8335 2021-04-12 11:15:43.000000 eddymotion-0.1.4/eddymotion/dmri.py
+-rw-r--r--   0 oesteban   (502) staff       (20)     7258 2021-04-08 20:39:44.000000 eddymotion-0.1.4/eddymotion/estimator.py
+-rw-r--r--   0 oesteban   (502) staff       (20)     6574 2021-04-12 11:15:43.000000 eddymotion-0.1.4/eddymotion/model.py
+-rw-r--r--   0 oesteban   (502) staff       (20)     7637 2021-04-12 11:15:43.000000 eddymotion-0.1.4/eddymotion/viz.py
+drwxr-xr-x   0 oesteban   (502) staff       (20)        0 2021-04-12 11:22:53.370628 eddymotion-0.1.4/eddymotion.egg-info/
+-rw-r--r--   0 oesteban   (502) staff       (20)     1107 2021-04-12 11:22:53.000000 eddymotion-0.1.4/eddymotion.egg-info/PKG-INFO
+-rw-r--r--   0 oesteban   (502) staff       (20)      650 2021-04-12 11:22:53.000000 eddymotion-0.1.4/eddymotion.egg-info/SOURCES.txt
+-rw-r--r--   0 oesteban   (502) staff       (20)        1 2021-04-12 11:22:53.000000 eddymotion-0.1.4/eddymotion.egg-info/dependency_links.txt
+-rw-r--r--   0 oesteban   (502) staff       (20)      834 2021-04-12 11:22:53.000000 eddymotion-0.1.4/eddymotion.egg-info/requires.txt
+-rw-r--r--   0 oesteban   (502) staff       (20)       11 2021-04-12 11:22:53.000000 eddymotion-0.1.4/eddymotion.egg-info/top_level.txt
+-rw-r--r--   0 oesteban   (502) staff       (20)        1 2021-04-09 14:12:40.000000 eddymotion-0.1.4/eddymotion.egg-info/zip-safe
+-rw-r--r--   0 oesteban   (502) staff       (20)      327 2021-04-08 20:39:09.000000 eddymotion-0.1.4/pyproject.toml
+-rw-r--r--   0 oesteban   (502) staff       (20)     1996 2021-04-12 11:22:53.373933 eddymotion-0.1.4/setup.cfg
+-rw-r--r--   0 oesteban   (502) staff       (20)      636 2021-04-08 20:37:47.000000 eddymotion-0.1.4/setup.py
```

### Comparing `eddymotion-0.1.3/CONTRIBUTING.md` & `eddymotion-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eddymotion-0.1.3/LICENSE` & `eddymotion-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eddymotion-0.1.3/Makefile` & `eddymotion-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `eddymotion-0.1.3/PKG-INFO` & `eddymotion-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eddymotion
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pure python eddy-current and head-motion correction for dMRI, an extension of QSIprep's SHOREline algorithm (Cieslak, 2020) to multiple diffusion models.
 Home-page: https://github.com/nipreps/EddyMotionCorrection
 Author: Derek Pisner
 Author-email: dpisner@utexas.edu
 Maintainer-email: nipreps@gmail.com, dpisner@utexas.edu
 License: Apache License, Version 2.0
 Description: UNKNOWN
```

### Comparing `eddymotion-0.1.3/eddymotion/config/dwi-to-b0_level1.json` & `eddymotion-0.1.4/eddymotion/config/dwi-to-b0_level1.json`

 * *Files identical despite different names*

### Comparing `eddymotion-0.1.3/eddymotion/config/dwi-to-dwi_level1.json` & `eddymotion-0.1.4/eddymotion/config/dwi-to-dwi_level1.json`

 * *Files identical despite different names*

### Comparing `eddymotion-0.1.3/eddymotion/dmri.py` & `eddymotion-0.1.4/eddymotion/dmri.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         """
         Produce one fold of LOGO (leave-one-gradient-out).
 
         Parameters
         ----------
         index : :obj:`int`
             Index of the DWI orientation to be left out in this fold.
+        with_b0 : :obj:`bool`
+            Insert the *b=0* reference at the beginning of the training dataset.
 
         Return
         ------
         (train_data, train_gradients) : :obj:`tuple`
             Training DWI and corresponding gradients.
             Training data/gradients come **from the updated dataset**.
         (test_data, test_gradients) :obj:`tuple`
@@ -182,14 +184,22 @@
         return plot_dwi(
             self.bzero if index is None else self.dataobj[..., index],
             self.affine,
             gradient=self.gradients[..., index] if index is not None else None,
             **kwargs,
         )
 
+    def plot_gradients(self, **kwargs):
+        """Visualize diffusion gradient."""
+        from eddymotion.viz import plot_gradients
+        return plot_gradients(
+            self.gradients,
+            **kwargs
+        )
+
     @classmethod
     def from_filename(cls, filename):
         """Read an HDF5 file from disk."""
         with h5py.File(filename, "r") as in_file:
             root = in_file["/0"]
             data = {k: np.asanyarray(v) for k, v in root.items()}
         return cls(**data)
```

### Comparing `eddymotion-0.1.3/eddymotion/estimator.py` & `eddymotion-0.1.4/eddymotion/estimator.py`

 * *Files identical despite different names*

### Comparing `eddymotion-0.1.3/eddymotion/model.py` & `eddymotion-0.1.4/eddymotion/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
         Parameters
         ----------
         gtab : :obj:`numpy.ndarray`
             An array representing the gradient table in RAS+B format.
         model : :obj:`str`
             Diffusion model.
-            Options: ``"3DShore"``, ``"SFM"``, ``"Tensor"``, ``"S0"``
+            Options: ``"3DShore"``, ``"SFM"``, ``"DTI"``, ``"DKI"``, ``"S0"``
 
         Return
         ------
         model : :obj:`~dipy.reconst.ReconstModel`
             An model object compliant with DIPY's interface.
 
         """
@@ -49,19 +49,16 @@
                 ExponentialIsotropicModel,
             )
 
             param = {
                 "isotropic": ExponentialIsotropicModel,
             }
 
-        elif model.lower().startswith("tensor"):
-            Model = TensorModel
-
-        elif model.lower().startswith("dki"):
-            Model = DKIModel
+        elif model.lower() in ("dti", "dki"):
+            Model = DTIModel if model.lower() == "dti" else DKIModel
 
         else:
             raise NotImplementedError(f"Unsupported model <{model}>.")
 
         param.update(kwargs)
         return Model(gtab, **param)
 
@@ -90,15 +87,15 @@
         """Do nothing."""
 
     def predict(self, gradient, **kwargs):
         """Return the *b=0* map."""
         return self._S0
 
 
-class TensorModel:
+class DTIModel:
     """A wrapper of :obj:`dipy.reconst.dti.TensorModel."""
 
     __slots__ = ("_model", "_S0", "_mask")
 
     def __init__(self, gtab, S0=None, mask=None, **kwargs):
         """Instantiate the wrapped tensor model."""
         from dipy.reconst.dti import TensorModel as DipyTensorModel
```

### Comparing `eddymotion-0.1.3/eddymotion.egg-info/PKG-INFO` & `eddymotion-0.1.4/eddymotion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eddymotion
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pure python eddy-current and head-motion correction for dMRI, an extension of QSIprep's SHOREline algorithm (Cieslak, 2020) to multiple diffusion models.
 Home-page: https://github.com/nipreps/EddyMotionCorrection
 Author: Derek Pisner
 Author-email: dpisner@utexas.edu
 Maintainer-email: nipreps@gmail.com, dpisner@utexas.edu
 License: Apache License, Version 2.0
 Description: UNKNOWN
```

### Comparing `eddymotion-0.1.3/eddymotion.egg-info/requires.txt` & `eddymotion-0.1.4/eddymotion.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eddymotion-0.1.3/setup.cfg` & `eddymotion-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `eddymotion-0.1.3/setup.py` & `eddymotion-0.1.4/setup.py`

 * *Files identical despite different names*

