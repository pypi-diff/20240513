# Comparing `tmp/gimme_aws_creds-2.8.1.1.tar.gz` & `tmp/gimme_aws_creds-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimme_aws_creds-2.8.1.1.tar", last modified: Wed Apr 24 18:36:57 2024, max compression
+gzip compressed data, was "gimme_aws_creds-2.8.2.tar", last modified: Mon May 13 17:38:45 2024, max compression
```

## Comparing `gimme_aws_creds-2.8.1.1.tar` & `gimme_aws_creds-2.8.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/LONG_DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20414 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.716482 gimme_aws_creds-2.8.1.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      753 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds-autocomplete.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds.cmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.720482 gimme_aws_creds-2.8.1.1/gimme_aws_creds/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    31632 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/duo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/duo_universal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    38953 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    50285 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/okta_classic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/okta_identity_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/registered_authenticators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_aws_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_duo_universal_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    61157 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_okta_classic_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    70663 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_okta_identity_engine_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_registered_authenticators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:45.956298 gimme_aws_creds-2.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/LONG_DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-13 17:38:45.956298 gimme_aws_creds-2.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21013 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:45.952298 gimme_aws_creds-2.8.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      753 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/bin/gimme-aws-creds
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/bin/gimme-aws-creds-autocomplete.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/bin/gimme-aws-creds.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:45.952298 gimme_aws_creds-2.8.2/gimme_aws_creds/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31570 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/dummy_webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/duo_universal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39012 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50885 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/okta_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/okta_identity_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/registered_authenticators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/gimme_aws_creds/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:45.956298 gimme_aws_creds-2.8.2/gimme_aws_creds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-13 17:38:45.000000 gimme_aws_creds-2.8.2/gimme_aws_creds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-13 17:38:45.000000 gimme_aws_creds-2.8.2/gimme_aws_creds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:38:45.000000 gimme_aws_creds-2.8.2/gimme_aws_creds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-13 17:38:45.000000 gimme_aws_creds-2.8.2/gimme_aws_creds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 17:38:45.000000 gimme_aws_creds-2.8.2/gimme_aws_creds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 17:38:45.956298 gimme_aws_creds-2.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:45.956298 gimme_aws_creds-2.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/tests/test_aws_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/tests/test_duo_universal_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14237 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61157 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/tests/test_okta_classic_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70663 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/tests/test_okta_identity_engine_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-13 17:38:36.000000 gimme_aws_creds-2.8.2/tests/test_registered_authenticators.py
```

### Comparing `gimme_aws_creds-2.8.1.1/LICENSE` & `gimme_aws_creds-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/LONG_DESCRIPTION.md` & `gimme_aws_creds-2.8.2/LONG_DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/NOTICE` & `gimme_aws_creds-2.8.2/NOTICE`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/PKG-INFO` & `gimme_aws_creds-2.8.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimme_aws_creds
-Version: 2.8.1.1
+Version: 2.8.2
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -14,15 +14,15 @@
 License-File: NOTICE
 Requires-Dist: boto3<2.0.0,>=1.7.70
 Requires-Dist: beautifulsoup4<5.0.0,>=4.6.0
 Requires-Dist: keyring>=21.4.0
 Requires-Dist: requests<3.0.0,>=2.25.0
 Requires-Dist: fido2<0.10.0,>=0.9.1
 Requires-Dist: okta<3.0.0,>=2.9.0
-Requires-Dist: ctap-keyring-device==1.0.6
+Requires-Dist: ctap-keyring-device==1.0.6; (sys_platform == "win32" and python_version < "3.10") or sys_platform != "win32"
 Requires-Dist: pyjwt<3.0.0,>=2.4.0
 Requires-Dist: urllib3<2.0.0,>=1.26.0
 Requires-Dist: html5lib<2.0.0,>=1.1
 Requires-Dist: furl<3.0.0,>=2.1.3
 
 # Gimme AWS Creds
```

### Comparing `gimme_aws_creds-2.8.1.1/README.md` & `gimme_aws_creds-2.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 ## Prerequisites
 
 [Okta SAML integration to AWS using the AWS App](https://help.okta.com/en/prod/Content/Topics/Miscellaneous/References/OktaAWSMulti-AccountConfigurationGuide.pdf)
 
 Python 3.7+
 
+####  A Note on Python 3.10+ Compatibility on Windows
+
+`gimme-aws-creds` depends on the [ctap-keyring-device](https://pypi.org/project/ctap-keyring-device/) library for WebAuthn support.  All of the released versions of ctap-keyring-device require [winRT](https://pypi.org/project/winrt/) on Windows, which only works on Python 3.9 and lower and is no longer maintained. Until a version of ctap-keyring-device that supports `winSDK` (the replacement for winRT) is released to PyPi, or some other solution is found, WebAuthn support will not be available for people running Python 3.10+ on Windows.
+
 ### Optional
 
 [Gimme-creds-lambda](https://github.com/Nike-Inc/gimme-aws-creds/tree/master/lambda) can be used as a proxy to the Okta APIs needed by gimme-aws-creds.  This removes the requirement of an Okta API key.  Gimme-aws-creds authenticates to gimme-creds-lambda using OpenID Connect and the lambda handles all interactions with the Okta APIs.  Alternately, you can set the `OKTA_API_KEY` environment variable and the `gimme_creds_server` configuration value to 'internal' to call the Okta APIs directly from gimme-aws-creds.
 
 ## Installation
 
 This is a Python 3 project.
```

### Comparing `gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds` & `gimme_aws_creds-2.8.2/bin/gimme-aws-creds`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds-autocomplete.sh` & `gimme_aws_creds-2.8.2/bin/gimme-aws-creds-autocomplete.sh`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds.cmd` & `gimme_aws_creds-2.8.2/bin/gimme-aws-creds.cmd`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/aws.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/aws.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/common.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/common.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/config.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,31 +197,30 @@
     def _handle_config(self, config, profile_config, include_inherits = True):
         # Convert True/False strings to booleans
         for key in profile_config:
             if profile_config[key] == 'True':
                 profile_config[key] = True
             elif profile_config[key] == 'False':
                 profile_config[key] = False
-        
-        # Empty string in force_classic should be handled as True - this makes sure that migrating from Classic to OIE is seamless
-        if profile_config.get('force_classic') == '' or profile_config.get('force_classic') is None:
-            profile_config['force_classic'] = True
 
         if "inherits" in profile_config.keys() and include_inherits:
             self.ui.message("Using inherited config: " + profile_config["inherits"])
             if profile_config["inherits"] not in config:
                 raise errors.GimmeAWSCredsError(self.conf_profile + " inherits from " + profile_config["inherits"] + ", but could not find " + profile_config["inherits"])
-            combined_config = {
+            profile_config = {
                 **self._handle_config(config, dict(config[profile_config["inherits"]])),
                 **profile_config,
             }
-            del combined_config["inherits"]
-            return combined_config
-        else:
-            return profile_config
+            del profile_config["inherits"]
+
+        # Empty string in force_classic should be handled as True - this makes sure that migrating from Classic to OIE is seamless
+        if profile_config.get('force_classic') == '' or profile_config.get('force_classic') is None:
+            profile_config['force_classic'] = True
+
+        return profile_config
 
     def get_config_dict(self, include_inherits = True):
         """returns the conf dict from the okta config file"""
         # Check to see if config file exists, if not complain and exit
         # If config file does exist return config dict from file
         if os.path.isfile(self.OKTA_CONFIG):
             config = configparser.ConfigParser()
```

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/default.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/default.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/duo.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/duo.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/duo_universal.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/duo_universal.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/errors.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/errors.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/main.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # For enumerating saml roles
 # standard imports
 import configparser
 import json
 import os
 import re
 import sys
+import platform
 import concurrent.futures
 
 # extras
 import boto3
 import requests
 from botocore.exceptions import ClientError
 from okta.api_client import APIClient
@@ -506,15 +507,15 @@
         if 'okta_platform' in self._cache:
             return self._cache['okta_platform']
 
         response = requests.get(
             self.okta_org_url + '/.well-known/okta-organization',
             headers={
                 'Accept': 'application/json',
-                'User-Agent': "gimme-aws-creds {}".format(version)
+                'User-Agent': "gimme-aws-creds {};{};{}".format(version, sys.platform, platform.python_version())
             },
             timeout=30
         )
 
         response_data = response.json()
 
         if response.status_code == 200:
@@ -814,24 +815,24 @@
             profile_name = naming_data['role']
         elif cred_profile.lower() == 'acc':
             profile_name = self._get_account_name(naming_data['account'], role, resolve_alias)
         elif cred_profile.lower() == 'acc-role':
             account = self._get_account_name(naming_data['account'], role, resolve_alias)
             role_name = naming_data['role']
             path = naming_data['path']
-            if include_path == 'True':
+            if include_path is True:
                 role_name = ''.join([path, role_name])
             profile_name = '-'.join([account,
                                      role_name])
         else:
             profile_name = cred_profile
         return profile_name
 
     def _get_account_name(self, account, role, resolve_alias):
-        if resolve_alias == "False":
+        if resolve_alias is False:
             return account
         account_alias = self._get_alias_from_friendly_name(role.friendly_account_name)
         return account_alias or account
 
     def iter_selected_aws_credentials(self):
         results = []
         aws_results = []
```

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/okta_classic.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/okta_classic.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
       http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and* limitations under the License.*
 """
 import base64
+import sys
+import platform
 import copy
 import re
 import socket
 import time
 import uuid
 import webbrowser
 from codecs import decode
@@ -26,21 +28,28 @@
 from bs4 import BeautifulSoup
 from fido2.utils import websafe_decode
 from keyring.backends.fail import Keyring as FailKeyring
 from keyring.errors import PasswordDeleteError
 from requests.adapters import HTTPAdapter, Retry
 
 from gimme_aws_creds.u2f import FactorU2F
-from gimme_aws_creds.webauthn import WebAuthnClient, FakeAssertion
+
+# avoid importing ctap-keyring-device on Windows until it supports Python 3.10+
+if sys.platform == "win32" and sys.version_info >= (3, 10):
+    from gimme_aws_creds.dummy_webauthn import WebAuthnClient, FakeAssertion
+else:
+    from gimme_aws_creds.webauthn import WebAuthnClient, FakeAssertion
+
 from . import errors, ui, version, duo
 from .duo_universal import OktaDuoUniversal
 from .errors import GimmeAWSCredsMFAEnrollStatus
 from .registered_authenticators import RegisteredAuthenticators
 
 
+
 class OktaClassicClient(object):
     """
        The Okta Client Class performs the necessary API
        calls to an Okta Classic domain to get temporary AWS credentials.
     """
 
     KEYRING_SERVICE = 'gimme-aws-creds'
@@ -280,15 +289,15 @@
 
         return tokens
 
     @staticmethod
     def _get_headers():
         """sets the default headers"""
         headers = {
-            'User-Agent': "gimme-aws-creds {}".format(version),
+            'User-Agent': "gimme-aws-creds {};{};{}".format(version, sys.platform, platform.python_version()),
             'Accept': 'application/json',
             'Content-Type': 'application/json',
         }
         return headers
 
     def _get_initial_flow_state(self, embed_link, state_token=None):
         """ Starts the authentication flow with Okta"""
@@ -618,15 +627,19 @@
         elif factor['factorType'] == 'token':
             return self._login_input_mfa_challenge(state_token, factor['_links']['verify']['href'])
         elif factor['factorType'] == 'push':
             return self._login_send_push(state_token, factor)
         elif factor['factorType'] == 'u2f':
             return self._login_input_webauthn_challenge(state_token, factor)
         elif factor['factorType'] == 'webauthn':
-            return self._login_input_webauthn_challenge(state_token, factor)
+            # Block webauthn until ctap-kering-device is updated to support Python 3.10+ on Windows
+            if sys.platform == "win32" and sys.version_info >= (3, 10):
+                raise errors.GimmeAWSCredsError("WebAuthn devices not supported on this platform", 2)
+            else:
+                return self._login_input_webauthn_challenge(state_token, factor)
         elif factor['factorType'] == 'token:hardware':
             return self._login_input_mfa_challenge(state_token, factor['_links']['verify']['href'])
         elif factor['factorType'] == 'claims_provider':
             return self._login_duo_universal(state_token, factor)
 
     def _login_input_mfa_challenge(self, state_token, next_url):
         """ Submit verification code for SMS or TOTP authentication methods"""
```

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/okta_identity_engine.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/okta_identity_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and* limitations under the License.*
 """
+import sys
+import platform
 import time
 import webbrowser
 import jwt
 import requests
 from bs4 import BeautifulSoup
 from requests.adapters import HTTPAdapter, Retry
 
@@ -196,15 +198,15 @@
         
         return {'SAMLResponse': saml_response, 'RelayState': relay_state, 'TargetUrl': form_action}
 
     @staticmethod
     def _get_headers():
         """sets the default headers"""
         headers = {
-            'User-Agent': "gimme-aws-creds {}".format(version),
+            'User-Agent': "gimme-aws-creds {};{};{}".format(version, sys.platform, platform.python_version()),
             'Accept': 'application/json'
         }
         return headers
     
     def check_kwargs(self, kwargs):
         if self._use_oauth_access_token is True:
             if 'headers' not in kwargs:
```

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/registered_authenticators.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/registered_authenticators.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/u2f.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/u2f.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/ui.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/ui.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds/webauthn.py` & `gimme_aws_creds-2.8.2/gimme_aws_creds/webauthn.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/PKG-INFO` & `gimme_aws_creds-2.8.2/gimme_aws_creds.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimme_aws_creds
-Version: 2.8.1.1
+Version: 2.8.2
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -14,15 +14,15 @@
 License-File: NOTICE
 Requires-Dist: boto3<2.0.0,>=1.7.70
 Requires-Dist: beautifulsoup4<5.0.0,>=4.6.0
 Requires-Dist: keyring>=21.4.0
 Requires-Dist: requests<3.0.0,>=2.25.0
 Requires-Dist: fido2<0.10.0,>=0.9.1
 Requires-Dist: okta<3.0.0,>=2.9.0
-Requires-Dist: ctap-keyring-device==1.0.6
+Requires-Dist: ctap-keyring-device==1.0.6; (sys_platform == "win32" and python_version < "3.10") or sys_platform != "win32"
 Requires-Dist: pyjwt<3.0.0,>=2.4.0
 Requires-Dist: urllib3<2.0.0,>=1.26.0
 Requires-Dist: html5lib<2.0.0,>=1.1
 Requires-Dist: furl<3.0.0,>=2.1.3
 
 # Gimme AWS Creds
```

### Comparing `gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/SOURCES.txt` & `gimme_aws_creds-2.8.2/gimme_aws_creds.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 bin/gimme-aws-creds-autocomplete.sh
 bin/gimme-aws-creds.cmd
 gimme_aws_creds/__init__.py
 gimme_aws_creds/aws.py
 gimme_aws_creds/common.py
 gimme_aws_creds/config.py
 gimme_aws_creds/default.py
+gimme_aws_creds/dummy_webauthn.py
 gimme_aws_creds/duo.py
 gimme_aws_creds/duo_universal.py
 gimme_aws_creds/errors.py
 gimme_aws_creds/main.py
 gimme_aws_creds/okta_classic.py
 gimme_aws_creds/okta_identity_engine.py
 gimme_aws_creds/registered_authenticators.py
```

### Comparing `gimme_aws_creds-2.8.1.1/setup.py` & `gimme_aws_creds-2.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='gimme_aws_creds',
-    version='2.8.1.1',
+    version='2.8.2',
     install_requires=requirements,
     author='Eric Pierce',
     author_email='eric.pierce@nike.com',
     description="A CLI to get temporary AWS credentials from Okta",
     url='https://github.com/Nike-Inc/gimme-aws-creds',
     long_description=open("LONG_DESCRIPTION.md").read(),
     python_requires=">=3.7",
```

### Comparing `gimme_aws_creds-2.8.1.1/tests/test_aws_resolver.py` & `gimme_aws_creds-2.8.2/tests/test_aws_resolver.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/tests/test_config.py` & `gimme_aws_creds-2.8.2/tests/test_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,14 +118,43 @@
         self.assertEqual(profile_config, {
             "client_id": "foo",
             "aws_appname": "baz",
             "aws_rolename": "myrole",
             "force_classic": True
         })
 
+    def test_read_nested_config_inherited_no_force_classic(self):
+        """Test to make sure getting config works when inherited"""
+        test_ui = MockUserInterface(argv = [
+            "--profile",
+            "myprofile",
+        ])
+        with open(test_ui.HOME + "/.okta_aws_login_config", "w") as config_file:
+            config_file.write("""
+[mybase-level1]
+client_id = bar
+[mybase-level2]
+inherits = mybase-level1
+aws_appname = baz
+force_classic = False
+[myprofile]
+inherits = mybase-level2
+client_id = foo
+aws_rolename = myrole
+""")
+        config = Config(gac_ui=test_ui, create_config=False)
+        config.conf_profile = "myprofile"
+        profile_config = config.get_config_dict()
+        self.assertEqual(profile_config, {
+            "client_id": "foo",
+            "aws_appname": "baz",
+            "aws_rolename": "myrole",
+            "force_classic": False
+        })
+
     def test_fail_if_profile_not_found(self):
         """Test to make sure missing Default fails properly"""
         test_ui = MockUserInterface(argv=[])
         with open(test_ui.HOME + "/.okta_aws_login_config", "w") as config_file:
             config_file.write("""
         [myprofile]
         client_id = foo
```

### Comparing `gimme_aws_creds-2.8.1.1/tests/test_duo_universal_client.py` & `gimme_aws_creds-2.8.2/tests/test_duo_universal_client.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/tests/test_main.py` & `gimme_aws_creds-2.8.2/tests/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -193,108 +193,108 @@
         creds = GimmeAWSCreds()
         naming_data = {'account': '123456789012', 'role': 'administrator', 'path': '/administrator/'}
         role = RoleSet(idp='arn:aws:iam::123456789012:saml-provider/my-okta-provider',
                        role='arn:aws:iam::123456789012:role/administrator/administrator',
                        friendly_account_name='Account: my-org-master (123456789012)',
                        friendly_role_name='administrator/administrator')
         cred_profile = 'acc-role'
-        resolve_alias = 'True'
-        include_path = 'False'
+        resolve_alias = True
+        include_path = False
         self.assertEqual(creds.get_profile_name(cred_profile, include_path, naming_data, resolve_alias, role), "my-org-master-administrator")
 
     def test_get_profile_accrole_name_do_not_resolve_alias_do_not_include_paths(self):
         "Testing the acc-role, without alias resolution, and not including full role path"
         creds = GimmeAWSCreds()
         naming_data = {'account': '123456789012', 'role': 'administrator', 'path': '/administrator/'}
         role = RoleSet(idp='arn:aws:iam::123456789012:saml-provider/my-okta-provider',
                        role='arn:aws:iam::123456789012:role/administrator/administrator',
                        friendly_account_name='Account: my-org-master (123456789012)',
                        friendly_role_name='administrator/administrator')
         cred_profile = 'acc-role'
-        resolve_alias = 'False'
-        include_path = 'False'
+        resolve_alias = False
+        include_path = False
         self.assertEqual(creds.get_profile_name(cred_profile, include_path, naming_data, resolve_alias, role),
                          "123456789012-administrator")
 
     def test_get_profile_accrole_name_do_not_resolve_alias_include_paths(self):
         "Testing the acc-role, without alias resolution, and including full role path"
         creds = GimmeAWSCreds()
         naming_data = {'account': '123456789012', 'role': 'administrator', 'path': '/some/long/extended/path/'}
         role = RoleSet(idp='arn:aws:iam::123456789012:saml-provider/my-okta-provider',
                        role='arn:aws:iam::123456789012:role/some/long/extended/path/administrator',
                        friendly_account_name='Account: my-org-master (123456789012)',
                        friendly_role_name='administrator/administrator')
         cred_profile = 'acc-role'
-        resolve_alias = 'False'
-        include_path = 'True'
+        resolve_alias = False
+        include_path = True
         self.assertEqual(creds.get_profile_name(cred_profile, include_path, naming_data, resolve_alias, role),
                          "123456789012-/some/long/extended/path/administrator")
 
     def test_get_profile_name_role(self):
         "Testing the role"
         creds = GimmeAWSCreds()
         naming_data = {'account': '123456789012', 'role': 'administrator', 'path': '/some/long/extended/path/'}
         role = RoleSet(idp='arn:aws:iam::123456789012:saml-provider/my-okta-provider',
                        role='arn:aws:iam::123456789012:role/some/long/extended/path/administrator',
                        friendly_account_name='Account: my-org-master (123456789012)',
                        friendly_role_name='administrator/administrator')
         cred_profile = 'role'
-        resolve_alias = 'False'
-        include_path = 'True'
+        resolve_alias = False
+        include_path = True
         self.assertEqual(creds.get_profile_name(cred_profile, include_path, naming_data, resolve_alias, role),
                          'administrator')
 
     def test_get_profile_name_account_resolve_alias(self):
         "Testing the account with alias resolution"
         creds = GimmeAWSCreds()
         naming_data = {'account': '123456789012', 'role': 'administrator', 'path': '/administrator/'}
         role = RoleSet(idp='arn:aws:iam::123456789012:saml-provider/my-okta-provider',
                        role='arn:aws:iam::123456789012:role/administrator/administrator',
                        friendly_account_name='Account: my-org-master (123456789012)',
                        friendly_role_name='administrator/administrator')
         cred_profile = 'acc'
-        resolve_alias = 'True'
-        include_path = 'True'
+        resolve_alias = True
+        include_path = True
         self.assertEqual(creds.get_profile_name(cred_profile, include_path, naming_data, resolve_alias, role),
                          'my-org-master')
 
     def test_get_profile_name_account_do_not_resolve_alias(self):
         "Testing the account without alias resolution"
         creds = GimmeAWSCreds()
         naming_data = {'account': '123456789012', 'role': 'administrator', 'path': '/administrator/'}
         role = RoleSet(idp='arn:aws:iam::123456789012:saml-provider/my-okta-provider',
                        role='arn:aws:iam::123456789012:role/administrator/administrator',
                        friendly_account_name='Account: my-org-master (123456789012)',
                        friendly_role_name='administrator/administrator')
         cred_profile = 'acc'
-        resolve_alias = 'False'
-        include_path = 'True'
+        resolve_alias = False
+        include_path = True
         self.assertEqual(creds.get_profile_name(cred_profile, include_path, naming_data, resolve_alias, role),
                          '123456789012')
 
     def test_get_profile_name_default(self):
         "Testing the default"
         creds = GimmeAWSCreds()
         naming_data = {'account': '123456789012', 'role': 'administrator', 'path': '/some/long/extended/path/'}
         role = RoleSet(idp='arn:aws:iam::123456789012:saml-provider/my-okta-provider',
                        role='arn:aws:iam::123456789012:role/some/long/extended/path/administrator',
                        friendly_account_name='Account: my-org-master (123456789012)',
                        friendly_role_name='administrator/administrator')
         cred_profile = 'default'
-        resolve_alias = 'False'
-        include_path = 'True'
+        resolve_alias = False
+        include_path = True
         self.assertEqual(creds.get_profile_name(cred_profile, include_path, naming_data, resolve_alias, role),
                          'default')
 
     def test_get_profile_name_else(self):
         "testing else statement in get_profile_name"
         creds = GimmeAWSCreds()
         naming_data = {'account': '123456789012', 'role': 'administrator', 'path': '/some/long/extended/path/'}
         role = RoleSet(idp='arn:aws:iam::123456789012:saml-provider/my-okta-provider',
                        role='arn:aws:iam::123456789012:role/some/long/extended/path/administrator',
                        friendly_account_name='Account: my-org-master (123456789012)',
                        friendly_role_name='administrator/administrator')
         cred_profile = 'foo'
-        resolve_alias = 'False'
-        include_path = 'True'
+        resolve_alias = False
+        include_path = True
         self.assertEqual(creds.get_profile_name(cred_profile, include_path, naming_data, resolve_alias, role),
                          'foo')
```

### Comparing `gimme_aws_creds-2.8.1.1/tests/test_okta_classic_client.py` & `gimme_aws_creds-2.8.2/tests/test_okta_classic_client.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/tests/test_okta_identity_engine_client.py` & `gimme_aws_creds-2.8.2/tests/test_okta_identity_engine_client.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1.1/tests/test_registered_authenticators.py` & `gimme_aws_creds-2.8.2/tests/test_registered_authenticators.py`

 * *Files identical despite different names*

