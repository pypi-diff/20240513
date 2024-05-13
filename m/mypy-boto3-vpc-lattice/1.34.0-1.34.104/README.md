# Comparing `tmp/mypy-boto3-vpc-lattice-1.34.0.tar.gz` & `tmp/mypy_boto3_vpc_lattice-1.34.104.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-vpc-lattice-1.34.0.tar", last modified: Wed Dec 13 21:24:04 2023, max compression
+gzip compressed data, was "mypy_boto3_vpc_lattice-1.34.104.tar", last modified: Mon May 13 19:18:07 2024, max compression
```

## Comparing `mypy-boto3-vpc-lattice-1.34.0.tar` & `mypy_boto3_vpc_lattice-1.34.104.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:04.823411 mypy-boto3-vpc-lattice-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2023-12-13 21:24:04.823411 mypy-boto3-vpc-lattice-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12588 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:04.823411 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38876 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38872 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2023-12-13 21:20:57.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    43061 2023-12-13 21:20:57.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43060 2023-12-13 21:20:57.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:04.823411 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2023-12-13 21:24:04.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-13 21:24:04.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:04.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:04.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:24:04.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 21:24:04.000000 mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:24:04.823411 mypy-boto3-vpc-lattice-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2023-12-13 21:20:56.000000 mypy-boto3-vpc-lattice-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:18:07.576499 mypy_boto3_vpc_lattice-1.34.104/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-13 19:18:07.576499 mypy_boto3_vpc_lattice-1.34.104/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:18:07.576499 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38962 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38959 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-13 19:17:55.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-13 19:17:55.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-05-13 19:17:55.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-05-13 19:17:55.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    44205 2024-05-13 19:17:55.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44205 2024-05-13 19:17:55.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:18:07.576499 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-13 19:18:07.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 19:18:07.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:18:07.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:18:07.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 19:18:07.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 19:18:07.000000 mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:18:07.576499 mypy_boto3_vpc_lattice-1.34.104/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-13 19:17:54.000000 mypy_boto3_vpc_lattice-1.34.104/setup.py
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/LICENSE` & `mypy_boto3_vpc_lattice-1.34.104/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/PKG-INFO` & `mypy_boto3_vpc_lattice-1.34.104/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.34.0
-Summary: Type annotations for boto3.VPCLattice 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.104
+Summary: Type annotations for boto3.VPCLattice 1.34.104 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-vpc-lattice"></a>
 
 # mypy-boto3-vpc-lattice
 
 [![PyPI - mypy-boto3-vpc-lattice](https://img.shields.io/pypi/v/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.34.104](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/README.md` & `mypy_boto3_vpc_lattice-1.34.104/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.34.104](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/__init__.py` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ListServicesPaginator,
     ListTargetGroupsPaginator,
     ListTargetsPaginator,
 )
 
 Client = VPCLatticeClient
 
-
 __all__ = (
     "Client",
     "ListAccessLogSubscriptionsPaginator",
     "ListListenersPaginator",
     "ListRulesPaginator",
     "ListServiceNetworkServiceAssociationsPaginator",
     "ListServiceNetworkVpcAssociationsPaginator",
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/__init__.pyi` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/client.py` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
-    RuleActionTypeDef,
-    RuleMatchTypeDef,
+    RuleActionUnionTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateServiceNetworkResponseTypeDef,
@@ -84,15 +84,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("VPCLatticeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -156,54 +155,54 @@
 
     def create_access_log_subscription(
         self,
         *,
         destinationArn: str,
         resourceIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAccessLogSubscriptionResponseTypeDef:
         """
         Enables access logs to be sent to Amazon CloudWatch, Amazon S3, and Amazon
         Kinesis Data
         Firehose.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_access_log_subscription)
         """
 
     def create_listener(
         self,
         *,
-        defaultAction: RuleActionTypeDef,
+        defaultAction: RuleActionUnionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateListenerResponseTypeDef:
         """
         Creates a listener for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_listener)
         """
 
     def create_rule(
         self,
         *,
-        action: RuleActionTypeDef,
+        action: RuleActionUnionTypeDef,
         listenerIdentifier: str,
-        match: RuleMatchTypeDef,
+        match: RuleMatchUnionTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a listener rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_rule)
         """
@@ -212,45 +211,45 @@
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         certificateArn: str = ...,
         clientToken: str = ...,
         customDomainName: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service)
         """
 
     def create_service_network(
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkResponseTypeDef:
         """
         Creates a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network)
         """
 
     def create_service_network_service_association(
         self,
         *,
         serviceIdentifier: str,
         serviceNetworkIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkServiceAssociationResponseTypeDef:
         """
         Associates a service with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_service_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network_service_association)
         """
@@ -258,15 +257,15 @@
     def create_service_network_vpc_association(
         self,
         *,
         serviceNetworkIdentifier: str,
         vpcIdentifier: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkVpcAssociationResponseTypeDef:
         """
         Associates a VPC with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network_vpc_association)
         """
@@ -274,15 +273,15 @@
     def create_target_group(
         self,
         *,
         name: str,
         type: TargetGroupTypeType,
         clientToken: str = ...,
         config: TargetGroupConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTargetGroupResponseTypeDef:
         """
         Creates a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_target_group)
         """
@@ -520,45 +519,45 @@
 
     def list_rules(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRulesResponseTypeDef:
         """
         Lists the rules for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_rules)
         """
 
     def list_service_network_service_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceIdentifier: str = ...,
-        serviceNetworkIdentifier: str = ...
+        serviceNetworkIdentifier: str = ...,
     ) -> ListServiceNetworkServiceAssociationsResponseTypeDef:
         """
         Lists the associations between the service network and the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_service_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_network_service_associations)
         """
 
     def list_service_network_vpc_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceNetworkIdentifier: str = ...,
-        vpcIdentifier: str = ...
+        vpcIdentifier: str = ...,
     ) -> ListServiceNetworkVpcAssociationsResponseTypeDef:
         """
         Lists the service network and VPC associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_vpc_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_network_vpc_associations)
         """
@@ -596,30 +595,30 @@
 
     def list_target_groups(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         targetGroupType: TargetGroupTypeType = ...,
-        vpcIdentifier: str = ...
+        vpcIdentifier: str = ...,
     ) -> ListTargetGroupsResponseTypeDef:
         """
         Lists your target groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_target_groups)
         """
 
     def list_targets(
         self,
         *,
         targetGroupIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        targets: Sequence[TargetTypeDef] = ...
+        targets: Sequence[TargetTypeDef] = ...,
     ) -> ListTargetsResponseTypeDef:
         """
         Lists the targets for the target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_targets)
         """
@@ -675,32 +674,36 @@
         Updates the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_access_log_subscription)
         """
 
     def update_listener(
-        self, *, defaultAction: RuleActionTypeDef, listenerIdentifier: str, serviceIdentifier: str
+        self,
+        *,
+        defaultAction: RuleActionUnionTypeDef,
+        listenerIdentifier: str,
+        serviceIdentifier: str,
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_listener)
         """
 
     def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: RuleActionTypeDef = ...,
-        match: RuleMatchTypeDef = ...,
-        priority: int = ...
+        action: RuleActionUnionTypeDef = ...,
+        match: RuleMatchUnionTypeDef = ...,
+        priority: int = ...,
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_rule)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/client.pyi` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
-    RuleActionTypeDef,
-    RuleMatchTypeDef,
+    RuleActionUnionTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateServiceNetworkResponseTypeDef,
@@ -152,54 +152,54 @@
 
     def create_access_log_subscription(
         self,
         *,
         destinationArn: str,
         resourceIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAccessLogSubscriptionResponseTypeDef:
         """
         Enables access logs to be sent to Amazon CloudWatch, Amazon S3, and Amazon
         Kinesis Data
         Firehose.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_access_log_subscription)
         """
 
     def create_listener(
         self,
         *,
-        defaultAction: RuleActionTypeDef,
+        defaultAction: RuleActionUnionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateListenerResponseTypeDef:
         """
         Creates a listener for a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_listener)
         """
 
     def create_rule(
         self,
         *,
-        action: RuleActionTypeDef,
+        action: RuleActionUnionTypeDef,
         listenerIdentifier: str,
-        match: RuleMatchTypeDef,
+        match: RuleMatchUnionTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a listener rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_rule)
         """
@@ -208,45 +208,45 @@
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         certificateArn: str = ...,
         clientToken: str = ...,
         customDomainName: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service)
         """
 
     def create_service_network(
         self,
         *,
         name: str,
         authType: AuthTypeType = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkResponseTypeDef:
         """
         Creates a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network)
         """
 
     def create_service_network_service_association(
         self,
         *,
         serviceIdentifier: str,
         serviceNetworkIdentifier: str,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkServiceAssociationResponseTypeDef:
         """
         Associates a service with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_service_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network_service_association)
         """
@@ -254,15 +254,15 @@
     def create_service_network_vpc_association(
         self,
         *,
         serviceNetworkIdentifier: str,
         vpcIdentifier: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateServiceNetworkVpcAssociationResponseTypeDef:
         """
         Associates a VPC with a service network.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_vpc_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_service_network_vpc_association)
         """
@@ -270,15 +270,15 @@
     def create_target_group(
         self,
         *,
         name: str,
         type: TargetGroupTypeType,
         clientToken: str = ...,
         config: TargetGroupConfigTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateTargetGroupResponseTypeDef:
         """
         Creates a target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_target_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#create_target_group)
         """
@@ -516,45 +516,45 @@
 
     def list_rules(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRulesResponseTypeDef:
         """
         Lists the rules for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_rules)
         """
 
     def list_service_network_service_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceIdentifier: str = ...,
-        serviceNetworkIdentifier: str = ...
+        serviceNetworkIdentifier: str = ...,
     ) -> ListServiceNetworkServiceAssociationsResponseTypeDef:
         """
         Lists the associations between the service network and the service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_service_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_network_service_associations)
         """
 
     def list_service_network_vpc_associations(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         serviceNetworkIdentifier: str = ...,
-        vpcIdentifier: str = ...
+        vpcIdentifier: str = ...,
     ) -> ListServiceNetworkVpcAssociationsResponseTypeDef:
         """
         Lists the service network and VPC associations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_vpc_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_service_network_vpc_associations)
         """
@@ -592,30 +592,30 @@
 
     def list_target_groups(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
         targetGroupType: TargetGroupTypeType = ...,
-        vpcIdentifier: str = ...
+        vpcIdentifier: str = ...,
     ) -> ListTargetGroupsResponseTypeDef:
         """
         Lists your target groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_target_groups)
         """
 
     def list_targets(
         self,
         *,
         targetGroupIdentifier: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        targets: Sequence[TargetTypeDef] = ...
+        targets: Sequence[TargetTypeDef] = ...,
     ) -> ListTargetsResponseTypeDef:
         """
         Lists the targets for the target group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#list_targets)
         """
@@ -671,32 +671,36 @@
         Updates the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_access_log_subscription)
         """
 
     def update_listener(
-        self, *, defaultAction: RuleActionTypeDef, listenerIdentifier: str, serviceIdentifier: str
+        self,
+        *,
+        defaultAction: RuleActionUnionTypeDef,
+        listenerIdentifier: str,
+        serviceIdentifier: str,
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_listener)
         """
 
     def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: RuleActionTypeDef = ...,
-        match: RuleMatchTypeDef = ...,
-        priority: int = ...
+        action: RuleActionUnionTypeDef = ...,
+        match: RuleMatchUnionTypeDef = ...,
+        priority: int = ...,
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/client/#update_rule)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/literals.py` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthPolicyStateType",
     "AuthTypeType",
     "HealthCheckProtocolVersionType",
     "IpAddressTypeType",
     "LambdaEventStructureVersionType",
     "ListAccessLogSubscriptionsPaginatorName",
@@ -47,15 +46,14 @@
     "VPCLatticeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AuthPolicyStateType = Literal["Active", "Inactive"]
 AuthTypeType = Literal["AWS_IAM", "NONE"]
 HealthCheckProtocolVersionType = Literal["HTTP1", "HTTP2"]
 IpAddressTypeType = Literal["IPV4", "IPV6"]
 LambdaEventStructureVersionType = Literal["V1", "V2"]
 ListAccessLogSubscriptionsPaginatorName = Literal["list_access_log_subscriptions"]
 ListListenersPaginatorName = Literal["list_listeners"]
@@ -64,15 +62,15 @@
     "list_service_network_service_associations"
 ]
 ListServiceNetworkVpcAssociationsPaginatorName = Literal["list_service_network_vpc_associations"]
 ListServiceNetworksPaginatorName = Literal["list_service_networks"]
 ListServicesPaginatorName = Literal["list_services"]
 ListTargetGroupsPaginatorName = Literal["list_target_groups"]
 ListTargetsPaginatorName = Literal["list_targets"]
-ListenerProtocolType = Literal["HTTP", "HTTPS"]
+ListenerProtocolType = Literal["HTTP", "HTTPS", "TLS_PASSTHROUGH"]
 ServiceNetworkServiceAssociationStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATE_IN_PROGRESS", "DELETE_FAILED", "DELETE_IN_PROGRESS"
 ]
 ServiceNetworkVpcAssociationStatusType = Literal[
     "ACTIVE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
@@ -80,15 +78,15 @@
     "DELETE_IN_PROGRESS",
     "UPDATE_FAILED",
     "UPDATE_IN_PROGRESS",
 ]
 ServiceStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATE_IN_PROGRESS", "DELETE_FAILED", "DELETE_IN_PROGRESS"
 ]
-TargetGroupProtocolType = Literal["HTTP", "HTTPS"]
+TargetGroupProtocolType = Literal["HTTP", "HTTPS", "TCP"]
 TargetGroupProtocolVersionType = Literal["GRPC", "HTTP1", "HTTP2"]
 TargetGroupStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATE_IN_PROGRESS", "DELETE_FAILED", "DELETE_IN_PROGRESS"
 ]
 TargetGroupTypeType = Literal["ALB", "INSTANCE", "IP", "LAMBDA"]
 TargetStatusType = Literal["DRAINING", "HEALTHY", "INITIAL", "UNAVAILABLE", "UNHEALTHY", "UNUSED"]
 VPCLatticeServiceName = Literal["vpc-lattice"]
@@ -114,14 +112,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -132,14 +131,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -157,14 +157,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -177,24 +178,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -255,15 +258,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -335,17 +337,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -390,14 +394,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -435,19 +440,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -496,11 +503,12 @@
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
+    "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/literals.pyi` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     "list_service_network_service_associations"
 ]
 ListServiceNetworkVpcAssociationsPaginatorName = Literal["list_service_network_vpc_associations"]
 ListServiceNetworksPaginatorName = Literal["list_service_networks"]
 ListServicesPaginatorName = Literal["list_services"]
 ListTargetGroupsPaginatorName = Literal["list_target_groups"]
 ListTargetsPaginatorName = Literal["list_targets"]
-ListenerProtocolType = Literal["HTTP", "HTTPS"]
+ListenerProtocolType = Literal["HTTP", "HTTPS", "TLS_PASSTHROUGH"]
 ServiceNetworkServiceAssociationStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATE_IN_PROGRESS", "DELETE_FAILED", "DELETE_IN_PROGRESS"
 ]
 ServiceNetworkVpcAssociationStatusType = Literal[
     "ACTIVE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
@@ -78,15 +78,15 @@
     "DELETE_IN_PROGRESS",
     "UPDATE_FAILED",
     "UPDATE_IN_PROGRESS",
 ]
 ServiceStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATE_IN_PROGRESS", "DELETE_FAILED", "DELETE_IN_PROGRESS"
 ]
-TargetGroupProtocolType = Literal["HTTP", "HTTPS"]
+TargetGroupProtocolType = Literal["HTTP", "HTTPS", "TCP"]
 TargetGroupProtocolVersionType = Literal["GRPC", "HTTP1", "HTTP2"]
 TargetGroupStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATE_IN_PROGRESS", "DELETE_FAILED", "DELETE_IN_PROGRESS"
 ]
 TargetGroupTypeType = Literal["ALB", "INSTANCE", "IP", "LAMBDA"]
 TargetStatusType = Literal["DRAINING", "HEALTHY", "INITIAL", "UNAVAILABLE", "UNHEALTHY", "UNUSED"]
 VPCLatticeServiceName = Literal["vpc-lattice"]
@@ -112,14 +112,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -130,14 +131,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -155,14 +157,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -175,24 +178,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -253,15 +258,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -333,17 +337,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -388,14 +394,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -433,19 +440,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -494,11 +503,12 @@
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
+    "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/paginator.py` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     "ListServiceNetworkVpcAssociationsPaginator",
     "ListServiceNetworksPaginator",
     "ListServicesPaginator",
     "ListTargetGroupsPaginator",
     "ListTargetsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -115,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listrulespaginator)
         """
 
 
@@ -134,15 +133,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 
@@ -153,15 +152,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 
@@ -202,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 
@@ -221,13 +220,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/paginator.pyi` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listrulespaginator)
         """
 
 class ListServiceNetworkServiceAssociationsPaginator(Paginator):
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 class ListServiceNetworkVpcAssociationsPaginator(Paginator):
@@ -146,15 +146,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 class ListServiceNetworksPaginator(Paginator):
@@ -192,15 +192,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 class ListTargetsPaginator(Paginator):
@@ -210,13 +210,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/type_defs.py` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AccessLogSubscriptionSummaryTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthPolicyStateType,
     AuthTypeType,
     HealthCheckProtocolVersionType,
     IpAddressTypeType,
     LambdaEventStructureVersionType,
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessLogSubscriptionSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "RuleUpdateFailureTypeDef",
     "CreateAccessLogSubscriptionRequestRequestTypeDef",
     "CreateServiceNetworkRequestRequestTypeDef",
     "CreateServiceNetworkServiceAssociationRequestRequestTypeDef",
@@ -130,14 +129,15 @@
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
+    "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
     "HeaderMatchTypeDef",
     "HealthCheckConfigTypeDef",
     "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     "ListListenersRequestListListenersPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
@@ -151,35 +151,40 @@
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
+    "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
-    "CreateListenerRequestRequestTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
-    "UpdateListenerRequestRequestTypeDef",
     "UpdateListenerResponseTypeDef",
+    "CreateListenerRequestRequestTypeDef",
+    "RuleActionUnionTypeDef",
+    "UpdateListenerRequestRequestTypeDef",
     "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
+    "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
+    "UpdateRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
+    "RuleMatchUnionTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleResponseTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
     "AccessLogSubscriptionSummaryTypeDef",
     {
@@ -192,18 +197,18 @@
         "resourceId": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 RuleUpdateFailureTypeDef = TypedDict(
     "RuleUpdateFailureTypeDef",
     {
         "failureCode": NotRequired[str],
         "failureMessage": NotRequired[str],
@@ -986,14 +991,20 @@
     "RegisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ForwardActionOutputTypeDef = TypedDict(
+    "ForwardActionOutputTypeDef",
+    {
+        "targetGroups": List[WeightedTargetGroupTypeDef],
+    },
+)
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
     },
 )
 HeaderMatchTypeDef = TypedDict(
@@ -1154,14 +1165,21 @@
     "ListServicesResponseTypeDef",
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "fixedResponse": NotRequired[FixedResponseActionTypeDef],
+        "forward": NotRequired[ForwardActionOutputTypeDef],
+    },
+)
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": NotRequired[FixedResponseActionTypeDef],
         "forward": NotRequired[ForwardActionTypeDef],
     },
 )
@@ -1180,86 +1198,95 @@
 UpdateTargetGroupRequestRequestTypeDef = TypedDict(
     "UpdateTargetGroupRequestRequestTypeDef",
     {
         "healthCheck": HealthCheckConfigTypeDef,
         "targetGroupIdentifier": str,
     },
 )
-HttpMatchTypeDef = TypedDict(
-    "HttpMatchTypeDef",
+HttpMatchOutputTypeDef = TypedDict(
+    "HttpMatchOutputTypeDef",
     {
-        "headerMatches": NotRequired[Sequence[HeaderMatchTypeDef]],
+        "headerMatches": NotRequired[List[HeaderMatchTypeDef]],
         "method": NotRequired[str],
         "pathMatch": NotRequired[PathMatchTypeDef],
     },
 )
-CreateListenerRequestRequestTypeDef = TypedDict(
-    "CreateListenerRequestRequestTypeDef",
+HttpMatchTypeDef = TypedDict(
+    "HttpMatchTypeDef",
     {
-        "defaultAction": RuleActionTypeDef,
-        "name": str,
-        "protocol": ListenerProtocolType,
-        "serviceIdentifier": str,
-        "clientToken": NotRequired[str],
-        "port": NotRequired[int],
-        "tags": NotRequired[Mapping[str, str]],
+        "headerMatches": NotRequired[Sequence[HeaderMatchTypeDef]],
+        "method": NotRequired[str],
+        "pathMatch": NotRequired[PathMatchTypeDef],
     },
 )
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateListenerRequestRequestTypeDef = TypedDict(
-    "UpdateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateListenerRequestRequestTypeDef = TypedDict(
+    "CreateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "name": str,
+        "protocol": ListenerProtocolType,
+        "serviceIdentifier": str,
+        "clientToken": NotRequired[str],
+        "port": NotRequired[int],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
+UpdateListenerRequestRequestTypeDef = TypedDict(
+    "UpdateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
 CreateTargetGroupRequestRequestTypeDef = TypedDict(
     "CreateTargetGroupRequestRequestTypeDef",
     {
         "name": str,
         "type": TargetGroupTypeType,
         "clientToken": NotRequired[str],
         "config": NotRequired[TargetGroupConfigTypeDef],
@@ -1303,72 +1330,92 @@
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-RuleMatchTypeDef = TypedDict(
-    "RuleMatchTypeDef",
+RuleMatchOutputTypeDef = TypedDict(
+    "RuleMatchOutputTypeDef",
     {
-        "httpMatch": NotRequired[HttpMatchTypeDef],
+        "httpMatch": NotRequired[HttpMatchOutputTypeDef],
     },
 )
-CreateRuleRequestRequestTypeDef = TypedDict(
-    "CreateRuleRequestRequestTypeDef",
+RuleMatchTypeDef = TypedDict(
+    "RuleMatchTypeDef",
     {
-        "action": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "serviceIdentifier": str,
-        "clientToken": NotRequired[str],
-        "tags": NotRequired[Mapping[str, str]],
+        "httpMatch": NotRequired[HttpMatchTypeDef],
     },
 )
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
-        "action": NotRequired[RuleActionTypeDef],
+        "action": NotRequired[RuleActionOutputTypeDef],
         "arn": NotRequired[str],
         "id": NotRequired[str],
         "isDefault": NotRequired[bool],
-        "match": NotRequired[RuleMatchTypeDef],
+        "match": NotRequired[RuleMatchOutputTypeDef],
         "name": NotRequired[str],
         "priority": NotRequired[int],
     },
 )
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "action": RuleActionOutputTypeDef,
+        "arn": str,
+        "id": str,
+        "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateRuleRequestRequestTypeDef = TypedDict(
+    "CreateRuleRequestRequestTypeDef",
+    {
+        "action": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "match": RuleMatchTypeDef,
+        "name": str,
+        "priority": int,
+        "serviceIdentifier": str,
+        "clientToken": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+RuleMatchUnionTypeDef = Union[RuleMatchTypeDef, RuleMatchOutputTypeDef]
 RuleUpdateTypeDef = TypedDict(
     "RuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
         "action": NotRequired[RuleActionTypeDef],
         "match": NotRequired[RuleMatchTypeDef],
         "priority": NotRequired[int],
@@ -1381,27 +1428,14 @@
         "ruleIdentifier": str,
         "serviceIdentifier": str,
         "action": NotRequired[RuleActionTypeDef],
         "match": NotRequired[RuleMatchTypeDef],
         "priority": NotRequired[int],
     },
 )
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "arn": str,
-        "id": str,
-        "isDefault": bool,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice/type_defs.pyi` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AccessLogSubscriptionSummaryTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthPolicyStateType,
     AuthTypeType,
     HealthCheckProtocolVersionType,
     IpAddressTypeType,
     LambdaEventStructureVersionType,
@@ -129,14 +129,15 @@
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
+    "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
     "HeaderMatchTypeDef",
     "HealthCheckConfigTypeDef",
     "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     "ListListenersRequestListListenersPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
@@ -150,35 +151,40 @@
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
+    "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
-    "CreateListenerRequestRequestTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
-    "UpdateListenerRequestRequestTypeDef",
     "UpdateListenerResponseTypeDef",
+    "CreateListenerRequestRequestTypeDef",
+    "RuleActionUnionTypeDef",
+    "UpdateListenerRequestRequestTypeDef",
     "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
+    "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
+    "UpdateRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
+    "RuleMatchUnionTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleResponseTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
     "AccessLogSubscriptionSummaryTypeDef",
     {
@@ -191,18 +197,18 @@
         "resourceId": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 RuleUpdateFailureTypeDef = TypedDict(
     "RuleUpdateFailureTypeDef",
     {
         "failureCode": NotRequired[str],
         "failureMessage": NotRequired[str],
@@ -985,14 +991,20 @@
     "RegisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ForwardActionOutputTypeDef = TypedDict(
+    "ForwardActionOutputTypeDef",
+    {
+        "targetGroups": List[WeightedTargetGroupTypeDef],
+    },
+)
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
     },
 )
 HeaderMatchTypeDef = TypedDict(
@@ -1153,14 +1165,21 @@
     "ListServicesResponseTypeDef",
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "fixedResponse": NotRequired[FixedResponseActionTypeDef],
+        "forward": NotRequired[ForwardActionOutputTypeDef],
+    },
+)
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": NotRequired[FixedResponseActionTypeDef],
         "forward": NotRequired[ForwardActionTypeDef],
     },
 )
@@ -1179,86 +1198,95 @@
 UpdateTargetGroupRequestRequestTypeDef = TypedDict(
     "UpdateTargetGroupRequestRequestTypeDef",
     {
         "healthCheck": HealthCheckConfigTypeDef,
         "targetGroupIdentifier": str,
     },
 )
-HttpMatchTypeDef = TypedDict(
-    "HttpMatchTypeDef",
+HttpMatchOutputTypeDef = TypedDict(
+    "HttpMatchOutputTypeDef",
     {
-        "headerMatches": NotRequired[Sequence[HeaderMatchTypeDef]],
+        "headerMatches": NotRequired[List[HeaderMatchTypeDef]],
         "method": NotRequired[str],
         "pathMatch": NotRequired[PathMatchTypeDef],
     },
 )
-CreateListenerRequestRequestTypeDef = TypedDict(
-    "CreateListenerRequestRequestTypeDef",
+HttpMatchTypeDef = TypedDict(
+    "HttpMatchTypeDef",
     {
-        "defaultAction": RuleActionTypeDef,
-        "name": str,
-        "protocol": ListenerProtocolType,
-        "serviceIdentifier": str,
-        "clientToken": NotRequired[str],
-        "port": NotRequired[int],
-        "tags": NotRequired[Mapping[str, str]],
+        "headerMatches": NotRequired[Sequence[HeaderMatchTypeDef]],
+        "method": NotRequired[str],
+        "pathMatch": NotRequired[PathMatchTypeDef],
     },
 )
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateListenerRequestRequestTypeDef = TypedDict(
-    "UpdateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateListenerRequestRequestTypeDef = TypedDict(
+    "CreateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "name": str,
+        "protocol": ListenerProtocolType,
+        "serviceIdentifier": str,
+        "clientToken": NotRequired[str],
+        "port": NotRequired[int],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
+UpdateListenerRequestRequestTypeDef = TypedDict(
+    "UpdateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
 CreateTargetGroupRequestRequestTypeDef = TypedDict(
     "CreateTargetGroupRequestRequestTypeDef",
     {
         "name": str,
         "type": TargetGroupTypeType,
         "clientToken": NotRequired[str],
         "config": NotRequired[TargetGroupConfigTypeDef],
@@ -1302,72 +1330,92 @@
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-RuleMatchTypeDef = TypedDict(
-    "RuleMatchTypeDef",
+RuleMatchOutputTypeDef = TypedDict(
+    "RuleMatchOutputTypeDef",
     {
-        "httpMatch": NotRequired[HttpMatchTypeDef],
+        "httpMatch": NotRequired[HttpMatchOutputTypeDef],
     },
 )
-CreateRuleRequestRequestTypeDef = TypedDict(
-    "CreateRuleRequestRequestTypeDef",
+RuleMatchTypeDef = TypedDict(
+    "RuleMatchTypeDef",
     {
-        "action": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "serviceIdentifier": str,
-        "clientToken": NotRequired[str],
-        "tags": NotRequired[Mapping[str, str]],
+        "httpMatch": NotRequired[HttpMatchTypeDef],
     },
 )
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
-        "action": NotRequired[RuleActionTypeDef],
+        "action": NotRequired[RuleActionOutputTypeDef],
         "arn": NotRequired[str],
         "id": NotRequired[str],
         "isDefault": NotRequired[bool],
-        "match": NotRequired[RuleMatchTypeDef],
+        "match": NotRequired[RuleMatchOutputTypeDef],
         "name": NotRequired[str],
         "priority": NotRequired[int],
     },
 )
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "action": RuleActionOutputTypeDef,
+        "arn": str,
+        "id": str,
+        "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateRuleRequestRequestTypeDef = TypedDict(
+    "CreateRuleRequestRequestTypeDef",
+    {
+        "action": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "match": RuleMatchTypeDef,
+        "name": str,
+        "priority": int,
+        "serviceIdentifier": str,
+        "clientToken": NotRequired[str],
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+RuleMatchUnionTypeDef = Union[RuleMatchTypeDef, RuleMatchOutputTypeDef]
 RuleUpdateTypeDef = TypedDict(
     "RuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
         "action": NotRequired[RuleActionTypeDef],
         "match": NotRequired[RuleMatchTypeDef],
         "priority": NotRequired[int],
@@ -1380,27 +1428,14 @@
         "ruleIdentifier": str,
         "serviceIdentifier": str,
         "action": NotRequired[RuleActionTypeDef],
         "match": NotRequired[RuleMatchTypeDef],
         "priority": NotRequired[int],
     },
 )
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "arn": str,
-        "id": str,
-        "isDefault": bool,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice.egg-info/PKG-INFO` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-vpc-lattice
-Version: 1.34.0
-Summary: Type annotations for boto3.VPCLattice 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.104
+Summary: Type annotations for boto3.VPCLattice 1.34.104 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-vpc-lattice"></a>
 
 # mypy-boto3-vpc-lattice
 
 [![PyPI - mypy-boto3-vpc-lattice](https://img.shields.io/pypi/v/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-vpc-lattice.svg?color=blue)](https://pypi.org/project/mypy-boto3-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-vpc-lattice)](https://pepy.tech/project/mypy-boto3-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VPCLattice 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[boto3.VPCLattice 1.34.104](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-vpc-lattice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-vpc-lattice-1.34.0/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt` & `mypy_boto3_vpc_lattice-1.34.104/mypy_boto3_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-vpc-lattice-1.34.0/setup.py` & `mypy_boto3_vpc_lattice-1.34.104/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-vpc-lattice",
-    version="1.34.0",
+    version="1.34.104",
     packages=["mypy_boto3_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.VPCLattice 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.VPCLattice 1.34.104 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 vpc-lattice type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_vpc_lattice": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

