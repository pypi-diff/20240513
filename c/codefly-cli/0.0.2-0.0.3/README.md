# Comparing `tmp/codefly_cli-0.0.2.tar.gz` & `tmp/codefly_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefly_cli-0.0.2.tar", max compression
+gzip compressed data, was "codefly_cli-0.0.3.tar", max compression
```

## Comparing `codefly_cli-0.0.2.tar` & `codefly_cli-0.0.3.tar`

### file list

```diff
@@ -1,94 +1,133 @@
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/actions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/actions/v0/__init__.py
--rw-r--r--   0        0        0     2004 2024-05-13 13:49:13.446542 codefly_cli-0.0.2/codefly_cli/actions/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448403 codefly_cli-0.0.2/codefly_cli/actions/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2009 2024-05-13 13:49:13.448579 codefly_cli-0.0.2/codefly_cli/actions/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.447517 codefly_cli-0.0.2/codefly_cli/actions/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     3743 2024-05-13 13:49:13.447494 codefly_cli-0.0.2/codefly_cli/actions/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.446585 codefly_cli-0.0.2/codefly_cli/actions/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2588 2024-05-13 13:49:13.448454 codefly_cli-0.0.2/codefly_cli/actions/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448732 codefly_cli-0.0.2/codefly_cli/actions/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/base/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/base/v0/__init__.py
--rw-r--r--   0        0        0     2399 2024-05-13 13:49:13.447867 codefly_cli-0.0.2/codefly_cli/base/v0/agent_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448589 codefly_cli-0.0.2/codefly_cli/base/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     2500 2024-05-13 13:49:13.448413 codefly_cli-0.0.2/codefly_cli/base/v0/configuration_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.446805 codefly_cli-0.0.2/codefly_cli/base/v0/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     5828 2024-05-13 13:49:13.449218 codefly_cli-0.0.2/codefly_cli/base/v0/endpoint_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449713 codefly_cli-0.0.2/codefly_cli/base/v0/endpoint_pb2_grpc.py
--rw-r--r--   0        0        0     2169 2024-05-13 13:49:13.449335 codefly_cli-0.0.2/codefly_cli/base/v0/environment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449018 codefly_cli-0.0.2/codefly_cli/base/v0/environment_pb2_grpc.py
--rw-r--r--   0        0        0     2402 2024-05-13 13:49:13.448914 codefly_cli-0.0.2/codefly_cli/base/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448654 codefly_cli-0.0.2/codefly_cli/base/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2768 2024-05-13 13:49:13.449677 codefly_cli-0.0.2/codefly_cli/base/v0/network_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.451000 codefly_cli-0.0.2/codefly_cli/base/v0/network_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-05-13 13:49:13.449946 codefly_cli-0.0.2/codefly_cli/base/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449931 codefly_cli-0.0.2/codefly_cli/base/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2024-05-13 13:49:13.450029 codefly_cli-0.0.2/codefly_cli/base/v0/scope_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450124 codefly_cli-0.0.2/codefly_cli/base/v0/scope_pb2_grpc.py
--rw-r--r--   0        0        0     4669 2024-05-13 13:49:13.450065 codefly_cli-0.0.2/codefly_cli/base/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450638 codefly_cli-0.0.2/codefly_cli/base/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2414 2024-05-13 13:49:13.450683 codefly_cli-0.0.2/codefly_cli/base/v0/spec_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450790 codefly_cli-0.0.2/codefly_cli/base/v0/spec_pb2_grpc.py
--rw-r--r--   0        0        0     3318 2024-05-13 13:49:13.450982 codefly_cli-0.0.2/codefly_cli/base/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450985 codefly_cli-0.0.2/codefly_cli/base/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/buf/__init__.py
--rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.2/codefly_cli/buf/validate/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/buf/validate/__init__.py
--rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.2/codefly_cli/buf/validate/expression.proto
--rw-r--r--   0        0        0     2292 2024-05-13 13:49:13.450790 codefly_cli-0.0.2/codefly_cli/buf/validate/expression_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450818 codefly_cli-0.0.2/codefly_cli/buf/validate/expression_pb2_grpc.py
--rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/__init__.py
--rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private.proto
--rw-r--r--   0        0        0     2332 2024-05-13 13:49:13.450797 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.451295 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.2/codefly_cli/buf/validate/validate.proto
--rw-r--r--   0        0        0   144402 2024-05-13 13:49:13.452802 codefly_cli-0.0.2/codefly_cli/buf/validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452137 codefly_cli-0.0.2/codefly_cli/buf/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/cli/v0/__init__.py
--rw-r--r--   0        0        0    11732 2024-05-13 13:49:13.451372 codefly_cli-0.0.2/codefly_cli/cli/v0/cli_pb2.py
--rw-r--r--   0        0        0    28562 2024-05-13 13:49:13.452428 codefly_cli-0.0.2/codefly_cli/cli/v0/cli_pb2_grpc.py
--rw-r--r--   0        0        0     4042 2024-05-13 13:46:59.095948 codefly_cli-0.0.2/codefly_cli/codefly.py
--rw-r--r--   0        0        0     1792 2024-05-13 13:49:13.453277 codefly_cli-0.0.2/codefly_cli/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453501 codefly_cli-0.0.2/codefly_cli/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2690 2024-05-13 13:49:13.453447 codefly_cli-0.0.2/codefly_cli/google/api/http_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453409 codefly_cli-0.0.2/codefly_cli/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/observability/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/observability/v0/__init__.py
--rw-r--r--   0        0        0     2474 2024-05-13 13:49:13.452611 codefly_cli-0.0.2/codefly_cli/observability/v0/dependencies_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452686 codefly_cli-0.0.2/codefly_cli/observability/v0/dependencies_pb2_grpc.py
--rw-r--r--   0        0        0     1837 2024-05-13 13:49:13.452443 codefly_cli-0.0.2/codefly_cli/observability/v0/inventory_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452782 codefly_cli-0.0.2/codefly_cli/observability/v0/inventory_pb2_grpc.py
--rw-r--r--   0        0        0     2961 2024-05-13 13:49:13.452547 codefly_cli-0.0.2/codefly_cli/observability/v0/logs_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453108 codefly_cli-0.0.2/codefly_cli/observability/v0/logs_pb2_grpc.py
--rw-r--r--   0        0        0     2098 2024-05-13 13:49:13.453294 codefly_cli-0.0.2/codefly_cli/observability/v0/metrics_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454033 codefly_cli-0.0.2/codefly_cli/observability/v0/metrics_pb2_grpc.py
--rw-r--r--   0        0        0     2985 2024-05-13 13:49:13.454381 codefly_cli-0.0.2/codefly_cli/observability/v0/sessions_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453846 codefly_cli-0.0.2/codefly_cli/observability/v0/sessions_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/agent/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/agent/v0/__init__.py
--rw-r--r--   0        0        0     5107 2024-05-13 13:49:13.453465 codefly_cli-0.0.2/codefly_cli/services/agent/v0/agent_pb2.py
--rw-r--r--   0        0        0     2895 2024-05-13 13:49:13.454028 codefly_cli-0.0.2/codefly_cli/services/agent/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     6560 2024-05-13 13:49:13.454342 codefly_cli-0.0.2/codefly_cli/services/agent/v0/communicate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454415 codefly_cli-0.0.2/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
--rw-r--r--   0        0        0     2426 2024-05-13 13:49:13.454363 codefly_cli-0.0.2/codefly_cli/services/agent/v0/cyclonedx_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454382 codefly_cli-0.0.2/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/builder/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/builder/v0/__init__.py
--rw-r--r--   0        0        0    11603 2024-05-13 13:49:13.455038 codefly_cli-0.0.2/codefly_cli/services/builder/v0/builder_pb2.py
--rw-r--r--   0        0        0    15720 2024-05-13 13:49:13.455498 codefly_cli-0.0.2/codefly_cli/services/builder/v0/builder_pb2_grpc.py
--rw-r--r--   0        0        0     3239 2024-05-13 13:49:13.455801 codefly_cli-0.0.2/codefly_cli/services/builder/v0/deployment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.455001 codefly_cli-0.0.2/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
--rw-r--r--   0        0        0     1959 2024-05-13 13:49:13.455543 codefly_cli-0.0.2/codefly_cli/services/builder/v0/docker_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.455789 codefly_cli-0.0.2/codefly_cli/services/builder/v0/docker_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/runtime/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/runtime/v0/__init__.py
--rw-r--r--   0        0        0    11345 2024-05-13 13:49:13.455933 codefly_cli-0.0.2/codefly_cli/services/runtime/v0/runtime_pb2.py
--rw-r--r--   0        0        0    15818 2024-05-13 13:49:13.456279 codefly_cli-0.0.2/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
--rw-r--r--   0        0        0      171 2024-05-11 14:38:58.454178 codefly_cli-0.0.2/codefly_cli/tests/test_cli.py
--rw-r--r--   0        0        0      481 2024-05-13 13:50:35.890474 codefly_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 codefly_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.3/codefly_cli/actions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/actions/v0/__init__.py
+-rw-r--r--   0        0        0     2004 2024-05-13 13:49:13.446542 codefly_cli-0.0.3/codefly_cli/actions/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448403 codefly_cli-0.0.3/codefly_cli/actions/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2009 2024-05-13 13:49:13.448579 codefly_cli-0.0.3/codefly_cli/actions/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.447517 codefly_cli-0.0.3/codefly_cli/actions/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     3743 2024-05-13 13:49:13.447494 codefly_cli-0.0.3/codefly_cli/actions/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.446585 codefly_cli-0.0.3/codefly_cli/actions/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2588 2024-05-13 13:49:13.448454 codefly_cli-0.0.3/codefly_cli/actions/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448732 codefly_cli-0.0.3/codefly_cli/actions/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.3/codefly_cli/base/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-13 14:09:42.444829 codefly_cli-0.0.3/codefly_cli/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/base/v0/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-13 13:43:44.892103 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1676 2024-05-13 13:49:49.184868 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1855 2024-05-13 13:49:49.188891 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     3371 2024-05-13 13:49:49.183146 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1615 2024-05-13 13:49:49.202244 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1791 2024-05-13 13:49:49.179812 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1950 2024-05-13 13:49:49.203856 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1704 2024-05-13 13:49:49.190337 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2613 2024-05-13 13:49:49.181480 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1701 2024-05-13 13:49:49.199660 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2168 2024-05-13 13:49:49.122019 codefly_cli-0.0.3/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2399 2024-05-13 13:49:13.447867 codefly_cli-0.0.3/codefly_cli/base/v0/agent_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448589 codefly_cli-0.0.3/codefly_cli/base/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     2500 2024-05-13 13:49:13.448413 codefly_cli-0.0.3/codefly_cli/base/v0/configuration_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.446805 codefly_cli-0.0.3/codefly_cli/base/v0/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     5828 2024-05-13 13:49:13.449218 codefly_cli-0.0.3/codefly_cli/base/v0/endpoint_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449713 codefly_cli-0.0.3/codefly_cli/base/v0/endpoint_pb2_grpc.py
+-rw-r--r--   0        0        0     2169 2024-05-13 13:49:13.449335 codefly_cli-0.0.3/codefly_cli/base/v0/environment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449018 codefly_cli-0.0.3/codefly_cli/base/v0/environment_pb2_grpc.py
+-rw-r--r--   0        0        0     2402 2024-05-13 13:49:13.448914 codefly_cli-0.0.3/codefly_cli/base/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448654 codefly_cli-0.0.3/codefly_cli/base/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2768 2024-05-13 13:49:13.449677 codefly_cli-0.0.3/codefly_cli/base/v0/network_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.451000 codefly_cli-0.0.3/codefly_cli/base/v0/network_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-05-13 13:49:13.449946 codefly_cli-0.0.3/codefly_cli/base/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449931 codefly_cli-0.0.3/codefly_cli/base/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2024-05-13 13:49:13.450029 codefly_cli-0.0.3/codefly_cli/base/v0/scope_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450124 codefly_cli-0.0.3/codefly_cli/base/v0/scope_pb2_grpc.py
+-rw-r--r--   0        0        0     4669 2024-05-13 13:49:13.450065 codefly_cli-0.0.3/codefly_cli/base/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450638 codefly_cli-0.0.3/codefly_cli/base/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2414 2024-05-13 13:49:13.450683 codefly_cli-0.0.3/codefly_cli/base/v0/spec_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450790 codefly_cli-0.0.3/codefly_cli/base/v0/spec_pb2_grpc.py
+-rw-r--r--   0        0        0     3318 2024-05-13 13:49:13.450982 codefly_cli-0.0.3/codefly_cli/base/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450985 codefly_cli-0.0.3/codefly_cli/base/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/buf/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-13 13:47:20.622712 codefly_cli-0.0.3/codefly_cli/buf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.3/codefly_cli/buf/validate/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/buf/validate/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-13 13:47:20.623558 codefly_cli-0.0.3/codefly_cli/buf/validate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1735 2024-05-13 13:49:49.171523 codefly_cli-0.0.3/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0   105220 2024-05-13 13:49:49.169873 codefly_cli-0.0.3/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.3/codefly_cli/buf/validate/expression.proto
+-rw-r--r--   0        0        0     2292 2024-05-13 13:49:13.450790 codefly_cli-0.0.3/codefly_cli/buf/validate/expression_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450818 codefly_cli-0.0.3/codefly_cli/buf/validate/expression_pb2_grpc.py
+-rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.3/codefly_cli/buf/validate/priv/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.3/codefly_cli/buf/validate/priv/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-11 14:39:48.143074 codefly_cli-0.0.3/codefly_cli/buf/validate/priv/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1833 2024-05-13 13:49:49.173958 codefly_cli-0.0.3/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.3/codefly_cli/buf/validate/priv/private.proto
+-rw-r--r--   0        0        0     2332 2024-05-13 13:49:13.450797 codefly_cli-0.0.3/codefly_cli/buf/validate/priv/private_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.451295 codefly_cli-0.0.3/codefly_cli/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.3/codefly_cli/buf/validate/validate.proto
+-rw-r--r--   0        0        0   144402 2024-05-13 13:49:13.452802 codefly_cli-0.0.3/codefly_cli/buf/validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452137 codefly_cli-0.0.3/codefly_cli/buf/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/cli/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-13 13:43:44.884477 codefly_cli-0.0.3/codefly_cli/cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/cli/v0/__init__.py
+-rw-r--r--   0        0        0      196 2024-05-13 13:43:44.885610 codefly_cli-0.0.3/codefly_cli/cli/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7578 2024-05-13 13:49:49.187411 codefly_cli-0.0.3/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    10048 2024-05-13 13:49:49.118488 codefly_cli-0.0.3/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0    11732 2024-05-13 13:49:13.451372 codefly_cli-0.0.3/codefly_cli/cli/v0/cli_pb2.py
+-rw-r--r--   0        0        0    28562 2024-05-13 13:49:13.452428 codefly_cli-0.0.3/codefly_cli/cli/v0/cli_pb2_grpc.py
+-rw-r--r--   0        0        0     4170 2024-05-13 14:13:11.788124 codefly_cli-0.0.3/codefly_cli/codefly.py
+-rw-r--r--   0        0        0     1517 2024-05-13 13:49:49.218228 codefly_cli-0.0.3/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1912 2024-05-13 13:49:49.220245 codefly_cli-0.0.3/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1792 2024-05-13 13:49:13.453277 codefly_cli-0.0.3/codefly_cli/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453501 codefly_cli-0.0.3/codefly_cli/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2690 2024-05-13 13:49:13.453447 codefly_cli-0.0.3/codefly_cli/google/api/http_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453409 codefly_cli-0.0.3/codefly_cli/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/observability/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-13 13:47:20.666896 codefly_cli-0.0.3/codefly_cli/observability/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/observability/v0/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-13 13:47:20.667998 codefly_cli-0.0.3/codefly_cli/observability/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-05-13 13:49:49.211153 codefly_cli-0.0.3/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1550 2024-05-13 13:49:49.209688 codefly_cli-0.0.3/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2265 2024-05-13 13:49:49.213031 codefly_cli-0.0.3/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2214 2024-05-13 13:49:49.214782 codefly_cli-0.0.3/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2474 2024-05-13 13:49:13.452611 codefly_cli-0.0.3/codefly_cli/observability/v0/dependencies_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452686 codefly_cli-0.0.3/codefly_cli/observability/v0/dependencies_pb2_grpc.py
+-rw-r--r--   0        0        0     1837 2024-05-13 13:49:13.452443 codefly_cli-0.0.3/codefly_cli/observability/v0/inventory_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452782 codefly_cli-0.0.3/codefly_cli/observability/v0/inventory_pb2_grpc.py
+-rw-r--r--   0        0        0     2961 2024-05-13 13:49:13.452547 codefly_cli-0.0.3/codefly_cli/observability/v0/logs_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453108 codefly_cli-0.0.3/codefly_cli/observability/v0/logs_pb2_grpc.py
+-rw-r--r--   0        0        0     2098 2024-05-13 13:49:13.453294 codefly_cli-0.0.3/codefly_cli/observability/v0/metrics_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454033 codefly_cli-0.0.3/codefly_cli/observability/v0/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0     2985 2024-05-13 13:49:13.454381 codefly_cli-0.0.3/codefly_cli/observability/v0/sessions_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453846 codefly_cli-0.0.3/codefly_cli/observability/v0/sessions_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/services/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-13 13:47:20.650463 codefly_cli-0.0.3/codefly_cli/services/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/services/agent/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-13 13:47:20.651647 codefly_cli-0.0.3/codefly_cli/services/agent/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/services/agent/v0/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-13 13:47:20.652542 codefly_cli-0.0.3/codefly_cli/services/agent/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3328 2024-05-13 13:49:49.194622 codefly_cli-0.0.3/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4050 2024-05-13 13:49:49.205929 codefly_cli-0.0.3/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     5107 2024-05-13 13:49:13.453465 codefly_cli-0.0.3/codefly_cli/services/agent/v0/agent_pb2.py
+-rw-r--r--   0        0        0     2895 2024-05-13 13:49:13.454028 codefly_cli-0.0.3/codefly_cli/services/agent/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     6560 2024-05-13 13:49:13.454342 codefly_cli-0.0.3/codefly_cli/services/agent/v0/communicate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454415 codefly_cli-0.0.3/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
+-rw-r--r--   0        0        0     2426 2024-05-13 13:49:13.454363 codefly_cli-0.0.3/codefly_cli/services/agent/v0/cyclonedx_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454382 codefly_cli-0.0.3/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/services/builder/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/services/builder/v0/__init__.py
+-rw-r--r--   0        0        0    11603 2024-05-13 13:49:13.455038 codefly_cli-0.0.3/codefly_cli/services/builder/v0/builder_pb2.py
+-rw-r--r--   0        0        0    15720 2024-05-13 13:49:13.455498 codefly_cli-0.0.3/codefly_cli/services/builder/v0/builder_pb2_grpc.py
+-rw-r--r--   0        0        0     3239 2024-05-13 13:49:13.455801 codefly_cli-0.0.3/codefly_cli/services/builder/v0/deployment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.455001 codefly_cli-0.0.3/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     1959 2024-05-13 13:49:13.455543 codefly_cli-0.0.3/codefly_cli/services/builder/v0/docker_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.455789 codefly_cli-0.0.3/codefly_cli/services/builder/v0/docker_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/services/runtime/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-13 13:47:20.655031 codefly_cli-0.0.3/codefly_cli/services/runtime/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.3/codefly_cli/services/runtime/v0/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-13 13:47:20.655871 codefly_cli-0.0.3/codefly_cli/services/runtime/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7530 2024-05-13 13:49:49.198194 codefly_cli-0.0.3/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    11345 2024-05-13 13:49:13.455933 codefly_cli-0.0.3/codefly_cli/services/runtime/v0/runtime_pb2.py
+-rw-r--r--   0        0        0    15818 2024-05-13 13:49:13.456279 codefly_cli-0.0.3/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
+-rw-r--r--   0        0        0      713 2024-05-13 14:13:15.469467 codefly_cli-0.0.3/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0      171 2024-05-13 14:10:06.354079 codefly_cli-0.0.3/codefly_cli/tests/test_cli.py
+-rw-r--r--   0        0        0      481 2024-05-13 14:30:31.425144 codefly_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 codefly_cli-0.0.3/PKG-INFO
```

### Comparing `codefly_cli-0.0.2/codefly_cli/actions/v0/module_pb2.py` & `codefly_cli-0.0.3/codefly_cli/actions/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/actions/v0/organization_pb2.py` & `codefly_cli-0.0.3/codefly_cli/actions/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/actions/v0/service_pb2.py` & `codefly_cli-0.0.3/codefly_cli/actions/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/actions/v0/workspace_pb2.py` & `codefly_cli-0.0.3/codefly_cli/actions/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/agent_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/configuration_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/endpoint_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/environment_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/module_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/network_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/network_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/organization_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/scope_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/service_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/spec_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/base/v0/workspace_pb2.py` & `codefly_cli-0.0.3/codefly_cli/base/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/buf/validate/BUILD.bazel` & `codefly_cli-0.0.3/codefly_cli/buf/validate/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/buf/validate/expression.proto` & `codefly_cli-0.0.3/codefly_cli/buf/validate/expression.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/buf/validate/expression_pb2.py` & `codefly_cli-0.0.3/codefly_cli/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/buf/validate/priv/BUILD.bazel` & `codefly_cli-0.0.3/codefly_cli/buf/validate/priv/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private.proto` & `codefly_cli-0.0.3/codefly_cli/buf/validate/priv/private.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private_pb2.py` & `codefly_cli-0.0.3/codefly_cli/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/buf/validate/validate.proto` & `codefly_cli-0.0.3/codefly_cli/buf/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/buf/validate/validate_pb2.py` & `codefly_cli-0.0.3/codefly_cli/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/cli/v0/cli_pb2.py` & `codefly_cli-0.0.3/codefly_cli/cli/v0/cli_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/cli/v0/cli_pb2_grpc.py` & `codefly_cli-0.0.3/codefly_cli/cli/v0/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/codefly.py` & `codefly_cli-0.0.3/codefly_cli/codefly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+import os, sys
+file_dir = os.path.dirname(os.path.abspath(__file__))
+# Add the directory to sys.path
+sys.path.append(file_dir)
+
 import subprocess
 import time
 import grpc
 from typing import Optional, List
 
 from codefly_sdk.codefly import init
```

### Comparing `codefly_cli-0.0.2/codefly_cli/google/api/annotations_pb2.py` & `codefly_cli-0.0.3/codefly_cli/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/google/api/http_pb2.py` & `codefly_cli-0.0.3/codefly_cli/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/observability/v0/dependencies_pb2.py` & `codefly_cli-0.0.3/codefly_cli/observability/v0/dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/observability/v0/inventory_pb2.py` & `codefly_cli-0.0.3/codefly_cli/observability/v0/inventory_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/observability/v0/logs_pb2.py` & `codefly_cli-0.0.3/codefly_cli/observability/v0/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/observability/v0/metrics_pb2.py` & `codefly_cli-0.0.3/codefly_cli/observability/v0/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/observability/v0/sessions_pb2.py` & `codefly_cli-0.0.3/codefly_cli/observability/v0/sessions_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/agent/v0/agent_pb2.py` & `codefly_cli-0.0.3/codefly_cli/services/agent/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/agent/v0/agent_pb2_grpc.py` & `codefly_cli-0.0.3/codefly_cli/services/agent/v0/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/agent/v0/communicate_pb2.py` & `codefly_cli-0.0.3/codefly_cli/services/agent/v0/communicate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/agent/v0/cyclonedx_pb2.py` & `codefly_cli-0.0.3/codefly_cli/services/agent/v0/cyclonedx_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/builder/v0/builder_pb2.py` & `codefly_cli-0.0.3/codefly_cli/services/builder/v0/builder_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/builder/v0/builder_pb2_grpc.py` & `codefly_cli-0.0.3/codefly_cli/services/builder/v0/builder_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/builder/v0/deployment_pb2.py` & `codefly_cli-0.0.3/codefly_cli/services/builder/v0/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/builder/v0/docker_pb2.py` & `codefly_cli-0.0.3/codefly_cli/services/builder/v0/docker_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/runtime/v0/runtime_pb2.py` & `codefly_cli-0.0.3/codefly_cli/services/runtime/v0/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py` & `codefly_cli-0.0.3/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.2/PKG-INFO` & `codefly_cli-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefly-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Antoine Toussaint
 Author-email: antoine.toussaint@codefly.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

