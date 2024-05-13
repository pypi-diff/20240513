# Comparing `tmp/pyobas-1.0.0.tar.gz` & `tmp/pyobas-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobas-1.0.0.tar", last modified: Mon May 13 10:07:34 2024, max compression
+gzip compressed data, was "pyobas-4.0.0.tar", last modified: Sat Mar 23 02:10:08 2024, max compression
```

## Comparing `pyobas-1.0.0.tar` & `pyobas-4.0.0.tar`

### file list

```diff
@@ -1,43 +1,20 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.549553 pyobas-1.0.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-13 10:07:24.000000 pyobas-1.0.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-13 10:07:34.549553 pyobas-1.0.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-13 10:07:24.000000 pyobas-1.0.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.545553 pyobas-1.0.0/pyobas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.545553 pyobas-1.0.0/pyobas/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      497 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/collector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/inject.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/injector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/me.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/organization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/team.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/apis/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.545553 pyobas-1.0.0/pyobas/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/backends/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/backends/backend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/backends/protocol.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16141 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.549553 pyobas-1.0.0/pyobas/contracts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/contract_builder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5582 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/contract_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/contract_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/contracts/variable_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14284 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyobas/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 10:07:34.549553 pyobas-1.0.0/pyobas.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-13 10:07:34.000000 pyobas-1.0.0/pyobas.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-13 10:07:24.000000 pyobas-1.0.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1386 2024-05-13 10:07:34.549553 pyobas-1.0.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-23 02:10:08.118317 pyobas-4.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-03-23 02:09:59.000000 pyobas-4.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2514 2024-03-23 02:10:08.118317 pyobas-4.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      808 2024-03-23 02:09:59.000000 pyobas-4.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-23 02:10:08.118317 pyobas-4.0.0/pyobas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2024-03-23 02:09:59.000000 pyobas-4.0.0/pyobas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-03-23 02:09:59.000000 pyobas-4.0.0/pyobas/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-03-23 02:09:59.000000 pyobas-4.0.0/pyobas/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15908 2024-03-23 02:09:59.000000 pyobas-4.0.0/pyobas/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-03-23 02:09:59.000000 pyobas-4.0.0/pyobas/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6580 2024-03-23 02:09:59.000000 pyobas-4.0.0/pyobas/mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-03-23 02:09:59.000000 pyobas-4.0.0/pyobas/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-23 02:10:08.118317 pyobas-4.0.0/pyobas.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2514 2024-03-23 02:10:08.000000 pyobas-4.0.0/pyobas.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      315 2024-03-23 02:10:08.000000 pyobas-4.0.0/pyobas.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-23 02:10:08.000000 pyobas-4.0.0/pyobas.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-03-23 02:10:08.000000 pyobas-4.0.0/pyobas.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-03-23 02:10:08.000000 pyobas-4.0.0/pyobas.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-03-23 02:09:59.000000 pyobas-4.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1338 2024-03-23 02:10:08.118317 pyobas-4.0.0/setup.cfg
```

### Comparing `pyobas-1.0.0/LICENSE` & `pyobas-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/base.py` & `pyobas-4.0.0/pyobas/base.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/client.py` & `pyobas-4.0.0/pyobas/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Any, BinaryIO, Dict, List, Optional, Union
 from urllib import parse
 
 import requests
 
-from pyobas import exceptions, utils
+from pyobas import _backends, exceptions, utils
 from pyobas._version import __version__  # noqa: F401
 
 REDIRECT_MSG = (
     "pyobas detected a {status_code} ({reason!r}) redirection. You must update "
     "your OpenBVAS URL to the correct URL to avoid issues. The redirection was from: "
     "{source!r} to {target!r}"
 )
@@ -37,38 +37,31 @@
         self.headers = {
             "User-Agent": "pyobas/" + __version__,
             "Authorization": "Bearer " + token,
         }
         #: Whether SSL certificates should be validated
         self.ssl_verify = ssl_verify
 
-        # Import backends
-        from pyobas import backends
-
-        self.backend = backends.RequestsBackend(**kwargs)
-        self._auth = backends.TokenAuth(token)
-        self.session = self.backend.client
+        self._backend = _backends.DefaultBackend(**kwargs)
+        self._auth = _backends.TokenAuth(token)
+        self.session = self._backend.client
 
         self.per_page = per_page
         self.pagination = pagination
         self.order_by = order_by
 
         # Import all apis
-        from pyobas import apis
+        from pyobas import _apis
 
-        self.me = apis.MeManager(self)
-        self.organization = apis.OrganizationManager(self)
-        self.injector = apis.InjectorManager(self)
-        self.collector = apis.CollectorManager(self)
-        self.inject = apis.InjectManager(self)
-        self.document = apis.DocumentManager(self)
-        self.kill_chain_phase = apis.KillChainPhaseManager(self)
-        self.attack_pattern = apis.AttackPatternManager(self)
-        self.team = apis.TeamManager(self)
-        self.user = apis.UserManager(self)
+        self.me = _apis.MeManager(self)
+        self.organization = _apis.OrganizationManager(self)
+        self.injector = _apis.InjectorManager(self)
+        self.inject = _apis.InjectManager(self)
+        self.kill_chain_phase = _apis.KillChainPhaseManager(self)
+        self.attack_pattern = _apis.AttackPatternManager(self)
 
     @staticmethod
     def _check_redirects(result: requests.Response) -> None:
         # Check the requests history to detect 301/302 redirections.
         # If the initial verb is POST or PUT, the redirected request will use a
         # GET request, leading to unwanted behaviour.
         # If we detect a redirection with a POST or a PUT request, we
@@ -99,15 +92,15 @@
         it to the stored url.
 
         Returns:
             The full URL
         """
         if path.startswith("http://") or path.startswith("https://"):
             return path
-        return f"{self.url}/api{path}"
+        return f"{self.url}{path}"
 
     def _get_session_opts(self) -> Dict[str, Any]:
         return {
             "headers": self.headers.copy(),
             "auth": self._auth,
             "timeout": self.timeout,
             "verify": self.ssl_verify,
@@ -169,21 +162,21 @@
         verify = opts.pop("verify")
         opts_timeout = opts.pop("timeout")
         # If timeout was passed into kwargs, allow it to override the default
         if timeout is None:
             timeout = opts_timeout
 
         # We need to deal with json vs. data when uploading files
-        send_data = self.backend.prepare_send_data(files, post_data, raw)
+        send_data = self._backend.prepare_send_data(files, post_data, raw)
         opts["headers"]["Content-type"] = send_data.content_type
 
         # cur_retries = 0
         while True:
             # noinspection PyTypeChecker
-            result = self.backend.http_request(
+            result = self._backend.http_request(
                 method=verb,
                 url=url,
                 json=send_data.json,
                 data=send_data.data,
                 params=params,
                 timeout=timeout,
                 verify=verify,
@@ -257,14 +250,15 @@
         post_data: Optional[Dict[str, Any]] = None,
         raw: bool = False,
         files: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Union[Dict[str, Any], requests.Response]:
         query_data = query_data or {}
         post_data = post_data or {}
+
         result = self.http_request(
             "post",
             path,
             query_data=query_data,
             post_data=post_data,
             files=files,
             raw=raw,
```

### Comparing `pyobas-1.0.0/pyobas/exceptions.py` & `pyobas-4.0.0/pyobas/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyobas/mixins.py` & `pyobas-4.0.0/pyobas/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -191,27 +191,19 @@
     _parent: Optional[base.RESTObject]
     _parent_attrs: Dict[str, Any]
     _path: Optional[str]
     openbas: pyobas.OpenBAS
 
     @exc.on_http_error(exc.OpenBASCreateError)
     def create(
-        self, data: Optional[Dict[str, Any]] = None, icon: tuple = None, **kwargs: Any
+        self, data: Optional[Dict[str, Any]] = None, **kwargs: Any
     ) -> base.RESTObject:
         if data is None:
             data = {}
         self._create_attrs.validate_attrs(data=data)
         # Handle specific URL for creation
         path = kwargs.pop("path", self.path)
-        if icon:
-            files = {"icon": icon}
-        elif icon is False:
-            files = {}
-        else:
-            files = None
-        server_data = self.openbas.http_post(
-            path, post_data=data, files=files, **kwargs
-        )
+        server_data = self.openbas.http_post(path, post_data=data, **kwargs)
         if TYPE_CHECKING:
             assert not isinstance(server_data, requests.Response)
             assert self._obj_cls is not None
         return self._obj_cls(self, server_data)
```

### Comparing `pyobas-1.0.0/pyobas/utils.py` & `pyobas-4.0.0/pyobas/utils.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/pyproject.toml` & `pyobas-4.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.0/setup.cfg` & `pyobas-4.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -22,32 +22,29 @@
 	Topic :: Security
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 python_requires = >=3.7
 packages = 
 	pyobas
-	pyobas.apis
-	pyobas.backends
-	pyobas.contracts
 include_package_data = True
 install_requires = 
 	dataclasses-json~=0.6.4
 	pika~=1.3.1
 	prometheus-client~=0.20.0
 	python_json_logger~=2.0.4
 	pyyaml~=6.0
 	requests~=2.31.0
 	requests-toolbelt~=1.0.0
-	setuptools~=69.5.1
+	setuptools~=69.2.0
 
 [options.extras_require]
 dev = 
-	black~=24.4.0
-	build~=1.2.1
+	black~=24.3.0
+	build~=1.1.1
 	isort~=5.13.0
 	types-pytz~=2024.1.0.20240203
 	pre-commit~=3.6.0
 	types-python-dateutil~=2.9.0
 	wheel~=0.43.0
 doc = 
 	autoapi~=2.0.1
```

