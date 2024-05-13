# Comparing `tmp/pyminufit-0.2.1.tar.gz` & `tmp/pyminufit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed May  8 13:01:50 2024, max compression
+gzip compressed data, last modified: Mon May 13 07:29:32 2024, max compression
```

## Comparing `pyminufit-0.2.1.tar` & `pyminufit-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      326 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.gitattributes
--rw-r--r--   0        0        0     2326 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2764 2024-05-08 13:01:50.000000 pyminufit-0.2.1/noxfile.py
--rw-r--r--   0        0        0     2394 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1121 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1710 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1267 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.github/workflows/pages.yml
--rw-r--r--   0        0        0      953 2024-05-08 13:01:50.000000 pyminufit-0.2.1/docs/conf.py
--rw-r--r--   0        0        0      196 2024-05-08 13:01:50.000000 pyminufit-0.2.1/docs/index.md
--rw-r--r--   0        0        0        6 2024-05-08 13:01:50.000000 pyminufit-0.2.1/docs/examples/.gitignore
--rw-r--r--   0        0        0    72124 2024-05-08 13:01:50.000000 pyminufit-0.2.1/examples/01_simple_fit.png
--rw-r--r--   0        0        0      767 2024-05-08 13:01:50.000000 pyminufit-0.2.1/examples/01_simple_fit.py
--rw-r--r--   0        0        0   108685 2024-05-08 13:01:50.000000 pyminufit-0.2.1/examples/02_add_pdf.png
--rw-r--r--   0        0        0      967 2024-05-08 13:01:50.000000 pyminufit-0.2.1/examples/02_add_pdf.py
--rw-r--r--   0        0        0      192 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/__init__.py
--rw-r--r--   0        0        0      118 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/_version.pyi
--rw-r--r--   0        0        0     5197 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/composites.py
--rw-r--r--   0        0        0     3006 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/models.py
--rw-r--r--   0        0        0     3215 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/observables.py
--rw-r--r--   0        0        0     7125 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/pdf.py
--rw-r--r--   0        0        0     7314 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/plotting.py
--rw-r--r--   0        0        0        0 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/py.typed
--rw-r--r--   0        0        0     1631 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/utils.py
--rw-r--r--   0        0        0      411 2024-05-08 13:01:50.000000 pyminufit-0.2.1/src/pyminufit/version.py
--rw-r--r--   0        0        0      757 2024-05-08 13:01:50.000000 pyminufit-0.2.1/tests/test_models.py
--rw-r--r--   0        0        0     1127 2024-05-08 13:01:50.000000 pyminufit-0.2.1/tests/test_observables.py
--rw-r--r--   0        0        0      175 2024-05-08 13:01:50.000000 pyminufit-0.2.1/tests/test_package.py
--rw-r--r--   0        0        0        0 2024-05-08 13:01:50.000000 pyminufit-0.2.1/tests/test_pdf.py
--rw-r--r--   0        0        0     1097 2024-05-08 13:01:50.000000 pyminufit-0.2.1/tests/test_utils.py
--rw-r--r--   0        0        0     2265 2024-05-08 13:01:50.000000 pyminufit-0.2.1/.gitignore
--rw-r--r--   0        0        0     1515 2024-05-08 13:01:50.000000 pyminufit-0.2.1/LICENSE
--rw-r--r--   0        0        0     3891 2024-05-08 13:01:50.000000 pyminufit-0.2.1/README.md
--rw-r--r--   0        0        0     4089 2024-05-08 13:01:50.000000 pyminufit-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7442 2024-05-08 13:01:50.000000 pyminufit-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      326 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.gitattributes
+-rw-r--r--   0        0        0     2326 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     2764 2024-05-13 07:29:32.000000 pyminufit-0.2.2/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1115 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1710 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1271 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.github/workflows/pages.yml
+-rw-r--r--   0        0        0      953 2024-05-13 07:29:32.000000 pyminufit-0.2.2/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-05-13 07:29:32.000000 pyminufit-0.2.2/docs/index.md
+-rw-r--r--   0        0        0        6 2024-05-13 07:29:32.000000 pyminufit-0.2.2/docs/examples/.gitignore
+-rw-r--r--   0        0        0    72124 2024-05-13 07:29:32.000000 pyminufit-0.2.2/examples/01_simple_fit.png
+-rw-r--r--   0        0        0      767 2024-05-13 07:29:32.000000 pyminufit-0.2.2/examples/01_simple_fit.py
+-rw-r--r--   0        0        0    48174 2024-05-13 07:29:32.000000 pyminufit-0.2.2/examples/02_add_pdf.png
+-rw-r--r--   0        0        0      916 2024-05-13 07:29:32.000000 pyminufit-0.2.2/examples/02_add_pdf.py
+-rw-r--r--   0        0        0      349 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/__init__.py
+-rw-r--r--   0        0        0      118 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/_version.pyi
+-rw-r--r--   0        0        0     5197 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/composites.py
+-rw-r--r--   0        0        0     3183 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/models.py
+-rw-r--r--   0        0        0     3215 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/observables.py
+-rw-r--r--   0        0        0     7182 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/pdf.py
+-rw-r--r--   0        0        0     7382 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/plotting.py
+-rw-r--r--   0        0        0        0 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/py.typed
+-rw-r--r--   0        0        0     1631 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/utils.py
+-rw-r--r--   0        0        0      411 2024-05-13 07:29:32.000000 pyminufit-0.2.2/src/pyminufit/version.py
+-rw-r--r--   0        0        0      757 2024-05-13 07:29:32.000000 pyminufit-0.2.2/tests/test_models.py
+-rw-r--r--   0        0        0     1127 2024-05-13 07:29:32.000000 pyminufit-0.2.2/tests/test_observables.py
+-rw-r--r--   0        0        0      175 2024-05-13 07:29:32.000000 pyminufit-0.2.2/tests/test_package.py
+-rw-r--r--   0        0        0        0 2024-05-13 07:29:32.000000 pyminufit-0.2.2/tests/test_pdf.py
+-rw-r--r--   0        0        0     1097 2024-05-13 07:29:32.000000 pyminufit-0.2.2/tests/test_utils.py
+-rw-r--r--   0        0        0     2265 2024-05-13 07:29:32.000000 pyminufit-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1515 2024-05-13 07:29:32.000000 pyminufit-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4464 2024-05-13 07:29:32.000000 pyminufit-0.2.2/README.md
+-rw-r--r--   0        0        0     4119 2024-05-13 07:29:32.000000 pyminufit-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8045 2024-05-13 07:29:32.000000 pyminufit-0.2.2/PKG-INFO
```

### Comparing `pyminufit-0.2.1/.pre-commit-config.yaml` & `pyminufit-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/noxfile.py` & `pyminufit-0.2.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/.github/CONTRIBUTING.md` & `pyminufit-0.2.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/.github/matchers/pylint.json` & `pyminufit-0.2.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/.github/workflows/cd.yml` & `pyminufit-0.2.2/.github/workflows/cd.yml`

 * *Files 0% similar despite different names*

```diff
@@ -43,10 +43,10 @@
         with:
           name: Packages
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
         if: github.event_name == 'release' && github.event.action == 'published'
         # with:
-          # Remember to tell (test-)pypi about this repo before publishing
-          # Remove this line to publish to PyPI
-          # repository-url: https://test.pypi.org/legacy/
+        # Remember to tell (test-)pypi about this repo before publishing
+        # Remove this line to publish to PyPI
+        # repository-url: https://test.pypi.org/legacy/
```

### Comparing `pyminufit-0.2.1/.github/workflows/ci.yml` & `pyminufit-0.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/.github/workflows/pages.yml` & `pyminufit-0.2.2/.github/workflows/pages.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Simple workflow for deploying static content to GitHub Pages
 name: Deploy static content to Pages
 
 on:
   # Runs on pushes targeting the default branch
-  push:
-    branches: ["main"]
+  # push:
+  #   branches: ["main"]
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
 permissions:
   contents: read
@@ -33,11 +33,11 @@
         uses: actions/checkout@v4
       - name: Setup Pages
         uses: actions/configure-pages@v5
       - name: Upload artifact
         uses: actions/upload-pages-artifact@v3
         with:
           # Upload entire repository
-          path: './docs/_build/html'
+          path: "./docs/_build/html"
       - name: Deploy to GitHub Pages
         id: deployment
         uses: actions/deploy-pages@v4
```

### Comparing `pyminufit-0.2.1/docs/conf.py` & `pyminufit-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/examples/01_simple_fit.png` & `pyminufit-0.2.2/examples/01_simple_fit.png`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/examples/01_simple_fit.py` & `pyminufit-0.2.2/examples/01_simple_fit.py`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/src/pyminufit/composites.py` & `pyminufit-0.2.2/src/pyminufit/composites.py`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/src/pyminufit/models.py` & `pyminufit-0.2.2/src/pyminufit/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Fit models predefined"""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Sequence
+from typing import Any, Dict, Sequence, Union
 
 import numpy as np
 from iminuit import Minuit
 from iminuit.cost import UnbinnedNLL
 from numpy.polynomial.chebyshev import chebval
 from numpy.typing import ArrayLike
 from scipy.stats import norm
 
+from .observables import RealVar
 from .pdf import Pdf
 
+__all__ = ["Gauss", "Normal", "Chebyshev"]
+
 
 class Gauss(Pdf):
     """Standard gaussian"""
 
     def __init__(
         self,
-        observable: Sequence[Any],
-        mean: Sequence[Any] = (-1, 0, 1),
-        sigma: Sequence[Any] = (0, 1),
+        observable: Union[Sequence[Any], RealVar],
+        mean: Union[Sequence[Any], RealVar] = (-1, 0, 1),
+        sigma: Union[Sequence[Any], RealVar] = (0, 1),
         name: str = "gauss",
         *args: Any,
         **kwds: Any,
     ):
         super().__init__(name, *args, **kwds)
 
         self.add_observable(observable)
@@ -46,20 +49,24 @@
         self._update_parameters(m)
         return m
 
     def pdf(self, x, mean, sigma):  # type: ignore[no-untyped-def]
         return norm.pdf(x, mean, sigma)
 
 
+# Add alias
+Normal = Gauss
+
+
 class Chebyshev(Pdf):
     """Chebyshev"""
 
     def __init__(
         self,
-        observable: Sequence[Any],
+        observable: Union[Sequence[Any], RealVar],
         order: int = 2,
         name: str = "chebyshev",
         do_normalize: bool = True,
         *args: Any,
         **kwds: Any,
     ):
         super().__init__(name, *args, **kwds)
```

### Comparing `pyminufit-0.2.1/src/pyminufit/observables.py` & `pyminufit-0.2.2/src/pyminufit/observables.py`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/src/pyminufit/pdf.py` & `pyminufit-0.2.2/src/pyminufit/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,17 +153,19 @@
         return AddPdf([self, other])
 
     def plot(
         self,
         data: ArrayLike,
         filename: Optional[str] = None,
         cfg: Optional[Dict[str, Any]] = None,
+        *args: Any,
+        **kwargs: Any,
     ) -> Plotter:
         """Plot the PDF"""
-        return Plotter(self, data, cfg=cfg).plot(filename=filename)
+        return Plotter(self, data, cfg=cfg).plot(None, filename, *args, **kwargs)
 
     def get(self, parameter: Optional[str] = None, as_ufloat: bool = False) -> Any:
         """Get one of the fitted parameter or print all if None is set
 
         Args:
             parameter (str): name of the parameter
             as_ufloat (bool, optional): If true return ufloat object, else tuple
```

### Comparing `pyminufit-0.2.1/src/pyminufit/plotting.py` & `pyminufit-0.2.2/src/pyminufit/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,19 @@
             if nx > 1:
                 ax = list(ax)
         if not isinstance(ax, list):
             ax = [ax]
         return ax  # type: ignore[no-any-return]
 
     def plot(
-        self, components: Optional[List[str]] = None, filename: Optional[str] = None
+        self,
+        components: Optional[List[str]] = None,
+        filename: Optional[str] = None,
+        *args: Any,
+        **kwargs: Any,
     ) -> Plotter:
         if not components:
             # check if self.model has attribute pdfs
             if hasattr(self.model, "pdfs"):
                 components = [
                     "hist",
                     "pdf",
@@ -139,15 +143,15 @@
                 components = ["hist", "pdf", "axes_labels", "distribution"]
         self.ax = self.setup_axis(None, components)
         for c in components:
             self.parts[c]()
         if len(self.ax) > 1:
             plt.subplots_adjust(hspace=0)
         if filename:
-            plt.savefig(filename, bbox_inches="tight", dpi=300)
+            plt.savefig(filename, *args, **kwargs, bbox_inches="tight")
         return self
 
     def plot_hist(self) -> None:
         self.ax[0].errorbar(self.h.cx, self.h.n, self.h.ne, self.h.dx / 2.0, fmt=".k")
         self.ax[0].set_xlim(min(self.data), max(self.data))
         self.ax[0].set_ylim(0, None)
```

### Comparing `pyminufit-0.2.1/src/pyminufit/utils.py` & `pyminufit-0.2.2/src/pyminufit/utils.py`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/tests/test_models.py` & `pyminufit-0.2.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/tests/test_observables.py` & `pyminufit-0.2.2/tests/test_observables.py`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/tests/test_utils.py` & `pyminufit-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/.gitignore` & `pyminufit-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/LICENSE` & `pyminufit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyminufit-0.2.1/README.md` & `pyminufit-0.2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -29,20 +29,25 @@
 This package is an interface to `iminuit` to allow for fast simple fits and
 mimics the functionality of `PyrooFit` which is an interface on top of the
 ROOT.RooFit package.
 
 The package allows for simple fits of standard PDFs and easy setup of custom
 PDFs in one or more fit dimensions.
 
-## Links
-| Description | Link |
-|-------------|------|
-| Documentation | [pyminufit Documentation][rtd-link] |
+### Links
+
+| Description       | Link                                        |
+| ----------------- | ------------------------------------------- |
+| Documentation     | [pyminufit Documentation][rtd-link]         |
 | GitHub Repository | [pyminufit GitHub Repository][actions-link] |
 
+This package is based on top of [iminuit](https://scikit-hep.org/iminuit/). For
+more information, you can refer to the
+[iminuit documentation](https://iminuit.readthedocs.io/en/latest/).
+
 ## Example
 
 Simple fit and plot of a Gaussian Distribution:
 
 ```python
 from pyminufit.models import Gauss
 import numpy as np
@@ -58,66 +63,82 @@
 pdf.get()
 ```
 
 A more complex example on combination of Gauss pdf for signal and Polynomial for
 background:
 
 ```python
-from pyminufit.models import Gauss, Chebychev
-import numpy as np
-import pandas as pd
-import ROOT
-
-
-from pyminufit.models import Gauss, Chebyshev
-from pyminufit.observables import create_real_var
+import pyminufit as mnf
 import numpy as np
 
-
 data = np.append(
     np.random.random_sample(1000) * 10 + 745, np.random.normal(750, 1, 1000)
 )
 
-x = create_real_var(("mass", 745, 755), unit="GeV")
+x = mnf.create_real_var(("mass", 745, 755), unit="GeV")
 
-pdf_sig = Gauss(x, mean=(745, 755), sigma=(0.1, 1, 2), title="Signal")
-pdf_bkg = Chebyshev(x, order=2, title="Background")
+pdf_sig = mnf.Gauss(x, mean=(745, 755), sigma=(0.1, 1, 2), title="Signal")
+pdf_bkg = mnf.Chebyshev(x, order=2, title="Background")
 
 pdf = pdf_sig + pdf_bkg
 
 pdf.fit(data)
-pdf.plot(data, "02_add_pdf.png")
+pdf.plot(data, "02_add_pdf.png", dpi=150)
 pdf.get()
 ```
 
-<img src="./examples/02_add_pdf.png" width="400" height="400" alt="Fitting multiple pdf to data.">
+![Fitting multiple pdf to data.](./examples/02_add_pdf.png)
 
 Observables can be initialised by a list or tuple with the column name /
 variable name as first argument, followed by the range and/or with the initial
 value and range:
 
 ```
 x = ('x', -3, 3)
 x = ('mass', -3, 0.02, 3)
 ```
 
 Parameters are initialised with a tuple: `sigma=(0,1)` or again including a
 starting parameter: `sigma=(0.01, 0, 1)` The order here is not important.
 
-# Installation
+## Installation
 
-(will be accessible via pip soon)
+You can install `pyminufit` directly from PyPI using pip:
 
+```bash
+pip install pyminufit
 ```
-pip install -e .
+
+Alternatively, if you want to install the development version directly from
+GitHub, you can do so with:
+
+```bash
+pip install git+https://github.com/simonuu/pyminufit.git
 ```
 
+For a development installation, download the git reposityro and run:
 
-# Development
+```bash
+pip install -e .
+```
 
-If you have any questions or need help with this package, your contributions are greatly appreciated. This project is a side project, so any assistance is welcome. When contributing, please follow design principles that prioritize simplicity of the interface while preserving the complexity of the underlying functionality. You can contribute by submitting a pull request (PR) to the GitHub repository. For larger changes consider discussing ideas in GitHub Issues. Thank you for your support!
+## Development
 
+If you have any questions or need help with this package, your contributions are
+greatly appreciated. This project is a side project, so any assistance is
+welcome. When contributing, please follow design principles that prioritize
+simplicity of the interface while preserving the complexity of the underlying
+functionality. You can contribute by submitting a pull request (PR) to the
+GitHub repository. For larger changes consider discussing ideas in GitHub
+Issues. Thank you for your support!
+
+## Planned Features
+
+- [ ] ProdPdf: Product pdf for multiple observables
+- [ ] Convolutions
+- [ ] Shared parameters
+- [ ] Backend options for the pdf calculation
 
 ---
 
 This package was created using the scientific python template from
 https://scientific-python.org/.
```

### Comparing `pyminufit-0.2.1/pyproject.toml` & `pyminufit-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 [project]
 name = "pyminufit"
 authors = [
   { name = "Simon", email = "simon@gmail.com" },
 ]
-description = "A great package."
+description = "A Python package for fitting data with iMinuit"
 readme = "README.md"
 license.file = "LICENSE"
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
```

### Comparing `pyminufit-0.2.1/PKG-INFO` & `pyminufit-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: pyminufit
-Version: 0.2.1
-Summary: A great package.
+Version: 0.2.2
+Summary: A Python package for fitting data with iMinuit
 Project-URL: Homepage, https://github.com/SimonUU/pyminufit
 Project-URL: Bug Tracker, https://github.com/SimonUU/pyminufit/issues
 Project-URL: Discussions, https://github.com/SimonUU/pyminufit/discussions
 Project-URL: Changelog, https://github.com/SimonUU/pyminufit/releases
 Author-email: Simon <simon@gmail.com>
 License: BSD 3-Clause License
         
@@ -103,20 +103,25 @@
 This package is an interface to `iminuit` to allow for fast simple fits and
 mimics the functionality of `PyrooFit` which is an interface on top of the
 ROOT.RooFit package.
 
 The package allows for simple fits of standard PDFs and easy setup of custom
 PDFs in one or more fit dimensions.
 
-## Links
-| Description | Link |
-|-------------|------|
-| Documentation | [pyminufit Documentation][rtd-link] |
+### Links
+
+| Description       | Link                                        |
+| ----------------- | ------------------------------------------- |
+| Documentation     | [pyminufit Documentation][rtd-link]         |
 | GitHub Repository | [pyminufit GitHub Repository][actions-link] |
 
+This package is based on top of [iminuit](https://scikit-hep.org/iminuit/). For
+more information, you can refer to the
+[iminuit documentation](https://iminuit.readthedocs.io/en/latest/).
+
 ## Example
 
 Simple fit and plot of a Gaussian Distribution:
 
 ```python
 from pyminufit.models import Gauss
 import numpy as np
@@ -132,66 +137,82 @@
 pdf.get()
 ```
 
 A more complex example on combination of Gauss pdf for signal and Polynomial for
 background:
 
 ```python
-from pyminufit.models import Gauss, Chebychev
-import numpy as np
-import pandas as pd
-import ROOT
-
-
-from pyminufit.models import Gauss, Chebyshev
-from pyminufit.observables import create_real_var
+import pyminufit as mnf
 import numpy as np
 
-
 data = np.append(
     np.random.random_sample(1000) * 10 + 745, np.random.normal(750, 1, 1000)
 )
 
-x = create_real_var(("mass", 745, 755), unit="GeV")
+x = mnf.create_real_var(("mass", 745, 755), unit="GeV")
 
-pdf_sig = Gauss(x, mean=(745, 755), sigma=(0.1, 1, 2), title="Signal")
-pdf_bkg = Chebyshev(x, order=2, title="Background")
+pdf_sig = mnf.Gauss(x, mean=(745, 755), sigma=(0.1, 1, 2), title="Signal")
+pdf_bkg = mnf.Chebyshev(x, order=2, title="Background")
 
 pdf = pdf_sig + pdf_bkg
 
 pdf.fit(data)
-pdf.plot(data, "02_add_pdf.png")
+pdf.plot(data, "02_add_pdf.png", dpi=150)
 pdf.get()
 ```
 
-<img src="./examples/02_add_pdf.png" width="400" height="400" alt="Fitting multiple pdf to data.">
+![Fitting multiple pdf to data.](./examples/02_add_pdf.png)
 
 Observables can be initialised by a list or tuple with the column name /
 variable name as first argument, followed by the range and/or with the initial
 value and range:
 
 ```
 x = ('x', -3, 3)
 x = ('mass', -3, 0.02, 3)
 ```
 
 Parameters are initialised with a tuple: `sigma=(0,1)` or again including a
 starting parameter: `sigma=(0.01, 0, 1)` The order here is not important.
 
-# Installation
+## Installation
 
-(will be accessible via pip soon)
+You can install `pyminufit` directly from PyPI using pip:
 
+```bash
+pip install pyminufit
 ```
-pip install -e .
+
+Alternatively, if you want to install the development version directly from
+GitHub, you can do so with:
+
+```bash
+pip install git+https://github.com/simonuu/pyminufit.git
 ```
 
+For a development installation, download the git reposityro and run:
 
-# Development
+```bash
+pip install -e .
+```
 
-If you have any questions or need help with this package, your contributions are greatly appreciated. This project is a side project, so any assistance is welcome. When contributing, please follow design principles that prioritize simplicity of the interface while preserving the complexity of the underlying functionality. You can contribute by submitting a pull request (PR) to the GitHub repository. For larger changes consider discussing ideas in GitHub Issues. Thank you for your support!
+## Development
 
+If you have any questions or need help with this package, your contributions are
+greatly appreciated. This project is a side project, so any assistance is
+welcome. When contributing, please follow design principles that prioritize
+simplicity of the interface while preserving the complexity of the underlying
+functionality. You can contribute by submitting a pull request (PR) to the
+GitHub repository. For larger changes consider discussing ideas in GitHub
+Issues. Thank you for your support!
+
+## Planned Features
+
+- [ ] ProdPdf: Product pdf for multiple observables
+- [ ] Convolutions
+- [ ] Shared parameters
+- [ ] Backend options for the pdf calculation
 
 ---
 
 This package was created using the scientific python template from
 https://scientific-python.org/.
```

