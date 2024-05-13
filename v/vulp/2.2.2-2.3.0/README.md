# Comparing `tmp/vulp-2.2.2.tar.gz` & `tmp/vulp-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulp-2.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vulp-2.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vulp-2.2.2.tar` & `vulp-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5422 2024-03-28 14:00:52.986919 vulp-2.2.2/CHANGELOG.md
--rw-r--r--   0        0        0      500 2024-01-04 16:25:56.440796 vulp-2.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-23 17:15:51.186624 vulp-2.2.2/LICENSE
--rw-r--r--   0        0        0    11533 2024-03-28 13:56:45.925657 vulp-2.2.2/README.md
--rw-r--r--   0        0        0     1590 2024-03-01 14:28:18.653450 vulp-2.2.2/pyproject.toml
--rw-r--r--   0        0        0      177 2024-03-28 14:00:42.999030 vulp-2.2.2/vulp/__init__.py
--rw-r--r--   0        0        0      441 2024-03-25 13:55:49.543349 vulp-2.2.2/vulp/spine/__init__.py
--rw-r--r--   0        0        0      515 2024-03-25 13:55:49.543349 vulp-2.2.2/vulp/spine/exceptions.py
--rw-r--r--   0        0        0      503 2024-03-25 13:55:49.543349 vulp-2.2.2/vulp/spine/request.py
--rw-r--r--   0        0        0     7186 2024-03-25 13:55:49.543349 vulp-2.2.2/vulp/spine/spine_interface.py
--rw-r--r--   0        0        0      168 2024-03-25 13:55:49.543349 vulp-2.2.2/vulp/utils/__init__.py
--rw-r--r--   0        0        0      931 2024-03-25 13:55:49.543349 vulp-2.2.2/vulp/utils/serialize.py
--rw-r--r--   0        0        0    12746 1970-01-01 00:00:00.000000 vulp-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6572 2024-05-02 16:31:59.443919 vulp-2.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      487 2024-05-02 12:21:06.231800 vulp-2.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-23 17:15:51.186624 vulp-2.3.0/LICENSE
+-rw-r--r--   0        0        0    11497 2024-05-02 12:21:06.231800 vulp-2.3.0/README.md
+-rw-r--r--   0        0        0     1590 2024-03-01 14:28:18.653450 vulp-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      177 2024-05-02 16:04:11.013221 vulp-2.3.0/vulp/__init__.py
+-rw-r--r--   0        0        0      441 2024-03-25 13:55:49.543349 vulp-2.3.0/vulp/spine/__init__.py
+-rw-r--r--   0        0        0      515 2024-03-25 13:55:49.543349 vulp-2.3.0/vulp/spine/exceptions.py
+-rw-r--r--   0        0        0      503 2024-03-25 13:55:49.543349 vulp-2.3.0/vulp/spine/request.py
+-rw-r--r--   0        0        0     7285 2024-05-02 16:04:28.409041 vulp-2.3.0/vulp/spine/spine_interface.py
+-rw-r--r--   0        0        0      168 2024-03-25 13:55:49.543349 vulp-2.3.0/vulp/utils/__init__.py
+-rw-r--r--   0        0        0      931 2024-03-25 13:55:49.543349 vulp-2.3.0/vulp/utils/serialize.py
+-rw-r--r--   0        0        0    12710 1970-01-01 00:00:00.000000 vulp-2.3.0/PKG-INFO
```

### Comparing `vulp-2.2.2/CHANGELOG.md` & `vulp-2.3.0/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,45 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 ## [Unreleased]
 
+## [2.3.0] - 2024-05-02
+
+### Added
+
+- Build test for the pi3hat interface
+- BulletInterface: internal ``get_link_index`` memoization
+- BulletInterface: introduce "monitor" configuration dictionary
+- BulletInterface: report contacts to bodies specified in configuration
+- CICD: Add a workflow for the pi3hat build test
+- Introduce ``observe`` method in actuation interfaces
+
+### Changed
+
+- CICD: Rename bazel.yml to ci.yml for consistency with other repos
+- Pi3HatInterface: make ``get_angular_velocity`` private
+- Pi3HatInterface: make ``get_attitude`` private
+- Pi3HatInterface: make ``get_linear_acceleration`` private
+- Pi3HatInterface: make ``imu_data`` private
+
+### Fixed
+
+- CICD: Clean up redundant Python build jobs
+- SpineInterface: Remove leading slashes from shared memory object names
+
+### Removed
+
+- Clean up unused ``MockInterface::get_angular_velocity``
+- Clean up unused ``MockInterface::get_attitude``
+- Clean up unused ``MockInterface::get_linear_acceleration``
+- Remove ``imu_data`` getter from actuation interfaces
+- Remove ``observe_imu`` function from observations
+
 ## [2.2.2] - 2024-03-28
 
 ### Added
 
 - BulletInterface: Set a default servo temperature of 20 °C
 - BulletInterface: Set a default servo voltage of 18 V
 
@@ -179,15 +211,16 @@
 - Clean up empty observation and observers directories
 - Fix calls to mpacklog logger functions
 
 ## [1.0.0] - 2022-06-10
 
 First release of the project.
 
-[unreleased]: https://github.com/upkie/vulp/compare/v2.2.2...HEAD
+[unreleased]: https://github.com/upkie/vulp/compare/v2.3.0...HEAD
+[2.3.0]: https://github.com/upkie/vulp/compare/v2.2.2...v2.3.0
 [2.2.2]: https://github.com/upkie/vulp/compare/v2.2.1...v2.2.2
 [2.2.1]: https://github.com/upkie/vulp/compare/v2.2.0...v2.2.1
 [2.2.0]: https://github.com/upkie/vulp/compare/v2.1.0...v2.2.0
 [2.1.0]: https://github.com/upkie/vulp/compare/v2.0.0...v2.1.0
 [2.0.0]: https://github.com/upkie/vulp/compare/v1.5.0...v2.0.0
 [1.5.0]: https://github.com/upkie/vulp/compare/v1.4.0...v1.5.0
 [1.4.0]: https://github.com/upkie/vulp/compare/v1.3.0...v1.4.0
```

### Comparing `vulp-2.2.2/LICENSE` & `vulp-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulp-2.2.2/README.md` & `vulp-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Vulp – Robot/simulation switch
 
-[![CI](https://github.com/upkie/vulp/actions/workflows/bazel.yml/badge.svg)](https://github.com/upkie/vulp/actions/workflows/bazel.yml)
-[![Documentation](https://img.shields.io/github/actions/workflow/status/upkie/vulp/docs.yml?branch=main&label=docs)](https://upkie.github.io/vulp/)
+[![CI](https://github.com/upkie/vulp/actions/workflows/ci.yml/badge.svg)](https://github.com/upkie/vulp/actions/workflows/ci.yml)
+[![Documentation](https://github.com/upkie/vulp/actions/workflows/docs.yml/badge.svg)](https://upkie.github.io/vulp/)
 [![Coverage](https://coveralls.io/repos/github/upkie/vulp/badge.svg?branch=main)](https://coveralls.io/github/upkie/vulp?branch=main)
 ![C++ version](https://img.shields.io/badge/C++-17-blue.svg?style=flat)
 [![Conda version](https://anaconda.org/conda-forge/vulp/badges/version.svg)](https://anaconda.org/conda-forge/vulp)
 [![PyPI version](https://img.shields.io/pypi/v/vulp)](https://pypi.org/project/vulp/)
 
 Vulp provides an action-observation loop to control robots from a standalone "agent" process, like this:
```

### Comparing `vulp-2.2.2/pyproject.toml` & `vulp-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vulp-2.2.2/vulp/spine/exceptions.py` & `vulp-2.3.0/vulp/spine/exceptions.py`

 * *Files identical despite different names*

### Comparing `vulp-2.2.2/vulp/spine/spine_interface.py` & `vulp-2.3.0/vulp/spine/spine_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     Connect to the spine shared memory.
 
     @param shm_name Name of the shared memory object.
     @param retries Number of times to try opening the shared-memory file.
     @raise SpineError If the spine did not respond after the prescribed number
         of trials.
     """
+    # Remove leading slash if present, as SharedMemory will prepend it
+    # See https://github.com/upkie/vulp/issues/92
+    shm_name = shm_name.lstrip("/")
+
     for trial in range(retries):
         if trial > 0:
             logging.info(
                 f"Waiting for spine {shm_name} to start "
                 f"(trial {trial} / {retries})..."
             )
             time.sleep(1.0)
@@ -189,15 +193,14 @@
             # perf_counter_ns clocks ~1 us on the raspi
             if perf_counter_ns() > stop:
                 raise TimeoutError(
                     "Spine did not process request within "
                     f"{timeout_ns / 1e6:.1f} ms, is it stopped?"
                 )
         if self._read_request() == Request.kError:
-            # TODO(scaron): cover this case by a unit test
             self._write_request(Request.kNone)
             raise SpineError("Invalid request, is the spine started?")
 
     def _write_request(self, request: int) -> None:
         """!
         Set request in shared memory.
         """
```

### Comparing `vulp-2.2.2/vulp/utils/serialize.py` & `vulp-2.3.0/vulp/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `vulp-2.2.2/PKG-INFO` & `vulp-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulp
-Version: 2.2.2
+Version: 2.3.0
 Summary: Real-time motion control for Python.
 Keywords: motion control,real time,robotics
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,16 +23,16 @@
 Project-URL: Changelog, https://github.com/upkie/vulp/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://upkie.github.io/vulp/
 Project-URL: Source, https://github.com/upkie/vulp
 Project-URL: Tracker, https://github.com/upkie/vulp/issues
 
 # Vulp – Robot/simulation switch
 
-[![CI](https://github.com/upkie/vulp/actions/workflows/bazel.yml/badge.svg)](https://github.com/upkie/vulp/actions/workflows/bazel.yml)
-[![Documentation](https://img.shields.io/github/actions/workflow/status/upkie/vulp/docs.yml?branch=main&label=docs)](https://upkie.github.io/vulp/)
+[![CI](https://github.com/upkie/vulp/actions/workflows/ci.yml/badge.svg)](https://github.com/upkie/vulp/actions/workflows/ci.yml)
+[![Documentation](https://github.com/upkie/vulp/actions/workflows/docs.yml/badge.svg)](https://upkie.github.io/vulp/)
 [![Coverage](https://coveralls.io/repos/github/upkie/vulp/badge.svg?branch=main)](https://coveralls.io/github/upkie/vulp?branch=main)
 ![C++ version](https://img.shields.io/badge/C++-17-blue.svg?style=flat)
 [![Conda version](https://anaconda.org/conda-forge/vulp/badges/version.svg)](https://anaconda.org/conda-forge/vulp)
 [![PyPI version](https://img.shields.io/pypi/v/vulp)](https://pypi.org/project/vulp/)
 
 Vulp provides an action-observation loop to control robots from a standalone "agent" process, like this:
```

