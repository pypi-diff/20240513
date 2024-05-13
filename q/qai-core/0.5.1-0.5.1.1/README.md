# Comparing `tmp/qai_core-0.5.1.tar.gz` & `tmp/qai_core-0.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_core-0.5.1.tar", max compression
+gzip compressed data, was "qai_core-0.5.1.1.tar", max compression
```

## Comparing `qai_core-0.5.1.tar` & `qai_core-0.5.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       46 2024-02-10 04:57:58.583991 qai_core-0.5.1/README.md
--rw-r--r--   0        0        0      657 2024-05-02 06:03:33.523583 qai_core-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      182 2024-02-14 16:52:33.551102 qai_core-0.5.1/src/qai/core/__init__.py
--rw-r--r--   0        0        0      527 2024-02-11 05:30:15.864404 qai_core-0.5.1/src/qai/core/message.py
--rw-r--r--   0        0        0    16834 2024-05-02 06:02:49.642603 qai_core-0.5.1/src/qai/core/meta.py
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 qai_core-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-05-02 06:52:43.909391 qai_core-0.5.1.1/README.md
+-rw-r--r--   0        0        0      659 2024-05-13 04:15:44.944807 qai_core-0.5.1.1/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-05-02 06:52:43.910350 qai_core-0.5.1.1/src/qai/core/__init__.py
+-rw-r--r--   0        0        0      527 2024-05-02 06:52:43.910591 qai_core-0.5.1.1/src/qai/core/message.py
+-rw-r--r--   0        0        0    16445 2024-05-13 04:14:55.654252 qai_core-0.5.1.1/src/qai/core/meta.py
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 qai_core-0.5.1.1/PKG-INFO
```

### Comparing `qai_core-0.5.1/pyproject.toml` & `qai_core-0.5.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["parnell <3028114+parnell@users.noreply.github.com>"]
 description = ""
 name = "qai-core"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.1"
+version = "0.5.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
 json-fix = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 toml-sort = "^0.23.1"
```

### Comparing `qai_core-0.5.1/src/qai/core/message.py` & `qai_core-0.5.1.1/src/qai/core/message.py`

 * *Files identical despite different names*

### Comparing `qai_core-0.5.1/src/qai/core/meta.py` & `qai_core-0.5.1.1/src/qai/core/meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import os
 import re
 import shutil
 import tempfile
 from collections import defaultdict
 from dataclasses import dataclass, field
-from datetime import datetime, UTC
+from datetime import UTC, datetime
 from pathlib import Path
 from typing import Any, Tuple, Type, TypeVar
 from urllib.parse import urlsplit
 
 import json_fix as json_fix
 
 default_meta_file = "metadata.json"
@@ -144,48 +144,36 @@
     options: MetaOptions = None
     is_root_temp: bool = False
 
     def __init__(
         self,
         initial_dict: dict = None,
         options: MetaOptions = None,
-        use_timed_group: bool = False,
         *args,
         **kwargs,
     ):
         self.options = options or MetaOptions()
         kwargs.update(initial_dict or {})
         super().__init__(*args, **kwargs)
         self.__dict__ = self
-        self._init(use_timed_group, *args, **kwargs)
+        self._init(*args, **kwargs)
 
     def __post_init__(self):
         self._init()
 
-    def _init(self, use_timed_group: bool = False, *args, **kwargs):
-        # if self.root and self.meta_file is None:
-        #     self.meta_file = Path(os.path.join(self.root, default_meta_file))
-        # if isinstance(self.root, str):
-        #     self.root = Path(self.root)
-
-        # print("here", self.root)
-        # print("meta_file", self.meta_file)
+    def _init(self, *args, **kwargs):
         if self.meta_file:
             if os.path.exists(self.meta_file):
                 self.load()
             elif self.options.create_root:
                 os.makedirs(self.root, exist_ok=True)
-                # self.save(indent=2)
 
         if isinstance(self._root, Path):
             self._root = str(self._root.absolute())
 
-        # print("here2", self.root)
-        # print("INIT", self.root, self.meta_file, self.created_at)
-
     def __del__(self):
         if self.is_root_temp:
             shutil.rmtree(self.root)
 
     @property
     def root(self):
         return None if self._root is None else Path(self._root)
@@ -199,35 +187,32 @@
         self._root = value
 
     @property
     def meta_file(self):
         return None if self._meta_file is None else Path(self._meta_file)
 
     def __json__(self):
-        # print("__json__ here!!")
         obj: Meta = self.copy()
         ## convert Path to string for any members that are Paths
         for k, v in obj.items():
             if isinstance(v, Path):
                 obj[k] = str(v)
-        # obj["root"] = str(obj["root"])
-        # obj["meta_file"] = str(obj["meta_file"])
         return obj
 
     def abs(self, s: str):
         return Path(self.root / s).absolute()
 
     @property
     def strdate(self):
         return self.created_at.strftime()
 
     @staticmethod
     def create_most_recent(dir_path: str) -> "Meta":
         dir_path = os.path.expanduser(dir_path)
-        now = datetime.utcnow().strftime(timeformat)
+        now = datetime.now(UTC).strftime(timeformat)
         time_path = os.path.join(dir_path, now)
         return Meta.from_directory(time_path, create=True)
 
     def get_group_meta(self, group: str = None) -> dict[str, Any]:
         group = group or ROOT_GROUP
 
         if not "_groups" in self:
@@ -269,14 +254,35 @@
         files = sorted(files)
         files = [f for f in files if re.search(r"[0-9]{8,8}-[0-9]{6,6}", f) is not None]
         try:
             return str(files[-1])
         except IndexError:
             raise IndexError(f"Could not find a folder with the correct format in {dir_path}")
 
+    @staticmethod 
+    def from_within_seconds(dir_path: str | Path, time: float) -> "Meta":
+        """
+        Get the most recent folder within time seconds in dir_path or create a new one
+        """
+        if isinstance(dir_path, str) and dir_path.startswith("~"):
+            dir_path = os.path.expanduser(dir_path)
+        files = glob.glob(f"{dir_path}/*")
+        files = sorted(files)
+        files = [f for f in files if re.search(r"[0-9]{8,8}-[0-9]{6,6}", f) is not None]
+        now = datetime.now(UTC)
+        for f in files:
+            timestr = f[-15:]
+            t = datetime.strptime(timestr, timeformat)
+            ## make t UTC 
+            t = t.replace(tzinfo=UTC)
+            if (now - t).seconds < time:
+                return Meta.from_directory(f)
+        else:
+            return Meta.create_most_recent(dir_path)
+    
     @staticmethod
     def from_most_recent(dir_path: str | Path, create: bool = False) -> "Meta":
         if isinstance(dir_path, str) and dir_path.startswith("~"):
             dir_path = os.path.expanduser(dir_path)
         now = datetime.now(UTC).strftime(timeformat)
         try:
             rootdir = Meta.get_most_recent_folder(dir_path)
@@ -321,43 +327,26 @@
     def save(self, file_name: str = None, indent: int = 2, **kwargs):
         if not file_name and not self.root:
             raise ValueError("No file_name or root directory to save the metadata")
         with tempfile.NamedTemporaryFile("w", delete=False) as f:
             json.dump(self, f, indent=indent, **kwargs)
             os.rename(f.name, self.meta_file)
 
-    # def _members_to_path(self):
-    #     for k in ["root", "meta_file"]:
-    #         try:
-    #             if self[k] is None:
-    #                 continue
-    #         except:
-    #             continue
-    #         if isinstance(self[k], str):
-    #             self[k] = Path(self[k])
-
     def load(self, file_name: str = None):
         if not file_name and not self.root:
             raise ValueError("No file_name or root directory to load the metadata")
         file_name = file_name or self.meta_file
         with open(file_name, "r") as f:
             self.update(json.load(f))
 
-    # def get_file(self, file_name: str, group=None, cls: Type["MetaObj"] = None) -> "MetaObj":
-    # def get_file(self, file_name: str, group=None, cls: Type["MetaObj"] = None) -> __qualname__:
     def get_file_meta(
         self, file_name: str, group: str = None, cls: Type[C] = MetaUri, create: bool = False
     ) -> C:
         group = group or ROOT_GROUP
 
-        # print("GET FILE", file_name, group, cls)
-        # if group is None:
-        #     if not "/" in file_name:
-        #         group = ROOT_GROUP
-        #     group, file_name = file_name.split("/", maxsplit=1)[0]
         group_path = self.get_group(group)
         urimeta = self.get_uri_meta(group)
         path = Path(self._path_join(group, file_name)).absolute()
         rel_path = os.path.relpath(str(path), str(group_path))
         if file_name in urimeta:
             key = file_name
         elif rel_path in urimeta:
@@ -403,15 +392,14 @@
     def get_file(self, file_name: str, group=None) -> MetaFile:
         if group is None:
             if not "/" in file_name:
                 full_path = os.path.join(self.root, file_name)
                 if not os.path.exists(full_path):
                     raise FileNotFoundError(f"Could not find file {full_path}")
                 return full_path
-                # raise ValueError(f"group must be a valid path")
             group, file_name = file_name.split("/", maxsplit=1)[0]
         full_path = self._path_join(group, file_name)
         if not os.path.exists(full_path):
             raise FileNotFoundError(f"Could not find file {full_path}")
         muri = self.get_file_meta(file_name, group)
         return MetaFile(path=full_path, metadata=muri)
 
@@ -490,11 +478,18 @@
         return self._path_join(group)
 
     def _path_join(self, group: str, *args) -> str:
         if group is None or group == ROOT_GROUP:
             return os.path.join(self.root, *args)
         return os.path.join(self.root, group, *args)
 
-    def has_directory(self, group: str = None):
+    def has_directory(self, group: str = None) -> bool:
+        """
+        Check if the directory exists
+        Args:
+            group: the group to check
+        Returns:
+            True if the directory exists, False otherwise
+        """
         if group is None:
             return os.path.exists(self.root)
         return os.path.exists(self._path_join(group))
```

