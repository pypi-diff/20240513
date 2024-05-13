# Comparing `tmp/codefly_cli-0.0.1.tar.gz` & `tmp/codefly_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefly_cli-0.0.1.tar", max compression
+gzip compressed data, was "codefly_cli-0.0.2.tar", max compression
```

## Comparing `codefly_cli-0.0.1.tar` & `codefly_cli-0.0.2.tar`

### file list

```diff
@@ -1,78 +1,94 @@
--rw-r--r--   0        0        0     2004 2024-05-10 20:30:20.177933 codefly_cli-0.0.1/codefly_cli/actions/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.180110 codefly_cli-0.0.1/codefly_cli/actions/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2009 2024-05-10 20:30:20.177929 codefly_cli-0.0.1/codefly_cli/actions/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.177116 codefly_cli-0.0.1/codefly_cli/actions/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     3743 2024-05-10 20:30:20.177547 codefly_cli-0.0.1/codefly_cli/actions/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.177854 codefly_cli-0.0.1/codefly_cli/actions/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2588 2024-05-10 20:30:20.178407 codefly_cli-0.0.1/codefly_cli/actions/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.177883 codefly_cli-0.0.1/codefly_cli/actions/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0     2399 2024-05-10 20:30:20.179371 codefly_cli-0.0.1/codefly_cli/base/v0/agent_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.177820 codefly_cli-0.0.1/codefly_cli/base/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     2500 2024-05-10 20:30:20.178265 codefly_cli-0.0.1/codefly_cli/base/v0/configuration_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.178422 codefly_cli-0.0.1/codefly_cli/base/v0/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     5828 2024-05-10 20:30:20.181292 codefly_cli-0.0.1/codefly_cli/base/v0/endpoint_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.178951 codefly_cli-0.0.1/codefly_cli/base/v0/endpoint_pb2_grpc.py
--rw-r--r--   0        0        0     2169 2024-05-10 20:30:20.178745 codefly_cli-0.0.1/codefly_cli/base/v0/environment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.179172 codefly_cli-0.0.1/codefly_cli/base/v0/environment_pb2_grpc.py
--rw-r--r--   0        0        0     2402 2024-05-10 20:30:20.179002 codefly_cli-0.0.1/codefly_cli/base/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.179132 codefly_cli-0.0.1/codefly_cli/base/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2768 2024-05-10 20:30:20.179130 codefly_cli-0.0.1/codefly_cli/base/v0/network_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.180315 codefly_cli-0.0.1/codefly_cli/base/v0/network_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-05-10 20:30:20.179186 codefly_cli-0.0.1/codefly_cli/base/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.180143 codefly_cli-0.0.1/codefly_cli/base/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2024-05-10 20:30:20.180176 codefly_cli-0.0.1/codefly_cli/base/v0/scope_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.181615 codefly_cli-0.0.1/codefly_cli/base/v0/scope_pb2_grpc.py
--rw-r--r--   0        0        0     4669 2024-05-10 20:30:20.181447 codefly_cli-0.0.1/codefly_cli/base/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.181304 codefly_cli-0.0.1/codefly_cli/base/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2414 2024-05-10 20:30:20.181320 codefly_cli-0.0.1/codefly_cli/base/v0/spec_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.181634 codefly_cli-0.0.1/codefly_cli/base/v0/spec_pb2_grpc.py
--rw-r--r--   0        0        0     3318 2024-05-10 20:30:20.181733 codefly_cli-0.0.1/codefly_cli/base/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.181813 codefly_cli-0.0.1/codefly_cli/base/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-05-10 18:40:43.976778 codefly_cli-0.0.1/codefly_cli/buf/__init__.py
--rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.1/codefly_cli/buf/validate/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-05-10 18:40:43.971863 codefly_cli-0.0.1/codefly_cli/buf/validate/__init__.py
--rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.1/codefly_cli/buf/validate/expression.proto
--rw-r--r--   0        0        0     2292 2024-05-10 20:30:20.182026 codefly_cli-0.0.1/codefly_cli/buf/validate/expression_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.182064 codefly_cli-0.0.1/codefly_cli/buf/validate/expression_pb2_grpc.py
--rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.1/codefly_cli/buf/validate/priv/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.1/codefly_cli/buf/validate/priv/__init__.py
--rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.1/codefly_cli/buf/validate/priv/private.proto
--rw-r--r--   0        0        0     2332 2024-05-10 20:30:20.182099 codefly_cli-0.0.1/codefly_cli/buf/validate/priv/private_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.181997 codefly_cli-0.0.1/codefly_cli/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.1/codefly_cli/buf/validate/validate.proto
--rw-r--r--   0        0        0   144402 2024-05-10 20:30:20.184363 codefly_cli-0.0.1/codefly_cli/buf/validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.182595 codefly_cli-0.0.1/codefly_cli/buf/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0    11732 2024-05-10 20:30:20.183306 codefly_cli-0.0.1/codefly_cli/cli/v0/cli_pb2.py
--rw-r--r--   0        0        0    28562 2024-05-10 20:30:20.182588 codefly_cli-0.0.1/codefly_cli/cli/v0/cli_pb2_grpc.py
--rw-r--r--   0        0        0     4156 2024-05-11 14:43:01.916175 codefly_cli-0.0.1/codefly_cli/codefly.py
--rw-r--r--   0        0        0     1792 2024-05-10 20:30:20.182613 codefly_cli-0.0.1/codefly_cli/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.182842 codefly_cli-0.0.1/codefly_cli/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2690 2024-05-10 20:30:20.182875 codefly_cli-0.0.1/codefly_cli/google/api/http_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.183367 codefly_cli-0.0.1/codefly_cli/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0     2474 2024-05-10 20:30:20.184126 codefly_cli-0.0.1/codefly_cli/observability/v0/dependencies_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.183982 codefly_cli-0.0.1/codefly_cli/observability/v0/dependencies_pb2_grpc.py
--rw-r--r--   0        0        0     1837 2024-05-10 20:30:20.184101 codefly_cli-0.0.1/codefly_cli/observability/v0/inventory_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.183839 codefly_cli-0.0.1/codefly_cli/observability/v0/inventory_pb2_grpc.py
--rw-r--r--   0        0        0     2961 2024-05-10 20:30:20.183860 codefly_cli-0.0.1/codefly_cli/observability/v0/logs_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.184610 codefly_cli-0.0.1/codefly_cli/observability/v0/logs_pb2_grpc.py
--rw-r--r--   0        0        0     2098 2024-05-10 20:30:20.184313 codefly_cli-0.0.1/codefly_cli/observability/v0/metrics_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.184206 codefly_cli-0.0.1/codefly_cli/observability/v0/metrics_pb2_grpc.py
--rw-r--r--   0        0        0     2985 2024-05-10 20:30:20.184231 codefly_cli-0.0.1/codefly_cli/observability/v0/sessions_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.184601 codefly_cli-0.0.1/codefly_cli/observability/v0/sessions_pb2_grpc.py
--rw-r--r--   0        0        0     5107 2024-05-10 20:30:20.184759 codefly_cli-0.0.1/codefly_cli/services/agent/v0/agent_pb2.py
--rw-r--r--   0        0        0     2895 2024-05-10 20:30:20.184952 codefly_cli-0.0.1/codefly_cli/services/agent/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     6560 2024-05-10 20:30:20.185081 codefly_cli-0.0.1/codefly_cli/services/agent/v0/communicate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.185131 codefly_cli-0.0.1/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
--rw-r--r--   0        0        0     2426 2024-05-10 20:30:20.185656 codefly_cli-0.0.1/codefly_cli/services/agent/v0/cyclonedx_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.185612 codefly_cli-0.0.1/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
--rw-r--r--   0        0        0    11603 2024-05-10 20:30:20.186118 codefly_cli-0.0.1/codefly_cli/services/builder/v0/builder_pb2.py
--rw-r--r--   0        0        0    15720 2024-05-10 20:30:20.185736 codefly_cli-0.0.1/codefly_cli/services/builder/v0/builder_pb2_grpc.py
--rw-r--r--   0        0        0     3239 2024-05-10 20:30:20.185223 codefly_cli-0.0.1/codefly_cli/services/builder/v0/deployment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.185948 codefly_cli-0.0.1/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
--rw-r--r--   0        0        0     1959 2024-05-10 20:30:20.186084 codefly_cli-0.0.1/codefly_cli/services/builder/v0/docker_pb2.py
--rw-r--r--   0        0        0      159 2024-05-10 20:30:20.186141 codefly_cli-0.0.1/codefly_cli/services/builder/v0/docker_pb2_grpc.py
--rw-r--r--   0        0        0    11345 2024-05-10 20:30:20.186481 codefly_cli-0.0.1/codefly_cli/services/runtime/v0/runtime_pb2.py
--rw-r--r--   0        0        0    15818 2024-05-10 20:30:20.186228 codefly_cli-0.0.1/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
--rw-r--r--   0        0        0      171 2024-05-11 14:38:58.454178 codefly_cli-0.0.1/codefly_cli/tests/test_cli.py
--rw-r--r--   0        0        0      481 2024-05-11 14:39:36.441270 codefly_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 codefly_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/actions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/actions/v0/__init__.py
+-rw-r--r--   0        0        0     2004 2024-05-13 13:49:13.446542 codefly_cli-0.0.2/codefly_cli/actions/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448403 codefly_cli-0.0.2/codefly_cli/actions/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2009 2024-05-13 13:49:13.448579 codefly_cli-0.0.2/codefly_cli/actions/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.447517 codefly_cli-0.0.2/codefly_cli/actions/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     3743 2024-05-13 13:49:13.447494 codefly_cli-0.0.2/codefly_cli/actions/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.446585 codefly_cli-0.0.2/codefly_cli/actions/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2588 2024-05-13 13:49:13.448454 codefly_cli-0.0.2/codefly_cli/actions/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448732 codefly_cli-0.0.2/codefly_cli/actions/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/base/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/base/v0/__init__.py
+-rw-r--r--   0        0        0     2399 2024-05-13 13:49:13.447867 codefly_cli-0.0.2/codefly_cli/base/v0/agent_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448589 codefly_cli-0.0.2/codefly_cli/base/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     2500 2024-05-13 13:49:13.448413 codefly_cli-0.0.2/codefly_cli/base/v0/configuration_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.446805 codefly_cli-0.0.2/codefly_cli/base/v0/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     5828 2024-05-13 13:49:13.449218 codefly_cli-0.0.2/codefly_cli/base/v0/endpoint_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449713 codefly_cli-0.0.2/codefly_cli/base/v0/endpoint_pb2_grpc.py
+-rw-r--r--   0        0        0     2169 2024-05-13 13:49:13.449335 codefly_cli-0.0.2/codefly_cli/base/v0/environment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449018 codefly_cli-0.0.2/codefly_cli/base/v0/environment_pb2_grpc.py
+-rw-r--r--   0        0        0     2402 2024-05-13 13:49:13.448914 codefly_cli-0.0.2/codefly_cli/base/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448654 codefly_cli-0.0.2/codefly_cli/base/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2768 2024-05-13 13:49:13.449677 codefly_cli-0.0.2/codefly_cli/base/v0/network_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.451000 codefly_cli-0.0.2/codefly_cli/base/v0/network_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-05-13 13:49:13.449946 codefly_cli-0.0.2/codefly_cli/base/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449931 codefly_cli-0.0.2/codefly_cli/base/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2024-05-13 13:49:13.450029 codefly_cli-0.0.2/codefly_cli/base/v0/scope_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450124 codefly_cli-0.0.2/codefly_cli/base/v0/scope_pb2_grpc.py
+-rw-r--r--   0        0        0     4669 2024-05-13 13:49:13.450065 codefly_cli-0.0.2/codefly_cli/base/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450638 codefly_cli-0.0.2/codefly_cli/base/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2414 2024-05-13 13:49:13.450683 codefly_cli-0.0.2/codefly_cli/base/v0/spec_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450790 codefly_cli-0.0.2/codefly_cli/base/v0/spec_pb2_grpc.py
+-rw-r--r--   0        0        0     3318 2024-05-13 13:49:13.450982 codefly_cli-0.0.2/codefly_cli/base/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450985 codefly_cli-0.0.2/codefly_cli/base/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/buf/__init__.py
+-rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.2/codefly_cli/buf/validate/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/buf/validate/__init__.py
+-rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.2/codefly_cli/buf/validate/expression.proto
+-rw-r--r--   0        0        0     2292 2024-05-13 13:49:13.450790 codefly_cli-0.0.2/codefly_cli/buf/validate/expression_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450818 codefly_cli-0.0.2/codefly_cli/buf/validate/expression_pb2_grpc.py
+-rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/__init__.py
+-rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private.proto
+-rw-r--r--   0        0        0     2332 2024-05-13 13:49:13.450797 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.451295 codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.2/codefly_cli/buf/validate/validate.proto
+-rw-r--r--   0        0        0   144402 2024-05-13 13:49:13.452802 codefly_cli-0.0.2/codefly_cli/buf/validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452137 codefly_cli-0.0.2/codefly_cli/buf/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/cli/v0/__init__.py
+-rw-r--r--   0        0        0    11732 2024-05-13 13:49:13.451372 codefly_cli-0.0.2/codefly_cli/cli/v0/cli_pb2.py
+-rw-r--r--   0        0        0    28562 2024-05-13 13:49:13.452428 codefly_cli-0.0.2/codefly_cli/cli/v0/cli_pb2_grpc.py
+-rw-r--r--   0        0        0     4042 2024-05-13 13:46:59.095948 codefly_cli-0.0.2/codefly_cli/codefly.py
+-rw-r--r--   0        0        0     1792 2024-05-13 13:49:13.453277 codefly_cli-0.0.2/codefly_cli/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453501 codefly_cli-0.0.2/codefly_cli/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2690 2024-05-13 13:49:13.453447 codefly_cli-0.0.2/codefly_cli/google/api/http_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453409 codefly_cli-0.0.2/codefly_cli/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/observability/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/observability/v0/__init__.py
+-rw-r--r--   0        0        0     2474 2024-05-13 13:49:13.452611 codefly_cli-0.0.2/codefly_cli/observability/v0/dependencies_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452686 codefly_cli-0.0.2/codefly_cli/observability/v0/dependencies_pb2_grpc.py
+-rw-r--r--   0        0        0     1837 2024-05-13 13:49:13.452443 codefly_cli-0.0.2/codefly_cli/observability/v0/inventory_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452782 codefly_cli-0.0.2/codefly_cli/observability/v0/inventory_pb2_grpc.py
+-rw-r--r--   0        0        0     2961 2024-05-13 13:49:13.452547 codefly_cli-0.0.2/codefly_cli/observability/v0/logs_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453108 codefly_cli-0.0.2/codefly_cli/observability/v0/logs_pb2_grpc.py
+-rw-r--r--   0        0        0     2098 2024-05-13 13:49:13.453294 codefly_cli-0.0.2/codefly_cli/observability/v0/metrics_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454033 codefly_cli-0.0.2/codefly_cli/observability/v0/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0     2985 2024-05-13 13:49:13.454381 codefly_cli-0.0.2/codefly_cli/observability/v0/sessions_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453846 codefly_cli-0.0.2/codefly_cli/observability/v0/sessions_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/agent/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/agent/v0/__init__.py
+-rw-r--r--   0        0        0     5107 2024-05-13 13:49:13.453465 codefly_cli-0.0.2/codefly_cli/services/agent/v0/agent_pb2.py
+-rw-r--r--   0        0        0     2895 2024-05-13 13:49:13.454028 codefly_cli-0.0.2/codefly_cli/services/agent/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     6560 2024-05-13 13:49:13.454342 codefly_cli-0.0.2/codefly_cli/services/agent/v0/communicate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454415 codefly_cli-0.0.2/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
+-rw-r--r--   0        0        0     2426 2024-05-13 13:49:13.454363 codefly_cli-0.0.2/codefly_cli/services/agent/v0/cyclonedx_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454382 codefly_cli-0.0.2/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/builder/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/builder/v0/__init__.py
+-rw-r--r--   0        0        0    11603 2024-05-13 13:49:13.455038 codefly_cli-0.0.2/codefly_cli/services/builder/v0/builder_pb2.py
+-rw-r--r--   0        0        0    15720 2024-05-13 13:49:13.455498 codefly_cli-0.0.2/codefly_cli/services/builder/v0/builder_pb2_grpc.py
+-rw-r--r--   0        0        0     3239 2024-05-13 13:49:13.455801 codefly_cli-0.0.2/codefly_cli/services/builder/v0/deployment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.455001 codefly_cli-0.0.2/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     1959 2024-05-13 13:49:13.455543 codefly_cli-0.0.2/codefly_cli/services/builder/v0/docker_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-13 13:49:13.455789 codefly_cli-0.0.2/codefly_cli/services/builder/v0/docker_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/runtime/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.2/codefly_cli/services/runtime/v0/__init__.py
+-rw-r--r--   0        0        0    11345 2024-05-13 13:49:13.455933 codefly_cli-0.0.2/codefly_cli/services/runtime/v0/runtime_pb2.py
+-rw-r--r--   0        0        0    15818 2024-05-13 13:49:13.456279 codefly_cli-0.0.2/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
+-rw-r--r--   0        0        0      171 2024-05-11 14:38:58.454178 codefly_cli-0.0.2/codefly_cli/tests/test_cli.py
+-rw-r--r--   0        0        0      481 2024-05-13 13:50:35.890474 codefly_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 codefly_cli-0.0.2/PKG-INFO
```

### Comparing `codefly_cli-0.0.1/codefly_cli/actions/v0/module_pb2.py` & `codefly_cli-0.0.2/codefly_cli/actions/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/actions/v0/organization_pb2.py` & `codefly_cli-0.0.2/codefly_cli/actions/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/actions/v0/service_pb2.py` & `codefly_cli-0.0.2/codefly_cli/actions/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/actions/v0/workspace_pb2.py` & `codefly_cli-0.0.2/codefly_cli/actions/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/agent_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/configuration_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/endpoint_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/environment_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/module_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/network_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/network_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/organization_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/scope_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/service_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/spec_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/base/v0/workspace_pb2.py` & `codefly_cli-0.0.2/codefly_cli/base/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/buf/validate/BUILD.bazel` & `codefly_cli-0.0.2/codefly_cli/buf/validate/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/buf/validate/expression.proto` & `codefly_cli-0.0.2/codefly_cli/buf/validate/expression.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/buf/validate/expression_pb2.py` & `codefly_cli-0.0.2/codefly_cli/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/buf/validate/priv/BUILD.bazel` & `codefly_cli-0.0.2/codefly_cli/buf/validate/priv/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/buf/validate/priv/private.proto` & `codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/buf/validate/priv/private_pb2.py` & `codefly_cli-0.0.2/codefly_cli/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/buf/validate/validate.proto` & `codefly_cli-0.0.2/codefly_cli/buf/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/buf/validate/validate_pb2.py` & `codefly_cli-0.0.2/codefly_cli/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/cli/v0/cli_pb2.py` & `codefly_cli-0.0.2/codefly_cli/cli/v0/cli_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/cli/v0/cli_pb2_grpc.py` & `codefly_cli-0.0.2/codefly_cli/cli/v0/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/codefly.py` & `codefly_cli-0.0.2/codefly_cli/codefly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-import sys
-import os
-
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), 'codefly_cli')))
-
 import subprocess
 import time
 import grpc
 from typing import Optional, List
-from google.protobuf.empty_pb2 import Empty
 
 from codefly_sdk.codefly import init
 
 from codefly_sdk.codefly import find_service_dir, unique_to_env_key
 
 import cli.v0.cli_pb2_grpc as cli_grpc
 import cli.v0.cli_pb2 as cli
 import base.v0.configuration_pb2 as configuration
 
+from google.protobuf.empty_pb2 import Empty
+
 
 def filter_configurations(configurations: List[configuration.Configuration], runtime_context: str) -> List[configuration.Configuration]:
     return [conf for conf in configurations if conf.runtime_context.kind == runtime_context]
 
 class Launcher:
     def __init__(self, root: str = "..", scope: str = "", show_cli_output: bool = False):
         self.cmd = None
```

### Comparing `codefly_cli-0.0.1/codefly_cli/google/api/annotations_pb2.py` & `codefly_cli-0.0.2/codefly_cli/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/google/api/http_pb2.py` & `codefly_cli-0.0.2/codefly_cli/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/observability/v0/dependencies_pb2.py` & `codefly_cli-0.0.2/codefly_cli/observability/v0/dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/observability/v0/inventory_pb2.py` & `codefly_cli-0.0.2/codefly_cli/observability/v0/inventory_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/observability/v0/logs_pb2.py` & `codefly_cli-0.0.2/codefly_cli/observability/v0/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/observability/v0/metrics_pb2.py` & `codefly_cli-0.0.2/codefly_cli/observability/v0/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/observability/v0/sessions_pb2.py` & `codefly_cli-0.0.2/codefly_cli/observability/v0/sessions_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/agent/v0/agent_pb2.py` & `codefly_cli-0.0.2/codefly_cli/services/agent/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/agent/v0/agent_pb2_grpc.py` & `codefly_cli-0.0.2/codefly_cli/services/agent/v0/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/agent/v0/communicate_pb2.py` & `codefly_cli-0.0.2/codefly_cli/services/agent/v0/communicate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/agent/v0/cyclonedx_pb2.py` & `codefly_cli-0.0.2/codefly_cli/services/agent/v0/cyclonedx_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/builder/v0/builder_pb2.py` & `codefly_cli-0.0.2/codefly_cli/services/builder/v0/builder_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/builder/v0/builder_pb2_grpc.py` & `codefly_cli-0.0.2/codefly_cli/services/builder/v0/builder_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/builder/v0/deployment_pb2.py` & `codefly_cli-0.0.2/codefly_cli/services/builder/v0/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/builder/v0/docker_pb2.py` & `codefly_cli-0.0.2/codefly_cli/services/builder/v0/docker_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/runtime/v0/runtime_pb2.py` & `codefly_cli-0.0.2/codefly_cli/services/runtime/v0/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py` & `codefly_cli-0.0.2/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.1/PKG-INFO` & `codefly_cli-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefly-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Antoine Toussaint
 Author-email: antoine.toussaint@codefly.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

