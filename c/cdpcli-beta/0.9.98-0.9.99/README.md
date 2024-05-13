# Comparing `tmp/cdpcli-beta-0.9.98.tar.gz` & `tmp/cdpcli-beta-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-beta-0.9.98.tar", last modified: Wed Sep 27 20:28:47 2023, max compression
+gzip compressed data, was "cdpcli-beta-0.9.99.tar", last modified: Thu Oct 12 21:16:30 2023, max compression
```

## Comparing `cdpcli-beta-0.9.98.tar` & `cdpcli-beta-0.9.99.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.858648 cdpcli-beta-0.9.98/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-09-27 20:28:47.858648 cdpcli-beta-0.9.98/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.858648 cdpcli-beta-0.9.98/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-09-27 20:28:47.858648 cdpcli-beta-0.9.98/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.842648 cdpcli-beta-0.9.98/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      278 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.842648 cdpcli-beta-0.9.98/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/cloudprivatelinks/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-09-27 20:28:44.000000 cdpcli-beta-0.9.98/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    96796 2023-09-27 20:28:43.000000 cdpcli-beta-0.9.98/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/consumption/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5243 2023-09-27 20:28:45.000000 cdpcli-beta-0.9.98/cdpcli/data/consumption/consumption.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   163250 2023-09-27 20:28:45.000000 cdpcli-beta-0.9.98/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   119309 2023-09-27 20:28:44.000000 cdpcli-beta-0.9.98/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32868 2023-09-27 20:28:46.000000 cdpcli-beta-0.9.98/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    94719 2023-09-27 20:28:45.000000 cdpcli-beta-0.9.98/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    82316 2023-09-27 20:28:46.000000 cdpcli-beta-0.9.98/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-09-27 20:28:44.000000 cdpcli-beta-0.9.98/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   208225 2023-09-27 20:28:44.000000 cdpcli-beta-0.9.98/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   205799 2023-09-27 20:28:43.000000 cdpcli-beta-0.9.98/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   153511 2023-09-27 20:28:45.000000 cdpcli-beta-0.9.98/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-09-27 20:28:44.000000 cdpcli-beta-0.9.98/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/metrics/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17516 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli/data/metrics/metrics.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    66512 2023-09-27 20:28:46.000000 cdpcli-beta-0.9.98/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    73666 2023-09-27 20:28:46.000000 cdpcli-beta-0.9.98/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    54815 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.838648 cdpcli-beta-0.9.98/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.846648 cdpcli-beta-0.9.98/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.850648 cdpcli-beta-0.9.98/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.850648 cdpcli-beta-0.9.98/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.850648 cdpcli-beta-0.9.98/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.850648 cdpcli-beta-0.9.98/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.850648 cdpcli-beta-0.9.98/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.850648 cdpcli-beta-0.9.98/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.850648 cdpcli-beta-0.9.98/cdpcli_beta.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli_beta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4371 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli_beta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli_beta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-09-27 20:28:47.000000 cdpcli-beta-0.9.98/cdpcli_beta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-09-27 20:28:47.858648 cdpcli-beta-0.9.98/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.838648 cdpcli-beta-0.9.98/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.854648 cdpcli-beta-0.9.98/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.854648 cdpcli-beta-0.9.98/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.854648 cdpcli-beta-0.9.98/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.854648 cdpcli-beta-0.9.98/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:28:47.858648 cdpcli-beta-0.9.98/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-09-27 20:18:21.000000 cdpcli-beta-0.9.98/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.568596 cdpcli-beta-0.9.99/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-10-12 21:16:30.568596 cdpcli-beta-0.9.99/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.568596 cdpcli-beta-0.9.99/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-10-12 21:16:30.568596 cdpcli-beta-0.9.99/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      278 2023-10-12 21:16:28.000000 cdpcli-beta-0.9.99/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-10-12 21:16:28.000000 cdpcli-beta-0.9.99/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/cloudprivatelinks/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-10-12 21:16:24.000000 cdpcli-beta-0.9.99/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    96796 2023-10-12 21:16:24.000000 cdpcli-beta-0.9.99/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/consumption/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5243 2023-10-12 21:16:26.000000 cdpcli-beta-0.9.99/cdpcli/data/consumption/consumption.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-10-12 21:16:28.000000 cdpcli-beta-0.9.99/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   163250 2023-10-12 21:16:26.000000 cdpcli-beta-0.9.99/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   119328 2023-10-12 21:16:25.000000 cdpcli-beta-0.9.99/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    35926 2023-10-12 21:16:27.000000 cdpcli-beta-0.9.99/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    94844 2023-10-12 21:16:26.000000 cdpcli-beta-0.9.99/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    92975 2023-10-12 21:16:27.000000 cdpcli-beta-0.9.99/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-10-12 21:16:25.000000 cdpcli-beta-0.9.99/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   236019 2023-10-12 21:16:25.000000 cdpcli-beta-0.9.99/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   209618 2023-10-12 21:16:24.000000 cdpcli-beta-0.9.99/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   153511 2023-10-12 21:16:26.000000 cdpcli-beta-0.9.99/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-10-12 21:16:25.000000 cdpcli-beta-0.9.99/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.556596 cdpcli-beta-0.9.99/cdpcli/data/metrics/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17516 2023-10-12 21:16:28.000000 cdpcli-beta-0.9.99/cdpcli/data/metrics/metrics.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    66512 2023-10-12 21:16:28.000000 cdpcli-beta-0.9.99/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    73589 2023-10-12 21:16:27.000000 cdpcli-beta-0.9.99/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-10-12 21:16:28.000000 cdpcli-beta-0.9.99/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    54815 2023-10-12 21:16:28.000000 cdpcli-beta-0.9.99/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.548596 cdpcli-beta-0.9.99/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29833 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.560596 cdpcli-beta-0.9.99/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.564596 cdpcli-beta-0.9.99/cdpcli_beta.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-10-12 21:16:29.000000 cdpcli-beta-0.9.99/cdpcli_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4371 2023-10-12 21:16:29.000000 cdpcli-beta-0.9.99/cdpcli_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-10-12 21:16:29.000000 cdpcli-beta-0.9.99/cdpcli_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-10-12 21:16:29.000000 cdpcli-beta-0.9.99/cdpcli_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-10-12 21:16:29.000000 cdpcli-beta-0.9.99/cdpcli_beta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-10-12 21:16:29.000000 cdpcli-beta-0.9.99/cdpcli_beta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-10-12 21:16:30.568596 cdpcli-beta-0.9.99/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.552596 cdpcli-beta-0.9.99/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.564596 cdpcli-beta-0.9.99/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.564596 cdpcli-beta-0.9.99/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.564596 cdpcli-beta-0.9.99/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.564596 cdpcli-beta-0.9.99/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:16:30.564596 cdpcli-beta-0.9.99/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38316 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-10-12 21:05:59.000000 cdpcli-beta-0.9.99/versioneer.py
```

### Comparing `cdpcli-beta-0.9.98/LICENSE.txt` & `cdpcli-beta-0.9.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-beta-0.9.99/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/PKG-INFO` & `cdpcli-beta-0.9.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.98
+Version: 0.9.99
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.98/README.md` & `cdpcli-beta-0.9.99/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/__init__.py` & `cdpcli-beta-0.9.99/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/argparser.py` & `cdpcli-beta-0.9.99/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/argprocess.py` & `cdpcli-beta-0.9.99/cdpcli/argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/arguments.py` & `cdpcli-beta-0.9.99/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/auth.py` & `cdpcli-beta-0.9.99/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/cdprequest.py` & `cdpcli-beta-0.9.99/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/clicommand.py` & `cdpcli-beta-0.9.99/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/clidriver.py` & `cdpcli-beta-0.9.99/cdpcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/client.py` & `cdpcli-beta-0.9.99/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/compat.py` & `cdpcli-beta-0.9.99/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/completer.py` & `cdpcli-beta-0.9.99/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/config.py` & `cdpcli-beta-0.9.99/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/configloader.py` & `cdpcli-beta-0.9.99/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/credentials.py` & `cdpcli-beta-0.9.99/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/_retry.json` & `cdpcli-beta-0.9.99/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/audit/audit.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/audit/audit.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: audit
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Audit Service
   license:
     name: Apache 2.0
   description: Cloudera CDP Auditing is a web service for interacting with the audit subsystem.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/cli.json` & `cdpcli-beta-0.9.99/cdpcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: cloudprivatelinks
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: BETA
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera CloudPrivateLinks API Service
   license:
     name: Apache 2.0
   description: Provisions PrivateLink Endpoints on the cloud environments.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/compute/compute.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/compute/compute.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: compute
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Compute Service
   license:
     name: Apache 2.0
   description: Defining service of compute public API service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/consumption/consumption.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/consumption/consumption.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: consumption
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Consumption API Service
   license:
     name: Apache 2.0
   description: Provides an interface to the consumption service.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/datacatalog/datacatalog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: datacatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera DataCatalog Service
   license:
     name: Apache 2.0
   description: Cloudera DataCatalog Service is a web service, using this service a user can execute operations like launching profilers in DataCatalog.
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/datahub/datahub.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/datahub/datahub.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datahub
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Data hub Service
   license:
     name: Apache 2.0
   description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/datalake/datalake.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/datalake/datalake.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datalake
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Datalake Service
   license:
     name: Apache 2.0
   description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1696,14 +1696,15 @@
         description: The datalake.
   DatalakeScaleType:
     type: string
     description: Represents the available datalake scales. Defaults to LIGHT_DUTY if not set.
     enum:
       - LIGHT_DUTY
       - MEDIUM_DUTY_HA
+      - ENTERPRISE
   DatalakeLoadBalancerSkuType:
     type: string
     description: Represents the Azure load balancer SKU type. The current default is BASIC. To disable the load balancer, use type NONE.
     enum:
       - BASIC
       - STANDARD
       - NONE
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/de/de.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/de/de.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: de
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Data Engineering
   license:
     name: Apache 2.0
   description: Create and manage Cloudera Data Engineering Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -396,14 +396,30 @@
         description: Maximum Number of Spot instances.
       initial_spot_instances:
         type: string
         description: Initial Spot Instances for the CDE Service.
       root_vol_size:
         type: string
         description: Root Volume Size.
+      cpuRequests:
+        type: string
+        description: CPU Requests for the entire CDE service quota.
+        x-form-factors: private
+      memoryRequests:
+        type: string
+        description: Memory requests for the entire CDE service quota, eg. 100Gi.
+        x-form-factors: private
+      gpuRequests:
+        type: string
+        description: GPU requests for the entire CDE service quota.
+        x-form-factors: private
+      resourcePool:
+        type: string
+        description: Resource Pool for the CDE service.
+        x-form-factors: private
   VcSummary:
     type: object
     description: CDE virtual cluster summary.
     required:
       - vcId
       - vcName
       - clusterId
@@ -507,14 +523,30 @@
         description: The Memory requests for VC for running spark jobs.
       actualCpuRequests:
         type: string
         description: Actual CPU request for the VC. This accounts for other dex apps(eg. livy, airflow), that run in the virtual cluster.
       actualMemoryRequests:
         type: string
         description: Actual Memory request for the VC. This accounts for other dex apps(eg. livy, airflow), that run in the virtual cluster.
+      gpuRequests:
+        type: string
+        description: GPU requests for autoscaling.
+        x-form-factors: private
+      guaranteedCpuRequests:
+        type: string
+        description: Guaranteed CPU requests for an Elastic Virtual Cluster.
+        x-form-factors: private
+      guaranteedMemoryRequests:
+        type: string
+        description: Guaranteed Memory requests for an Elastic Virtual Cluster - eg. 30Gi.
+        x-form-factors: private
+      guaranteedGpuRequests:
+        type: string
+        description: Guaranteed GPU requests for an Elastic Virtual Cluster.
+        x-form-factors: private
     description: Object to store resources for a CDE service
   ChartValueOverridesRequest:
     type: object
     properties:
       chartName:
         type: string
         description: Name of the chart that has to be overridden, for eg- "dex-app", "dex-base".
@@ -710,14 +742,34 @@
         $ref: '#/definitions/CustomAzureFilesConfigs'
         description: CDE uses a default public File Shares storage provisioned by AKS. Enable this option to use your own public/private File Shares.
       networkOutboundType:
         type: string
         enum:
           - UDR
         description: Network outbound type. Currently 'udr' is the only supported.
+      cpuRequests:
+        x-form-factors: private
+        type: string
+        description: CPU Requests for the entire CDE service quota.
+      memoryRequests:
+        x-form-factors: private
+        type: string
+        description: Memory requests for the entire CDE service quota, eg. 100Gi.
+      gpuRequests:
+        x-form-factors: private
+        type: string
+        description: GPU requests for the entire CDE service quota.
+      resourcePool:
+        x-form-factors: private
+        type: string
+        description: Resource Pool for the CDE service.
+      nfsStorageClass:
+        x-form-factors: private
+        type: string
+        description: NFS Storage class to override the default storage class in private cloud.
   CustomAzureFilesConfigs:
     type: object
     description: Override Azure Files Configs.
     required:
       - storageAccountName
       - resourceGroup
     properties:
@@ -768,14 +820,26 @@
           type: string
         description: List of CIDRs that would be allowed to access kubernetes master API server.
       loadbalancerAllowlist:
         type: array
         items:
           type: string
         description: List of CIDRs that would be allowed to access the load balancer.
+      cpuRequests:
+        x-form-factors: private
+        type: string
+        description: CPU Requests for the entire CDE service quota.
+      memoryRequests:
+        x-form-factors: private
+        type: string
+        description: Memory requests for the entire CDE service quota, eg. 100Gi.
+      gpuRequests:
+        x-form-factors: private
+        type: string
+        description: GPU requests for the entire CDE service quota.
   UpdateServiceResponse:
     type: object
     description: Response object for UpdateService request.
     properties:
       operationId:
         type: string
         description: Deprecated. The operation ID of the update request.
@@ -899,14 +963,30 @@
         description: Cluster id of the CDE service where virtual cluster has to be created.
       cpuRequests:
         type: string
         description: Cpu requests for autoscaling.
       memoryRequests:
         type: string
         description: Memory requests for autoscaling - eg. 30Gi.
+      gpuRequests:
+        x-form-factors: private
+        type: string
+        description: GPU requests for autoscaling.
+      guaranteedCpuRequests:
+        x-form-factors: private
+        type: string
+        description: Guaranteed CPU requests for an Elastic Virtual Cluster.
+      guaranteedMemoryRequests:
+        x-form-factors: private
+        type: string
+        description: Guaranteed Memory requests for an Elastic Virtual Cluster - eg. 30Gi.
+      guaranteedGpuRequests:
+        x-form-factors: private
+        type: string
+        description: Guaranteed GPU requests for an Elastic Virtual Cluster.
       chartValueOverrides:
         type: array
         items:
           $ref: '#/definitions/ChartValueOverridesRequest'
         description: Chart overrides for creating a virtual cluster.
       smtpConfigs:
         $ref: '#/definitions/SmtpConfigRequest'
@@ -918,15 +998,19 @@
           - ALL
           - NONE
       sparkVersion:
         type: string
         description: Spark version for the virtual cluster. Currently supported spark versions are SPARK2(deprecated), SPARK3 and SPARK3_3. This feature is only supported in CDE-1.7.0 and beyond. SPARK3_3 is supported in CDE-1.19 and beyond.
         enum:
           - SPARK2
+          - SPARK2_4
           - SPARK3
+          - SPARK3_0
+          - SPARK3_1
+          - SPARK3_2
           - SPARK3_3
       vcTier:
         type: string
         description: Tier of the virtual cluster. Currently supported tiers are CORE and ALLP. CORE tiered virtual cluster enables operational deployment via batch jobs. ALLP virtual clusters are all-purpose virtual clusters supporting both operational batch jobs and interactive sessions. This feature is only supported in CDE-1.19.0 and beyond.
         enum:
           - ALLP
           - CORE
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/df/df.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/df/df.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: df
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera DataFlow Service
   license:
     name: Apache 2.0
   description: Manage DataFlow Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1807,14 +1807,15 @@
         description: The newly created deployment request CRN.
       dfxLocalUrl:
         type: string
         description: Base URL to the dfx-local instance running an eventually created deployment
   DeploymentState:
     type: string
     description: The state that the deployment is currently in.
+    x-deprecated-enum-values: SUSPENDING_FLOW
     enum:
       - DEPLOYING
       - GOOD_HEALTH
       - CONCERNING_HEALTH
       - BAD_HEALTH
       - STARTING_FLOW
       - SUSPENDING_FLOW
@@ -1823,14 +1824,18 @@
       - TERMINATING
       - RESTARTING
       - UPGRADING
       - ROLLING_BACK
       - STOPPED
       - UNKNOWN
       - IMPORTING_FLOW
+      - STOPPING_FLOW
+      - FLOW_STOPPED
+      - SUSPENDING
+      - RESUMING
   DeploymentStatus:
     type: object
     description: The status of a deployment
     required:
       - detailedState
       - message
       - state
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 swagger: '2.0'
 x-endpoint-name: dfworkload
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
   description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
@@ -380,14 +380,144 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/GetDeploymentRequestDetailsResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /dfx/api/rpc-v1/deployments/restart-deployment:
+    post:
+      summary: Restart a deployment.
+      description: Initiates restart of a deployment.
+      operationId: restartDeployment
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
+      parameters:
+        - in: body
+          name: input
+          description: Restart Deployment Request
+          required: true
+          schema:
+            $ref: '#/definitions/RestartDeploymentRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/RestartDeploymentResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /dfx/api/rpc-v1/deployments/resume-deployment:
+    post:
+      summary: Resumes a deployment.
+      description: Initiates the deployment resume.
+      operationId: resumeDeployment
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
+      parameters:
+        - in: body
+          name: input
+          description: Resume Deployment Request
+          required: true
+          schema:
+            $ref: '#/definitions/ResumeDeploymentRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/ResumeDeploymentResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /dfx/api/rpc-v1/deployments/start-flow:
+    post:
+      summary: Starts a flow.
+      description: Starts the NiFi flow of a deployment.
+      operationId: startFlow
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
+      parameters:
+        - in: body
+          name: input
+          description: Start Flow
+          required: true
+          schema:
+            $ref: '#/definitions/StartFlowRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/StartFlowResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /dfx/api/rpc-v1/deployments/stop-flow:
+    post:
+      summary: Stops a flow.
+      description: Stops the NiFi flow of a deployment.
+      operationId: stopFlow
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
+      parameters:
+        - in: body
+          name: input
+          description: Stop Flow
+          required: true
+          schema:
+            $ref: '#/definitions/StopFlowRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/StopFlowResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /dfx/api/rpc-v1/deployments/suspend-deployment:
+    post:
+      summary: Suspends a deployment.
+      description: Initiates the deployment suspend.
+      operationId: suspendDeployment
+      x-workload: true
+      x-client-only: true
+      x-extensions: workload
+      tags:
+        - CDFLocalRPCAPIVersion1
+      parameters:
+        - in: body
+          name: input
+          description: Suspend Deployment Request
+          required: true
+          schema:
+            $ref: '#/definitions/SuspendDeploymentRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/SuspendDeploymentResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /dfx/api/rpc-v1/deployments/terminate-deployment:
     post:
       summary: Terminates a deployment.
       description: Initiates the termination of a deployment.
       operationId: terminateDeployment
       x-workload: true
       x-client-only: true
@@ -409,15 +539,15 @@
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
   /dfx/api/rpc-v1/deployments/transition-flow:
     post:
       summary: Transitions a flow.
-      description: Transitions the NiFi flow of a deployment to the specified state.
+      description: Transitions the NiFi flow of a deployment to the specified state. Deprecated. Use `start-flow` and `stop-flow` instead.
       operationId: transitionFlow
       x-workload: true
       x-client-only: true
       x-extensions: workload
       tags:
         - CDFLocalRPCAPIVersion1
       parameters:
@@ -432,14 +562,16 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/TransitionFlowResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+      deprecated: true
+      x-deprecated: true
   /dfx/api/rpc-v1/deployments/update-deployment:
     post:
       summary: Updates a deployment.
       description: Updates a deployment.
       operationId: updateDeployment
       x-workload: true
       x-client-only: true
@@ -1087,14 +1219,23 @@
         type: string
         description: The FQDN of inbound hostname or just the prefix part
       listenComponents:
         type: array
         description: Listen components port and protocol data
         items:
           $ref: '#/definitions/ListenComponent'
+      nodeStorageProfileName:
+        type: string
+        description: Node storage profile name
+        enum:
+          - STANDARD_AWS
+          - STANDARD_AZURE
+          - PERFORMANCE_AWS
+          - PERFORMANCE_AZURE
+          - LOCAL_K8S
       customNarConfigurationCrn:
         type: string
         description: The CRN of the custom NAR configuration.
   CreateDeploymentResponse:
     type: object
     description: Response object from creating a deployment.
     x-workload: true
@@ -1189,135 +1330,54 @@
         type: string
         description: The CRN of the Inbound Connection Endpoint
   DeleteInboundConnectionEndpointResponse:
     type: object
     description: Response object returned during deletion of an Inbound Connection Endpoint
     x-workload: true
     x-client-only: true
-  DeploymentConfiguration:
-    type: object
-    description: Provides all of the configuration that dictates how a flow should be deployed
-    x-workload: true
-    x-client-only: true
-    required:
-      - configurationVersion
-    properties:
-      configurationVersion:
-        type: integer
-        format: int32
-        description: The version of this configuration
-      parameterGroups:
-        type: array
-        description: The list of flow parameter groups
-        items:
-          $ref: '#/definitions/FlowParameterGroup'
-      autoScalingEnabled:
-        type: boolean
-        description: Specifies that auto-scaling should be enabled.
-      flowMetricsScalingEnabled:
-        type: boolean
-        description: Specifies that Flow metrics should be enabled for scaling.
-      autoScaleMinNodes:
-        type: integer
-        format: int32
-        description: The minimum number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is true.
-      autoScaleMaxNodes:
-        type: integer
-        format: int32
-        description: The maximum number of nodes that the cluster should scale to. May only be specified when autoScalingEnabled is true.
-      staticNodeCount:
-        type: integer
-        format: int32
-        description: The static number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is false.
-      kpis:
-        type: array
-        description: The list of configured KPIs
-        items:
-          $ref: '#/definitions/ConfiguredKpi'
-      deploymentId:
-        type: string
-        description: The id of the deployment.
-      deploymentCrn:
-        type: string
-        description: The CRN of the deployment.
-      name:
-        type: string
-        description: The name of the deployment
-      cfmNifiVersion:
-        type: string
-        description: The CFM NiFi version associated with the deployment
-      autoStartFlow:
-        type: boolean
-        description: Indicates whether or not the flow should be started during deployment creation
-      clusterSizeName:
-        type: string
-        description: The size of the cluster to deploy
-        enum:
-          - EXTRA_SMALL
-          - SMALL
-          - MEDIUM
-          - LARGE
-      parametersDirty:
-        type: boolean
-        description: Indicates whether or not all current parameter values have successfully been applied to NiFi
-        readOnly: true
-      kpisDirty:
-        type: boolean
-        description: Indicates whether or not the current KPIs have successfully been deployed as alert rules
-        readOnly: true
-      sizingAndScalingDirty:
-        type: boolean
-        description: Indicates whether or not the current sizing and scaling configuration has been successfully applied in Kubernetes
-        readOnly: true
-      lastUpdatedByUsername:
-        type: string
-        description: The username of the last person to update the deployment configuration
-        readOnly: true
-      inboundHostname:
-        type: string
-        description: The inbound hostname
-      listenComponents:
-        type: array
-        description: Listen components port and protocol data
-        items:
-          $ref: '#/definitions/ListenComponent'
   DeploymentStatus:
     type: object
     description: The state and state message associated with a deployment
     x-workload: true
     x-client-only: true
     required:
       - detailedState
       - state
     properties:
       detailedState:
         type: string
         description: The detailed state that the deployment is currently in
+        x-deprecated-enum-values: FAILED_TO_START,SUSPENDING_FLOW
         enum:
           - GOOD_HEALTH
-          - FAILED_TO_SUSPEND
+          - FAILED_TO_STOP_FLOW
           - FAILED_TO_UPDATE_NIFI_VERSION
-          - FAILED_TO_START
+          - FAILED_TO_START_FLOW
           - FAILED_TO_RESTART
-          - SUSPENDED
+          - FLOW_STOPPED
           - FAILED_TO_DEPLOY
           - FAILED_TO_IMPORT
           - FAILED_TO_UPDATE
           - FAILED_TO_TERMINATE
           - NEW
           - CREATING_NODES
           - DEPLOYING_ASSETS
           - DEPLOYING_FLOW_DEFINITION
           - IMPORTING_FLOW
           - STARTING_FLOW
-          - SUSPENDING_FLOW
+          - STOPPING_FLOW
           - UPDATING
           - UPDATING_NIFI_VERSION
           - CANCELLING_NIFI_VERSION_UPDATE
           - RESTARTING
+          - SUSPENDING
+          - RESUMING
+          - SUSPENDED
+          - FAILED_TO_SUSPEND
+          - FAILED_TO_RESUME
           - TERMINATING
           - CANCEL_REQUESTED
           - STOPPED
           - UNKNOWN
           - UPGRADING
           - FAILED_TO_UPGRADE
           - ROLLING_BACK
@@ -1328,33 +1388,41 @@
           - AT_CAPACITY
           - SDX_OUTPUT_CHANGED
           - METRICS_UNAVAILABLE
           - METERING_WARNING
           - METERING_OFFLINE
           - CERTIFICATE_RENEWED
           - NOT_HEALTHY
+          - EXCESSIVE_OFFLOAD_TIME
+          - FAILED_TO_START
+          - SUSPENDING_FLOW
       state:
         type: string
         description: The state that the deployment is currently in
+        x-deprecated-enum-values: SUSPENDING_FLOW
         enum:
           - DEPLOYING
           - GOOD_HEALTH
           - CONCERNING_HEALTH
           - BAD_HEALTH
           - IMPORTING_FLOW
           - STARTING_FLOW
-          - SUSPENDING_FLOW
-          - SUSPENDED
+          - STOPPING_FLOW
+          - FLOW_STOPPED
           - UPDATING
           - TERMINATING
           - RESTARTING
+          - SUSPENDING
+          - RESUMING
+          - SUSPENDED
           - UPGRADING
           - ROLLING_BACK
           - STOPPED
           - UNKNOWN
+          - SUSPENDING_FLOW
       message:
         type: string
         description: Detail message relating to the current status of the deployment
   DescribeInboundConnectionEndpointRequest:
     type: object
     description: Request object that contains the identifier of the Inbound Connection Endpoint to describe
     x-workload: true
@@ -1429,14 +1497,18 @@
           - FILE
           - FILES
       assetReferences:
         type: array
         description: The list of referenced assets.
         items:
           $ref: '#/definitions/AssetReference'
+      valueSet:
+        type: boolean
+        description: Indicates if the value of this parameter is set (i.e. not null)
+        readOnly: true
   FlowParameterGroup:
     type: object
     description: A flow parameter group
     x-workload: true
     x-client-only: true
     properties:
       name:
@@ -1569,15 +1641,15 @@
     type: object
     description: Response object for retrieving deployment configuration request.
     x-workload: true
     x-client-only: true
     properties:
       deploymentConfiguration:
         description: The deployment configuration.
-        $ref: '#/definitions/DeploymentConfiguration'
+        $ref: '#/definitions/RpcDeploymentConfiguration'
   GetDeploymentRequestDetailsRequest:
     type: object
     description: Request object for retrieving deployment request details.
     x-workload: true
     x-client-only: true
     required:
       - environmentCrn
@@ -1632,27 +1704,24 @@
         description: The status message of the Inbound Connection Endpoint Certificate
         readOnly: true
   InboundConnectionEndpointClientCertificateRequest:
     type: object
     description: Request object to retrieve Inbound Connection Endpoint client's certificate.
     x-workload: true
     x-client-only: true
+    required:
+      - environmentCrn
+      - crn
     properties:
       environmentCrn:
         type: string
         description: The CRN of an environment to execute the command.
-      id:
-        type: string
-        description: The Inbound Connection Endpoint identifier. Deprecated. Use 'crn' instead
-        x-deprecated: true
       crn:
         type: string
         description: The CRN of the Inbound Connection Endpoint
-    required:
-      - environmentCrn
   InboundConnectionEndpointClientCertificateResponse:
     type: object
     description: Response object that contains the client's certificate.
     x-workload: true
     x-client-only: true
     properties:
       certificate:
@@ -1660,27 +1729,24 @@
         description: The client's encoded certificate.
         readOnly: true
   InboundConnectionEndpointClientPrivateKeyRequest:
     type: object
     description: Request object to retrieve Inbound Connection Endpoint client's private key.
     x-workload: true
     x-client-only: true
+    required:
+      - environmentCrn
+      - crn
     properties:
       environmentCrn:
         type: string
         description: The CRN of an environment to execute the command.
-      id:
-        type: string
-        description: The Inbound Connection Endpoint identifier. Deprecated. Use 'crn' instead
-        x-deprecated: true
       crn:
         type: string
         description: The CRN of the Inbound Connection Endpoint
-    required:
-      - environmentCrn
   InboundConnectionEndpointClientPrivateKeyResponse:
     type: object
     description: Response object that contains the client's private key.
     x-workload: true
     x-client-only: true
     properties:
       privateKey:
@@ -1947,14 +2013,68 @@
           - ListenBeats
           - ListenLumberjack
           - ListenWebSocket
           - HandleHttpRequest
       port:
         type: string
         description: Inbound port
+  NodeStorageProfileMetadata:
+    type: object
+    description: Provides details about the node storage options.
+    x-workload: true
+    x-client-only: true
+    required:
+      - contentRepoSize
+      - flowfileRepoSize
+      - iops
+      - provenanceRepoSize
+      - storageVolumeType
+      - throughput
+    properties:
+      contentRepoSize:
+        type: integer
+        format: int32
+        description: Content repository size
+        readOnly: true
+      provenanceRepoSize:
+        type: integer
+        format: int32
+        description: Provenance repository size
+        readOnly: true
+      flowfileRepoSize:
+        type: integer
+        format: int32
+        description: FlowFile repository size
+        readOnly: true
+      iops:
+        type: string
+        description: IOPS
+        readOnly: true
+      throughput:
+        type: string
+        description: Throughput
+        readOnly: true
+      storageVolumeType:
+        type: string
+        description: Storage volume type
+        readOnly: true
+      name:
+        type: string
+        description: The name of this Storage Profile
+        enum:
+          - LEGACY_STANDARD
+          - LEGACY_PERFORMANCE
+          - STANDARD_AWS
+          - STANDARD_AZURE
+          - PERFORMANCE_AWS
+          - PERFORMANCE_AZURE
+          - LOCAL_K8S
+      text:
+        type: string
+        description: The text (i.e., the human readable name) for this Storage Profile
   RenewInboundConnectionEndpointCertificateRequest:
     type: object
     description: Request object to renew Inbound Connection Endpoint certificate(s)
     x-workload: true
     x-client-only: true
     required:
       - environmentCrn
@@ -1976,14 +2096,65 @@
         type: boolean
         description: Whether to revoke existing Inbound Connection Endpoint's client certificates
   RenewInboundConnectionEndpointCertificateResponse:
     type: object
     description: Response object for Inbound Connection Endpoint certificate renewal request
     x-workload: true
     x-client-only: true
+  RestartDeploymentRequest:
+    type: object
+    description: Request object to restart a deployment.
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - deploymentCrn
+    properties:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
+        type: string
+        description: The deployment crn.
+      forceStopFlow:
+        type: boolean
+        description: Whether to force stop the NiFi flow during restart.
+  RestartDeploymentResponse:
+    type: object
+    description: Response object for restarting a deployment request.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
+  ResumeDeploymentRequest:
+    type: object
+    description: Request object to resume a deployment.
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - deploymentCrn
+    properties:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
+        type: string
+        description: The deployment crn.
+  ResumeDeploymentResponse:
+    type: object
+    description: Response object for resuming a deployment.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
   RpcDeployment:
     type: object
     description: Provides details about a deployment.
     x-workload: true
     x-client-only: true
     required:
       - name
@@ -2027,23 +2198,29 @@
         description: Valid actions that can be applied to the deployment in its current state
         uniqueItems: true
         items:
           type: string
           enum:
             - VIEW_NIFI
             - START_FLOW
-            - SUSPEND_FLOW
+            - STOP_FLOW
             - EDIT
             - CANCEL_CREATE
             - TERMINATE
             - VIEW_METRICS
             - UPDATE_NIFI_VERSION
             - CANCEL_NIFI_VERSION_UPDATE
             - RESTART_DEPLOYMENT
             - MANAGE_DEPLOYMENT
+            - EXPORT
+            - SUSPEND
+            - RESUME
+            - DOWNLOAD_LOG
+            - SUSPEND_FLOW
+          x-deprecated-enum-values: SUSPEND_FLOW
       nifiUrl:
         type: string
         description: The url to open the deployed flow in NiFi
       clusterSize:
         type: string
         description: The initial size of the deployment
         enum:
@@ -2086,14 +2263,17 @@
         description: The version of the flow
       flowVersionCrn:
         type: string
         description: The deployment's current flow version CRN
       flowCrn:
         type: string
         description: The deployment's current flow CRN
+      creatorCrn:
+        type: string
+        description: The CRN of the user who deployed the flow
       artifactTypeName:
         type: string
         description: The type of artifact of the flow
       currentNodeCount:
         type: integer
         format: int32
         description: The current node count
@@ -2128,14 +2308,115 @@
         description: Indicates this deployment was created as a test session for designing a flow
       flowDesignerId:
         type: string
         description: The ID of the flow design for a test session deployment.
       customNarConfigurationId:
         type: string
         description: The identifier of the custom NAR configuration, if used.
+      nodeStorageProfile:
+        type: string
+        description: The node storage profile
+  RpcDeploymentConfiguration:
+    type: object
+    description: Provides all of the configuration that dictates how a flow should be deployed
+    x-workload: true
+    x-client-only: true
+    required:
+      - configurationVersion
+    properties:
+      configurationVersion:
+        type: integer
+        format: int32
+        description: The version of this configuration
+      parameterGroups:
+        type: array
+        description: The list of flow parameter groups
+        items:
+          $ref: '#/definitions/FlowParameterGroup'
+      autoScalingEnabled:
+        type: boolean
+        description: Specifies that auto-scaling should be enabled.
+      flowMetricsScalingEnabled:
+        type: boolean
+        description: Specifies that Flow metrics should be enabled for scaling.
+      autoScaleMinNodes:
+        type: integer
+        format: int32
+        description: The minimum number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is true.
+      autoScaleMaxNodes:
+        type: integer
+        format: int32
+        description: The maximum number of nodes that the cluster should scale to. May only be specified when autoScalingEnabled is true.
+      staticNodeCount:
+        type: integer
+        format: int32
+        description: The static number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is false.
+      kpis:
+        type: array
+        description: The list of configured KPIs
+        items:
+          $ref: '#/definitions/ConfiguredKpi'
+      deploymentId:
+        type: string
+        description: The id of the deployment.
+      deploymentCrn:
+        type: string
+        description: The CRN of the deployment.
+      name:
+        type: string
+        description: The name of the deployment
+      cfmNifiVersion:
+        type: string
+        description: The CFM NiFi version associated with the deployment
+      autoStartFlow:
+        type: boolean
+        description: Indicates whether or not the flow should be started during deployment creation
+      clusterSizeName:
+        type: string
+        description: The size of the cluster to deploy
+        enum:
+          - EXTRA_SMALL
+          - SMALL
+          - MEDIUM
+          - LARGE
+      nodeStorageProfileName:
+        type: string
+        description: Node storage profile name
+        enum:
+          - LEGACY_STANDARD
+          - LEGACY_PERFORMANCE
+          - STANDARD_AWS
+          - STANDARD_AZURE
+          - PERFORMANCE_AWS
+          - PERFORMANCE_AZURE
+          - LOCAL_K8S
+      parametersDirty:
+        type: boolean
+        description: Indicates whether or not all current parameter values have successfully been applied to NiFi
+        readOnly: true
+      kpisDirty:
+        type: boolean
+        description: Indicates whether or not the current KPIs have successfully been deployed as alert rules
+        readOnly: true
+      sizingAndScalingDirty:
+        type: boolean
+        description: Indicates whether or not the current sizing and scaling configuration has been successfully applied in Kubernetes
+        readOnly: true
+      lastUpdatedByUsername:
+        type: string
+        description: The username of the last person to update the deployment configuration
+        readOnly: true
+      inboundHostname:
+        type: string
+        description: The inbound hostname
+      listenComponents:
+        type: array
+        description: Listen components port and protocol data
+        items:
+          $ref: '#/definitions/ListenComponent'
   RpcDeploymentConfigurationMetadata:
     type: object
     description: Provides details about the deployment and all of the different configuration items that are available.
     x-workload: true
     x-client-only: true
     required:
       - flowCrn
@@ -2178,14 +2459,19 @@
         description: The KPI meta data
         $ref: '#/definitions/KpiMetaData'
       clusterSizingOptions:
         type: array
         description: The options that are available for determining the size of the deployed cluster
         items:
           $ref: '#/definitions/ClusterSize'
+      nodeStorageProfileMetadata:
+        type: array
+        description: The list of node storage profiles
+        items:
+          $ref: '#/definitions/NodeStorageProfileMetadata'
   ServiceMeta:
     type: object
     description: The meta information about a DataFlow service.
     x-workload: true
     x-client-only: true
     required:
       - cloudPlatform
@@ -2214,14 +2500,86 @@
           - MOCK
       region:
         description: The region of the DataFlow service
         $ref: '#/definitions/EnvCloudRegion'
       environmentCrn:
         type: string
         description: Crn of associated CDP environment
+  StartFlowRequest:
+    type: object
+    description: Request object for starting the NiFi flow.
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - deploymentCrn
+    properties:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
+        type: string
+        description: The deployment crn.
+  StartFlowResponse:
+    type: object
+    description: Response object for starting the NiFi flow.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
+  StopFlowRequest:
+    type: object
+    description: Request object for stopping the NiFi flow.
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - deploymentCrn
+    properties:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
+        type: string
+        description: The deployment crn.
+  StopFlowResponse:
+    type: object
+    description: Response object for stopping the NiFi flow.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
+  SuspendDeploymentRequest:
+    type: object
+    description: Request object to suspend a deployment.
+    x-workload: true
+    x-client-only: true
+    required:
+      - environmentCrn
+      - deploymentCrn
+    properties:
+      environmentCrn:
+        type: string
+        description: The CRN of an environment to execute the command.
+      deploymentCrn:
+        type: string
+        description: The deployment crn.
+  SuspendDeploymentResponse:
+    type: object
+    description: Response object for suspending a deployment.
+    x-workload: true
+    x-client-only: true
+    properties:
+      deployment:
+        description: The deployment.
+        $ref: '#/definitions/RpcDeployment'
   TerminateDeploymentRequest:
     type: object
     description: Request object to terminate a deployment.
     x-workload: true
     x-client-only: true
     required:
       - environmentCrn
@@ -2260,14 +2618,15 @@
         description: The deployment crn.
       flowState:
         type: string
         description: The desired state of the NiFi flow
         enum:
           - STARTED
           - SUSPENDED
+          - STOPPED
   TransitionFlowResponse:
     type: object
     description: Response object for transitioning the state of the NiFi flow.
     x-workload: true
     x-client-only: true
     properties:
       deployment:
@@ -2375,26 +2734,34 @@
         format: int32
         description: The static number of nodes that the cluster should allocate. May only be specified when autoScalingEnabled is false.
       kpis:
         type: array
         description: The list of configured KPIs
         items:
           $ref: '#/definitions/ConfiguredKpi'
+      clusterSizeName:
+        type: string
+        description: The deployment t-shirt size
+        enum:
+          - EXTRA_SMALL
+          - SMALL
+          - MEDIUM
+          - LARGE
       assetUpdateRequestCrn:
         type: string
         description: The CRN of the asset update request. Required when updating assets of an existing deployment.
   UpdateDeploymentResponse:
     type: object
     description: Response object from updating a deployment.
     x-workload: true
     x-client-only: true
     properties:
       deploymentConfiguration:
         description: The deployment configuration.
-        $ref: '#/definitions/DeploymentConfiguration'
+        $ref: '#/definitions/RpcDeploymentConfiguration'
   UpdateNifiVersionRequest:
     type: object
     description: Request object for updating the NiFi version of a deployment.
     x-workload: true
     x-client-only: true
     required:
       - environmentCrn
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/drscp/drscp.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/drscp/drscp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: drscp
 x-products: CDP
 x-form-factors: private
 x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: CDP Control Plane Data Recovery Service
   license:
     name: Apache 2.0
   description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/dw/dw.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/dw/dw.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swagger: '2.0'
 x-endpoint-name: dw
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Data Warehouse [EXPERIMENTAL]
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Data Warehouse clusters.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -234,14 +234,36 @@
           schema:
             $ref: '#/definitions/UpdateServerSettingResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
       x-mutating: true
+  /api/v1/dw/listEvents:
+    post:
+      x-form-factors: public,private
+      x-mutating: false
+      summary: Get the list of events.
+      description: 'Get the list of events for the given Operation or a specific Service (Cluster, Database Catalog, Virtual Warehouse, or Data Visualization App). Events can belong to a particular Operation which might span across multiple Services. This happens if the given operation affects one or more Services e.g.: restore-cluster. It is also possible to return the events only for a given Service, in this case it is enough to pass the Id of a Service (e.g.: env-sq7hfv, warehouse-1696571829-pps2, compute-1696571962-8dd8, impala-1696572085-cn44).'
+      operationId: listEvents
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/ListEventsRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/ListEventsResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/dw/updateSshKey:
     post:
       x-form-factors: public
       summary: Update the SSH Key for a Cloudera Data Warehouse cluster
       description: Update the SSH Key for a Cloudera Data Warehouse cluster
       operationId: updateSshKey
       parameters:
@@ -303,14 +325,127 @@
           schema:
             $ref: '#/definitions/CreateClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
       x-mutating: true
+  /api/v1/dw/suspendCluster:
+    post:
+      x-no-compatibility-guarantee: true
+      x-mutating: true
+      x-form-factors: public
+      summary: Suspend Cloudera Data Warehouse cluster.
+      description: Suspend Cloudera Data Warehouse cluster. Supported only on Azure. Suspend cluster requires a "Running" Azure CDW, trying to suspend a cluster already in "Stopped" or "Error" state is not supported. Every Virtual Warehouse and Database Catalog which belongs to that CDW must be stopped first. This operation will stop the AKS cluster for this CDW instance, however leaves other cloud resources in "Running" state, including the Postgres database.
+      operationId: suspendCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/SuspendClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/SuspendClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/dw/resumeCluster:
+    post:
+      x-no-compatibility-guarantee: true
+      x-mutating: true
+      x-form-factors: public
+      summary: Resume Cloudera Data Warehouse cluster.
+      description: Resume Cloudera Data Warehouse cluster. Supported only on Azure. Resume cluster will start a stopped CDW cluster. Resuming a cluster in "Running" or "Error" state is not supported. Resume will start the AKS instance which belongs to this CDW.
+      operationId: resumeCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/ResumeClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/ResumeClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/dw/createAwsCluster:
+    post:
+      x-no-compatibility-guarantee: true
+      x-mutating: true
+      summary: Create an AWS cluster in the Cloudera Data Warehouse.
+      description: Create an AWS cluster in the Cloudera Data Warehouse environment with the provided settings.
+      operationId: createAwsCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/CreateAwsClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/CreateAwsClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/dw/createAzureCluster:
+    post:
+      x-no-compatibility-guarantee: true
+      x-mutating: true
+      summary: Create an Azure cluster in the Cloudera Data Warehouse.
+      description: Create an Azure cluster in the Cloudera Data Warehouse environment with the provided settings.
+      operationId: createAzureCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/CreateAzureClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/CreateAzureClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/dw/createPrivateCluster:
+    post:
+      x-form-factors: private
+      x-no-compatibility-guarantee: true
+      x-mutating: true
+      summary: Create a  a Private Cloud cluster in the Cloudera Data Warehouse.
+      description: Create a Private Cloud cluster in the Cloudera Data Warehouse environment with the provided settings.
+      operationId: createPrivateCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/CreatePrivateClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/CreatePrivateClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/dw/deleteCluster:
     post:
       x-no-compatibility-guarantee: true
       summary: Delete a Cloudera Data Warehouse cluster.
       description: Delete a Cloudera Data Warehouse cluster.
       operationId: deleteCluster
       parameters:
@@ -346,14 +481,78 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/UpdateClusterResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/dw/updateAwsCluster:
+    post:
+      x-mutating: true
+      summary: Updates an AWS cluster in the Cloudera Data Warehouse.
+      description: Update an AWS cluster in the Cloudera Data Warehouse with the provided settings.
+      operationId: updateAwsCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdateAwsClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdateAwsClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/dw/updateAzureCluster:
+    post:
+      x-mutating: true
+      summary: Updates an Azure cluster in the Cloudera Data Warehouse.
+      description: Update an Azure cluster in the Cloudera Data Warehouse with the provided settings.
+      operationId: updateAzureCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdateAzureClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdateAzureClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/dw/updatePrivateCluster:
+    post:
+      x-form-factors: private
+      x-mutating: true
+      summary: Updates a Private Cloud (PvC) cluster in the Cloudera Data Warehouse.
+      description: Update a Private Cloud cluster (PvC) in the Cloudera Data Warehouse with the provided settings.
+      operationId: updatePrivateCluster
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdatePrivateClusterRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdatePrivateClusterResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/dw/upgradeCluster:
     post:
       x-mutating: true
       summary: Upgrade the Cloudera Data Warehouse cluster.
       description: Upgrade the Cloudera Data Warehouse cluster to the latest supported version. Expect downtime during the upgrade and refrain issuing queries. You can check the current status of the cluster with the describe-cluster command.
       operationId: upgradeCluster
       parameters:
@@ -1745,14 +1944,50 @@
   DescribeClusterResponse:
     type: object
     description: Response object for the describeCluster method.
     properties:
       cluster:
         description: The cluster.
         $ref: '#/definitions/ClusterSummaryResponse'
+  SuspendClusterRequest:
+    x-no-compatibility-guarantee: true
+    type: object
+    description: Request object for suspend cluster method.
+    required:
+      - clusterId
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the cluster to suspend.
+  ResumeClusterRequest:
+    x-no-compatibility-guarantee: true
+    type: object
+    description: Request object for resume cluster method.
+    required:
+      - clusterId
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the cluster to resume.
+  SuspendClusterResponse:
+    x-no-compatibility-guarantee: true
+    type: object
+    description: The response object for the suspendCluster method.
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the cluster to describe.
+  ResumeClusterResponse:
+    x-no-compatibility-guarantee: true
+    type: object
+    description: The response object for the resumeCluster method.
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the cluster to describe.
   DescribeKubeconfigRequest:
     type: object
     description: Request object for the describeKubeconfig method.
     required:
       - clusterId
     properties:
       clusterId:
@@ -1780,20 +2015,20 @@
     description: Response object for the describeAllowedInstanceTypes method.
   AllowedInstanceTypes:
     type: object
     description: Allowed compute instance type values and default compute instance type value.
     properties:
       default:
         type: array
-        description: Default value for the compute instance type usage.
+        description: Default value for the compute instance type usage. This setting is Cluster-wide.
         items:
           type: string
       allowed:
         type: array
-        description: Allowed values for the instance type.
+        description: Allowed values for the instance type. This setting is Cluster-wide.
         items:
           type: string
   DescribeServerSettingRequest:
     type: object
     description: Request object for the describeServerSetting method.
     x-form-factors: private
   DescribeServerSettingResponse:
@@ -1862,14 +2097,64 @@
     properties:
       configurationKey:
         type: string
         description: The identifier of the setting.
       enabled:
         type: boolean
         description: The state of the setting.
+  ListEventsRequest:
+    x-form-factors: public,private
+    type: object
+    description: Request object for the listEvents method.
+    properties:
+      operationId:
+        type: string
+        description: Filter events based on the operation ID. Either operation ID or service ID is required.
+      serviceId:
+        type: string
+        description: Filter events based on the service ID. It can be Cluster ID, Database Catalog ID, Virtual Warehouse ID or Data Visualization App ID.
+      limit:
+        type: integer
+        format: int32
+        description: Limit the number of returned rows. If not specified then the recent 20 events will be returned. The maximum is 100.
+      ascending:
+        type: boolean
+        default: false
+        description: Provide the result in ascending order, default is descending.
+  ListEventsResponse:
+    x-form-factors: public,private
+    type: object
+    description: Response object for the listEvents method.
+    properties:
+      events:
+        type: array
+        description: List of the events.
+        items:
+          $ref: '#/definitions/Event'
+  Event:
+    x-form-factors: public,private
+    type: object
+    description: Represents a Event.
+    properties:
+      operationId:
+        type: string
+        description: The ID of the operation to which the event belongs.
+      serviceId:
+        type: string
+        description: The ID of the service to which the event belongs.
+      event:
+        type: string
+        description: The name of the event.
+      message:
+        type: string
+        description: Detailed message.
+      timestamp:
+        type: string
+        format: date-time
+        description: The timestamp of the event.
   UpdateSshKeyRequest:
     type: object
     description: Request object for the updateSshKey method.
     required:
       - clusterId
     properties:
       clusterId:
@@ -1964,14 +2249,234 @@
       privateCloudOptions:
         description: Options for activating a Private Cloud environment.
         $ref: '#/definitions/PrivateCloudActivationOptions'
         x-form-factors: private
       customSubdomain:
         type: string
         description: Custom environment subdomain. Overrides the environment subdomain using a customized domain either in the old subdomain format like ENV_ID.dw or the new format like dw-ENV_NAME.
+  CreateAwsClusterRequest:
+    type: object
+    description: Request object for the createAwsCluster method.
+    required:
+      - environmentCrn
+    properties:
+      environmentCrn:
+        type: string
+        description: The CRN of the environment for the cluster to create.
+      useOverlayNetwork:
+        type: boolean
+        description: Using an overlay network will save IP addresses in the VPC by using a private IP address range for Pods in the cluster.
+      databaseBackupRetentionPeriod:
+        type: integer
+        format: int32
+        default: 30
+        description: PostgreSQL server backup retention days.
+      whitelistK8sClusterAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for kubernetes cluster access.
+      whitelistWorkloadAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for workload access.
+      usePrivateLoadBalancer:
+        type: boolean
+        description: Set up load balancer with private IP address. In AWS it is created in private subnets. In Azure an internal load balancer gets created. Make sure there is connectivity between your client network and the network (VPC/VNet) where CDW environment is deployed.
+      usePublicWorkerNode:
+        type: boolean
+        description: Set up worker node with public IP address. In AWS it is created in public subnets.
+      enableStorageRoles:
+        type: boolean
+        description: Enable Storage Roles
+        default: false
+        x-form-factors: public
+        x-entitlement: CDW_STORAGE_ROLES
+      reservedComputeNodes:
+        x-entitlement: CDW_CLUSTER_OVERPROVISIONER
+        type: integer
+        format: int32
+        description: Set additional number of nodes to reserve for executors and coordinators to use during autoscaling. Adding more reserved nodes increases your cloud costs.
+      reservedSharedServicesNodes:
+        x-entitlement: CDW_CLUSTER_OVERPROVISIONER
+        type: integer
+        format: int32
+        description: Set additional number of nodes to reserve for other services in the cluster. Adding more reserved nodes increases your cloud costs.
+      customRegistryOptions:
+        description: Options for custom ACR/ECR/Docker registries.
+        $ref: '#/definitions/CustomRegistryOptions'
+      customSubdomain:
+        type: string
+        description: Custom environment subdomain. Overrides the environment subdomain using a customized domain either in the old subdomain format like ENV_ID.dw or the new format like dw-ENV_NAME.
+      privateSubnetIds:
+        type: array
+        description: IDs of private AWS subnets where the cluster should be deployed.
+        items:
+          type: string
+      publicSubnetIds:
+        type: array
+        description: IDs of public AWS subnets where the cluster should be deployed.
+        items:
+          type: string
+      workerSubnetIds:
+        type: array
+        description: IDs of AWS subnets where the cluster worker nodes should be deployed.
+        items:
+          type: string
+      lbSubnetIds:
+        type: array
+        description: IDs of AWS subnets where the cluster load balancer should be deployed.
+        items:
+          type: string
+      customAmiId:
+        type: string
+        description: Custom AMI ID.
+      nodeRoleCDWManagedPolicyArn:
+        type: string
+        description: Managed Policy Arn to be attached to the Node Instance Role.
+      enableSpotInstances:
+        type: boolean
+        description: Whether to enable Spot instances for Virtual warehouses. It cannot be updated later. Defaults to false.
+        default: false
+      reducedPermissionMode:
+        type: boolean
+        description: Use this option to activate the environment with fewer than half of the standard required IAM permissions on your AWS cross-account IAM role.
+      computeInstanceTypes:
+        type: array
+        items:
+          type: string
+        description: AWS compute instance types that the environment is restricted to use. This affects the creation of virtual warehouses where this restriction will apply. Select an instance type that meets your computing, memory, networking, or storage needs. As of now, only a single instance type can be listed. Use describe-allowed-instance-types to see currently possible values.
+      additionalInstanceTypes:
+        type: array
+        items:
+          type: string
+        description: Additional (fallback) instance types listed in their priority order. They will be used instead of the primary compute instance type in case it is unavailable. You cannot include any instance type that was already indicated in computeInstanceTypes. Use describe-allowed-instance-types to see currently supported values and also the default value when nothing is provided for the computeInstanceTypes.
+  CreateAzureClusterRequest:
+    type: object
+    description: Request object for the createAzureCluster method.
+    required:
+      - environmentCrn
+      - userAssignedManagedIdentity
+    properties:
+      environmentCrn:
+        type: string
+        description: The CRN of the environment for the cluster to create.
+      userAssignedManagedIdentity:
+        type: string
+        description: Resource ID of the managed identity used by AKS. It is a mandatory parameter for Azure cluster creation.
+      subnetId:
+        type: string
+        description: ID of Azure subnet where the cluster should be deployed. It is a mandatory parameter for Azure cluster creation.
+      kubenet:
+        type: boolean
+        description: With kubenet, nodes get an IP address from the Azure virtual network subnet. Pods receive an IP address from a logically different address space to the Azure virtual network subnet of the nodes.
+      databaseBackupRetentionPeriod:
+        type: integer
+        format: int32
+        default: 30
+        description: PostgreSQL server backup retention days.
+      whitelistK8sClusterAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for kubernetes cluster access.
+      whitelistWorkloadAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for workload access.
+      usePrivateLoadBalancer:
+        type: boolean
+        description: Set up load balancer with private IP address. An internal load balancer gets created. Make sure there is connectivity between your client network and the network VNet where CDW environment is deployed.
+      enableStorageRoles:
+        type: boolean
+        description: Enable Storage Roles
+        default: false
+        x-form-factors: public
+        x-entitlement: CDW_STORAGE_ROLES
+      reservedComputeNodes:
+        x-entitlement: CDW_CLUSTER_OVERPROVISIONER
+        type: integer
+        format: int32
+        description: Set additional number of nodes to reserve for executors and coordinators to use during autoscaling. Adding more reserved nodes increases your cloud costs.
+      reservedSharedServicesNodes:
+        x-entitlement: CDW_CLUSTER_OVERPROVISIONER
+        type: integer
+        format: int32
+        description: Set additional number of nodes to reserve for other services in the cluster. Adding more reserved nodes increases your cloud costs.
+      customRegistryOptions:
+        description: Options for custom ACR/ECR/Docker registries.
+        $ref: '#/definitions/CustomRegistryOptions'
+      customSubdomain:
+        type: string
+        description: Custom environment subdomain. Overrides the environment subdomain using a customized domain either in the old subdomain format like ENV_ID.dw or the new format like dw-ENV_NAME.
+      enableAZ:
+        type: boolean
+        description: Enables Azure Availability Zones for the cluster deployment.
+      enableSpotInstances:
+        type: boolean
+        description: Whether to enable spot instances for Virtual warehouses. It cannot be updated later. Defaults to false.
+        default: false
+      computeInstanceTypes:
+        type: array
+        items:
+          type: string
+        description: Azure compute instance types that the environment is restricted to use. This affects the creation of virtual warehouses where this restriction will apply. Select an instance type that meets your computing, memory, networking, or storage needs. As of now, only a single instance type can be listed. Use describe-allowed-instance-types to see currently possible values and the default value used for the case it is not provided.
+      logAnalyticsWorkspaceId:
+        type: string
+        description: Enable monitoring of Azure Kubernetes Service (AKS) cluster. Workspace ID for Azure log analytics.
+      outboundType:
+        type: string
+        description: Network outbound type. This setting controls the egress traffic for cluster nodes in Azure Kubernetes Service. Please refer to the following AKS documentation on the Azure portal. https://learn.microsoft.com/en-us/azure/aks/egress-outboundtype, https://learn.microsoft.com/en-us/azure/aks/nat-gateway
+        enum:
+          - LoadBalancer
+          - UserAssignedNATGateway
+          - UserDefinedRouting
+      enablePrivateSQL:
+        type: boolean
+        description: Enables private SQL for the cluster deployment.
+        default: false
+      privateDNSZoneAKS:
+        type: string
+        description: Private DNS zone AKS resource ID.
+      enablePrivateAks:
+        type: boolean
+        description: Enable Azure Private AKS mode. Note that this feature is currently unstable due to critical networking issues within the Azure Software Definition Layer (SDN). This problem prevents the deployment of necessary components and results in unpredictable behavior and instability, impacting operations such as environment activation, VW creation, modification, and start/stop operations. While we work towards a resolution with Microsoft, estimated within the next 6-9 months, we recommend utilizing alternative methods like enabling public endpoints or virtual network peering for accessing your Azure Cluster.
+        default: false
+      aksVNetIntegrationSubnetName:
+        type: string
+        description: Enable AKS VNet Azure Virtual Network (VNet) integration by specifying the delegated subnet name. An Azure Kubernetes Service (AKS) cluster configured with API Server VNet Integration projects the API server endpoint directly into a delegated subnet in the VNet where AKS is deployed. API Server VNet Integration enables network communication between the API server and the cluster nodes without requiring a private link or tunnel.
+  CreatePrivateClusterRequest:
+    x-form-factors: private
+    type: object
+    description: Request object for the createPrivateCluster method.
+    required:
+      - environmentCrn
+      - delegationUsername
+      - delegationPassword
+    properties:
+      environmentCrn:
+        type: string
+        description: The CRN of the environment for the cluster to create.
+      delegationUsername:
+        type: string
+        description: Name of delegation user. This user is used between Hue - Impala to create a session, as Hue should not pass the user credentials, instead Hue authenticates with the delegation user, then this user will impersonate the logged in user. This means that the Delegation User and Password should be able to authenticate through LDAP.
+      delegationPassword:
+        type: string
+        description: Password of delegation user.
+      securityContextConstraintName:
+        type: string
+        description: The name of the Hive Security Context Constraint.
+      storageClass:
+        type: string
+        description: The storage class for the Local Storage Operator.
+      dbHue:
+        type: string
+        description: The name of the HUE database. Not required for embedded databases.
   BackupClusterRequest:
     type: object
     description: Request object for the backupCluster method.
     required:
       - clusterId
     properties:
       clusterId:
@@ -2018,14 +2523,20 @@
     properties:
       clusterId:
         type: string
         description: The the ID of the cluster.
       operationId:
         type: string
         description: The the ID of the restore operation.
+      action:
+        type: string
+        description: 'The cluster action. Possible actions: Create, Skip'
+      message:
+        type: string
+        description: The description of the cluster action.
       dbcRestorePlans:
         type: array
         description: Information about the restore-plan of the DbCatalogs.
         items:
           $ref: '#/definitions/RestoreClusterEntityPlan'
       hueRestorePlans:
         type: array
@@ -2087,26 +2598,14 @@
       disableImageVerification:
         type: boolean
         description: Disable image verification.
   AwsActivationOptions:
     type: object
     description: Options for activating an AWS environment.
     properties:
-      privateSubnetIds:
-        type: array
-        description: DEPRECATED in favour of workerSubnetIds and lbSubnetIds field. IDs of private AWS subnets where the cluster should be deployed.
-        x-deprecated: true
-        items:
-          type: string
-      publicSubnetIds:
-        type: array
-        description: DEPRECATED in favour of workerSubnetIds and lbSubnetIds field. IDs of public AWS subnets where the cluster should be deployed.
-        x-deprecated: true
-        items:
-          type: string
       workerSubnetIds:
         type: array
         description: IDs of AWS subnets where the cluster worker nodes should be deployed.
         items:
           type: string
       lbSubnetIds:
         type: array
@@ -2210,14 +2709,36 @@
   CreateClusterResponse:
     type: object
     description: Response object for the createCluster method.
     properties:
       clusterId:
         type: string
         description: ID of new cluster.
+  CreateAwsClusterResponse:
+    type: object
+    description: Response object for the createAwsCluster method.
+    properties:
+      clusterId:
+        type: string
+        description: ID of new AWS cluster.
+  CreateAzureClusterResponse:
+    type: object
+    description: Response object for the createCluster method.
+    properties:
+      clusterId:
+        type: string
+        description: ID of new Azure cluster.
+  CreatePrivateClusterResponse:
+    x-form-factors: private
+    type: object
+    description: Response object for the createPrivateCluster method.
+    properties:
+      clusterId:
+        type: string
+        description: ID of new Private Cloud cluster.
   DeleteClusterRequest:
     type: object
     description: Request object for the deleteCluster method.
     properties:
       clusterId:
         type: string
         description: The ID of the cluster to delete.
@@ -2300,14 +2821,96 @@
           renewCertificate:
             type: boolean
             default: false
             description: Renew Azure cluster certificate.
       observabilityConfig:
         description: Cluster observability configurations to update. You can forward logs from environments activated in Cloudera Data Warehouse (CDW) to observability and monitoring systems such as Datadog, New Relic, or Splunk. Please refer to the following Cloudera documentation for more info. https://docs.cloudera.com/data-warehouse/cloud/monitoring/topics/dw-observability-log-forwarding.html
         $ref: '#/definitions/UpdateClusterObservabilityConfig'
+  UpdateAwsClusterRequest:
+    type: object
+    description: Request object for the updateAwsCluster method.
+    required:
+      - clusterId
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the AWS cluster to update.
+      description:
+        type: string
+        description: Cluster description.
+      whitelistK8sClusterAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for kubernetes cluster access.
+      whitelistWorkloadAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for workload access.
+      observabilityConfig:
+        description: Cluster observability configurations to update. You can forward logs from environments activated in Cloudera Data Warehouse (CDW) to observability and monitoring systems such as Datadog, New Relic, or Splunk. Please refer to the following Cloudera documentation for more info. https://docs.cloudera.com/data-warehouse/cloud/monitoring/topics/dw-observability-log-forwarding.html
+        $ref: '#/definitions/UpdateClusterObservabilityConfig'
+      externalBuckets:
+        type: object
+        description: Cluster external bucket definition to update.
+        additionalProperties:
+          description: External bucket access information.
+          $ref: '#/definitions/UpdateClusterExternalBucketAccessInfo'
+  UpdateAzureClusterRequest:
+    type: object
+    description: Request object for the updateAzureCluster method.
+    required:
+      - clusterId
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the Azure cluster to update.
+      description:
+        type: string
+        description: Cluster description.
+      whitelistK8sClusterAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for kubernetes cluster access.
+      whitelistWorkloadAccessIpCIDRs:
+        type: array
+        items:
+          type: string
+        description: List of IP address CIDRs to whitelist for workload access.
+      observabilityConfig:
+        description: Cluster observability configurations to update. You can forward logs from environments activated in Cloudera Data Warehouse (CDW) to observability and monitoring systems such as Datadog, New Relic, or Splunk. Please refer to the following Cloudera documentation for more info. https://docs.cloudera.com/data-warehouse/cloud/monitoring/topics/dw-observability-log-forwarding.html
+        $ref: '#/definitions/UpdateClusterObservabilityConfig'
+      renewCertificate:
+        type: boolean
+        default: false
+        description: Renew Azure cluster certificate.
+  UpdatePrivateClusterRequest:
+    x-form-factors: private
+    type: object
+    description: Request object for the updatePrivateCluster method.
+    required:
+      - clusterId
+    properties:
+      clusterId:
+        type: string
+        description: The ID of the Private Cloud cluster to update.
+      description:
+        type: string
+        description: Cluster description.
+      delegationUsername:
+        type: string
+        description: The user name to update for delegation user. Setting it to the same value as the existing delegation user name will be a no-op.
+      delegationPassword:
+        type: string
+        description: The password to update for delegation user. Setting it to the same value as the existing password will be a no-op.
+      dedicatedExecutorNodes:
+        type: boolean
+        description: Set it true to enable dedicated nodes exclusively for executors and coordinators, and improve performance. You can enable this only if you reserve nodes while adding a CDP Private Cloud containerized ECS cluster. When disabled, non-compute pods such as MetaStore and Data Visualization can also use the reserved nodes.
   ExternalBucketAccessInfo:
     type: object
     description: External bucket definition.
     properties:
       accessMode:
         type: string
         description: Specifies whether the external bucket will be added in read-only or read-write mode.
@@ -2339,14 +2942,24 @@
         description: Create the log forwarding configuration in a valid fluentd format. Then that configuration is later inserted into a larger fluentd configuration.
       proxyCABundle:
         type: string
         description: Set the proxy CA certificates (PEM Bundle). If you use a TLS-terminating proxy server to inspect outbound internet traffic, you need to provide the proxy server's CA certificates bundle in PEM bundle format when you configure log forwarding.
   UpdateClusterResponse:
     type: object
     description: Response object for the updateCluster method.
+  UpdateAwsClusterResponse:
+    type: object
+    description: Response object for the updateAwsCluster method.
+  UpdateAzureClusterResponse:
+    type: object
+    description: Response object for the updateAzureCluster method.
+  UpdatePrivateClusterResponse:
+    x-form-factors: private
+    type: object
+    description: Response object for the updatePrivateCluster method.
   ListClustersRequest:
     type: object
     description: Request object for the listClusters method.
     properties:
       environmentCrn:
         type: string
         description: Filter returned clusters for the belonging Environment CRN.
@@ -4571,14 +5184,27 @@
     properties:
       clusterId:
         type: string
         description: ID of the Virtual Warehouse's cluster.
       vwId:
         type: string
         description: ID of the Virtual Warehouse.
+      template:
+        type: string
+        description: Name of configuration template to use.
+        enum:
+          - xsmall
+          - small
+          - medium
+          - large
+      nodeCount:
+        type: integer
+        format: int32
+        default: 0
+        description: Nodes per compute cluster. If specified, forces 'template' to be 'custom'
       config:
         description: The service configuration to update the VW with. This will be applied on top of the existing configuration so there's no need to list configurations that stay the same.
         $ref: '#/definitions/ServiceConfigReq'
       autoscaling:
         description: Autoscaling settings for the Virtual Warehouse.
         $ref: '#/definitions/AutoscalingOptionsUpdateRequest'
       impalaHaSettings:
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/environments/environments.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/environments/environments.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: environments2
 x-display-name: environments
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Environments Service
   license:
     name: Apache 2.0
   description: Cloudera Environments Service is a web service that manages cloud provider access.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1795,14 +1795,56 @@
           description: Expected response to a valid request.
           schema:
             $ref: '#/definitions/UpdateProxyConfigResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/environments2/updateAzureImageTermsPolicy:
+    post:
+      summary: Updates account level Azure Marketplace image policy. CDP is capable to automatically accept Azure Marketplace image terms during cluster deployment. You can use this setting in your account to opt in or opt out this behaviour.
+      description: Updates account level Azure Marketplace image policy. CDP is capable to automatically accept Azure Marketplace image terms during cluster deployment. You can use this setting in your account to opt in or opt out this behaviour.
+      operationId: updateAzureImageTermsPolicy
+      x-mutating: true
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdateAzureImageTermsPolicyRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdateAzureImageTermsPolicyResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+  /api/v1/environments2/getAzureImageTermsPolicy:
+    post:
+      summary: Gets account level Azure Marketplace image policy. CDP is capable to automatically accept Azure Marketplace image terms during cluster deployment. You can use this setting in your account to opt in or opt out this behaviour.
+      description: Gets account level Azure Marketplace image policy. CDP is capable to automatically accept Azure Marketplace image terms during cluster deployment. You can use this setting in your account to opt in or opt out this behaviour.
+      operationId: getAzureImageTermsPolicy
+      x-mutating: false
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/GetAzureImageTermsPolicyRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/GetAzureImageTermsPolicyResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
 definitions:
   Error:
     type: object
     description: An object returned on an error.
     properties:
       code:
         type: string
@@ -2198,14 +2240,23 @@
         type: string
         description: The related role definition json encoded in base64
       policies:
         type: array
         description: The fine-grained policies related to each service.
         items:
           $ref: '#/definitions/CredentialGranularPolicyResponse'
+  GcpCredentialPrerequisitesResponse:
+    type: object
+    description: Response object for getting GCP credential prerequisites.
+    required:
+      - serviceAccountCreationCommand
+    properties:
+      serviceAccountCreationCommand:
+        type: string
+        description: GCP CLI command to create service account encoded in base64.
   GetGovCloudCredentialPrerequisitesRequest:
     type: object
     description: Request object for getting the credential prerequisites for GovCloud for the enabled providers.
     required:
       - cloudPlatform
     properties:
       cloudPlatform:
@@ -4741,14 +4792,38 @@
         description: Flag to enable environment level workload analytics.
       reportDeploymentLogs:
         type: boolean
         description: Flag to enable environment level deployment log collection.
   SetTelemetryFeaturesResponse:
     type: object
     description: Response object to enable environment level telemetry features.
+  UpdateAzureImageTermsPolicyRequest:
+    type: object
+    description: Request object to enable or disable automatic acceptance of Azure Marketplace image terms.
+    required:
+      - accepted
+    properties:
+      accepted:
+        type: boolean
+        description: Flag to enable or disable automatic acceptance of Azure Marketplace image terms.
+  UpdateAzureImageTermsPolicyResponse:
+    type: object
+    description: Response object to enable or disable automatic acceptance of Azure Marketplace image terms.
+  GetAzureImageTermsPolicyRequest:
+    type: object
+    description: Request object to retrieve current value of setting that controls automatic acceptance of Azure Marketplace image terms.
+  GetAzureImageTermsPolicyResponse:
+    type: object
+    description: Response object to retrieve current value of setting that controls automatic acceptance of Azure Marketplace image terms.
+    required:
+      - accepted
+    properties:
+      accepted:
+        type: boolean
+        description: Flag denoting whether automatic Azure Marketplace image terms acceptance is enabled or disabled.
   GetEnvironmentSettingRequest:
     x-form-factors: private
     type: object
     description: Request object to query environment configuration settings.
     required:
       - attrs
     properties:
@@ -5136,14 +5211,15 @@
       - cloudPlatform
     properties:
       cloudPlatform:
         type: string
         enum:
           - AWS
           - AZURE
+          - GCP
         description: The kind of cloud platform.
   GetAuditCredentialPrerequisitesResponse:
     type: object
     description: The audit credential prerequisites.
     required:
       - cloudPlatform
     properties:
@@ -5155,14 +5231,17 @@
         description: The provider specific identifier of the account/subscription/project that is used by Cloudbreak.
       aws:
         description: Provides the external id and policy JSON (this one encoded in base64) for AWS credential creation.
         $ref: '#/definitions/AwsCredentialPrerequisitesResponse'
       azure:
         description: Provides the app creation command and role definition Json for Azure credential creation.
         $ref: '#/definitions/AzureCredentialPrerequisitesResponse'
+      gcp:
+        description: Provides the service account creation command for GCP credential creation.
+        $ref: '#/definitions/GcpCredentialPrerequisitesResponse'
   GetGovCloudAuditCredentialPrerequisitesRequest:
     type: object
     description: Request object for getting the audit credential prerequisites for GovCloud for the enabled providers.
     required:
       - cloudPlatform
     properties:
       cloudPlatform:
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/iam/iam.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/iam/iam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: iam
 x-products: ALTUS,CDP
 x-form-factors: public,private
 x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera IAM Service
   license:
     name: Apache 2.0
   description: Cloudera CDP IAM is a web service that you can use to manage users and user permissions under your CDP account.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/imagecatalog/imagecatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: imagecatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Image catalog service
   license:
     name: Apache 2.0
   description: Service for managing custom image catalogs and their associated Cloudera Runtime and FreeIPA images.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/metrics/metrics.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/metrics/metrics.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 produces:
   - application/json
 info:
   description: Cloudera Private Cloud Control Plane Monitoring Metrics Administration API
   license:
     name: Apache 2.0
   title: Cloudera Control Plane Monitoring Metrics Administration
-  version: 0.9.98
+  version: 0.9.99
 x-audit: true
 paths:
   /api/v1/metrics/createRemoteWriteConfig:
     post:
       summary: Create remote storage configuration
       description: Creates a new remote storage configuration.
       operationId: createRemoteWriteConfig
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/ml/ml.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/ml/ml.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: ml
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Machine Learning
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Machine Learning applications.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/opdb/opdb.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/opdb/opdb.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: opdb
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Operational Database service
   license:
     name: Apache 2.0
   description: Interact with the Cloudera Operational Database service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -753,20 +753,14 @@
         type: string
         description: Override subnet where the database will be deployed. Disables Multi-AZ if set.
       customUserTags:
         type: array
         items:
           $ref: '#/definitions/KeyValuePair'
         description: Optional tags to apply to launched infrastructure resources
-      useHdfs:
-        type: boolean
-        description: Controls whether hbase root be deployed on hdfs
-      disableEphemeralStorage:
-        type: boolean
-        description: Disable large block cache on ephemeral storage.
       disableMultiAz:
         type: boolean
         description: Disable deployment into multiple availability-zones (the database will be deployed into one subnet).
       attachedStorageForWorkers:
         description: Attached storage for the worker nodes for AWS, Azure, and GCP cloud providers.
         $ref: '#/definitions/AttachedStorageForWorkers'
       disableKerberos:
@@ -802,14 +796,17 @@
       enableGrafana:
         type: boolean
         description: To enable grafana server for the database.
       javaVersion:
         type: integer
         format: int32
         description: Optional tag to configure the major version of Java on the cluster.
+      computeClusterId:
+        type: string
+        description: Uses provided compute cluster for Kubernetes clusters instead of creating a new one.
   VolumeType:
     type: string
     description: "Volume Type.\n `HDD` - Hard disk drives (HDD) volume type. Default is HDD. `SSD` - Solid disk drives (SSD) volume type. `LOCAL_SSD` - Local SSD volume type."
     enum:
       - HDD
       - SSD
       - LOCAL_SSD
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-beta-0.9.99/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: replicationmanager
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.98
+  version: 0.9.99
   title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
   description: Create and manage replication policies using Cloudera Replication Manager.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/doc/docstringparser.py` & `cdpcli-beta-0.9.99/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/doc/restdoc.py` & `cdpcli-beta-0.9.99/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/doc/style.py` & `cdpcli-beta-0.9.99/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/docs.py` & `cdpcli-beta-0.9.99/cdpcli/docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/endpoint.py` & `cdpcli-beta-0.9.99/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/examples/configure/_description.rst` & `cdpcli-beta-0.9.99/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/examples/configure/get/_description.rst` & `cdpcli-beta-0.9.99/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-beta-0.9.99/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/examples/configure/set/_description.rst` & `cdpcli-beta-0.9.99/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-beta-0.9.99/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/exceptions.py` & `cdpcli-beta-0.9.99/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/__init__.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/arguments.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/cliinputjson.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/commands.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/commands.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/configure/__init__.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/configure/classify.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/configure/configure.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/configure/get.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/configure/list.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/configure/set.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/df/__init__.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/df/createdeployment.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/df/createdeployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,24 @@
             },
             'listenComponents': {
                 'type': 'array',
                 'description': 'Listen components port and protocol data',
                 'items': {
                     '$ref': '#/definitions/ListenComponent'
                 }
+            },
+            'nodeStorageProfileName': {
+                'type': 'string',
+                'description': 'Node storage profile name',
+                'enum': [
+                    'STANDARD_AWS',
+                    'STANDARD_AZURE',
+                    'PERFORMANCE_AWS',
+                    'PERFORMANCE_AZURE'
+                ]
             }
         }
     },
     'CreateDeploymentResponse': {
         'type': 'object',
         'description': 'Response for Create Deployment command.',
         'properties': {
@@ -527,14 +537,22 @@
             'name': parameters.get('deploymentName', None),
             'deploymentRequestCrn': deployment_request_crn,
             'configurationVersion': INITIAL_CONFIGURATION_VERSION,
             'clusterSizeName': parameters.get('clusterSizeName', 'EXTRA_SMALL'),
             'staticNodeCount': parameters.get('staticNodeCount', 1)
         }
 
+        # If nodeStorageProfileName is not set, then
+        # sending it as empty in the configuration will trigger
+        # dfx-local to choose the default nodeStorageProfileName for
+        # the given cloud platform
+        nodeStorageProfileName = parameters.get('nodeStorageProfileName', None)
+        if nodeStorageProfileName is not None:
+            deployment_configuration['nodeStorageProfileName'] = nodeStorageProfileName
+
         inboundHostname = parameters.get('inboundHostname', None)
         if inboundHostname is not None:
             deployment_configuration['inboundHostname'] = inboundHostname
             deployment_configuration['listenComponents'] = \
                 parameters.get('listenComponents', None)
 
         autoScalingEnabled = parameters.get('autoScalingEnabled', None)
```

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/df/register.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/interactivelogin.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/logout.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/paginate.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/redirect.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/refdoc.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/workload.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/extensions/writer.py` & `cdpcli-beta-0.9.99/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/formatter.py` & `cdpcli-beta-0.9.99/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/help.py` & `cdpcli-beta-0.9.99/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/loader.py` & `cdpcli-beta-0.9.99/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/main.py` & `cdpcli-beta-0.9.99/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/model.py` & `cdpcli-beta-0.9.99/cdpcli/model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/paginate.py` & `cdpcli-beta-0.9.99/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/paramfile.py` & `cdpcli-beta-0.9.99/cdpcli/paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/paramformfactor.py` & `cdpcli-beta-0.9.99/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/parser.py` & `cdpcli-beta-0.9.99/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/retryhandler.py` & `cdpcli-beta-0.9.99/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/schema.py` & `cdpcli-beta-0.9.99/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/serialize.py` & `cdpcli-beta-0.9.99/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/shorthand.py` & `cdpcli-beta-0.9.99/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/signers.py` & `cdpcli-beta-0.9.99/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/table.py` & `cdpcli-beta-0.9.99/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/text.py` & `cdpcli-beta-0.9.99/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/textwriter.py` & `cdpcli-beta-0.9.99/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/thirdparty/six.py` & `cdpcli-beta-0.9.99/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/translate.py` & `cdpcli-beta-0.9.99/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/utils.py` & `cdpcli-beta-0.9.99/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli/validate.py` & `cdpcli-beta-0.9.99/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/cdpcli_beta.egg-info/PKG-INFO` & `cdpcli-beta-0.9.99/cdpcli_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.98
+Version: 0.9.99
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.98/cdpcli_beta.egg-info/SOURCES.txt` & `cdpcli-beta-0.9.99/cdpcli_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/setup.py` & `cdpcli-beta-0.9.99/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/setup_common.py` & `cdpcli-beta-0.9.99/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/__init__.py` & `cdpcli-beta-0.9.99/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/cdp/__init__.py` & `cdpcli-beta-0.9.99/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/__init__.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_classify.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_configure.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_get.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_list.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/configure/test_set.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/df/test_createdeployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,14 +264,15 @@
             create_deployment_parameters[0])
 
     def test_invoke_create_deployment(self):
         self.maxDiff = 2000
         service_crn = 'SERVICE_CRN'
         flow_version_crn = 'FLOW_VERSION_CRN'
         deployment_name = 'DEPLOYMENT'
+        node_storage_profile_name = 'STANDARD_AWS'
 
         parameter_group_name = 'ParameterGroup'
         parameter_name = 'Files'
         asset_reference_name = 'df-workload.asset.bin'
         asset_reference_file_path = os.path.join(BASE_DIR, asset_reference_name)
 
         frequencyUnit = {
@@ -329,15 +330,16 @@
                         }
                     ]
                 }
             ],
             'kpis': [
                 kpi
             ],
-            'customNarConfiguration': custom_nar_configuration
+            'customNarConfiguration': custom_nar_configuration,
+            'nodeStorageProfileName': node_storage_profile_name
         }
         parsed_args = {}
         parsed_globals = Mock()
         parsed_globals.output = 'json'
 
         environment_crn = 'ENVIRONMENT_CRN'
         deployment_request_crn = 'DEPLOYMENT_REQUEST_CRN'
@@ -466,15 +468,16 @@
                             }
                         ]
                     }
                 ],
                 'kpis': [
                     kpi
                 ],
-                'customNarConfigurationCrn': custom_nar_configuration_crn
+                'customNarConfigurationCrn': custom_nar_configuration_crn,
+                'nodeStorageProfileName': node_storage_profile_name
             },
             create_deployment_parameters[0])
 
         custom_nar_configuration['environmentCrn'] = environment_crn
         self.assertEquals(
             custom_nar_configuration,
             create_custom_nar_configuration_params[0]
```

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_df.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_logout.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_operation_extension.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_paginate.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_redirect.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_workload.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/extensions/test_writer.py` & `cdpcli-beta-0.9.99/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_argparser.py` & `cdpcli-beta-0.9.99/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_argprocess.py` & `cdpcli-beta-0.9.99/tests/unit/test_argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_auth.py` & `cdpcli-beta-0.9.99/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_cli_data.py` & `cdpcli-beta-0.9.99/tests/unit/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_client.py` & `cdpcli-beta-0.9.99/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_completer.py` & `cdpcli-beta-0.9.99/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_credentials.py` & `cdpcli-beta-0.9.99/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_docs.py` & `cdpcli-beta-0.9.99/tests/unit/test_docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_endpoint.py` & `cdpcli-beta-0.9.99/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_help.py` & `cdpcli-beta-0.9.99/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_loaders.py` & `cdpcli-beta-0.9.99/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_model.py` & `cdpcli-beta-0.9.99/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_paginate.py` & `cdpcli-beta-0.9.99/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_paramfile.py` & `cdpcli-beta-0.9.99/tests/unit/test_paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_protocol.py` & `cdpcli-beta-0.9.99/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_retryhandler.py` & `cdpcli-beta-0.9.99/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_shorthand.py` & `cdpcli-beta-0.9.99/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_signers.py` & `cdpcli-beta-0.9.99/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_table_formatter.py` & `cdpcli-beta-0.9.99/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_utils.py` & `cdpcli-beta-0.9.99/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/tests/unit/test_validate.py` & `cdpcli-beta-0.9.99/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.98/versioneer.py` & `cdpcli-beta-0.9.99/versioneer.py`

 * *Files identical despite different names*

