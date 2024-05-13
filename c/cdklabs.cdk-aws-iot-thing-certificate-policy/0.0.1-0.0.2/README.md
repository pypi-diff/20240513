# Comparing `tmp/cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1.tar.gz` & `tmp/cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1.tar", last modified: Thu May  9 14:18:46 2024, max compression
+gzip compressed data, was "cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2.tar", last modified: Mon May 13 12:41:48 2024, max compression
```

## Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1.tar` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.604357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-09 14:18:46.604357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:18:46.604357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/
--rw-r--r--   0 runner    (1001) docker     (127)    22931 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1212807 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:41:48.128284 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-05-13 12:41:48.128284 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:41:48.128284 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:41:48.124284 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:41:48.124284 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:41:48.124284 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs/cdk_aws_iot_thing_certificate_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)    23037 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:41:48.124284 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1212935 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:41:37.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs/cdk_aws_iot_thing_certificate_policy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:41:48.124284 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-05-13 12:41:48.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-13 12:41:48.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:41:48.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 12:41:48.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 12:41:48.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/LICENSE` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/PKG-INFO` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-aws-iot-thing-certificate-policy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Creates an AWS IoT thing, certificate, policy, and associates the three together
 Home-page: https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -18,26 +18,26 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
-# AWS IoT Thing, Certificate, and Policy Construct Library
+## AWS IoT Thing, Certificate, and Policy Construct Library
 
 [![NPM](https://img.shields.io/npm/v/@cdklabs/cdk-aws-iot-thing-certificate-policy?label=npm+cdk+v2)](https://www.npmjs.com/package/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 [![PyPI](https://img.shields.io/pypi/v/cdklabs.cdk-aws-iot-thing-certificate-policy?label=pypi+cdk+v2)](https://pypi.org/project/cdklabs.cdk-aws-iot-thing-certificate-policy/)
 [![Maven version](https://img.shields.io/maven-central/v/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy?label=maven+cdk+v2)](https://central.sonatype.com/artifact/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy)
-[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkNag)
-[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy?label=go+cdk+v2)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
-[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
+[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkAwsIotThingCertificatePolicy)
+[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy-go?label=go+cdk+v2&&filename=cdklabscdkawsiotthingcertificatepolicy%2Fgo.mod))](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
+[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/LICENSE)
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
-[![View on Construct Hub](https://constructs.dev/badge?package=@cdklabs/cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![View on Construct Hub](https://constructs.dev/badge?package=%40cdklabs%2Fcdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 
 An [L3 CDK construct](https://docs.aws.amazon.com/cdk/v2/guide/constructs.html#constructs_lib) to create and associate a singular AWS IoT Thing, Certificate, and IoT Policy. The construct also retrieves and returns AWS IoT account specific details such as the AWS IoT data endpoint and the AWS IoT Credential provider endpoint.
 
 The certificate and its private key are stored as AWS Systems Manager Parameter Store parameters that can be retrieved via the AWS Console or programmatically via construct members.
 
 ## Installation and use
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/README.md` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# AWS IoT Thing, Certificate, and Policy Construct Library
+## AWS IoT Thing, Certificate, and Policy Construct Library
 
 [![NPM](https://img.shields.io/npm/v/@cdklabs/cdk-aws-iot-thing-certificate-policy?label=npm+cdk+v2)](https://www.npmjs.com/package/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 [![PyPI](https://img.shields.io/pypi/v/cdklabs.cdk-aws-iot-thing-certificate-policy?label=pypi+cdk+v2)](https://pypi.org/project/cdklabs.cdk-aws-iot-thing-certificate-policy/)
 [![Maven version](https://img.shields.io/maven-central/v/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy?label=maven+cdk+v2)](https://central.sonatype.com/artifact/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy)
-[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkNag)
-[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy?label=go+cdk+v2)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
-[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
+[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkAwsIotThingCertificatePolicy)
+[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy-go?label=go+cdk+v2&&filename=cdklabscdkawsiotthingcertificatepolicy%2Fgo.mod))](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
+[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/LICENSE)
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
-[![View on Construct Hub](https://constructs.dev/badge?package=@cdklabs/cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![View on Construct Hub](https://constructs.dev/badge?package=%40cdklabs%2Fcdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 
 An [L3 CDK construct](https://docs.aws.amazon.com/cdk/v2/guide/constructs.html#constructs_lib) to create and associate a singular AWS IoT Thing, Certificate, and IoT Policy. The construct also retrieves and returns AWS IoT account specific details such as the AWS IoT data endpoint and the AWS IoT Credential provider endpoint.
 
 The certificate and its private key are stored as AWS Systems Manager Parameter Store parameters that can be retrieved via the AWS Console or programmatically via construct members.
 
 ## Installation and use
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/setup.py` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-aws-iot-thing-certificate-policy",
-    "version": "0.0.1",
+    "version": "0.0.2",
     "description": "Creates an AWS IoT thing, certificate, policy, and associates the three together",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdklabs.cdk_aws_iot_thing_certificate_policy",
         "cdklabs.cdk_aws_iot_thing_certificate_policy._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_aws_iot_thing_certificate_policy._jsii": [
-            "cdk-aws-iot-thing-certificate-policy@0.0.1.jsii.tgz"
+            "cdk-aws-iot-thing-certificate-policy@0.0.2.jsii.tgz"
         ],
         "cdklabs.cdk_aws_iot_thing_certificate_policy": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 '''
-# AWS IoT Thing, Certificate, and Policy Construct Library
+## AWS IoT Thing, Certificate, and Policy Construct Library
 
 [![NPM](https://img.shields.io/npm/v/@cdklabs/cdk-aws-iot-thing-certificate-policy?label=npm+cdk+v2)](https://www.npmjs.com/package/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 [![PyPI](https://img.shields.io/pypi/v/cdklabs.cdk-aws-iot-thing-certificate-policy?label=pypi+cdk+v2)](https://pypi.org/project/cdklabs.cdk-aws-iot-thing-certificate-policy/)
 [![Maven version](https://img.shields.io/maven-central/v/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy?label=maven+cdk+v2)](https://central.sonatype.com/artifact/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy)
-[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkNag)
-[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy?label=go+cdk+v2)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
-[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
+[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkAwsIotThingCertificatePolicy)
+[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy-go?label=go+cdk+v2&&filename=cdklabscdkawsiotthingcertificatepolicy%2Fgo.mod))](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
+[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/LICENSE)
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
-[![View on Construct Hub](https://constructs.dev/badge?package=@cdklabs/cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![View on Construct Hub](https://constructs.dev/badge?package=%40cdklabs%2Fcdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 
 An [L3 CDK construct](https://docs.aws.amazon.com/cdk/v2/guide/constructs.html#constructs_lib) to create and associate a singular AWS IoT Thing, Certificate, and IoT Policy. The construct also retrieves and returns AWS IoT account specific details such as the AWS IoT data endpoint and the AWS IoT Credential provider endpoint.
 
 The certificate and its private key are stored as AWS Systems Manager Parameter Store parameters that can be retrieved via the AWS Console or programmatically via construct members.
 
 ## Installation and use
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-aws-iot-thing-certificate-policy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Creates an AWS IoT thing, certificate, policy, and associates the three together
 Home-page: https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -18,26 +18,26 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
-# AWS IoT Thing, Certificate, and Policy Construct Library
+## AWS IoT Thing, Certificate, and Policy Construct Library
 
 [![NPM](https://img.shields.io/npm/v/@cdklabs/cdk-aws-iot-thing-certificate-policy?label=npm+cdk+v2)](https://www.npmjs.com/package/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 [![PyPI](https://img.shields.io/pypi/v/cdklabs.cdk-aws-iot-thing-certificate-policy?label=pypi+cdk+v2)](https://pypi.org/project/cdklabs.cdk-aws-iot-thing-certificate-policy/)
 [![Maven version](https://img.shields.io/maven-central/v/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy?label=maven+cdk+v2)](https://central.sonatype.com/artifact/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy)
-[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkNag)
-[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy?label=go+cdk+v2)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
-[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
+[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkAwsIotThingCertificatePolicy)
+[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy-go?label=go+cdk+v2&&filename=cdklabscdkawsiotthingcertificatepolicy%2Fgo.mod))](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
+[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/LICENSE)
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
-[![View on Construct Hub](https://constructs.dev/badge?package=@cdklabs/cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![View on Construct Hub](https://constructs.dev/badge?package=%40cdklabs%2Fcdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 
 An [L3 CDK construct](https://docs.aws.amazon.com/cdk/v2/guide/constructs.html#constructs_lib) to create and associate a singular AWS IoT Thing, Certificate, and IoT Policy. The construct also retrieves and returns AWS IoT account specific details such as the AWS IoT data endpoint and the AWS IoT Credential provider endpoint.
 
 The certificate and its private key are stored as AWS Systems Manager Parameter Store parameters that can be retrieved via the AWS Console or programmatically via construct members.
 
 ## Installation and use
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.2/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/dependency_links.txt
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/requires.txt
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/top_level.txt
 src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py
 src/cdklabs/cdk_aws_iot_thing_certificate_policy/py.typed
 src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py
-src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.1.jsii.tgz
+src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.2.jsii.tgz
```

