# Comparing `tmp/astrodata-2.9.1.dev1.tar.gz` & `tmp/astrodata-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrodata-2.9.1.dev1.tar", max compression
+gzip compressed data, was "astrodata-2.9.2.tar", max compression
```

## Comparing `astrodata-2.9.1.dev1.tar` & `astrodata-2.9.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     5270 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/README.rst
--rw-r--r--   0        0        0      756 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/.readthedocs.yaml
--rw-r--r--   0        0        0     2321 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/__init__.py
--rw-r--r--   0        0        0     8180 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/adfactory.py
--rw-r--r--   0        0        0    49485 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/core.py
--rw-r--r--   0        0        0      245 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/data/README.rst
--rw-r--r--   0        0        0    38531 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/fits.py
--rw-r--r--   0        0        0    20953 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/nddata.py
--rw-r--r--   0        0        0    11833 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/provenance.py
--rw-r--r--   0        0        0    34488 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/testing.py
--rw-r--r--   0        0        0    12869 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/utils.py
--rw-r--r--   0        0        0    39849 2024-03-19 20:11:53.817868 astrodata-2.9.1.dev1/astrodata/wcs.py
--rw-r--r--   0        0        0     2401 2024-03-19 20:12:11.577874 astrodata-2.9.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     5994 1970-01-01 00:00:00.000000 astrodata-2.9.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1826 2024-05-13 19:19:04.316784 astrodata-2.9.2/LICENSE
+-rw-r--r--   0        0        0     6804 2024-05-13 19:19:04.316784 astrodata-2.9.2/README.md
+-rw-r--r--   0        0        0      756 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/.readthedocs.yaml
+-rw-r--r--   0        0        0     2322 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/__init__.py
+-rw-r--r--   0        0        0     8181 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/adfactory.py
+-rw-r--r--   0        0        0    49486 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/core.py
+-rw-r--r--   0        0        0      245 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/data/README.rst
+-rw-r--r--   0        0        0    38532 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/fits.py
+-rw-r--r--   0        0        0    20952 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/nddata.py
+-rw-r--r--   0        0        0    11834 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/provenance.py
+-rw-r--r--   0        0        0    35495 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/testing.py
+-rw-r--r--   0        0        0    12870 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/utils.py
+-rw-r--r--   0        0        0    40692 2024-05-13 19:19:04.316784 astrodata-2.9.2/astrodata/wcs.py
+-rw-r--r--   0        0        0     2477 2024-05-13 19:19:21.180851 astrodata-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0     7526 1970-01-01 00:00:00.000000 astrodata-2.9.2/PKG-INFO
```

### Comparing `astrodata-2.9.1.dev1/astrodata/.readthedocs.yaml` & `astrodata-2.9.2/astrodata/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `astrodata-2.9.1.dev1/astrodata/__init__.py` & `astrodata-2.9.2/astrodata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """This package adds an abstraction layer to astronomical data by parsing the
 information contained in the headers as attributes. To do so, one must subclass
 :class:`astrodata.AstroData` and add parse methods accordingly to the
 :class:`~astrodata.TagSet` received.
 
 """
+
 from .core import AstroData
 from .adfactory import AstroDataFactory, AstroDataError
 from .fits import add_header_to_table
 from .nddata import NDAstroData, AstroDataMixin
 from .utils import (
     Section,
     TagSet,
```

### Comparing `astrodata-2.9.1.dev1/astrodata/adfactory.py` & `astrodata-2.9.2/astrodata/adfactory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Factory for AstroData objects."""
+
 import copy
 import logging
 import os
 from contextlib import contextmanager
 from copy import deepcopy
 
 from astropy.io import fits
```

### Comparing `astrodata-2.9.1.dev1/astrodata/core.py` & `astrodata-2.9.2/astrodata/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This is the core module of the AstroData package. It provides the
 `AstroData` class, which is the main interface to manipulate astronomical
 data sets.
 """
+
 import inspect
 import logging
 import os
 import re
 import textwrap
 import warnings
 from collections import OrderedDict
```

### Comparing `astrodata-2.9.1.dev1/astrodata/fits.py` & `astrodata-2.9.2/astrodata/fits.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .. |NDData| replace:: :class:`~astropy.nddata.NDData`
 .. |NDDataRef| replace:: :class:`~astropy.nddata.NDDataRef`
 .. |BinTableHDU| replace:: :class:`~astropy.io.fits.BinTableHDU`
 .. |TableHDU| replace:: :class:`~astropy.io.fits.TableHDU`
 .. |NDAstroData| replace:: :class:`~astrodata.nddata.NDAstroData`
 .. |NDAstroDataRef| replace:: :class:`~astrodata.nddata.NDAstroDataRef`
 """
+
 from collections import OrderedDict
 from copy import deepcopy
 from io import BytesIO
 from itertools import product as cart_product, zip_longest
 import gc
 import logging
 import os
```

### Comparing `astrodata-2.9.1.dev1/astrodata/nddata.py` & `astrodata-2.9.2/astrodata/nddata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """This module implements a derivative class based on NDData with some Mixins,
 implementing windowing and on-the-fly data scaling.
 """
 
-
 import warnings
 from copy import deepcopy
 from functools import reduce
 
 import numpy as np
 
 from astropy.io.fits import ImageHDU
```

### Comparing `astrodata-2.9.1.dev1/astrodata/provenance.py` & `astrodata-2.9.2/astrodata/provenance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Provides functions for adding provenance information to
 `~astrodata.core.AstroData` objects.
 """
+
 from datetime import datetime
 import json
 
 from astropy.table import Table
 
 
 def add_provenance(ad, filename, md5, primitive, timestamp=None):
```

### Comparing `astrodata-2.9.1.dev1/astrodata/testing.py` & `astrodata-2.9.2/astrodata/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # pragma: no cover
-"""Fixtures to be used in tests in DRAGONS
-"""
+"""Fixtures to be used in tests in DRAGONS"""
+
+import enum
 import functools
 import io
+import itertools
+import logging
 import os
+import re
 import shutil
-import tempfile
+import subprocess
 import unittest
 import urllib
 import warnings
 import xml.etree.ElementTree as et
 
 from astropy.io import fits
 from astropy.table import Table
@@ -26,26 +30,89 @@
 # from gempy.library import astrotools as at
 
 GEMINI_ARCHIVE_URL = "https://archive.gemini.edu/file/"
 
 # numpy random number generator for consistency.
 _RANDOM_NUMBER_GEN = np.random.default_rng(42)
 
+log = logging.getLogger(__name__)
+
+
+class DownloadResult(enum.Enum):
+    SUCCESS = 2
+    NOT_FOUND = 1
+    NONE = 0
+
+
+class DownloadState:
+    """Singleton class to hold the state of the download_from_archive function.
+    A bit of an annoying workaround because of conflicts with how ``pytest``'s
+    fixtures work.
+
+    The class is meant to be used as a singleton, so it should not be
+    instantiated directly. Instead, the instance should be accessed via the
+    ``_self`` variable. Instantiation using ``_DownloadState()`` will do this
+    automatically.
+    """
+
+    __slots__ = ["_state", "_valid_state", "test_result"]
+
+    _instance = None
+
+    def __new__(cls):
+        if cls._instance is None:
+            cls._instance = super().__new__(cls)
+            cls._instance._state = None
+            cls._instance._valid_state = False
+            cls._instance.test_result = None
+
+        return cls._instance
+
+    def check_state(self) -> DownloadResult:
+        """Check the state of the download_from_archive function."""
+        SUCCESS = DownloadResult.SUCCESS
+        NOT_FOUND = DownloadResult.NOT_FOUND
+        NONE = DownloadResult.NONE
+
+        if self._state is not NONE and self._valid_state:
+            return self._state
+
+        # Test if downloads are possible
+        try:
+            self.test_result = download_from_archive(
+                "test.fits", cache=False, fail_on_error=True
+            )
+
+        except IOError:
+            self._state = NOT_FOUND
+
+        else:
+            self._state = SUCCESS if self.test_result else NOT_FOUND
+
+        self._valid_state = True
+        return self._state
+
+    def invalidate_cache(self):
+        """Invalidate the cache of the download state."""
+        self._valid_state = False
+
 
 def skip_if_download_none(func):
     """Skip test if download_from_archive is returning None. Otherwise,
     continue.
 
     Used as a wrapper for testing functions. Works with nose, pynose, and
     pytest.
     """
+    if not callable(func):
+        raise TypeError("Argument must be a callable")
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
-        if download_from_archive("N20160727S0077.fits") is None:
+        if DownloadState().check_state() is DownloadResult.NOT_FOUND:
             raise unittest.SkipTest(
                 "Skipping test because download_from_archive returned None"
             )
 
         return func(*args, **kwargs)
 
     return wrapper
@@ -65,14 +132,17 @@
     (11/2/2023)
 
     This is required for a couple of the legacy tests.
     """
     if not isinstance(shape, tuple):
         raise TypeError("get_corners argument is non-tuple")
 
+    if not shape:
+        raise ValueError("get_corners argument is empty")
+
     if len(shape) == 1:
         corners = [(0,), (shape[0] - 1,)]
     else:
         size = len(shape)
         shape_less1 = shape[1:size]
         corners_less1 = get_corners(shape_less1)
         corners = []
@@ -261,37 +331,50 @@
         model1 = [model1]
         model2 = [model2]
 
     # Compare the constituent model definitions:
     for m1, m2 in zip(model1, model2):
         assert type(m1) is type(m2)
         assert len(m1.parameters) == len(m2.parameters)
+
         # NB. For 1D models the degrees match if the numbers of parameters do
         if hasattr(m1, "x_degree"):
             assert m1.x_degree == m2.x_degree
+
         if hasattr(m1, "y_degree"):
             assert m1.y_degree == m2.y_degree
+
         if hasattr(m1, "domain"):
             assert m1.domain == m2.domain
+
         if hasattr(m1, "x_domain"):
             assert m1.x_domain == m2.x_domain
+
         if hasattr(m1, "y_domain"):
             assert m1.y_domain == m2.y_domain
 
+    # Return from lists if need be.
+    if model1[0].n_submodels == 1 and len(model1) == 1:
+        model1 = model1[0]
+        model2 = model2[0]
+
     # Compare the model parameters (coefficients):
     assert_allclose(model1.parameters, model2.parameters, rtol=rtol, atol=atol)
 
     # Now check for any inverse models and require them both to have the same
     # type or be undefined:
     try:
         inverse1 = model1.inverse
+
     except NotImplementedError:
         inverse1 = None
+
     try:
         inverse2 = model2.inverse
+
     except NotImplementedError:
         inverse2 = None
 
     assert type(inverse1) is type(inverse2)
 
     # Compare inverses only if they exist and are not the forward model itself:
     if inverse1 is None or (inverse1 is model1 and inverse2 is model2):
@@ -301,15 +384,20 @@
     if check_inverse:
         compare_models(
             inverse1, inverse2, rtol=rtol, atol=atol, check_inverse=False
         )
 
 
 def download_from_archive(
-    filename, path=None, sub_path="raw_files", env_var="ASTRODATA_TEST"
+    filename,
+    path=None,
+    sub_path="raw_files",
+    env_var="ASTRODATA_TEST",
+    cache=True,
+    fail_on_error=True,
 ):
     """Download file from the archive and store it in the local cache.
 
     Parameters
     ----------
     filename : str
         The filename, e.g. N20160524S0119.fits
@@ -322,63 +410,89 @@
     sub_path : str
         By default the file is stored at the root of the cache directory, but
         using ``path`` allows to specify a sub-directory.
 
     env_var: str
         Environment variable containing the path to the cache directory.
 
+    cache : bool
+        If False, the file is downloaded and replaced in the cache directory.
+
+    fail_on_error : bool
+        If True, raise an error if the download fails. If False, return None.
+
     Returns
     -------
     str
         Name of the cached file with the path added to it.
     """
+    # Handle None sub_path
+    if sub_path is None:
+        sub_path = ""
+        warnings.warn(
+            "sub_path is None, so the file will be saved to the root of the "
+            "cache directory. To suppress this warning, set sub_path to a "
+            "valid path (e.g., empty string)."
+        )
+
     # Check that the environment variable is a valid name.
     if not isinstance(env_var, str) or not env_var.isidentifier():
         raise ValueError(f"Environment variable name is not valid: {env_var}")
 
     # Find cache path and make sure it exists
     root_cache_path = os.getenv(env_var)
 
     if root_cache_path is None:
-        root_cache_path = os.path.join(os.getcwd(), "_test_cache")
-        warnings.warn(
-            f"Environment variable not set: {env_var}, writing "
-            f"to {root_cache_path}. To suppress this warning, set "
-            f"the environment variable {env_var} to the desired path "
-            f"for the testing cache."
-        )
+        if path is not None:
+            root_cache_path = os.path.expanduser(path)
 
-        # This is cleaned up once the program finishes.
-        os.environ[env_var] = str(root_cache_path)
+        else:
+            root_cache_path = os.path.join(os.getcwd(), "_test_cache")
+            warnings.warn(
+                f"Environment variable not set: {env_var}, writing "
+                f"to {root_cache_path}. To suppress this warning, set "
+                f"the environment variable {env_var} to the desired path "
+                f"for the testing cache."
+            )
+
+            # This is cleaned up once the program finishes.
+            os.environ[env_var] = str(root_cache_path)
 
     root_cache_path = os.path.expanduser(root_cache_path)
 
-    if sub_path is not None:
-        cache_path = os.path.join(root_cache_path, sub_path)
+    if path is None:
+        path = root_cache_path
 
-    if path is not None:
-        path = os.path.expanduser(path)
-        cache_path = os.path.join(path, sub_path)
+    cache_path = os.path.join(os.path.expanduser(path), sub_path)
 
     if not os.path.exists(cache_path):
         os.makedirs(cache_path)
 
     # Now check if the local file exists and download if not
     try:
         local_path = os.path.join(cache_path, filename)
         url = GEMINI_ARCHIVE_URL + filename
-        if not os.path.exists(local_path):
-            tmp_path = download_file(url, cache=False)
 
-            shutil.move(tmp_path, local_path)
+        if cache and os.path.exists(local_path):
+            # Use the cached file
+            return local_path
+
+        tmp_path = download_file(url, cache=False)
+
+        shutil.move(tmp_path, local_path)
 
-            # `download_file` ignores Access Control List - fixing it
-            os.chmod(local_path, 0o664)
+        # `download_file` ignores Access Control List - fixing it
+        os.chmod(local_path, 0o664)
 
     except Exception as err:
+        if not fail_on_error:
+            log.debug(f"Failed to download {filename} from the archive")
+            log.debug(f" - Error: {err}")
+            return None
+
         raise IOError(
             f"Failed to download {filename} from the archive ({url})"
         ) from err
 
     return local_path
 
 
@@ -604,24 +718,32 @@
                     if v1 != v2:
                         errorlist.append(f"{kw} value inequality: {v1} v {v2}")
 
         return errorlist
 
     def refcat(self):
         """Check both ADs have REFCATs (or not) and that the lengths agree"""
-        refcat1 = getattr(self.ad1, "REFCAT", None)
-        refcat2 = getattr(self.ad2, "REFCAT", None)
+        # REFCAT can be in the PHU or the AD itself, depending on if REFCAT is
+        # implemented as a property/attr or not in the parent class.
+        refcat1 = getattr(self.ad1.phu, "REFCAT", None)
+        refcat2 = getattr(self.ad2.phu, "REFCAT", None)
+
+        # Check if only one is missing
         if (refcat1 is None) ^ (refcat2 is None):
             return [f"presence: {refcat1 is not None} v {refcat2 is not None}"]
 
+        # Match the lengths
         if refcat1 is not None:  # and refcat2 must also exist
             len1, len2 = len(refcat1), len(refcat2)
             if len1 != len2:
                 return [f"lengths: {len1} v {len2}"]
 
+        # TODO: Should we check the contents of the REFCATs? Or is that checked
+        # elsewhere/by some other method/equality impl?
+
         return []
 
     def attributes(self):
         """Check extension-level attributes"""
         errorlist = []
         for i, (ext1, ext2) in enumerate(zip(self.ad1, self.ad2)):
             elist = self._attributes(ext1, ext2)
@@ -631,57 +753,22 @@
 
     def _attributes(self, ext1, ext2):
         """Helper method for checking attributes"""
         errorlist = []
         for attr in ["data", "mask", "variance", "OBJMASK", "OBJCAT"]:
             attr1 = getattr(ext1, attr, None)
             attr2 = getattr(ext2, attr, None)
-            if (attr1 is None) ^ (attr2 is None):
-                errorlist.append(
-                    f"Attribute error for {attr}: "
-                    f"{attr1 is not None} v {attr2 is not None}"
-                )
-            elif attr1 is not None:
-                if isinstance(attr1, Table):
-                    if len(attr1) != len(attr2):
-                        errorlist.append(
-                            f"attr lengths differ: "
-                            f"{len(attr1)} v {len(attr2)}"
-                        )
-                else:  # everything else is pixel-like
-                    if attr1.dtype.name != attr2.dtype.name:
-                        errorlist.append(
-                            f"Datatype mismatch for {attr}: "
-                            f"{attr1.dtype} v {attr2.dtype}"
-                        )
-                    if attr1.shape != attr2.shape:
-                        errorlist.append(
-                            f"Shape mismatch for {attr}: "
-                            f"{attr1.shape} v {attr2.shape}"
-                        )
-                    if "int" in attr1.dtype.name:
-                        try:
-                            assert_most_equal(
-                                attr1, attr2, max_miss=self.max_miss
-                            )
-                        except AssertionError as e:
-                            errorlist.append(
-                                f"Inequality for {attr}: " + str(e)
-                            )
-                    else:
-                        try:
-                            assert_most_close(
-                                attr1,
-                                attr2,
-                                max_miss=self.max_miss,
-                                rtol=self.rtol,
-                                atol=self.atol,
-                            )
-                        except AssertionError as e:
-                            errorlist.append(f"Mismatch for {attr}: " + str(e))
+
+            if all(attr is None for attr in [attr1, attr2]):
+                continue
+
+            if not np.array_equal(attr1, attr2):
+                errorlist.append(f"{attr} mismatch: {attr1} v {attr2}")
+                continue
+
         return errorlist
 
     def wcs(self):
         """Check WCS agrees"""
 
         def compare_frames(frame1, frame2):
             """Compare the important stuff of two CoordinateFrame instances"""
@@ -762,16 +849,21 @@
     ad2: AstroData
         second AD object
 
     Returns
     -------
     bool: are the two AD instances basically the same?
     """
-    compare = ADCompare(ad1, ad2).run_comparison(**kwargs)
-    return not compare
+    try:
+        ADCompare(ad1, ad2).run_comparison(**kwargs)
+
+    except AssertionError:
+        return False
+
+    return True
 
 
 _HDUL_LIKE_TYPE = fits.HDUList | list[fits.hdu.FitsHDU]
 
 
 def fake_fits_bytes(
     hdus: _HDUL_LIKE_TYPE | None = None,
@@ -928,166 +1020,149 @@
         hdus.writeto(file_data)
 
     file_data.seek(0)
 
     return file_data
 
 
-def create_test_file(
-    path: os.PathLike | None = None,
-    hdus: _HDUL_LIKE_TYPE | None = None,
-    n_extensions: int = 1,
-    image_shape: tuple[int, int] | None = None,
-    include_header_keys: Iterable[str] | None = None,
-    file_type: str = "fits",
-) -> str:
-    """Create a temporary file of a given type and return a path to the file.
+def test_script_file(
+    script_path: os.PathLike | str,
+    stdout_result: str | None = None,
+    stderr_result: str | None = None,
+    python_options: str | list[str] = "",
+    script_options: str | list[str] = "",
+    fail_on_error: bool = True,
+    break_after_run: bool = False,
+    regex_options: re.RegexFlag = re.MULTILINE | re.DOTALL,
+) -> bool:
+    """Run a script file and check the output.
 
-    Arguments
-    ---------
-    path : os.PathLike | None
-        The path to the file to be created. If None, a temporary file is
-        created.
+    All matches (i.e., stdout_result and stderr_result) can use regular
+    expressions.
 
-    hdus : HDUList | list[HDUBase] | None
-        The HDUList or list of HDUBase objects to be written to the file.  If
-        None, a file with a primary HDU and n_extension extension HDUs are
-        generated.
+    Parameters
+    ----------
+    script_path : str
+        The path to the script to be run.
 
-    n_extensions : int
-        The number of extension HDUs to be created if hdus is None.
-        Default is 1 (primary HDU + single extension)
+    stdout_result : str | None
+        The expected result from the standard output. If None, the standard
+        output is not checked.
+
+    stderr_result : str | None
+        The expected result from the standard error. If None, the standard
+        error is not checked.
+
+    python_options : str | list[str]
+        Options to be passed to the python interpreter when running the script.
+
+    script_options : str | list[str]
+        Options to be passed to the script when running it.
+
+    fail_on_error : bool
+        If True, an AssertionError is raised if the output does not match the
+        expected results.
+
+    break_after_run : bool
+        If True, the script will pause at the end before closing, and escape
+        using the built-in `breakpoint()` function.
+
+    regex_options : re.RegexFlag
+        The regular expression flags to be used when matching the output.
+        The default is re.MULTILINE | re.DOTALL.
 
-    image_shape : tuple[int, int] | None
-        The shape of the image to be created in the primary HDU. If None, no
-        image is created.
+    Returns
+    -------
+    bool
+        True if the output matches the expected results.
 
-    include_header_keys : Iterable[str] | None
-        A list of header keywords to be included in the primary HDU. If None,
-        no header keywords are included.
+    Raises
+    ------
+    FileNotFoundError
+        If the script file is not found.
 
-    file_type : str
-        The type of file to be created. Default is 'fits'.
-    """
-    if file_type.casefold() == "fits":
-        file_data = fake_fits_bytes(
-            hdus=hdus,
-            n_extensions=n_extensions,
-            image_shape=image_shape,
-            include_header_keys=include_header_keys,
-        )
+    subprocess.CalledProcessError
+        If the script returns a non-zero exit code.
 
-    else:
-        raise NotImplementedError(f"File type {file_type} not supported.")
+    AssertionError
+        If the output does not match the expected results.
 
-    if path is None:
-        temp_file, path = tempfile.mkstemp(suffix=f".{file_type}")
+    Notes
+    -----
+    The script is run using the python interpreter, so the script file should
+    have a shebang line at the top to specify the interpreter to be used. This
+    isn't an issue for most scripts, but it is something to be aware of if you
+    are expecting to use/test with a sepcific interpreter.
+    """
+    if not os.path.exists(script_path):
+        raise FileNotFoundError(f"Script file {script_path} not found.")
 
-    else:
-        if not path.endswith(f".{file_type}"):
-            directory = os.path.dirname(path)
-            file_name = os.path.basename(path).replace(".file_type", "")
-            temp_file, path = tempfile.mkstemp(
-                suffix=f".{file_type}", dir=directory, prefix=file_name
-            )
+    if isinstance(python_options, str):
+        python_options = python_options.split()
 
-        else:
-            temp_file, path = tempfile.mkstemp(suffix=f".{file_type}")
+    command_components = [
+        ["python"],
+        python_options,
+        [script_path],
+        script_options,
+    ]
+
+    command = [x for x in itertools.chain(*command_components)]
+
+    process = subprocess.run(
+        command,
+        capture_output=True,
+    )
+
+    stdout = process.stdout
+    stderr = process.stderr
+
+    # Helper function to check the output against the expected results using
+    # regex.
+    def _reg_assert(result, expected):
+        match = re.match(expected, result, flags=regex_options)
+
+        if not match:
+            raise AssertionError(
+                f"Expected pattern {expected!r} but got:\n{result!r}"
+            )
 
-    file = os.fdopen(temp_file, "w+b")
+    if stdout_result is not None:
+        _reg_assert(stdout.decode("utf-8"), stdout_result)
 
-    for chunk in iter(lambda: file_data.read(10000), b""):
-        file.write(chunk)
+    if stderr_result is not None:
+        _reg_assert(stderr.decode("utf-8"), stderr_result)
 
-    file.flush()
+    if fail_on_error and process.returncode:
+        raise subprocess.CalledProcessError(
+            process.returncode, command, stdout, stderr
+        )
 
-    return path
+    return True
 
 
-class ProgramTempFile:
-    """This is a temporary file that lasts the lifetime of the object (until it
-    is garbage collected).
+def process_string_to_python_script(string: str) -> str:
+    """Takes an input string and performs tasks to make it properly python-formatted.
 
-    Note: this does *not* mean the file will be deleted when the object is no
-    longer referenced. It will be deleted when the object is garbage collected,
-    which may not be until the end of the program.
+    Parameters
+    ----------
+    string : str
+        The string to be processed.
     """
+    # For multiline strings, need to get rid of possible hanging indents
+    # The first line may be unindented.
+    lines = string.split("\n")
+    first_line = lines[0].strip()
 
-    path: str
-    _is_open: bool
-    _file_obj: io.IOBase | None
-
-    def __init__(self, path: str = ""):
-        self.path = path
-
-        if not self.path:
-            self.path = tempfile.mkstemp()[1]
+    # Determine the minimum indentation of the other lines.
+    min_indent = min(
+        len(line) - len(line.lstrip()) for line in lines[1:] if line.strip()
+    )
 
-        self._is_open = False
-        self._file_obj = None
+    # Remove the minimum indentation from all lines.
+    lines = [first_line] + [line[min_indent:] for line in lines[1:]]
 
-    def __del__(self):
-        self.close()
-
-    def open(
-        self,
-        mode: str = "r",
-        encoding="utf-8",
-        **kwargs,
-    ) -> io.IOBase:
-        """Open the temporary file and return an opened File object.
-
-        It takes the same arguments as the built in open() function, except for
-        the file name (which is provided by the ProgramTempFile object).
-        """
-        try:
-            # pylint: disable=consider-using-with
-            file = open(self.path, mode, encoding=encoding, **kwargs)
-
-        except FileNotFoundError as fnf_err:
-            msg = "Temporary file could not be opened."
-            raise FileNotFoundError(msg) from fnf_err
-
-        self._is_open = True
-        self._file_obj = file
-        return file
-
-    def close(self, delete: bool = True):
-        """If the file is open, close it and delete it from disk."""
-        if delete and os.path.exists(self.path):
-            os.remove(self.path)
-
-        if not getattr(self._file_obj, "closed", True):
-            self._file_obj.close()
-
-        self._is_open = False
-
-    @property
-    def is_open(self) -> bool:
-        """True if the temporary file is 'open' for reading, writing, or both.
-        False otherwise.
-        """
-        return self._is_open
+    return "\n".join(lines)
 
 
-class FITSTempFile(ProgramTempFile):
-    """A temporary FITS file that lasts the lifetime of the object (until it
-    is garbage collected), and is initialized with FITS-like data.
-    """
-
-    path: str
-    _raw_test_file: str
-
-    def __init__(
-        self,
-        path: os.PathLike | None = None,
-        hdus: _HDUL_LIKE_TYPE | None = None,
-        n_extensions: int = 1,
-        image_shape: tuple[int, int] | None = None,
-        include_header_keys: Iterable[str] | None = None,
-        file_type: str = "fits",
-    ):
-        """Initializes the FITSTempFile. See
-        :func:`~astropy.testing.create_test_file()` for details on the
-        arguments passed.
-        """
-        super().__init__(path)
+def get_program_observations():
+    raise NotImplementedError
```

### Comparing `astrodata-2.9.1.dev1/astrodata/utils.py` & `astrodata-2.9.2/astrodata/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions and classes for AstroData objects."""
+
 import inspect
 import logging
 import warnings
 from collections import namedtuple
 from functools import wraps
 from traceback import format_stack
```

### Comparing `astrodata-2.9.1.dev1/astrodata/wcs.py` & `astrodata-2.9.2/astrodata/wcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """World Coordinate System (WCS) support for AstroData objects."""
+
 import functools
 import logging
 import re
 from collections import namedtuple
 from copy import deepcopy
 
 import numpy as np
@@ -53,32 +54,57 @@
         axes_order=tuple(range(naxes)),
         name=name,
         axes_names=axes_names,
         unit=[u.pix] * naxes,
     )
 
 
-def fitswcs_to_gwcs(input_data):
+def fitswcs_to_gwcs(input_data, *, raise_errors: bool = False):
     """Create and return a gWCS object from a FITS header or NDData object.  If
     it can't construct one, it should quietly return None.
+
+    Parameters
+    ----------
+    input_data : `astropy.io.fits.Header` or `astropy.nddata.NDData`
+        FITS Header or NDData object with basic FITS WCS keywords.
+
+    raise_errors : bool
+        If True, raise an exception if the gWCS cannot be created.
+
+    Returns
+    -------
+    gWCS or None
+        A gWCS object or None if it can't be created.
+
+    Raises
+    ------
+    TypeError
+        If the input is not a FITS Header or a NDData object.
+
+    ValueError
+        If the WCS cannot be constructed and raise_errors is True.
     """
     # coordinate names for CelestialFrame
     coordinate_outputs = {"alpha_C", "delta_C"}
 
     # transform = gw.make_fitswcs_transform(hdr)
     try:
         transform = make_fitswcs_transform(input_data)
 
-    except (TypeError, ValueError) as err:
-        logging.warning(
-            "Could not create gWCS: %s: %s",
-            err.__class__.__name__,
-            err,
-        )
-        return None
+    except (IndexError, TypeError, ValueError) as err:
+        if not raise_errors:
+            logging.warning(
+                "Could not create gWCS: %s: %s",
+                err.__class__.__name__,
+                err,
+            )
+
+            return None
+
+        raise
 
     outputs = transform.outputs
 
     try:
         wcs_info = read_wcs_from_header(input_data.meta["header"])
 
     except AttributeError:
@@ -152,22 +178,25 @@
         out_frames.append(cel_frame)
 
     out_frame = (
         out_frames[0]
         if len(out_frames) == 1
         else cf.CompositeFrame(out_frames, name="world")
     )
+
     return gWCS([(in_frame, transform), (out_frame, None)])
 
 
 # -----------------------------------------------------------------------------
 # gWCS -> FITS-WCS
 # -----------------------------------------------------------------------------
 
 
+# TODO: Rename this and deprecate this function. The name implies it is a
+# gwcs object being passed, but it requires an NDData object.
 def gwcs_to_fits(ndd, hdr=None):
     """Convert a gWCS object to a collection of FITS WCS keyword/value pairs,
     if possible. If the FITS WCS is only approximate, this should be indicated
     with a dict entry {'FITS-WCS': 'APPROXIMATE'}. If there is no suitable FITS
     representation, then a ValueError or NotImplementedError can be raised.
 
     Parameters
@@ -189,33 +218,42 @@
     wcs = ndd.wcs
     # Don't need to "copy" because any changes to transform use
     # replace_submodel, which creates a new instance
     transform = wcs.forward_transform
     world_axes = list(wcs.output_frame.axes_names)
     nworld_axes = len(world_axes)
     tabular_axes = {}
+
+    # Depending on how NDData is generated, it may not have a shape attr.
+    try:
+        shape = ndd.shape
+
+    except AttributeError:
+        # Try to get the shape from the contained data
+        shape = ndd.data.shape
+
     wcs_dict = {
-        "NAXIS": len(ndd.shape),  # in case it's not written to a file
+        "NAXIS": len(shape),  # in case it's not written to a file
         "WCSAXES": nworld_axes,
         "WCSDIM": nworld_axes,
     }
+
     wcs_dict.update(
-        {
-            f"NAXIS{i}": length
-            for i, length in enumerate(ndd.shape[::-1], start=1)
-        }
+        {f"NAXIS{i}": length for i, length in enumerate(shape[::-1], start=1)}
     )
+
     wcs_dict.update(
         {
             f"CD{i+1}_{j+1}": 0.0
             for j in range(nworld_axes)
             for i in range(nworld_axes)
         }
     )
-    pix_center = [0.5 * (length - 1) for length in ndd.shape[::-1]]
+
+    pix_center = [0.5 * (length - 1) for length in shape[::-1]]
     wcs_center = transform(*pix_center)
     if nworld_axes == 1:
         wcs_center = (wcs_center,)
 
     # Find and process the sky projection first
     if {"lon", "lat"}.issubset(world_axes):
         if isinstance(wcs.output_frame, cf.CelestialFrame):
@@ -344,24 +382,24 @@
         else:  # Just something
             wcs_dict[f"CRVAL{i}"] = wcs_center[i - 1]
 
     # Flag if we can't construct a perfect CD matrix
     if not model_is_affine(transform):
         wcs_dict["FITS-WCS"] = ("APPROXIMATE", "FITS WCS is approximate")
 
-    affine = calculate_affine_matrices(transform, ndd.shape)
+    affine = calculate_affine_matrices(transform, shape)
 
     # Convert to x-first order
     affine_matrix = np.flip(affine.matrix)
 
     # Require an inverse to write out
     wcs_dict.update(
         {
             f"CD{i+1}_{j+1}": affine_matrix[i, j]
-            for j, _ in enumerate(ndd.shape)
+            for j, _ in enumerate(shape)
             for i, _ in enumerate(world_axes)
         }
     )
 
     # Don't overwrite CTYPEi keywords we've already created
     wcs_dict.update(
         {
@@ -385,29 +423,29 @@
     modified_wcs_center = transform(*pix_center)
     if nworld_axes == 1:
         modified_wcs_center = (modified_wcs_center,)
 
     wcs_gen = enumerate(zip(wcs_center, modified_wcs_center), start=1)
     for world_axis, (wcs_val, modified_wcs_val) in wcs_gen:
         if wcs_val > 0 and np.isclose(modified_wcs_val, np.log(wcs_val)):
-            for j, _ in enumerate(ndd.shape, start=1):
+            for j, _ in enumerate(shape, start=1):
                 wcs_dict[f"CD{world_axis}_{j}"] *= crval[world_axis - 1]
                 wcs_dict[f"CTYPE{world_axis}"] = (
                     wcs_dict[f"CTYPE{world_axis}"][:4] + "-LOG"
                 )
 
             crval[world_axis - 1] = np.log(crval[world_axis - 1])
 
     # This (commented) line fails for un-invertable Tabular2D
     # crpix = np.array(wcs.backward_transform(*crval)) + 1
     crpix = np.array(transform.inverse(*crval)) + 1
 
     # Cope with a situation where the sky projection center is not in the slit
     # We may be able to fix this in future, but FITS doesn't handle it well.
-    if len(ndd.shape) > 1:
+    if len(shape) > 1:
         crval2 = wcs(*(crpix - 1))
         try:
             sky_center = coord.SkyCoord(
                 nat2cel.lon.value,
                 nat2cel.lat.value,
                 unit=u.deg,
             )
@@ -424,41 +462,39 @@
 
             if sky_center.separation(sky_center2).arcsec > 0.01:
                 wcs_dict["FITS-WCS"] = (
                     "APPROXIMATE",
                     "FITS WCS is approximate",
                 )
 
-    if len(ndd.shape) == 1:
+    if len(shape) == 1:
         wcs_dict["CRPIX1"] = crpix
 
     else:
         # Comply with FITS standard, must define CRPIXj for "extra" axes
         wcs_dict.update(
             {
                 f"CRPIX{j}": cpix
                 for j, cpix in enumerate(
-                    np.concatenate(
-                        [crpix, [1] * (nworld_axes - len(ndd.shape))]
-                    ),
+                    np.concatenate([crpix, [1] * (nworld_axes - len(shape))]),
                     start=1,
                 )
             }
         )
 
     for i, unit in enumerate(wcs.output_frame.unit, start=1):
         try:
             wcs_dict[f"CUNIT{i}"] = unit.name
 
         except AttributeError:
             pass
 
     # To ensure an invertable CD matrix, we need to get nonexistent pixel axes
     # "involved".
-    for j in range(len(ndd.shape), nworld_axes):
+    for j in range(len(shape), nworld_axes):
         wcs_dict[f"CD{nworld_axes}_{j+1}"] = 1
 
     return wcs_dict
 
 
 # -----------------------------------------------------------------------------
 # Helper functions
@@ -637,27 +673,25 @@
 
             else:
                 mult = header.get(f"PC{i}_{j}", 1 if i == j else 0)
                 cd[i - 1, j - 1] = cdelt[i - 1] * mult
 
     # Hack to deal with non-FITS-compliant data where one axis is ignored
     unspecified_pixel_axes = [
-        axis for axis, unused in enumerate(np.all(cd == 0, axis=1)) if unused
+        axis for axis, unused in enumerate(np.all(cd == 0, axis=0)) if unused
     ]
 
     if unspecified_pixel_axes:
         unused_world_axes = [
             axis
-            for axis, unused in enumerate(np.all(cd == 0, axis=0))
+            for axis, unused in enumerate(np.all(cd == 0, axis=1))
             if unused
         ]
 
-        unused_world_axes += list(
-            range(wcsaxes, wcsaxes + len(unspecified_pixel_axes))
-        )
+        unused_world_axes += [wcsaxes - 1] * len(unspecified_pixel_axes)
 
         for pixel_axis, world_axis in zip(
             unspecified_pixel_axes, unused_world_axes
         ):
             cd[world_axis, pixel_axis] = 1.0
 
     wcs_info["CTYPE"] = ctype
@@ -693,16 +727,15 @@
     # Split each CTYPE value at "-" and take the first part.
     # This should represent the coordinate system.
     ctype = [ax.split("-")[0].upper() for ax in wcs_info["CTYPE"]]
     sky_inmap = []
     spec_inmap = []
     unknown = []
     skysystems = np.array(list(sky_pairs.values())).flatten()
-    for ax in ctype:
-        ind = ctype.index(ax)
+    for ind, ax in enumerate(ctype):
         if ax in specsystems:
             spec_inmap.append(ind)
         elif ax in skysystems:
             sky_inmap.append(ind)
         else:
             unknown.append(ind)
```

### Comparing `astrodata-2.9.1.dev1/pyproject.toml` & `astrodata-2.9.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "astrodata"
-version = "2.9.1.dev1"
+version = "2.9.2"
 description = "A package for managing astronomical data through a uniform interface"
 authors = ["D. J. Teal <dillon.teal@noirlab.com>", "DRAGONS development team"]
 license = "BSD3"
-readme = "README.rst"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 astropy = "^6.0.0"
 asdf = "^3.1.0"
 gwcs = "^0.21.0"
 jsonschema = "^4.21.1"
@@ -18,14 +18,15 @@
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.3"
 coverage = "^7.4.4"
 isort = "^5.13.2"
 poetry = "^1.8.2"
 pre-commit = "^3.6.2"
+xenon = "^0.9.1"
 
 [tool.poetry.group.docs]
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 sphinx-automodapi = "^0.17.0"
 sphinx-autoapi = "^3.0.0"
@@ -39,14 +40,15 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.4.4"
 pytest-cov = "^4.1.0"
 pytest-doctestplus = "^1.2.1"
 tox = "^4.14.1"
+hypothesis = "^6.99.13"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = [
@@ -76,15 +78,14 @@
  "*/astrodata/__init*",
  "*/astrodata/conftest.py",
  "*/astrodata/*setup_package*",
  "*/astrodata/tests/*",
  "*/astrodata/*/tests/*",
  "*/astrodata/extern/*",
  "*/astrodata/version*",
- "*/*/astrodata/testing.py",
  "_*.py",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   # Have to re-enable the standard pragma
   "pragma: no cover",
@@ -95,8 +96,10 @@
   "raise NotImplementedError",
   # Don't complain about script hooks
   "def main(.*):",
   # Ignore branches that don't pertain to this version of Python
   "pragma: py{ignore_python_version}",
   # Don't complain about IPython completion helper
   "def _ipython_key_completions_",
+  # Don't worry about breakpoints (from testing file)
+  "breakpoint",
 ]
```

### Comparing `astrodata-2.9.1.dev1/PKG-INFO` & `astrodata-2.9.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrodata
-Version: 2.9.1.dev1
+Version: 2.9.2
 Summary: A package for managing astronomical data through a uniform interface
 License: BSD3
 Author: D. J. Teal
 Author-email: dillon.teal@noirlab.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,146 +12,205 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asdf (>=3.1.0,<4.0.0)
 Requires-Dist: astropy (>=6.0.0,<7.0.0)
 Requires-Dist: gwcs (>=0.21.0,<0.22.0)
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-.. |DRAGONS| replace:: ``DRAGONS``
-..  _DRAGONS: https://https://github.com/GeminiDRSoftware/DRAGONS/
+[DRAGONS link]: https://github.com/GeminiDRSoftware/DRAGONS
+[astrodata docs]: https://geminidrsoftware.github.io/astrodata/
+[astrodata repo]: https://geminidrsoftware.github.io/astrodata/
+[astropy link]: https://astropy.org
+[pypi link]: https://pypi.org/project/astrodata
+
+[coverage badge]: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/teald/d2f3af2a279efc1f6e90d457a3c50e47/raw/covbadge.json
+[docs build badge]: https://github.com/GeminiDRSoftware/astrodata/actions/workflows/documentation.yml/badge.svg
+[pypi packaging badge]: https://github.com/GeminiDRSoftware/astrodata/actions/workflows/publish_pypi.yml/badge.svg
+[pypi package version badge]: https://badge.fury.io/py/astrodata.svg
+[test status badge]: https://github.com/GeminiDRSoftware/astrodata/actions/workflows/testing.yml/badge.svg
 
-.. |astrodatadocs| replace:: `astrodata documentation`
-..  _astrodatadocs: https://geminidrsoftware.github.io/astrodata/
 
-.. |astrodatarepo| replace:: `astrodata repository`
-.. _astrodatarepo: https://github.com/GeminiDRSoftware/astrodata
-
-``astrodata``
+`astrodata`
 =============
 
-.. image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/teald/d2f3af2a279efc1f6e90d457a3c50e47/raw/covbadge.json
-    :alt: A badge displaying the coverage level of this repository.
+<img align="left" src="docs/static/logo.png" height=200
+style="padding-right: 10; padding-bottom: 10; border: none;">
+
+### Tests
+![A badge displaying the testing coverage percentage of this repository.][coverage badge]
+![Testing status badge][test status badge]
+
+### Building & Publishing
+![Documentation build status badge][docs build badge]
+[![PyPI version badge](https://badge.fury.io/py/astrodata.svg)](https://badge.fury.io/py/astrodata)
+![pypi packaging status badge][pypi packaging badge]
+
+<!-- Clearing the logo for the next header -->
+<br clear="left">
 
-A package for managing astronomical data through a uniform interface
+Making astronomical data consistent and approachable
 --------------------------------------------------------------------
 
-``astrodata`` is a package for managing astronomical data through a uniform
+`astrodata` is a package for managing astronomical data through a uniform
 interface. It is designed to be used with the
-`Astropy <https://www.astropy.org>`_ package. ``astrodata`` was designed by and
-for use as part of the |DRAGONS|_ data reduction pipeline, but it is now
+[Astropy package][astropy link]. `astrodata` was designed by and
+for use as part of the [`DRAGONS`][DRAGONS link] data reduction pipeline, but it is now
 implemented to be useful for any astronomical data reduction or analysis
 project.
 
 Unlike managing files using the ``astropy.io.fits`` package alone, ``astrodata``
 is designed to be extendible to any data format, and to parse, respond to, and
 store metadata in a consistent, intentional way. This makes it especially
 useful for managing data from multiple instruments, telescopes, and data
 generation utilities.
 
-**Note:** If you are trying to reduce Gemini data, please use |DRAGONS|_.
-Interaction with this package directly is primarily suited for developers, and 
+**Note:** If you are trying to reduce Gemini data, please use [`DRAGONS`][DRAGONS link].
+Interaction with this package directly is primarily suited for developers, and
 does not come with any tools for data reduction on any specific instrument or
 data.
 
 Installation
 ------------
 
-``astrodata`` is available on `PyPI <https://pypi.org/project/astrodata>`_ and
-can be installed using ``pip``:
+`astrodata` is available on the [Python Package Index][pypi link] and
+can be installed using `pip`:
 
-.. code-block:: bash
+```
+pip install astrodata
+```
+
+Documentation
+-------------
+
+Documentation for ``astrodata`` is available on our [GitHub pages site][astrodata docs]. This documentation includes a
+user and programmer's guide, as well as a full API reference.
 
-    pip install astrodata
 
 Usage
 -----
 
 The most basic usage of ``astrodata`` is to extend the ``astrodata.AstroData``
 class, which includes some basic FITS file handling methods by default:
 
-.. code-block:: python
+```python
+from astrodata import AstroData, astro_data_descriptor, factory, from_file
 
-    from astrodata import AstroData
 
-    class MyData(AstroData):
-        def __init__(self, *args, **kwargs):
-            super().__init__(*args, **kwargs)
+class MyData(AstroData):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-        def my_method(self):
-            print('This is my method, and it tells me about my data.')
-            print(self.info())
+    @astro_data_descriptor
+    def color(self):
+        # The color filter used for our image is stored in a few different
+        # ways, let's unify them.
+        blue_labels = {"blue", "bl", "b"}
+        green_labels = {"green", "gr", "g"}
+        red_labels = {"red", "re", "r"}
 
-    data = MyData.read('my_file.fits')
-    data.my_method()
+        header_value = self.phu.get("COLOR", None).casefold()
 
-This will print out the header of the FITS file, as well as the filename and
-path of the file (as it does for ``astropy.io.fits`` objects).
+        if header_value in blue_labels:
+            return "BLUE"
 
-``astrodata`` is designed to be extendible, so you can add your own methods to
+        if header_value in green_labels:
+            return "GREEN"
 
-Documentation
--------------
+        if header_value in red_labels:
+            return "RED"
 
-Documentation for ``astrodata`` is available at
-|astrodatadocs|_. This documentation includes a
-user and programmer's guide, as well as a full API reference.
+        if header_value is None:
+            raise ValueError("No color found")
 
+        # Unrecognized color
+        raise ValueError(f"Did not recognize COLOR value: {header_value}")
 
-Installing development dependencies
------------------------------------
 
-``astrodata`` uses `Poetry <https://github.com/python-poetry/poetry>`_ for build
-and package management. To install development dependencies, you must clone this
-repository. Once you have, at the top level directory of the ``astrodata``
-repository run
+# Now, define our instruments with nuanced, individual data formats
+class MyInstrument1(MyData):
+    # These use a special method to resolve the metadata and apply the correct
+    # class.
+    @staticmethod
+    def _matches_data(source):
+        return source[0].header.get("INSTRUME", "").upper() == "MYINSTRUMENT1"
 
-.. code-block:: terminal
 
-    pip -m install poetry
-    poetry install
+class MyInstrument2(MyData):
+    @staticmethod
+    def _matches_data(source):
+        return source[0].header.get("INSTRUME", "").upper() == "MYINSTRUMENT2"
 
-    # To install without specific development groups
-    poetry install --without test,docs,dev
 
-License
--------
+class MyInstrument3(MyData):
+    @staticmethod
+    def _matches_data(source):
+        return source[0].header.get("INSTRUME", "").upper() == "MYINSTRUMENT3"
+
 
-This project is Copyright 2024 (c)  and licensed under
-the terms of the BSD 3-clause license. This package is based upon
-the `Openastronomy packaging guide <https://github.com/OpenAstronomy/packaging-guide>`_
-which is licensed under the BSD 3-clause licence. See the LICENSE folder for
-more information.
+for cls in [MyInstrument1, MyInstrument2, MyInstrument3]:
+    factory.add_class(cls)
+
+# my_file.fits has some color data depending on the instrument it comes from,
+# but now we can access it and handle a single value.
+data = from_file("README_example.fits")
+
+# the astrodata factory has already resolved the correct class for us.
+print(f"File used to create class: {data.__class__.__name__}")
+if data.color() == "BLUE":
+    print("I used the blue filter!")
+
+else:
+    print("I used a red or green filter!")
+
+# Get all the info about the astrodata object.
+data.info()
+
+```
+
+This will print out the filter used as extracted from the header of the FITS
+file. `data.info()` offers a more complete look at the file's data including
+the filename and path of the file (as it does for `astropy.io.fits` objects).
+
+`astrodata` is designed to be extensible, so you can add your own methods to
+analyze and process data based on your specific needs and use cases.
+
+For a complete example, see the
+[Quickstart](https://geminidrsoftware.github.io/astrodata/quickstart.html) in
+our documentation.
+
+Installing development dependencies
+-----------------------------------
+
+``astrodata`` uses [Poetry](https://github.com/python-poetry/poetry) for build
+and package management. To install development dependencies, you must clone
+this repository. Once you have, at the top level directory of the `astrodata`
+repository run
+
+```
+pip install --upgrade pip
+pip install poetry
+poetry install
+
+# To install without specific development groups. Omit those you would prefer
+# not be installed
+poetry install --without test,docs,dev
+```
 
 Contributing
 ------------
 
-We love contributions! astrodata is open source,
-built on open source, and we'd love to have you hang out in our community.
+See [our contributing guidelines](CONTRIBUTING.md) for information on
+contributing. If you're worried about contributing, or feel intimidated, please
+remember that your contribution is immensly appreciated---no matter how small!
 
-**Imposter syndrome disclaimer**: We want your help. No, really.
+License
+-------
 
-There may be a little voice inside your head that is telling you that you're not
-ready to be an open source contributor; that your skills aren't nearly good
-enough to contribute. What could you possibly offer a project like this one?
-
-We assure you - the little voice in your head is wrong. If you can write code at
-all, you can contribute code to open source. Contributing to open source
-projects is a fantastic way to advance one's coding skills. Writing perfect code
-isn't the measure of a good developer (that would disqualify all of us!); it's
-trying to create something, making mistakes, and learning from those
-mistakes. That's how we all improve, and we are happy to help others learn.
-
-Being an open source contributor doesn't just mean writing code, either. You can
-help out by writing documentation, tests, or even giving feedback about the
-project (and yes - that includes giving feedback about the contribution
-process). Some of these contributions may be the most valuable to the project as
-a whole, because you're coming to the project with fresh eyes, so you can see
-the errors and assumptions that seasoned contributors have glossed over.
-
-Note: This disclaimer was originally written by
-`Adrienne Lowe <https://github.com/adriennefriend>`_ for a
-`PyCon talk <https://www.youtube.com/watch?v=6Uj746j9Heo>`_, and was adapted by
-astrodata based on its use in the README file for the
-`MetPy project <https://github.com/Unidata/MetPy>`_.
+This project is Copyright 2024 (c)  and licensed under the terms of a modified
+BSD 3-clause license through AURA astronomy. This package is based upon the
+[Openastronomy packaging
+guide](https://github.com/OpenAstronomy/packaging-guide) which is licensed
+under the standard BSD 3-clause licence. See the LICENSE file for more
+information.
```

