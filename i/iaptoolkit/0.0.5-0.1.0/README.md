# Comparing `tmp/iaptoolkit-0.0.5.tar.gz` & `tmp/iaptoolkit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iaptoolkit-0.0.5.tar", max compression
+gzip compressed data, was "iaptoolkit-0.1.0.tar", max compression
```

## Comparing `iaptoolkit-0.0.5.tar` & `iaptoolkit-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1072 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/LICENSE
--rwxr-xr-x   0        0        0     1343 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/README.md
--rwxr-xr-x   0        0        0     1010 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       77 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/__init__.py
--rw-r--r--   0        0        0      522 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/constants.py
--rw-r--r--   0        0        0     1507 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/exceptions.py
--rw-r--r--   0        0        0     4041 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/headers.py
--rw-r--r--   0        0        0      931 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/tokens/__init__.py
--rw-r--r--   0        0        0     8135 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/tokens/service_account.py
--rw-r--r--   0        0        0     1330 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/tokens/structs.py
--rw-r--r--   0        0        0     2689 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/tokens/token_datastore.py
--rw-r--r--   0        0        0        0 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/utils/__init__.py
--rw-r--r--   0        0        0     1477 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/utils/urls.py
--rw-r--r--   0        0        0      817 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/vars.py
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 iaptoolkit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-13 01:02:13.498532 iaptoolkit-0.1.0/LICENSE
+-rwxr-xr-x   0        0        0     1343 2024-05-13 01:02:13.498532 iaptoolkit-0.1.0/README.md
+-rwxr-xr-x   0        0        0     1010 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4742 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/__init__.py
+-rw-r--r--   0        0        0      522 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/constants.py
+-rw-r--r--   0        0        0     1507 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/exceptions.py
+-rw-r--r--   0        0        0     2896 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/headers.py
+-rw-r--r--   0        0        0      673 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/tokens/__init__.py
+-rw-r--r--   0        0        0     8036 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/tokens/service_account.py
+-rw-r--r--   0        0        0     1330 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/tokens/structs.py
+-rw-r--r--   0        0        0     2699 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/tokens/token_datastore.py
+-rw-r--r--   0        0        0        0 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/utils/__init__.py
+-rw-r--r--   0        0        0     1477 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/utils/urls.py
+-rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 iaptoolkit-0.1.0/PKG-INFO
```

### Comparing `iaptoolkit-0.0.5/LICENSE` & `iaptoolkit-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.5/README.md` & `iaptoolkit-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.5/pyproject.toml` & `iaptoolkit-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iaptoolkit"
-version = "0.0.5"
+version = "0.1.0"
 description = "Library of common utils for interacting with Identity-Aware Proxies"
 authors = ["Rob Voigt <code@ravoigt.com>"]
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `iaptoolkit-0.0.5/src/iaptoolkit/constants.py` & `iaptoolkit-0.1.0/src/iaptoolkit/constants.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.5/src/iaptoolkit/exceptions.py` & `iaptoolkit-0.1.0/src/iaptoolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.5/src/iaptoolkit/headers.py` & `iaptoolkit-0.1.0/src/iaptoolkit/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,130 @@
+from __future__ import annotations
+
+import logging
+logging.getLogger(__name__).addHandler(logging.NullHandler())
+
 import typing as t
+from urllib.parse import ParseResult
 from urllib.parse import urlparse
+
 from kvcommon import logger
 
-from iaptoolkit.constants import GOOGLE_IAP_AUTH_HEADER
-from iaptoolkit.constants import GOOGLE_IAP_AUTH_HEADER_PROXY
-from iaptoolkit.tokens import get_token_for_google_service_account
+from iaptoolkit import headers
+from iaptoolkit.exceptions import ServiceAccountTokenException
+from iaptoolkit.tokens.service_account import ServiceAccount
 from iaptoolkit.tokens.structs import ResultAddTokenHeader
+
+from iaptoolkit.tokens.structs import TokenRefreshStruct
 from iaptoolkit.utils.urls import is_url_safe_for_token
-from iaptoolkit.vars import IAPTOOLKIT_USE_AUTH_HEADER
-from iaptoolkit.vars import GOOGLE_IAP_CLIENT_ID
 
 LOG = logger.get_logger("iaptk")
 
 
-def _sanitize_request_header(headers_dict: dict, header_key: str):
-    auth_header = headers_dict.get(header_key, None)
-    if auth_header:
-        # TODO: Handle multiple tokens (e.g.; "Bearer <token1>, Bearer  <token2>") properly
-        if "Bearer" in auth_header:
-            headers_dict[header_key] = "Bearer <token_hidden>"
-        elif "Basic" in auth_header:
-            headers_dict[header_key] = "Basic <basic_auth_hidden>"
-        else:
-            headers_dict[header_key] = "<contents_hidden>"
-
-
-def sanitize_request_headers(headers: dict) -> dict:
+class IAPToolkit:
     """
-    Sanitizes a headers dict to remove sensitive strings for logging purposes.
-    Returns A COPY of the dict with sensitive k/v pairs replaced. Does NOT modify in-place/by-reference.
+    Class to encapsulate client-specific vars and forward them to static functions
     """
-    log_safe_headers = headers.copy()
 
-    _sanitize_request_header(log_safe_headers, GOOGLE_IAP_AUTH_HEADER)
-    _sanitize_request_header(log_safe_headers, GOOGLE_IAP_AUTH_HEADER_PROXY)
-    _sanitize_request_header(log_safe_headers, "X-Goog-Iap-Jwt-Assertion")
+    _GOOGLE_IAP_CLIENT_ID: str
+    _USE_AUTH_HEADER: bool
+    # _GOOGLE_CLIENT_ID: str   # TODO: OAuth2
+    # _GOOGLE_CLIENT_SECRET: str  # TODO: OAuth2
+
+    def __init__(
+        self,
+        google_iap_client_id: str,
+        use_auth_header: bool,
+        # google_client_id: str,
+        # google_client_secret: str,
+    ) -> None:
+        self._GOOGLE_IAP_CLIENT_ID = google_iap_client_id
+        self._USE_AUTH_HEADER = use_auth_header
+        # self._GOOGLE_CLIENT_ID = google_client_id
+        # self._GOOGLE_CLIENT_SECRET = google_client_secret
+
+        # self.ServiceAccount = GoogleServiceAccount(iap_client_id=google_iap_client_id)
+
+    @staticmethod
+    def sanitize_request_headers(request_headers: dict) -> dict:
+        return headers.sanitize_request_headers(request_headers)
+
+    def get_token_oidc(self, bypass_cached: bool = False) -> TokenRefreshStruct:
+        try:
+            return ServiceAccount.get_token(
+                iap_client_id=self._GOOGLE_IAP_CLIENT_ID, bypass_cached=bypass_cached
+            )
+        except ServiceAccountTokenException as ex:
+            LOG.debug(ex)
+            raise
+
+    def get_token_oauth2(self) -> TokenRefreshStruct:
+        # TODO
+        raise NotImplementedError()
+
+    def get_token_and_add_to_headers(self, request_headers: dict, use_oauth2: bool = False) -> bool:
+        """
+        Retrieves an auth token and inserts it into the supplied request_headers dict.
+        request_headers is modified in-place
+
+        Params:
+            request_headers: dict of headers to insert into
+            use_oauth2: Use OAuth2.0 credentials and respective token, else use OIDC (default)
+                As a general guideline, OIDC is the assumed default approach for ServiceAccounts.
+
+
+        """
+        if not use_oauth2:
+            token_refresh_struct: TokenRefreshStruct = self.get_token_oidc()
+        else:
+            token_refresh_struct: TokenRefreshStruct = self.get_token_oauth2()
 
-    return log_safe_headers
+        headers.add_token_to_request_headers(
+            request_headers=request_headers,
+            id_token=token_refresh_struct.id_token,
+            use_auth_header=self._USE_AUTH_HEADER,
+        )
 
+        return token_refresh_struct.token_is_new
 
-def add_token_to_request_headers(request_headers: dict, use_oauth2: bool, iap_client_id: str) -> bool:
-    """
-    Adds Bearer token to headers dict. Modifies dict in-place.
-    Returns True if added token is a fresh one, or False if token is from cache
-    """
-    # TODO: Make this less google-specific, or move it to a google-specific implementation
-    # TODO: oauth2
-
-    token_refresh_struct = get_token_for_google_service_account(iap_client_id=iap_client_id)
-    id_token: str = token_refresh_struct.id_token
-    auth_header_str = "Bearer {}".format(id_token)
-
-    auth_header_key = GOOGLE_IAP_AUTH_HEADER_PROXY
-    # Don't override an existing authorization header if there is one
-    # Google IAP supports passing the token in 'Proxy-Authorization' header if `Authorization` is already in use
-    if IAPTOOLKIT_USE_AUTH_HEADER:
-        if GOOGLE_IAP_AUTH_HEADER not in request_headers:
-            request_headers[GOOGLE_IAP_AUTH_HEADER] = auth_header_str
-            auth_header_key = GOOGLE_IAP_AUTH_HEADER
+    @staticmethod
+    def is_url_safe_for_token(
+        url: str | ParseResult,
+        valid_domains: t.Optional[t.List[str] | t.Set[str] | t.Tuple[str]] = None,
+    ):
+        if not isinstance(url, ParseResult):
+            url = urlparse(url)
+
+        return is_url_safe_for_token(url_parts=url, allowed_domains=valid_domains)
+
+    def check_url_and_add_token_header(
+        self,
+        url: str | ParseResult,
+        request_headers: dict,
+        valid_domains: t.List[str] | None = None,
+        use_oauth2: bool = False,
+    ) -> ResultAddTokenHeader:
+        """
+            Checks that the supplied URL is valid (i.e.; in valid_domains) and if so, retrieves a
+            token and adds it to request_headers.
+
+            i.e.; A convenience wrapper with logging for is_url_safe_for_token() and get_token_and_add_to_headers()
+
+            Params:
+                url: URL string or urllib.ParseResult to check for validity
+                request_headers: Dict of headers to insert into
+                valid_domains: List of domains to validate URL against
+                use_oauth2: Passed to get_token_and_add_to_headers() to determine if OAuth2.0 is used or OIDC (default)
+        """
+
+        if self.is_url_safe_for_token(url=url, valid_domains=valid_domains):
+            token_is_fresh = self.get_token_and_add_to_headers(
+                request_headers=request_headers, use_oauth2=use_oauth2
+            )
+            return ResultAddTokenHeader(token_added=True, token_is_fresh=token_is_fresh)
         else:
-            LOG.debug(
-                "IAPTOOLKIT_USE_AUTH_HEADER is set but 'Authorization' header already exists. "
-                "Adding IAP token to Proxy-Authorization header only."
+            LOG.warn(
+                "URL is not approved: %s - Token will not be added to headers. Valid domains are: %s",
+                url,
+                valid_domains,
             )
-
-    request_headers[auth_header_key] = auth_header_str
-
-    return token_refresh_struct.token_is_new
-
-
-def check_url_and_add_token_header(
-    url: str,
-    request_headers: dict,
-    use_oauth2: bool = False,
-    valid_domains: t.List[str] | None = None,
-    iap_client_id: str = GOOGLE_IAP_CLIENT_ID
-) -> ResultAddTokenHeader:
-    """Prevent inadvertently sending private tokens to arbitrary locations.
-    Returns:
-        True, True: Adding token was allowed and token is fresh
-        True, False: Adding token was allowed and token is from cache
-        False, False: Adding token was not allowed
-    """
-    url_parts = urlparse(url)
-
-    # Verify that the url's domain is one we allow before adding a token
-    if is_url_safe_for_token(url_parts, valid_domains):
-        token_is_fresh = add_token_to_request_headers(request_headers, use_oauth2, iap_client_id=iap_client_id)
-        return ResultAddTokenHeader(token_added=True, token_is_fresh=token_is_fresh)
-    else:
-        LOG.warn(
-            "URL is not approved: %s - Token will not be added to headers. Valid domains are: %s",
-            url,
-            valid_domains,
-        )
-        return ResultAddTokenHeader(token_added=False, token_is_fresh=False)
+            return ResultAddTokenHeader(token_added=False, token_is_fresh=False)
```

### Comparing `iaptoolkit-0.0.5/src/iaptoolkit/tokens/__init__.py` & `iaptoolkit-0.1.0/src/iaptoolkit/tokens/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,23 +11,14 @@
 # from .oauth2 import get_token_for_oauth2  # TODO: OAuth2
 # from .service_account import ServiceAccount
 from .service_account import GoogleServiceAccount
 
 LOG = logger.get_logger("iaptk")
 
 
-def get_token_for_google_service_account(iap_client_id):
-    try:
-        return GoogleServiceAccount(iap_client_id).get_token()
-    except ServiceAccountTokenException as ex:
-        LOG.debug(ex)
-        raise
-
-
 __all__ = [
-    "get_token_for_google_service_account",
     "TokenStruct",
     "TokenRefreshStruct",
     # "TokenStructOAuth2",  # TODO: OAuth2
     "TokenException",
     "TokenStorageException",
 ]
```

### Comparing `iaptoolkit-0.0.5/src/iaptoolkit/tokens/service_account.py` & `iaptoolkit-0.1.0/src/iaptoolkit/tokens/service_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 # TODO: Don't hardcode the association between OIDC/SA and dict-datastore
 from iaptoolkit.tokens.token_datastore import datastore
 from iaptoolkit.exceptions import ServiceAccountTokenException
 from iaptoolkit.exceptions import ServiceAccountTokenFailedRefresh
 from iaptoolkit.exceptions import ServiceAccountNoDefaultCredentials
 from iaptoolkit.exceptions import TokenStorageException
 
-# from iaptoolkit.vars import GOOGLE_CLIENT_ID
-# from iaptoolkit.vars import GOOGLE_CLIENT_SECRET
-
 from .structs import TokenStruct
 from .structs import TokenRefreshStruct
 
 
 LOG = logger.get_logger("iaptk")
 MAX_RECURSE = 3
```

### Comparing `iaptoolkit-0.0.5/src/iaptoolkit/tokens/structs.py` & `iaptoolkit-0.1.0/src/iaptoolkit/tokens/structs.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.5/src/iaptoolkit/tokens/token_datastore.py` & `iaptoolkit-0.1.0/src/iaptoolkit/tokens/token_datastore.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from kvcommon import logger
 from kvcommon.datastore.backend import DatastoreBackend
 from kvcommon.datastore.backend import DictBackend
 from kvcommon.datastore.backend import TOMLBackend
 from kvcommon.datastore import VersionedDatastore
 
 from iaptoolkit.constants import IAPTOOLKIT_CONFIG_VERSION
-from iaptoolkit.vars import PERSISTENT_DATASTORE_ENABLED
-from iaptoolkit.vars import PERSISTENT_DATASTORE_PATH
-from iaptoolkit.vars import PERSISTENT_DATASTORE_USERNAME
+# from iaptoolkit.vars import PERSISTENT_DATASTORE_ENABLED
+# from iaptoolkit.vars import PERSISTENT_DATASTORE_PATH
+# from iaptoolkit.vars import PERSISTENT_DATASTORE_USERNAME
 
 
 LOG = logger.get_logger("iaptk-ds")
 
 
 class TokenDatastore(VersionedDatastore):
     _service_account_tokens_key = "service_account_tokens"
@@ -63,9 +63,9 @@
 
     # def store_oauth2_token(self, iap_client_id: str):
     #     # TODO: OAuth2
     #     raise NotImplementedError()
 
 datastore = TokenDatastore(DictBackend)
 
-if PERSISTENT_DATASTORE_ENABLED:
-    datastore_toml = TokenDatastore(TOMLBackend(PERSISTENT_DATASTORE_PATH, PERSISTENT_DATASTORE_USERNAME))
+# if PERSISTENT_DATASTORE_ENABLED:
+#     datastore_toml = TokenDatastore(TOMLBackend(PERSISTENT_DATASTORE_PATH, PERSISTENT_DATASTORE_USERNAME))
```

### Comparing `iaptoolkit-0.0.5/src/iaptoolkit/utils/urls.py` & `iaptoolkit-0.1.0/src/iaptoolkit/utils/urls.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.5/PKG-INFO` & `iaptoolkit-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaptoolkit
-Version: 0.0.5
+Version: 0.1.0
 Summary: Library of common utils for interacting with Identity-Aware Proxies
 Author: Rob Voigt
 Author-email: code@ravoigt.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

