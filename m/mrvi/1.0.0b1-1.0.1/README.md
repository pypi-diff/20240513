# Comparing `tmp/mrvi-1.0.0b1.tar.gz` & `tmp/mrvi-1.0.1.tar.gz`

## Comparing `mrvi-1.0.0b1.tar` & `mrvi-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.bumpversion.cfg
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.codecov.yaml
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.editorconfig
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.flake8
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.readthedocs.yaml
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/CHANGELOG.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.github/workflows/build.yaml
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.github/workflows/test_linux.yaml
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.github/workflows/test_linux_cuda.yaml
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.github/workflows/test_linux_pre.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/Makefile
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/changelog.md
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/conf.py
--rw-r--r--   0        0        0    14803 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/developer_docs.md
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/make.bat
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/docs/notebooks/example.ipynb
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/src/mrvi/__init__.py
--rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/src/mrvi/_components.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/src/mrvi/_constants.py
--rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/src/mrvi/_model.py
--rw-r--r--   0        0        0    15908 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/src/mrvi/_module.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/src/mrvi/_types.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/src/mrvi/_utils.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/tests/test_basic.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/tests/test_components.py
--rw-r--r--   0        0        0     9481 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/tests/test_model.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/README.md
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 mrvi-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mrvi-1.0.1/.bumpversion.cfg
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 mrvi-1.0.1/.codecov.yaml
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 mrvi-1.0.1/.editorconfig
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mrvi-1.0.1/.flake8
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 mrvi-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mrvi-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 mrvi-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 mrvi-1.0.1/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 mrvi-1.0.1/.github/workflows/test_linux.yaml
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 mrvi-1.0.1/.github/workflows/test_linux_cuda.yaml
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 mrvi-1.0.1/.github/workflows/test_linux_pre.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/changelog.md
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0    14803 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/developer_docs.md
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mrvi-1.0.1/docs/notebooks/example.ipynb
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 mrvi-1.0.1/src/mrvi/__init__.py
+-rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 mrvi-1.0.1/src/mrvi/_components.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 mrvi-1.0.1/src/mrvi/_constants.py
+-rw-r--r--   0        0        0    61758 2020-02-02 00:00:00.000000 mrvi-1.0.1/src/mrvi/_model.py
+-rw-r--r--   0        0        0    15640 2020-02-02 00:00:00.000000 mrvi-1.0.1/src/mrvi/_module.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 mrvi-1.0.1/src/mrvi/_types.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 mrvi-1.0.1/src/mrvi/_utils.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 mrvi-1.0.1/tests/test_basic.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mrvi-1.0.1/tests/test_components.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 mrvi-1.0.1/tests/test_model.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mrvi-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mrvi-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 mrvi-1.0.1/README.md
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 mrvi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8193 2020-02-02 00:00:00.000000 mrvi-1.0.1/PKG-INFO
```

### Comparing `mrvi-1.0.0b1/.flake8` & `mrvi-1.0.1/.flake8`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/.pre-commit-config.yaml` & `mrvi-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/CHANGELOG.md` & `mrvi-1.0.1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,27 @@
 
 The format is based on [Keep a Changelog][],
 and this project adheres to [Semantic Versioning][].
 
 [keep a changelog]: https://keepachangelog.com/en/1.0.0/
 [semantic versioning]: https://semver.org/spec/v2.0.0.html
 
-## [1.0.0b1] - 2023-02-21
+## [1.0.1] - 2024-05-10
+
+### :warning: Deprecation Warning
+
+-   The MrVI implementation has been moved to `scvi-tools` (`from scvi.external import MRVI`),
+    and this package will no longer be maintained.
+
+### Added
+
+-   Adds deprecation warning in the form of a FutureWarning on import.
+-   Various fixes and UX improvements to the model kwargs, DE, and DA functions.
+
+## [1.0.0b1] - 2024-02-21
 
 ### :warning: Breaking Changes
 
 -   This release is a major rework of the mrvi model and is generally incompatible with
     the previous v0.x.x releases.
 
 ### Added
```

### Comparing `mrvi-1.0.0b1/.github/workflows/build.yaml` & `mrvi-1.0.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/.github/workflows/test_linux.yaml` & `mrvi-1.0.1/.github/workflows/test_linux.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
       - name: Install test dependencies
         run: |
           python -m pip install --upgrade pip wheel
 
       - name: Install dependencies
         run: |
-          pip install --pre ".[dev,test]"
+          pip install ".[dev,test]"
 
       - name: Test
         env:
           MPLBACKEND: agg
           PLATFORM: ${{ matrix.os }}
           DISPLAY: :42
         run: |
```

### Comparing `mrvi-1.0.0b1/.github/workflows/test_linux_cuda.yaml` & `mrvi-1.0.1/.github/workflows/test_linux_cuda.yaml`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/.github/workflows/test_linux_pre.yaml` & `mrvi-1.0.1/.github/workflows/test_linux_pre.yaml`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/docs/Makefile` & `mrvi-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/docs/conf.py` & `mrvi-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/docs/developer_docs.md` & `mrvi-1.0.1/docs/developer_docs.md`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/docs/make.bat` & `mrvi-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/docs/references.bib` & `mrvi-1.0.1/docs/references.bib`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/docs/_templates/autosummary/class.rst` & `mrvi-1.0.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/docs/extensions/typed_returns.py` & `mrvi-1.0.1/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/docs/notebooks/example.ipynb` & `mrvi-1.0.1/docs/notebooks/example.ipynb`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/src/mrvi/_components.py` & `mrvi-1.0.1/src/mrvi/_components.py`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/src/mrvi/_model.py` & `mrvi-1.0.1/src/mrvi/_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
 import numpyro.distributions as dist
 import pandas as pd
 import xarray as xr
 from anndata import AnnData
+from scipy.special import logsumexp
 from scvi import REGISTRY_KEYS
 from scvi.data import AnnDataManager
 from scvi.data.fields import (
     CategoricalObsField,
     LayerField,
     NumericalJointObsField,
     NumericalObsField,
@@ -53,27 +54,45 @@
 
 class MrVI(JaxTrainingMixin, BaseModelClass):
     """
     Multi-resolution Variational Inference (MrVI).
 
     Parameters
     ----------
-    adata
+    adata : AnnData
         AnnData object that has been registered via ``setup_anndata``.
-    n_latent
-        Dimensionality of the latent space.
-    n_latent_donor
-        Dimensionality of the latent space for sample embeddings.
-    encoder_n_hidden
+    n_latent : int
+        Dimensionality of the latent space for `z`.
+    n_latent_u : int
+        Dimensionality of the latent space for `u`.
+    encoder_n_hidden : int
         Number of nodes per hidden layer in the encoder.
-    px_kwargs
+    encoder_n_layers : int
+        Number of hidden layers in the encoder.
+    z_u_prior : bool
+        Whether to use a prior for `z_u`.
+    z_u_prior_scale : float
+        Scale of the prior for the difference between `z` and `u`.
+    u_prior_scale : float
+        Scale of the prior for `u`.
+    u_prior_mixture : bool
+        Whether to use a mixture model for the `u` prior.
+    u_prior_mixture_k : int
+        Number of components in the mixture model for the `u` prior.
+    learn_z_u_prior_scale : bool
+        Whether to learn the scale of the `z` and `u` difference prior during training.
+    laplace_scale : float, optional
+        Scale parameter for the Laplace distribution in the decoder.
+    scale_observations : bool
+        Whether to scale loss by the number of observations per sample.
+    px_kwargs : dict, optional
         Keyword args for :class:`~mrvi.DecoderZX`.
-    qz_kwargs
+    qz_kwargs : dict, optional
         Keyword args for :class:`~mrvi.EncoderUZ`.
-    qu_kwargs
+    qu_kwargs : dict, optional
         Keyword args for :class:`~mrvi.EncoderXU`.
     """
 
     def __init__(
         self,
         adata,
         **model_kwargs,
@@ -83,16 +102,18 @@
         n_sample = self.summary_stats.n_sample
         n_batch = self.summary_stats.n_batch
         n_labels = self.summary_stats.n_labels
         n_continuous_cov = self.summary_stats.get("n_extra_continuous_covs", 0)
 
         obs_df = adata.obs.copy()
         obs_df = obs_df.loc[~obs_df._scvi_sample.duplicated("first")]
-        self.donor_info = obs_df.set_index("_scvi_sample").sort_index()
-        self.sample_key = self.adata_manager.get_state_registry("sample").original_key
+        self.sample_info = obs_df.set_index("_scvi_sample").sort_index()
+        self.sample_key = self.adata_manager.get_state_registry(
+            MRVI_REGISTRY_KEYS.SAMPLE_KEY
+        ).original_key
         self.sample_order = self.adata_manager.get_state_registry(
             MRVI_REGISTRY_KEYS.SAMPLE_KEY
         ).categorical_mapping
 
         self.n_obs_per_sample = jnp.array(
             adata.obs._scvi_sample.value_counts().sort_index().values
         )
@@ -104,19 +125,14 @@
             n_labels=n_labels,
             n_continuous_cov=n_continuous_cov,
             n_obs_per_sample=self.n_obs_per_sample,
             **model_kwargs,
         )
         self.init_params_ = self._get_init_params(locals())
 
-    @property
-    def original_donor_key(self):
-        """Original donor key used for training the model."""
-        return self.adata_manager.registry["setup_args"]["sample_key"]
-
     def to_device(self, device):
         # TODO(jhong): remove this once we have a better way to handle device.
         pass
 
     def _generate_stacked_rngs(
         self, n_sets: int | tuple
     ) -> dict[str, jax.random.PRNGKey]:
@@ -377,15 +393,15 @@
                     cf_sample=jnp.array(cf_sample),
                     use_mean=True,
                 )
                 mean_zs = xr.DataArray(
                     mean_zs_,
                     dims=["cell_name", "sample", "latent_dim"],
                     coords={
-                        "cell_name": self.adata.obs_names[indices],
+                        "cell_name": self.adata.obs_names[indices].values,
                         "sample": self.sample_order,
                     },
                     name="sample_representations",
                 )
             if reqs.needs_sampled_representations:
                 sampled_zs_ = mapped_inference_fn(
                     stacked_rngs=stacked_rngs,
@@ -396,15 +412,15 @@
                     mc_samples=mc_samples,
                 )  # (n_mc_samples, n_cells, n_samples, n_latent)
                 sampled_zs_ = sampled_zs_.transpose((1, 0, 2, 3))
                 sampled_zs = xr.DataArray(
                     sampled_zs_,
                     dims=["cell_name", "mc_sample", "sample", "latent_dim"],
                     coords={
-                        "cell_name": self.adata.obs_names[indices],
+                        "cell_name": self.adata.obs_names[indices].values,
                         "sample": self.sample_order,
                     },
                     name="sample_representations",
                 )
 
             if reqs.needs_mean_distances:
                 mean_dists = self._compute_distances_from_representations(
@@ -426,16 +442,15 @@
                         normalization_vars,
                     ) = self._compute_local_baseline_dists(
                         array_dict, mc_samples=mc_samples
                     )  # both are shape (n_cells,)
                     normalization_means = normalization_means.reshape(-1, 1, 1, 1)
                     normalization_vars = normalization_vars.reshape(-1, 1, 1, 1)
                     normalized_dists = (
-                        np.clip(sampled_dists - normalization_means, a_min=0, a_max=None)
-                        / (normalization_vars**0.5)
+                        (sampled_dists - normalization_means) / (normalization_vars**0.5)
                     ).mean(dim="mc_sample")  # (n_cells, n_samples, n_samples)
 
             # Compute each reduction
             for r in reductions:
                 if r.input == "mean_representations":
                     inputs = mean_zs
                 elif r.input == "sampled_representations":
@@ -543,39 +558,39 @@
 
         if reps.ndim == 3:
             dists = jax.vmap(_compute_distance)(reps)
             return xr.DataArray(
                 dists,
                 dims=["cell_name", "sample_x", "sample_y"],
                 coords={
-                    "cell_name": self.adata.obs_names[indices],
+                    "cell_name": self.adata.obs_names[indices].values,
                     "sample_x": self.sample_order,
                     "sample_y": self.sample_order,
                 },
                 name="sample_distances",
             )
         else:
             # Case with sampled representations
             dists = jax.vmap(jax.vmap(_compute_distance))(reps)
             return xr.DataArray(
                 dists,
                 dims=["cell_name", "mc_sample", "sample_x", "sample_y"],
                 coords={
-                    "cell_name": self.adata.obs_names[indices],
+                    "cell_name": self.adata.obs_names[indices].values,
                     "mc_sample": np.arange(reps.shape[1]),
                     "sample_x": self.sample_order,
                     "sample_y": self.sample_order,
                 },
                 name="sample_distances",
             )
 
     def get_local_sample_representation(
         self,
         adata: AnnData | None = None,
-        indices: list[str] | None = None,
+        indices: list[int] | None = None,
         batch_size: int = 256,
         use_mean: bool = True,
         use_vmap: bool = True,
     ) -> xr.DataArray:
         """
         Computes the local sample representation of the cells in the adata object.
 
@@ -697,35 +712,44 @@
             norm=norm,
             mc_samples=mc_samples,
         )
 
     def get_aggregated_posterior(
         self,
         adata: AnnData | None = None,
-        indices: list[str] | None = None,
+        sample: str | int | None = None,
+        indices: list[int] | None = None,
         batch_size: int = 256,
     ) -> dist.Distribution:
         """
         Computes the aggregated posterior over the ``u`` latent representations.
 
         Parameters
         ----------
         adata
             AnnData object to use. Defaults to the AnnData object used to initialize the model.
+        sample
+            Name or index of the sample to filter on. If None, uses all cells.
         indices
             Indices of cells to use.
         batch_size
             Batch size to use for computing the latent representation.
 
         Returns
         -------
         A mixture distribution of the aggregated posterior.
         """
         self._check_if_trained(warn=False)
         adata = self._validate_anndata(adata)
+        if indices is None:
+            indices = np.arange(self.adata.n_obs)
+        if sample is not None:
+            indices = np.intersect1d(
+                np.array(indices), np.where(adata.obs[self.sample_key] == sample)[0]
+            )
         scdl = self._make_data_loader(
             adata=adata, indices=indices, batch_size=batch_size, iter_ndarray=True
         )
 
         qu_locs = []
         qu_scales = []
         jit_inference_fn = self.module.get_jit_inference_fn(
@@ -740,21 +764,182 @@
         qu_loc = jnp.concatenate(qu_locs, axis=0).T
         qu_scale = jnp.concatenate(qu_scales, axis=0).T
         return dist.MixtureSameFamily(
             dist.Categorical(probs=jnp.ones(qu_loc.shape[1]) / qu_loc.shape[1]),
             dist.Normal(qu_loc, qu_scale),
         )
 
+    def differential_abundance(
+        self,
+        adata: AnnData | None = None,
+        sample_cov_keys: list[str] | None = None,
+        sample_subset: list[str] | None = None,
+        compute_log_enrichment: bool = False,
+        batch_size: int = 128,
+    ) -> xr.Dataset:
+        """
+        Compute the differential abundance between samples.
+
+        Computes the logarithm of the ratio of the probabilities of each sample
+        conditioned on the estimated aggregate posterior distribution of each cell.
+
+        Parameters
+        ----------
+        adata
+            The data object to compute the differential abundance for.
+            If not given, the data object stored in the model is used.
+        sample_cov_keys
+            Keys for covariates (batch, etc.) that should also be taken into account
+            when computing the differential abundance. At the moment, only discrete covariates are supported.
+        sample_subset
+            Only compute differential abundance for these sample labels.
+        compute_log_enrichment
+            Whether to compute the log enrichment scores for each covariate value.
+        batch_size
+            Minibatch size for computing the differential abundance.
+
+        Returns
+        -------
+        :class:`xarray.Dataset`
+            Returns an xarray.Dataset with data variables:
+            - `log_probs`: Array of shape (n_cells, n_samples) containing the log probabilities for each cell across samples.
+            - `{cov_key}_log_probs`: For each key in `sample_cov_keys`, an array of shape (n_cells, n_cov_values) containing the log probabilities for each cell across covariate values.
+        """
+        adata = self._validate_anndata(adata)
+
+        if sample_cov_keys is not None:
+            for key in sample_cov_keys:
+                n_cov_values = len(adata.obs[key].unique())
+                n_samples = len(adata.obs[self.sample_key].unique())
+                if n_cov_values > n_samples / 2:
+                    warnings.warn(
+                        f"The covariate '{key}' does not seem to refer to a discrete key. "
+                        f"It has {len(n_cov_values)} unique values, which exceeds one half of the total samples ({n_samples}).",
+                        UserWarning,
+                        stacklevel=2,
+                    )
+
+        us = self.get_latent_representation(
+            adata, use_mean=True, give_z=False, batch_size=batch_size
+        )
+
+        log_probs = []
+        unique_samples = adata.obs[self.sample_key].unique()
+        for sample_name in tqdm(unique_samples):
+            ap = self.get_aggregated_posterior(
+                adata=adata, sample=sample_name, batch_size=batch_size
+            )
+            n_splits = max(adata.n_obs // batch_size, 1)
+            log_probs_ = []
+            for u_rep in np.array_split(us, n_splits):
+                log_probs_.append(
+                    jax.device_get(ap.log_prob(u_rep).sum(-1, keepdims=True))
+                )
+
+            log_probs.append(np.concatenate(log_probs_, axis=0))  # (n_cells, 1)
+
+        log_probs = np.concatenate(log_probs, 1)
+
+        coords = {
+            "cell_name": adata.obs_names.to_numpy(),
+            "sample": unique_samples,
+        }
+        data_vars = {
+            "log_probs": (["cell_name", "sample"], log_probs),
+        }
+        log_probs_arr = xr.Dataset(data_vars, coords=coords)
+
+        if sample_cov_keys is None or len(sample_cov_keys) == 0:
+            return log_probs_arr
+
+        sample_cov_log_probs_map = {}  # maps sample_cov_key to log_probs dataframe (n_cells, n_cov_values)
+        sample_cov_log_enrichs_map = {}  # maps sample_cov_key to log_enrichs dataframe (n_cells, n_cov_values)
+        for sample_cov_key in sample_cov_keys:
+            sample_cov_unique_values = self.sample_info[sample_cov_key].unique()
+            per_val_log_probs = {}
+            per_val_log_enrichs = {}
+            for sample_cov_value in sample_cov_unique_values:
+                cov_samples = (
+                    self.sample_info[
+                        self.sample_info[sample_cov_key] == sample_cov_value
+                    ]
+                )[self.sample_key].to_numpy()
+                if sample_subset is not None:
+                    cov_samples = np.intersect1d(cov_samples, np.array(sample_subset))
+                if len(cov_samples) == 0:
+                    continue
+
+                sel_log_probs = log_probs_arr.log_probs.loc[{"sample": cov_samples}]
+                val_log_probs = logsumexp(sel_log_probs, axis=1) - np.log(
+                    sel_log_probs.shape[1]
+                )
+                per_val_log_probs[sample_cov_value] = val_log_probs
+
+                if compute_log_enrichment:
+                    rest_samples = np.setdiff1d(unique_samples, cov_samples)
+                    if len(rest_samples) == 0:
+                        warnings.warn(
+                            f"All samples have {sample_cov_key}={sample_cov_value}. Skipping log enrichment computation.",
+                            UserWarning,
+                            stacklevel=2,
+                        )
+                        continue
+                    rest_log_probs = log_probs_arr.log_probs.loc[
+                        {"sample": rest_samples}
+                    ]
+                    rest_val_log_probs = logsumexp(rest_log_probs, axis=1) - np.log(
+                        rest_log_probs.shape[1]
+                    )
+                    enrichment_scores = val_log_probs - rest_val_log_probs
+                    per_val_log_enrichs[sample_cov_value] = enrichment_scores
+            sample_cov_log_probs_map[sample_cov_key] = pd.DataFrame.from_dict(
+                per_val_log_probs
+            )
+            if compute_log_enrichment and len(per_val_log_enrichs) > 0:
+                sample_cov_log_enrichs_map[sample_cov_key] = pd.DataFrame.from_dict(
+                    per_val_log_enrichs
+                )
+
+        coords = {
+            "cell_name": adata.obs_names.to_numpy(),
+            "sample": unique_samples,
+            **{
+                sample_cov_key: sample_cov_log_probs.columns
+                for sample_cov_key, sample_cov_log_probs in sample_cov_log_probs_map.items()
+            },
+        }
+        data_vars = {
+            "log_probs": (["cell_name", "sample"], log_probs),
+            **{
+                f"{sample_cov_key}_log_probs": (
+                    ["cell_name", sample_cov_key],
+                    sample_cov_log_probs.values,
+                )
+                for sample_cov_key, sample_cov_log_probs in sample_cov_log_probs_map.items()
+            },
+        }
+        if compute_log_enrichment:
+            data_vars.update(
+                {
+                    f"{sample_cov_key}_log_enrichs": (
+                        ["cell_name", sample_cov_key],
+                        sample_cov_log_enrichs.values,
+                    )
+                    for sample_cov_key, sample_cov_log_enrichs in sample_cov_log_enrichs_map.items()
+                }
+            )
+        return xr.Dataset(data_vars, coords=coords)
+
     def get_outlier_cell_sample_pairs(
         self,
         adata=None,
         subsample_size: int = 5_000,
         quantile_threshold: float = 0.05,
         admissibility_threshold: float = 0.0,
-        minibatch_size: int = 256,
+        batch_size: int = 256,
     ) -> xr.Dataset:
         """Utils function to get outlier cell-sample pairs.
 
         This function fits a GMM for each sample based on the latent representation
         of the cells in the sample or computes an approximate aggregated posterior for each sample.
         Then, for every cell, it computes the log-probability of the cell under the approximated posterior
         of each sample as a measure of admissibility.
@@ -765,19 +950,18 @@
             AnnData object containing the cells for which to compute the outlier cell-sample pairs.
         subsample_size
             Number of cells to use from each sample to approximate the posterior. If None, uses all of the available cells.
         quantile_threshold
             Quantile of the within-sample log probabilities to use as a baseline for admissibility.
         admissibility_threshold
             Threshold for admissibility. Cell-sample pairs with admissibility below this threshold are considered outliers.
+        batch_size
+            Size of the batch to use for computing outlier cell-sample pairs.
         """
-        adata = self.adata if adata is None else adata
         adata = self._validate_anndata(adata)
-
-        # Compute u reps
         us = self.get_latent_representation(adata, use_mean=True, give_z=False)
         adata.obsm["U"] = us
 
         log_probs = []
         threshs = []
         unique_samples = adata.obs[self.sample_key].unique()
         for sample_name in tqdm(unique_samples):
@@ -788,15 +972,15 @@
                 )
             adata_s = adata[sample_idxs]
 
             ap = self.get_aggregated_posterior(adata=adata, indices=sample_idxs)
             log_probs_s = jnp.quantile(
                 ap.log_prob(adata_s.obsm["U"]).sum(axis=1), q=quantile_threshold
             )
-            n_splits = adata.n_obs // minibatch_size
+            n_splits = adata.n_obs // batch_size
             log_probs_ = []
             for u_rep in np.array_split(adata.obsm["U"], n_splits):
                 log_probs_.append(
                     jax.device_get(ap.log_prob(u_rep).sum(-1, keepdims=True))
                 )
 
             log_probs_ = np.concatenate(log_probs_, axis=0)  # (n_cells, 1)
@@ -821,51 +1005,51 @@
             "is_admissible": (
                 ["cell_name", "sample"],
                 log_ratios > admissibility_threshold,
             ),
         }
         return xr.Dataset(data_vars, coords=coords)
 
-    def perform_multivariate_analysis(
+    def differential_expression(
         self,
         adata: AnnData | None = None,
-        donor_keys: list[tuple] = None,
-        donor_subset: list[str] | None = None,
-        batch_size: int = 256,
+        sample_cov_keys: list[str] | None = None,
+        sample_subset: list[str] | None = None,
+        batch_size: int = 128,
         use_vmap: bool = True,
         normalize_design_matrix: bool = True,
         add_batch_specific_offsets: bool = False,
         mc_samples: int = 100,
         store_lfc: bool = False,
         store_lfc_metadata_subset: list[str] | None = None,
         store_baseline: bool = False,
-        eps_lfc: float = 1e-3,
-        filter_donors: bool = False,
+        eps_lfc: float = 1e-4,
+        filter_inadmissible_samples: bool = False,
         lambd: float = 0.0,
         delta: float | None = 0.3,
-        **filter_donors_kwargs,
+        **filter_samples_kwargs,
     ) -> xr.Dataset:
-        """Utility function to perform cell-specific multivariate analysis.
+        """Utility function to perform cell-specific multivariate differential expression.
 
         For every cell, we first compute all counterfactual cell-state shifts, defined as
-        e_d = z_d - u, where z_d is the latent representation of the cell for donor d and u is the donor-unaware latent representation.
-        Then, we fit a linear model in each cell of the form
-        e_d = X_d * beta_d + iid gaussian noise.
+        e_d = z_d - u, where z_d is the latent representation of the cell for sample d and u
+        is the sample-unaware latent representation. Then, we fit a linear model in each cell
+        of the form: e_d = X_d * beta_d + iid gaussian noise.
 
         Parameters
         ----------
+        sample_cov_keys
+            List of sample covariates to consider for the multivariate analysis.
+            These keys should be present in `adata.obs`.
         adata
             AnnData object to use for computing the local sample representation.
             If None, the analysis is performed on all cells in the dataset.
-        donor_keys
-            List of donor metadata to consider for the multivariate analysis.
-            These keys should be present in `adata.obs`.
-        donor_subset
-            Optional list of donors to consider for the multivariate analysis.
-            If None, all donors are considered.
+        sample_subset
+            Optional list of samples to consider for the multivariate analysis.
+            If None, all samples are considered.
         batch_size
             Batch size to use for computing the local sample representation.
         use_vmap
             Whether to use vmap for computing the local sample representation.
         normalize_design_matrix
             Whether to normalize the design matrix.
         add_batch_specific_offsets
@@ -875,102 +1059,119 @@
             How many MC samples should be taken for computing betas.
         store_lfc
             Whether to store the log-fold changes in the module.
             Storing log-fold changes is memory-intensive and may require to specify
             a smaller set of cells to analyze, e.g., by specifying `adata`.
         store_lfc_metadata_subset
             Specifies a subset of metadata for which log-fold changes are computed.
-            These keys must be a subset of `donor_keys`.
+            These keys must be a subset of `sample_cov_keys`.
             Only applies when `store_lfc=True`.
         store_baseline
             Whether to store the expression in the module if logfoldchanges are computed.
         eps_lfc
             Epsilon to add to the log-fold changes to avoid detecting genes with low expression.
-        filter_donors
-            Whether to filter out-of-distribution donors prior to performing the analysis.
-        filter_donors_kwargs
-            Keyword arguments to pass to `get_outlier_cell_sample_pairs`.
+        filter_inadmissible_samples
+            Whether to filter out-of-distribution samples prior to performing the analysis.
         lambd
             Regularization parameter for the linear model.
         delta
             LFC threshold used to compute posterior DE probabilities.
             If None does not compute them to save memory consumption.
+        filter_samples_kwargs
+            Keyword arguments to pass to `get_outlier_cell_sample_pairs`.
+
+        Returns
+        -------
+        xr.Dataset
+            An xarray Dataset containing the results of the differential expression analysis. The dataset includes:
+            - `beta`: Coefficients for each covariate across cells and latent dimensions.
+            - `effect_size`: Effect sizes for each covariate across cells.
+            - `pvalue`: P-values for each covariate across cells.
+            - `padj`: Adjusted P-values for each covariate across cells using the Benjamini-Hochberg procedure.
+            - `lfc`: Log fold changes for each covariate across cells and genes, if `store_lfc` is True.
+            - `lfc_std`: Standard deviation of log fold changes, if `store_lfc` is True and `delta` is not None.
+            - `pde`: Posterior DE probabilities, if `store_lfc` is True and `delta` is not None.
+            - `baseline_expression`: Baseline expression levels for each covariate across cells and genes, if `store_baseline` is True.
+            - `n_samples`: Number of admissible samples for each cell, if `filter_inadmissible_samples` is True.
         """
+        if sample_cov_keys is None:
+            # Hack: kept as kwarg to maintain order of arguments.
+            raise ValueError("Must assign `sample_cov_keys`")
         adata = self.adata if adata is None else adata
         self._check_if_trained(warn=False)
         # Hack to ensure new AnnDatas have indices and indices have correct dimensions.
         if adata is not None:
             adata.obs["_indices"] = np.arange(adata.n_obs).astype(int)
 
         adata = self._validate_anndata(adata)
         scdl = self._make_data_loader(
             adata=adata, indices=None, batch_size=batch_size, iter_ndarray=True
         )
         n_sample = self.summary_stats.n_sample
         vars_in = {"params": self.module.params, **self.module.state}
 
-        donor_mask = (
-            np.isin(self.sample_order, donor_subset)
-            if donor_subset is not None
+        sample_mask = (
+            np.isin(self.sample_order, sample_subset)
+            if sample_subset is not None
             else np.ones(n_sample, dtype=bool)
         )
-        donor_mask = np.array(donor_mask)
-        donor_order = self.sample_order[donor_mask]
-        n_samples_kept = donor_mask.sum()
-
-        if filter_donors:
-            admissible_donors = self.get_outlier_cell_sample_pairs(
-                adata=adata, **filter_donors_kwargs
-            )["is_admissible"].loc[{"sample": donor_order}]
-            assert (admissible_donors.sample == donor_order).all()
-            admissible_donors = admissible_donors.values
+        sample_mask = np.array(sample_mask)
+        sample_order = self.sample_order[sample_mask]
+        n_samples_kept = sample_mask.sum()
+
+        if filter_inadmissible_samples:
+            admissible_samples = self.get_outlier_cell_sample_pairs(
+                adata=adata, **filter_samples_kwargs
+            )["is_admissible"].loc[{"sample": sample_order}]
+            assert (admissible_samples.sample == sample_order).all()
+            admissible_samples = admissible_samples.values
         else:
-            admissible_donors = np.ones((adata.n_obs, n_samples_kept), dtype=bool)
-        n_admissible_donors = admissible_donors.sum(1)
+            admissible_samples = np.ones((adata.n_obs, n_samples_kept), dtype=bool)
+        n_admissible_samples = admissible_samples.sum(1)
 
         (
             Xmat,
             Xmat_names,
             covariates_require_lfc,
             offset_indices,
         ) = self._construct_design_matrix(
-            donor_keys=donor_keys,
-            donor_mask=donor_mask,
+            sample_cov_keys=sample_cov_keys,
+            sample_mask=sample_mask,
             normalize_design_matrix=normalize_design_matrix,
             add_batch_specific_offsets=add_batch_specific_offsets,
             store_lfc=store_lfc,
             store_lfc_metadata_subset=store_lfc_metadata_subset,
         )
         add_batch_specific_offsets = offset_indices is not None
         n_covariates = Xmat.shape[1]
 
         @partial(jax.jit, backend="cpu")
         def process_design_matrix(
-            admissible_donors_dmat,
+            admissible_samples_dmat,
             Xmat,
         ):
-            xtmx = jnp.einsum("ak,nkl,lm->nam", Xmat.T, admissible_donors_dmat, Xmat)
+            xtmx = jnp.einsum("ak,nkl,lm->nam", Xmat.T, admissible_samples_dmat, Xmat)
             xtmx += lambd * jnp.eye(n_covariates)
 
             prefactor = jnp.real(jax.vmap(jax.scipy.linalg.sqrtm)(xtmx))
             inv_ = jax.vmap(jnp.linalg.pinv)(xtmx)
-            Amat = jnp.einsum("nab,bc,ncd->nad", inv_, Xmat.T, admissible_donors_dmat)
+            Amat = jnp.einsum("nab,bc,ncd->nad", inv_, Xmat.T, admissible_samples_dmat)
             return Amat, prefactor
 
         @partial(jax.jit, static_argnames=["use_mean", "mc_samples"])
         def mapped_inference_fn(
             stacked_rngs,
             x,
             sample_index,
             continuous_covs,
             cf_sample,
             Amat,
             prefactor,
-            n_donors_per_cell,
-            admissible_donors_mat,
+            n_samples_per_cell,
+            admissible_samples_mat,
             use_mean,
             mc_samples,
             rngs_de=None,
         ):
             def inference_fn(
                 rngs,
                 cf_sample,
@@ -993,33 +1194,36 @@
                 )
             else:
 
                 def per_sample_inference_fn(pair):
                     rngs, cf_sample = pair
                     return inference_fn(rngs, cf_sample)
 
-                # eps_ has shape (mc_samples, n_cells, n_donors, n_latent)
+                # eps_ has shape (mc_samples, n_cells, n_samples, n_latent)
                 eps_ = jax.lax.transpose(
                     jax.lax.map(per_sample_inference_fn, (stacked_rngs, cf_sample)),
                     (1, 2, 0, 3),
                 )
             eps_std = eps_.std(axis=2, keepdims=True)
             eps_mean = eps_.mean(axis=2, keepdims=True)
 
-            eps = (eps_ - eps_mean) / (1e-6 + eps_std)  # over donors
+            eps = (eps_ - eps_mean) / (1e-6 + eps_std)  # over samples
             # MLE for betas
             betas = jnp.einsum("nks,ansd->ankd", Amat, eps)
 
             # Statistical tests
             betas_norm = jnp.einsum("ankd,nkl->anld", betas, prefactor)
             ts = (betas_norm**2).mean(axis=0).sum(axis=-1)
-            pvals = 1 - jax.scipy.stats.chi2.cdf(ts, df=n_donors_per_cell[:, None])
+            pvals = 1 - jax.scipy.stats.chi2.cdf(ts, df=n_samples_per_cell[:, None])
 
             betas = betas * eps_std
 
+            lfc_mean = None
+            lfc_std = None
+            pde = None
             if store_lfc:
                 betas_ = betas.transpose((0, 2, 1, 3))
                 eps_mean_ = eps_mean.transpose((0, 2, 1, 3))
                 betas_covariates = betas_[:, covariates_require_lfc, :, :]
 
                 def h_inference_fn(extra_eps, batch_index_cf, batch_offset_eps):
                     extra_eps += batch_offset_eps
@@ -1041,15 +1245,15 @@
                 batch_index_ = jnp.repeat(batch_index_, repeats=n_cells, axis=1)[
                     ..., None
                 ]  # (n_batch, n_cells, 1)
                 betas_null = jnp.zeros_like(betas_covariates)
 
                 if add_batch_specific_offsets:
                     batch_weights = jnp.einsum(
-                        "nd,db->nb", admissible_donors_mat, Xmat[:, offset_indices]
+                        "nd,db->nb", admissible_samples_mat, Xmat[:, offset_indices]
                     ).mean(0)
                     betas_offset_ = betas_[:, offset_indices, :, :] + eps_mean_
                 else:
                     batch_weights = (1.0 / self.summary_stats.n_batch) * jnp.ones(
                         self.summary_stats.n_batch
                     )
                     mc_samples, _, n_cells_, n_latent = betas_covariates.shape
@@ -1078,21 +1282,15 @@
                 lfcs = jnp.log2(x_1 + eps_lfc) - jnp.log2(x_0 + eps_lfc)
                 lfc_mean = jnp.average(lfcs.mean(1), weights=batch_weights, axis=0)
                 if delta is not None:
                     lfc_std = jnp.sqrt(
                         jnp.average(lfcs.var(1), weights=batch_weights, axis=0)
                     )
                     pde = (jnp.abs(lfcs) >= delta).mean(1).mean(0)
-                else:
-                    lfc_std = None
-                    pde = None
-            else:
-                lfc_mean = None
-                lfc_std = None
-                pde = None
+
             if store_baseline:
                 baseline_expression = x_1.mean(1)
             else:
                 baseline_expression = None
             return {
                 "beta": betas.mean(0),
                 "effect_size": ts,
@@ -1110,47 +1308,47 @@
         lfc_std = []
         pde = []
         baseline_expression = []
         for array_dict in tqdm(scdl):
             indices = array_dict[REGISTRY_KEYS.INDICES_KEY].astype(int).flatten()
             n_cells = array_dict[REGISTRY_KEYS.X_KEY].shape[0]
             cf_sample = np.broadcast_to(
-                (np.where(donor_mask)[0])[:, None, None], (n_samples_kept, n_cells, 1)
+                (np.where(sample_mask)[0])[:, None, None], (n_samples_kept, n_cells, 1)
             )
             inf_inputs = self.module._get_inference_input(
                 array_dict,
             )
             continuous_covs = inf_inputs.get(REGISTRY_KEYS.CONT_COVS_KEY, None)
             if continuous_covs is not None:
                 continuous_covs = jnp.array(continuous_covs)
             stacked_rngs = self._generate_stacked_rngs(cf_sample.shape[0])
 
             rngs_de = self.module.rngs if store_lfc else None
-            admissible_donors_mat = jnp.array(
-                admissible_donors[indices]
-            )  # (n_cells, n_donors)
-            n_donors_per_cell = admissible_donors_mat.sum(axis=1)
-            admissible_donors_dmat = jax.vmap(jnp.diag)(admissible_donors_mat).astype(
+            admissible_samples_mat = jnp.array(
+                admissible_samples[indices]
+            )  # (n_cells, n_samples)
+            n_samples_per_cell = admissible_samples_mat.sum(axis=1)
+            admissible_samples_dmat = jax.vmap(jnp.diag)(admissible_samples_mat).astype(
                 float
-            )  # (n_cells, n_donors, n_donors)
-            # element nij is 1 if donor i is admissible and i=j for cell n
-            Amat, prefactor = process_design_matrix(admissible_donors_dmat, Xmat)
+            )  # (n_cells, n_samples, n_samples)
+            # element nij is 1 if sample i is admissible and i=j for cell n
+            Amat, prefactor = process_design_matrix(admissible_samples_dmat, Xmat)
             Amat = jax.device_put(Amat, self.device)
             prefactor = jax.device_put(prefactor, self.device)
 
             res = mapped_inference_fn(
                 stacked_rngs=stacked_rngs,
                 x=jnp.array(inf_inputs["x"]),
                 sample_index=jnp.array(inf_inputs["sample_index"]),
                 continuous_covs=continuous_covs,
                 cf_sample=jnp.array(cf_sample),
                 Amat=Amat,
                 prefactor=prefactor,
-                n_donors_per_cell=n_donors_per_cell,
-                admissible_donors_mat=admissible_donors_mat,
+                n_samples_per_cell=n_samples_per_cell,
+                admissible_samples_mat=admissible_samples_mat,
                 use_mean=False,
                 rngs_de=rngs_de,
                 mc_samples=mc_samples,
             )
             beta.append(np.array(res["beta"]))
             effect_size.append(np.array(res["effect_size"]))
             pvalue.append(np.array(res["pvalue"]))
@@ -1187,18 +1385,18 @@
                 pvalue,
             ),
             "padj": (
                 ["cell_name", "covariate"],
                 padj,
             ),
         }
-        if filter_donors:
-            data_vars["n_donor"] = (
+        if filter_inadmissible_samples:
+            data_vars["n_samples"] = (
                 ["cell_name"],
-                n_admissible_donors,
+                n_admissible_samples,
             )
         if store_lfc:
             if store_lfc_metadata_subset is None and not add_batch_specific_offsets:
                 coords_lfc = ["covariate", "cell_name", "gene"]
             else:
                 coords_lfc = ["covariate_sub", "cell_name", "gene"]
                 coords["covariate_sub"] = (
@@ -1219,36 +1417,36 @@
                 ["covariate", "cell_name", "gene"],
                 baseline_expression,
             )
         return xr.Dataset(data_vars, coords=coords)
 
     def _construct_design_matrix(
         self,
-        donor_keys: list[str],
-        donor_mask: np.ndarray,
+        sample_cov_keys: list[str],
+        sample_mask: np.ndarray,
         normalize_design_matrix: bool,
         add_batch_specific_offsets: bool,
         store_lfc: bool,
         store_lfc_metadata_subset: list[str] | None = None,
     ):
         """
-        Starting from a list of donor keys, construct a design matrix of donors and covariates.
+        Starting from a list of sample covariate keys, construct a design matrix of samples and covariates.
 
         Categorical covariates are one-hot encoded.
         This method returns a tuple of:
         1. The design matrix
         2. A name for each column in the design matrix
-        3. The original donor key for each column in the design matrix
+        3. The original sample key for each column in the design matrix
 
         Parameters
         ----------
-        donor_keys:
-            List of donor metadata to use as covariates.
-        donor_mask:
-            Mask of admissible donors. Must have the same length as the number of donors in the dataset.
+        sample_cov_keys:
+            List of sample metadata to use as covariates.
+        sample_mask:
+            Mask of admissible samples. Must have the same length as the number of samples in the dataset.
         normalize_design_matrix:
             Whether the design matrix should be 0-1 normalized. This is useful to ensure that the
             beta coefficients are comparable across covariates.
         add_batch_specific_offsets:
             Whether the design matrix should be offset. If True, the matrix includes batch-specific
             offsets. This ensures that we can learn perturbation effects that do not depend on batch effects.
 
@@ -1259,42 +1457,42 @@
         2. Names for each column in the design matrix
         3. A mask precising which coefficients from the design matrix require to compute LFCs.
         4. A mask precising which coefficients from the design matrix correspond to offsets.
         """
         Xmat = []
         Xmat_names = []
         Xmat_dim_to_key = []
-        donor_info = self.donor_info.iloc[donor_mask]
-        for donor_key in tqdm(donor_keys):
-            cov = donor_info[donor_key]
+        sample_info = self.sample_info.iloc[sample_mask]
+        for sample_cov_key in tqdm(sample_cov_keys):
+            cov = sample_info[sample_cov_key]
             if (cov.dtype == str) or (cov.dtype == "category"):
                 cov = cov.cat.remove_unused_categories()
                 cov = pd.get_dummies(cov, drop_first=True)
-                cov_names = donor_key + np.array(cov.columns)
+                cov_names = np.array([f"{sample_cov_key}_{col}" for col in cov.columns])
                 cov = cov.values
             else:
-                cov_names = np.array([donor_key])
+                cov_names = np.array([sample_cov_key])
                 cov = cov.values[:, None]
             n_covs = cov.shape[1]
             Xmat.append(cov)
             Xmat_names.append(cov_names)
-            Xmat_dim_to_key.append([donor_key] * n_covs)
+            Xmat_dim_to_key.append([sample_cov_key] * n_covs)
         Xmat_names = np.concatenate(Xmat_names)
         Xmat = np.concatenate(Xmat, axis=1).astype(np.float32)
         Xmat_dim_to_key = np.concatenate(Xmat_dim_to_key)
 
         if normalize_design_matrix:
             Xmat = (Xmat - Xmat.min(axis=0)) / (
                 1e-6 + Xmat.max(axis=0) - Xmat.min(axis=0)
             )
         if add_batch_specific_offsets:
-            cov = donor_info["_scvi_batch"]
+            cov = sample_info["_scvi_batch"]
             if cov.nunique() == self.summary_stats.n_batch:
                 cov = np.eye(self.summary_stats.n_batch)[
-                    donor_info["_scvi_batch"].values
+                    sample_info["_scvi_batch"].values
                 ]
                 cov_names = [
                     "offset_batch_" + str(i) for i in range(self.summary_stats.n_batch)
                 ]
                 Xmat = np.concatenate([cov, Xmat], axis=1)
                 Xmat_names = np.concatenate([np.array(cov_names), Xmat_names])
                 Xmat_dim_to_key = np.concatenate([np.array(cov_names), Xmat_dim_to_key])
@@ -1305,29 +1503,29 @@
                     .loc[cov_names]
                     .values
                 )
                 offset_indices = jnp.array(offset_indices)
             else:
                 warnings.warn(
                     """
-                        Number of batches in donor_info does not match number of batches in summary_stats.
+                        Number of batches in sample_info does not match number of batches in summary_stats.
                         `add_batch_specific_offsets=True` assumes that samples are not shared across batches.
                         Setting `add_batch_specific_offsets=False`...
                     """,
                     stacklevel=2,
                 )
                 offset_indices = None
         else:
             offset_indices = None
 
         Xmat = jnp.array(Xmat)
         if store_lfc:
             covariates_require_lfc = (
                 np.isin(Xmat_dim_to_key, store_lfc_metadata_subset)
                 if store_lfc_metadata_subset is not None
-                else np.isin(Xmat_dim_to_key, donor_keys)
+                else np.isin(Xmat_dim_to_key, sample_cov_keys)
             )
         else:
             covariates_require_lfc = np.zeros(len(Xmat_names), dtype=bool)
         covariates_require_lfc = jnp.array(covariates_require_lfc)
 
         return Xmat, Xmat_names, covariates_require_lfc, offset_indices
```

### Comparing `mrvi-1.0.0b1/src/mrvi/_module.py` & `mrvi-1.0.1/src/mrvi/_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -403,26 +403,20 @@
             ) - generative_outputs["pu"].log_prob(inference_outputs["u"])
             kl_u = kl_u.sum(-1)
         else:
             kl_u = dist.kl_divergence(
                 inference_outputs["qu"], generative_outputs["pu"]
             ).sum(-1)
         inference_outputs["qeps"]
+
+        kl_z = 0.0
         eps = inference_outputs["z"] - inference_outputs["z_base"]
         if self.z_u_prior:
             peps = dist.Normal(0, jnp.exp(self.pz_scale))
             kl_z = -peps.log_prob(eps).sum(-1)
-        else:
-            kl_z = (
-                -dist.Normal(inference_outputs["z_base"], jnp.exp(self.z_u_prior_scale))
-                .log_prob(inference_outputs["z"])
-                .sum(-1)
-                if self.z_u_prior_scale is not None
-                else 0
-            )
 
         weighted_kl_local = kl_weight * (kl_u + kl_z)
         loss = reconstruction_loss + weighted_kl_local
 
         if self.laplace_scale is not None:
             As = inference_outputs["As"]
             n_obs = As.shape[0]
```

### Comparing `mrvi-1.0.0b1/src/mrvi/_types.py` & `mrvi-1.0.1/src/mrvi/_types.py`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/src/mrvi/_utils.py` & `mrvi-1.0.1/src/mrvi/_utils.py`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/tests/test_components.py` & `mrvi-1.0.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/LICENSE` & `mrvi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mrvi-1.0.0b1/pyproject.toml` & `mrvi-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 
 [project]
 name = "mrvi"
-version = "1.0.0b1"
+version = "1.0.1"
 description = "Multi-resolution Variational Inference"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Justin Hong"},
     {name = "Pierre Boyeau"},
     {name = "Adam Gayoso"},
-    {name = "Can Ergan"},
+    {name = "Can Ergen"},
     {name = "Martin Kim"},
 ]
 maintainers = [
     {name = "Justin Hong", email = "justin.hong@columbia.edu"},
     {name = "Pierre Boyeau", email = "pierreboyeau@berkeley.edu"},
     {name = "Martin Kim", email = "martinkim@berkeley.edu"},
 ]
```

