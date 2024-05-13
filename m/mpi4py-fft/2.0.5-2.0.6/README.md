# Comparing `tmp/mpi4py-fft-2.0.5.tar.gz` & `tmp/mpi4py_fft-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpi4py-fft-2.0.5.tar", last modified: Wed Apr 26 08:43:50 2023, max compression
+gzip compressed data, was "mpi4py_fft-2.0.6.tar", last modified: Mon May 13 07:49:54 2024, max compression
```

## Comparing `mpi4py-fft-2.0.5.tar` & `mpi4py_fft-2.0.6.tar`

### file list

```diff
@@ -1,35 +1,44 @@
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.846779 mpi4py-fft-2.0.5/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1439 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/LICENSE.rst
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      160 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/MANIFEST.in
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3810 2023-04-26 08:43:50.846459 mpi4py-fft-2.0.5/PKG-INFO
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2980 2023-04-26 08:39:58.000000 mpi4py-fft-2.0.5/README.rst
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.835841 mpi4py-fft-2.0.5/mpi4py_fft/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1001 2023-04-26 08:42:41.000000 mpi4py-fft-2.0.5/mpi4py_fft/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    17899 2022-06-10 04:50:35.000000 mpi4py-fft-2.0.5/mpi4py_fft/distarray.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.842475 mpi4py-fft-2.0.5/mpi4py_fft/fftw/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      155 2022-11-02 13:12:48.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5262 2022-11-02 13:56:49.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/factory.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2467 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_planxfftn.c
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      530 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_planxfftn.h
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1550 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_xfftn.pxd
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11115 2021-03-25 16:57:58.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_xfftn.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     2458 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/utilities.pyx
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    27897 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/fftw/xfftn.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.845694 mpi4py-fft-2.0.5/mpi4py_fft/io/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)      114 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/__init__.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     4705 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/file_base.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11792 2023-04-26 07:18:14.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/generate_xdmf.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     5889 2022-05-31 13:12:18.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/h5py_file.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     7675 2021-03-25 15:19:51.000000 mpi4py-fft-2.0.5/mpi4py_fft/io/nc_file.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    15717 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/mpi4py_fft/libfft.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    15692 2023-04-14 11:12:30.000000 mpi4py-fft-2.0.5/mpi4py_fft/mpifft.py
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)    11808 2023-04-14 11:15:06.000000 mpi4py-fft-2.0.5/mpi4py_fft/pencil.py
-drwxr-xr-x   0 mikaelmortensen   (501) staff       (20)        0 2023-04-26 08:43:50.837671 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     3810 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/PKG-INFO
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     1254 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/SOURCES.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)        1 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/dependency_links.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       13 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/requires.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       11 2023-04-26 08:43:50.000000 mpi4py-fft-2.0.5/mpi4py_fft.egg-info/top_level.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       20 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/requirements.txt
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)       38 2023-04-26 08:43:50.846875 mpi4py-fft-2.0.5/setup.cfg
--rw-r--r--   0 mikaelmortensen   (501) staff       (20)     7375 2019-12-10 15:59:29.000000 mpi4py-fft-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:49:54.680592 mpi4py_fft-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-13 07:49:54.680592 mpi4py_fft-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:49:54.676592 mpi4py_fft-2.0.6/mpi4py_fft/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/distarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:49:54.676592 mpi4py_fft-2.0.6/mpi4py_fft/fftw/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/fftw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/fftw/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/fftw/fftw_planxfftn.c
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/fftw/fftw_planxfftn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/fftw/fftw_xfftn.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/fftw/fftw_xfftn.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/fftw/utilities.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    27897 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/fftw/xfftn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:49:54.676592 mpi4py_fft-2.0.6/mpi4py_fft/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/io/file_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/io/generate_xdmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/io/h5py_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/io/nc_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/libfft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15692 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/mpifft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/mpi4py_fft/pencil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:49:54.680592 mpi4py_fft-2.0.6/mpi4py_fft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-13 07:49:54.000000 mpi4py_fft-2.0.6/mpi4py_fft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 07:49:54.000000 mpi4py_fft-2.0.6/mpi4py_fft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:49:54.000000 mpi4py_fft-2.0.6/mpi4py_fft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 07:49:54.000000 mpi4py_fft-2.0.6/mpi4py_fft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 07:49:54.000000 mpi4py_fft-2.0.6/mpi4py_fft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:49:54.680592 mpi4py_fft-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:49:54.680592 mpi4py_fft-2.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/tests/test_darray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/tests/test_fftw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/tests/test_libfft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/tests/test_mpifft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/tests/test_pencil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-13 07:49:43.000000 mpi4py_fft-2.0.6/tests/test_speed.py
```

### Comparing `mpi4py-fft-2.0.5/LICENSE.rst` & `mpi4py_fft-2.0.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/PKG-INFO` & `mpi4py_fft-2.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: mpi4py-fft
-Version: 2.0.5
+Version: 2.0.6
 Summary: mpi4py-fft -- Parallel Fast Fourier Transforms (FFTs) using MPI for Python
-Home-page: https://bitbucket.org/mpi4py/mpi4py-fft
+Home-page: https://github.com/mpi4py/mpi4py-fft
 Author: Lisandro Dalcin and Mikael Mortensen
-License: UNKNOWN
 Keywords: Python,FFTW,FFT,DCT,DST,MPI
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
+Requires-Dist: mpi4py
+Requires-Dist: numpy
 
 mpi4py-fft
 ----------
 
 
 .. image:: https://dev.azure.com/mpi4py/mpi4py-fft/_apis/build/status/mpi4py.mpi4py-fft?branchName=master
     :target: https://dev.azure.com/mpi4py/mpi4py-fft
@@ -96,9 +97,7 @@
 
 For IO you need to install either `h5py <https://www.h5py.org>`_ or
 `netCDF4 <http://unidata.github.io/netcdf4-python/>`_ with support for
 MPI. Both are available from the coda-forge channel through::
 
     conda install -c conda-forge h5py=*=mpi* netcdf4=*=mpi*
 
-
-
```

### Comparing `mpi4py-fft-2.0.5/README.rst` & `mpi4py_fft-2.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/__init__.py` & `mpi4py_fft-2.0.6/mpi4py_fft/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 is supported. Furthermore, **mpi4py-fft** can also be used simply to perform
 global redistributions (distribute and communicate) of large arrays with MPI,
 without any transforms at all.
 
 For more information, see `documentation <https://mpi4py-fft.readthedocs.io>`_.
 
 """
-__version__ = '2.0.5'
+__version__ = '2.0.6'
 __author__ = 'Lisandro Dalcin and Mikael Mortensen'
 
 from .distarray import DistArray, newDistArray, Function
 from .mpifft import PFFT
 from . import fftw
 from .fftw import fftlib
 from .io import HDF5File, NCFile, generate_xdmf
```

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/distarray.py` & `mpi4py_fft-2.0.6/mpi4py_fft/distarray.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/fftw/factory.py` & `mpi4py_fft-2.0.6/mpi4py_fft/fftw/factory.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_planxfftn.c` & `mpi4py_fft-2.0.6/mpi4py_fft/fftw/fftw_planxfftn.c`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_planxfftn.h` & `mpi4py_fft-2.0.6/mpi4py_fft/fftw/fftw_planxfftn.h`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_xfftn.pxd` & `mpi4py_fft-2.0.6/mpi4py_fft/fftw/fftw_xfftn.pxd`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-cdef extern from "fftw3.h":
+# cython: language_level=3str
+cdef extern from "fftw3.h" nogil:
 
     ctypedef struct fftw_complex_struct:
         pass
 
     ctypedef fftw_complex_struct *fftw_complex
 
     ctypedef struct fftw_plan_struct:
         pass
 
     ctypedef fftw_plan_struct *fftw_plan
 
     void fftw_destroy_plan(fftw_plan)
 
-    void fftw_execute_dft(fftw_plan, void *_in, void *_out) nogil
+    void fftw_execute_dft(fftw_plan, void *_in, void *_out)
 
-    void fftw_execute_dft_c2r(fftw_plan, void *_in, void *_out) nogil
+    void fftw_execute_dft_c2r(fftw_plan, void *_in, void *_out)
 
-    void fftw_execute_dft_r2c(fftw_plan, void *_in, void *_out) nogil
+    void fftw_execute_dft_r2c(fftw_plan, void *_in, void *_out)
 
-    void fftw_execute_r2r(fftw_plan, void *_in, void *_out) nogil
+    void fftw_execute_r2r(fftw_plan, void *_in, void *_out)
 
-    void fftw_execute(fftw_plan) nogil
+    void fftw_execute(fftw_plan)
 
     void fftw_init_threads()
 
     void fftw_plan_with_nthreads(int n)
 
     int fftw_export_wisdom_to_filename(const char *filename)
 
@@ -39,22 +40,22 @@
     void fftw_cleanup_threads()
 
     int fftw_alignment_of(void *_in)
 
     void fftw_print_plan(fftw_plan)
 
 
-cdef extern from "fftw_planxfftn.h":
+cdef extern from "fftw_planxfftn.h" nogil:
 
     ctypedef double fftw_real
 
     fftw_plan fftw_planxfftn(int      ndims,
                              int      sizes_in[],
                              void     *_in,
                              int      sizes_out[],
                              void     *_out,
                              int      naxes,
                              int      axes[],
                              int      kind[],
                              unsigned flags)
 
-ctypedef void (*generic_function)(void *plan, void *_in, void *_out) nogil
+ctypedef void (*generic_function)(void *plan, void *_in, void *_out) noexcept nogil
```

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/fftw/fftw_xfftn.pyx` & `mpi4py_fft-2.0.6/mpi4py_fft/fftw/fftw_xfftn.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-cimport fftw_xfftn
-#cython: language_level=3
+# cython: language_level=3str
+from . cimport fftw_xfftn
 cimport numpy as np
 from .utilities import *
 import numpy as np
 from libc.stdint cimport intptr_t
 from libc.stdlib cimport malloc, free
 
 cpdef int alignment_of(input_array):
@@ -22,24 +22,24 @@
 cpdef void set_timelimit(fftw_real limit):
     fftw_set_timelimit(limit)
 
 cpdef void cleanup():
     fftw_cleanup()
     fftw_cleanup_threads()
 
-cdef void _fftw_execute_dft(void *plan, void *_in, void *_out) nogil:
+cdef void _fftw_execute_dft(void *plan, void *_in, void *_out) noexcept nogil:
     fftw_execute_dft(<fftw_plan>plan, <fftw_complex *>_in, <fftw_complex *>_out)
 
-cdef void _fftw_execute_dft_r2c(void *plan, void *_in, void *_out) nogil:
+cdef void _fftw_execute_dft_r2c(void *plan, void *_in, void *_out) noexcept nogil:
     fftw_execute_dft_r2c(<fftw_plan>plan, <fftw_real *>_in, <fftw_complex *>_out)
 
-cdef void _fftw_execute_dft_c2r(void *plan, void *_in, void *_out) nogil:
+cdef void _fftw_execute_dft_c2r(void *plan, void *_in, void *_out) noexcept nogil:
     fftw_execute_dft_c2r(<fftw_plan>plan, <fftw_complex *>_in, <fftw_real *>_out)
 
-cdef void _fftw_execute_r2r(void *plan, void *_in, void *_out) nogil:
+cdef void _fftw_execute_r2r(void *plan, void *_in, void *_out) noexcept nogil:
     fftw_execute_r2r(<fftw_plan>plan, <fftw_real *>_in, <fftw_real *>_out)
 
 cdef generic_function _get_execute_function(kind):
     if kind in (C2C_FORWARD, C2C_BACKWARD):
         return _fftw_execute_dft
     elif kind == R2C:
         return _fftw_execute_dft_r2c
```

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/fftw/utilities.pyx` & `mpi4py_fft-2.0.6/mpi4py_fft/fftw/utilities.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#cython: language_level=3
+#cython: language_level=3str
 
 cimport numpy as np
 import numpy as np
 from libc.stdint cimport intptr_t
 
 cpdef enum:
     FFTW_FORWARD  = -1
```

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/fftw/xfftn.py` & `mpi4py_fft-2.0.6/mpi4py_fft/fftw/xfftn.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/io/file_base.py` & `mpi4py_fft-2.0.6/mpi4py_fft/io/file_base.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/io/generate_xdmf.py` & `mpi4py_fft-2.0.6/mpi4py_fft/io/generate_xdmf.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/io/h5py_file.py` & `mpi4py_fft-2.0.6/mpi4py_fft/io/h5py_file.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/io/nc_file.py` & `mpi4py_fft-2.0.6/mpi4py_fft/io/nc_file.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/libfft.py` & `mpi4py_fft-2.0.6/mpi4py_fft/libfft.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/mpifft.py` & `mpi4py_fft-2.0.6/mpi4py_fft/mpifft.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft/pencil.py` & `mpi4py_fft-2.0.6/mpi4py_fft/pencil.py`

 * *Files identical despite different names*

### Comparing `mpi4py-fft-2.0.5/mpi4py_fft.egg-info/PKG-INFO` & `mpi4py_fft-2.0.6/mpi4py_fft.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: mpi4py-fft
-Version: 2.0.5
+Version: 2.0.6
 Summary: mpi4py-fft -- Parallel Fast Fourier Transforms (FFTs) using MPI for Python
-Home-page: https://bitbucket.org/mpi4py/mpi4py-fft
+Home-page: https://github.com/mpi4py/mpi4py-fft
 Author: Lisandro Dalcin and Mikael Mortensen
-License: UNKNOWN
 Keywords: Python,FFTW,FFT,DCT,DST,MPI
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
+Requires-Dist: mpi4py
+Requires-Dist: numpy
 
 mpi4py-fft
 ----------
 
 
 .. image:: https://dev.azure.com/mpi4py/mpi4py-fft/_apis/build/status/mpi4py.mpi4py-fft?branchName=master
     :target: https://dev.azure.com/mpi4py/mpi4py-fft
@@ -96,9 +97,7 @@
 
 For IO you need to install either `h5py <https://www.h5py.org>`_ or
 `netCDF4 <http://unidata.github.io/netcdf4-python/>`_ with support for
 MPI. Both are available from the coda-forge channel through::
 
     conda install -c conda-forge h5py=*=mpi* netcdf4=*=mpi*
 
-
-
```

### Comparing `mpi4py-fft-2.0.5/setup.py` & `mpi4py_fft-2.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
+"""mpi4py-fft -- Parallel Fast Fourier Transforms (FFTs) using MPI for Python"""
 
 import os
 import sys
 import re
 import platform
 import sysconfig
 from distutils import ccompiler
+from distutils.errors import DistutilsPlatformError
 from setuptools import setup
 from setuptools.dist import Distribution
 from setuptools.extension import Extension
 import numpy
 
 cwd = os.path.abspath(os.path.dirname(__file__))
 fftwdir = os.path.join(cwd, 'mpi4py_fft', 'fftw')
@@ -29,14 +31,16 @@
     for envvar in ('FFTW_ROOT', 'FFTW_DIR'):
         if envvar in os.environ:
             prefix = os.environ[envvar]
             append(dirs, prefix)
     append(dirs, sys.prefix)
     if 'CONDA_BUILD' not in os.environ:
         append(dirs, '/usr')
+        append(dirs, '/usr/local')
+        append(dirs, '/opt/homebrew')
     return dirs
 
 def get_include_dirs():
     dirs = []
     if 'FFTW_INCLUDE_DIR' in os.environ:
         entry = os.environ['FFTW_INCLUDE_DIR']
         append(dirs, entry)
@@ -67,20 +71,28 @@
         tlib = lib+'_threads'
         if compiler.find_library_file(library_dirs, lib):
             libs[d] = [lib]
             if compiler.find_library_file(library_dirs, tlib):
                 libs[d].append(tlib)
             if os.name == 'posix':
                 libs[d].append('m')
-    assert len(libs) > 0, "No FFTW libraries found in {}".format(library_dirs)
+    if not libs:
+        message = "No FFTW libraries found in {}".format(library_dirs)
+        raise DistutilsPlatformError(message)
     return libs
 
 def generate_extensions(fftwlibs, force=True):
     """Generate files with float and long double"""
-    from distutils.dep_util import newer_group
+    try:
+        from setuptools.modified import newer_group
+    except ImportError:
+        try:
+            from setuptools.dep_util import newer_group
+        except ImportError:
+            from distutils.dep_util import newer_group
 
     for d in fftwlibs:
         if d == 'double':
             continue
         p = 'fftw'+prec_map[d]+'_'
         for fname in (
                 'fftw_planxfftn.h',
@@ -97,58 +109,74 @@
                     code = re.sub('double', d, code)
                     with open(dst, 'w') as fout:
                         fout.write(code)
 
 def remove_extensions(fftwlibs):
     """Remove generated files"""
     for fname in (
-            'utilities.c',
-            'fftw_xfftn.c',
-            'fftwf_xfftn.c',
-            'fftwl_xfftn.c',
+        'utilities.c',
+        'fftw_xfftn.c',
+        'fftwf_xfftn.c',
+        'fftwl_xfftn.c',
     ):
         dst = os.path.join(fftwdir, fname)
         try:
             os.remove(dst)
         except OSError:
             pass
     for d in fftwlibs:
         if d == 'double':
             continue
         p = 'fftw'+prec_map[d]+'_'
         for fname in (
-                'fftw_planxfftn.h',
-                'fftw_planxfftn.c',
-                'fftw_xfftn.pyx',
-                'fftw_xfftn.pxd',
+            'fftw_planxfftn.h',
+            'fftw_planxfftn.c',
+            'fftw_xfftn.pyx',
+            'fftw_xfftn.pxd',
         ):
             dst = os.path.join(fftwdir, fname.replace('fftw_', p))
             try:
                 os.remove(dst)
             except OSError:
                 pass
 
 def get_extensions():
     """Return list of extension modules"""
     include_dirs = get_include_dirs()
     library_dirs = get_library_dirs()
-    ext = [Extension("mpi4py_fft.fftw.utilities",
-                     sources=[os.path.join(fftwdir, "utilities.pyx")],
-                     include_dirs=include_dirs)]
-
-    fftwlibs = get_fftw_libs()
+    ext = [
+        Extension(
+            "mpi4py_fft.fftw.utilities",
+            sources=[os.path.join(fftwdir, "utilities.pyx")],
+            define_macros=[('NPY_NO_DEPRECATED_API', 'NPY_1_7_API_VERSION')],
+            include_dirs=include_dirs,
+        ),
+    ]
+
+    sdist = 'sdist' in sys.argv
+    egg_info = 'egg_info' in sys.argv
+    fftwlibs = (
+        get_fftw_libs() if not (sdist or egg_info) else
+        {d: [] for d in ('float', 'double', 'long double')}
+    )
     for d, libs in fftwlibs.items():
-        p = 'fftw'+prec_map[d]+'_'
-        ext.append(Extension("mpi4py_fft.fftw.{}xfftn".format(p),
-                             sources=[os.path.join(fftwdir, "{}xfftn.pyx".format(p)),
-                                      os.path.join(fftwdir, "{}planxfftn.c".format(p))],
-                             #define_macros=[('NPY_NO_DEPRECATED_API', 'NPY_1_7_API_VERSION')],
-                             libraries=libs,
-                             include_dirs=include_dirs,
-                             library_dirs=library_dirs))
+        p = 'fftw' + prec_map[d] + '_'
+        ext.append(
+            Extension(
+                "mpi4py_fft.fftw.{}xfftn".format(p),
+                sources=[
+                    os.path.join(fftwdir, "{}xfftn.pyx".format(p)),
+                    os.path.join(fftwdir, "{}planxfftn.c".format(p)),
+                ],
+                define_macros=[('NPY_NO_DEPRECATED_API', 'NPY_1_7_API_VERSION')],
+                libraries=libs,
+                include_dirs=include_dirs,
+                library_dirs=library_dirs,
+            )
+        )
     return ext
 
 
 class Dist(Distribution):
 
     def get_command_class(self, command):
         get_command_class = Distribution.get_command_class
@@ -186,33 +214,37 @@
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 if __name__ == '__main__':
     setup(name="mpi4py-fft",
           version=version(),
-          description="mpi4py-fft -- Parallel Fast Fourier Transforms (FFTs) using MPI for Python",
+          description=__doc__.strip(),
           long_description=long_description,
+          long_description_content_type='text/x-rst',
           author="Lisandro Dalcin and Mikael Mortensen",
-          url='https://bitbucket.org/mpi4py/mpi4py-fft',
-          packages=["mpi4py_fft",
-                    "mpi4py_fft.fftw",
-                    "mpi4py_fft.io"],
-          package_dir={"mpi4py_fft": "mpi4py_fft"},
+          url="https://github.com/mpi4py/mpi4py-fft",
+          packages=[
+              "mpi4py_fft",
+              "mpi4py_fft.fftw",
+              "mpi4py_fft.io",
+          ],
+          package_dir={
+              "mpi4py_fft": "mpi4py_fft",
+          },
           classifiers=[
               'Development Status :: 4 - Beta',
               'Environment :: Console',
               'Intended Audience :: Developers',
               'Intended Audience :: Science/Research',
               'Programming Language :: Python',
               'Programming Language :: Python :: 2',
               'Programming Language :: Python :: 3',
               'License :: OSI Approved :: BSD License',
               'Topic :: Scientific/Engineering :: Mathematics',
               'Topic :: Software Development :: Libraries :: Python Modules',
-              ],
+          ],
+          keywords=['Python', 'FFTW', 'FFT', 'DCT', 'DST', 'MPI'],
           distclass=Dist,
           ext_modules=get_extensions(),
           install_requires=["mpi4py", "numpy"],
-          setup_requires=["setuptools>=18.0", "cython>=0.25"],
-          keywords=['Python', 'FFTW', 'FFT', 'DCT', 'DST', 'MPI']
          )
```

