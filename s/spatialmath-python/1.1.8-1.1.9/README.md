# Comparing `tmp/spatialmath-python-1.1.8.tar.gz` & `tmp/spatialmath-python-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialmath-python-1.1.8.tar", last modified: Wed May 10 21:12:21 2023, max compression
+gzip compressed data, was "spatialmath-python-1.1.9.tar", last modified: Wed Jan  3 17:06:35 2024, max compression
```

## Comparing `spatialmath-python-1.1.8.tar` & `spatialmath-python-1.1.9.tar`

### file list

```diff
@@ -1,60 +1,51 @@
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-10 21:12:21.353217 spatialmath-python-1.1.8/
--rw-r--r--   0 corkep     (503) staff       (20)     1068 2020-05-03 01:56:32.000000 spatialmath-python-1.1.8/LICENSE
--rw-rw----   0 corkep     (503) staff       (20)    15921 2023-05-10 21:12:21.352718 spatialmath-python-1.1.8/PKG-INFO
--rw-r--r--   0 corkep     (503) staff       (20)    14506 2023-03-08 07:55:36.000000 spatialmath-python-1.1.8/README.md
--rw-rw----   0 corkep     (503) staff       (20)     2238 2023-05-10 21:12:01.000000 spatialmath-python-1.1.8/pyproject.toml
--rw-rw----   0 corkep     (503) staff       (20)       38 2023-05-10 21:12:21.353324 spatialmath-python-1.1.8/setup.cfg
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-10 21:12:21.278752 spatialmath-python-1.1.8/spatialmath/
--rw-rw----   0 corkep     (503) staff       (20)    10757 2023-05-03 11:39:26.000000 spatialmath-python-1.1.8/spatialmath/DualQuaternion.py
--rw-rw----   0 corkep     (503) staff       (20)     1223 2023-03-06 05:53:49.000000 spatialmath-python-1.1.8/spatialmath/__init__.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-10 21:12:21.320152 spatialmath-python-1.1.8/spatialmath/base/
--rw-r--r--   0 corkep     (503) staff       (20)     6133 2023-03-15 07:14:42.000000 spatialmath-python-1.1.8/spatialmath/base/__init__.py
--rw-rw----   0 corkep     (503) staff       (20)     4376 2023-02-26 06:08:44.000000 spatialmath-python-1.1.8/spatialmath/base/_types_311.py
--rw-rw----   0 corkep     (503) staff       (20)     3668 2023-02-27 02:47:31.000000 spatialmath-python-1.1.8/spatialmath/base/_types_35.py
--rw-rw----   0 corkep     (503) staff       (20)     4453 2023-02-26 06:08:44.000000 spatialmath-python-1.1.8/spatialmath/base/_types_39.py
--rwxrwx---   0 corkep     (503) staff       (20)    28884 2023-03-21 10:14:47.000000 spatialmath-python-1.1.8/spatialmath/base/animate.py
--rw-r--r--   0 corkep     (503) staff       (20)      600 2021-05-23 01:42:29.000000 spatialmath-python-1.1.8/spatialmath/base/animationbug.py
--rw-r--r--   0 corkep     (503) staff       (20)    21504 2023-03-16 00:24:27.000000 spatialmath-python-1.1.8/spatialmath/base/argcheck.py
--rw-r--r--   0 corkep     (503) staff       (20)    62772 2023-04-23 00:46:05.000000 spatialmath-python-1.1.8/spatialmath/base/graphics.py
--rwxr--r--   0 corkep     (503) staff       (20)     2091 2021-05-23 01:42:29.000000 spatialmath-python-1.1.8/spatialmath/base/m2p.py
--rw-r--r--   0 corkep     (503) staff       (20)    11666 2023-03-06 07:02:14.000000 spatialmath-python-1.1.8/spatialmath/base/numeric.py
--rwxrwx---   0 corkep     (503) staff       (20)    29711 2023-03-28 10:16:43.000000 spatialmath-python-1.1.8/spatialmath/base/quaternions.py
--rw-rw----   0 corkep     (503) staff       (20)     6973 2023-02-27 02:51:57.000000 spatialmath-python-1.1.8/spatialmath/base/symbolic.py
--rw-r--r--   0 corkep     (503) staff       (20)     2526 2023-02-01 09:24:26.000000 spatialmath-python-1.1.8/spatialmath/base/timing.py
--rw-r--r--   0 corkep     (503) staff       (20)    45818 2023-03-28 11:10:08.000000 spatialmath-python-1.1.8/spatialmath/base/transforms2d.py
--rw-rw----   0 corkep     (503) staff       (20)   110878 2023-03-28 22:05:19.000000 spatialmath-python-1.1.8/spatialmath/base/transforms3d.py
--rw-rw----   0 corkep     (503) staff       (20)    24862 2023-03-26 07:02:50.000000 spatialmath-python-1.1.8/spatialmath/base/transformsNd.py
--rw-r--r--   0 corkep     (503) staff       (20)     1700 2023-02-01 09:24:27.000000 spatialmath-python-1.1.8/spatialmath/base/trplot2.py
--rw-rw----   0 corkep     (503) staff       (20)      229 2023-02-26 06:08:44.000000 spatialmath-python-1.1.8/spatialmath/base/types.py
--rw-rw----   0 corkep     (503) staff       (20)    19884 2023-03-26 23:53:23.000000 spatialmath-python-1.1.8/spatialmath/base/vectors.py
--rw-r--r--   0 corkep     (503) staff       (20)    23769 2023-05-10 02:44:03.000000 spatialmath-python-1.1.8/spatialmath/baseposelist.py
--rw-r--r--   0 corkep     (503) staff       (20)    62090 2023-05-10 10:13:23.000000 spatialmath-python-1.1.8/spatialmath/baseposematrix.py
--rwxr--r--   0 corkep     (503) staff       (20)    33281 2023-05-03 11:51:44.000000 spatialmath-python-1.1.8/spatialmath/geom2d.py
--rwxrwx---   0 corkep     (503) staff       (20)    44801 2023-05-03 11:49:05.000000 spatialmath-python-1.1.8/spatialmath/geom3d.py
--rw-r--r--   0 corkep     (503) staff       (20)      504 2023-02-19 01:27:48.000000 spatialmath-python-1.1.8/spatialmath/play_with_types.py
--rw-r--r--   0 corkep     (503) staff       (20)      669 2023-02-02 19:54:18.000000 spatialmath-python-1.1.8/spatialmath/pluckertest.py
--rw-rw----   0 corkep     (503) staff       (20)    19392 2023-05-03 11:56:11.000000 spatialmath-python-1.1.8/spatialmath/pose2d.py
--rw-r--r--   0 corkep     (503) staff       (20)    62953 2023-05-10 10:12:02.000000 spatialmath-python-1.1.8/spatialmath/pose3d.py
--rw-r--r--   0 corkep     (503) staff       (20)      194 2023-02-02 19:54:18.000000 spatialmath-python-1.1.8/spatialmath/profiling.py
--rw-rw----   0 corkep     (503) staff       (20)    78882 2023-05-03 11:46:14.000000 spatialmath-python-1.1.8/spatialmath/quaternion.py
--rw-rw----   0 corkep     (503) staff       (20)    25874 2023-02-26 06:08:44.000000 spatialmath-python-1.1.8/spatialmath/spatialvector.py
--rw-r--r--   0 corkep     (503) staff       (20)      666 2023-02-02 19:54:18.000000 spatialmath-python-1.1.8/spatialmath/test.py
--rwxrwx---   0 corkep     (503) staff       (20)     8106 2023-02-26 06:08:44.000000 spatialmath-python-1.1.8/spatialmath/timing.py
--rw-r--r--   0 corkep     (503) staff       (20)       69 2020-09-23 08:34:00.000000 spatialmath-python-1.1.8/spatialmath/timing_constructor.py
--rw-r--r--   0 corkep     (503) staff       (20)    55284 2023-05-10 20:32:19.000000 spatialmath-python-1.1.8/spatialmath/twist.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-10 21:12:21.343230 spatialmath-python-1.1.8/spatialmath_python.egg-info/
--rw-rw----   0 corkep     (503) staff       (20)    15921 2023-05-10 21:12:21.000000 spatialmath-python-1.1.8/spatialmath_python.egg-info/PKG-INFO
--rw-rw----   0 corkep     (503) staff       (20)     1449 2023-05-10 21:12:21.000000 spatialmath-python-1.1.8/spatialmath_python.egg-info/SOURCES.txt
--rw-rw----   0 corkep     (503) staff       (20)        1 2023-05-10 21:12:21.000000 spatialmath-python-1.1.8/spatialmath_python.egg-info/dependency_links.txt
--rw-rw----   0 corkep     (503) staff       (20)      230 2023-05-10 21:12:21.000000 spatialmath-python-1.1.8/spatialmath_python.egg-info/requires.txt
--rw-rw----   0 corkep     (503) staff       (20)       12 2023-05-10 21:12:21.000000 spatialmath-python-1.1.8/spatialmath_python.egg-info/top_level.txt
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-10 21:12:21.351768 spatialmath-python-1.1.8/tests/
--rw-r--r--   0 corkep     (503) staff       (20)     4072 2021-03-28 05:22:23.000000 spatialmath-python-1.1.8/tests/test_baseposelist.py
--rw-r--r--   0 corkep     (503) staff       (20)     3323 2021-01-16 23:30:46.000000 spatialmath-python-1.1.8/tests/test_dualquaternion.py
--rwxr--r--   0 corkep     (503) staff       (20)     8051 2023-03-08 02:59:23.000000 spatialmath-python-1.1.8/tests/test_geom2d.py
--rwxrwx---   0 corkep     (503) staff       (20)     9378 2023-02-26 06:08:44.000000 spatialmath-python-1.1.8/tests/test_geom3d.py
--rwxr--r--   0 corkep     (503) staff       (20)    13380 2021-04-06 10:29:33.000000 spatialmath-python-1.1.8/tests/test_pose2d.py
--rwxr--r--   0 corkep     (503) staff       (20)    33496 2021-04-06 10:29:51.000000 spatialmath-python-1.1.8/tests/test_pose3d.py
--rw-rw----   0 corkep     (503) staff       (20)    32754 2023-02-26 06:08:44.000000 spatialmath-python-1.1.8/tests/test_quaternion.py
--rw-r--r--   0 corkep     (503) staff       (20)     7266 2020-11-08 07:59:28.000000 spatialmath-python-1.1.8/tests/test_spatialvector.py
--rwxrwx---   0 corkep     (503) staff       (20)    10657 2023-02-26 06:08:44.000000 spatialmath-python-1.1.8/tests/test_twist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:06:35.887358 spatialmath-python-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17312 2024-01-03 17:06:35.887358 spatialmath-python-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 17:06:35.887358 spatialmath-python-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:06:35.879358 spatialmath-python-1.1.9/spatialmath/
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/DualQuaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:06:35.883358 spatialmath-python-1.1.9/spatialmath/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/_types_311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/_types_35.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/_types_39.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28880 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/argcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62772 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/numeric.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29956 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/quaternions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48675 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/transforms2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111398 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/transforms3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24948 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/transformsNd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21946 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/base/vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23769 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/baseposelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61986 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/baseposematrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33591 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/geom2d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44892 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/geom3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/pose2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68458 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/pose3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79429 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25876 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/spatialvector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8106 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55284 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/spatialmath/twist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:06:35.883358 spatialmath-python-1.1.9/spatialmath_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17312 2024-01-03 17:06:35.000000 spatialmath-python-1.1.9/spatialmath_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-03 17:06:35.000000 spatialmath-python-1.1.9/spatialmath_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 17:06:35.000000 spatialmath-python-1.1.9/spatialmath_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-03 17:06:35.000000 spatialmath-python-1.1.9/spatialmath_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-03 17:06:35.000000 spatialmath-python-1.1.9/spatialmath_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:06:35.883358 spatialmath-python-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/tests/test_baseposelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/tests/test_dualquaternion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8220 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/tests/test_geom2d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9547 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/tests/test_geom3d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12997 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/tests/test_pose2d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36441 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/tests/test_pose3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33830 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/tests/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/tests/test_spatialvector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10657 2024-01-03 17:06:19.000000 spatialmath-python-1.1.9/tests/test_twist.py
```

### Comparing `spatialmath-python-1.1.8/LICENSE` & `spatialmath-python-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/PKG-INFO` & `spatialmath-python-1.1.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,35 @@
-Metadata-Version: 2.1
-Name: spatialmath-python
-Version: 1.1.8
-Summary: Provides spatial maths capability for Python
-Author-email: Peter Corke <rvc@petercorke.com>
-Project-URL: Homepage, https://github.com/petercorke/spatialmath-python
-Project-URL: Bug Tracker, https://github.com/petercorke/spatialmath-python/issues
-Project-URL: Documentation, https://petercorke.github.io/petercorke/spatialmath-python
-Project-URL: Source, https://github.com/petercorke/petercorke/spatialmath-python
-Keywords: spatial-math,spatial math,SO2,SE2,SO3,SE3,SO(2),SE(2),SO(3),SE(3),twist,product of exponential,translation,orientation,angle-axis,Lie group,skew symmetric matrix,pose,translation,rotation matrix,rigid body transform,homogeneous transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-quaternion,robotics,robot vision,computer vision
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 # Spatial Maths for Python
 
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 
 [![PyPI version](https://badge.fury.io/py/spatialmath-python.svg)](https://badge.fury.io/py/spatialmath-python)
 [![Anaconda version](https://anaconda.org/conda-forge/spatialmath-python/badges/version.svg)](https://anaconda.org/conda-forge/spatialmath-python)
 ![Python Version](https://img.shields.io/pypi/pyversions/spatialmath-python.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-[![Build Status](https://github.com/petercorke/spatialmath-python/workflows/build/badge.svg?branch=master)](https://github.com/petercorke/spatialmath-python/actions?query=workflow%3Abuild)
-[![Coverage](https://codecov.io/gh/petercorke/spatialmath-python/branch/master/graph/badge.svg)](https://codecov.io/gh/petercorke/spatialmath-python)
+[![Build Status](https://github.com/bdaiinstitute/spatialmath-python/actions/workflows/master.yml/badge.svg?branch=master)](https://github.com/bdaiinstitute/spatialmath-python/actions/workflows/master.yml?query=workflow%3Abuild+branch%3Amaster)
+[![Coverage](https://codecov.io/github/bdaiinstitute/spatialmath-python/graph/badge.svg?token=W15FGBA059)](https://codecov.io/github/bdaiinstitute/spatialmath-python)
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/spatialmath-python)](https://pypistats.org/packages/spatialmath-python)
-[![GitHub stars](https://img.shields.io/github/stars/petercorke/spatialmath-python.svg?style=social&label=Star)](https://GitHub.com/petercorke/spatialmath-python/stargazers/)
+[![GitHub stars](https://img.shields.io/github/stars/bdaiinstitute/spatialmath-python.svg?style=social&label=Star)](https://GitHub.com/bdaiinstitute/spatialmath-python/stargazers/)
 
 
 
 <table style="border:0px">
 <tr style="border:0px">
 <td style="border:0px">
-<img src="https://github.com/petercorke/spatialmath-python/raw/master/docs/figs/CartesianSnakes_LogoW.png" width="200"></td>
+<img src="https://github.com/bdaiinstitute/spatialmath-python/raw/master/docs/figs/CartesianSnakes_LogoW.png" width="200"></td>
 <td style="border:0px">
 A Python implementation of the <a href="https://github.com/petercorke/spatial-math">Spatial Math Toolbox for MATLAB<sup>&reg;</sup></a>
 <ul>
-<li><a href="https://github.com/petercorke/spatialmath-python">GitHub repository </a></li>
-<li><a href="https://petercorke.github.io/spatialmath-python">Documentation</a></li>
-<li><a href=https://github.com/petercorke/spatialmath-python/discussions/categories/changes>Recent changes</a>
-<li><a href="https://github.com/petercorke/spatialmath-python/wiki">Wiki (examples and details)</a></li>
+<li><a href="https://github.com/bdaiinstitute/spatialmath-python">GitHub repository </a></li>
+<li><a href="https://bdaiinstitute.github.io/spatialmath-python">Documentation</a></li>
+<li><a href=https://github.com/bdaiinstitute/spatialmath-python/discussions/categories/changes>Recent changes</a>
+<li><a href="https://github.com/bdaiinstitute/spatialmath-python/wiki">Wiki (examples and details)</a></li>
 <li><a href="installation#">Installation</a></li>
 </ul>
 </td>
 </tr>
 </table>
 
 Spatial mathematics capability underpins all of robotics and robotic vision where we need to describe the position, orientation or pose of objects in 2D or 3D spaces.
@@ -95,15 +70,15 @@
  * conversion of orientation to/from Euler angles, roll-pitch-yaw angles and angle-axis forms.
  * list operations such as append, insert and get
 
 These are layered over a set of base functions that perform many of the same operations but represent data explicitly in terms of `numpy` arrays.
 
 The class, method and functions names largely mirror those of the MATLAB toolboxes, and the semantics are quite similar.
 
-![trplot](https://github.com/petercorke/spatialmath-python/raw/master/docs/figs/fig1.png)
+![trplot](https://github.com/bdaiinstitute/spatialmath-python/raw/master/docs/figs/fig1.png)
 
 ![animation video](./docs/figs/animate.gif)
 
 # Citing
 
 Check out our ICRA 2021 paper on [IEEE Xplore](https://ieeexplore.ieee.org/document/9561366) or get the PDF from [Peter's website](https://bit.ly/icra_rtb).  This describes the [Robotics Toolbox for Python](https://github.com/petercorke/robotics-toolbox-python) as well Spatial Maths.
 
@@ -124,20 +99,20 @@
 
 <a id='6'></a>
 
 ## Using the Toolbox in your Open Source Code?
 
 If you are using the Toolbox in your open source code, feel free to add our badge to your readme!
 
-[![Powered by the Robotics Toolbox](https://github.com/petercorke/spatialmath-python/raw/master/.github/svg/sm_powered.min.svg)](https://github.com/petercorke/spatialmath-python)
+[![Powered by the Spatial Math Toolbox](https://github.com/bdaiinstitute/spatialmath-python/raw/master/.github/svg/sm_powered.min.svg)](https://github.com/bdaiinstitute/spatialmath-python)
 
 Simply copy the following
 
 ```
-[![Powered by the Spatial Math Toolbox](https://github.com/petercorke/spatialmath-python/raw/master/.github/svg/sm_powered.min.svg)](https://github.com/petercorke/spatialmath-python)
+[![Powered by the Spatial Math Toolbox](https://github.com/bdaiinstitute/spatialmath-python/raw/master/.github/svg/sm_powered.min.svg)](https://github.com/bdaiinstitute/spatialmath-python)
 ```
 
 
 # Installation
 
 ## Using pip
 
@@ -148,17 +123,19 @@
 ```
 
 ## From GitHub
 
 Install the current code base from GitHub and pip install a link to that cloned copy
 
 ```
-git clone https://github.com/petercorke/spatialmath-python.git
+git clone https://github.com/bdaiinstitute/spatialmath-python.git
 cd spatialmath-python
 pip install -e .
+# Optional: if you would like to contribute and commit code changes to the repository,
+# pre-commit install
 ```
 
 ## Dependencies
 
 `numpy`, `scipy`, `matplotlib`, `ffmpeg` (if rendering animations as a movie)
 
 # Examples
@@ -290,22 +267,22 @@
 
 >>> T.printline()
 t =        1,        2,        3; rpy/zyx =       30,        0,        0 deg
 
 >>> T.plot()
 ```
 
-![trplot](https://github.com/petercorke/spatialmath-python/raw/master/docs/figs/fig1.png)
+![trplot](https://github.com/bdaiinstitute/spatialmath-python/raw/master/docs/figs/fig1.png)
 
 `printline` is a compact single line format for tabular listing, whereas `print` shows the underlying matrix and for consoles that support it, it is colorised, with rotational elements in red and translational elements in blue.
 
 For more detail checkout the shipped Python notebooks:
 
-* [gentle introduction](https://github.com/petercorke/spatialmath-python/blob/master/spatialmath/gentle-introduction.ipynb)
-* [deeper introduction](https://github.com/petercorke/spatialmath-python/blob/master/spatialmath/introduction.ipynb)
+* [gentle introduction](https://github.com/bdaiinstitute/spatialmath-python/blob/master/notebooks/gentle-introduction.ipynb)
+* [deeper introduction](https://github.com/bdaiinstitute/spatialmath-python/blob/master/notebooks/introduction.ipynb)
 
 
 You can browse it statically through the links above, or clone the toolbox and run them interactively using [Jupyter](https://jupyter.org) or [JupyterLab](https://jupyter.org).
 
 
 ## Low-level spatial math
 
@@ -383,15 +360,15 @@
 -60.000000 < 12.000000, 30.000000, 24.000000 >
 >>> qnorm(q)
 72.24956747275377
 ```
 
 ## Graphics
 
-![trplot](https://github.com/petercorke/spatialmath-python/raw/master/docs/figs/transforms3d.png)
+![trplot](https://github.com/bdaiinstitute/spatialmath-python/raw/master/docs/figs/transforms3d.png)
 
 The functions support various plotting styles
 
 ```
 trplot( transl(1,2,3), frame='A', rviz=True, width=1, dims=[0, 10, 0, 10, 0, 10])
 trplot( transl(3,1, 2), color='red', width=3, frame='B')
 trplot( transl(4, 3, 1)@trotx(math.pi/3), color='green', frame='c', dims=[0,4,0,4,0,4])
@@ -457,14 +434,12 @@
 type(a)
 Out[255]: cos
 ```
 We see that the symbolic constants are converted back to Python numeric types on read.
 
 Similarly when we assign an element or slice of the symbolic matrix to a numeric value, they are converted to symbolic constants on the way in.
 
+## History & Contributors
 
+This package was originally created by [Peter Corke](https://github.com/petercorke) and [Jesse Haviland](https://github.com/jhavl) and was inspired by the [Spatial Math Toolbox for MATLAB](https://github.com/petercorke/spatialmath-matlab).  It supports the textbook [Robotics, Vision & Control in Python 3e](https://github.com/petercorke/RVC3-python).
 
-
-
-
-
-
+The package is now a collaboration with [Boston Dynamics AI Institute](https://theaiinstitute.com/).
```

#### html2text {}

```diff
@@ -1,49 +1,32 @@
-Metadata-Version: 2.1 Name: spatialmath-python Version: 1.1.8 Summary: Provides
-spatial maths capability for Python Author-email: Peter Corke
-petercorke.com> Project-URL: Homepage, https://github.com/petercorke/
-spatialmath-python Project-URL: Bug Tracker, https://github.com/petercorke/
-spatialmath-python/issues Project-URL: Documentation, https://
-petercorke.github.io/petercorke/spatialmath-python Project-URL: Source, https:/
-/github.com/petercorke/petercorke/spatialmath-python Keywords: spatial-
-math,spatial math,SO2,SE2,SO3,SE3,SO(2),SE(2),SO(3),SE(3),twist,product of
-exponential,translation,orientation,angle-axis,Lie group,skew symmetric
-matrix,pose,translation,rotation matrix,rigid body transform,homogeneous
-transformation,Euler angles,roll-pitch-yaw angles,quaternion,unit-
-quaternion,robotics,robot vision,computer vision Classifier: Development Status
-:: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
-docs License-File: LICENSE # Spatial Maths for Python [![A Python Robotics
-Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/
-master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/
-robotics-toolbox-python) [![QUT Centre for Robotics Open Source](https://
-github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
-[![PyPI version](https://badge.fury.io/py/spatialmath-python.svg)](https://
+# Spatial Maths for Python [![A Python Robotics Package](https://
+raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/
+svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-
+python) [![QUT Centre for Robotics Open Source](https://github.com/qcr/
+qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io) [![PyPI
+version](https://badge.fury.io/py/spatialmath-python.svg)](https://
 badge.fury.io/py/spatialmath-python) [![Anaconda version](https://anaconda.org/
 conda-forge/spatialmath-python/badges/version.svg)](https://anaconda.org/conda-
 forge/spatialmath-python) ![Python Version](https://img.shields.io/pypi/
 pyversions/spatialmath-python.svg) [![License: MIT](https://img.shields.io/
 badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Build
-Status](https://github.com/petercorke/spatialmath-python/workflows/build/
-badge.svg?branch=master)](https://github.com/petercorke/spatialmath-python/
-actions?query=workflow%3Abuild) [![Coverage](https://codecov.io/gh/petercorke/
-spatialmath-python/branch/master/graph/badge.svg)](https://codecov.io/gh/
-petercorke/spatialmath-python) [![PyPI - Downloads](https://img.shields.io/
-pypi/dw/spatialmath-python)](https://pypistats.org/packages/spatialmath-python)
-[![GitHub stars](https://img.shields.io/github/stars/petercorke/spatialmath-
-python.svg?style=social&label=Star)](https://GitHub.com/petercorke/spatialmath-
-python/stargazers/)
+Status](https://github.com/bdaiinstitute/spatialmath-python/actions/workflows/
+master.yml/badge.svg?branch=master)](https://github.com/bdaiinstitute/
+spatialmath-python/actions/workflows/
+master.yml?query=workflow%3Abuild+branch%3Amaster) [![Coverage](https://
+codecov.io/github/bdaiinstitute/spatialmath-python/graph/
+badge.svg?token=W15FGBA059)](https://codecov.io/github/bdaiinstitute/
+spatialmath-python) [![PyPI - Downloads](https://img.shields.io/pypi/dw/
+spatialmath-python)](https://pypistats.org/packages/spatialmath-python) [!
+[GitHub stars](https://img.shields.io/github/stars/bdaiinstitute/spatialmath-
+python.svg?style=social&label=Star)](https://GitHub.com/bdaiinstitute/
+spatialmath-python/stargazers/)
                                          A Python implementation of the _S_p_a_t_i_a_l
                                          _M_a_t_h_ _T_o_o_l_b_o_x_ _f_o_r_ _M_A_T_L_A_B_®
-[https://github.com/petercorke/              * _G_i_t_H_u_b_ _r_e_p_o_s_i_t_o_r_y
+[https://github.com/bdaiinstitute/           * _G_i_t_H_u_b_ _r_e_p_o_s_i_t_o_r_y
 spatialmath-python/raw/master/docs/figs/     * _D_o_c_u_m_e_n_t_a_t_i_o_n
 CartesianSnakes_LogoW.png]                   * _R_e_c_e_n_t_ _c_h_a_n_g_e_s
                                              * _W_i_k_i_ _(_e_x_a_m_p_l_e_s_ _a_n_d_ _d_e_t_a_i_l_s_)
                                              * _I_n_s_t_a_l_l_a_t_i_o_n
 Spatial mathematics capability underpins all of robotics and robotic vision
 where we need to describe the position, orientation or pose of objects in 2D or
 3D spaces. # What it does The package provides classes to represent pose and
@@ -66,129 +49,137 @@
 operator * exponent, using the `**` operator * normalization * inversion *
 connection to the Lie algebra via matrix exponential and logarithm operations *
 conversion of orientation to/from Euler angles, roll-pitch-yaw angles and
 angle-axis forms. * list operations such as append, insert and get These are
 layered over a set of base functions that perform many of the same operations
 but represent data explicitly in terms of `numpy` arrays. The class, method and
 functions names largely mirror those of the MATLAB toolboxes, and the semantics
-are quite similar. ![trplot](https://github.com/petercorke/spatialmath-python/
-raw/master/docs/figs/fig1.png) ![animation video](./docs/figs/animate.gif) #
-Citing Check out our ICRA 2021 paper on [IEEE Xplore](https://
+are quite similar. ![trplot](https://github.com/bdaiinstitute/spatialmath-
+python/raw/master/docs/figs/fig1.png) ![animation video](./docs/figs/
+animate.gif) # Citing Check out our ICRA 2021 paper on [IEEE Xplore](https://
 ieeexplore.ieee.org/document/9561366) or get the PDF from [Peter's website]
 (https://bit.ly/icra_rtb). This describes the [Robotics Toolbox for Python]
 (https://github.com/petercorke/robotics-toolbox-python) as well Spatial Maths.
 If the toolbox helped you in your research, please cite ``` @inproceedings{rtb,
 title={Not your grandmotherâs toolbox--the Robotics Toolbox reinvented for
 Python}, author={Corke, Peter and Haviland, Jesse}, booktitle={2021 IEEE
 International Conference on Robotics and Automation (ICRA)}, pages={11357--
 11363}, year={2021}, organization={IEEE} } ```
 ## Using the Toolbox in your Open Source Code? If you are using the Toolbox in
 your open source code, feel free to add our badge to your readme! [![Powered by
-the Robotics Toolbox](https://github.com/petercorke/spatialmath-python/raw/
-master/.github/svg/sm_powered.min.svg)](https://github.com/petercorke/
+the Spatial Math Toolbox](https://github.com/bdaiinstitute/spatialmath-python/
+raw/master/.github/svg/sm_powered.min.svg)](https://github.com/bdaiinstitute/
 spatialmath-python) Simply copy the following ``` [![Powered by the Spatial
-Math Toolbox](https://github.com/petercorke/spatialmath-python/raw/
-master/.github/svg/sm_powered.min.svg)](https://github.com/petercorke/
+Math Toolbox](https://github.com/bdaiinstitute/spatialmath-python/raw/
+master/.github/svg/sm_powered.min.svg)](https://github.com/bdaiinstitute/
 spatialmath-python) ``` # Installation ## Using pip Install a snapshot from
 PyPI ``` pip install spatialmath-python ``` ## From GitHub Install the current
 code base from GitHub and pip install a link to that cloned copy ``` git clone
-https://github.com/petercorke/spatialmath-python.git cd spatialmath-python pip
-install -e . ``` ## Dependencies `numpy`, `scipy`, `matplotlib`, `ffmpeg` (if
-rendering animations as a movie) # Examples ## High-level classes These classes
-abstract the low-level numpy arrays into objects that obey the rules associated
-with the mathematical groups SO(2), SE(2), SO(3), SE(3) as well as twists and
-quaternions. Using classes ensures type safety, for example it stops us mixing
-a 2D homogeneous transformation with a 3D rotation matrix -- both of which are
-3x3 matrices. It also ensures that the internal matrix representation is always
-a valid member of the relevant group. For example, to create an object
-representing a rotation of 0.3 radians about the x-axis is simply ```python >>>
-from spatialmath import SO3, SE3 >>> R1 = SO3.Rx(0.3) >>> R1 1 0 0 0 0.955336 -
-0.29552 0 0.29552 0.955336 ``` while a rotation of 30 deg about the z-axis is
-```python >>> R2 = SO3.Rz(30, 'deg') >>> R2 0.866025 -0.5 0 0.5 0.866025 0 0 0
-1 ``` and the composition of these two rotations is ```python >>> R = R1 * R2
-0.866025 -0.5 0 0.433013 0.75 -0.5 0.25 0.433013 0.866025 ``` We can find the
-corresponding Euler angles (in radians) ```python >> R.eul() array([-
-1.57079633, 0.52359878, 2.0943951 ]) ``` Frequently in robotics we want a
-sequence, a trajectory, of rotation matrices or poses. These pose classes
-inherit capability from the `list` class ```python >>> R = SO3() # the null
-rotation or identity matrix >>> R.append(R1) >>> R.append(R2) >>> len(R) 3 >>>
-R[1] 1 0 0 0 0.955336 -0.29552 0 0.29552 0.955336 ``` and this can be used in
-`for` loops and list comprehensions. An alternative way of constructing this
-would be (`R1`, `R2` defined above) ```python >>> R = SO3( [ SO3(), R1, R2 ] )
->>> len(R) 3 ``` Many of the constructors such as `.Rx`, `.Ry` and `.Rz`
-support vectorization ```python >>> R = SO3.Rx( np.arange(0, 2*np.pi, 0.2)) >>>
-len(R) 32 ``` which has created, in a single line, a list of rotation matrices.
-Vectorization also applies to the operators, for instance ```python >>> A = R *
-SO3.Ry(0.5) >>> len(R) 32 ``` will produce a result where each element is the
-product of each element of the left-hand side with the right-hand side, ie. `R
-[i] * SO3.Ry(0.5)`. Similarly ```python >>> A = SO3.Ry(0.5) * R >>> len(R) 32
-``` will produce a result where each element is the product of the left-hand
-side with each element of the right-hand side , ie. `SO3.Ry(0.5) * R[i] `.
-Finally ```python >>> A = R * R >>> len(R) 32 ``` will produce a result where
-each element is the product of each element of the left-hand side with each
-element of the right-hand side , ie. `R[i] * R[i] `. The underlying
-representation of these classes is a numpy matrix, but the class ensures that
-the structure of that matrix is valid for the particular group represented: SO
-(2), SE(2), SO(3), SE(3). Any operation that is not valid for the group will
-return a matrix rather than a pose class, for example ```python >>> SO3.Rx(0.3)
-* 2 array([[ 2. , 0. , 0. ], [ 0. , 1.91067298, -0.59104041], [ 0. ,
-0.59104041, 1.91067298]]) >>> SO3.Rx(0.3) - 1 array([[ 0. , -1. , -1. ], [-1. ,
--0.04466351, -1.29552021], [-1. , -0.70447979, -0.04466351]]) ``` We can print
-and plot these objects as well ``` >>> T = SE3(1,2,3) * SE3.Rx(30, 'deg') >>>
-T.print() 1 0 0 1 0 0.866025 -0.5 2 0 0.5 0.866025 3 0 0 0 1 >>> T.printline()
-t = 1, 2, 3; rpy/zyx = 30, 0, 0 deg >>> T.plot() ``` ![trplot](https://
-github.com/petercorke/spatialmath-python/raw/master/docs/figs/fig1.png)
-`printline` is a compact single line format for tabular listing, whereas
-`print` shows the underlying matrix and for consoles that support it, it is
-colorised, with rotational elements in red and translational elements in blue.
-For more detail checkout the shipped Python notebooks: * [gentle introduction]
-(https://github.com/petercorke/spatialmath-python/blob/master/spatialmath/
-gentle-introduction.ipynb) * [deeper introduction](https://github.com/
-petercorke/spatialmath-python/blob/master/spatialmath/introduction.ipynb) You
-can browse it statically through the links above, or clone the toolbox and run
-them interactively using [Jupyter](https://jupyter.org) or [JupyterLab](https:/
-/jupyter.org). ## Low-level spatial math Import the low-level transform
-functions ``` >>> from spatialmath.base import * ``` We can create a 3D
-rotation matrix ``` >>> rotx(0.3) array([[ 1. , 0. , 0. ], [ 0. , 0.95533649, -
-0.29552021], [ 0. , 0.29552021, 0.95533649]]) >>> rotx(30, unit='deg') array([
-[ 1. , 0. , 0. ], [ 0. , 0.8660254, -0.5 ], [ 0. , 0.5 , 0.8660254]]) ``` The
-results are `numpy` arrays so to perform matrix multiplication you need to use
-the `@` operator, for example ``` rotx(0.3) @ roty(0.2) ``` We also support
-multiple ways of passing vector information to functions that require it: * as
-separate positional arguments ``` transl2(1, 2) array([[1., 0., 1.], [0., 1.,
-2.], [0., 0., 1.]]) ``` * as a list or a tuple ``` transl2( [1,2] ) array([[1.,
-0., 1.], [0., 1., 2.], [0., 0., 1.]]) transl2( (1,2) ) Out[444]: array([[1.,
-0., 1.], [0., 1., 2.], [0., 0., 1.]]) ``` * or as a `numpy` array ``` transl2
-( np.array([1,2]) ) Out[445]: array([[1., 0., 1.], [0., 1., 2.], [0., 0., 1.]])
-``` There is a single module that deals with quaternions, unit or not, and the
-representation is a `numpy` array of four elements. As above, functions can
-accept the `numpy` array, a list, dict or `numpy` row or column vectors. ```
->>> from spatialmath.base.quaternion import * >>> q = qqmul([1,2,3,4],
-[5,6,7,8]) >>> q array([-60, 12, 30, 24]) >>> qprint(q) -60.000000 < 12.000000,
-30.000000, 24.000000 > >>> qnorm(q) 72.24956747275377 ``` ## Graphics ![trplot]
-(https://github.com/petercorke/spatialmath-python/raw/master/docs/figs/
-transforms3d.png) The functions support various plotting styles ``` trplot
-( transl(1,2,3), frame='A', rviz=True, width=1, dims=[0, 10, 0, 10, 0, 10])
-trplot( transl(3,1, 2), color='red', width=3, frame='B') trplot( transl(4, 3,
-1)@trotx(math.pi/3), color='green', frame='c', dims=[0,4,0,4,0,4]) ```
-Animation is straightforward ``` tranimate(transl(4, 3, 4)@trotx(2)@troty(-2),
-frame='A', arrow=False, dims=[0, 5], nframes=200) ``` and it can be saved to a
-file by ``` tranimate(transl(4, 3, 4)@trotx(2)@troty(-2), frame='A',
-arrow=False, dims=[0, 5], nframes=200, movie='out.mp4') ``` ![animation video]
-(./docs/figs/animate.gif) At the moment we can only save as an MP4, but the
-following incantation will covert that to an animated GIF for embedding in web
-pages ``` ffmpeg -i out -r 20 -vf "fps=10,scale=640:-1:flags=lanczos,split[s0]
-[s1];[s0]palettegen[p];[s1][p]paletteuse" out.gif ``` For use in a Jupyter
-notebook, or on Colab, you can display an animation by ``` from
-IPython.core.display import HTML HTML(tranimate(transl(4, 3, 4)@trotx(2)@troty
-(-2), frame='A', arrow=False, dims=[0, 5], nframes=200, movie=True)) ``` The
-`movie=True` option causes `tranimate` to output an HTML5 fragment which is
-displayed inline by the `HTML` function. ## Symbolic support Some functions
-have support for symbolic variables, for example ``` import sympy theta =
-sym.symbols('theta') print(rotx(theta)) [[1 0 0] [0 cos(theta) -sin(theta)] [0
-sin(theta) cos(theta)]] ``` The resulting `numpy` array is an array of symbolic
-objects not numbers – the constants are also symbolic objects. You can read the
-elements of the matrix ``` a = T[0,0] a Out[258]: 1 type(a) Out[259]: int a = T
-[1,1] a Out[256]: cos(theta) type(a) Out[255]: cos ``` We see that the symbolic
-constants are converted back to Python numeric types on read. Similarly when we
-assign an element or slice of the symbolic matrix to a numeric value, they are
-converted to symbolic constants on the way in.
+https://github.com/bdaiinstitute/spatialmath-python.git cd spatialmath-python
+pip install -e . # Optional: if you would like to contribute and commit code
+changes to the repository, # pre-commit install ``` ## Dependencies `numpy`,
+`scipy`, `matplotlib`, `ffmpeg` (if rendering animations as a movie) # Examples
+## High-level classes These classes abstract the low-level numpy arrays into
+objects that obey the rules associated with the mathematical groups SO(2), SE
+(2), SO(3), SE(3) as well as twists and quaternions. Using classes ensures type
+safety, for example it stops us mixing a 2D homogeneous transformation with a
+3D rotation matrix -- both of which are 3x3 matrices. It also ensures that the
+internal matrix representation is always a valid member of the relevant group.
+For example, to create an object representing a rotation of 0.3 radians about
+the x-axis is simply ```python >>> from spatialmath import SO3, SE3 >>> R1 =
+SO3.Rx(0.3) >>> R1 1 0 0 0 0.955336 -0.29552 0 0.29552 0.955336 ``` while a
+rotation of 30 deg about the z-axis is ```python >>> R2 = SO3.Rz(30, 'deg') >>>
+R2 0.866025 -0.5 0 0.5 0.866025 0 0 0 1 ``` and the composition of these two
+rotations is ```python >>> R = R1 * R2 0.866025 -0.5 0 0.433013 0.75 -0.5 0.25
+0.433013 0.866025 ``` We can find the corresponding Euler angles (in radians)
+```python >> R.eul() array([-1.57079633, 0.52359878, 2.0943951 ]) ```
+Frequently in robotics we want a sequence, a trajectory, of rotation matrices
+or poses. These pose classes inherit capability from the `list` class ```python
+>>> R = SO3() # the null rotation or identity matrix >>> R.append(R1) >>>
+R.append(R2) >>> len(R) 3 >>> R[1] 1 0 0 0 0.955336 -0.29552 0 0.29552 0.955336
+``` and this can be used in `for` loops and list comprehensions. An alternative
+way of constructing this would be (`R1`, `R2` defined above) ```python >>> R =
+SO3( [ SO3(), R1, R2 ] ) >>> len(R) 3 ``` Many of the constructors such as
+`.Rx`, `.Ry` and `.Rz` support vectorization ```python >>> R = SO3.Rx
+( np.arange(0, 2*np.pi, 0.2)) >>> len(R) 32 ``` which has created, in a single
+line, a list of rotation matrices. Vectorization also applies to the operators,
+for instance ```python >>> A = R * SO3.Ry(0.5) >>> len(R) 32 ``` will produce a
+result where each element is the product of each element of the left-hand side
+with the right-hand side, ie. `R[i] * SO3.Ry(0.5)`. Similarly ```python >>> A =
+SO3.Ry(0.5) * R >>> len(R) 32 ``` will produce a result where each element is
+the product of the left-hand side with each element of the right-hand side ,
+ie. `SO3.Ry(0.5) * R[i] `. Finally ```python >>> A = R * R >>> len(R) 32 ```
+will produce a result where each element is the product of each element of the
+left-hand side with each element of the right-hand side , ie. `R[i] * R[i] `.
+The underlying representation of these classes is a numpy matrix, but the class
+ensures that the structure of that matrix is valid for the particular group
+represented: SO(2), SE(2), SO(3), SE(3). Any operation that is not valid for
+the group will return a matrix rather than a pose class, for example ```python
+>>> SO3.Rx(0.3) * 2 array([[ 2. , 0. , 0. ], [ 0. , 1.91067298, -0.59104041],
+[ 0. , 0.59104041, 1.91067298]]) >>> SO3.Rx(0.3) - 1 array([[ 0. , -1. , -1. ],
+[-1. , -0.04466351, -1.29552021], [-1. , -0.70447979, -0.04466351]]) ``` We can
+print and plot these objects as well ``` >>> T = SE3(1,2,3) * SE3.Rx(30, 'deg')
+>>> T.print() 1 0 0 1 0 0.866025 -0.5 2 0 0.5 0.866025 3 0 0 0 1 >>>
+T.printline() t = 1, 2, 3; rpy/zyx = 30, 0, 0 deg >>> T.plot() ``` ![trplot]
+(https://github.com/bdaiinstitute/spatialmath-python/raw/master/docs/figs/
+fig1.png) `printline` is a compact single line format for tabular listing,
+whereas `print` shows the underlying matrix and for consoles that support it,
+it is colorised, with rotational elements in red and translational elements in
+blue. For more detail checkout the shipped Python notebooks: * [gentle
+introduction](https://github.com/bdaiinstitute/spatialmath-python/blob/master/
+notebooks/gentle-introduction.ipynb) * [deeper introduction](https://
+github.com/bdaiinstitute/spatialmath-python/blob/master/notebooks/
+introduction.ipynb) You can browse it statically through the links above, or
+clone the toolbox and run them interactively using [Jupyter](https://
+jupyter.org) or [JupyterLab](https://jupyter.org). ## Low-level spatial math
+Import the low-level transform functions ``` >>> from spatialmath.base import *
+``` We can create a 3D rotation matrix ``` >>> rotx(0.3) array([[ 1. , 0. , 0.
+], [ 0. , 0.95533649, -0.29552021], [ 0. , 0.29552021, 0.95533649]]) >>> rotx
+(30, unit='deg') array([[ 1. , 0. , 0. ], [ 0. , 0.8660254, -0.5 ], [ 0. , 0.5
+, 0.8660254]]) ``` The results are `numpy` arrays so to perform matrix
+multiplication you need to use the `@` operator, for example ``` rotx(0.3) @
+roty(0.2) ``` We also support multiple ways of passing vector information to
+functions that require it: * as separate positional arguments ``` transl2(1, 2)
+array([[1., 0., 1.], [0., 1., 2.], [0., 0., 1.]]) ``` * as a list or a tuple
+``` transl2( [1,2] ) array([[1., 0., 1.], [0., 1., 2.], [0., 0., 1.]]) transl2
+( (1,2) ) Out[444]: array([[1., 0., 1.], [0., 1., 2.], [0., 0., 1.]]) ``` * or
+as a `numpy` array ``` transl2( np.array([1,2]) ) Out[445]: array([[1., 0.,
+1.], [0., 1., 2.], [0., 0., 1.]]) ``` There is a single module that deals with
+quaternions, unit or not, and the representation is a `numpy` array of four
+elements. As above, functions can accept the `numpy` array, a list, dict or
+`numpy` row or column vectors. ``` >>> from spatialmath.base.quaternion import
+* >>> q = qqmul([1,2,3,4], [5,6,7,8]) >>> q array([-60, 12, 30, 24]) >>> qprint
+(q) -60.000000 < 12.000000, 30.000000, 24.000000 > >>> qnorm(q)
+72.24956747275377 ``` ## Graphics ![trplot](https://github.com/bdaiinstitute/
+spatialmath-python/raw/master/docs/figs/transforms3d.png) The functions support
+various plotting styles ``` trplot( transl(1,2,3), frame='A', rviz=True,
+width=1, dims=[0, 10, 0, 10, 0, 10]) trplot( transl(3,1, 2), color='red',
+width=3, frame='B') trplot( transl(4, 3, 1)@trotx(math.pi/3), color='green',
+frame='c', dims=[0,4,0,4,0,4]) ``` Animation is straightforward ``` tranimate
+(transl(4, 3, 4)@trotx(2)@troty(-2), frame='A', arrow=False, dims=[0, 5],
+nframes=200) ``` and it can be saved to a file by ``` tranimate(transl(4, 3,
+4)@trotx(2)@troty(-2), frame='A', arrow=False, dims=[0, 5], nframes=200,
+movie='out.mp4') ``` ![animation video](./docs/figs/animate.gif) At the moment
+we can only save as an MP4, but the following incantation will covert that to
+an animated GIF for embedding in web pages ``` ffmpeg -i out -r 20 -vf
+"fps=10,scale=640:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1]
+[p]paletteuse" out.gif ``` For use in a Jupyter notebook, or on Colab, you can
+display an animation by ``` from IPython.core.display import HTML HTML
+(tranimate(transl(4, 3, 4)@trotx(2)@troty(-2), frame='A', arrow=False, dims=[0,
+5], nframes=200, movie=True)) ``` The `movie=True` option causes `tranimate` to
+output an HTML5 fragment which is displayed inline by the `HTML` function. ##
+Symbolic support Some functions have support for symbolic variables, for
+example ``` import sympy theta = sym.symbols('theta') print(rotx(theta)) [[1 0
+0] [0 cos(theta) -sin(theta)] [0 sin(theta) cos(theta)]] ``` The resulting
+`numpy` array is an array of symbolic objects not numbers – the constants are
+also symbolic objects. You can read the elements of the matrix ``` a = T[0,0] a
+Out[258]: 1 type(a) Out[259]: int a = T[1,1] a Out[256]: cos(theta) type(a) Out
+[255]: cos ``` We see that the symbolic constants are converted back to Python
+numeric types on read. Similarly when we assign an element or slice of the
+symbolic matrix to a numeric value, they are converted to symbolic constants on
+the way in. ## History & Contributors This package was originally created by
+[Peter Corke](https://github.com/petercorke) and [Jesse Haviland](https://
+github.com/jhavl) and was inspired by the [Spatial Math Toolbox for MATLAB]
+(https://github.com/petercorke/spatialmath-matlab). It supports the textbook
+[Robotics, Vision & Control in Python 3e](https://github.com/petercorke/RVC3-
+python). The package is now a collaboration with [Boston Dynamics AI Institute]
+(https://theaiinstitute.com/).
```

### Comparing `spatialmath-python-1.1.8/pyproject.toml` & `spatialmath-python-1.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spatialmath-python"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="Peter Corke", email="rvc@petercorke.com" },
 ]
 description = "Provides spatial maths capability for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -36,21 +36,22 @@
 
 dependencies = [
     "numpy>=1.17.4",
     "scipy",
     "matplotlib",
     "ansitable",
     "typing_extensions",
+    "pre-commit",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/petercorke/spatialmath-python"
-"Bug Tracker" = "https://github.com/petercorke/spatialmath-python/issues"
-"Documentation" = "https://petercorke.github.io/petercorke/spatialmath-python"
-"Source" = "https://github.com/petercorke/petercorke/spatialmath-python"
+"Homepage" = "https://github.com/bdaiinstitute/spatialmath-python"
+"Bug Tracker" = "https://github.com/bdaiinstitute/spatialmath-python/issues"
+"Documentation" = "https://bdaiinstitute.github.io/spatialmath-python/"
+"Source" = "https://github.com/bdaiinstitute/spatialmath-python"
 
 [project.optional-dependencies]
 
 dev = [
     "sympy",
     "pytest",
     "pytest-timeout",
```

### Comparing `spatialmath-python-1.1.8/spatialmath/DualQuaternion.py` & `spatialmath-python-1.1.9/spatialmath/DualQuaternion.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/__init__.py` & `spatialmath-python-1.1.9/spatialmath/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/base/__init__.py` & `spatialmath-python-1.1.9/spatialmath/base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
     "rot2",
     "trot2",
     "transl2",
     "ishom2",
     "isrot2",
     "trlog2",
     "trexp2",
+    "trnorm2",
     "tr2jac2",
     "trinterp2",
     "trprint2",
     "trplot2",
     "tranimate2",
     "xyt2tr",
     "tr2xyt",
```

### Comparing `spatialmath-python-1.1.8/spatialmath/base/_types_311.py` & `spatialmath-python-1.1.9/spatialmath/base/_types_311.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/base/_types_35.py` & `spatialmath-python-1.1.9/spatialmath/base/_types_35.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/base/_types_39.py` & `spatialmath-python-1.1.9/spatialmath/base/_types_39.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/base/animate.py` & `spatialmath-python-1.1.9/spatialmath/base/animate.py`

 * *Files 0% similar despite different names*

```diff
@@ -889,18 +889,18 @@
     #         yield attitude.R
     # plt.figure()
     # plotvol3(2)
     # tranimate(attitude())
 
     from spatialmath import base
 
-    T = smb.rpy2r(0.3, 0.4, 0.5)
-    smb.tranimate(T, wait=True)
+    # T = smb.rpy2r(0.3, 0.4, 0.5)
+    # # smb.tranimate(T, wait=True)
     # s = smb.tranimate(T, movie=True)
     # with open("zz.html", "w") as f:
     #     print(f"<html>{s}</html>", file=f)
 
-    # T = smb.rot2(2)
-    # # smb.tranimate2(T, wait=True)
-    # s = smb.tranimate2(T, movie=True)
-    # with open("zz.html", "w") as f:
-    #     print(f"<html>{s}</html>", file=f)
+    T = smb.rot2(2)
+    # smb.tranimate2(T, wait=True)
+    s = smb.tranimate2(T, movie=True)
+    with open("zz.html", "w") as f:
+        print(f"<html>{s}</html>", file=f)
```

### Comparing `spatialmath-python-1.1.8/spatialmath/base/argcheck.py` & `spatialmath-python-1.1.9/spatialmath/base/argcheck.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/base/graphics.py` & `spatialmath-python-1.1.9/spatialmath/base/graphics.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/base/numeric.py` & `spatialmath-python-1.1.9/spatialmath/base/numeric.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/base/quaternions.py` & `spatialmath-python-1.1.9/spatialmath/base/quaternions.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,20 +102,22 @@
     :seealso: :func:`qunit`
 
     """
     q = smb.getvector(q, 4)
     return np.linalg.norm(q)
 
 
-def qunit(q: ArrayLike4, tol: Optional[float] = 10) -> UnitQuaternionArray:
+def qunit(q: ArrayLike4, tol: float = 20) -> UnitQuaternionArray:
     """
     Create a unit quaternion
 
     :arg v: quaterion
     :type v: array_like(4)
+    :param tol: Tolerance in multiples of eps, defaults to 20
+    :type tol: float, optional
     :return: a pure quaternion
     :rtype: ndarray(4)
     :raises ValueError: quaternion has (near) zero norm
 
     Creates a unit quaternion, with unit norm, by scaling the input quaternion.
 
     .. runblock:: pycon
@@ -140,21 +142,21 @@
 
     if q[0] >= 0:
         return q
     else:
         return -q
 
 
-def qisunit(q: ArrayLike4, tol: Optional[float] = 100) -> bool:
+def qisunit(q: ArrayLike4, tol: float = 20) -> bool:
     """
     Test if quaternion has unit length
 
     :param v: quaternion
     :type v: array_like(4)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether quaternion has unit length
     :rtype: bool
 
     .. runblock:: pycon
 
         >>> from spatialmath.base import qeye, qpure, qisunit
@@ -168,41 +170,41 @@
     return smb.iszerovec(q, tol=tol)
 
 
 @overload
 def qisequal(
     q1: ArrayLike4,
     q2: ArrayLike4,
-    tol: Optional[float] = 100,
+    tol: float = 20,
     unitq: Optional[bool] = False,
 ) -> bool:
     ...
 
 
 @overload
 def qisequal(
     q1: ArrayLike4,
     q2: ArrayLike4,
-    tol: Optional[float] = 100,
+    tol: float = 20,
     unitq: Optional[bool] = True,
 ) -> bool:
     ...
 
 
-def qisequal(q1, q2, tol: Optional[float] = 100, unitq: Optional[bool] = False):
+def qisequal(q1, q2, tol: float = 20, unitq: Optional[bool] = False):
     """
     Test if quaternions are equal
 
     :param q1: quaternion
     :type q1: array_like(4)
     :param q2: quaternion
     :type q2: array_like(4)
     :param unitq: quaternions are unit quaternions
     :type unitq: bool
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether quaternions are equal
     :rtype: bool
 
     Tests if two quaternions are equal.
 
     For unit-quaternions ``unitq=True`` the double mapping is taken into account,
@@ -541,25 +543,25 @@
         ]
     )
 
 
 def r2q(
     R: SO3Array,
     check: Optional[bool] = False,
-    tol: Optional[float] = 100,
+    tol: float = 20,
     order: Optional[str] = "sxyz",
 ) -> UnitQuaternionArray:
     """
     Convert SO(3) rotation matrix to unit-quaternion
 
     :arg R: SO(3) rotation matrix
     :type R: ndarray(3,3)
     :param check: check validity of rotation matrix, default False
     :type check: bool
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :param order: the order of the returned quaternion elements. Must be 'sxyz' or
         'xyzs'. Defaults to 'sxyz'.
     :type order: str
     :return: unit-quaternion as Euler parameters
     :rtype: ndarray(4)
     :raises ValueError: for non SO(3) argument
@@ -755,27 +757,33 @@
 #     if abs(nm) < tol * _eps:
 #         return qeye()
 #     else:
 #         return np.r_[qs, (math.sqrt(1.0 - qs**2) / nm) * kv]
 
 
 def qslerp(
-    q0: ArrayLike4, q1: ArrayLike4, s: float, shortest: Optional[bool] = False
+    q0: ArrayLike4,
+    q1: ArrayLike4,
+    s: float,
+    shortest: Optional[bool] = False,
+    tol: float = 20,
 ) -> UnitQuaternionArray:
     """
     Quaternion conjugate
 
     :arg q0: initial unit quaternion
     :type q0: array_like(4)
     :arg q1: final unit quaternion
     :type q1: array_like(4)
     :arg s: interpolation coefficient in the range [0,1]
     :type s: float
     :arg shortest: choose shortest distance [default False]
     :type shortest: bool
+    :param tol: Tolerance when checking for identical quaternions, in multiples of eps, defaults to 20
+    :type tol: float, optional
     :return: interpolated unit-quaternion
     :rtype: ndarray(4)
     :raises ValueError: s is outside interval [0, 1]
 
     An interpolated quaternion between ``q0`` when ``s`` = 0 to ``q1`` when ``s`` = 1.
 
     Interpolation is performed on a great circle on a 4D hypersphere. This is
@@ -816,15 +824,15 @@
     if shortest:
         if dotprod < 0:
             q0 = -q0  # pylint: disable=invalid-unary-operand-type
             dotprod = -dotprod  # pylint: disable=invalid-unary-operand-type
 
     dotprod = np.clip(dotprod, -1, 1)  # Clip within domain of acos()
     theta = math.acos(dotprod)  # theta is the angle between rotation vectors
-    if abs(theta) > 10 * _eps:
+    if abs(theta) > tol * _eps:
         s0 = math.sin((1 - s) * theta)
         s1 = math.sin(s * theta)
         return ((q0 * s0) + (q1 * s1)) / math.sin(theta)
     else:
         # quaternions are identical
         return q0
 
@@ -981,15 +989,15 @@
     .. warning:: There is no check that the passed values are unit-quaternions.
 
     """
     # TODO different methods
 
     q1 = smb.getvector(q1, 4)
     q2 = smb.getvector(q2, 4)
-    return 2.0 * math.atan2(smb.norm(q1 - q2), smb.norm(q1 + q2))
+    return 4.0 * math.atan2(smb.norm(q1 - q2), smb.norm(q1 + q2))
 
 
 def qprint(
     q: Union[ArrayLike4, ArrayLike4],
     delim: Optional[Tuple[str, str]] = ("<", ">"),
     fmt: Optional[str] = "{: .4f}",
     file: Optional[TextIO] = sys.stdout,
```

### Comparing `spatialmath-python-1.1.8/spatialmath/base/symbolic.py` & `spatialmath-python-1.1.9/spatialmath/base/symbolic.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/base/transforms2d.py` & `spatialmath-python-1.1.9/spatialmath/base/transforms2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     _matplotlib_exists = True
 except ImportError:
     _matplotlib_exists = False
 
 import spatialmath.base as smb
 from spatialmath.base.types import *
 from spatialmath.base.transformsNd import rt2tr
+from spatialmath.base.vectors import unitvec
 
 _eps = np.finfo(np.float64).eps
 
 try:  # pragma: no cover
     # print('Using SymPy')
     import sympy
 
@@ -261,23 +262,23 @@
     Extract translation from SE(2) matrix
 
     :param x: SE(2) transform matrix
     :type x: ndarray(3,3)
     :return: translation elements of SE(2) matrix
     :rtype: ndarray(2)
 
-    - ``t = transl2(T)`` is the translational part of the SE(3) matrix ``T`` as a
+    - ``t = tr2pos2(T)`` is the translational part of the SE(3) matrix ``T`` as a
       2-element NumPy array.
 
     .. runblock:: pycon
 
         >>> from spatialmath.base import *
         >>> import numpy as np
         >>> T = np.array([[1, 0, 3], [0, 1, 4], [0, 0, 1]])
-        >>> transl2(T)
+        >>> tr2pos2(T)
 
     :seealso: :func:`pos2tr2` :func:`transl2`
     """
     return T[:2, 2]
 
 
 def pos2tr2(x, y=None):
@@ -287,27 +288,27 @@
     :param x: translation along X-axis
     :type x: float
     :param y: translation along Y-axis
     :type y: float
     :return: SE(2) matrix
     :rtype: ndarray(3,3)
 
-    - ``T = transl2([X, Y])`` is an SE(2) homogeneous transform (3x3)
+    - ``T = pos2tr2([X, Y])`` is an SE(2) homogeneous transform (3x3)
       representing a pure translation.
-    - ``T = transl2( V )`` as above but the translation is given by a 2-element
+    - ``T = pos2tr2( V )`` as above but the translation is given by a 2-element
       list, dict, or a numpy array, row or column vector.
 
 
     .. runblock:: pycon
 
         >>> from spatialmath.base import *
         >>> import numpy as np
-        >>> transl2(3, 4)
-        >>> transl2([3, 4])
-        >>> transl2(np.array([3, 4]))
+        >>> pos2tr2(3, 4)
+        >>> pos2tr2([3, 4])
+        >>> pos2tr2(np.array([3, 4]))
 
     :seealso: :func:`tr2pos2` :func:`transl2`
     """
     if smb.isscalar(x) and smb.isscalar(y):
         # (x, y) -> SE(2)
         t = np.r_[x, y]
     elif smb.isvector(x, 2):
@@ -319,22 +320,24 @@
     if t.dtype != "O":
         t = t.astype("float64")
     T = np.identity(3, dtype=t.dtype)
     T[:2, 2] = t
     return T
 
 
-def ishom2(T: Any, check: bool = False) -> bool:  # TypeGuard(SE2):
+def ishom2(T: Any, check: bool = False, tol: float = 20) -> bool:  # TypeGuard(SE2):
     """
     Test if matrix belongs to SE(2)
 
     :param T: SE(2) matrix to test
     :type T: ndarray(3,3)
     :param check: check validity of rotation submatrix
     :type check: bool
+    :param tol: Tolerance in units of eps for zero-rotation case, defaults to 20
+    :type: float
     :return: whether matrix is an SE(2) homogeneous transformation matrix
     :rtype: bool
 
     - ``ishom2(T)`` is True if the argument ``T`` is of dimension 3x3
     - ``ishom2(T, check=True)`` as above, but also checks orthogonality of the
       rotation sub-matrix and validitity of the bottom row.
 
@@ -351,26 +354,31 @@
         >>> ishom2(R)
 
     :seealso: isR, isrot2, ishom, isvec
     """
     return (
         isinstance(T, np.ndarray)
         and T.shape == (3, 3)
-        and (not check or (smb.isR(T[:2, :2]) and all(T[2, :] == np.array([0, 0, 1]))))
+        and (
+            not check
+            or (smb.isR(T[:2, :2], tol=tol) and all(T[2, :] == np.array([0, 0, 1])))
+        )
     )
 
 
-def isrot2(R: Any, check: bool = False) -> bool:  # TypeGuard(SO2):
+def isrot2(R: Any, check: bool = False, tol: float = 20) -> bool:  # TypeGuard(SO2):
     """
     Test if matrix belongs to SO(2)
 
     :param R: SO(2) matrix to test
     :type R: ndarray(3,3)
     :param check: check validity of rotation submatrix
     :type check: bool
+    :param tol: Tolerance in units of eps for zero-rotation case, defaults to 20
+    :type: float
     :return: whether matrix is an SO(2) rotation matrix
     :rtype: bool
 
     - ``isrot2(R)`` is True if the argument ``R`` is of dimension 2x2
     - ``isrot2(R, check=True)`` as above, but also checks orthogonality of the rotation matrix.
 
     .. runblock:: pycon
@@ -383,15 +391,19 @@
         >>> isrot2(R)
         >>> R = np.array([[1, 1], [0, 1]])  # invalid SO(2)
         >>> isrot2(R)  # a quick check says it is an SO(2)
         >>> isrot2(R, check=True)  # but if we check more carefully...
 
     :seealso: isR, ishom2, isrot
     """
-    return isinstance(R, np.ndarray) and R.shape == (2, 2) and (not check or smb.isR(R))
+    return (
+        isinstance(R, np.ndarray)
+        and R.shape == (2, 2)
+        and (not check or smb.isR(R, tol=tol))
+    )
 
 
 # ---------------------------------------------------------------------------------------#
 
 
 def trinv2(T: SE2Array) -> SE2Array:
     r"""
@@ -429,65 +441,65 @@
 
 
 @overload  # pragma: no cover
 def trlog2(
     T: SO2Array,
     twist: bool = False,
     check: bool = True,
-    tol: float = 10,
+    tol: float = 20,
 ) -> so2Array:
     ...
 
 
 @overload  # pragma: no cover
 def trlog2(
     T: SE2Array,
     twist: bool = False,
     check: bool = True,
-    tol: float = 10,
+    tol: float = 20,
 ) -> se2Array:
     ...
 
 
 @overload  # pragma: no cover
 def trlog2(
     T: SO2Array,
     twist: bool = True,
     check: bool = True,
-    tol: float = 10,
+    tol: float = 20,
 ) -> float:
     ...
 
 
 @overload  # pragma: no cover
 def trlog2(
     T: SE2Array,
     twist: bool = True,
     check: bool = True,
-    tol: float = 10,
+    tol: float = 20,
 ) -> R3:
     ...
 
 
 def trlog2(
     T: Union[SO2Array, SE2Array],
     twist: bool = False,
     check: bool = True,
-    tol: float = 10,
+    tol: float = 20,
 ) -> Union[float, R3, so2Array, se2Array]:
     """
     Logarithm of SO(2) or SE(2) matrix
 
     :param T: SE(2) or SO(2) matrix
     :type T: ndarray(3,3) or ndarray(2,2)
     :param check: check that matrix is valid
     :type check: bool
     :param twist: return a twist vector instead of matrix [default]
     :type twist: bool
-    :param tol: Tolerance in units of eps for zero-rotation case, defaults to 10
+    :param tol: Tolerance in units of eps for zero-rotation case, defaults to 20
     :type: float
     :return: logarithm
     :rtype: ndarray(3,3) or ndarray(3); or ndarray(2,2) or ndarray(1)
     :raises ValueError: bad argument
 
     An efficient closed-form solution of the matrix logarithm for arguments that
     are SO(2) or SE(2).
@@ -509,18 +521,18 @@
         >>> trlog2(rot2(0.3))
         >>> trlog2(rot2(0.3), twist=True)
 
     :seealso: :func:`~trexp`, :func:`~spatialmath.base.transformsNd.vex`,
               :func:`~spatialmath.base.transformsNd.vexa`
     """
 
-    if ishom2(T, check=check):
+    if ishom2(T, check=check, tol=tol):
         # SE(2) matrix
 
-        if smb.iseye(T, tol):
+        if smb.iseye(T, tol=tol):
             # is identity matrix
             if twist:
                 return np.zeros((3,))
             else:
                 return np.zeros((3, 3))
         else:
             st = T[1, 0]
@@ -534,15 +546,15 @@
             if twist:
                 return np.hstack([tr, theta])
             else:
                 return np.block(
                     [[smb.skew(theta), tr[:, np.newaxis]], [np.zeros((1, 3))]]
                 )
 
-    elif isrot2(T, check=check):
+    elif isrot2(T, check=check, tol=tol):
         # SO(2) rotation matrix
         theta = math.atan(T[1, 0] / T[0, 0])
         if twist:
             return theta
         else:
             return smb.skew(theta)
     else:
@@ -676,14 +688,80 @@
         # compute rotation matrix, simpler than Rodrigues for 2D case
         return smb.rot2(w[0])
     else:
         raise ValueError(" First argument must be SO(2), 1-vector, SE(2) or 3-vector")
 
 
 @overload  # pragma: no cover
+def trnorm2(R: SO2Array) -> SO2Array:
+    ...
+
+
+def trnorm2(T: SE2Array) -> SE2Array:
+    r"""
+    Normalize an SO(2) or SE(2) matrix
+
+    :param T: SE(2) or SO(2) matrix
+    :type T: ndarray(3,3) or ndarray(2,2)
+    :return: normalized SE(2) or SO(2) matrix
+    :rtype: ndarray(3,3) or ndarray(2,2)
+    :raises ValueError: bad arguments
+
+    - ``trnorm(R)`` is guaranteed to be a proper orthogonal matrix rotation
+      matrix (2,2) which is *close* to the input matrix R (2,2).
+    - ``trnorm(T)`` as above but the rotational submatrix of the homogeneous
+      transformation T (3,3) is normalised while the translational part is
+      unchanged.
+
+    The steps in normalization are:
+
+    #. If :math:`\mathbf{R} = [a, b]`
+    #. Form unit vectors :math:`\hat{b}
+    #. Form the orthogonal planar vector :math:`\hat{a} = [\hat{b}_y  -\hat{b}_x]`
+    #. Form the normalized SO(2) matrix :math:`\mathbf{R} = [\hat{a}, \hat{b}]`
+
+    .. runblock:: pycon
+
+        >>> from spatialmath.base import trnorm, troty
+        >>> from numpy import linalg
+        >>> T = trot2(45, 'deg', t=[3, 4])
+        >>> linalg.det(T[:2,:2]) - 1 # is a valid SO(3)
+        >>> T = T @ T @ T @ T @ T @ T @ T @ T @ T @ T @ T @ T @ T
+        >>> linalg.det(T[:2,:2]) - 1  # not quite a valid SE(2) anymore
+        >>> T = trnorm2(T)
+        >>> linalg.det(T[:2,:2]) - 1  # once more a valid SE(2)
+
+    .. note::
+
+        - Only the direction of a-vector (the z-axis) is unchanged.
+        - Used to prevent finite word length arithmetic causing transforms to
+          become 'unnormalized', ie. determinant :math:`\ne 1`.
+    """
+
+    if not ishom2(T) and not isrot2(T):
+        raise ValueError("expecting SO(2) or SE(2)")
+
+    a = T[:, 0]
+    b = T[:, 1]
+
+    b = unitvec(b)
+    # fmt: off
+    R = np.array([
+        [ b[1], b[0]], 
+        [-b[0], b[1]]
+    ])
+    # fmt: on
+
+    if ishom2(T):
+        return rt2tr(cast(SO2Array, R), T[:2, 2])
+    else:
+        return R
+
+
+@overload  # pragma: no cover
 def tradjoint2(T: SO2Array) -> R1x1:
     ...
 
 
 @overload  # pragma: no cover
 def tradjoint2(T: SE2Array) -> R3x3:
     ...
@@ -941,16 +1019,30 @@
         s += " {} rad".format(_vec2s(fmt, [angle]))
 
     if file:
         print(s, file=file)
     return s
 
 
-def _vec2s(fmt: str, v: ArrayLikePure):
-    v = [x if np.abs(x) > 100 * _eps else 0.0 for x in v]
+def _vec2s(fmt: str, v: ArrayLikePure, tol: float = 20) -> str:
+    """
+    Return a string representation for vector using the provided fmt.
+
+    :param fmt: format string for each value in v
+    :type fmt: str
+    :param tol: Tolerance when checking for near-zero values, in multiples of eps, defaults to 20
+    :type tol: float, optional
+    :return: string representation for the vector
+    :rtype: str
+
+    Return a string representation for vector using the provided fmt, where
+    near-zero values are rounded to 0.
+    """
+
+    v = [x if np.abs(x) > tol * _eps else 0.0 for x in v]
     return ", ".join([fmt.format(x) for x in v])
 
 
 def points2tr2(p1: NDArray, p2: NDArray) -> SE2Array:
     """
     SE(2) transform from corresponding points
```

### Comparing `spatialmath-python-1.1.8/spatialmath/base/transforms3d.py` & `spatialmath-python-1.1.9/spatialmath/base/transforms3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,22 +345,22 @@
         t = t.astype("float64")
 
     T = np.identity(4, dtype=t.dtype)
     T[:3, 3] = t
     return T
 
 
-def ishom(T: Any, check: bool = False, tol: float = 100) -> bool:
+def ishom(T: Any, check: bool = False, tol: float = 20) -> bool:
     """
     Test if matrix belongs to SE(3)
 
     :param T: SE(3) matrix to test
     :type T: numpy(4,4)
     :param check: check validity of rotation submatrix
-    :param tol: Tolerance in units of eps for rotation submatrix check, defaults to 100
+    :param tol: Tolerance in units of eps for rotation submatrix check, defaults to 20
     :return: whether matrix is an SE(3) homogeneous transformation matrix
 
     - ``ishom(T)`` is True if the argument ``T`` is of dimension 4x4
     - ``ishom(T, check=True)`` as above, but also checks orthogonality of the
       rotation sub-matrix and validitity of the bottom row.
 
     .. runblock:: pycon
@@ -383,22 +383,22 @@
         and (
             not check
             or (isR(T[:3, :3], tol=tol) and all(T[3, :] == np.array([0, 0, 0, 1])))
         )
     )
 
 
-def isrot(R: Any, check: bool = False, tol: float = 100) -> bool:
+def isrot(R: Any, check: bool = False, tol: float = 20) -> bool:
     """
     Test if matrix belongs to SO(3)
 
     :param R: SO(3) matrix to test
     :type R: numpy(3,3)
     :param check: check validity of rotation submatrix
-    :param tol: Tolerance in units of eps for rotation matrix test, defaults to 100
+    :param tol: Tolerance in units of eps for rotation matrix test, defaults to 20
     :return: whether matrix is an SO(3) rotation matrix
 
     - ``isrot(R)`` is True if the argument ``R`` is of dimension 3x3
     - ``isrot(R, check=True)`` as above, but also checks orthogonality of the
       rotation matrix.
 
     .. runblock:: pycon
@@ -709,24 +709,26 @@
     R = eul2r(phi, theta, psi, unit=unit)
     return r2t(R)
 
 
 # ---------------------------------------------------------------------------------------#
 
 
-def angvec2r(theta: float, v: ArrayLike3, unit="rad") -> SO3Array:
+def angvec2r(theta: float, v: ArrayLike3, unit="rad", tol: float = 20) -> SO3Array:
     """
     Create an SO(3) rotation matrix from rotation angle and axis
 
     :param theta: rotation
     :type theta: float
     :param unit: angular units: 'rad' [default], or 'deg'
     :type unit: str
     :param v: 3D rotation axis
     :type v: array_like(3)
+    :param tol: Tolerance in units of eps for zero-rotation case, defaults to 20
+    :type: float
     :return: SO(3) rotation matrix
     :rtype: ndarray(3,3)
     :raises ValueError: bad arguments
 
     ``angvec2r(θ, V)`` is an SO(3) orthonormal rotation matrix
     equivalent to a rotation of ``θ`` about the vector ``V``.
 
@@ -744,15 +746,15 @@
     :seealso: :func:`~angvec2tr` :func:`~tr2angvec`
 
     :SymPy: not supported
     """
     if not isscalar(theta) or not isvector(v, 3):
         raise ValueError("Arguments must be angle and vector")
 
-    if np.linalg.norm(v) < 10 * _eps:
+    if np.linalg.norm(v) < tol * _eps:
         return np.eye(3)
 
     θ = getunit(theta, unit)
 
     # Rodrigue's equation
 
     sk = skew(cast(ArrayLike3, unitvec(v)))
@@ -1019,15 +1021,15 @@
     if ismatrix(T, (4, 4)):
         R = t2r(T)
     else:
         R = T
     if not isrot(R, check=check):
         raise ValueError("argument is not SO(3)")
 
-    v = vex(trlog(cast(SO3Array, R)))
+    v = vex(trlog(cast(SO3Array, R), check=check))
 
     try:
         theta = norm(v)
         v = unitvec(v)
     except ValueError:
         theta = 0
         v = np.r_[0, 0, 0]
@@ -1040,26 +1042,29 @@
 
 # ------------------------------------------------------------------------------------------------------------------- #
 def tr2eul(
     T: Union[SO3Array, SE3Array],
     unit: str = "rad",
     flip: bool = False,
     check: bool = False,
+    tol: float = 20,
 ) -> R3:
     r"""
     Convert SO(3) or SE(3) to ZYX Euler angles
 
     :param R: SE(3) or SO(3) matrix
     :type R: ndarray(4,4) or ndarray(3,3)
     :param unit: 'rad' or 'deg'
     :type unit: str
     :param flip: choose first Euler angle to be in quadrant 2 or 3
     :type flip: bool
     :param check: check that rotation matrix is valid
     :type check: bool
+    :param tol: Tolerance in units of eps for near-zero checks, defaults to 20
+    :type: float
     :return: ZYZ Euler angles
     :rtype: ndarray(3)
 
     ``tr2eul(R)`` are the Euler angles corresponding to
     the rotation part of ``R``.
 
     The 3 angles :math:`[\phi, \theta, \psi]` correspond to sequential rotations
@@ -1086,19 +1091,19 @@
 
     """
 
     if ismatrix(T, (4, 4)):
         R = t2r(T)
     else:
         R = T
-    if not isrot(R, check=check):
+    if not isrot(R, check=check, tol=tol):
         raise ValueError("argument is not SO(3)")
 
     eul = np.zeros((3,))
-    if abs(R[0, 2]) < 10 * _eps and abs(R[1, 2]) < 10 * _eps:
+    if abs(R[0, 2]) < tol * _eps and abs(R[1, 2]) < tol * _eps:
         eul[0] = 0
         sp = 0
         cp = 1
         eul[1] = math.atan2(cp * R[0, 2] + sp * R[1, 2], R[2, 2])
         eul[2] = math.atan2(-sp * R[0, 0] + cp * R[1, 0], -sp * R[0, 1] + cp * R[1, 1])
     else:
         if flip:
@@ -1120,26 +1125,29 @@
 
 
 def tr2rpy(
     T: Union[SO3Array, SE3Array],
     unit: str = "rad",
     order: str = "zyx",
     check: bool = False,
+    tol: float = 20,
 ) -> R3:
     r"""
     Convert SO(3) or SE(3) to roll-pitch-yaw angles
 
     :param R: SE(3) or SO(3) matrix
     :type R: ndarray(4,4) or ndarray(3,3)
     :param unit: 'rad' or 'deg'
     :type unit: str
     :param order: 'xyz', 'zyx' or 'yxz' [default 'zyx']
     :type order: str
     :param check: check that rotation matrix is valid
     :type check: bool
+    :param tol: Tolerance in units of eps, defaults to 20
+    :type: float
     :return: Roll-pitch-yaw angles
     :rtype: ndarray(3)
     :raises ValueError: bad arguments
 
     ``tr2rpy(R)`` are the roll-pitch-yaw angles corresponding to
     the rotation part of ``R``.
 
@@ -1172,21 +1180,21 @@
     :SymPy: not supported
     """
 
     if ismatrix(T, (4, 4)):
         R = t2r(T)
     else:
         R = T
-    if not isrot(R, check=check):
+    if not isrot(R, check=check, tol=tol):
         raise ValueError("not a valid SO(3) matrix")
 
     rpy = np.zeros((3,))
     if order in ("xyz", "arm"):
         # XYZ order
-        if abs(abs(R[0, 2]) - 1) < 10 * _eps:  # when |R13| == 1
+        if abs(abs(R[0, 2]) - 1) < tol * _eps:  # when |R13| == 1
             # singularity
             rpy[0] = 0  # roll is zero
             if R[0, 2] > 0:
                 rpy[2] = math.atan2(R[2, 1], R[1, 1])  # R+Y
             else:
                 rpy[2] = -math.atan2(R[1, 0], R[2, 0])  # R-Y
             rpy[1] = math.asin(np.clip(R[0, 2], -1.0, 1.0))
@@ -1202,15 +1210,15 @@
             elif k == 2:
                 rpy[1] = -math.atan(R[0, 2] * math.sin(rpy[2]) / R[1, 2])
             elif k == 3:
                 rpy[1] = math.atan(R[0, 2] * math.cos(rpy[2]) / R[2, 2])
 
     elif order in ("zyx", "vehicle"):
         # old ZYX order (as per Paul book)
-        if abs(abs(R[2, 0]) - 1) < 10 * _eps:  # when |R31| == 1
+        if abs(abs(R[2, 0]) - 1) < tol * _eps:  # when |R31| == 1
             # singularity
             rpy[0] = 0  # roll is zero
             if R[2, 0] < 0:
                 rpy[2] = -math.atan2(R[0, 1], R[0, 2])  # R-Y
             else:
                 rpy[2] = math.atan2(-R[0, 1], -R[0, 2])  # R+Y
             rpy[1] = -math.asin(np.clip(R[2, 0], -1.0, 1.0))
@@ -1225,15 +1233,15 @@
                 rpy[1] = -math.atan(R[2, 0] * math.sin(rpy[2]) / R[1, 0])
             elif k == 2:
                 rpy[1] = -math.atan(R[2, 0] * math.sin(rpy[0]) / R[2, 1])
             elif k == 3:
                 rpy[1] = -math.atan(R[2, 0] * math.cos(rpy[0]) / R[2, 2])
 
     elif order in ("yxz", "camera"):
-        if abs(abs(R[1, 2]) - 1) < 10 * _eps:  # when |R23| == 1
+        if abs(abs(R[1, 2]) - 1) < tol * _eps:  # when |R23| == 1
             # singularity
             rpy[0] = 0
             if R[1, 2] < 0:
                 rpy[2] = -math.atan2(R[2, 0], R[0, 0])  # R-Y
             else:
                 rpy[2] = math.atan2(-R[2, 0], -R[2, 1])  # R+Y
             rpy[1] = -math.asin(np.clip(R[1, 2], -1.0, 1.0))  # P
@@ -1259,52 +1267,52 @@
 
     return rpy  # type: ignore
 
 
 # ---------------------------------------------------------------------------------------#
 @overload  # pragma: no cover
 def trlog(
-    T: SO3Array, check: bool = True, twist: bool = False, tol: float = 10
+    T: SO3Array, check: bool = True, twist: bool = False, tol: float = 20
 ) -> so3Array:
     ...
 
 
 @overload  # pragma: no cover
 def trlog(
-    T: SE3Array, check: bool = True, twist: bool = False, tol: float = 10
+    T: SE3Array, check: bool = True, twist: bool = False, tol: float = 20
 ) -> se3Array:
     ...
 
 
 @overload  # pragma: no cover
-def trlog(T: SO3Array, check: bool = True, twist: bool = True, tol: float = 10) -> R3:
+def trlog(T: SO3Array, check: bool = True, twist: bool = True, tol: float = 20) -> R3:
     ...
 
 
 @overload  # pragma: no cover
-def trlog(T: SE3Array, check: bool = True, twist: bool = True, tol: float = 10) -> R6:
+def trlog(T: SE3Array, check: bool = True, twist: bool = True, tol: float = 20) -> R6:
     ...
 
 
 def trlog(
     T: Union[SO3Array, SE3Array],
     check: bool = True,
     twist: bool = False,
-    tol: float = 10,
+    tol: float = 20,
 ) -> Union[R3, R6, so3Array, se3Array]:
     """
     Logarithm of SO(3) or SE(3) matrix
 
     :param R: SE(3) or SO(3) matrix
     :type R: ndarray(4,4) or ndarray(3,3)
     :param check: check that matrix is valid
     :type check: bool
     :param twist: return a twist vector instead of matrix [default]
     :type twist: bool
-    :param tol: Tolerance in units of eps for zero-rotation case, defaults to 10
+    :param tol: Tolerance in units of eps for zero-rotation case, defaults to 20
     :type: float
     :return: logarithm
     :rtype: ndarray(4,4) or ndarray(3,3)
     :raises ValueError: bad argument
 
     An efficient closed-form solution of the matrix logarithm for arguments that
     are SO(3) or SE(3).
@@ -1325,21 +1333,21 @@
         >>> trlog(trotx(0.3), twist=True)
         >>> trlog(rotx(0.3))
         >>> trlog(rotx(0.3), twist=True)
 
     :seealso: :func:`~trexp` :func:`~spatialmath.base.transformsNd.vex` :func:`~spatialmath.base.transformsNd.vexa`
     """
 
-    if ishom(T, check=check, tol=10):
+    if ishom(T, check=check, tol=tol):
         # SE(3) matrix
 
         [R, t] = tr2rt(T)
 
         # S = trlog(R, check=False)  # recurse
-        S = trlog(cast(SO3Array, R), check=False)  # recurse
+        S = trlog(cast(SO3Array, R), check=False, tol=tol)  # recurse
         w = vex(S)
         theta = norm(w)
         if theta == 0:
             # rotation matrix is identity
             if twist:
                 return np.r_[t, 0, 0, 0]
             else:
@@ -1353,15 +1361,15 @@
             )
             v = Ginv @ t
             if twist:
                 return np.r_[v, w]
             else:
                 return Ab2M(S, v)
 
-    elif isrot(T, check=check):
+    elif isrot(T, check=check, tol=tol):
         # deal with rotation matrix
         R = T
         if abs(np.trace(R) + 1) < tol * _eps:
             # check for trace = -1
             #   rotation by +/- pi, +/- 3pi etc.
             diagonal = R.diagonal()
             k = diagonal.argmax()
@@ -1372,15 +1380,17 @@
             theta = math.pi
             if twist:
                 return w * theta
             else:
                 return skew(w * theta)
         else:
             # general case
-            theta = math.acos((np.trace(R) - 1) / 2)
+            tr = (np.trace(R) - 1) / 2
+            # min for inaccuracies near identity yielding trace > 3
+            theta = math.acos(min(tr, 1.0))
             st = math.sin(theta)
             if st == 0:
                 if twist:
                     return np.zeros((3,))
                 else:
                     return np.zeros((3, 3))
             else:
@@ -1527,21 +1537,25 @@
 
         # do Rodrigues' formula for rotation
         return rodrigues(w, theta)
     else:
         raise ValueError(" First argument must be SO(3), 3-vector, SE(3) or 6-vector")
 
 
+@overload  # pragma: no cover
+def trnorm(R: SO3Array) -> SO3Array:
+    ...
+
+
 def trnorm(T: SE3Array) -> SE3Array:
     r"""
     Normalize an SO(3) or SE(3) matrix
 
-    :param R: SE(3) or SO(3) matrix
-    :type R: ndarray(4,4) or ndarray(3,3)
-    :param T1: second SE(3) matrix
+    :param T: SE(3) or SO(3) matrix
+    :type T: ndarray(4,4) or ndarray(3,3)
     :return: normalized SE(3) or SO(3) matrix
     :rtype: ndarray(4,4) or ndarray(3,3)
     :raises ValueError: bad arguments
 
     - ``trnorm(R)`` is guaranteed to be a proper orthogonal matrix rotation
       matrix (3x3) which is *close* to the input matrix R (3x3).
     - ``trnorm(T)`` as above but the rotational submatrix of the homogeneous
@@ -1559,17 +1573,17 @@
     .. runblock:: pycon
 
         >>> from spatialmath.base import trnorm, troty
         >>> from numpy import linalg
         >>> T = troty(45, 'deg', t=[3, 4, 5])
         >>> linalg.det(T[:3,:3]) - 1 # is a valid SO(3)
         >>> T = T @ T @ T @ T @ T @ T @ T @ T @ T @ T @ T @ T @ T
-        >>> linalg.det(T[:3,:3]) - 1  # not quite a valid SO(3) anymore
+        >>> linalg.det(T[:3,:3]) - 1  # not quite a valid SE(3) anymore
         >>> T = trnorm(T)
-        >>> linalg.det(T[:3,:3]) - 1  # once more a valid SO(3)
+        >>> linalg.det(T[:3,:3]) - 1  # once more a valid SE(3)
 
     .. note::
 
         - Only the direction of a-vector (the z-axis) is unchanged.
         - Used to prevent finite word length arithmetic causing transforms to
           become 'unnormalized', ie. determinant :math:`\ne 1`.
     """
```

### Comparing `spatialmath-python-1.1.8/spatialmath/base/transformsNd.py` & `spatialmath-python-1.1.9/spatialmath/base/transformsNd.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,17 @@
             T[:2, :2] = R
             T[:2, 2] = t
         elif R.shape == (3, 3):
             T = np.eye(4)
             T[:3, :3] = R
             T[:3, 3] = t
         else:
-            raise ValueError(f"R must be an SO(2) or SO(3) rotation matrix, not {R.shape}")
+            raise ValueError(
+                f"R must be an SO(2) or SO(3) rotation matrix, not {R.shape}"
+            )
 
     return T
 
 
 # ---------------------------------------------------------------------------------------#
 
 
@@ -349,21 +351,21 @@
 
     return T
 
 
 # ======================= predicates
 
 
-def isR(R: NDArray, tol: float = 100) -> bool:  # -> TypeGuard[SOnArray]:
+def isR(R: NDArray, tol: float = 20) -> bool:  # -> TypeGuard[SOnArray]:
     r"""
     Test if matrix belongs to SO(n)
 
     :param R: matrix to test
     :type R: ndarray(2,2) or ndarray(3,3)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether matrix is a proper orthonormal rotation matrix
     :rtype: bool
 
     Checks orthogonality, ie. :math:`{\bf R} {\bf R}^T = {\bf I}` and :math:`\det({\bf R}) > 0`.
     For the first test we check that the norm of the residual is less than ``tol * eps``.
 
@@ -374,25 +376,25 @@
         >>> isR(rot2(0.5))
         >>> isR(np.zeros((3,3)))
 
     :seealso: isrot2, isrot
     """
     return bool(
         np.linalg.norm(R @ R.T - np.eye(R.shape[0])) < tol * _eps
-        and np.linalg.det(R @ R.T) > 0
+        and np.linalg.det(R) > 0
     )
 
 
-def isskew(S: NDArray, tol: float = 10) -> bool:  # -> TypeGuard[sonArray]:
+def isskew(S: NDArray, tol: float = 20) -> bool:  # -> TypeGuard[sonArray]:
     r"""
     Test if matrix belongs to so(n)
 
     :param S: matrix to test
     :type S: ndarray(2,2) or ndarray(3,3)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether matrix is a proper skew-symmetric matrix
     :rtype: bool
 
     Checks skew-symmetry, ie. :math:`{\bf S} + {\bf S}^T = {\bf 0}`.
     We check that the norm of the residual is less than ``tol * eps``.
 
@@ -405,21 +407,21 @@
         >>> isskew(np.eye(3))
 
     :seealso: isskewa
     """
     return bool(np.linalg.norm(S + S.T) < tol * _eps)
 
 
-def isskewa(S: NDArray, tol: float = 10) -> bool:  # -> TypeGuard[senArray]:
+def isskewa(S: NDArray, tol: float = 20) -> bool:  # -> TypeGuard[senArray]:
     r"""
     Test if matrix belongs to se(n)
 
     :param S: matrix to test
     :type S: ndarray(3,3) or ndarray(4,4)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether matrix is a proper skew-symmetric matrix
     :rtype: bool
 
     Check if matrix is augmented skew-symmetric, ie. the top left (n-1xn-1) partition ``S`` is
     skew-symmetric :math:`{\bf S} + {\bf S}^T = {\bf 0}`, and the bottom row is zero
     We check that the norm of the residual is less than ``tol * eps``.
@@ -435,26 +437,26 @@
     :seealso: isskew
     """
     return bool(np.linalg.norm(S[0:-1, 0:-1] + S[0:-1, 0:-1].T) < tol * _eps) and all(
         S[-1, :] == 0
     )
 
 
-def iseye(S: NDArray, tol: float = 10) -> bool:
+def iseye(S: NDArray, tol: float = 20) -> bool:
     """
     Test if matrix is identity
 
     :param S: matrix to test
     :type S: ndarray(n,n)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether matrix is a proper skew-symmetric matrix
     :rtype: bool
 
-    Check if matrix is an identity matrix. 
+    Check if matrix is an identity matrix.
     We check that the sum of the absolute value of the residual is less than ``tol * eps``.
 
     .. runblock:: pycon
 
         >>> from spatialmath.base import *
         >>> import numpy as np
         >>> iseye(np.array([[1,0], [0,1]]))
```

### Comparing `spatialmath-python-1.1.8/spatialmath/base/vectors.py` & `spatialmath-python-1.1.9/spatialmath/base/vectors.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,20 +138,22 @@
         >>> from spatialmath.base import *
         >>> colvec([1, 2, 3])
     """
     v = getvector(v)
     return np.array(v).reshape((len(v), 1))
 
 
-def unitvec(v: ArrayLike) -> NDArray:
+def unitvec(v: ArrayLike, tol: float = 20) -> NDArray:
     """
     Create a unit vector
 
     :param v: any vector
     :type v: array_like(n)
+    :param tol: Tolerance in units of eps for zero-norm case, defaults to 20
+    :type: float
     :return: a unit-vector parallel to ``v``.
     :rtype: ndarray(n)
     :raises ValueError: for zero length vector
 
     ``unitvec(v)`` is a vector parallel to `v` of unit length.
 
     .. runblock:: pycon
@@ -162,26 +164,28 @@
     :seealso: :func:`~numpy.linalg.norm`
 
     """
 
     v = getvector(v)
     n = norm(v)
 
-    if n > 100 * _eps:  # if greater than eps
+    if n > tol * _eps:  # if greater than eps
         return v / n
     else:
         raise ValueError("zero norm vector")
 
 
-def unitvec_norm(v: ArrayLike, tol: float = 100) -> Tuple[NDArray, float]:
+def unitvec_norm(v: ArrayLike, tol: float = 20) -> Tuple[NDArray, float]:
     """
     Create a unit vector
 
     :param v: any vector
     :type v: array_like(n)
+    :param tol: Tolerance in units of eps for zero-norm case, defaults to 20
+    :type: float
     :return: a unit-vector parallel to ``v`` and the norm
     :rtype: (ndarray(n), float)
     :raises ValueError: for zero length vector
 
     ``unitvec(v)`` is a vector parallel to `v` of unit length.
 
     .. runblock:: pycon
@@ -198,21 +202,21 @@
 
     if nm > tol * _eps:  # if greater than eps
         return (v / nm, nm)
     else:
         raise ValueError("zero norm vector")
 
 
-def isunitvec(v: ArrayLike, tol: float = 10) -> bool:
+def isunitvec(v: ArrayLike, tol: float = 20) -> bool:
     """
     Test if vector has unit length
 
     :param v: vector to test
     :type v: ndarray(n)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether vector has unit length
     :rtype: bool
 
     .. runblock:: pycon
 
         >>> from spatialmath.base import *
@@ -220,21 +224,21 @@
         >>> isunitvec([1, 2])
 
     :seealso: unit, iszerovec, isunittwist
     """
     return bool(abs(np.linalg.norm(v) - 1) < tol * _eps)
 
 
-def iszerovec(v: ArrayLike, tol: float = 10) -> bool:
+def iszerovec(v: ArrayLike, tol: float = 20) -> bool:
     """
     Test if vector has zero length
 
     :param v: vector to test
     :type v: ndarray(n)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether vector has zero length
     :rtype: bool
 
     .. runblock:: pycon
 
         >>> from spatialmath.base import *
@@ -242,21 +246,21 @@
         >>> iszerovec([1, 2])
 
     :seealso: unit, isunitvec, isunittwist
     """
     return bool(np.linalg.norm(v) < tol * _eps)
 
 
-def iszero(v: float, tol: float = 10) -> bool:
+def iszero(v: float, tol: float = 20) -> bool:
     """
     Test if scalar is zero
 
     :param v: value to test
     :type v: float
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether value is zero
     :rtype: bool
 
     .. runblock:: pycon
 
         >>> from spatialmath.base import *
@@ -264,21 +268,21 @@
         >>> iszero(1)
 
     :seealso: unit, iszerovec, isunittwist
     """
     return bool(abs(v) < tol * _eps)
 
 
-def isunittwist(v: ArrayLike6, tol: float = 10) -> bool:
+def isunittwist(v: ArrayLike6, tol: float = 20) -> bool:
     r"""
     Test if vector represents a unit twist in SE(2) or SE(3)
 
     :param v: twist vector to test
     :type v: array_like(6)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether twist has unit length
     :rtype: bool
     :raises ValueError: for incorrect vector length
 
 
     Vector is is intepretted as :math:`[v, \omega]` where :math:`v \in \mathbb{R}^n` and
@@ -298,27 +302,27 @@
     :seealso: unit, isunitvec
     """
     v = getvector(v)
 
     if len(v) == 6:
         # test for SE(3) twist
         return isunitvec(v[3:6], tol=tol) or (
-            bool(np.linalg.norm(v[3:6]) < tol * _eps) and isunitvec(v[0:3], tol=tol)
+            iszerovec(v[3:6], tol=tol) and isunitvec(v[0:3], tol=tol)
         )
     else:
         raise ValueError
 
 
-def isunittwist2(v: ArrayLike3, tol: float = 10) -> bool:
+def isunittwist2(v: ArrayLike3, tol: float = 20) -> bool:
     r"""
     Test if vector represents a unit twist in SE(2) or SE(3)
 
     :param v: twist vector to test
     :type v: array_like(3)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: whether vector has unit length
     :rtype: bool
     :raises ValueError: for incorrect vector length
 
     Vector is is intepretted as :math:`[v, \omega]` where :math:`v \in \mathbb{R}^n` and
     :math:`\omega \in \mathbb{R}^1` for SE(2) and :math:`\omega \in \mathbb{R}^3` for SE(3).
@@ -337,27 +341,27 @@
     :seealso: unit, isunitvec
     """
     v = getvector(v)
 
     if len(v) == 3:
         # test for SE(2) twist
         return isunitvec(v[2], tol=tol) or (
-            np.abs(v[2]) < tol * _eps and isunitvec(v[0:2], tol=tol)
+            iszero(v[2], tol=tol) and isunitvec(v[0:2], tol=tol)
         )
     else:
         raise ValueError
 
 
-def unittwist(S: ArrayLike6, tol: float = 10) -> Union[R6, None]:
+def unittwist(S: ArrayLike6, tol: float = 20) -> Union[R6, None]:
     """
     Convert twist to unit twist
 
     :param S: twist vector
     :type S: array_like(6)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: unit twist
     :rtype: ndarray(6)
 
     A unit twist is a twist where:
 
     - the rotation part has unit magnitude
@@ -376,29 +380,31 @@
 
     if iszerovec(S, tol=tol):
         return None
 
     v = S[0:3]
     w = S[3:6]
 
-    if iszerovec(w):
+    if iszerovec(w, tol=tol):
         th = norm(v)
     else:
         th = norm(w)
 
     return S / th
 
 
-def unittwist_norm(S: Union[R6, ArrayLike6], tol: float = 10) -> Tuple[R6, float]:
+def unittwist_norm(
+    S: Union[R6, ArrayLike6], tol: float = 20
+) -> Tuple[Union[R6, None], Union[float, None]]:
     """
     Convert twist to unit twist and norm
 
     :param S: twist vector
     :type S: array_like(6)
-    :param tol: tolerance in units of eps
+    :param tol: tolerance in units of eps, defaults to 20
     :type tol: float
     :return: unit twist and scalar motion
     :rtype: tuple (ndarray(6), float)
 
     A unit twist is a twist where:
 
     - the rotation part has unit magnitude
@@ -416,88 +422,104 @@
 
     .. note:: Returns (None,None) if the twist has zero magnitude
     """
 
     S = getvector(S, 6)
 
     if iszerovec(S, tol=tol):
-        raise ValueError("zero norm")
+        return (None, None)  # according to "note" in docstring.
 
     v = S[0:3]
     w = S[3:6]
 
-    if iszerovec(w):
+    if iszerovec(w, tol=tol):
         th = norm(v)
     else:
         th = norm(w)
 
     return (S / th, th)
 
 
-def unittwist2(S: ArrayLike3) -> R3:
+def unittwist2(S: ArrayLike3, tol: float = 20) -> Union[R3, None]:
     """
     Convert twist to unit twist
 
     :param S: twist vector
     :type S: array_like(3)
+    :param tol: tolerance in units of eps, defaults to 20
+    :type tol: float
     :return: unit twist
     :rtype: ndarray(3)
 
     A unit twist is a twist where:
 
     - the rotation part has unit magnitude
     - if the rotational part is zero, then the translational part has unit magnitude
 
     .. runblock:: pycon
 
         >>> from spatialmath.base import *
         >>> unittwist2([2, 4, 2)
         >>> unittwist2([2, 0, 0])
 
+    .. note:: Returns None if the twist has zero magnitude
     """
 
     S = getvector(S, 3)
+
+    if iszerovec(S, tol=tol):
+        return None
+
     v = S[0:2]
     w = S[2]
 
-    if iszero(w):
+    if iszero(w, tol=tol):
         th = norm(v)
     else:
         th = abs(w)
 
     return S / th
 
 
-def unittwist2_norm(S: ArrayLike3) -> Tuple[R3, float]:
+def unittwist2_norm(
+    S: ArrayLike3, tol: float = 20
+) -> Tuple[Union[R3, None], Union[float, None]]:
     """
     Convert twist to unit twist
 
     :param S: twist vector
     :type S: array_like(3)
+    :param tol: tolerance in units of eps, defaults to 20
+    :type tol: float
     :return: unit twist and scalar motion
     :rtype: tuple (ndarray(3), float)
 
     A unit twist is a twist where:
 
     - the rotation part has unit magnitude
     - if the rotational part is zero, then the translational part has unit magnitude
 
     .. runblock:: pycon
 
         >>> from spatialmath.base import *
         >>> unittwist2([2, 4, 2)
         >>> unittwist2([2, 0, 0])
 
+    .. note:: Returns (None, None) if the twist has zero magnitude
     """
 
     S = getvector(S, 3)
+
+    if iszerovec(S, tol=tol):
+        return (None, None)
+
     v = S[0:2]
     w = S[2]
 
-    if iszero(w):
+    if iszero(w, tol=tol):
         th = norm(v)
     else:
         th = abs(w)
 
     return (S / th, th)
 
 
@@ -643,15 +665,19 @@
     :seealso: :func:`vector_diff` :func:`wrap_mpi_pi`
     """
     a = getvector(a)
     if b is not None:
         b = getvector(b)
         a = a - b  # cannot use -= here, numpy wont broadcast
 
-    return np.mod(a + math.pi, 2 * math.pi) - math.pi
+    y = np.mod(a + math.pi, 2 * math.pi) - math.pi
+    if isinstance(y, np.ndarray) and len(y) == 1:
+        return float(y)
+    else:
+        return y
 
 
 def angle_std(theta: ArrayLike) -> float:
     r"""
     Standard deviation of angular values
 
     :param theta: angular values
@@ -712,15 +738,15 @@
     """
     if mode == "0:2pi":
         return wrap_0_2pi(theta)
     elif mode == "-pi:pi":
         return wrap_mpi_pi(theta)
     elif mode == "0:pi":
         return wrap_0_pi(theta)
-    elif mode == "0:pi":
+    elif mode == "-pi/2:pi/2":
         return wrap_mpi2_pi2(theta)
     else:
         raise ValueError("bad method specified")
 
 
 def vector_diff(v1: ArrayLike, v2: ArrayLike, mode: str) -> NDArray:
     """
@@ -759,21 +785,21 @@
             v[i] = wrap_0_pi(v[i])
         else:
             raise ValueError("bad mode character")
 
     return v
 
 
-def removesmall(v: ArrayLike, tol: float = 100) -> NDArray:
+def removesmall(v: ArrayLike, tol: float = 20) -> NDArray:
     """
     Set small values to zero
 
     :param v: any vector
     :type v: array_like(n) or ndarray(n,m)
-    :param tol: Tolerance in units of eps, defaults to 100
+    :param tol: Tolerance in units of eps, defaults to 20
     :type tol: int, optional
     :return: vector with small values set to zero
     :rtype: ndarray(n) or ndarray(n,m)
 
     Values with absolute value less than ``tol`` will be set to zero.
 
     .. runblock:: pycon
@@ -785,14 +811,48 @@
         >>> print(a)
         >>> print(a[3])
 
     """
     return np.where(np.abs(v) < tol * _eps, 0, v)
 
 
+def project(v1: ArrayLike3, v2: ArrayLike3) -> ArrayLike3:
+    """
+    Projects vector v1 onto v2. Returns a vector parallel to v2.
+
+    :param v1: vector to be projected
+    :type v1: array_like(n)
+    :param v2: vector to be projected onto
+    :type v2: array_like(n)
+    :return: vector projection of v1 onto v2 (parrallel to v2)
+    :rtype: ndarray(n)
+    """
+    return np.dot(v1, v2) * v2
+
+
+def orthogonalize(v1: ArrayLike3, v2: ArrayLike3, normalize: bool = True) -> ArrayLike3:
+    """
+    Orthoginalizes vector v1 with respect to v2 with minimum rotation.
+    Returns a the nearest vector to v1 that is orthoginal to v2.
+
+    :param v1: vector to be orthoginalized
+    :type v1: array_like(n)
+    :param v2: vector that returned vector will be orthoginal to
+    :type v2: array_like(n)
+    :param normalize: whether to normalize the output vector
+    :type normalize: bool
+    :return: nearest vector to v1 that is orthoginal to v2
+    :rtype: ndarray(n)
+    """
+    v_orth = v1 - project(v1, v2)
+    if normalize:
+        v_orth = v_orth / np.linalg.norm(v_orth)
+    return v_orth
+
+
 if __name__ == "__main__":  # pragma: no cover
     import pathlib
 
     exec(
         open(
             pathlib.Path(__file__).parent.parent.parent.absolute()
             / "tests"
```

### Comparing `spatialmath-python-1.1.8/spatialmath/baseposelist.py` & `spatialmath-python-1.1.9/spatialmath/baseposelist.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/baseposematrix.py` & `spatialmath-python-1.1.9/spatialmath/baseposematrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -878,16 +878,14 @@
 
     def _string_color(self, color: Optional[bool] = False) -> str:
         """
         Pretty print the matrix value
 
         :param color: colorise the output, defaults to False
         :type color: bool, optional
-        :param tol: zero values smaller than tol*eps, defaults to 10
-        :type tol: float, optional
         :return: multiline matrix representation
         :rtype: str
 
         Convert a matrix to a simple grid of numbers with optional
         colorization for an ANSI terminal console:
 
                 * red: rotational elements
```

### Comparing `spatialmath-python-1.1.8/spatialmath/geom2d.py` & `spatialmath-python-1.1.9/spatialmath/geom2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,55 +117,63 @@
         """
         Plot the line using matplotlib
 
         :param kwargs: arguments passed to Matplotlib ``pyplot.plot``
         """
         smb.plot_homline(self.line, **kwargs)
 
-    def intersect(self, other: Line2, tol: float = 10) -> R3:
+    def intersect(self, other: Line2, tol: float = 20) -> R3:
         """
         Intersection with line
 
         :param other: another 2D line
         :type other: Line2
+        :param tol: tolerance in units of eps, defaults to 20
+        :type tol: float
         :return: intersection point in homogeneous form
         :rtype: ndarray(3)
 
         If the lines are parallel then the third element of the returned
         homogeneous point will be zero (an ideal point).
         """
         # return intersection of 2 lines
         # return mindist and points if no intersect
         c = np.cross(self.line, other.line)
         return abs(c[2]) > tol * _eps
 
-    def contains(self, p: ArrayLike2, tol: float = 10) -> bool:
+    def contains(self, p: ArrayLike2, tol: float = 20) -> bool:
         """
         Test if point is in line
 
         :param p1: point to test
         :type p1: array_like(2) or array_like(3)
+        :param tol: tolerance in units of eps, defaults to 20
+        :type tol: float
         :return: True if point lies in the line
         :rtype: bool
         """
         p = smb.getvector(p)
         if len(p) == 2:
             p = np.r_[p, 1]
         return abs(np.dot(self.line, p)) < tol * _eps
 
     # variant that gives lambda
 
-    def intersect_segment(self, p1: ArrayLike2, p2: ArrayLike2) -> bool:
+    def intersect_segment(
+        self, p1: ArrayLike2, p2: ArrayLike2, tol: float = 20
+    ) -> bool:
         """
         Test for line intersecting line segment
 
         :param p1: start of line segment
         :type p1: array_like(2) or array_like(3)
         :param p2: end of line segment
         :type p2: array_like(2) or array_like(3)
+        :param tol: tolerance in units of eps, defaults to 20
+        :type tol: float
         :return: True if they intersect
         :rtype: bool
 
         Tests whether the line intersects the line segment defined by endpoints
         ``p1`` and ``p2`` which are given in Euclidean or homogeneous form.
         """
         p1 = smb.getvector(p1)
@@ -176,15 +184,15 @@
             p2 = np.r_[p2, 1]
 
         z1 = np.dot(self.line, p1)
         z2 = np.dot(self.line, p2)
 
         if np.sign(z1) != np.sign(z2):
             return True
-        if self.contains(p1) or self.contains(p2):
+        if self.contains(p1, tol=tol) or self.contains(p2, tol=tol):
             return True
         return False
 
     # these should have same names as for 3d case
     def distance_line_line(self):
         pass
 
@@ -1112,15 +1120,15 @@
         """
         return smb.ellipse(self.E, self.centre, resolution=resolution)
 
     def polygon(self, resolution=10) -> Polygon2:
         """
         Approximate with a polygon
 
-        :param resolution: number of polygon vertices, defaults to 10
+        :param resolution: number of polygon vertices, defaults to 20
         :type resolution: int, optional
         :return: a polygon approximating the ellipse
         :rtype: :class:`Polygon2` instance
 
         Return a polygon instance with ``resolution`` vertices.  A :class:`Polygon2`` can be
         used for intersection testing with lines or other polygons.
```

### Comparing `spatialmath-python-1.1.8/spatialmath/geom3d.py` & `spatialmath-python-1.1.9/spatialmath/geom3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,22 +172,22 @@
         :math:`d`.
 
 
         :seealso: :meth:`n`
         """
         return self.plane[3]
 
-    def contains(self, p: ArrayLike3, tol: float = 10) -> bool:
+    def contains(self, p: ArrayLike3, tol: float = 20) -> bool:
         """
         Test if point in plane
 
         :param p: A 3D point
         :type p: array_like(3)
-        :param tol: Tolerance, defaults to 10*_eps
-        :type tol: float in multiples of eps, optional
+        :param tol: tolerance in units of eps, defaults to 20
+        :type tol: float
         :return: if the point is in the plane
         :rtype: bool
         """
         return abs(np.dot(self.n, p) - self.d) < tol * _eps
 
     def plot(
         self,
@@ -614,22 +614,22 @@
         return np.dot(base.getvector(point, 3, out="row") - self.pp, self.uw)
 
     # ------------------------------------------------------------------------- #
     #  TESTS ON PLUCKER OBJECTS
     # ------------------------------------------------------------------------- #
 
     def contains(
-        self, x: Union[R3, Points3], tol: float = 50
+        self, x: Union[R3, Points3], tol: float = 20
     ) -> Union[bool, List[bool]]:
         """
         Test if points are on the line
 
         :param x: 3D point
         :type x: 3-element array_like, or ndarray(3,N)
-        :param tol: Tolerance in units of eps, defaults to 50
+        :param tol: Tolerance in units of eps, defaults to 20
         :type tol: float, optional
         :raises ValueError: Bad argument
         :return: Whether point is on the line
         :rtype: bool or numpy.ndarray(N) of bool
 
         ``line.contains(X)`` is true if the point ``X`` lies on the line defined by
         the Line3 object self.
@@ -645,76 +645,78 @@
                 bool(np.linalg.norm(np.cross(p - self.pp, self.w)) < tol * _eps)
                 for p in x.T
             ]
         else:
             raise ValueError("bad argument")
 
     def isequal(
-        l1, l2: Line3, tol: float = 10  # type: ignore
+        l1, l2: Line3, tol: float = 20  # type: ignore
     ) -> bool:  # pylint: disable=no-self-argument
         """
         Test if two lines are equivalent
 
         :param l2: Second line
         :type l2: ``Line3``
+        :param tol: Tolerance in multiples of eps, defaults to 20
+        :type tol: float, optional
         :return: lines are equivalent
         :rtype: bool
 
         ``L1 == L2`` is True if the ``Line3`` objects describe the same line in
         space.  Note that because of the over parameterization, lines can be
         equivalent even if their coordinate vectors are different.
 
         :seealso: :meth:`__eq__`
         """
         return bool(
             abs(1 - np.dot(base.unitvec(l1.vec), base.unitvec(l2.vec))) < tol * _eps
         )
 
     def isparallel(
-        l1, l2: Line3, tol: float = 10  # type: ignore
+        l1, l2: Line3, tol: float = 20  # type: ignore
     ) -> bool:  # pylint: disable=no-self-argument
         """
         Test if lines are parallel
 
         :param l2: Second line
         :type l2: ``Line3``
-        :param tol: Tolerance in multiples of eps, defaults to 10
+        :param tol: Tolerance in multiples of eps, defaults to 20
         :type tol: float, optional
         :return: lines are parallel
         :rtype: bool
 
         ``l1.isparallel(l2)`` is true if the two lines are parallel.
 
         ``l1 | l2`` as above but in binary operator form
 
         :seealso: :meth:`__or__` :meth:`intersects`
         """
         return bool(np.linalg.norm(np.cross(l1.w, l2.w)) < tol * _eps)
 
     def isintersecting(
-        l1, l2: Line3, tol: float = 10  # type: ignore
+        l1, l2: Line3, tol: float = 20  # type: ignore
     ) -> bool:  # pylint: disable=no-self-argument
         """
         Test if lines are intersecting
 
         :param l2: Second line
         :type l2: Line3
-        :param tol: Tolerance in multiples of eps, defaults to 10
+        :param tol: Tolerance in multiples of eps, defaults to 20
         :type tol: float, optional
         :return: lines intersect
         :rtype: bool
 
         ``l1.isintersecting(l2)`` is true if the two lines intersect.
 
         .. note:: Is ``False`` if the lines are equivalent since they would intersect at
               an infinite number of points.
 
         :seealso: :meth:`__xor__` :meth:`intersects` :meth:`isparallel`
         """
-        return not l1.isparallel(l2) and bool(abs(l1 * l2) < 10 * _eps)
+        return not l1.isparallel(l2, tol=tol) and bool(abs(l1 * l2) < tol * _eps)
 
     def __eq__(l1, l2: Line3) -> bool:  # type: ignore pylint: disable=no-self-argument
         """
         Test if two lines are equivalent
 
         :param l2: Second line
         :type l2: ``Line3``
@@ -820,22 +822,22 @@
                 - l2.w.reshape((3, 1)) @ l1.v.reshape((1, 3))
             ) * base.unitvec(np.cross(l1.w, l2.w))
         else:
             # lines don't intersect
             return None
 
     def distance(
-        l1, l2: Line3, tol: float = 10  # type:ignore
+        l1, l2: Line3, tol: float = 20  # type:ignore
     ) -> float:  # pylint: disable=no-self-argument
         """
         Minimum distance between lines
 
         :param l2: Second line
         :type l2: ``Line3``
-        :param tol: Tolerance in multiples of eps, defaults to 10
+        :param tol: Tolerance in multiples of eps, defaults to 20
         :type tol: float, optional
         :return: Closest distance between lines
         :rtype: float
 
         ``l1.distance(l2) is the minimum distance between two lines.
 
         .. note:: Works for parallel, skew and intersecting lines.
@@ -1069,22 +1071,22 @@
             raise ValueError("can only premultiply Line3 by SE3")
 
     # ------------------------------------------------------------------------- #
     #  PLUCKER LINE DISTANCE AND INTERSECTION
     # ------------------------------------------------------------------------- #
 
     def intersect_plane(
-        self, plane: Union[ArrayLike4, Plane3], tol: float = 100
+        self, plane: Union[ArrayLike4, Plane3], tol: float = 20
     ) -> Tuple[R3, float]:
         r"""
         Line intersection with a plane
 
         :param plane: A plane
         :type plane: array_like(4) or Plane3
-        :param tol: Tolerance in multiples of eps, defaults to 10
+        :param tol: Tolerance in multiples of eps, defaults to 20
         :type tol: float, optional
         :return: Intersection point, λ
         :rtype: ndarray(3), float
 
         - ``P, λ = line.intersect_plane(plane)`` is the point where the line
           intersects the plane, and the corresponding λ value.
           Return None, None if no intersection.
```

### Comparing `spatialmath-python-1.1.8/spatialmath/pose2d.py` & `spatialmath-python-1.1.9/spatialmath/pose2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -524,14 +524,54 @@
         - N>1, return an ndarray with shape=(N,2)
         """
         if len(self) == 1:
             return self.A[:2, 2]
         else:
             return np.array([x[:2, 2] for x in self.A])
 
+    @property
+    def x(self):
+        """
+        First element of the translational component of SE(2)
+
+        :param self: SE(2)
+        :type self: SE2 instance
+        :return: translational component
+        :rtype: float
+
+        ``v.x`` is the first element of the translational vector component.  If ``len(x)`` is:
+
+        - 1, return an float
+        - N>1, return an ndarray with shape=(N,)
+        """
+        if len(self) == 1:
+            return self.A[0, 2]
+        else:
+            return np.array([v[0, 2] for v in self.A])
+
+    @property
+    def y(self):
+        """
+        Second element of the translational component of SE(2)
+
+        :param self: SE(2)
+        :type self: SE2 instance
+        :return: translational component
+        :rtype: float
+
+        ``v.y`` is the second element of the translational vector component.  If ``len(x)`` is:
+
+        - 1, return an float
+        - N>1, return an ndarray with shape=(N,)
+        """
+        if len(self) == 1:
+            return self.A[1, 2]
+        else:
+            return np.array([v[1, 2] for v in self.A])
+
     def xyt(self):
         r"""
         SE(2) as a configuration vector
 
         :return: An array :math:`[x, y, \theta]` :rtype: numpy.ndarray
 
         ``x.xyt`` is the rigidbody motion in minimal form as a translation and
```

### Comparing `spatialmath-python-1.1.8/spatialmath/pose3d.py` & `spatialmath-python-1.1.9/spatialmath/pose3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 # pylint: disable=invalid-name
 
 import numpy as np
 
 import spatialmath.base as smb
 from spatialmath.base.types import *
+from spatialmath.base.vectors import orthogonalize
 from spatialmath.baseposematrix import BasePoseMatrix
 from spatialmath.pose2d import SE2
 
 from spatialmath.twist import Twist3
 
 
 # ============================== SO3 =====================================#
@@ -647,16 +648,18 @@
         :param z: new z-axis, defaults to None
         :type z: str, array_like(3), optional
 
         Create a rotation by defining the direction of two of the new
         axes in terms of the old axes.  Axes are denoted by strings ``"x"``,
         ``"y"``, ``"z"``, ``"-x"``, ``"-y"``, ``"-z"``.
 
-        The directions can also be specified by 3-element vectors, but these
-        must be orthogonal.
+        The directions can also be specified by 3-element vectors. If the vectors are not orthogonal,
+        they will orthogonalized w.r.t. the first available dimension. I.e. if x is available, it will be
+        normalized and the remaining vector will be orthogonalized w.r.t. x, else, y will be normalized
+        and z will be orthogonalized w.r.t. y.
 
         To create a rotation where the new frame has its x-axis in -z-direction
         of the previous frame, and its z-axis in the x-direction of the previous
         frame is::
 
             >>> SO3.TwoVectors(x='-z', z='x')
         """
@@ -675,33 +678,49 @@
                     v = [0, sign, 0]
                 elif v[0] == "z":
                     v = [0, 0, sign]
                 return np.r_[v]
             else:
                 return smb.unitvec(smb.getvector(v, 3))
 
-        if x is not None and y is not None and z is None:
+        if x is not None and y is not None and z is not None:
+            raise ValueError(
+                "Only two vectors should be provided. Please set one to None."
+            )
+
+        elif x is not None and y is not None and z is None:
             # z = x x y
             x = vval(x)
             y = vval(y)
+            # Orthogonalizes y w.r.t. x
+            y = orthogonalize(y, x, normalize=True)
             z = np.cross(x, y)
 
         elif x is None and y is not None and z is not None:
             # x = y x z
             y = vval(y)
             z = vval(z)
+            # Orthogonalizes z w.r.t. y
+            z = orthogonalize(z, y, normalize=True)
             x = np.cross(y, z)
 
         elif x is not None and y is None and z is not None:
             # y = z x x
             z = vval(z)
             x = vval(x)
+            # Orthogonalizes z w.r.t. x
+            z = orthogonalize(z, x, normalize=True)
             y = np.cross(z, x)
 
-        return cls(np.c_[x, y, z], check=False)
+        else:
+            raise ValueError(
+                "Insufficient number of vectors. Please provide exactly two vectors."
+            )
+
+        return cls(np.c_[x, y, z], check=True)
 
     @classmethod
     def AngleAxis(cls, theta: float, v: ArrayLike3, *, unit: str = "rad") -> Self:
         r"""
         Construct a new SO(3) rotation matrix from rotation angle and axis
 
         :param theta: rotation
@@ -957,37 +976,32 @@
             # just one argument passed
 
             if super().arghandler(x, check=check):
                 return
             elif isinstance(x, SO3):
                 self.data = [smb.r2t(_x) for _x in x.data]
             elif isinstance(x, SE2):  # type(x).__name__ == "SE2":
-
-                def convert(x):
-                    # convert SE(2) to SE(3)
-                    out = np.identity(4, dtype=x.dtype)
-                    out[:2, :2] = x[:2, :2]
-                    out[:2, 3] = x[:2, 2]
-                    return out
-
-                self.data = [convert(_x) for _x in x.data]
+                self.data = x.SE3().data
             elif smb.isvector(x, 3):
                 # SE3( [x, y, z] )
                 self.data = [smb.transl(x)]
             elif isinstance(x, np.ndarray) and x.shape[1] == 3:
                 # SE3( Nx3 )
                 self.data = [smb.transl(T) for T in x]
 
             else:
                 raise ValueError("bad argument to constructor")
 
         elif y is not None and z is not None:
             # SE3(x, y, z)
             self.data = [smb.transl(x, y, z)]
 
+        else:
+            raise ValueError("Invalid arguments. See documentation for correct format.")
+
     @staticmethod
     def _identity() -> NDArray:
         return np.eye(4)
 
     # ------------------------------------------------------------------------ #
     @property
     def shape(self) -> Tuple[int, int]:
@@ -1032,14 +1046,113 @@
     @t.setter
     def t(self, v: ArrayLike3):
         if len(self) > 1:
             raise ValueError("can only assign translation to length 1 object")
         v = smb.getvector(v, 3)
         self.A[:3, 3] = v
 
+    @property
+    def x(self) -> float:
+        """
+        First element of translational component of SE(3)
+
+        :return: first element of translational component of SE(3)
+        :rtype: float
+
+        If ``len(v) > 1``, return an array with shape=(N,).
+
+        Example:
+
+        .. runblock:: pycon
+
+            >>> from spatialmath import SE3
+            >>> v = SE3(1,2,3)
+            >>> v.x
+            >>> v = SE3([ SE3(1,2,3), SE3(4,5,6)])
+            >>> v.x
+
+        :SymPy: supported
+        """
+        if len(self) == 1:
+            return self.A[0, 3]
+        else:
+            return np.array([v[0, 3] for v in self.A])
+
+    @x.setter
+    def x(self, x: float):
+        if len(self) > 1:
+            raise ValueError("can only assign elements to length 1 object")
+        self.A[0, 3] = x
+
+    @property
+    def y(self) -> float:
+        """
+        Second element of translational component of SE(3)
+
+        :return: second element of translational component of SE(3)
+        :rtype: float
+
+        If ``len(v) > 1``, return an array with shape=(N,).
+
+        Example:
+
+        .. runblock:: pycon
+
+            >>> from spatialmath import SE3
+            >>> v = SE3(1,2,3)
+            >>> v.y
+            >>> v = SE3([ SE3(1,2,3), SE3(4,5,6)])
+            >>> v.y
+
+        :SymPy: supported
+        """
+        if len(self) == 1:
+            return self.A[1, 3]
+        else:
+            return np.array([v[1, 3] for v in self.A])
+
+    @y.setter
+    def y(self, y: float):
+        if len(self) > 1:
+            raise ValueError("can only assign elements to length 1 object")
+        self.A[1, 3] = y
+
+    @property
+    def z(self) -> float:
+        """
+        Third element of translational component of SE(3)
+
+        :return: third element of translational component of SE(3)
+        :rtype: float
+
+        If ``len(v) > 1``, return an array with shape=(N,).
+
+        Example:
+
+        .. runblock:: pycon
+
+            >>> from spatialmath import SE3
+            >>> v = SE3(1,2,3)
+            >>> v.z
+            >>> v = SE3([ SE3(1,2,3), SE3(4,5,6)])
+            >>> v.z
+
+        :SymPy: supported
+        """
+        if len(self) == 1:
+            return self.A[2, 3]
+        else:
+            return np.array([v[2, 3] for v in self.A])
+
+    @z.setter
+    def z(self, z: float):
+        if len(self) > 1:
+            raise ValueError("can only assign elements to length 1 object")
+        self.A[2, 3] = z
+
     # ------------------------------------------------------------------------ #
 
     def inv(self) -> SE3:
         r"""
         Inverse of SE(3)
 
         :return: inverse
@@ -1067,14 +1180,47 @@
         :SymPy: supported
         """
         if len(self) == 1:
             return SE3(smb.trinv(self.A), check=False)
         else:
             return SE3([smb.trinv(x) for x in self.A], check=False)
 
+    def yaw_SE2(self, order: str = "zyx") -> SE2:
+        """
+        Create SE(2) from SE(3) yaw angle.
+
+        :param order: angle sequence order, default to 'zyx'
+        :type order: str
+        :return: SE(2) with same rotation as the yaw angle using the roll-pitch-yaw convention,
+            and translation along the roll-pitch axes.
+        :rtype: SE2 instance
+
+        Roll-pitch-yaw corresponds to successive rotations about the axes specified by ``order``:
+
+            - ``'zyx'`` [default], rotate by yaw about the z-axis, then by pitch about the new y-axis,
+              then by roll about the new x-axis.  Convention for a mobile robot with x-axis forward
+              and y-axis sideways.
+            - ``'xyz'``, rotate by yaw about the x-axis, then by pitch about the new y-axis,
+              then by roll about the new z-axis. Convention for a robot gripper with z-axis forward
+              and y-axis between the gripper fingers.
+            - ``'yxz'``, rotate by yaw about the y-axis, then by pitch about the new x-axis,
+              then by roll about the new z-axis. Convention for a camera with z-axis parallel
+              to the optic axis and x-axis parallel to the pixel rows.
+
+        """
+        if len(self) == 1:
+            if order == "zyx":
+                return SE2(self.x, self.y, self.rpy(order = order)[2])
+            elif order == "xyz":
+                return SE2(self.z, self.y, self.rpy(order = order)[2])
+            elif order == "yxz":
+                return SE2(self.z, self.x, self.rpy(order = order)[2])
+        else:
+            return SE2([e.yaw_SE2() for e in self])
+
     def delta(self, X2: Optional[SE3] = None) -> R6:
         r"""
         Infinitesimal difference of SE(3) values
 
         :return: differential motion vector
         :rtype: ndarray(6)
 
@@ -1806,14 +1952,35 @@
         else:
             raise ValueError("expecting SO3 or rotation matrix")
 
         if t is None:
             t = np.zeros((3,))
         return cls(smb.rt2tr(R, t, check=check), check=check)
 
+    @classmethod
+    def CopyFrom(
+        cls,
+        T: SE3Array,
+        check: bool = True
+    ) -> SE3:
+        """
+        Create an SE(3) from a 4x4 numpy array that is passed by value.
+
+        :param T: homogeneous transformation
+        :type T: ndarray(4, 4)
+        :param check: check rotation validity, defaults to True
+        :type check: bool, optional
+        :raises ValueError: bad rotation matrix, bad transformation matrix
+        :return: SE(3) matrix representing that transformation
+        :rtype: SE3 instance
+        """
+        if T is None:
+            raise ValueError("Transformation matrix must not be None")
+        return cls(np.copy(T), check=check)
+
     def angdist(self, other: SE3, metric: int = 6) -> float:
         r"""
         Angular distance metric between poses
 
         :param other: second rotation
         :type other: SE3 instance
         :param metric: metric, default is 6
```

### Comparing `spatialmath-python-1.1.8/spatialmath/quaternion.py` & `spatialmath-python-1.1.9/spatialmath/quaternion.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,21 +389,23 @@
 
         :reference: `Wikipedia <https://en.wikipedia.org/wiki/Quaternion#Exponential,_logarithm,_and_power_functions>`_
 
         :seealso: :meth:`Quaternion.exp` :meth:`Quaternion.log` :meth:`UnitQuaternion.angvec`
         """
         norm = self.norm()
         s = math.log(norm)
-        v = math.acos(self.s / norm) * smb.unitvec(self.v)
+        v = math.acos(np.clip(self.s / norm, -1, 1)) * smb.unitvec(self.v)
         return Quaternion(s=s, v=v)
 
-    def exp(self) -> Quaternion:
+    def exp(self, tol: float = 20) -> Quaternion:
         r"""
         Exponential of quaternion
 
+        :param tol: Tolerance when checking for pure quaternion, in multiples of eps, defaults to 20
+        :type tol: float, optional
         :rtype: Quaternion instance
 
         ``q.exp()`` is the exponential of the quaternion ``q``, ie.
 
         .. math::
 
              e^s \cos \| v \|,  \langle e^s \frac{\vec{v}}{\| \vec{v} \|} \sin \| \vec{v} \| \rangle
@@ -429,15 +431,15 @@
 
         :seealso: :meth:`Quaternion.log` :meth:`UnitQuaternion.log` :meth:`UnitQuaternion.AngVec` :meth:`UnitQuaternion.EulerVec`
         """
         exp_s = math.exp(self.s)
         norm_v = smb.norm(self.v)
         s = exp_s * math.cos(norm_v)
         v = exp_s * self.v / norm_v * math.sin(norm_v)
-        if abs(self.s) < 100 * _eps:
+        if abs(self.s) < tol * _eps:
             # result will be a unit quaternion
             return UnitQuaternion(s=s, v=v)
         else:
             return Quaternion(s=s, v=v)
 
     def inner(self, other) -> float:
         """
@@ -985,29 +987,36 @@
 
             elif isinstance(s, np.ndarray):
                 # passed a NumPy array, it could be:
                 #  an SO(3) or SE(3) matrix
                 #  a quaternion as a 1D array
                 #  an array of quaternions as an nx4 array
 
-                if smb.isrot(s, check=check):
-                    # UnitQuaternion(R) R is 3x3 rotation matrix
-                    self.data = [smb.r2q(s)]
+                if s.shape == (3, 3):
+                    if smb.isrot(s, check=check):
+                        # UnitQuaternion(R) R is 3x3 rotation matrix
+                        self.data = [smb.r2q(s)]
+                    else:
+                        raise ValueError(
+                            "invalid rotation matrix provided to UnitQuaternion constructor"
+                        )
                 elif s.shape == (4,):
                     # passed a 4-vector
                     if norm:
                         self.data = [smb.qunit(s)]
                     else:
                         self.data = [s]
                 elif s.ndim == 2 and s.shape[1] == 4:
                     if norm:
                         self.data = [smb.qunit(x) for x in s]
                     else:
                         # self.data = [smb.qpositive(x) for x in s]
                         self.data = [x for x in s]
+                else:
+                    raise ValueError("array could not be interpreted as UnitQuaternion")
 
             elif isinstance(s, SO3):
                 # UnitQuaternion(x) x is SO3 or SE3 (since SE3 is subclass of SO3)
                 self.data = [smb.r2q(x.R) for x in s]
 
             elif isinstance(s[0], SO3):
                 # list of SO3 or SE3
@@ -2229,30 +2238,30 @@
         """
         if not isinstance(other, UnitQuaternion):
             raise TypeError("bad operand")
 
         if metric == 0:
             measure = lambda p, q: 1 - abs(np.dot(p, q))
         elif metric == 1:
-            measure = lambda p, q: math.acos(abs(np.dot(p, q)))
+            measure = lambda p, q: math.acos(min(1.0, abs(np.dot(p, q))))
         elif metric == 2:
-            measure = lambda p, q: math.acos(abs(np.dot(p, q)))
+            measure = lambda p, q: math.acos(min(1.0, abs(np.dot(p, q))))
         elif metric == 3:
 
             def metric3(p, q):
                 x = smb.norm(p - q)
                 y = smb.norm(p + q)
                 if x >= y:
                     return 2 * math.atan(y / x)
                 else:
                     return 2 * math.atan(x / y)
 
             measure = metric3
         elif metric == 4:
-            measure = lambda p, q: math.acos(2 * np.dot(p, q) ** 2 - 1)
+            measure = lambda p, q: math.acos(min(1.0, 2 * np.dot(p, q) ** 2 - 1))
 
         ad = self.binop(other, measure)
         if len(ad) == 1:
             return ad[0]
         else:
             return np.array(ad)
```

### Comparing `spatialmath-python-1.1.8/spatialmath/spatialvector.py` & `spatialmath-python-1.1.9/spatialmath/spatialvector.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
         :param m: mass
         :type m: float
         :param r: centre of mass relative to link frame
         :type r: 3-element array_like
         :param I: inertia about the centre of mass, axes aligned with link frame
         :type I: numpy.array, shape=(6,6)
 
-        - ``SpatialInertia(m, r I)`` is a spatial inertia object for a rigid-body
+        - ``SpatialInertia(m, r, I)`` is a spatial inertia object for a rigid-body
           with mass ``m``, centre of mass at ``r`` relative to the link frame, and an
           inertia matrix ``I`` (3x3) about the centre of mass.
 
         - ``SpatialInertia(I)`` is a spatial inertia object with a value equal
           to ``I`` (6x6).
 
         :SymPy: supported
@@ -584,30 +584,30 @@
         :param x: matrix to test
         :type x: numpy.ndarray
         :arg check: ignored
         :type check: bool
         :return: True if the matrix has shape (6,6).
         :rtype: bool
         """
-        return self.shape == SpatialVector.shape
+        return self.shape == x.shape
 
+    @property
     def shape(self):
         """
         Shape of the object's interal matrix representation
 
         :return: (6,6)
         :rtype: tuple
         """
         return (6, 6)
 
     def __getitem__(self, i):
         return SpatialInertia(self.data[i])
 
     def __repr__(self):
-
         """
         Convert to string
 
         s = SI.char() is a string showing spatial inertia parameters in a
         compact format.
         If SI is an array of spatial inertia objects return a string with the
         inertia values in a vertical list.
@@ -630,15 +630,15 @@
         :raises TypeError: attempting to add invalid type to SpatialInertia
 
         - ``SI1 + SI2`` is the SpatialInertia of a composite body when bodies with
            SpatialInertia ``SI1`` and ``SI2`` are connected.
         """
         if not isinstance(right, SpatialInertia):
             raise TypeError("can only add spatial inertia to spatial inertia")
-        return SpatialInertia(left.I + left.I)
+        return SpatialInertia(left.A + right.A)
 
     def __mul__(
         left, right
     ):  # lgtm[py/not-named-self] pylint: disable=no-self-argument
         """
         Overloaded ``*`` operator (superclass method)
 
@@ -678,15 +678,14 @@
           the SpatialAcceleration ``a``.
         - ``v * I`` is the SpatialMomemtum of a body with SpatialInertia ``I`` and SpatialVelocity ``v``.
         """
         return right.__mul__(left)
 
 
 if __name__ == "__main__":
-
     import numpy.testing as nt
     import pathlib
 
     v = SpatialVelocity()
     print(v)
     print(len(v))
     v.append(v)
```

### Comparing `spatialmath-python-1.1.8/spatialmath/timing.py` & `spatialmath-python-1.1.9/spatialmath/timing.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath/twist.py` & `spatialmath-python-1.1.9/spatialmath/twist.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/spatialmath_python.egg-info/SOURCES.txt` & `spatialmath-python-1.1.9/spatialmath_python.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -3,42 +3,33 @@
 pyproject.toml
 spatialmath/DualQuaternion.py
 spatialmath/__init__.py
 spatialmath/baseposelist.py
 spatialmath/baseposematrix.py
 spatialmath/geom2d.py
 spatialmath/geom3d.py
-spatialmath/play_with_types.py
-spatialmath/pluckertest.py
 spatialmath/pose2d.py
 spatialmath/pose3d.py
-spatialmath/profiling.py
 spatialmath/quaternion.py
 spatialmath/spatialvector.py
-spatialmath/test.py
 spatialmath/timing.py
-spatialmath/timing_constructor.py
 spatialmath/twist.py
 spatialmath/base/__init__.py
 spatialmath/base/_types_311.py
 spatialmath/base/_types_35.py
 spatialmath/base/_types_39.py
 spatialmath/base/animate.py
-spatialmath/base/animationbug.py
 spatialmath/base/argcheck.py
 spatialmath/base/graphics.py
-spatialmath/base/m2p.py
 spatialmath/base/numeric.py
 spatialmath/base/quaternions.py
 spatialmath/base/symbolic.py
-spatialmath/base/timing.py
 spatialmath/base/transforms2d.py
 spatialmath/base/transforms3d.py
 spatialmath/base/transformsNd.py
-spatialmath/base/trplot2.py
 spatialmath/base/types.py
 spatialmath/base/vectors.py
 spatialmath_python.egg-info/PKG-INFO
 spatialmath_python.egg-info/SOURCES.txt
 spatialmath_python.egg-info/dependency_links.txt
 spatialmath_python.egg-info/requires.txt
 spatialmath_python.egg-info/top_level.txt
```

### Comparing `spatialmath-python-1.1.8/tests/test_baseposelist.py` & `spatialmath-python-1.1.9/tests/test_baseposelist.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/tests/test_dualquaternion.py` & `spatialmath-python-1.1.9/tests/test_dualquaternion.py`

 * *Files identical despite different names*

### Comparing `spatialmath-python-1.1.8/tests/test_geom2d.py` & `spatialmath-python-1.1.9/tests/test_geom2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 @author: corkep
 """
 
 from spatialmath.geom2d import *
 from spatialmath.pose2d import SE2
 
 import unittest
+import pytest
+import sys
 import numpy.testing as nt
 import spatialmath.base as smb
 
 
 class Polygon2Test(unittest.TestCase):
     # Primitives
     def test_constructor1(self):
@@ -81,14 +83,18 @@
 
         l = Line2.Join((-10, 0), (10, 0))
         self.assertTrue(p.intersects(l))
 
         l = Line2.Join((-10, 1.1), (10, 1.1))
         self.assertFalse(p.intersects(l))
 
+    @pytest.mark.skipif(
+        sys.platform.startswith("darwin") and sys.version_info < (3, 11),
+        reason="tkinter bug with mac",
+    )
     def test_plot(self):
         p = Polygon2(np.array([[-1, 1, 1, -1], [-1, -1, 1, 1]]))
         p.plot()
 
         p.animate(SE2(1, 2))
 
     def test_edges(self):
```

### Comparing `spatialmath-python-1.1.8/tests/test_geom3d.py` & `spatialmath-python-1.1.9/tests/test_geom3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from spatialmath.geom3d import *
 from spatialmath.pose3d import SE3
 
 import unittest
 import numpy.testing as nt
 import spatialmath.base as base
+import pytest
+import sys
 
 
 class Line3Test(unittest.TestCase):
     # Primitives
     def test_constructor1(self):
         # construct from 6-vector
 
@@ -119,14 +121,18 @@
         nt.assert_array_almost_equal(p, L.pp)
         self.assertEqual(d, L.ppd)
 
         p, d = L.closest_to_point([5, 1, 0])
         nt.assert_array_almost_equal(p, [5, 1, 2])
         self.assertAlmostEqual(d, 2)
 
+    @pytest.mark.skipif(
+        sys.platform.startswith("darwin") and sys.version_info < (3, 11),
+        reason="tkinter bug with mac",
+    )
     def test_plot(self):
         P = [2, 3, 7]
         Q = [2, 1, 0]
         L = Line3.Join(P, Q)
 
         fig = plt.figure()
         ax = fig.add_subplot(111, projection="3d", proj_type="ortho")
```

### Comparing `spatialmath-python-1.1.8/tests/test_pose2d.py` & `spatialmath-python-1.1.9/tests/test_pose2d.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,509 +1,490 @@
 import numpy.testing as nt
 import matplotlib.pyplot as plt
 import unittest
+import sys
+import pytest
 
 """
 we will assume that the primitives rotx,trotx, etc. all work
 """
 from math import pi
 from spatialmath.pose2d import *
+
 # from spatialmath import super_pose as sp
 from spatialmath.base import *
 import spatialmath.base.argcheck as argcheck
 import spatialmath as sm
 from spatialmath.baseposematrix import BasePoseMatrix
 from spatialmath.twist import BaseTwist
 
+
 def array_compare(x, y):
     if isinstance(x, BasePoseMatrix):
         x = x.A
     if isinstance(y, BasePoseMatrix):
         y = y.A
     if isinstance(x, BaseTwist):
         x = x.S
     if isinstance(y, BaseTwist):
         y = y.S
     nt.assert_array_almost_equal(x, y)
 
 
 class TestSO2(unittest.TestCase):
-
     @classmethod
     def tearDownClass(cls):
-        plt.close('all')
+        plt.close("all")
 
     def test_constructor(self):
-        
-        
         # null case
         x = SO2()
         self.assertIsInstance(x, SO2)
         self.assertEqual(len(x), 1)
-        array_compare(x.A, np.eye(2,2))
-        
+        array_compare(x.A, np.eye(2, 2))
+
         ## from angle
-        
+
         array_compare(SO2(0).A, np.eye(2))
         array_compare(SO2(pi / 2).A, rot2(pi / 2))
-        array_compare(SO2(90, unit='deg').A, rot2(pi / 2))
-       
+        array_compare(SO2(90, unit="deg").A, rot2(pi / 2))
+
         ## from R
-        
-        array_compare(SO2(np.eye(2,2)).A, np.eye(2,2))
-    
-        array_compare(SO2( rot2(pi / 2)).A, rot2(pi / 2))
-        array_compare(SO2( rot2(pi)).A, rot2(pi))
-           
-        
+
+        array_compare(SO2(np.eye(2, 2)).A, np.eye(2, 2))
+
+        array_compare(SO2(rot2(pi / 2)).A, rot2(pi / 2))
+        array_compare(SO2(rot2(pi)).A, rot2(pi))
+
         ## R,T
-        array_compare(SO2( np.eye(2)).R, np.eye(2))
-       
-        array_compare(SO2( rot2(pi / 2)).R, rot2(pi / 2))
-        
-        
+        array_compare(SO2(np.eye(2)).R, np.eye(2))
+
+        array_compare(SO2(rot2(pi / 2)).R, rot2(pi / 2))
+
         ## vectorised forms of R
         R = SO2.Empty()
         for theta in [-pi / 2, 0, pi / 2, pi]:
             R.append(SO2(theta))
         self.assertEqual(len(R), 4)
         array_compare(R[0], rot2(-pi / 2))
         array_compare(R[3], rot2(pi))
 
         # TODO self.assertEqual(SO2(R).R, R)
-        
+
         ## copy constructor
         r = SO2(0.3)
         c = SO2(r)
         array_compare(r, c)
         r = SO2(0.4)
         array_compare(c, SO2(0.3))
-    
+
     def test_concat(self):
         x = SO2()
         xx = SO2([x, x, x, x])
-        
+
         self.assertIsInstance(xx, SO2)
         self.assertEqual(len(xx), 4)
-    
+
     def test_primitive_convert(self):
         # char
-        
-        s = str( SO2())
+
+        s = str(SO2())
         self.assertIsInstance(s, str)
-    
+
     def test_shape(self):
         a = SO2()
         self.assertEqual(a._A.shape, a.shape)
 
     def test_constructor_Exp(self):
-
-        array_compare(SO2.Exp( skew(0.3)).R, rot2(0.3))
-        array_compare(SO2.Exp( 0.3).R, rot2(0.3))
+        array_compare(SO2.Exp(skew(0.3)).R, rot2(0.3))
+        array_compare(SO2.Exp(0.3).R, rot2(0.3))
 
         x = SO2.Exp([0, 0.3, 1])
         self.assertEqual(len(x), 3)
         array_compare(x[0], rot2(0))
         array_compare(x[1], rot2(0.3))
         array_compare(x[2], rot2(1))
 
         x = SO2.Exp([skew(x) for x in [0, 0.3, 1]])
         self.assertEqual(len(x), 3)
         array_compare(x[0], rot2(0))
         array_compare(x[1], rot2(0.3))
         array_compare(x[2], rot2(1))
-    
+
     def test_isa(self):
-        
         self.assertTrue(SO2.isvalid(rot2(0)))
-    
+
         self.assertFalse(SO2.isvalid(1))
-    
+
     def test_resulttype(self):
-        
         r = SO2()
         self.assertIsInstance(r, SO2)
-    
+
         self.assertIsInstance(r * r, SO2)
-        
-    
+
         self.assertIsInstance(r / r, SO2)
-        
+
         self.assertIsInstance(r.inv(), SO2)
-    
-    
+
     def test_multiply(self):
-        
         vx = np.r_[1, 0]
         vy = np.r_[0, 1]
-        
+
         r0 = SO2(0)
         r1 = SO2(pi / 2)
         r2 = SO2(pi)
         u = SO2()
-        
+
         ## SO2-SO2, product
         # scalar x scalar
-        
+
         array_compare(r0 * u, r0)
         array_compare(u * r0, r0)
-        
+
         # vector x vector
-        array_compare(SO2([r0, r1, r2]) * SO2([r2, r0, r1]), SO2([r0 * r2, r1 * r0, r2 * r1]))
-        
+        array_compare(
+            SO2([r0, r1, r2]) * SO2([r2, r0, r1]), SO2([r0 * r2, r1 * r0, r2 * r1])
+        )
+
         # scalar x vector
         array_compare(r1 * SO2([r0, r1, r2]), SO2([r1 * r0, r1 * r1, r1 * r2]))
-        
+
         # vector x scalar
         array_compare(SO2([r0, r1, r2]) * r2, SO2([r0 * r2, r1 * r2, r2 * r2]))
-        
+
         ## SO2-vector product
         # scalar x scalar
-        
+
         array_compare(r1 * vx, np.c_[vy])
-        
+
         # vector x vector
-        #array_compare(SO2([r0, r1, r0]) * np.c_[vy, vx, vx], np.c_[vy, vy, vx])
-        
+        # array_compare(SO2([r0, r1, r0]) * np.c_[vy, vx, vx], np.c_[vy, vy, vx])
+
         # scalar x vector
         array_compare(r1 * np.c_[vx, vy, -vx], np.c_[vy, -vx, -vy])
-        
+
         # vector x scalar
         array_compare(SO2([r0, r1, r2]) * vy, np.c_[vy, -vx, -vy])
 
-    
     def test_divide(self):
-        
         r0 = SO2(0)
         r1 = SO2(pi / 2)
         r2 = SO2(pi)
         u = SO2()
-        
+
         # scalar / scalar
         # implicity tests inv
-    
+
         array_compare(r1 / u, r1)
         array_compare(r1 / r1, u)
-    
+
         # vector / vector
-        array_compare(SO2([r0, r1, r2]) / SO2([r2, r1, r0]), SO2([r0 / r2, r1 / r1, r2 / r0]))
-        
+        array_compare(
+            SO2([r0, r1, r2]) / SO2([r2, r1, r0]), SO2([r0 / r2, r1 / r1, r2 / r0])
+        )
+
         # vector / scalar
         array_compare(SO2([r0, r1, r2]) / r1, SO2([r0 / r1, r1 / r1, r2 / r1]))
-    
-    
+
     def test_conversions(self):
-        
         T = SO2(pi / 2).SE2()
 
         self.assertIsInstance(T, SE2)
-    
-        
+
         ## Lie stuff
         th = 0.3
         RR = SO2(th)
         array_compare(RR.log(), skew(th))
-    
-    
+
     def test_miscellany(self):
-        
-        r = SO2( 0.3,)
+        r = SO2(
+            0.3,
+        )
         self.assertAlmostEqual(np.linalg.det(r.A), 1)
-        
+
         self.assertEqual(r.N, 2)
-        
+
         self.assertFalse(r.isSE)
-    
-    
+
     def test_printline(self):
-        
-        R = SO2( 0.3)
-        
+        R = SO2(0.3)
+
         R.printline()
         # s = R.printline(file=None)
         # self.assertIsInstance(s, str)
 
         R = SO2([0.3, 0.4, 0.5])
         s = R.printline(file=None)
         # self.assertIsInstance(s, str)
         # self.assertEqual(s.count('\n'), 2)
-        
+
+    @pytest.mark.skipif(
+        sys.platform.startswith("darwin") and sys.version_info < (3, 11),
+        reason="tkinter bug with mac",
+    )
     def test_plot(self):
-        plt.close('all')
-        
-        R = SO2( 0.3)
+        plt.close("all")
+
+        R = SO2(0.3)
         R.plot(block=False)
-        
+
         R2 = SO2(0.6)
         # R.animate()
         # R.animate(start=R2)
-        
-        
+
+
 # ============================== SE2 =====================================#
 
-class TestSE2(unittest.TestCase):
 
+class TestSE2(unittest.TestCase):
     @classmethod
     def tearDownClass(cls):
-        plt.close('all')
+        plt.close("all")
 
     def test_constructor(self):
-        
         self.assertIsInstance(SE2(), SE2)
-    
+
         ## null
-        array_compare(SE2().A, np.eye(3,3))
-        
+        array_compare(SE2().A, np.eye(3, 3))
+
         # from x,y
         x = SE2(2, 3)
         self.assertIsInstance(x, SE2)
         self.assertEqual(len(x), 1)
-        array_compare(x.A, np.array([[1,0,2],[0,1,3],[0,0,1]]))
-        
+        array_compare(x.A, np.array([[1, 0, 2], [0, 1, 3], [0, 0, 1]]))
+
         x = SE2([2, 3])
         self.assertIsInstance(x, SE2)
         self.assertEqual(len(x), 1)
-        array_compare(x.A, np.array([[1,0,2],[0,1,3],[0,0,1]]))
+        array_compare(x.A, np.array([[1, 0, 2], [0, 1, 3], [0, 0, 1]]))
 
         # from x,y,theta
         x = SE2(2, 3, pi / 2)
         self.assertIsInstance(x, SE2)
         self.assertEqual(len(x), 1)
-        array_compare(x.A, np.array([[0,-1,2],[1,0,3],[0,0,1]]))
-        
+        array_compare(x.A, np.array([[0, -1, 2], [1, 0, 3], [0, 0, 1]]))
+
         x = SE2([2, 3, pi / 2])
         self.assertIsInstance(x, SE2)
         self.assertEqual(len(x), 1)
-        array_compare(x.A, np.array([[0,-1,2],[1,0,3],[0,0,1]]))
-        
-        x = SE2(2, 3, 90, unit='deg')
+        array_compare(x.A, np.array([[0, -1, 2], [1, 0, 3], [0, 0, 1]]))
+
+        x = SE2(2, 3, 90, unit="deg")
         self.assertIsInstance(x, SE2)
         self.assertEqual(len(x), 1)
-        array_compare(x.A, np.array([[0,-1,2],[1,0,3],[0,0,1]]))
-        
-        x = SE2([2, 3, 90], unit='deg')
+        array_compare(x.A, np.array([[0, -1, 2], [1, 0, 3], [0, 0, 1]]))
+
+        x = SE2([2, 3, 90], unit="deg")
         self.assertIsInstance(x, SE2)
         self.assertEqual(len(x), 1)
-        array_compare(x.A, np.array([[0,-1,2],[1,0,3],[0,0,1]]))
-    
-        
+        array_compare(x.A, np.array([[0, -1, 2], [1, 0, 3], [0, 0, 1]]))
+
         ## T
         T = transl2(1, 2) @ trot2(0.3)
         x = SE2(T)
         self.assertIsInstance(x, SE2)
         self.assertEqual(len(x), 1)
         array_compare(x.A, T)
-        
-        
+
         ## copy constructor
         TT = SE2(x)
         array_compare(SE2(TT).A, T)
         x = SE2()
         array_compare(SE2(TT).A, T)
-        
+
         ## vectorised versions
-        
-        T1 = transl2(1,2) @ trot2(0.3)
-        T2 = transl2(1,-2) @ trot2(-0.4)
-        
-        x =SE2([T1, T2, T1, T2])
+
+        T1 = transl2(1, 2) @ trot2(0.3)
+        T2 = transl2(1, -2) @ trot2(-0.4)
+
+        x = SE2([T1, T2, T1, T2])
         self.assertIsInstance(x, SE2)
         self.assertEqual(len(x), 4)
         array_compare(x[0], T1)
         array_compare(x[1], T2)
 
     def test_shape(self):
         a = SE2()
         self.assertEqual(a._A.shape, a.shape)
 
     def test_concat(self):
         x = SE2()
         xx = SE2([x, x, x, x])
-        
+
         self.assertIsInstance(xx, SE2)
         self.assertEqual(len(xx), 4)
-    
-    
-    def test_constructor_Exp(self):
 
-        array_compare(SE2.Exp(skewa([1,2,0])), transl2(1,2))
-        array_compare(SE2.Exp(np.r_[1,2,0]), transl2(1,2))
+    def test_constructor_Exp(self):
+        array_compare(SE2.Exp(skewa([1, 2, 0])), transl2(1, 2))
+        array_compare(SE2.Exp(np.r_[1, 2, 0]), transl2(1, 2))
 
-        x = SE2.Exp([(1,2,0), (3,4,0), (5,6,0)])
+        x = SE2.Exp([(1, 2, 0), (3, 4, 0), (5, 6, 0)])
         self.assertEqual(len(x), 3)
-        array_compare(x[0], transl2(1,2))
-        array_compare(x[1], transl2(3,4))
-        array_compare(x[2], transl2(5,6))
+        array_compare(x[0], transl2(1, 2))
+        array_compare(x[1], transl2(3, 4))
+        array_compare(x[2], transl2(5, 6))
 
-        x = SE2.Exp([skewa(x) for x in [(1,2,0), (3,4,0), (5,6,0)]])
+        x = SE2.Exp([skewa(x) for x in [(1, 2, 0), (3, 4, 0), (5, 6, 0)]])
         self.assertEqual(len(x), 3)
-        array_compare(x[0], transl2(1,2))
-        array_compare(x[1], transl2(3,4))
-        array_compare(x[2], transl2(5,6))
-    
+        array_compare(x[0], transl2(1, 2))
+        array_compare(x[1], transl2(3, 4))
+        array_compare(x[2], transl2(5, 6))
+
     def test_isa(self):
-        
         self.assertTrue(SE2.isvalid(trot2(0)))
         self.assertFalse(SE2.isvalid(1))
 
-    
     def test_resulttype(self):
-        
         t = SE2()
         self.assertIsInstance(t, SE2)
         self.assertIsInstance(t * t, SE2)
         self.assertIsInstance(t / t, SE2)
         self.assertIsInstance(t.inv(), SE2)
         self.assertIsInstance(t + t, np.ndarray)
         self.assertIsInstance(t + 1, np.ndarray)
         self.assertIsInstance(t - 1, np.ndarray)
         self.assertIsInstance(1 + t, np.ndarray)
         self.assertIsInstance(1 - t, np.ndarray)
         self.assertIsInstance(2 * t, np.ndarray)
         self.assertIsInstance(t * 2, np.ndarray)
 
-    
-    def test_inverse(self):    
-        
+    def test_inverse(self):
         T1 = transl2(1, 2) @ trot2(0.3)
         TT1 = SE2(T1)
-        
+
         # test inverse
         array_compare(TT1.inv().A, np.linalg.inv(T1))
-        
-        array_compare(TT1 * TT1.inv(),  np.eye(3))
+
+        array_compare(TT1 * TT1.inv(), np.eye(3))
         array_compare(TT1.inv() * TT1, np.eye(3))
-        
+
         # vector case
         TT2 = SE2([TT1, TT1])
         u = [np.eye(3), np.eye(3)]
         array_compare(TT2.inv() * TT1, u)
-    
-    
+
     def test_Rt(self):
-       
-        
         TT1 = SE2.Rand()
         T1 = TT1.A
         R1 = t2r(T1)
         t1 = transl2(T1)
-        
+
         array_compare(TT1.A, T1)
         array_compare(TT1.R, R1)
         array_compare(TT1.t, t1)
-        
+        self.assertEqual(TT1.x, t1[0])
+        self.assertEqual(TT1.y, t1[1])
+
         TT = SE2([TT1, TT1, TT1])
         array_compare(TT.t, [t1, t1, t1])
-    
-    
+
     def test_arith(self):
-        
-        
         TT1 = SE2.Rand()
         T1 = TT1.A
         TT2 = SE2.Rand()
         T2 = TT2.A
-    
+
         I = SE2()
-        
+
         ## SE2, * SE2, product
         # scalar x scalar
-        
+
         array_compare(TT1 * TT2, T1 @ T2)
         array_compare(TT2 * TT1, T2 @ T1)
         array_compare(TT1 * I, T1)
         array_compare(TT2 * I, TT2)
 
-        
         # vector x vector
-        array_compare(SE2([TT1, TT1, TT2]) * SE2([TT2, TT1, TT1]), SE2([TT1*TT2, TT1*TT1, TT2*TT1]))
-        
+        array_compare(
+            SE2([TT1, TT1, TT2]) * SE2([TT2, TT1, TT1]),
+            SE2([TT1 * TT2, TT1 * TT1, TT2 * TT1]),
+        )
+
         # scalar x vector
-        array_compare(TT1 * SE2([TT2, TT1]), SE2([TT1*TT2, TT1*TT1]))
-        
+        array_compare(TT1 * SE2([TT2, TT1]), SE2([TT1 * TT2, TT1 * TT1]))
+
         # vector x scalar
-        array_compare(SE2([TT1, TT2]) * TT2, SE2([TT1*TT2, TT2*TT2]))
-        
+        array_compare(SE2([TT1, TT2]) * TT2, SE2([TT1 * TT2, TT2 * TT2]))
+
         ## SE2, * vector product
         vx = np.r_[1, 0]
         vy = np.r_[0, 1]
-    
+
         # scalar x scalar
-        
-        array_compare(TT1 * vy, h2e( T1 @ e2h(vy)))
-        
+
+        array_compare(TT1 * vy, h2e(T1 @ e2h(vy)))
+
         # # vector x vector
         # array_compare(SE2([TT1, TT2]) * np.c_[vx, vy], np.c_[h2e(T1 @ e2h(vx)), h2e(T2 @ e2h(vy))])
-        
+
         # scalar x vector
-        array_compare(TT1 * np.c_[vx, vy], h2e( T1 @ e2h(np.c_[vx, vy])))
-        
+        array_compare(TT1 * np.c_[vx, vy], h2e(T1 @ e2h(np.c_[vx, vy])))
+
         # vector x scalar
-        array_compare(SE2([TT1, TT2, TT1]) * vy, np.c_[h2e(T1 @ e2h(vy)), h2e(T2 @ e2h(vy)), h2e(T1 @ e2h(vy))])
-    
+        array_compare(
+            SE2([TT1, TT2, TT1]) * vy,
+            np.c_[h2e(T1 @ e2h(vy)), h2e(T2 @ e2h(vy)), h2e(T1 @ e2h(vy))],
+        )
+
     def test_defs(self):
-        
         # log
         # x = SE2.Exp([2, 3, 0.5])
         # array_compare(x.log(), np.array([[0, -0.5, 2], [0.5, 0, 3], [0, 0, 0]]))
         pass
-    
+
     def test_conversions(self):
-        
-        
         ##  SE2,                     convert to SE2, class
-    
+
         TT = SE2(1, 2, 0.3)
-        
+
         array_compare(TT, transl2(1, 2) @ trot2(0.3))
-        
+
         ## xyt
         array_compare(TT.xyt(), np.r_[1, 2, 0.3])
-        
+
         ## Lie stuff
         x = TT.log()
         self.assertTrue(isskewa(x))
 
-    
     def test_interp(self):
         TT = SE2(2, -4, 0.6)
         I = SE2()
-        
+
         z = I.interp(TT, s=0)
         self.assertIsInstance(z, SE2)
-        
+
         array_compare(I.interp(TT, s=0), I)
         array_compare(I.interp(TT, s=1), TT)
         array_compare(I.interp(TT, s=0.5), SE2(1, -2, 0.3))
-    
+
     def test_miscellany(self):
-        
         TT = SE2(1, 2, 0.3)
-        
-        self.assertEqual(TT.A.shape, (3,3))
-            
+
+        self.assertEqual(TT.A.shape, (3, 3))
+
         self.assertTrue(TT.isSE)
-        
+
         self.assertIsInstance(TT, SE2)
-    
+
     def test_display(self):
-        
         T1 = SE2.Rand()
-        
+
         T1.printline()
-        
+
+    @pytest.mark.skipif(
+        sys.platform.startswith("darwin") and sys.version_info < (3, 11),
+        reason="tkinter bug with mac",
+    )
     def test_graphics(self):
-        
-        plt.close('all')
+        plt.close("all")
         T1 = SE2.Rand()
         T2 = SE2.Rand()
-        
-        T1.plot(block=False, dims=[-2,2])
-        
-        T1.animate(repeat=False, dims=[-2,2], nframes=10)
-        T1.animate(T0=T2, repeat=False, dims=[-2,2], nframes=10)
 
+        T1.plot(block=False, dims=[-2, 2])
+
+        T1.animate(repeat=False, dims=[-2, 2], nframes=10)
+        T1.animate(T0=T2, repeat=False, dims=[-2, 2], nframes=10)
 
-# ---------------------------------------------------------------------------------------#
-if __name__ == '__main__':
 
+# ---------------------------------------------------------------------------------------#
+if __name__ == "__main__":
     unittest.main(buffer=True)
```

### Comparing `spatialmath-python-1.1.8/tests/test_pose3d.py` & `spatialmath-python-1.1.9/tests/test_pose3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy.testing as nt
 import matplotlib.pyplot as plt
 import unittest
+import sys
+import pytest
 
 """
 we will assume that the primitives rotx,trotx, etc. all work
 """
 from math import pi
 from spatialmath import SE3, SO3, SE2
 import numpy as np
-# from spatialmath import super_pose as sp
 from spatialmath.base import *
-from spatialmath.base import argcheck
-import spatialmath as sm
 from spatialmath.baseposematrix import BasePoseMatrix
 from spatialmath.twist import BaseTwist
 
+
 def array_compare(x, y):
     if isinstance(x, BasePoseMatrix):
         x = x.A
     if isinstance(y, BasePoseMatrix):
         y = y.A
     if isinstance(x, BaseTwist):
         x = x.S
@@ -26,18 +26,17 @@
         y = y.S
     nt.assert_array_almost_equal(x, y)
 
 
 class TestSO3(unittest.TestCase):
     @classmethod
     def tearDownClass(cls):
-        plt.close('all')
+        plt.close("all")
 
     def test_constructor(self):
-
         # null constructor
         R = SO3()
         nt.assert_equal(len(R), 1)
         array_compare(R, np.eye(3))
         self.assertIsInstance(R, SO3)
 
         # empty constructor
@@ -81,15 +80,14 @@
         # copy constructor
         R = SO3.Rx(pi / 2)
         R2 = SO3(R)
         R = SO3.Ry(pi / 2)
         array_compare(R2, rotx(pi / 2))
 
     def test_constructor_Eul(self):
-
         R = SO3.Eul([0.1, 0.2, 0.3])
         nt.assert_equal(len(R), 1)
         array_compare(R, eul2r([0.1, 0.2, 0.3]))
         self.assertIsInstance(R, SO3)
 
         R = SO3.Eul(0.1, 0.2, 0.3)
         nt.assert_equal(len(R), 1)
@@ -97,173 +95,193 @@
         self.assertIsInstance(R, SO3)
 
         R = SO3.Eul(np.r_[0.1, 0.2, 0.3])
         nt.assert_equal(len(R), 1)
         array_compare(R, eul2r([0.1, 0.2, 0.3]))
         self.assertIsInstance(R, SO3)
 
-        R = SO3.Eul([10, 20, 30], unit='deg')
+        R = SO3.Eul([10, 20, 30], unit="deg")
         nt.assert_equal(len(R), 1)
-        array_compare(R, eul2r([10, 20, 30], unit='deg'))
+        array_compare(R, eul2r([10, 20, 30], unit="deg"))
         self.assertIsInstance(R, SO3)
 
-        R = SO3.Eul(10, 20, 30, unit='deg')
+        R = SO3.Eul(10, 20, 30, unit="deg")
         nt.assert_equal(len(R), 1)
-        array_compare(R, eul2r([10, 20, 30], unit='deg'))
+        array_compare(R, eul2r([10, 20, 30], unit="deg"))
         self.assertIsInstance(R, SO3)
 
         # matrix input
 
-        angles = np.array([
-            [0.1, 0.2, 0.3],
-            [0.2, 0.3, 0.4],
-            [0.3, 0.4, 0.5],
-            [0.4, 0.5, 0.6]
-        ])
+        angles = np.array(
+            [[0.1, 0.2, 0.3], [0.2, 0.3, 0.4], [0.3, 0.4, 0.5], [0.4, 0.5, 0.6]]
+        )
         R = SO3.Eul(angles)
         self.assertIsInstance(R, SO3)
         nt.assert_equal(len(R), 4)
         for i in range(4):
-            array_compare(R[i], eul2r(angles[i,:]))
+            array_compare(R[i], eul2r(angles[i, :]))
 
         angles *= 10
-        R = SO3.Eul(angles, unit='deg')
+        R = SO3.Eul(angles, unit="deg")
         self.assertIsInstance(R, SO3)
         nt.assert_equal(len(R), 4)
         for i in range(4):
-            array_compare(R[i], eul2r(angles[i,:], unit='deg'))
-
+            array_compare(R[i], eul2r(angles[i, :], unit="deg"))
 
     def test_constructor_RPY(self):
-
-        R = SO3.RPY(0.1, 0.2, 0.3, order='zyx')
+        R = SO3.RPY(0.1, 0.2, 0.3, order="zyx")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2r([0.1, 0.2, 0.3], order='zyx'))
+        array_compare(R, rpy2r([0.1, 0.2, 0.3], order="zyx"))
         self.assertIsInstance(R, SO3)
 
-        R = SO3.RPY(10, 20, 30, unit='deg', order='zyx')
+        R = SO3.RPY(10, 20, 30, unit="deg", order="zyx")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2r([10, 20, 30], order='zyx', unit='deg'))
+        array_compare(R, rpy2r([10, 20, 30], order="zyx", unit="deg"))
         self.assertIsInstance(R, SO3)
 
-        R = SO3.RPY([0.1, 0.2, 0.3], order='zyx')
+        R = SO3.RPY([0.1, 0.2, 0.3], order="zyx")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2r([0.1, 0.2, 0.3], order='zyx'))
+        array_compare(R, rpy2r([0.1, 0.2, 0.3], order="zyx"))
         self.assertIsInstance(R, SO3)
 
-        R = SO3.RPY(np.r_[0.1, 0.2, 0.3], order='zyx')
+        R = SO3.RPY(np.r_[0.1, 0.2, 0.3], order="zyx")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2r([0.1, 0.2, 0.3], order='zyx'))
+        array_compare(R, rpy2r([0.1, 0.2, 0.3], order="zyx"))
         self.assertIsInstance(R, SO3)
 
         # check default
         R = SO3.RPY([0.1, 0.2, 0.3])
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2r([0.1, 0.2, 0.3], order='zyx'))
+        array_compare(R, rpy2r([0.1, 0.2, 0.3], order="zyx"))
         self.assertIsInstance(R, SO3)
 
         # XYZ order
 
-        R = SO3.RPY(0.1, 0.2, 0.3, order='xyz')
+        R = SO3.RPY(0.1, 0.2, 0.3, order="xyz")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2r([0.1, 0.2, 0.3], order='xyz'))
+        array_compare(R, rpy2r([0.1, 0.2, 0.3], order="xyz"))
         self.assertIsInstance(R, SO3)
 
-        R = SO3.RPY(10, 20, 30, unit='deg', order='xyz')
+        R = SO3.RPY(10, 20, 30, unit="deg", order="xyz")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2r([10, 20, 30], order='xyz', unit='deg'))
+        array_compare(R, rpy2r([10, 20, 30], order="xyz", unit="deg"))
         self.assertIsInstance(R, SO3)
 
-        R = SO3.RPY([0.1, 0.2, 0.3], order='xyz')
+        R = SO3.RPY([0.1, 0.2, 0.3], order="xyz")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2r([0.1, 0.2, 0.3], order='xyz'))
+        array_compare(R, rpy2r([0.1, 0.2, 0.3], order="xyz"))
         self.assertIsInstance(R, SO3)
 
-        R = SO3.RPY(np.r_[0.1, 0.2, 0.3], order='xyz')
+        R = SO3.RPY(np.r_[0.1, 0.2, 0.3], order="xyz")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2r([0.1, 0.2, 0.3], order='xyz'))
+        array_compare(R, rpy2r([0.1, 0.2, 0.3], order="xyz"))
         self.assertIsInstance(R, SO3)
 
         # matrix input
 
-        angles = np.array([
-            [0.1, 0.2, 0.3],
-            [0.2, 0.3, 0.4],
-            [0.3, 0.4, 0.5],
-            [0.4, 0.5, 0.6]
-        ])
-        R = SO3.RPY(angles, order='zyx')
+        angles = np.array(
+            [[0.1, 0.2, 0.3], [0.2, 0.3, 0.4], [0.3, 0.4, 0.5], [0.4, 0.5, 0.6]]
+        )
+        R = SO3.RPY(angles, order="zyx")
         self.assertIsInstance(R, SO3)
         nt.assert_equal(len(R), 4)
         for i in range(4):
-            array_compare(R[i], rpy2r(angles[i,:], order='zyx'))
+            array_compare(R[i], rpy2r(angles[i, :], order="zyx"))
 
         angles *= 10
-        R = SO3.RPY(angles, unit='deg', order='zyx')
+        R = SO3.RPY(angles, unit="deg", order="zyx")
         self.assertIsInstance(R, SO3)
         nt.assert_equal(len(R), 4)
         for i in range(4):
-            array_compare(R[i], rpy2r(angles[i,:], unit='deg', order='zyx'))
+            array_compare(R[i], rpy2r(angles[i, :], unit="deg", order="zyx"))
 
     def test_constructor_AngVec(self):
         # angvec
         R = SO3.AngVec(0.2, [1, 0, 0])
         nt.assert_equal(len(R), 1)
         array_compare(R, rotx(0.2))
         self.assertIsInstance(R, SO3)
 
         R = SO3.AngVec(0.3, [0, 1, 0])
         nt.assert_equal(len(R), 1)
         array_compare(R, roty(0.3))
         self.assertIsInstance(R, SO3)
 
-
+    def test_constructor_TwoVec(self):
+        # Randomly selected vectors
+        v1 = [1, 73, -42]
+        v2 = [0, 0.02, 57]
+        v3 = [-2, 3, 9]
+
+        # x and y given
+        R = SO3.TwoVectors(x=v1, y=v2)
+        self.assertIsInstance(R, SO3)
+        nt.assert_almost_equal(R.det(), 1, 5)
+        # x axis should equal normalized x vector
+        nt.assert_almost_equal(R.R[:, 0], v1 / np.linalg.norm(v1), 5)
+
+        # y and z given
+        R = SO3.TwoVectors(y=v2, z=v3)
+        self.assertIsInstance(R, SO3)
+        nt.assert_almost_equal(R.det(), 1, 5)
+        # y axis should equal normalized y vector
+        nt.assert_almost_equal(R.R[:, 1], v2 / np.linalg.norm(v2), 5)
+
+        # x and z given
+        R = SO3.TwoVectors(x=v3, z=v1)
+        self.assertIsInstance(R, SO3)
+        nt.assert_almost_equal(R.det(), 1, 5)
+        # x axis should equal normalized x vector
+        nt.assert_almost_equal(R.R[:, 0], v3 / np.linalg.norm(v3), 5)
 
     def test_shape(self):
         a = SO3()
         self.assertEqual(a._A.shape, a.shape)
 
     def test_about(self):
         R = SO3()
         R.about
 
     def test_str(self):
         R = SO3()
 
         s = str(R)
         self.assertIsInstance(s, str)
-        self.assertEqual(s.count('\n'), 3)
+        self.assertEqual(s.count("\n"), 3)
 
         s = repr(R)
         self.assertIsInstance(s, str)
-        self.assertEqual(s.count('\n'), 2)
+        self.assertEqual(s.count("\n"), 2)
 
     def test_printline(self):
-        
-        R = SO3.Rx( 0.3)
-        
+        R = SO3.Rx(0.3)
+
         R.printline()
         # s = R.printline(file=None)
         # self.assertIsInstance(s, str)
 
         R = SO3.Rx([0.3, 0.4, 0.5])
         s = R.printline(file=None)
         # self.assertIsInstance(s, str)
         # self.assertEqual(s.count('\n'), 2)
-        
+
+    @pytest.mark.skipif(
+        sys.platform.startswith("darwin") and sys.version_info < (3, 11),
+        reason="tkinter bug with mac",
+    )
     def test_plot(self):
-        plt.close('all')
-        
-        R = SO3.Rx( 0.3)
+        plt.close("all")
+
+        R = SO3.Rx(0.3)
         R.plot(block=False)
-        
+
         R2 = SO3.Rx(0.6)
         # R.animate()
         # R.animate(start=R.inv())
-        
+
     def test_listpowers(self):
         R = SO3()
         R1 = SO3.Rx(0.2)
         R2 = SO3.Ry(0.3)
 
         R.append(R1)
         R.append(R2)
@@ -285,24 +303,22 @@
         nt.assert_equal(len(R), 3)
         self.assertIsInstance(R, SO3)
         array_compare(R[0], rotx(0.1))
         array_compare(R[1], rotx(0.2))
         array_compare(R[2], rotx(0.3))
 
     def test_tests(self):
-
         R = SO3()
 
         self.assertEqual(R.isrot(), True)
         self.assertEqual(R.isrot2(), False)
         self.assertEqual(R.ishom(), False)
         self.assertEqual(R.ishom2(), False)
 
     def test_properties(self):
-
         R = SO3()
 
         self.assertEqual(R.isSO, True)
         self.assertEqual(R.isSE, False)
 
         array_compare(R.n, np.r_[1, 0, 0])
         array_compare(R.n, np.r_[1, 0, 0])
@@ -335,16 +351,14 @@
         array_compare(a, np.array([[2, 0, 0], [0, 2, 0], [0, 0, 2]]))
 
         # a =  np.eye(3) + R
         # self.assertNotIsInstance(a, SO3)
         # array_compare(a, np.array([ [2,0,0], [0,2,0], [0,0,2]]))
         #  this invokes the __add__ method for numpy
 
-
-
         # difference
         R = SO3()
 
         a = R - R
         self.assertNotIsInstance(a, SO3)
         array_compare(a, np.zeros((3, 3)))
 
@@ -425,34 +439,31 @@
 
         a = R / 2
         self.assertNotIsInstance(a, SO3)
         array_compare(a, roty(0.3) / 2)
 
         # power
 
-        R = SO3.Rx(pi/2)
+        R = SO3.Rx(pi / 2)
         R = R**2
         array_compare(R, SO3.Rx(pi))
 
-        R = SO3.Rx(pi/2)
+        R = SO3.Rx(pi / 2)
         R **= 2
         array_compare(R, SO3.Rx(pi))
 
-        R = SO3.Rx(pi/4)
-        R = R**(-2)
-        array_compare(R, SO3.Rx(-pi/2))
+        R = SO3.Rx(pi / 4)
+        R = R ** (-2)
+        array_compare(R, SO3.Rx(-pi / 2))
 
-        R = SO3.Rx(pi/4)
+        R = SO3.Rx(pi / 4)
         R **= -2
-        array_compare(R, SO3.Rx(-pi/2))
-
-
+        array_compare(R, SO3.Rx(-pi / 2))
 
     def test_arith_vect(self):
-
         rx = SO3.Rx(pi / 2)
         ry = SO3.Ry(pi / 2)
         rz = SO3.Rz(pi / 2)
         u = SO3()
 
         # multiply
         R = SO3([rx, ry, rz])
@@ -626,15 +637,14 @@
         a = R + 1
         self.assertNotIsInstance(a, SO3)
         nt.assert_equal(len(a), 3)
         array_compare(a[0], rx + 1)
         array_compare(a[1], ry + 1)
         array_compare(a[2], rz + 1)
 
-
         # subtract
         R = SO3([rx, ry, rz])
         a = R - rx
         self.assertNotIsInstance(a, SO3)
         nt.assert_equal(len(a), 3)
         array_compare(a[0], rx - rx)
         array_compare(a[1], ry - rx)
@@ -650,36 +660,55 @@
         a = R - R
         self.assertNotIsInstance(a, SO3)
         nt.assert_equal(len(a), 3)
         array_compare(a[0], rx - rx)
         array_compare(a[1], ry - ry)
         array_compare(a[2], rz - rz)
 
-
-
     def test_functions(self):
         # inv
         # .T
-        pass
+
+        # conversion to SE2
+        poseSE3 = SE3.Tx(3.3) * SE3.Rz(1.5)
+        poseSE2 = poseSE3.yaw_SE2()
+        nt.assert_almost_equal(poseSE3.R[0:2, 0:2], poseSE2.R[0:2, 0:2])
+        nt.assert_equal(poseSE3.x, poseSE2.x)
+        nt.assert_equal(poseSE3.y, poseSE2.y)
+
+        posesSE3 = SE3([poseSE3, poseSE3])
+        posesSE2 = posesSE3.yaw_SE2()
+        nt.assert_equal(len(posesSE2), 2)
 
     def test_functions_vect(self):
         # inv
         # .T
         pass
 
+    def test_functions_lie(self):
+        R = SO3.EulerVec([0.42, 0.73, -1.17])
+
+        # Check log and exponential map
+        nt.assert_equal(R, SO3.Exp(R.log()))
+        np.testing.assert_equal((R.inv() * R).log(), np.zeros([3, 3]))
+
+        # Check euler vector map
+        nt.assert_equal(R, SO3.EulerVec(R.eulervec()))
+        np.testing.assert_equal((R.inv() * R).eulervec(), np.zeros(3))
+
+
 # ============================== SE3 =====================================#
 
-class TestSE3(unittest.TestCase):
 
+class TestSE3(unittest.TestCase):
     @classmethod
     def tearDownClass(cls):
-        plt.close('all')
+        plt.close("all")
 
     def test_constructor(self):
-
         # null constructor
         R = SE3()
         nt.assert_equal(len(R), 1)
         array_compare(R, np.eye(4))
         self.assertIsInstance(R, SE3)
 
         # construct from matrix
@@ -727,37 +756,37 @@
         self.assertIsInstance(R, SE3)
 
         R = SE3.Eul(np.r_[0.1, 0.2, 0.3])
         nt.assert_equal(len(R), 1)
         array_compare(R, eul2tr([0.1, 0.2, 0.3]))
         self.assertIsInstance(R, SE3)
 
-        R = SE3.Eul([10, 20, 30], unit='deg')
+        R = SE3.Eul([10, 20, 30], unit="deg")
         nt.assert_equal(len(R), 1)
-        array_compare(R, eul2tr([10, 20, 30], unit='deg'))
+        array_compare(R, eul2tr([10, 20, 30], unit="deg"))
         self.assertIsInstance(R, SE3)
 
         R = SE3.RPY([0.1, 0.2, 0.3])
         nt.assert_equal(len(R), 1)
         array_compare(R, rpy2tr([0.1, 0.2, 0.3]))
         self.assertIsInstance(R, SE3)
 
         R = SE3.RPY(np.r_[0.1, 0.2, 0.3])
         nt.assert_equal(len(R), 1)
         array_compare(R, rpy2tr([0.1, 0.2, 0.3]))
         self.assertIsInstance(R, SE3)
 
-        R = SE3.RPY([10, 20, 30], unit='deg')
+        R = SE3.RPY([10, 20, 30], unit="deg")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2tr([10, 20, 30], unit='deg'))
+        array_compare(R, rpy2tr([10, 20, 30], unit="deg"))
         self.assertIsInstance(R, SE3)
 
-        R = SE3.RPY([0.1, 0.2, 0.3], order='xyz')
+        R = SE3.RPY([0.1, 0.2, 0.3], order="xyz")
         nt.assert_equal(len(R), 1)
-        array_compare(R, rpy2tr([0.1, 0.2, 0.3], order='xyz'))
+        array_compare(R, rpy2tr([0.1, 0.2, 0.3], order="xyz"))
         self.assertIsInstance(R, SE3)
 
         # angvec
         R = SE3.AngVec(0.2, [1, 0, 0])
         nt.assert_equal(len(R), 1)
         array_compare(R, trotx(0.2))
         self.assertIsInstance(R, SE3)
@@ -780,19 +809,33 @@
 
         # random
         T = SE3.Rand()
         R = T.R
         t = T.t
         T = SE3.Rt(R, t)
         self.assertIsInstance(T, SE3)
-        self.assertEqual(T.A.shape, (4,4))
+        self.assertEqual(T.A.shape, (4, 4))
 
         nt.assert_equal(T.R, R)
         nt.assert_equal(T.t, t)
 
+        nt.assert_equal(T.x, t[0])
+        nt.assert_equal(T.y, t[1])
+        nt.assert_equal(T.z, t[2])
+
+        TT = SE3([T, T, T])
+        desired_shape = (3,)
+        nt.assert_equal(TT.x.shape, desired_shape)
+        nt.assert_equal(TT.y.shape, desired_shape)
+        nt.assert_equal(TT.z.shape, desired_shape)
+
+        ones = np.ones(desired_shape)
+        nt.assert_equal(TT.x, ones * t[0])
+        nt.assert_equal(TT.y, ones * t[1])
+        nt.assert_equal(TT.z, ones * t[2])
 
         # copy constructor
         R = SE3.Rx(pi / 2)
         R2 = SE3(R)
         R = SE3.Ry(pi / 2)
         array_compare(R2, trotx(pi / 2))
 
@@ -802,17 +845,23 @@
         self.assertIsInstance(T, SE3)
         nt.assert_equal(T.A, np.eye(4))
 
         # SE2
         T = SE3(SE2(1, 2, 0.4))
         nt.assert_equal(len(T), 1)
         self.assertIsInstance(T, SE3)
-        self.assertEqual(T.A.shape, (4,4))
+        self.assertEqual(T.A.shape, (4, 4))
         nt.assert_equal(T.t, [1, 2, 0])
 
+        # Bad number of arguments
+        with self.assertRaises(ValueError):
+            T = SE3(1.0, 0.0)
+        with self.assertRaises(TypeError):
+            T = SE3(1.0, 0.0, 0.0, 0.0)
+
     def test_shape(self):
         a = SE3()
         self.assertEqual(a._A.shape, a.shape)
 
     def test_listpowers(self):
         R = SE3()
         R1 = SE3.Rx(0.2)
@@ -838,55 +887,70 @@
         nt.assert_equal(len(R), 3)
         self.assertIsInstance(R, SE3)
         array_compare(R[0], trotx(0.1))
         array_compare(R[1], trotx(0.2))
         array_compare(R[2], trotx(0.3))
 
     def test_tests(self):
-
         R = SE3()
 
         self.assertEqual(R.isrot(), False)
         self.assertEqual(R.isrot2(), False)
         self.assertEqual(R.ishom(), True)
         self.assertEqual(R.ishom2(), False)
 
     def test_properties(self):
-
         R = SE3()
 
         self.assertEqual(R.isSO, False)
         self.assertEqual(R.isSE, True)
 
         array_compare(R.n, np.r_[1, 0, 0])
         array_compare(R.n, np.r_[1, 0, 0])
         array_compare(R.n, np.r_[1, 0, 0])
 
         nt.assert_equal(R.N, 3)
         nt.assert_equal(R.shape, (4, 4))
 
+        # Testing the CopyFrom function
+        mutable_array = np.eye(4)
+        pass_by_ref = SE3(mutable_array)
+        pass_by_val = SE3.CopyFrom(mutable_array)
+        mutable_array[0, 3] = 5.0
+        nt.assert_allclose(pass_by_val.data[0], np.eye(4))
+        nt.assert_allclose(pass_by_ref.data[0], mutable_array)
+        nt.assert_raises(
+            AssertionError, nt.assert_allclose, pass_by_val.data[0], pass_by_ref.data[0]
+        )
+
     def test_arith(self):
         T = SE3(1, 2, 3)
 
         # sum
         a = T + T
         self.assertNotIsInstance(a, SE3)
-        array_compare(a, np.array([[2, 0, 0, 2], [0, 2, 0, 4], [0, 0, 2, 6], [0, 0, 0, 2]]))
+        array_compare(
+            a, np.array([[2, 0, 0, 2], [0, 2, 0, 4], [0, 0, 2, 6], [0, 0, 0, 2]])
+        )
 
         a = T + 1
         self.assertNotIsInstance(a, SE3)
-        array_compare(a, np.array([[2, 1, 1, 2], [1, 2, 1, 3], [1, 1, 2, 4], [1, 1, 1, 2]]))
+        array_compare(
+            a, np.array([[2, 1, 1, 2], [1, 2, 1, 3], [1, 1, 2, 4], [1, 1, 1, 2]])
+        )
 
         # a = 1 + T
         # self.assertNotIsInstance(a, SE3)
         # array_compare(a, np.array([ [2,1,1], [1,2,1], [1,1,2]]))
 
         a = T + np.eye(4)
         self.assertNotIsInstance(a, SE3)
-        array_compare(a, np.array([[2, 0, 0, 1], [0, 2, 0, 2], [0, 0, 2, 3], [0, 0, 0, 2]]))
+        array_compare(
+            a, np.array([[2, 0, 0, 1], [0, 2, 0, 2], [0, 0, 2, 3], [0, 0, 0, 2]])
+        )
 
         # a =  np.eye(3) + T
         # self.assertNotIsInstance(a, SE3)
         # array_compare(a, np.array([ [2,0,0], [0,2,0], [0,0,2]]))
         #  this invokes the __add__ method for numpy
 
         # difference
@@ -894,23 +958,28 @@
 
         a = T - T
         self.assertNotIsInstance(a, SE3)
         array_compare(a, np.zeros((4, 4)))
 
         a = T - 1
         self.assertNotIsInstance(a, SE3)
-        array_compare(a, np.array([[0, -1, -1, 0], [-1, 0, -1, 1], [-1, -1, 0, 2], [-1, -1, -1, 0]]))
+        array_compare(
+            a,
+            np.array([[0, -1, -1, 0], [-1, 0, -1, 1], [-1, -1, 0, 2], [-1, -1, -1, 0]]),
+        )
 
         # a = 1 - T
         # self.assertNotIsInstance(a, SE3)
         # array_compare(a, -np.array([ [0,-1,-1], [-1,0,-1], [-1,-1,0]]))
 
         a = T - np.eye(4)
         self.assertNotIsInstance(a, SE3)
-        array_compare(a, np.array([[0, 0, 0, 1], [0, 0, 0, 2], [0, 0, 0, 3], [0, 0, 0, 0]]))
+        array_compare(
+            a, np.array([[0, 0, 0, 1], [0, 0, 0, 2], [0, 0, 0, 3], [0, 0, 0, 0]])
+        )
 
         # a =  np.eye(3) - T
         # self.assertNotIsInstance(a, SE3)
         # array_compare(a, np.zeros((3,3)))
 
         a = T
         a -= T
@@ -931,15 +1000,17 @@
         a = 2 * T
         self.assertNotIsInstance(a, SE3)
         array_compare(a, 2 * transl(1, 2, 3))
 
         T = SE3(1, 2, 3)
         T *= SE3.Ry(pi / 2)
         self.assertIsInstance(T, SE3)
-        array_compare(T, np.array([[0, 0, 1, 1], [0, 1, 0, 2], [-1, 0, 0, 3], [0, 0, 0, 1]]))
+        array_compare(
+            T, np.array([[0, 0, 1, 1], [0, 1, 0, 2], [-1, 0, 0, 3], [0, 0, 0, 1]])
+        )
 
         T = SE3()
         T *= 2
         self.assertNotIsInstance(T, SE3)
         array_compare(T, 2 * np.eye(4))
 
         array_compare(SE3.Rx(pi / 2) * SE3.Ry(pi / 2) * SE3.Rx(-pi / 2), SE3.Rz(pi / 2))
@@ -974,15 +1045,14 @@
         array_compare(a, np.eye(4))
 
         a = T / 2
         self.assertNotIsInstance(a, SE3)
         array_compare(a, troty(0.3) / 2)
 
     def test_arith_vect(self):
-
         rx = SE3.Rx(pi / 2)
         ry = SE3.Ry(pi / 2)
         rz = SE3.Rz(pi / 2)
         u = SE3()
 
         # multiply
         T = SE3([rx, ry, rz])
@@ -1186,22 +1256,21 @@
         a = T - 1
         self.assertNotIsInstance(a, SE3)
         nt.assert_equal(len(a), 3)
         array_compare(a[0], rx - 1)
         array_compare(a[1], ry - 1)
         array_compare(a[2], rz - 1)
 
-
     def test_functions(self):
         # inv
         # .T
         pass
 
     def test_functions_vect(self):
         # inv
         # .T
         pass
 
+
 # ---------------------------------------------------------------------------------------#
-if __name__ == '__main__':
-    
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `spatialmath-python-1.1.8/tests/test_quaternion.py` & `spatialmath-python-1.1.9/tests/test_quaternion.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,27 @@
         # nt.assert_array_almost_equal(UnitQuaternion(R).R, R)
         # nt.assert_array_almost_equal(UnitQuaternion(T).T, T)
 
         # copy constructor
         q = UnitQuaternion(rotx(0.3))
         qcompare(UnitQuaternion(q), q)
 
+        # fail when invalid arrays are provided
+        # invalid rotation matrix
+        R = 1.1 * np.eye(3)
+        with self.assertRaises(ValueError):
+            UnitQuaternion(R, check=True)
+
+        # wrong shape to be anything
+        R = np.zeros((5, 5))
+        with self.assertRaises(ValueError):
+            UnitQuaternion(R, check=True)
+        with self.assertRaises(ValueError):
+            UnitQuaternion(R, check=False)
+
     def test_concat(self):
         u = UnitQuaternion()
         uu = UnitQuaternion([u, u, u, u])
 
         self.assertIsInstance(uu, UnitQuaternion)
         self.assertEqual(len(uu), 4)
 
@@ -480,16 +493,24 @@
         qcompare(
             ry / UnitQuaternion([rx, ry, rz]),
             UnitQuaternion([ry / rx, ry / ry, ry / rz]),
         )
 
     def test_angle(self):
         # angle between quaternions
-        # pure
-        v = [5, 6, 7]
+        uq1 = UnitQuaternion.Rx(0.1)
+        uq2 = UnitQuaternion.Ry(0.1)
+        for metric in range(5):
+            self.assertEqual(uq1.angdist(other=uq1, metric=metric), 0.0)
+            self.assertEqual(uq2.angdist(other=uq2, metric=metric), 0.0)
+            self.assertEqual(
+                uq1.angdist(other=uq2, metric=metric),
+                uq2.angdist(other=uq1, metric=metric),
+            )
+            self.assertTrue(uq1.angdist(other=uq2, metric=metric) > 0)
 
     def test_conversions(self):
         # , 3 angle
         qcompare(UnitQuaternion.RPY([0.1, 0.2, 0.3]).rpy(), [0.1, 0.2, 0.3])
         qcompare(UnitQuaternion.RPY(0.1, 0.2, 0.3).rpy(), [0.1, 0.2, 0.3])
 
         qcompare(UnitQuaternion.Eul([0.1, 0.2, 0.3]).eul(), [0.1, 0.2, 0.3])
@@ -776,16 +797,23 @@
     def log_test_exp(self):
         q1 = Quaternion([4, 3, 2, 1])
         q2 = Quaternion([-1, 2, -3, 4])
 
         nt.assert_array_almost_equal(exp(log(q1)), q1)
         nt.assert_array_almost_equal(exp(log(q2)), q2)
 
-        # nt.assert_array_almost_equal(log(exp(q1)), q1)
-        # nt.assert_array_almost_equal(log(exp(q2)), q2)
+    def test_log(self):
+        q1 = Quaternion([4, 3, 2, 1])
+        q2 = Quaternion([-1, 2, -3, 4])
+
+        self.assertTrue(isscalar(q1.log().s))
+        self.assertTrue(isvector(q1.log().v, 3))
+
+        nt.assert_array_almost_equal(q1.log().exp(), q1)
+        nt.assert_array_almost_equal(q2.log().exp(), q2)
 
     def test_concat(self):
         u = Quaternion()
         uu = Quaternion([u, u, u, u])
 
         self.assertIsInstance(uu, Quaternion)
         self.assertEqual(len(uu), 4)
```

### Comparing `spatialmath-python-1.1.8/tests/test_spatialvector.py` & `spatialmath-python-1.1.9/tests/test_spatialvector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import unittest
 import numpy.testing as nt
 import numpy as np
 
 from spatialmath.spatialvector import *
 
 
@@ -51,34 +50,34 @@
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialM6)
         self.assertEqual(len(a), 1)
         self.assertTrue(all(a.A == np.r_[1, 2, 3, 4, 5, 6]))
 
         s = str(a)
         self.assertIsInstance(s, str)
-        self.assertEqual(s.count('\n'), 0)
-        self.assertTrue(s.startswith('SpatialVelocity'))
+        self.assertEqual(s.count("\n"), 0)
+        self.assertTrue(s.startswith("SpatialVelocity"))
 
         r = np.random.rand(6, 10)
         a = SpatialVelocity(r)
         self.assertIsInstance(a, SpatialVelocity)
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialM6)
         self.assertEqual(len(a), 10)
 
         b = a[3]
         self.assertIsInstance(b, SpatialVelocity)
         self.assertIsInstance(b, SpatialVector)
         self.assertIsInstance(b, SpatialM6)
         self.assertEqual(len(b), 1)
-        self.assertTrue(all(b.A == r[:,3]))
+        self.assertTrue(all(b.A == r[:, 3]))
 
         s = str(a)
         self.assertIsInstance(s, str)
-        self.assertEqual(s.count('\n'), 9)
+        self.assertEqual(s.count("\n"), 9)
 
     def test_acceleration(self):
         a = SpatialAcceleration([1, 2, 3, 4, 5, 6])
         self.assertIsInstance(a, SpatialAcceleration)
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialM6)
         self.assertEqual(len(a), 1)
@@ -89,37 +88,35 @@
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialM6)
         self.assertEqual(len(a), 1)
         self.assertTrue(all(a.A == np.r_[1, 2, 3, 4, 5, 6]))
 
         s = str(a)
         self.assertIsInstance(s, str)
-        self.assertEqual(s.count('\n'), 0)
-        self.assertTrue(s.startswith('SpatialAcceleration'))
+        self.assertEqual(s.count("\n"), 0)
+        self.assertTrue(s.startswith("SpatialAcceleration"))
 
         r = np.random.rand(6, 10)
         a = SpatialAcceleration(r)
         self.assertIsInstance(a, SpatialAcceleration)
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialM6)
         self.assertEqual(len(a), 10)
 
         b = a[3]
         self.assertIsInstance(b, SpatialAcceleration)
         self.assertIsInstance(b, SpatialVector)
         self.assertIsInstance(b, SpatialM6)
         self.assertEqual(len(b), 1)
-        self.assertTrue(all(b.A == r[:,3]))
+        self.assertTrue(all(b.A == r[:, 3]))
 
         s = str(a)
         self.assertIsInstance(s, str)
 
-
     def test_force(self):
-
         a = SpatialForce([1, 2, 3, 4, 5, 6])
         self.assertIsInstance(a, SpatialForce)
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialF6)
         self.assertEqual(len(a), 1)
         self.assertTrue(all(a.A == np.r_[1, 2, 3, 4, 5, 6]))
 
@@ -128,16 +125,16 @@
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialF6)
         self.assertEqual(len(a), 1)
         self.assertTrue(all(a.A == np.r_[1, 2, 3, 4, 5, 6]))
 
         s = str(a)
         self.assertIsInstance(s, str)
-        self.assertEqual(s.count('\n'), 0)
-        self.assertTrue(s.startswith('SpatialForce'))
+        self.assertEqual(s.count("\n"), 0)
+        self.assertTrue(s.startswith("SpatialForce"))
 
         r = np.random.rand(6, 10)
         a = SpatialForce(r)
         self.assertIsInstance(a, SpatialForce)
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialF6)
         self.assertEqual(len(a), 10)
@@ -149,15 +146,14 @@
         self.assertEqual(len(b), 1)
         self.assertTrue(all(b.A == r[:, 3]))
 
         s = str(a)
         self.assertIsInstance(s, str)
 
     def test_momentum(self):
-
         a = SpatialMomentum([1, 2, 3, 4, 5, 6])
         self.assertIsInstance(a, SpatialMomentum)
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialF6)
         self.assertEqual(len(a), 1)
         self.assertTrue(all(a.A == np.r_[1, 2, 3, 4, 5, 6]))
 
@@ -166,16 +162,16 @@
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialF6)
         self.assertEqual(len(a), 1)
         self.assertTrue(all(a.A == np.r_[1, 2, 3, 4, 5, 6]))
 
         s = str(a)
         self.assertIsInstance(s, str)
-        self.assertEqual(s.count('\n'), 0)
-        self.assertTrue(s.startswith('SpatialMomentum'))
+        self.assertEqual(s.count("\n"), 0)
+        self.assertTrue(s.startswith("SpatialMomentum"))
 
         r = np.random.rand(6, 10)
         a = SpatialMomentum(r)
         self.assertIsInstance(a, SpatialMomentum)
         self.assertIsInstance(a, SpatialVector)
         self.assertIsInstance(a, SpatialF6)
         self.assertEqual(len(a), 10)
@@ -186,38 +182,53 @@
         self.assertIsInstance(b, SpatialF6)
         self.assertEqual(len(b), 1)
         self.assertTrue(all(b.A == r[:, 3]))
 
         s = str(a)
         self.assertIsInstance(s, str)
 
-
     def test_arith(self):
-
         # just test SpatialVelocity since all types derive from same superclass
 
         r1 = np.r_[1, 2, 3, 4, 5, 6]
         r2 = np.r_[7, 8, 9, 10, 11, 12]
         a1 = SpatialVelocity(r1)
         a2 = SpatialVelocity(r2)
 
         self.assertTrue(all((a1 + a2).A == r1 + r2))
         self.assertTrue(all((a1 - a2).A == r1 - r2))
         self.assertTrue(all((-a1).A == -r1))
 
     def test_inertia(self):
         # constructor
+        i0 = SpatialInertia()
+        nt.assert_equal(i0.A, np.zeros((6, 6)))
+
+        i1 = SpatialInertia(np.eye(6, 6))
+        nt.assert_equal(i1.A, np.eye(6, 6))
+
+        i2 = SpatialInertia(m=1, r=(1, 2, 3))
+        nt.assert_almost_equal(i2.A, i2.A.T)
+
+        i3 = SpatialInertia(m=1, r=(1, 2, 3), I=np.ones((3, 3)))
+        nt.assert_almost_equal(i3.A, i3.A.T)
+
         # addition
-        pass
+        m_a, m_b = 1.1, 2.2
+        r = (1, 2, 3)
+        i4a, i4b = SpatialInertia(m=m_a, r=r), SpatialInertia(m=m_b, r=r)
+        nt.assert_almost_equal((i4a + i4b).A, SpatialInertia(m=m_a + m_b, r=r).A)
+
+        # isvalid - note this method is very barebone, to be improved
+        self.assertTrue(SpatialInertia().isvalid(np.ones((6, 6)), check=False))
 
     def test_products(self):
         # v x v = a  *, v x F6 = a
         # a x I, I x a
         # v x I, I x v
         # twist x v, twist x a, twist x F
         pass
 
 
 # ---------------------------------------------------------------------------------------#
-if __name__ == '__main__':
-
-    unittest.main()
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `spatialmath-python-1.1.8/tests/test_twist.py` & `spatialmath-python-1.1.9/tests/test_twist.py`

 * *Files identical despite different names*

