# Comparing `tmp/synapse_token_authenticator-0.4.5.tar.gz` & `tmp/synapse_token_authenticator-0.4.6.tar.gz`

## Comparing `synapse_token_authenticator-0.4.5.tar` & `synapse_token_authenticator-0.4.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/CHANGELOG.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/CODEOWNERS
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/cliff.toml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.github/CODEOWNERS
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.github/workflows/main.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.github/workflows/python.yml
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/synapse_token_authenticator/__init__.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/synapse_token_authenticator/config.py
--rw-r--r--   0        0        0    10012 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/synapse_token_authenticator/token_authenticator.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/synapse_token_authenticator/utils.py
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/server.py
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_jwt.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_oidc.py
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/unittest.py
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/utils.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_utils/html_parsers.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/tests/test_utils/logging_setup.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/.gitignore
--rw-r--r--   0        0        0    34468 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/LICENSE
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/README.md
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/CHANGELOG.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/CODEOWNERS
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/cliff.toml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.github/CODEOWNERS
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.github/workflows/python.yml
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/synapse_token_authenticator/__init__.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/synapse_token_authenticator/config.py
+-rw-r--r--   0        0        0    13575 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/synapse_token_authenticator/token_authenticator.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/synapse_token_authenticator/utils.py
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/__init__.py
+-rw-r--r--   0        0        0    13774 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/server.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_custom.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_jwt.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_oidc.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/unittest.py
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/utils.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_utils/html_parsers.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_utils/logging_setup.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.gitignore
+-rw-r--r--   0        0        0    34468 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/LICENSE
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/README.md
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/PKG-INFO
```

### Comparing `synapse_token_authenticator-0.4.5/CHANGELOG.md` & `synapse_token_authenticator-0.4.6/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.4.6] - 2024-05-06
+
+### Features
+
+- Add custom jwt flow
+
 ## [0.4.5] - 2024-04-25
 
 ### Continuous Integration Pipeline
 
 - Bump pypi publish action
 
 ## [0.4.4] - 2024-04-24
```

### Comparing `synapse_token_authenticator-0.4.5/cliff.toml` & `synapse_token_authenticator-0.4.6/cliff.toml`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/.github/workflows/publish.yml` & `synapse_token_authenticator-0.4.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/.github/workflows/python.yml` & `synapse_token_authenticator-0.4.6/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/synapse_token_authenticator/config.py` & `synapse_token_authenticator-0.4.6/synapse_token_authenticator/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                     self.algorithm: str = other.get("algorithm", "HS512")
                     self.allow_registration: bool = other.get(
                         "allow_registration", False
                     )
                     self.require_expiry: bool = other.get("require_expiry", True)
 
             self.jwt = JwtConfig(jwt)
-            self.verify_jwt()
+            verify_jwt_based_cfg(self.jwt)
 
         if oidc := other.get("oidc"):
 
             class OIDCConfig:
                 def __init__(self, other: dict):
                     try:
                         self.issuer: str = other["issuer"]
@@ -42,29 +42,49 @@
 
                     self.allow_registration: bool = other.get(
                         "allow_registration", False
                     )
 
             self.oidc = OIDCConfig(oidc)
 
-    def verify_jwt(self):
-        if self.jwt.secret is None and self.jwt.keyfile is None:
-            raise Exception("Missing secret or keyfile")
-        if self.jwt.keyfile is not None and not os.path.exists(self.jwt.keyfile):
-            raise Exception("Keyfile doesn't exist")
-
-        if self.jwt.algorithm not in [
-            "HS256",
-            "HS384",
-            "HS512",
-            "RS256",
-            "RS384",
-            "RS512",
-            "ES256",
-            "ES384",
-            "ES512",
-            "PS256",
-            "PS384",
-            "PS512",
-            "EdDSA",
-        ]:
-            raise Exception(f"Unknown algorithm: '{self.jwt.algorithm}'")
+        if custom_flow := other.get("custom_flow"):
+
+            class CustomFlowConfig:
+                def __init__(self, other: dict):
+                    self.secret: str | None = other.get("secret")
+                    self.keyfile: str | None = other.get("keyfile")
+
+                    self.algorithm: str = other.get("algorithm", "RS256")
+                    self.require_expiry: bool = other.get("require_expiry", True)
+                    self.notify_on_registration_uri: str = other.get(
+                        "notify_on_registration_uri"
+                    )
+                    self.notification_access_token: str | None = other.get(
+                        "notification_access_token", None
+                    )
+
+            self.custom_flow = CustomFlowConfig(custom_flow)
+            verify_jwt_based_cfg(self.custom_flow)
+
+
+def verify_jwt_based_cfg(cfg):
+    if cfg.secret is None and cfg.keyfile is None:
+        raise Exception("Missing secret or keyfile")
+    if cfg.keyfile is not None and not os.path.exists(cfg.keyfile):
+        raise Exception("Keyfile doesn't exist")
+
+    if cfg.algorithm not in [
+        "HS256",
+        "HS384",
+        "HS512",
+        "RS256",
+        "RS384",
+        "RS512",
+        "ES256",
+        "ES384",
+        "ES512",
+        "PS256",
+        "PS384",
+        "PS512",
+        "EdDSA",
+    ]:
+        raise Exception(f"Unknown algorithm: '{cfg.algorithm}'")
```

### Comparing `synapse_token_authenticator-0.4.5/synapse_token_authenticator/token_authenticator.py` & `synapse_token_authenticator-0.4.6/synapse_token_authenticator/token_authenticator.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 class TokenAuthenticator:
     __version__ = "0.0.0"
 
-    def __init__(self, config: dict, api: ModuleApi):
-        self.api = api
+    def __init__(self, config: dict, account_handler: ModuleApi):
+        self.api = account_handler
 
         auth_checkers = {}
 
         self.config: TokenAuthenticatorConfig = config
         if (jwt := getattr(self.config, "jwt", None)) is not None:
             if jwt.secret:
                 k = {
@@ -63,14 +63,30 @@
             )
 
             self.api.register_web_resource(
                 "/_famedly/login/com.famedly.login.token.oidc",
                 self.LoginMetadataResource(oidc),
             )
 
+        if (custom_flow := getattr(self.config, "custom_flow", None)) is not None:
+            if custom_flow.secret:
+                k = {
+                    "k": base64.urlsafe_b64encode(
+                        custom_flow.secret.encode("utf-8")
+                    ).decode("utf-8"),
+                    "kty": "oct",
+                }
+                self.custom_flow_key = jwk.JWK(**k)
+            else:
+                with open(custom_flow.keyfile) as f:
+                    self.key = jwk.JWK.from_pem(f.read())
+            auth_checkers[("com.famedly.login.token.custom", ("token",))] = (
+                self.check_custom_flow
+            )
+
         self.api.register_password_auth_provider_callbacks(auth_checkers=auth_checkers)
 
     class LoginMetadataResource(resource.Resource):
         def __init__(self, oidc_config: object):
             self.issuer = oidc_config.issuer
             self.metadata_url = urljoin(
                 oidc_config.issuer, "/.well-known/openid-configuration"
@@ -266,10 +282,92 @@
             await self.api.register_user(user_id.localpart)
 
         user_id_str = self.api.get_qualified_user_id(username)
 
         logger.info("All done and valid, logging in!")
         return (user_id_str, None)
 
+    async def check_custom_flow(
+        self, username: str, login_type: str, login_dict: "synapse.module_api.JsonDict"
+    ) -> Optional[
+        tuple[
+            str,
+            Optional[Callable[["synapse.module_api.LoginResponse"], Awaitable[None]]],
+        ]
+    ]:
+        logger.info("Receiving auth request")
+        if login_type != "com.famedly.login.token.custom":
+            logger.info("Wrong login type")
+            return None
+        if "token" not in login_dict:
+            logger.info("Missing token")
+            return None
+        token = login_dict["token"]
+
+        check_claims = {}
+
+        user_id_str = self.api.get_qualified_user_id(username)
+        check_claims["urn:messaging:matrix:localpart"] = username
+        check_claims["urn:messaging:matrix:mxid"] = user_id_str
+
+        if self.config.custom_flow.require_expiry:
+            check_claims["exp"] = None
+        try:
+            token = jwt.JWT(
+                jwt=token,
+                key=self.custom_flow_key,
+                check_claims=check_claims,
+                algs=[self.config.custom_flow.algorithm],
+            )
+        except ValueError as e:
+            logger.info("Unrecognized token %s", e)
+            return None
+        except JWException as e:
+            logger.info("Invalid token %s", e)
+            return None
+        payload = json_decode(token.claims)
+        sub = payload["sub"]
+        if not isinstance(sub, str):
+            logger.info("user_id isn't a string")
+            return None
+
+        if "name" not in payload:
+            logger.info("No name claim in payload")
+            return None
+
+        user_id = UserID.from_string(user_id_str)
+        user_exists = await self.api.check_user_exists(user_id_str)
+
+        if not user_exists:
+            logger.info("User doesn't exist, registering them...")
+            await self.api.register_user(user_id.localpart)
+
+            # notification_access_token
+            headers = {}
+            if self.config.custom_flow.notification_access_token is not None:
+                headers = {
+                    b"Authorization": [
+                        b"Bearer " + self.config.custom_flow.notification_access_token
+                    ]
+                }
+
+            await self.api.http_client.post_json_get_json(
+                self.config.custom_flow.notify_on_registration_uri,
+                {"token": login_dict["token"]},
+                headers=headers,
+            )
+
+            logger.info("Registered user %s (%s)", user_id, payload["name"])
+
+        await self.api._hs.get_profile_handler().set_displayname(
+            requester=synapse.types.create_requester(user_id),
+            target_user=user_id,
+            by_admin=True,
+            new_displayname=payload["name"],
+        )
+
+        logger.info("All done and valid, logging in!")
+        return (user_id_str, None)
+
     @staticmethod
     def parse_config(config: dict):
         return TokenAuthenticatorConfig(config)
```

### Comparing `synapse_token_authenticator-0.4.5/synapse_token_authenticator/utils.py` & `synapse_token_authenticator-0.4.6/synapse_token_authenticator/utils.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/tests/__init__.py` & `synapse_token_authenticator-0.4.6/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,41 +42,44 @@
 
         async def register_user(
             localpart: str,
             admin: bool = False,
         ):
             return "@alice:example.test"
 
-        cls._patcher1 = patch(
-            "synapse.module_api.ModuleApi.set_user_admin",
-            new=AsyncMock(side_effect=set_user_admin),
-        )
-        cls._patcher2 = patch(
-            "synapse.module_api.ModuleApi.is_user_admin",
-            new=AsyncMock(side_effect=is_user_admin),
-        )
-        cls._patcher3 = patch(
-            "synapse.module_api.ModuleApi.check_user_exists",
-            new=AsyncMock(return_value=True),
-        )
-        cls._patcher4 = patch(
-            "synapse.module_api.ModuleApi.register_user",
-            new=AsyncMock(side_effect=register_user),
-        )
-        cls._patcher1.start()
-        cls._patcher2.start()
-        cls._patcher3.start()
-        cls._patcher4.start()
+        cls.patchers = [
+            patch(
+                "synapse.module_api.ModuleApi.set_user_admin",
+                new=AsyncMock(side_effect=set_user_admin),
+            ),
+            patch(
+                "synapse.module_api.ModuleApi.is_user_admin",
+                new=AsyncMock(side_effect=is_user_admin),
+            ),
+            patch(
+                "synapse.module_api.ModuleApi.check_user_exists",
+                new=AsyncMock(return_value=True),
+            ),
+            patch(
+                "synapse.module_api.ModuleApi.register_user",
+                new=AsyncMock(side_effect=register_user),
+            ),
+            patch(
+                "synapse.handlers.profile.ProfileHandler.set_displayname",
+                new=AsyncMock(return_value=None),
+            ),
+        ]
+
+        for patcher in cls.patchers:
+            patcher.start()
 
     @classmethod
     def tearDownClass(cls):
-        cls._patcher1.stop()
-        cls._patcher2.stop()
-        cls._patcher3.stop()
-        cls._patcher4.stop()
+        for patcher in cls.patchers:
+            patcher.stop()
 
     # Ignore ARG001
     @override
     def prepare(
         self, reactor: MemoryReactor, clock: Clock, homeserver: HomeServer
     ) -> None:
         self.store = homeserver.get_datastores().main
@@ -100,14 +103,19 @@
         conf["server_name"] = "example.test"
         if "modules" not in conf:
             conf["modules"] = [
                 {
                     "module": "synapse_token_authenticator.TokenAuthenticator",
                     "config": {
                         "jwt": {"secret": "foxies"},
+                        "custom_flow": {
+                            "algorithm": "HS512",
+                            "secret": "foxies",
+                            "notify_on_registration_uri": "http://example.test",
+                        },
                         "oidc": {
                             "issuer": "https://idp.example.test",
                             "client_id": "1111@project",
                             "client_secret": "2222@project",
                             "project_id": "231872387283",
                             "organization_id": "2283783782778",
                         },
```

### Comparing `synapse_token_authenticator-0.4.5/tests/server.py` & `synapse_token_authenticator-0.4.6/tests/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
     # Make the threadpool and database transactions synchronous for testing.
     _make_test_homeserver_synchronous(hs)
 
     # Load any configured modules into the homeserver
     module_api = hs.get_module_api()
     for module, module_config in hs.config.modules.loaded_modules:
-        hs.mockmod = module(config=module_config, api=module_api)
+        hs.mockmod = module(module_config, module_api)
         logger.debug("Loaded module %s %r", module, module_config)
 
     load_legacy_spam_checkers(hs)
     load_legacy_third_party_event_rules(hs)
     load_legacy_presence_router(hs)
     load_legacy_password_auth_providers(hs)
```

### Comparing `synapse_token_authenticator-0.4.5/tests/test_jwt.py` & `synapse_token_authenticator-0.4.6/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/tests/test_oidc.py` & `synapse_token_authenticator-0.4.6/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/tests/unittest.py` & `synapse_token_authenticator-0.4.6/tests/unittest.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/tests/utils.py` & `synapse_token_authenticator-0.4.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/tests/test_utils/__init__.py` & `synapse_token_authenticator-0.4.6/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/tests/test_utils/html_parsers.py` & `synapse_token_authenticator-0.4.6/tests/test_utils/html_parsers.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/tests/test_utils/logging_setup.py` & `synapse_token_authenticator-0.4.6/tests/test_utils/logging_setup.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/LICENSE` & `synapse_token_authenticator-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.5/pyproject.toml` & `synapse_token_authenticator-0.4.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["jwcrypto", "twisted"]
-version = "0.4.5"
+version = "0.4.6"
 
 [project.urls]
 Documentation = "https://github.com/famedly/synapse-token-authenticator"
 Issues = "https://github.com/famedly/synapse-token-authenticator/issues"
 Source = "https://github.com/famedly/synapse-token-authenticator"
 
 [tool.hatch.envs.default]
```

