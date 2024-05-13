# Comparing `tmp/pyfirecrest-2.4.0.tar.gz` & `tmp/pyfirecrest-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirecrest-2.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyfirecrest-2.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyfirecrest-2.4.0.tar` & `pyfirecrest-2.5.0.tar`

### file list

```diff
@@ -1,52 +1,50 @@
--rw-r--r--   0        0        0      549 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1699 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/.github/workflows/testing.yml
--rw-r--r--   0        0        0     2773 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/.gitignore
--rw-r--r--   0        0        0      318 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/.readthedocs.yml
--rw-r--r--   0        0        0     1515 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/LICENSE
--rw-r--r--   0        0        0     3245 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/README.md
--rw-r--r--   0        0        0     2502 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/async-example.md
--rw-r--r--   0        0        0      638 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/Makefile
--rw-r--r--   0        0        0     1639 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/authorization.rst
--rw-r--r--   0        0        0     2012 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/conf.py
--rw-r--r--   0        0        0      786 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/index.rst
--rw-r--r--   0        0        0      678 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/reference_async.rst
--rw-r--r--   0        0        0     1048 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/reference_basic.rst
--rw-r--r--   0        0        0      342 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/reference_cli.rst
--rw-r--r--   0        0        0      129 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/reference_index.rst
--rw-r--r--   0        0        0     4735 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_async.rst
--rw-r--r--   0        0        0    10119 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_basic.rst
--rw-r--r--   0        0        0     1499 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_cli.rst
--rw-r--r--   0        0        0     1523 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_errors.rst
--rw-r--r--   0        0        0      165 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_index.rst
--rw-r--r--   0        0        0      679 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_logging.rst
--rw-r--r--   0        0        0    63287 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/AsyncClient.py
--rw-r--r--   0        0        0     9887 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/AsyncExternalStorage.py
--rw-r--r--   0        0        0     3794 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/Authorization.py
--rw-r--r--   0        0        0    56050 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/BasicClient.py
--rw-r--r--   0        0        0     9908 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/ExternalStorage.py
--rw-r--r--   0        0        0     2690 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/FirecrestException.py
--rw-r--r--   0        0        0     1082 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/__init__.py
--rw-r--r--   0        0        0    48797 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/cli/__init__.py
--rw-r--r--   0        0        0      329 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/cli_script.py
--rw-r--r--   0        0        0    22147 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/path.py
--rw-r--r--   0        0        0       26 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/py.typed
--rw-r--r--   0        0        0     3004 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/types.py
--rw-r--r--   0        0        0      268 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/firecrest/utilities.py
--rw-r--r--   0        0        0     1709 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      146 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/common.py
--rw-r--r--   0        0        0      123 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/context.py
--rw-r--r--   0        0        0     3069 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_authorisation.py
--rw-r--r--   0        0        0    44983 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_compute.py
--rw-r--r--   0        0        0    12812 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_compute_async.py
--rw-r--r--   0        0        0    11109 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_extras.py
--rw-r--r--   0        0        0     4808 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_extras_async.py
--rw-r--r--   0        0        0     6326 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_reservation.py
--rw-r--r--   0        0        0     3752 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_reservation_async.py
--rw-r--r--   0        0        0    14130 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_status.py
--rw-r--r--   0        0        0     6207 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_status_async.py
--rw-r--r--   0        0        0    25285 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_storage.py
--rw-r--r--   0        0        0     8947 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_storage_async.py
--rw-r--r--   0        0        0    50807 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_utilities.py
--rw-r--r--   0        0        0    21316 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_utilities_async.py
--rw-r--r--   0        0        0      255 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tox.ini
--rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 pyfirecrest-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0      549 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1699 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0     2773 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/.gitignore
+-rw-r--r--   0        0        0      318 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1515 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/LICENSE
+-rw-r--r--   0        0        0     3245 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/README.md
+-rw-r--r--   0        0        0     2502 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/async-example.md
+-rw-r--r--   0        0        0      638 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/Makefile
+-rw-r--r--   0        0        0     1639 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/authorization.rst
+-rw-r--r--   0        0        0     2012 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/conf.py
+-rw-r--r--   0        0        0      786 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/index.rst
+-rw-r--r--   0        0        0      678 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/reference_async.rst
+-rw-r--r--   0        0        0     1048 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/reference_basic.rst
+-rw-r--r--   0        0        0      342 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/reference_cli.rst
+-rw-r--r--   0        0        0      129 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/reference_index.rst
+-rw-r--r--   0        0        0     4735 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/tutorial_async.rst
+-rw-r--r--   0        0        0    10119 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/tutorial_basic.rst
+-rw-r--r--   0        0        0     1499 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/tutorial_cli.rst
+-rw-r--r--   0        0        0     1523 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/tutorial_errors.rst
+-rw-r--r--   0        0        0      165 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/tutorial_index.rst
+-rw-r--r--   0        0        0      679 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/docs/source/tutorial_logging.rst
+-rw-r--r--   0        0        0    72816 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/AsyncClient.py
+-rw-r--r--   0        0        0     9887 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/AsyncExternalStorage.py
+-rw-r--r--   0        0        0     3794 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/Authorization.py
+-rw-r--r--   0        0        0    65804 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/BasicClient.py
+-rw-r--r--   0        0        0     9908 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/ExternalStorage.py
+-rw-r--r--   0        0        0     2690 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/FirecrestException.py
+-rw-r--r--   0        0        0     1082 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/__init__.py
+-rw-r--r--   0        0        0    55812 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/cli/__init__.py
+-rw-r--r--   0        0        0      329 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/cli_script.py
+-rw-r--r--   0        0        0    22147 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/path.py
+-rw-r--r--   0        0        0       26 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/py.typed
+-rw-r--r--   0        0        0     3573 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/types.py
+-rw-r--r--   0        0        0      268 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/firecrest/utilities.py
+-rw-r--r--   0        0        0     1709 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/tests/common.py
+-rw-r--r--   0        0        0      123 2024-05-13 06:26:57.657527 pyfirecrest-2.5.0/tests/context.py
+-rw-r--r--   0        0        0     3069 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_authorisation.py
+-rw-r--r--   0        0        0    58346 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_compute.py
+-rw-r--r--   0        0        0    16607 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_compute_async.py
+-rw-r--r--   0        0        0    11109 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_extras.py
+-rw-r--r--   0        0        0     4808 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_extras_async.py
+-rw-r--r--   0        0        0    14130 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_status.py
+-rw-r--r--   0        0        0     6207 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_status_async.py
+-rw-r--r--   0        0        0    25285 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_storage.py
+-rw-r--r--   0        0        0     8947 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_storage_async.py
+-rw-r--r--   0        0        0    54861 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_utilities.py
+-rw-r--r--   0        0        0    22224 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tests/test_utilities_async.py
+-rw-r--r--   0        0        0      255 2024-05-13 06:26:57.661527 pyfirecrest-2.5.0/tox.ini
+-rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 pyfirecrest-2.5.0/PKG-INFO
```

### Comparing `pyfirecrest-2.4.0/.github/workflows/python-publish.yml` & `pyfirecrest-2.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/.github/workflows/testing.yml` & `pyfirecrest-2.5.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/.gitignore` & `pyfirecrest-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/LICENSE` & `pyfirecrest-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/README.md` & `pyfirecrest-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/async-example.md` & `pyfirecrest-2.5.0/async-example.md`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/Makefile` & `pyfirecrest-2.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/authorization.rst` & `pyfirecrest-2.5.0/docs/source/authorization.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/conf.py` & `pyfirecrest-2.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/index.rst` & `pyfirecrest-2.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/reference_async.rst` & `pyfirecrest-2.5.0/docs/source/reference_async.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/reference_basic.rst` & `pyfirecrest-2.5.0/docs/source/reference_basic.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/tutorial_async.rst` & `pyfirecrest-2.5.0/docs/source/tutorial_async.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/tutorial_basic.rst` & `pyfirecrest-2.5.0/docs/source/tutorial_basic.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/tutorial_cli.rst` & `pyfirecrest-2.5.0/docs/source/tutorial_cli.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/tutorial_errors.rst` & `pyfirecrest-2.5.0/docs/source/tutorial_errors.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/docs/source/tutorial_logging.rst` & `pyfirecrest-2.5.0/docs/source/tutorial_logging.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/firecrest/AsyncClient.py` & `pyfirecrest-2.5.0/firecrest/AsyncClient.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 import pathlib
 import requests
 import sys
 import tempfile
 import time
 
 from contextlib import nullcontext
-from typing import Any, ContextManager, Optional, overload, Sequence, Tuple, List
+from typing import Any, ContextManager, Optional, overload, Sequence, List
 from requests.compat import json  # type: ignore
 from packaging.version import Version, parse
 
 import firecrest.FirecrestException as fe
 import firecrest.types as t
 from firecrest.AsyncExternalStorage import AsyncExternalUpload, AsyncExternalDownload
-from firecrest.utilities import time_block
 
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -629,27 +628,34 @@
             return result
         else:
             resp = await self._get_request(endpoint="/status/filesystems")
             return self._json_response([resp], 200)["out"]
 
     # Utilities
     async def list_files(
-        self, machine: str, target_path: str, show_hidden: bool = False
+        self, machine: str, target_path: str, show_hidden: bool = False,
+        recursive: bool = False
     ) -> List[t.LsFile]:
         """Returns a list of files in a directory.
 
         :param machine: the machine name where the filesystem belongs to
         :param target_path: the absolute target path
         :param show_hidden: show hidden files
+        :param recursive: recursively list directories encountered
         :calls: GET `/utilities/ls`
+
+        .. warning:: The argument ``recursive`` is available only for FirecREST>=1.16.0
         """
         params: dict[str, Any] = {"targetPath": f"{target_path}"}
         if show_hidden is True:
             params["showhidden"] = show_hidden
 
+        if recursive is True:
+            params["recursive"] = recursive
+
         resp = await self._get_request(
             endpoint="/utilities/ls",
             additional_headers={"X-Machine-Name": machine},
             params=params,
         )
         return self._json_response([resp], 200)["output"]
 
@@ -754,14 +760,60 @@
             endpoint="/utilities/copy",
             additional_headers={"X-Machine-Name": machine},
             data={"targetPath": target_path, "sourcePath": source_path},
         )
         self._json_response([resp], 201)
         return target_path
 
+    async def compress(self, machine: str, source_path: str, target_path: str) -> str:
+        """Compress files using gzip compression.
+        You can name the output file as you like, but typically these files have a .tar.gz extension.
+        When successful, the method returns a string with the path of the newly created file.
+
+        :param machine: the machine name where the filesystem belongs to
+        :param source_path: the absolute source path
+        :param target_path: the absolute target path
+        :calls: POST `/utilities/compress`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        resp = await self._post_request(
+            endpoint="/utilities/compress",
+            additional_headers={"X-Machine-Name": machine},
+            data={"targetPath": target_path, "sourcePath": source_path},
+        )
+        self._json_response([resp], 201)
+        return target_path
+
+    async def extract(self, machine: str, source_path: str, target_path: str, extension: str = "auto") -> str:
+        """Extract files.
+        If you don't select the extension, FirecREST will try to guess the right command based on the extension of the sourcePath.
+        Supported extensions are `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`.
+        When successful, the method returns a string with the path of the newly created file.
+
+        :param machine: the machine name where the filesystem belongs to
+        :param source_path: the absolute path of the file to be extracted
+        :param target_path: the absolute target path where the `source_path` is extracted
+        :param file_extension: possible values are `auto`, `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`
+        :calls: POST `/utilities/extract`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        resp = await self._post_request(
+            endpoint="/utilities/extract",
+            additional_headers={"X-Machine-Name": machine},
+            data={
+                "targetPath": target_path,
+                "sourcePath": source_path,
+                "extension": extension
+            },
+        )
+        self._json_response([resp], 201)
+        return target_path
+
     async def file_type(self, machine: str, target_path: str) -> str:
         """Uses the `file` linux application to determine the type of a file.
 
         :param machine: the machine name where the filesystem belongs to
         :param target_path: the absolute target path
         :calls: GET `/utilities/file`
         """
@@ -1242,14 +1294,101 @@
         if len(jobids):
             ret = [i for i in dict_result.values() if i["jobid"] in jobids]
         else:
             ret = list(dict_result.values())
 
         return ret
 
+    async def nodes(
+        self,
+        machine: str,
+        nodes: Optional[Sequence[str]] = None,
+    ) -> List[t.NodeInfo]:
+        """Retrieves information about the compute nodes.
+        This call uses the `scontrol show nodes` command.
+
+        :param machine: the machine name where the scheduler belongs to
+        :param nodes: specific compute nodes to query
+        :calls: GET `/compute/nodes`
+
+                GET `/tasks/{taskid}`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        params = {}
+        if nodes:
+            params["nodes"] = ",".join(nodes)
+
+        resp = await self._get_request(
+            endpoint="/compute/nodes",
+            additional_headers={"X-Machine-Name": machine},
+            params=params,
+        )
+        json_response = self._json_response([resp], 200)
+        t = ComputeTask(self, json_response["task_id"], [resp])
+        result = await t.poll_task("200")
+        return result
+
+    async def partitions(
+        self,
+        machine: str,
+        partitions: Optional[Sequence[str]] = None,
+    ) -> List[t.PartitionInfo]:
+        """Retrieves information about the partitions.
+        This call uses the `scontrol show partitions` command.
+
+        :param machine: the machine name where the scheduler belongs to
+        :param partitions: specific partitions nodes to query
+        :calls: GET `/compute/partitions`
+
+                GET `/tasks/{taskid}`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        params = {}
+        if partitions:
+            params["partitions"] = ",".join(partitions)
+
+        resp = await self._get_request(
+            endpoint="/compute/partitions",
+            additional_headers={"X-Machine-Name": machine},
+            params=params,
+        )
+        json_response = self._json_response([resp], 200)
+        t = ComputeTask(self, json_response["task_id"], [resp])
+        result = await t.poll_task("200")
+        return result
+
+    async def reservations(
+        self,
+        machine: str,
+        reservations: Optional[Sequence[str]] = None,
+    ) -> List[t.ReservationInfo]:
+        """Retrieves information about the reservations.
+        This call uses the `scontrol show reservations` command.
+        :param machine: the machine name where the scheduler belongs to
+        :param reservations: specific reservations to query
+        :calls: GET `/compute/reservations`
+                GET `/tasks/{taskid}`
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        params = {}
+        if reservations:
+            params["reservations"] = ",".join(reservations)
+
+        resp = await self._get_request(
+            endpoint="/compute/reservations",
+            additional_headers={"X-Machine-Name": machine},
+            params=params,
+        )
+        json_response = self._json_response([resp], 200)
+        t = ComputeTask(self, json_response["task_id"], [resp])
+        result = await t.poll_task("200")
+        return result
+
     async def cancel(self, machine: str, job_id: str | int) -> str:
         """Cancels running job.
         This call uses the `scancel` command.
 
         :param machine: the machine name where the scheduler belongs to
         :param job_id: the ID of the job
         :calls: DELETE `/compute/jobs/{job_id}`
@@ -1273,14 +1412,15 @@
         source_path,
         target_path,
         job_name,
         time,
         stage_out_job_id,
         account,
         ret_response,
+        extension=None,
     ):
         data = {"targetPath": target_path}
         if source_path:
             data["sourcePath"] = source_path
 
         if job_name:
             data["jobname"] = job_name
@@ -1290,14 +1430,17 @@
 
         if stage_out_job_id:
             data["stageOutJobId"] = stage_out_job_id
 
         if account:
             data["account"] = account
 
+        if extension:
+            data["extension"] = extension
+
         resp = await self._post_request(
             endpoint=endpoint, additional_headers={"X-Machine-Name": machine}, data=data
         )
         ret_response.append(resp)
         return self._json_response([resp], 201)
 
     async def submit_move_job(
@@ -1374,14 +1517,105 @@
         json_response = await self._internal_transfer(
             endpoint,
             machine,
             source_path,
             target_path,
             job_name,
             time,
+            stage_out_job_id,
+            account,
+            resp,
+        )
+        logger.info(f"Job submission task: {json_response['task_id']}")
+        t = ComputeTask(self, json_response["task_id"], resp)
+        return await t.poll_task("200")
+
+    async def submit_compress_job(
+        self,
+        machine: str,
+        source_path: str,
+        target_path: str,
+        job_name: Optional[str] = None,
+        time: Optional[str] = None,
+        stage_out_job_id: Optional[str] = None,
+        account: Optional[str] = None,
+    ) -> t.JobSubmit:
+        """Compress files using gzip compression.
+        You can name the output file as you like, but typically these files have a .tar.gz extension.
+        Possible to stage-out jobs providing the SLURM Id of a production job.
+
+        :param machine: the machine name where the scheduler belongs to
+        :param source_path: the absolute source path
+        :param target_path: the absolute target path
+        :param job_name: job name
+        :param time: limit on the total run time of the job. Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
+        :param stage_out_job_id: transfer data after job with ID {stage_out_job_id} is completed
+        :param account: name of the bank account to be used in SLURM. If not set, system default is taken.
+        :calls: POST `/storage/xfer-internal/compress`
+
+                GET `/tasks/{taskid}`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        resp: List[requests.Response] = []
+        endpoint = "/storage/xfer-internal/compress"
+        json_response = await self._internal_transfer(
+            endpoint,
+            machine,
+            source_path,
+            target_path,
+            job_name,
+            time,
+            stage_out_job_id,
+            account,
+            resp,
+        )
+        logger.info(f"Job submission task: {json_response['task_id']}")
+        t = ComputeTask(self, json_response["task_id"], resp)
+        return await t.poll_task("200")
+
+    async def submit_extract_job(
+        self,
+        machine: str,
+        source_path: str,
+        target_path: str,
+        extension: str = "auto",
+        job_name: Optional[str] = None,
+        time: Optional[str] = None,
+        stage_out_job_id: Optional[str] = None,
+        account: Optional[str] = None,
+    ) -> t.JobSubmit:
+        """Extract files.
+        If you don't select the extension, FirecREST will try to guess the right command based on the extension of the sourcePath.
+        Supported extensions are `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`.
+        Possible to stage-out jobs providing the SLURM Id of a production job.
+
+        :param machine: the machine name where the scheduler belongs to
+        :param source_path: the absolute source path
+        :param target_path: the absolute target path
+        :param extension: file extension, possible values are `auto`, `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`
+        :param job_name: job name
+        :param time: limit on the total run time of the job. Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
+        :param stage_out_job_id: transfer data after job with ID {stage_out_job_id} is completed
+        :param account: name of the bank account to be used in SLURM. If not set, system default is taken.
+        :calls: POST `/storage/xfer-internal/extract`
+
+                GET `/tasks/{taskid}`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        resp: List[requests.Response] = []
+        endpoint = "/storage/xfer-internal/extract"
+        json_response = await self._internal_transfer(
+            endpoint,
+            machine,
+            source_path,
+            target_path,
+            job_name,
+            time,
             stage_out_job_id,
             account,
             resp,
         )
         logger.info(f"Job submission task: {json_response['task_id']}")
         t = ComputeTask(self, json_response["task_id"], resp)
         return await t.poll_task("200")
```

### Comparing `pyfirecrest-2.4.0/firecrest/AsyncExternalStorage.py` & `pyfirecrest-2.5.0/firecrest/AsyncExternalStorage.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/firecrest/Authorization.py` & `pyfirecrest-2.5.0/firecrest/Authorization.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/firecrest/BasicClient.py` & `pyfirecrest-2.5.0/firecrest/BasicClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -445,27 +445,34 @@
             return result
         else:
             resp = self._get_request(endpoint="/status/filesystems")
             return self._json_response([resp], 200)["out"]
 
     # Utilities
     def list_files(
-        self, machine: str, target_path: str, show_hidden: bool = False
+        self, machine: str, target_path: str, show_hidden: bool = False,
+        recursive: bool = False
     ) -> List[t.LsFile]:
         """Returns a list of files in a directory.
 
         :param machine: the machine name where the filesystem belongs to
         :param target_path: the absolute target path
         :param show_hidden: show hidden files
+        :param recursive: recursively list directories encountered
         :calls: GET `/utilities/ls`
+
+        .. warning:: The argument ``recursive`` is available only for FirecREST>=1.16.0
         """
         params: dict[str, Any] = {"targetPath": f"{target_path}"}
         if show_hidden is True:
             params["showhidden"] = show_hidden
 
+        if recursive is True:
+            params["recursive"] = recursive
+
         resp = self._get_request(
             endpoint="/utilities/ls",
             additional_headers={"X-Machine-Name": machine},
             params=params,
         )
         return self._json_response([resp], 200)["output"]
 
@@ -568,14 +575,60 @@
             endpoint="/utilities/copy",
             additional_headers={"X-Machine-Name": machine},
             data={"targetPath": target_path, "sourcePath": source_path},
         )
         self._json_response([resp], 201)
         return target_path
 
+    def compress(self, machine: str, source_path: str, target_path: str) -> str:
+        """Compress files using gzip compression.
+        You can name the output file as you like, but typically these files have a .tar.gz extension.
+        When successful, the method returns a string with the path of the newly created file.
+
+        :param machine: the machine name where the filesystem belongs to
+        :param source_path: the absolute source path
+        :param target_path: the absolute target path
+        :calls: POST `/utilities/compress`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        resp = self._post_request(
+            endpoint="/utilities/compress",
+            additional_headers={"X-Machine-Name": machine},
+            data={"targetPath": target_path, "sourcePath": source_path},
+        )
+        self._json_response([resp], 201)
+        return target_path
+
+    def extract(self, machine: str, source_path: str, target_path: str, extension: str = "auto") -> str:
+        """Extract files.
+        If you don't select the extension, FirecREST will try to guess the right command based on the extension of the sourcePath.
+        Supported extensions are `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`.
+        When successful, the method returns a string with the path of the newly created file.
+
+        :param machine: the machine name where the filesystem belongs to
+        :param source_path: the absolute path of the file to be extracted
+        :param target_path: the absolute target path where the `source_path` is extracted
+        :param extension: file extension, possible values are `auto`, `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`
+        :calls: POST `/utilities/extract`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        resp = self._post_request(
+            endpoint="/utilities/extract",
+            additional_headers={"X-Machine-Name": machine},
+            data={
+                "targetPath": target_path,
+                "sourcePath": source_path,
+                "extension": extension
+            },
+        )
+        self._json_response([resp], 201)
+        return target_path
+
     def file_type(self, machine: str, target_path: str) -> str:
         """Uses the `file` linux application to determine the type of a file.
 
         :param machine: the machine name where the filesystem belongs to
         :param target_path: the absolute target path
         :calls: GET `/utilities/file`
         """
@@ -1078,14 +1131,107 @@
         json_response = self._squeue_request(machine, jobids, page_size, page_number)
         logger.info(f"Job active polling task: {json_response['task_id']}")
         dict_result = self._poll_tasks(
             json_response["task_id"], "200", iter([1, 0.5, 0.25])
         )
         return list(dict_result.values())
 
+    def nodes(
+        self,
+        machine: str,
+        nodes: Optional[Sequence[str]] = None,
+    ) -> List[t.NodeInfo]:
+        """Retrieves information about the compute nodes.
+        This call uses the `scontrol show nodes` command.
+
+        :param machine: the machine name where the scheduler belongs to
+        :param nodes: specific compute nodes to query
+        :calls: GET `/compute/nodes`
+
+                GET `/tasks/{taskid}`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        params = {}
+        if nodes:
+            params["nodes"] = ",".join(nodes)
+
+        resp = self._get_request(
+            endpoint="/compute/nodes",
+            additional_headers={"X-Machine-Name": machine},
+            params=params,
+        )
+        self._current_method_requests.append(resp)
+        json_response = self._json_response(self._current_method_requests, 200)
+        result = self._poll_tasks(
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
+        )
+        return result
+
+    def partitions(
+        self,
+        machine: str,
+        partitions: Optional[Sequence[str]] = None,
+    ) -> List[t.PartitionInfo]:
+        """Retrieves information about the compute partitions.
+        This call uses the `scontrol show partitions` command.
+
+        :param machine: the machine name where the scheduler belongs to
+        :param nodes: specific compute nodes to query
+        :calls: GET `/compute/partitions`
+
+                GET `/tasks/{taskid}`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        params = {}
+        if partitions:
+            params["partitions"] = ",".join(partitions)
+
+        resp = self._get_request(
+            endpoint="/compute/partitions",
+            additional_headers={"X-Machine-Name": machine},
+            params=params,
+        )
+        self._current_method_requests.append(resp)
+        json_response = self._json_response(self._current_method_requests, 200)
+        result = self._poll_tasks(
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
+        )
+        return result
+
+    def reservations(
+        self,
+        machine: str,
+        reservations: Optional[Sequence[str]] = None,
+    ) -> List[t.ReservationInfo]:
+        """Retrieves information about the compute reservations.
+        This call uses the `scontrol show reservations` command.
+        :param machine: the machine name where the scheduler belongs to
+        :param nodes: specific reservations to query
+        :calls: GET `/compute/reservations`
+                GET `/tasks/{taskid}`
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        params = {}
+        if reservations:
+            params["reservations"] = ",".join(reservations)
+
+        resp = self._get_request(
+            endpoint="/compute/reservations",
+            additional_headers={"X-Machine-Name": machine},
+            params=params,
+        )
+        self._current_method_requests.append(resp)
+        json_response = self._json_response(self._current_method_requests, 200)
+        result = self._poll_tasks(
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
+        )
+        return result
+
     def cancel(self, machine: str, job_id: str | int) -> str:
         """Cancels running job.
         This call uses the `scancel` command.
 
         :param machine: the machine name where the scheduler belongs to
         :param job_id: the ID of the job
         :calls: DELETE `/compute/jobs/{job_id}`
@@ -1111,14 +1257,15 @@
         machine,
         source_path,
         target_path,
         job_name,
         time,
         stage_out_job_id,
         account,
+        extension=None,
     ):
         data = {"targetPath": target_path}
         if source_path:
             data["sourcePath"] = source_path
 
         if job_name:
             data["jobName"] = job_name
@@ -1128,14 +1275,17 @@
 
         if stage_out_job_id:
             data["stageOutJobId"] = stage_out_job_id
 
         if account:
             data["account"] = account
 
+        if extension:
+            data["extension"] = extension
+
         resp = self._post_request(
             endpoint=endpoint, additional_headers={"X-Machine-Name": machine}, data=data
         )
         self._current_method_requests.append(resp)
         return self._json_response(self._current_method_requests, 201)
 
     def submit_move_job(
@@ -1338,14 +1488,106 @@
             additional_headers={"X-Machine-Name": machine},
             data={"sourcePath": source_path},
         )
         return ExternalDownload(
             self, self._json_response([resp], 201)["task_id"], [resp]
         )
 
+    def submit_compress_job(
+        self,
+        machine: str,
+        source_path: str,
+        target_path: str,
+        job_name: Optional[str] = None,
+        time: Optional[str] = None,
+        stage_out_job_id: Optional[str] = None,
+        account: Optional[str] = None,
+    ) -> t.JobSubmit:
+        """Compress files using gzip compression.
+        You can name the output file as you like, but typically these files have a .tar.gz extension.
+        Possible to stage-out jobs providing the SLURM Id of a production job.
+
+        :param machine: the machine name where the scheduler belongs to
+        :param source_path: the absolute source path
+        :param target_path: the absolute target path
+        :param job_name: job name
+        :param time: limit on the total run time of the job. Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
+        :param stage_out_job_id: transfer data after job with ID {stage_out_job_id} is completed
+        :param account: name of the bank account to be used in SLURM. If not set, system default is taken.
+        :calls: POST `/storage/xfer-internal/compress`
+
+                GET `/tasks/{taskid}`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        self._current_method_requests = []
+        endpoint = "/storage/xfer-internal/compress"
+        json_response = self._internal_transfer(
+            endpoint,
+            machine,
+            source_path,
+            target_path,
+            job_name,
+            time,
+            stage_out_job_id,
+            account,
+        )
+        logger.info(f"Job submission task: {json_response['task_id']}")
+        return self._poll_tasks(
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
+        )
+
+    def submit_extract_job(
+        self,
+        machine: str,
+        source_path: str,
+        target_path: str,
+        extension: Optional[str] = "auto",
+        job_name: Optional[str] = None,
+        time: Optional[str] = None,
+        stage_out_job_id: Optional[str] = None,
+        account: Optional[str] = None,
+    ) -> t.JobSubmit:
+        """Extract files.
+        If you don't select the extension, FirecREST will try to guess the right command based on the extension of the sourcePath.
+        Supported extensions are `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`.
+        Possible to stage-out jobs providing the SLURM Id of a production job.
+
+        :param machine: the machine name where the scheduler belongs to
+        :param source_path: the absolute source path
+        :param target_path: the absolute target path
+        :param extension: file extension, possible values are `auto`, `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`
+        :param job_name: job name
+        :param time: limit on the total run time of the job. Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
+        :param stage_out_job_id: transfer data after job with ID {stage_out_job_id} is completed
+        :param account: name of the bank account to be used in SLURM. If not set, system default is taken.
+        :calls: POST `/storage/xfer-internal/extract`
+
+                GET `/tasks/{taskid}`
+
+        .. warning:: This is available only for FirecREST>=1.16.0
+        """
+        self._current_method_requests = []
+        endpoint = "/storage/xfer-internal/extract"
+        json_response = self._internal_transfer(
+            endpoint,
+            machine,
+            source_path,
+            target_path,
+            job_name,
+            time,
+            stage_out_job_id,
+            account,
+            extension
+        )
+        logger.info(f"Job submission task: {json_response['task_id']}")
+        return self._poll_tasks(
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
+        )
+
     # Reservation
     def all_reservations(self, machine: str) -> List[dict]:
         """List all active reservations and their status
 
         :param machine: the machine name
         :calls: GET `/reservations`
         """
```

### Comparing `pyfirecrest-2.4.0/firecrest/ExternalStorage.py` & `pyfirecrest-2.5.0/firecrest/ExternalStorage.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/firecrest/FirecrestException.py` & `pyfirecrest-2.5.0/firecrest/FirecrestException.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/firecrest/__init__.py` & `pyfirecrest-2.5.0/firecrest/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 #  Please, refer to the LICENSE file in the root directory.
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 import sys
 
 
-__version__ = "2.4.0"
+__version__ = "2.5.0"
 __app_name__ = "firecrest"
 MIN_PYTHON_VERSION = (3, 7, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
     sys.stderr.write(
         "Unsupported Python version: "
```

### Comparing `pyfirecrest-2.4.0/firecrest/cli/__init__.py` & `pyfirecrest-2.5.0/firecrest/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -289,19 +289,25 @@
     path: str = typer.Argument(..., help="The absolute target path."),
     show_hidden: bool = typer.Option(
         False,
         "-a",
         "--show-hidden",
         help="Include directory entries whose names begin with a dot (‘.’).",
     ),
+    recursive: bool = typer.Option(
+        False,
+        "-R",
+        "--recursive",
+        help="Recursively list directories encountered.",
+    ),
     raw: bool = typer.Option(False, "--raw", help="Print unformatted."),
 ):
     """List directory contents"""
     try:
-        result = client.list_files(system, path, show_hidden)
+        result = client.list_files(system, path, show_hidden, recursive)
         if raw:
             console.print(result)
         else:
             table = create_table(
                 f"Files in system `{system}` and path `{path}`",
                 result,
                 ("Filename", "name"),
@@ -450,14 +456,70 @@
         client.copy(system, source, destination)
     except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
+def compress(
+    config_from_parent: str = typer.Option(None,
+        callback=config_parent_load_callback,
+        is_eager=True,
+        hidden=True
+    ),
+    system: str = typer.Option(
+        ...,
+        "-s",
+        "--system",
+        help="The name of the system where the filesystem belongs to.",
+        envvar="FIRECREST_SYSTEM",
+    ),
+    source: str = typer.Argument(..., help="The absolute source path."),
+    destination: str = typer.Argument(..., help="The absolute destination path."),
+):
+    """Compress files using gzip compression.
+    You can name the output file as you like, but typically these files have a .tar.gz extension.
+    """
+    try:
+        client.compress(system, source, destination)
+    except Exception as e:
+        examine_exeption(e)
+        raise typer.Exit(code=1)
+
+
+@app.command(rich_help_panel="Utilities commands")
+def extract(
+    config_from_parent: str = typer.Option(None,
+        callback=config_parent_load_callback,
+        is_eager=True,
+        hidden=True
+    ),
+    system: str = typer.Option(
+        ...,
+        "-s",
+        "--system",
+        help="The name of the system where the filesystem belongs to.",
+        envvar="FIRECREST_SYSTEM",
+    ),
+    source: str = typer.Argument(..., help="The absolute source path."),
+    destination: str = typer.Argument(..., help="The absolute destination path."),
+    extension: str = typer.Argument("auto", help="Extension of file. Possible values are `auto`, `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`."),
+):
+    """Extract files.
+    If you don't select the extension, FirecREST will try to guess the right command based on the extension of the sourcePath.
+    Supported extensions are `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`.
+    """
+    try:
+        client.extract(system, source, destination)
+    except Exception as e:
+        examine_exeption(e)
+        raise typer.Exit(code=1)
+
+
+@app.command(rich_help_panel="Utilities commands")
 def file(
     config_from_parent: str = typer.Option(None,
         callback=config_parent_load_callback,
         is_eager=True,
         hidden=True
     ),
     system: str = typer.Option(
@@ -1149,14 +1211,115 @@
             )
         )
     except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
+@submit_template_app.command("compress")
+def submit_compress(
+    config_from_parent: str = typer.Option(None,
+        callback=config_parent_load_callback,
+        is_eager=True,
+        hidden=True
+    ),
+    system: str = typer.Option(
+        ...,
+        "-s",
+        "--system",
+        help="The name of the system where the filesystem belongs to.",
+        envvar="FIRECREST_SYSTEM",
+    ),
+    source: str = typer.Argument(..., help="The absolute source path."),
+    destination: str = typer.Argument(..., help="The absolute destination path."),
+    job_name: Optional[str] = typer.Option(None, help="Job name in the script."),
+    time: Optional[str] = typer.Option(
+        None,
+        help="""
+        Limit on the total run time of the job.
+
+        Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
+        """,
+    ),
+    jobid: Optional[str] = typer.Option(
+        None, help="Transfer data after job with ID JOBID is completed."
+    ),
+    account: Optional[str] = typer.Option(
+        None,
+        help="""
+        Name of the project account to be used in SLURM script.
+        If not set, system default is taken.
+        """,
+    ),
+):
+    """Compress files using gzip compression.
+    You can name the output file as you like, but typically these files have a .tar.gz extension."""
+    try:
+        console.print(
+            client.submit_compress_job(
+                system, source, destination, job_name, time, jobid, account
+            )
+        )
+    except Exception as e:
+        examine_exeption(e)
+        raise typer.Exit(code=1)
+
+
+@submit_template_app.command("extract")
+def submit_extract(
+    config_from_parent: str = typer.Option(None,
+        callback=config_parent_load_callback,
+        is_eager=True,
+        hidden=True
+    ),
+    system: str = typer.Option(
+        ...,
+        "-s",
+        "--system",
+        help="The name of the system where the filesystem belongs to.",
+        envvar="FIRECREST_SYSTEM",
+    ),
+    source: str = typer.Argument(..., help="The absolute source path."),
+    destination: str = typer.Argument(..., help="The absolute destination path."),
+    extension: str = typer.Argument("auto", help="File extension, possible values are `auto`, `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`."),
+    job_name: Optional[str] = typer.Option(None, help="Job name in the script."),
+    time: Optional[str] = typer.Option(
+        None,
+        help="""
+        Limit on the total run time of the job.
+
+        Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
+        """,
+    ),
+    jobid: Optional[str] = typer.Option(
+        None, help="Transfer data after job with ID JOBID is completed."
+    ),
+    account: Optional[str] = typer.Option(
+        None,
+        help="""
+        Name of the project account to be used in SLURM script.
+        If not set, system default is taken.
+        """,
+    ),
+):
+    """Extract files.
+    If you don't select the extension, FirecREST will try to guess the right command based on the extension of the sourcePath.
+    Supported extensions are `.zip`, `.tar`, `.tgz`, `.gz` and `.bz2`.
+    """
+    try:
+        console.print(
+            client.submit_extract_job(
+                system, source, destination, job_name, time, jobid, account
+            )
+        )
+    except Exception as e:
+        examine_exeption(e)
+        raise typer.Exit(code=1)
+
+
 @submit_template_app.command("rm")
 def submit_rm(
     config_from_parent: str = typer.Option(None,
         callback=config_parent_load_callback,
         is_eager=True,
         hidden=True
     ),
@@ -1289,138 +1452,175 @@
             console.print(table)
     except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Compute commands")
-def cancel(
+def get_nodes(
     config_from_parent: str = typer.Option(None,
         callback=config_parent_load_callback,
         is_eager=True,
         hidden=True
     ),
     system: str = typer.Option(
         ..., "-s", "--system", help="The name of the system.", envvar="FIRECREST_SYSTEM"
     ),
-    job: str = typer.Argument(..., help="The ID of the job that will be cancelled."),
+    nodes: Optional[List[str]] = typer.Argument(
+        None, help="List of specific compute nodes to query."
+    ),
+    raw: bool = typer.Option(False, "--raw", help="Print unformatted."),
 ):
-    """Cancel job"""
+    """Retrieves information about the compute nodes.
+    This call uses the `scontrol show nodes` command
+    """
     try:
-        client.cancel(system, job)
-    except Exception as e:
-        examine_exeption(e)
-        raise typer.Exit(code=1)
+        results = client.nodes(system, nodes)
+        if raw:
+            console.print(results)
+        else:
+            parsed_results = []
+            for item in results:
+                parsed_item = {}
+                for key, value in item.items():
+                    if isinstance(value, list):
+                        parsed_item[key] = ", ".join(value)
+                    else:
+                        parsed_item[key] = str(value)
 
+                parsed_results.append(parsed_item)
 
-@reservation_app.command(rich_help_panel="Reservation commands")
-def list(
-    config_from_parent: str = typer.Option(None,
-        callback=config_parent_load_callback,
-        is_eager=True,
-        hidden=True
-    ),
-    system: str = typer.Option(
-        ..., "-s", "--system", help="The name of the system.", envvar="FIRECREST_SYSTEM"
-    ),
-):
-    """List all active reservations and their status"""
-    try:
-        res = client.all_reservations(system)
-        console.print(res)
+            table = create_table(
+                "Information about jobs in the queue",
+                parsed_results,
+                ("Name", "NodeName"),
+                ("Partitions", "Partitions"),
+                ("State", "State"),
+                ("Active Features", "ActiveFeatures"),
+            )
+            console.print(table)
     except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
-@reservation_app.command(rich_help_panel="Reservation commands")
-def create(
+@app.command(rich_help_panel="Compute commands")
+def get_partitions(
     config_from_parent: str = typer.Option(None,
         callback=config_parent_load_callback,
         is_eager=True,
         hidden=True
     ),
     system: str = typer.Option(
         ..., "-s", "--system", help="The name of the system.", envvar="FIRECREST_SYSTEM"
     ),
-    name: str = typer.Argument(..., help="The reservation name."),
-    account: str = typer.Argument(
-        ..., help="The account in SLURM to which the reservation is made for."
-    ),
-    num_nodes: str = typer.Argument(
-        ..., help="The number of nodes needed for the reservation."
-    ),
-    node_type: str = typer.Argument(..., help="The node type."),
-    start_time: str = typer.Argument(
-        ..., help="The start time for reservation (YYYY-MM-DDTHH:MM:SS)."
-    ),
-    end_time: str = typer.Argument(
-        ..., help="The end time for reservation (YYYY-MM-DDTHH:MM:SS)."
+    partitions: Optional[List[str]] = typer.Argument(
+        None, help="List of specific partitions to query."
     ),
+    raw: bool = typer.Option(False, "--raw", help="Print unformatted."),
 ):
-    """Create a reservation"""
+    """Retrieves information about the partitions.
+    This call uses the `scontrol show partitions` command
+    """
     try:
-        client.create_reservation(
-            system, name, account, num_nodes, node_type, start_time, end_time
-        )
+        results = client.partitions(system, partitions)
+        if raw:
+            console.print(results)
+        else:
+            parsed_results = []
+            for item in results:
+                parsed_item = {}
+                for key, value in item.items():
+                    if isinstance(value, list):
+                        parsed_item[key] = ", ".join(value)
+                    else:
+                        parsed_item[key] = str(value)
+
+                parsed_results.append(parsed_item)
+
+            table = create_table(
+                "Information about partitions in the system",
+                parsed_results,
+                ("Name", "PartitionName"),
+                ("State", "State"),
+                ("Total CPUs", "TotalCPUs"),
+                ("Total Nodes", "TotalNodes"),
+                ("Is default", "Default"),
+            )
+            console.print(table)
     except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
-@reservation_app.command(rich_help_panel="Reservation commands")
-def update(
+@app.command(rich_help_panel="Compute commands")
+def cancel(
     config_from_parent: str = typer.Option(None,
         callback=config_parent_load_callback,
         is_eager=True,
         hidden=True
     ),
     system: str = typer.Option(
         ..., "-s", "--system", help="The name of the system.", envvar="FIRECREST_SYSTEM"
     ),
-    name: str = typer.Argument(..., help="The reservation name."),
-    account: str = typer.Argument(
-        ..., help="The account in SLURM to which the reservation is made for."
-    ),
-    num_nodes: str = typer.Argument(
-        ..., help="The number of nodes needed for the reservation."
-    ),
-    node_type: str = typer.Argument(..., help="The node type."),
-    start_time: str = typer.Argument(
-        ..., help="The start time for reservation (YYYY-MM-DDTHH:MM:SS)."
-    ),
-    end_time: str = typer.Argument(
-        ..., help="The end time for reservation (YYYY-MM-DDTHH:MM:SS)."
-    ),
+    job: str = typer.Argument(..., help="The ID of the job that will be cancelled."),
 ):
-    """Update a reservation"""
+    """Cancel job"""
     try:
-        client.update_reservation(
-            system, name, account, num_nodes, node_type, start_time, end_time
-        )
+        client.cancel(system, job)
     except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
-@reservation_app.command(rich_help_panel="Reservation commands")
-def delete(
+@app.command(rich_help_panel="Compute commands")
+def get_reservations(
     config_from_parent: str = typer.Option(None,
         callback=config_parent_load_callback,
         is_eager=True,
         hidden=True
     ),
     system: str = typer.Option(
         ..., "-s", "--system", help="The name of the system.", envvar="FIRECREST_SYSTEM"
     ),
-    name: str = typer.Argument(..., help="The reservation name."),
+    reservations: Optional[List[str]] = typer.Argument(
+        None, help="List of specific reservations to query."
+    ),
+    raw: bool = typer.Option(False, "--raw", help="Print unformatted."),
 ):
-    """Delete a reservation"""
+    """Retrieves information about the reservations.
+    This call uses the `scontrol show reservations` command
+    """
     try:
-        client.delete_reservation(system, name)
+        results = client.reservations(system, reservations)
+        if raw:
+            console.print(results)
+        else:
+            parsed_results = []
+            for item in results:
+                parsed_item = {}
+                for key, value in item.items():
+                    if isinstance(value, list):
+                        parsed_item[key] = ", ".join(value)
+                    else:
+                        parsed_item[key] = str(value)
+
+                parsed_results.append(parsed_item)
+
+            table = create_table(
+                "Information about reservations in the system",
+                parsed_results,
+                ("Name", "ReservationName"),
+                ("State", "State"),
+                ("Nodes", "Nodes"),
+                ("StartTime", "StartTime"),
+                ("EndTime", "EndTime"),
+                ("Features", "Features"),
+            )
+            console.print(table)
     except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.callback()
 def main(
```

### Comparing `pyfirecrest-2.4.0/firecrest/path.py` & `pyfirecrest-2.5.0/firecrest/path.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/firecrest/types.py` & `pyfirecrest-2.5.0/firecrest/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -135,14 +135,44 @@
     start_time: str
     state: str
     time: str
     time_left: str
     user: str
 
 
+class NodeInfo(TypedDict):
+    """A node record record, from `compute/nodes`"""
+
+    NodeName: str
+    ActiveFeatures: list[str]
+    Partitions: list[str]
+    State: list[str]
+
+
+class PartitionInfo(TypedDict):
+    """A node record record, from `compute/partitions`"""
+
+    Default: str
+    PartitionName: str
+    State: str
+    TotalCPUs: str
+    TotalNodes: str
+
+
+class ReservationInfo(TypedDict):
+    """A job queue record, from `compute/reservations`"""
+
+    ReservationName: str
+    State: str
+    Nodes: str
+    StartTime: str
+    EndTime: str
+    Features: str
+
+
 class JobSubmit(TypedDict):
     """A job submit record, from `compute/jobs`"""
 
     firecrest_taskid: str
     job_data_err: str
     job_data_out: str
     job_file: str
```

### Comparing `pyfirecrest-2.4.0/pyproject.toml` & `pyfirecrest-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/tests/test_authorisation.py` & `pyfirecrest-2.5.0/tests/test_authorisation.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/tests/test_compute.py` & `pyfirecrest-2.5.0/tests/test_compute.py`

 * *Files 13% similar despite different names*

```diff
@@ -119,14 +119,83 @@
         json.dumps(ret),
         status=status_code,
         headers=extra_headers,
         content_type="application/json",
     )
 
 
+def nodes_request_handler(request: Request):
+    if not request.query_string or request.query_string == b"nodes=nid001":
+        ret = {
+            "success": "Task created",
+            "task_id": "nodes_info",
+            "task_url": "/tasks/nodes_info",
+        }
+        status_code = 200
+
+    if request.query_string == b"nodes=nidunknown":
+        ret = {
+            "success": "Task created",
+            "task_id": "info_unknown_node",
+            "task_url": "/tasks/info_unknown_node",
+        }
+        status_code = 200
+
+    return Response(
+        json.dumps(ret), status=status_code, content_type="application/json"
+    )
+
+
+def reservations_request_handler(request: Request):
+    if not request.query_string or request.query_string == b"reservations=res01":
+        ret = {
+            "success": "Task created",
+            "task_id": "reservations_info",
+            "task_url": "/tasks/reservations_info",
+        }
+        status_code = 200
+
+    if request.query_string == b"reservations=invalid_res":
+        ret = {
+            "success": "Task created",
+            "task_id": "info_unknown_reservations",
+            "task_url": "/tasks/info_unknown_reservations",
+        }
+        status_code = 200
+
+    return Response(
+        json.dumps(ret), status=status_code, content_type="application/json"
+    )
+
+
+def partitions_request_handler(request: Request):
+    if (
+        not request.query_string or
+        request.query_string == b'partitions=part01%2Cpart02%2Cxfer'
+    ):
+        ret = {
+            "success": "Task created",
+            "task_id": "partitions_info",
+            "task_url": "/tasks/partitions_info"
+        }
+        status_code = 200
+
+    if request.query_string == b'partitions=invalid_part':
+        ret = {
+            "success": "Task created",
+            "task_id": "info_unknown_partition",
+            "task_url": "/tasks/info_unknown_partition"
+        }
+        status_code = 200
+
+    return Response(
+        json.dumps(ret), status=status_code, content_type="application/json"
+    )
+
+
 def submit_upload_handler(request: Request):
     if request.headers["Authorization"] != "Bearer VALID_TOKEN":
         return Response(
             json.dumps({"message": "Bad token; invalid JSON"}),
             status=401,
             content_type="application/json",
         )
@@ -840,14 +909,183 @@
                         "task_id": taskid,
                         "task_url": f"TASK_IP/tasks/{taskid}",
                         "user": "username",
                     }
                 }
             }
             status_code = 200
+    elif taskid == "nodes_info":
+        ret = {
+            "tasks": {
+                taskid: {
+                    "created_at": "2024-04-16T09:47:06",
+                    "data": [
+                        {
+                            "ActiveFeatures": ["f7t"],
+                            "NodeName": "nid001",
+                            "Partitions": [
+                                "part01",
+                                "part02",
+                            ],
+                            "State": ["IDLE"],
+                        }
+                    ],
+                    "description": "Finished successfully",
+                    "hash_id": "nodes_info",
+                    "last_modify": "2024-04-16T09:47:06",
+                    "service": "compute",
+                    "status": "200",
+                    "system": "cluster",
+                    "task_id": "nodes_info",
+                    "task_url": "/tasks/nodes_info",
+                    "updated_at": "2024-04-16T09:47:06",
+                    "user": "service-account-firecrest-sample",
+                }
+            }
+        }
+        status_code = 200
+    elif taskid == "info_unknown_node":
+        ret = {
+            "tasks": {
+                taskid: {
+                    "created_at": "2024-04-16T09:56:14",
+                    "data": "Node nidunknown not found",
+                    "description": "Finished with errors",
+                    "hash_id": "info_unknown_node",
+                    "last_modify": "2024-04-16T09:56:14",
+                    "service": "compute",
+                    "status": "400",
+                    "system": "cluster",
+                    "task_id": "info_unknown_node",
+                    "task_url": "/tasks/info_unknown_node",
+                    "updated_at": "2024-04-16T09:56:14",
+                    "user": "service-account-firecrest-sample",
+                }
+            }
+        }
+        status_code = 200
+    elif taskid == "partitions_info":
+        ret = {
+            "tasks": {
+                taskid: {
+                    "created_at": "2024-04-24T12:02:25",
+                    "data": [
+                        {
+                            "Default": "YES",
+                            "PartitionName": "part01",
+                            "State": "UP",
+                            "TotalCPUs": "2",
+                            "TotalNodes": "1"
+                        },
+                        {
+                            "Default": "NO",
+                            "PartitionName": "part02",
+                            "State": "UP",
+                            "TotalCPUs": "2",
+                            "TotalNodes": "1"
+                        },
+                        {
+                            "Default": "NO",
+                            "PartitionName": "xfer",
+                            "State": "UP",
+                            "TotalCPUs": "2",
+                            "TotalNodes": "1"
+                        }
+                    ],
+                    "description": "Finished successfully",
+                    "hash_id": taskid,
+                    "last_modify": "2024-04-24T12:02:25",
+                    "service": "compute",
+                    "status": "200",
+                    "system": "cluster",
+                    "task_id": taskid,
+                    "task_url": f"/tasks/{taskid}",
+                    "updated_at": "2024-04-24T12:02:25",
+                    "user": "service-account-firecrest-sample"
+                }
+            }
+        }
+        status_code = 200
+    elif taskid == "info_unknown_partition":
+        ret = {
+            "tasks": {
+                taskid: {
+                    "created_at": "2024-04-24T12:17:13",
+                    "data": "Partition invalid_part not found",
+                    "description": "Finished with errors",
+                    "hash_id": taskid,
+                    "last_modify": "2024-04-24T12:02:25",
+                    "service": "compute",
+                    "status": "400",
+                    "system": "cluster",
+                    "task_id": taskid,
+                    "task_url": f"/tasks/{taskid}",
+                    "updated_at": "2024-04-24T12:17:14",
+                    "user": "service-account-firecrest-sample"
+                }
+            }
+        }
+        status_code = 200
+    elif taskid == "reservations_info":
+        ret = {
+            "tasks": {
+                taskid: {
+                    "created_at": "2024-04-24T12:02:25",
+                    "data": [
+                        {
+                            "EndTime": "2024-05-01T15:00:00",
+                            "Features": "(null)",
+                            "Nodes": "nid001",
+                            "ReservationName": "res01",
+                            "StartTime": "2024-05-01T12:00:00",
+                            "State": "INACTIVE"
+                        },
+                        {
+                            "EndTime": "2024-06-01T15:00:00",
+                            "Features": ["f7t1", "f7t2"],
+                            "Nodes": "nid002",
+                            "ReservationName": "res04",
+                            "StartTime": "2024-06-01T12:00:00",
+                            "State": "INACTIVE"
+                        }
+                    ],
+                    "description": "Finished successfully",
+                    "hash_id": taskid,
+                    "last_modify": "2024-04-24T12:02:25",
+                    "service": "compute",
+                    "status": "200",
+                    "system": "cluster",
+                    "task_id": taskid,
+                    "task_url": f"/tasks/{taskid}",
+                    "updated_at": "2024-04-24T12:02:25",
+                    "user": "service-account-firecrest-sample",
+                }
+            }
+        }
+        status_code = 200
+    elif taskid == "info_unknown_reservations":
+        ret = {
+            "tasks": {
+                taskid: {
+                    "created_at": "2024-04-24T12:17:13",
+                    "data": [],
+                    "description": "Finished with errors",
+                    "hash_id": taskid,
+                    "last_modify": "2024-04-24T12:02:25",
+                    "service": "compute",
+                    "status": "200",
+                    "system": "cluster",
+                    "task_id": taskid,
+                    "task_url": f"/tasks/{taskid}",
+                    "updated_at": "2024-04-24T12:17:14",
+                    "user": "service-account-firecrest-sample",
+                }
+            }
+        }
+        status_code = 200
 
     return Response(
         json.dumps(ret), status=status_code, content_type="application/json"
     )
 
 
 @pytest.fixture
@@ -868,17 +1106,29 @@
         queue_handler
     )
 
     httpserver.expect_request(
         re.compile("^/compute/jobs.*"), method="DELETE"
     ).respond_with_handler(cancel_handler)
 
+    httpserver.expect_request("/tasks", method="GET").respond_with_handler(
+        tasks_handler
+    )
+
+    httpserver.expect_request("/compute/nodes", method="GET").respond_with_handler(
+        nodes_request_handler
+    )
+
     httpserver.expect_request(
-        "/tasks", method="GET"
-    ).respond_with_handler(tasks_handler)
+        "/compute/reservations", method="GET"
+    ).respond_with_handler(reservations_request_handler)
+
+    httpserver.expect_request(
+        "/compute/partitions", method="GET"
+    ).respond_with_handler(partitions_request_handler)
 
     return httpserver
 
 
 @pytest.fixture
 def auth_server(httpserver):
     httpserver.expect_request("/auth/token").respond_with_handler(auth.auth_handler)
@@ -980,15 +1230,15 @@
         "result": "Job submitted",
     }
 
 
 def test_cli_submit_local(valid_credentials, slurm_script):
     global submit_upload_retry
     submit_upload_retry = 0
-    args = valid_credentials + ["submit", "--system",  "cluster1", str(slurm_script)]
+    args = valid_credentials + ["submit", "--system", "cluster1", str(slurm_script)]
     result = runner.invoke(cli.app, args=args)
     stdout = common.clean_stdout(result.stdout)
     assert result.exit_code == 0
     assert "'jobid': 35342667" in stdout
     assert "'result': 'Job submitted'" in stdout
 
     submit_upload_retry = 0
@@ -1215,15 +1465,22 @@
         },
     ]
 
 
 def test_cli_poll_active(valid_credentials):
     global queue_retry
     queue_retry = 0
-    args = valid_credentials + ["poll-active", "--system", "cluster1", "352", "2", "334"]
+    args = valid_credentials + [
+        "poll-active",
+        "--system",
+        "cluster1",
+        "352",
+        "2",
+        "334",
+    ]
     result = runner.invoke(cli.app, args=args)
     stdout = common.clean_stdout(result.stdout)
     assert result.exit_code == 0
     assert "Information about jobs in the queue" in stdout
     assert "352" in stdout
 
     queue_retry = 0
@@ -1290,7 +1547,155 @@
     with pytest.raises(firecrest.HeaderException):
         valid_client.cancel(machine="cluster2", job_id=35360071)
 
 
 def test_cancel_invalid_client(invalid_client):
     with pytest.raises(firecrest.UnauthorizedException):
         invalid_client.cancel(machine="cluster1", job_id=35360071)
+
+
+def test_get_nodes(valid_client):
+    response = [
+        {
+            "ActiveFeatures": ["f7t"],
+            "NodeName": "nid001",
+            "Partitions": ["part01", "part02"],
+            "State": ["IDLE"],
+        }
+    ]
+    assert valid_client.nodes(machine="cluster1") == response
+
+
+def test_get_nodes_from_list(valid_client):
+    response = [
+        {
+            "ActiveFeatures": ["f7t"],
+            "NodeName": "nid001",
+            "Partitions": ["part01", "part02"],
+            "State": ["IDLE"],
+        }
+    ]
+    assert valid_client.nodes(machine="cluster1", nodes=["nid001"]) == response
+
+
+def test_get_nodes_unknown(valid_client):
+    with pytest.raises(firecrest.FirecrestException):
+        valid_client.nodes(machine="cluster1", nodes=["nidunknown"])
+
+
+def test_cli_get_nodes(valid_credentials):
+    args = valid_credentials + ["get-nodes", "--system", "cluster1", "nid001"]
+    result = runner.invoke(cli.app, args=args)
+    stdout = common.clean_stdout(result.stdout)
+    assert result.exit_code == 0
+    assert "Information about jobs in the queue" in stdout
+    assert "nid001" in stdout
+    assert "part01, part02" in stdout
+    assert "IDLE" in stdout
+    assert "f7t" in stdout
+
+
+def test_get_partitions(valid_client):
+    response = [
+        {
+            "Default": "YES",
+            "PartitionName": "part01",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        },
+        {
+            "Default": "NO",
+            "PartitionName": "part02",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        },
+        {
+            "Default": "NO",
+            "PartitionName": "xfer",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        }
+    ]
+    assert valid_client.partitions(machine="cluster1") == response
+
+
+def test_get_partitions_from_list(valid_client):
+    response = [
+        {
+            "Default": "YES",
+            "PartitionName": "part01",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        },
+        {
+            "Default": "NO",
+            "PartitionName": "part02",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        },
+        {
+            "Default": "NO",
+            "PartitionName": "xfer",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        }
+    ]
+    assert valid_client.partitions(
+        machine="cluster1", partitions=["part01", "part02", "xfer"]
+    ) == response
+
+
+def test_get_partitions_unknown(valid_client):
+    with pytest.raises(firecrest.FirecrestException):
+        valid_client.partitions(
+            machine="cluster1",
+            partitions=["invalid_part"]
+        )
+
+
+def test_cli_get_partitions(valid_credentials):
+    args = (
+        valid_credentials +
+        ["get-partitions", "--system", "cluster1"]
+    )
+    result = runner.invoke(cli.app, args=args)
+    stdout = common.clean_stdout(result.stdout)
+    assert result.exit_code == 0
+    assert "Information about partitions in the system" in stdout
+    assert "part01" in stdout
+    assert "part02" in stdout
+    assert "UP" in stdout
+
+def test_get_reservations(valid_client):
+    response = [
+        {
+            "EndTime": "2024-05-01T15:00:00",
+            "Features": "(null)",
+            "Nodes": "nid001",
+            "ReservationName": "res01",
+            "StartTime": "2024-05-01T12:00:00",
+            "State": "INACTIVE"
+        },
+        {
+            "EndTime": "2024-06-01T15:00:00",
+            "Features": ["f7t1", "f7t2"],
+            "Nodes": "nid002",
+            "ReservationName": "res04",
+            "StartTime": "2024-06-01T12:00:00",
+            "State": "INACTIVE"
+        }
+    ]
+    assert valid_client.reservations(machine="cluster1") == response
+
+
+def test_cli_get_reservations(valid_credentials):
+    args = valid_credentials + ["get-reservations", "--system", "cluster1"]
+    result = runner.invoke(cli.app, args=args)
+    stdout = common.clean_stdout(result.stdout)
+    assert result.exit_code == 0
+    assert "Information about reservations in the system" in stdout
```

### Comparing `pyfirecrest-2.4.0/tests/test_compute_async.py` & `pyfirecrest-2.5.0/tests/test_compute_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -88,14 +88,26 @@
         re.compile("^/compute/jobs.*"), method="DELETE"
     ).respond_with_handler(basic_compute.cancel_handler)
 
     httpserver.expect_request(
         "/tasks", method="GET"
     ).respond_with_handler(basic_compute.tasks_handler)
 
+    httpserver.expect_request(
+        "/compute/nodes", method="GET"
+    ).respond_with_handler(basic_compute.nodes_request_handler)
+
+    httpserver.expect_request(
+        "/compute/partitions", method="GET"
+    ).respond_with_handler(basic_compute.partitions_request_handler)
+
+    httpserver.expect_request(
+        "/compute/reservations", method="GET"
+    ).respond_with_handler(basic_compute.reservations_request_handler)
+
     return httpserver
 
 
 @pytest.mark.asyncio
 async def test_submit_remote(valid_client):
     global submit_path_retry
     submit_path_retry = 0
@@ -403,7 +415,137 @@
         await valid_client.cancel(machine="cluster2", job_id=35360071)
 
 
 @pytest.mark.asyncio
 async def test_cancel_invalid_client(invalid_client):
     with pytest.raises(firecrest.UnauthorizedException):
         await invalid_client.cancel(machine="cluster1", job_id=35360071)
+
+
+@pytest.mark.asyncio
+async def test_get_nodes(valid_client):
+    response = [{
+        "ActiveFeatures": ["f7t"],
+        "NodeName": "nid001",
+        "Partitions": [
+            "part01",
+            "part02"
+        ],
+        "State": [
+            "IDLE"
+        ]
+    }]
+    assert await valid_client.nodes(machine="cluster1") == response
+
+
+@pytest.mark.asyncio
+async def test_get_nodes_from_list(valid_client):
+    response = [{
+        "ActiveFeatures": ["f7t"],
+        "NodeName": "nid001",
+        "Partitions": [
+            "part01",
+            "part02"
+        ],
+        "State": [
+            "IDLE"
+        ]
+    }]
+    assert await valid_client.nodes(machine="cluster1",
+                                    nodes=["nid001"]) == response
+
+
+@pytest.mark.asyncio
+async def test_get_nodes_unknown(valid_client):
+    with pytest.raises(firecrest.FirecrestException):
+        await valid_client.nodes(machine="cluster1",
+                                 nodes=["nidunknown"])
+
+
+@pytest.mark.asyncio
+async def test_get_partitions(valid_client):
+    response = [
+        {
+            "Default": "YES",
+            "PartitionName": "part01",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        },
+        {
+            "Default": "NO",
+            "PartitionName": "part02",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        },
+        {
+            "Default": "NO",
+            "PartitionName": "xfer",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        }
+    ]
+    assert await valid_client.partitions(machine="cluster1") == response
+
+
+@pytest.mark.asyncio
+async def test_get_partitions_from_list(valid_client):
+    response = [
+        {
+            "Default": "YES",
+            "PartitionName": "part01",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        },
+        {
+            "Default": "NO",
+            "PartitionName": "part02",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        },
+        {
+            "Default": "NO",
+            "PartitionName": "xfer",
+            "State": "UP",
+            "TotalCPUs": "2",
+            "TotalNodes": "1"
+        }
+    ]
+    assert await valid_client.partitions(
+        machine="cluster1", partitions=["part01", "part02", "xfer"]
+    ) == response
+
+
+@pytest.mark.asyncio
+async def test_get_partitions_unknown(valid_client):
+    with pytest.raises(firecrest.FirecrestException):
+        await valid_client.partitions(
+            machine="cluster1",
+            partitions=["invalid_part"]
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_reservations(valid_client):
+    response = [
+        {
+            "EndTime": "2024-05-01T15:00:00",
+            "Features": "(null)",
+            "Nodes": "nid001",
+            "ReservationName": "res01",
+            "StartTime": "2024-05-01T12:00:00",
+            "State": "INACTIVE"
+        },
+        {
+            "EndTime": "2024-06-01T15:00:00",
+            "Features": ["f7t1", "f7t2"],
+            "Nodes": "nid002",
+            "ReservationName": "res04",
+            "StartTime": "2024-06-01T12:00:00",
+            "State": "INACTIVE"
+        }
+    ]
+    assert await valid_client.reservations(machine="cluster1") == response
```

### Comparing `pyfirecrest-2.4.0/tests/test_extras.py` & `pyfirecrest-2.5.0/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/tests/test_extras_async.py` & `pyfirecrest-2.5.0/tests/test_extras_async.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/tests/test_status.py` & `pyfirecrest-2.5.0/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/tests/test_status_async.py` & `pyfirecrest-2.5.0/tests/test_status_async.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/tests/test_storage.py` & `pyfirecrest-2.5.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/tests/test_storage_async.py` & `pyfirecrest-2.5.0/tests/test_storage_async.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.4.0/tests/test_utilities.py` & `pyfirecrest-2.5.0/tests/test_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,14 +329,94 @@
         json.dumps(ret),
         status=status_code,
         headers=extra_headers,
         content_type="application/json",
     )
 
 
+def compress_handler(request: Request):
+    if request.headers["Authorization"] != "Bearer VALID_TOKEN":
+        return Response(
+            json.dumps({"message": "Bad token; invalid JSON"}),
+            status=401,
+            content_type="application/json",
+        )
+
+    if request.headers["X-Machine-Name"] != "cluster1":
+        return Response(
+            json.dumps(
+                {"description": "Error on compress operation", "error": "Machine does not exist"}
+            ),
+            status=400,
+            headers={"X-Machine-Does-Not-Exist": "Machine does not exist"},
+            content_type="application/json",
+        )
+
+    extra_headers = None
+    source_path = request.form["sourcePath"]
+    target_path = request.form["targetPath"]
+    if (
+        source_path == "/path/to/valid/source"
+        and target_path == "/path/to/valid/destination.tar.gz"
+    ):
+        ret = {"description": "Success to compress file or directory.", "output": ""}
+        status_code = 201
+    else:
+        extra_headers = {"X-Invalid-Path": "path is an invalid path"}
+        ret = {"description": "Error on compress operation"}
+        status_code = 400
+
+    return Response(
+        json.dumps(ret),
+        status=status_code,
+        headers=extra_headers,
+        content_type="application/json",
+    )
+
+
+def extract_handler(request: Request):
+    if request.headers["Authorization"] != "Bearer VALID_TOKEN":
+        return Response(
+            json.dumps({"message": "Bad token; invalid JSON"}),
+            status=401,
+            content_type="application/json",
+        )
+
+    if request.headers["X-Machine-Name"] != "cluster1":
+        return Response(
+            json.dumps(
+                {"description": "Error on compress operation", "error": "Machine does not exist"}
+            ),
+            status=400,
+            headers={"X-Machine-Does-Not-Exist": "Machine does not exist"},
+            content_type="application/json",
+        )
+
+    extra_headers = None
+    source_path = request.form["sourcePath"]
+    target_path = request.form["targetPath"]
+    if (
+        source_path == "/path/to/valid/source.tar.gz"
+        and target_path == "/path/to/valid/destination"
+    ):
+        ret = {"description": "Success to extract file or directory.", "output": ""}
+        status_code = 201
+    else:
+        extra_headers = {"X-Invalid-Path": "path is an invalid path"}
+        ret = {"description": "Error on extract operation"}
+        status_code = 400
+
+    return Response(
+        json.dumps(ret),
+        status=status_code,
+        headers=extra_headers,
+        content_type="application/json",
+    )
+
+
 def file_type_handler(request: Request):
     if request.headers["Authorization"] != "Bearer VALID_TOKEN":
         return Response(
             json.dumps({"message": "Bad token; invalid JSON"}),
             status=401,
             content_type="application/json",
         )
@@ -772,14 +852,22 @@
         chown_handler
     )
 
     httpserver.expect_request("/utilities/copy", method="POST").respond_with_handler(
         copy_handler
     )
 
+    httpserver.expect_request("/utilities/compress", method="POST").respond_with_handler(
+        compress_handler
+    )
+
+    httpserver.expect_request("/utilities/extract", method="POST").respond_with_handler(
+        extract_handler
+    )
+
     httpserver.expect_request("/utilities/file", method="GET").respond_with_handler(
         file_type_handler
     )
 
     httpserver.expect_request("/utilities/stat", method="GET").respond_with_handler(
         stat_handler
     )
@@ -1109,14 +1197,60 @@
 
 
 def test_copy_invalid_client(invalid_client):
     with pytest.raises(firecrest.UnauthorizedException):
         invalid_client.copy("cluster1", "/path/to/source", "/path/to/destination")
 
 
+def test_compress(valid_client):
+    # Mostly sure this doesn't raise an error
+    assert (
+        valid_client.compress(
+            "cluster1",
+            "/path/to/valid/source",
+            "/path/to/valid/destination.tar.gz"
+        ) == "/path/to/valid/destination.tar.gz"
+    )
+
+
+def test_cli_compress(valid_credentials):
+    args = valid_credentials + [
+        "compress",
+        "--system",
+        "cluster1",
+        "/path/to/valid/source",
+        "/path/to/valid/destination.tar.gz",
+    ]
+    result = runner.invoke(cli.app, args=args)
+    assert result.exit_code == 0
+
+
+def test_extract(valid_client):
+    # Mostly sure this doesn't raise an error
+    assert (
+        valid_client.extract(
+            "cluster1",
+            "/path/to/valid/source.tar.gz",
+            "/path/to/valid/destination"
+        ) == "/path/to/valid/destination"
+    )
+
+
+def test_cli_extract(valid_credentials):
+    args = valid_credentials + [
+        "extract",
+        "--system",
+        "cluster1",
+        "/path/to/valid/source.tar.gz",
+        "/path/to/valid/destination",
+    ]
+    result = runner.invoke(cli.app, args=args)
+    assert result.exit_code == 0
+
+
 def test_file_type(valid_client):
     assert valid_client.file_type("cluster1", "/path/to/empty/file") == "empty"
     assert valid_client.file_type("cluster1", "/path/to/directory") == "directory"
 
 
 def test_cli_file_type(valid_credentials):
     args = valid_credentials + ["file", "--system", "cluster1", "/path/to/empty/file"]
```

### Comparing `pyfirecrest-2.4.0/tests/test_utilities_async.py` & `pyfirecrest-2.5.0/tests/test_utilities_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,22 @@
         basic_utilities.chown_handler
     )
 
     httpserver.expect_request("/utilities/copy", method="POST").respond_with_handler(
         basic_utilities.copy_handler
     )
 
+    httpserver.expect_request("/utilities/compress", method="POST").respond_with_handler(
+        basic_utilities.compress_handler
+    )
+
+    httpserver.expect_request("/utilities/extract", method="POST").respond_with_handler(
+        basic_utilities.extract_handler
+    )
+
     httpserver.expect_request("/utilities/file", method="GET").respond_with_handler(
         basic_utilities.file_type_handler
     )
 
     httpserver.expect_request("/utilities/stat", method="GET").respond_with_handler(
         basic_utilities.stat_handler
     )
@@ -355,14 +363,38 @@
 @pytest.mark.asyncio
 async def test_copy_invalid_client(invalid_client):
     with pytest.raises(firecrest.UnauthorizedException):
         await invalid_client.copy("cluster1", "/path/to/source", "/path/to/destination")
 
 
 @pytest.mark.asyncio
+async def test_compress(valid_client):
+    # Mostly sure this doesn't raise an error
+    assert (
+       await valid_client.compress(
+            "cluster1",
+            "/path/to/valid/source",
+            "/path/to/valid/destination.tar.gz"
+        ) == "/path/to/valid/destination.tar.gz"
+    )
+
+
+@pytest.mark.asyncio
+async def test_extract(valid_client):
+    # Mostly sure this doesn't raise an error
+    assert (
+        await valid_client.extract(
+            "cluster1",
+            "/path/to/valid/source.tar.gz",
+            "/path/to/valid/destination"
+        ) == "/path/to/valid/destination"
+    )
+
+
+@pytest.mark.asyncio
 async def test_file_type(valid_client):
     assert await valid_client.file_type("cluster1", "/path/to/empty/file") == "empty"
     assert await valid_client.file_type("cluster1", "/path/to/directory") == "directory"
 
 
 @pytest.mark.asyncio
 async def test_file_type_invalid_arguments(valid_client):
```

### Comparing `pyfirecrest-2.4.0/PKG-INFO` & `pyfirecrest-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfirecrest
-Version: 2.4.0
+Version: 2.5.0
 Summary: pyFirecrest is a python wrapper for FirecREST
 Author: CSCS Swiss National Supercomputing Center
 Maintainer-email: Eirini Koutsaniti <eirini.koutsaniti@cscs.ch>, Juan Pablo Dorsch <juanpablo.dorsch@cscs.ch>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

