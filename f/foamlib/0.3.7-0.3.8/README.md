# Comparing `tmp/foamlib-0.3.7.tar.gz` & `tmp/foamlib-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.3.7.tar", last modified: Mon Apr 22 13:21:08 2024, max compression
+gzip compressed data, was "foamlib-0.3.8.tar", last modified: Mon May 13 16:43:48 2024, max compression
```

## Comparing `foamlib-0.3.7.tar` & `foamlib-0.3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:21:08.228658 foamlib-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-22 13:20:59.000000 foamlib-0.3.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-22 13:21:08.228658 foamlib-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-22 13:20:59.000000 foamlib-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:21:08.224658 foamlib-0.3.7/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:21:08.224658 foamlib-0.3.7/foamlib/_files/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/_files/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/_files/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/_files/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/_files/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/_files/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:20:59.000000 foamlib-0.3.7/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:21:08.224658 foamlib-0.3.7/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-22 13:21:08.000000 foamlib-0.3.7/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 13:21:08.000000 foamlib-0.3.7/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:21:08.000000 foamlib-0.3.7/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-22 13:21:08.000000 foamlib-0.3.7/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 13:21:08.000000 foamlib-0.3.7/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-22 13:20:59.000000 foamlib-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:21:08.228658 foamlib-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:48.977108 foamlib-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-05-13 16:43:41.000000 foamlib-0.3.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-13 16:43:48.977108 foamlib-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-13 16:43:41.000000 foamlib-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:48.973108 foamlib-0.3.8/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21142 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:48.973108 foamlib-0.3.8/foamlib/_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_files/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:41.000000 foamlib-0.3.8/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:43:48.973108 foamlib-0.3.8/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 16:43:48.000000 foamlib-0.3.8/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-13 16:43:41.000000 foamlib-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:43:48.977108 foamlib-0.3.8/setup.cfg
```

### Comparing `foamlib-0.3.7/LICENSE.txt` & `foamlib-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.7/PKG-INFO` & `foamlib-0.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -41,24 +41,25 @@
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: numpy<2,>=1; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx<8,>=7; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: numpy<2,>=1; extra == "docs"
 
-# foamlib
+[<img alt="foamlib" src="https://github.com/gerlero/foamlib/raw/main/logo.png" height="50">](https://github.com/gerlero/foamlib)
 
 [![Documentation](https://img.shields.io/readthedocs/foamlib)](https://foamlib.readthedocs.io/)
 [![CI](https://github.com/gerlero/foamlib/actions/workflows/ci.yml/badge.svg)](https://github.com/gerlero/foamlib/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/gerlero/foamlib/branch/main/graph/badge.svg)](https://codecov.io/gh/gerlero/foamlib)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/foamlib)](https://pypi.org/project/foamlib/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/foamlib)](https://pypi.org/project/foamlib/)
-[![Docker image](https://img.shields.io/badge/docker%20image-gerlero%2Ffoamlib-informational)](https://hub.docker.com/r/gerlero/foamlib/)
+![OpenFOAM](https://img.shields.io/badge/openfoam-.com%20|%20.org-informational)
+[![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Ffoamlib-0085a0)](https://hub.docker.com/r/microfluidica/foamlib/)
 
 **foamlib** provides a simple, modern and ergonomic Python interface for interacting with [OpenFOAM](https://www.openfoam.com).
 
 It offers the following classes:
 
 * [`FoamFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFile) (and [`FoamFieldFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFieldFile)): read-write access to OpenFOAM configuration and field files as if they were Python `dict`s, using `foamlib`'s own parser. Supports both ASCII and binary field formats.
 * [`FoamCase`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamCase): a class for manipulating, executing and accessing the results of OpenFOAM cases.
```

### Comparing `foamlib-0.3.7/README.md` & `foamlib-0.3.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# foamlib
+[<img alt="foamlib" src="https://github.com/gerlero/foamlib/raw/main/logo.png" height="50">](https://github.com/gerlero/foamlib)
 
 [![Documentation](https://img.shields.io/readthedocs/foamlib)](https://foamlib.readthedocs.io/)
 [![CI](https://github.com/gerlero/foamlib/actions/workflows/ci.yml/badge.svg)](https://github.com/gerlero/foamlib/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/gerlero/foamlib/branch/main/graph/badge.svg)](https://codecov.io/gh/gerlero/foamlib)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/foamlib)](https://pypi.org/project/foamlib/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/foamlib)](https://pypi.org/project/foamlib/)
-[![Docker image](https://img.shields.io/badge/docker%20image-gerlero%2Ffoamlib-informational)](https://hub.docker.com/r/gerlero/foamlib/)
+![OpenFOAM](https://img.shields.io/badge/openfoam-.com%20|%20.org-informational)
+[![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Ffoamlib-0085a0)](https://hub.docker.com/r/microfluidica/foamlib/)
 
 **foamlib** provides a simple, modern and ergonomic Python interface for interacting with [OpenFOAM](https://www.openfoam.com).
 
 It offers the following classes:
 
 * [`FoamFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFile) (and [`FoamFieldFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFieldFile)): read-write access to OpenFOAM configuration and field files as if they were Python `dict`s, using `foamlib`'s own parser. Supports both ASCII and binary field formats.
 * [`FoamCase`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamCase): a class for manipulating, executing and accessing the results of OpenFOAM cases.
```

### Comparing `foamlib-0.3.7/foamlib/_cases.py` & `foamlib-0.3.8/foamlib/_cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,30 +28,26 @@
 from ._files import FoamFieldFile, FoamFile
 from ._util import is_sequence, run_process, run_process_async
 
 
 class FoamCaseBase(Sequence["FoamCaseBase.TimeDirectory"]):
     def __init__(self, path: Union[Path, str] = Path()):
         self.path = Path(path).absolute()
-        if not self.path.is_dir():
-            raise NotADirectoryError(f"{self.path} is not a directory")
 
     class TimeDirectory(Set[FoamFieldFile]):
         """
         An OpenFOAM time directory in a case.
 
         Use to access field files in the directory, e.g. `time["U"]`.
 
         :param path: The path to the time directory.
         """
 
         def __init__(self, path: Union[Path, str]):
             self.path = Path(path).absolute()
-            if not self.path.is_dir():
-                raise NotADirectoryError(f"{self.path} is not a directory")
 
         @property
         def time(self) -> float:
             """The time that corresponds to this directory."""
             return float(self.path.name)
 
         @property
@@ -144,17 +140,23 @@
                 else:
                     if t != 0:
                         paths.add(p)
 
                 if has_decompose_par_dict and p.name.startswith("processor"):
                     paths.add(p)
 
+        if (self.path / "0.orig").is_dir() and (self.path / "0").is_dir():
+            paths.add(self.path / "0")
+
         if has_block_mesh_dict and (self.path / "constant" / "polyMesh").exists():
             paths.add(self.path / "constant" / "polyMesh")
 
+        if self._run_script() is not None:
+            paths.update(self.path.glob("log.*"))
+
         return paths
 
     def _clone_ignore(
         self,
     ) -> Callable[[Union[Path, str], Collection[str]], Collection[str]]:
         clean_paths = self._clean_paths()
 
@@ -172,15 +174,15 @@
         if clean.is_file():
             return clean
         elif all_clean.is_file():
             return all_clean
         else:
             return None
 
-    def _run_script(self, *, parallel: Optional[bool]) -> Optional[Path]:
+    def _run_script(self, *, parallel: Optional[bool] = None) -> Optional[Path]:
         """Return the path to the (All)run script, or None if no run script is found."""
         run = self.path / "run"
         run_parallel = self.path / "run-parallel"
         all_run = self.path / "Allrun"
         all_run_parallel = self.path / "Allrun-parallel"
 
         if run.is_file() or all_run.is_file():
@@ -321,15 +323,18 @@
         """
         script_path = self._clean_script() if script else None
 
         if script_path is not None:
             self.run([script_path], check=check)
         else:
             for p in self._clean_paths():
-                shutil.rmtree(p)
+                if p.is_dir():
+                    shutil.rmtree(p)
+                else:
+                    p.unlink()
 
     def run(
         self,
         cmd: Optional[Union[Sequence[Union[str, Path]], str, Path]] = None,
         *,
         script: bool = True,
         parallel: Optional[bool] = None,
@@ -355,14 +360,17 @@
         else:
             script_path = self._run_script(parallel=parallel) if script else None
 
             if script_path is not None:
                 return self.run([script_path], check=check)
 
             else:
+                if not self and (self.path / "0.orig").is_dir():
+                    self.restore_0_dir()
+
                 if (self.path / "system" / "blockMeshDict").is_file():
                     self.block_mesh()
 
                 if parallel is None:
                     parallel = (
                         self._nprocessors > 0
                         or (self.path / "system" / "decomposeParDict").is_file()
@@ -389,14 +397,19 @@
         """Decompose this case for parallel running."""
         self.run(["decomposePar"], check=check)
 
     def reconstruct_par(self, *, check: bool = True) -> None:
         """Reconstruct this case after parallel running."""
         self.run(["reconstructPar"], check=check)
 
+    def restore_0_dir(self) -> None:
+        """Restore the 0 directory from the 0.orig directory."""
+        shutil.rmtree(self.path / "0", ignore_errors=True)
+        shutil.copytree(self.path / "0.orig", self.path / "0")
+
     def copy(self, dest: Union[Path, str]) -> "FoamCase":
         """
         Make a copy of this case.
 
         :param dest: The destination path.
         """
         return FoamCase(shutil.copytree(self.path, dest, symlinks=True))
@@ -474,15 +487,18 @@
         """
         script_path = self._clean_script() if script else None
 
         if script_path is not None:
             await self.run([script_path], check=check)
         else:
             for p in self._clean_paths():
-                await aioshutil.rmtree(p)
+                if p.is_dir():
+                    await aioshutil.rmtree(p)
+                else:
+                    p.unlink()
 
     async def run(
         self,
         cmd: Optional[Union[Sequence[Union[str, Path]], str, Path]] = None,
         *,
         script: bool = True,
         parallel: Optional[bool] = None,
@@ -527,14 +543,17 @@
                             cpus = nsubdomains
                         else:
                             cpus = 1
 
                 await self.run([script_path], check=check, cpus=cpus)
 
             else:
+                if not self and (self.path / "0.orig").is_dir():
+                    await self.restore_0_dir()
+
                 if (self.path / "system" / "blockMeshDict").is_file():
                     await self.block_mesh()
 
                 if parallel is None:
                     parallel = (
                         self._nprocessors > 0
                         or (self.path / "system" / "decomposeParDict").is_file()
@@ -568,14 +587,19 @@
         """Decompose this case for parallel running."""
         await self.run(["decomposePar"], check=check)
 
     async def reconstruct_par(self, *, check: bool = True) -> None:
         """Reconstruct this case after parallel running."""
         await self.run(["reconstructPar"], check=check)
 
+    async def restore_0_dir(self) -> None:
+        """Restore the 0 directory from the 0.orig directory."""
+        await aioshutil.rmtree(self.path / "0", ignore_errors=True)
+        await aioshutil.copytree(self.path / "0.orig", self.path / "0")
+
     async def copy(self, dest: Union[Path, str]) -> "AsyncFoamCase":
         """
         Make a copy of this case.
 
         :param dest: The destination path.
         """
         return AsyncFoamCase(await aioshutil.copytree(self.path, dest, symlinks=True))
```

### Comparing `foamlib-0.3.7/foamlib/_files/_base.py` & `foamlib-0.3.8/foamlib/_files/_base.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.7/foamlib/_files/_files.py` & `foamlib-0.3.8/foamlib/_files/_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         _, parsed = self._read()
 
         value = parsed[keywords]
 
         if value is ...:
             return FoamFile.SubDict(self, keywords)
         else:
-            return value  # type: ignore [return-value]
+            return value
 
     @property
     def _binary(self) -> bool:
         return self.get(("FoamFile", "format"), None) == "binary"
 
     def __setitem__(
         self,
```

### Comparing `foamlib-0.3.7/foamlib/_files/_io.py` & `foamlib-0.3.8/foamlib/_files/_io.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 
 from ._parsing import Parsed
 
 
 class FoamFileIO:
     def __init__(self, path: Union[str, Path]) -> None:
         self.path = Path(path).absolute()
-        if self.path.is_dir():
-            raise IsADirectoryError(self.path)
-        elif not self.path.is_file():
-            raise FileNotFoundError(self.path)
 
         self.__contents: Optional[bytes] = None
         self.__parsed: Optional[Parsed] = None
         self.__defer_io = 0
         self.__dirty = False
 
     def __enter__(self) -> Self:
```

### Comparing `foamlib-0.3.7/foamlib/_files/_parsing.py` & `foamlib-0.3.8/foamlib/_files/_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,10 +243,10 @@
             for k in keywords[:-1]:
                 assert isinstance(r, dict)
                 v = r[k]
                 assert isinstance(v, dict)
                 r = v
 
             assert isinstance(r, dict)
-            r[keywords[-1]] = {} if data is ... else data  # type: ignore [assignment]
+            r[keywords[-1]] = {} if data is ... else data
 
         return ret
```

### Comparing `foamlib-0.3.7/foamlib/_files/_serialization.py` & `foamlib-0.3.8/foamlib/_files/_serialization.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.7/foamlib/_util.py` & `foamlib-0.3.8/foamlib/_util.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.7/foamlib.egg-info/PKG-INFO` & `foamlib-0.3.8/foamlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -41,24 +41,25 @@
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: numpy<2,>=1; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx<8,>=7; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: numpy<2,>=1; extra == "docs"
 
-# foamlib
+[<img alt="foamlib" src="https://github.com/gerlero/foamlib/raw/main/logo.png" height="50">](https://github.com/gerlero/foamlib)
 
 [![Documentation](https://img.shields.io/readthedocs/foamlib)](https://foamlib.readthedocs.io/)
 [![CI](https://github.com/gerlero/foamlib/actions/workflows/ci.yml/badge.svg)](https://github.com/gerlero/foamlib/actions/workflows/ci.yml)
 [![Codecov](https://codecov.io/gh/gerlero/foamlib/branch/main/graph/badge.svg)](https://codecov.io/gh/gerlero/foamlib)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/foamlib)](https://pypi.org/project/foamlib/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/foamlib)](https://pypi.org/project/foamlib/)
-[![Docker image](https://img.shields.io/badge/docker%20image-gerlero%2Ffoamlib-informational)](https://hub.docker.com/r/gerlero/foamlib/)
+![OpenFOAM](https://img.shields.io/badge/openfoam-.com%20|%20.org-informational)
+[![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Ffoamlib-0085a0)](https://hub.docker.com/r/microfluidica/foamlib/)
 
 **foamlib** provides a simple, modern and ergonomic Python interface for interacting with [OpenFOAM](https://www.openfoam.com).
 
 It offers the following classes:
 
 * [`FoamFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFile) (and [`FoamFieldFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFieldFile)): read-write access to OpenFOAM configuration and field files as if they were Python `dict`s, using `foamlib`'s own parser. Supports both ASCII and binary field formats.
 * [`FoamCase`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamCase): a class for manipulating, executing and accessing the results of OpenFOAM cases.
```

### Comparing `foamlib-0.3.7/pyproject.toml` & `foamlib-0.3.8/pyproject.toml`

 * *Files identical despite different names*

