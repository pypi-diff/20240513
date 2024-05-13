# Comparing `tmp/resc_backend-3.1.2.tar.gz` & `tmp/resc_backend-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-3.1.2.tar", last modified: Mon May 13 14:12:39 2024, max compression
+gzip compressed data, was "resc_backend-4.0.0.tar", last modified: Tue Apr 30 15:21:35 2024, max compression
```

## Comparing `resc_backend-3.1.2.tar` & `resc_backend-4.0.0.tar`

### file list

```diff
@@ -1,117 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.265376 resc_backend-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 14:12:35.000000 resc_backend-3.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-13 14:12:39.265376 resc_backend-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-13 14:12:35.000000 resc_backend-3.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 14:12:35.000000 resc_backend-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-13 14:12:35.000000 resc_backend-3.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-13 14:12:39.265376 resc_backend-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-13 14:12:35.000000 resc_backend-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.249376 resc_backend-3.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.253376 resc_backend-3.1.2/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.253376 resc_backend-3.1.2/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.253376 resc_backend-3.1.2/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/engine_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.257376 resc_backend-3.1.2/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.257376 resc_backend-3.1.2/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/helpers/environment_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.257376 resc_backend-3.1.2/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.257376 resc_backend-3.1.2/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.257376 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    33218 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/rule_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.261376 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9582 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.261376 resc_backend-3.1.2/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13978 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/helpers/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.265376 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/time_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.265376 resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-13 14:12:35.000000 resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:12:39.265376 resc_backend-3.1.2/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-13 14:12:39.000000 resc_backend-3.1.2/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-13 14:12:39.000000 resc_backend-3.1.2/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:12:39.000000 resc_backend-3.1.2/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 14:12:39.000000 resc_backend-3.1.2/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:12:39.000000 resc_backend-3.1.2/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-13 14:12:39.000000 resc_backend-3.1.2/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 14:12:39.000000 resc_backend-3.1.2/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 15:21:29.000000 resc_backend-4.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-30 15:21:35.881999 resc_backend-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-30 15:21:29.000000 resc_backend-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-30 15:21:29.000000 resc_backend-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 15:21:35.885999 resc_backend-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 15:21:29.000000 resc_backend-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.865998 resc_backend-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.865998 resc_backend-4.0.0/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/engine_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.869998 resc_backend-4.0.0/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/environment_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.873998 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.873998 resc_backend-4.0.0/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.873998 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34253 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.877998 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20677 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.877998 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/audit_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/personal_audit_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/time_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 15:21:29.000000 resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:21:35.881999 resc_backend-4.0.0/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 15:21:35.000000 resc_backend-4.0.0/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-3.1.2/LICENSE.md` & `resc_backend-4.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/PKG-INFO` & `resc_backend-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.1.2
+Version: 4.0.0
 Summary: Repository Scanner - Backend
-Home-page: https://github.com/abnamro/resc-backend
+Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: celery==5.3.1
@@ -19,15 +19,15 @@
 Requires-Dist: pydantic==1.10.15
 Requires-Dist: uvicorn==0.17.6
 Requires-Dist: waitress==2.1.2
 Requires-Dist: pyjwt[crypto]==2.8.0
 Requires-Dist: cryptography==42.0.4
 Requires-Dist: tenacity==8.2.2
 Requires-Dist: tomlkit==0.12.1
-Requires-Dist: python-multipart==0.0.9
+Requires-Dist: python-multipart==0.0.7
 Requires-Dist: aiofiles==0.8.0
 Requires-Dist: packaging==23.1
 Requires-Dist: fastapi-cache2==0.2.1
 Requires-Dist: redis==4.6.0
 Requires-Dist: azure-identity==1.15.0
 Requires-Dist: setuptools==69.5.1
```

### Comparing `resc_backend-3.1.2/README.md` & `resc_backend-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/setup.cfg` & `resc_backend-4.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = resc_backend
 description = Repository Scanner - Backend
-version = 3.1.2
+version = 4.0.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
-url = https://github.com/abnamro/resc-backend
+url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
 requirements_files = file: requirements.txt
 
 [options]
```

### Comparing `resc_backend-3.1.2/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-4.0.0/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,22 @@
 env_variables = validate_environment(REQUIRED_ENV_VARS)
 logger = logging.getLogger(__name__)
 
 
 def create_cli_argparser() -> ArgumentParser:
     rabbitmq_service_host = f"{env_variables[RESC_RABBITMQ_SERVICE_HOST]}"
     rabbitmq_service_port = f"{env_variables[RESC_RABBITMQ_SERVICE_PORT_MGMT]}"
-    rabbitmq_api_base_url = "http://" + rabbitmq_service_host + ":" + rabbitmq_service_port
+    rabbitmq_api_base_url = (
+        "http://" + rabbitmq_service_host + ":" + rabbitmq_service_port
+    )
 
     parser: ArgumentParser = ArgumentParser()
-    parser.add_argument("--rabbitmq-url", type=str, default=rabbitmq_api_base_url, help="RabbitMQ URL")
+    parser.add_argument(
+        "--rabbitmq-url", type=str, default=rabbitmq_api_base_url, help="RabbitMQ URL"
+    )
 
     return parser
 
 
 def validate_cli_arguments(args: Namespace):
     valid_arguments = True
     if not args.rabbitmq_url:
@@ -44,14 +48,16 @@
     """
     This function creates users in RabbitMQ server along with required permissions.
     """
     parser: ArgumentParser = create_cli_argparser()
     args: Namespace = parser.parse_args()
     args = validate_cli_arguments(args)
     if not args:
-        logger.error("CLI arguments validation failed while bootstrapping rabbitmq users")
+        logger.error(
+            "CLI arguments validation failed while bootstrapping rabbitmq users"
+        )
         sys.exit(-1)
 
     server_up = wait_for_rabbitmq_server_to_up(rabbitmq_api_base_url=args.rabbitmq_url)
     if not server_up:
         raise TimeoutError("Wait for rabbitmq server to up has been failed.")
     create_queue_user_and_set_permission(rabbitmq_api_base_url=args.rabbitmq_url)
```

### Comparing `resc_backend-3.1.2/src/resc_backend/common.py` & `resc_backend-4.0.0/src/resc_backend/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # Third Party
 import pkg_resources
 
 logger = logging.getLogger(__name__)
 
 
 def get_logging_settings_path():
-    if path.isfile(sysconfig.get_path("purelib") + "/resc"):
-        base_dir = sysconfig.get_path("purelib") + "/resc"
+    if path.isfile(sysconfig.get_path('purelib') + "/resc"):
+        base_dir = sysconfig.get_path('purelib') + "/resc"
     else:
         base_dir = path.dirname(__file__)
 
     return base_dir + "/static/logging.ini"
 
 
 def initialise_logs(log_file_path: str, debug=True):
```

### Comparing `resc_backend-3.1.2/src/resc_backend/constants.py` & `resc_backend-4.0.0/src/resc_backend/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,17 @@
 # Logging
 LOG_FILE_PATH_RABBITMQ = "rabbitmq_initialization.log"
 LOG_FILE_CACHING = "redis_cache.log"
 LOGGING_FILE = "logging.ini"
 
 # Error message
 ERROR_MESSAGE_500 = "Internal server error. Contact your system administrator"
-ERROR_MESSAGE_503 = "Unable to communicate with DataBase, Please contact your system administrator"
+ERROR_MESSAGE_503 = (
+    "Unable to communicate with DataBase, Please contact your system administrator"
+)
 
 # Redis Cache
 REDIS_CACHE_EXPIRE = 60 * 60 * 24  # set to 24 hours
 
 # HTTP Security Response Headers
 STRICT_TRANSPORT_SECURITY = "max-age=31536000; includeSubDomains; preload"
 CACHE_CONTROL = "no-cache, no-store"
```

### Comparing `resc_backend-3.1.2/src/resc_backend/db/connection.py` & `resc_backend-4.0.0/src/resc_backend/db/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,23 @@
 
 echo_queries = os.getenv("SQL_ALCHEMY_ECHO_QUERIES", "False").lower() in (
     "true",
     "1",
     "y",
 )
 pool_size = int(os.environ.get("SQL_ALCHEMY_POOL_SIZE", SQL_ALCHEMY_POOL_SIZE_DEFAULT))
-max_overflow = int(os.environ.get("SQL_ALCHEMY_MAX_OVERFLOW", SQL_ALCHEMY_MAX_OVERFLOW_DEFAULT))
+max_overflow = int(
+    os.environ.get("SQL_ALCHEMY_MAX_OVERFLOW", SQL_ALCHEMY_MAX_OVERFLOW_DEFAULT)
+)
 
 if DB_CONNECTION_STRING:
     logger.info("Using provided environment variable to connect to the Database")
-    use_azure_token_auth = os.environ.get("DB_USE_AZURE_TOKEN_AUTH", "False").lower() in ("true", "1", "y")
+    use_azure_token_auth = os.environ.get(
+        "DB_USE_AZURE_TOKEN_AUTH", "False"
+    ).lower() in ("true", "1", "y")
     if use_azure_token_auth:
         engine = create_azure_engine(
             connection_string=DB_CONNECTION_STRING,
             echo_queries=echo_queries,
             pool_size=pool_size,
             max_overflow=max_overflow,
         )
@@ -51,13 +55,17 @@
         engine = create_engine(
             DB_CONNECTION_STRING,
             echo=echo_queries,
             pool_size=pool_size,
             max_overflow=max_overflow,
         )
 else:
-    DATABASE_URL = "sqlite:///" + os.path.join(basedir, "db.sqlite?check_same_thread=False")
-    logger.info(f"Database environment variables were not provided, defaulting to {DATABASE_URL}")
+    DATABASE_URL = "sqlite:///" + os.path.join(
+        basedir, "db.sqlite?check_same_thread=False"
+    )
+    logger.info(
+        f"Database environment variables were not provided, defaulting to {DATABASE_URL}"
+    )
     engine = create_engine(DATABASE_URL, echo=echo_queries)
     Base.metadata.create_all(engine, checkfirst=True)
 
 Session = sessionmaker()
```

### Comparing `resc_backend-3.1.2/src/resc_backend/db/engine_azure.py` & `resc_backend-4.0.0/src/resc_backend/db/engine_azure.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from azure.identity import DefaultAzureCredential
 from sqlalchemy import create_engine, event
 
 basedir = os.path.abspath(os.path.dirname(__file__))
 logger = logging.getLogger(__name__)
 
 
-def create_azure_engine(connection_string: str, echo_queries: bool, pool_size: int, max_overflow: int):
+def create_azure_engine(
+    connection_string: str, echo_queries: bool, pool_size: int, max_overflow: int
+):
     """
         Create a SQLAlchemy Engine with added azure token injection
     :param connection_string:
         the connection string to the database
     :param echo_queries:
         bool, echo queries as defined in SQLAlchemy
     :param pool_size:
@@ -32,22 +34,26 @@
     credential = DefaultAzureCredential(
         managed_identity_client_id=managed_identity_client_id,
         logging_enable=True,
         logging_body=True,
     )
     sql_copt_ss_access_token = 1256
 
-    logger.info("Using provided environment variable to connect to the Database with azure token auth")
+    logger.info(
+        "Using provided environment variable to connect to the Database with azure token auth"
+    )
     engine = create_engine(
         connection_string,
         echo=echo_queries,
         pool_size=pool_size,
         max_overflow=max_overflow,
     )
 
     @event.listens_for(engine, "do_connect")
     def provide_token(dialect, conn_rec, cargs, cparams):
-        token = credential.get_token("https://database.windows.net/.default").token.encode("UTF-16-LE")
+        token = credential.get_token(
+            "https://database.windows.net/.default"
+        ).token.encode("UTF-16-LE")
         token_struct = struct.pack(f"<I{len(token)}s", len(token), token)
         cparams["attrs_before"] = {sql_copt_ss_access_token: token_struct}
 
     return engine
```

### Comparing `resc_backend-3.1.2/src/resc_backend/db/model/__init__.py` & `resc_backend-4.0.0/src/resc_backend/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/db/model/audit.py` & `resc_backend-4.0.0/src/resc_backend/db/model/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/db/model/finding.py` & `resc_backend-4.0.0/src/resc_backend/db/model/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/db/model/repository.py` & `resc_backend-4.0.0/src/resc_backend/db/model/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,17 @@
             "project_key",
             "repository_id",
             "vcs_instance",
             name="unique_repository_id_per_project",
         ),
     )
 
-    def __init__(self, project_key, repository_id, repository_name, repository_url, vcs_instance):
+    def __init__(
+        self, project_key, repository_id, repository_name, repository_url, vcs_instance
+    ):
         self.project_key = project_key
         self.repository_id = repository_id
         self.repository_name = repository_name
         self.repository_url = repository_url
         self.vcs_instance = vcs_instance
 
     @staticmethod
```

### Comparing `resc_backend-3.1.2/src/resc_backend/db/model/rule.py` & `resc_backend-4.0.0/src/resc_backend/db/model/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,19 @@
     rule_name = Column(String(400), nullable=False)
     description = Column(String(2000), nullable=True)
     entropy = Column(Float, nullable=True)
     secret_group = Column(Integer, nullable=True)
     regex = Column(Text, nullable=True)
     path = Column(Text, nullable=True)
     keywords = Column(Text, nullable=True)
-    __table_args__ = (UniqueConstraint("rule_name", "rule_pack", name="unique_rule_name_per_rule_pack_version"),)
+    __table_args__ = (
+        UniqueConstraint(
+            "rule_name", "rule_pack", name="unique_rule_name_per_rule_pack_version"
+        ),
+    )
 
     def __init__(
         self,
         rule_pack: str,
         rule_name: str,
         description: str,
         allow_list: int = None,
```

### Comparing `resc_backend-3.1.2/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-4.0.0/src/resc_backend/db/model/rule_allow_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,17 @@
         self.description = description
         self.regexes = regexes
         self.paths = paths
         self.commits = commits
         self.stop_words = stop_words
 
     @staticmethod
-    def create_from_metadata(description: str, regexes: str, paths: str, commits: str, stop_words: str):
+    def create_from_metadata(
+        description: str, regexes: str, paths: str, commits: str, stop_words: str
+    ):
         db_rule_allow_list = DBruleAllowList(
             description=description,
             regexes=regexes,
             paths=paths,
             commits=commits,
             stop_words=stop_words,
         )
```

### Comparing `resc_backend-3.1.2/src/resc_backend/db/model/rule_pack.py` & `resc_backend-4.0.0/src/resc_backend/db/model/rule_pack.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     ):
         self.version = version
         self.global_allow_list = global_allow_list
         self.active = active
         self.created = created
 
     @staticmethod
-    def create_from_metadata(version: str, global_allow_list: int, active: bool, created: datetime):
+    def create_from_metadata(
+        version: str, global_allow_list: int, active: bool, created: datetime
+    ):
         db_rule_pack = DBrulePack(
             version=version,
             global_allow_list=global_allow_list,
             active=active,
             created=created,
         )
         return db_rule_pack
```

### Comparing `resc_backend-3.1.2/src/resc_backend/db/model/scan.py` & `resc_backend-4.0.0/src/resc_backend/db/model/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,22 @@
 
 
 class DBscan(Base):
     __tablename__ = "scan"
     id_ = Column("id", Integer, primary_key=True)
     repository_id = Column(Integer, ForeignKey(REPOSITORY_ID))
     rule_pack = Column(String(100), ForeignKey(DBrulePack.version), nullable=False)
-    scan_type = Column(Enum(ScanType), default=ScanType.BASE, server_default=BASE_SCAN, nullable=False)
+    scan_type = Column(
+        Enum(ScanType), default=ScanType.BASE, server_default=BASE_SCAN, nullable=False
+    )
     last_scanned_commit = Column(String(100), nullable=False)
     timestamp = Column(DateTime, nullable=False, default=datetime.utcnow)
-    increment_number = Column(Integer, server_default=text("0"), default=0, nullable=False)
+    increment_number = Column(
+        Integer, server_default=text("0"), default=0, nullable=False
+    )
     is_latest = Column(Boolean, nullable=False, default=False, server_default=text("0"))
 
     def __init__(
         self,
         repository_id: int,
         scan_type: ScanType,
         last_scanned_commit: str,
```

### Comparing `resc_backend-3.1.2/src/resc_backend/db/model/vcs_instance.py` & `resc_backend-4.0.0/src/resc_backend/db/model/vcs_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from resc_backend.db.model import Base
 
 
 class DBVcsInstance(Base):
     __tablename__ = "vcs_instance"
     id_ = Column("id", Integer, primary_key=True)
     name = Column(String(200), nullable=False)
-    provider_type = Column(Enum(BITBUCKET, AZURE_DEVOPS, GITHUB_PUBLIC, name="provider_type"))
+    provider_type = Column(
+        Enum(BITBUCKET, AZURE_DEVOPS, GITHUB_PUBLIC, name="provider_type")
+    )
     scheme = Column(String(50), nullable=False)
     hostname = Column(String(200), nullable=False)
     port = Column(Integer, nullable=False)
     organization = Column(String(200), nullable=True)
     scope = Column("vcs_scope", Text, nullable=True)
     exceptions = Column(Text, nullable=True)
     __table_args__ = (
```

### Comparing `resc_backend-3.1.2/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-4.0.0/src/resc_backend/helpers/dict_remapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 from functools import reduce
 from typing import List
 
 
 def remap_dict_keys(input_dict: dict, transformation_map: List):
     new_keys = [val[1] for val in transformation_map]
     for old_key, new_key in transformation_map:
-        create_nested_dictionary(input_dict, new_key, get_value_from_nested_dictionary(input_dict, *old_key))
-
-    output_dict = {k: v for k, v in input_dict.items() if k in [key[0] for key in new_keys]}
+        create_nested_dictionary(
+            input_dict, new_key, get_value_from_nested_dictionary(input_dict, *old_key)
+        )
+
+    output_dict = {
+        k: v for k, v in input_dict.items() if k in [key[0] for key in new_keys]
+    }
 
     return output_dict
 
 
 def create_nested_dictionary(dictionary, keys, value):
     for key in keys[:-1]:
         dictionary = dictionary.setdefault(key, {})
```

### Comparing `resc_backend-3.1.2/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-4.0.0/src/resc_backend/helpers/environment_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,9 +18,11 @@
         value = os.environ.get(env_variable.key_name, env_variable.default)
         if not value and env_variable.required:
             missing.append(f"{env_variable.key_name}: {env_variable.help_text}")
         else:
             values[env_variable.key_name] = value
 
     if missing:
-        raise EnvironmentError(f"The following env variables need to be set: {', '.join(missing)}")
+        raise EnvironmentError(
+            f"The following env variables need to be set: {', '.join(missing)}"
+        )
     return values
```

### Comparing `resc_backend-3.1.2/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-4.0.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,28 @@
     rabbitmq_admin_user = f"{env_variables[RABBITMQ_DEFAULT_USER]}"
     rabbitmq_admin_password = f"{env_variables[RABBITMQ_DEFAULT_PASSWORD]}"
 
     session = requests.Session()
     retries = Retry(total=100, backoff_factor=1, status_forcelist=[500, 502, 503, 504])
     uri = rabbitmq_api_base_url + "/api/health/checks/alarms"
     session.mount("http://", HTTPAdapter(max_retries=retries))
-    response = session.get(uri, auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password))
+    response = session.get(
+        uri, auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password)
+    )
 
     if hasattr(response, "status_code") and int(response.status_code) == 200:
         logger.debug("Rabbitmq server is up.")
         return True
     logger.error(f"Rabbitmq server is down, HTTP status: '{response.status_code}'")
     return False
 
 
-def create_user(rabbitmq_api_base_url: str, username: str, password: str, role: str) -> bool:
+def create_user(
+    rabbitmq_api_base_url: str, username: str, password: str, role: str
+) -> bool:
     """
         Creates a user in RabbitMQ server, it would return true if the operation was a success, false otherwise
     :param rabbitmq_api_base_url:
         RabbitMQ API base url
     :param username:
         Username to be created
     :param password:
@@ -79,15 +83,17 @@
     if hasattr(response, "status_code") and int(response.status_code) == 201:
         logger.info(f"User: {username} with role: {role} created successfully.")
         return True
     if hasattr(response, "status_code") and int(response.status_code) == 204:
         logger.info(f"User: {username} with role: {role} already exists.")
         return True
     logger.error(
-        f"Failed while creating user: '{username}' " f"with role: '{role}' " f", HTTP status: '{response.status_code}'"
+        f"Failed while creating user: '{username}' "
+        f"with role: '{role}' "
+        f", HTTP status: '{response.status_code}'"
     )
     return False
 
 
 def set_resource_permissions(
     rabbitmq_api_base_url: str,
     v_host: str,
@@ -125,15 +131,17 @@
     response = requests.put(
         uri,
         json=permission_data,
         auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password),
         timeout=10,
     )
     if hasattr(response, "status_code") and int(response.status_code) == 201:
-        logger.debug(f"vHost permission successfully assigned to user: {username} for vHost: {v_host}.")
+        logger.debug(
+            f"vHost permission successfully assigned to user: {username} for vHost: {v_host}."
+        )
         return True
     logger.error(
         f"Failed while assigning vhost permission to user: '{username}' "
         f"for vhost: '{v_host}' "
         f", HTTP status: '{response.status_code}'"
     )
     return False
@@ -186,15 +194,17 @@
     response = requests.put(
         uri,
         json=topic_permission_data,
         auth=HTTPBasicAuth(rabbitmq_admin_user, rabbitmq_admin_password),
         timeout=10,
     )
 
-    if hasattr(response, "status_code") and (int(response.status_code) == 201 or int(response.status_code) == 204):
+    if hasattr(response, "status_code") and (
+        int(response.status_code) == 201 or int(response.status_code) == 204
+    ):
         logger.debug(
             f"Topic permission successfully assigned to user: {username} for topic: {topic_name} in vhost: {v_host}."
         )
         return True
     logger.error(
         f"Failed while assigning topic permission to user: '{username}' "
         f"with vhost: '{v_host}' "
@@ -221,17 +231,19 @@
         role="monitoring",
     )
     if user_created:
         set_resource_permissions(
             rabbitmq_api_base_url=rabbitmq_api_base_url,
             v_host=rabbitmq_vhost,
             username=queue_user,
-            configure_resources_regex=f"^({PROJECT_QUEUE}|{REPOSITORY_QUEUE}" f"|.*celery.*)$",
+            configure_resources_regex=f"^({PROJECT_QUEUE}|{REPOSITORY_QUEUE}"
+            f"|.*celery.*)$",
             read_resources_regex=f"^{PROJECT_QUEUE}|{REPOSITORY_QUEUE}" f"|.*celery.*$",
-            write_resources_regex=f"^{PROJECT_QUEUE}|{REPOSITORY_QUEUE}" f"|amq.default|.*celery.*$",
+            write_resources_regex=f"^{PROJECT_QUEUE}|{REPOSITORY_QUEUE}"
+            f"|amq.default|.*celery.*$",
         )
         set_topic_permissions(
             rabbitmq_api_base_url=rabbitmq_api_base_url,
             v_host=rabbitmq_vhost,
             username=queue_user,
             topic_name=f"{PROJECT_QUEUE}",
             allow_read=True,
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/api.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,17 @@
     """
 
     logging_level = "DEBUG" if debug else "INFO"
     logging_config = {
         "version": 1,
         "disable_existing_loggers": False,
         "formatters": {
-            "generic-log-formatter": {"format": "[%(levelname)s] [%(name)s] [%(asctime)s] %(message)s"},
+            "generic-log-formatter": {
+                "format": "[%(levelname)s] [%(name)s] [%(asctime)s] %(message)s"
+            },
         },
         "handlers": {
             "console": {
                 "level": logging_level,
                 "class": "logging.StreamHandler",
                 "formatter": "generic-log-formatter",
             },
@@ -130,15 +132,17 @@
     )
 
 app.include_router(health.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(common.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(rules.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(rule_packs.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(findings.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
-app.include_router(detailed_findings.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
+app.include_router(
+    detailed_findings.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH
+)
 app.include_router(repositories.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(scans.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(vcs_instances.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 app.include_router(metrics.router, prefix=RWS_VERSION_PREFIX, dependencies=AUTH)
 
 # Apply the security headers to the app in the form of middleware
 app.middleware("http")(add_security_headers)
@@ -152,15 +156,17 @@
     CacheManager.initialize_cache(env_variables=env_variables)
     try:
         _ = Session(bind=engine)
         check_db_initialized()
 
         logger.info("Database is connected, expected table(s) found")
     except RetryError as exc:
-        raise SystemExit("Error while connecting to the database, retry timed out") from exc
+        raise SystemExit(
+            "Error while connecting to the database, retry timed out"
+        ) from exc
 
 
 @app.on_event("shutdown")
 async def app_shutdown():
     await CacheManager.clear_all_cache()
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/cache_manager.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/cache_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     def initialize_cache(cls, env_variables):
         cache_enabled = env_variables[RESC_REDIS_CACHE_ENABLE].lower() in ["true"]
         if cache_enabled:
             env_variables.update(validate_environment(CONDITIONAL_REDIS_ENV_VARS))
             redis_host = f"{env_variables[RESC_REDIS_SERVICE_HOST]}"
             redis_port = f"{env_variables[RESC_REDIS_SERVICE_PORT]}"
             redis_password = f"{env_variables[REDIS_PASSWORD]}"
-            redis_backend = cls.get_cache_client(host=redis_host, port=int(redis_port), password=redis_password)
+            redis_backend = cls.get_cache_client(
+                host=redis_host, port=int(redis_port), password=redis_password
+            )
             FastAPICache.init(
                 RedisBackend(redis_backend),
                 prefix=CACHE_PREFIX,
                 key_builder=cls.request_key_builder,
                 enable=cache_enabled,
             )
         else:
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/configuration.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/audit.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/audit.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,17 @@
         audit status to set, type FindingStatus
     :param comment:
         audit comment to set
     :return: DBaudit
         The output will contain the audit that was created
     """
     # UPDATE FINDING to set is_latest to FALSE.
-    db_connection.execute(update(DBaudit).where(DBaudit.finding_id == finding_id).values(is_latest=False))
+    db_connection.execute(
+        update(DBaudit).where(DBaudit.finding_id == finding_id).values(is_latest=False)
+    )
 
     # Insert new Audit.
     db_audit = DBaudit(
         finding_id=finding_id,
         auditor=auditor,
         status=status,
         comment=comment,
@@ -81,15 +83,17 @@
     :param skip:
         integer amount of records to skip to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [DBaudit]
         The output will contain the list of audit items for the given finding
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
     query = select(DBaudit).where(DBaudit.finding_id == finding_id)
     query = query.order_by(DBaudit.id_.desc()).offset(skip).limit(limit_val)
     finding_audits = db_connection.execute(query).scalars().all()
     return finding_audits
 
 
 def get_finding_audits_count(db_connection: Session, finding_id: int) -> int:
@@ -103,15 +107,17 @@
         count of audit entries
     """
     query = select(func.count(DBaudit.id_)).where(DBaudit.finding_id == finding_id)
     total_count = db_connection.execute(query).scalars().one()
     return total_count
 
 
-def get_audit_count_by_auditor_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
+def get_audit_count_by_auditor_over_time(
+    db_connection: Session, weeks: int = 13
+) -> list[Row]:
     """
         Retrieve count audits by auditor over time for given weeks
     :param db_connection:
         Session of the database connection
     :param weeks:
         optional, filter on last n weeks, default 13
     :return: count_over_time
@@ -125,16 +131,22 @@
             extract(WEEK, DBaudit.timestamp).label(WEEK),
             DBaudit.auditor,
             func.count(DBaudit.id_).label("audit_count"),
         )
         .filter(
             (extract(YEAR, DBaudit.timestamp) > extract(YEAR, last_nth_week_date_time))
             | (
-                (extract(YEAR, DBaudit.timestamp) == extract(YEAR, last_nth_week_date_time))
-                & (extract(WEEK, DBaudit.timestamp) >= extract(WEEK, last_nth_week_date_time))
+                (
+                    extract(YEAR, DBaudit.timestamp)
+                    == extract(YEAR, last_nth_week_date_time)
+                )
+                & (
+                    extract(WEEK, DBaudit.timestamp)
+                    >= extract(WEEK, last_nth_week_date_time)
+                )
             )
         )
         .group_by(
             extract(YEAR, DBaudit.timestamp).label(YEAR),
             extract(WEEK, DBaudit.timestamp).label(WEEK),
             DBaudit.auditor,
         )
@@ -145,15 +157,17 @@
         )
     )
     finding_audits = query.all()
 
     return finding_audits
 
 
-def get_personal_audit_count(db_connection: Session, auditor: str, time_period: TimePeriod) -> int:
+def get_personal_audit_count(
+    db_connection: Session, auditor: str, time_period: TimePeriod
+) -> int:
     """
         Get count of Audit entries for finding
     :param db_connection:
         Session of the database connection
     :param auditor:
         id of the auditor
     :param time_period:
@@ -162,23 +176,35 @@
         count of audit entries
     """
     date_today = datetime.utcnow()
 
     total_count = db_connection.query(func.count(DBaudit.id_))
 
     if time_period in (time_period.DAY, time_period.MONTH, time_period.YEAR):
-        total_count = total_count.filter(extract(YEAR, DBaudit.timestamp) == extract(YEAR, date_today))
+        total_count = total_count.filter(
+            extract(YEAR, DBaudit.timestamp) == extract(YEAR, date_today)
+        )
 
         if time_period in (time_period.DAY, time_period.MONTH):
-            total_count = total_count.filter(extract(MONTH, DBaudit.timestamp) == extract(MONTH, date_today))
+            total_count = total_count.filter(
+                extract(MONTH, DBaudit.timestamp) == extract(MONTH, date_today)
+            )
 
             if time_period == time_period.DAY:
-                total_count = total_count.filter(extract(DAY, DBaudit.timestamp) == extract(DAY, date_today))
+                total_count = total_count.filter(
+                    extract(DAY, DBaudit.timestamp) == extract(DAY, date_today)
+                )
 
     if time_period in (time_period.WEEK, time_period.LAST_WEEK):
         date_last_week = datetime.utcnow() - timedelta(weeks=1)
-        date_week = date_last_week if time_period == time_period.LAST_WEEK else date_today
-        total_count = total_count.filter(extract(YEAR, DBaudit.timestamp) == extract(YEAR, date_week))
-        total_count = total_count.filter(extract(WEEK, DBaudit.timestamp) == extract(WEEK, date_week))
+        date_week = (
+            date_last_week if time_period == time_period.LAST_WEEK else date_today
+        )
+        total_count = total_count.filter(
+            extract(YEAR, DBaudit.timestamp) == extract(YEAR, date_week)
+        )
+        total_count = total_count.filter(
+            extract(WEEK, DBaudit.timestamp) == extract(WEEK, date_week)
+        )
 
     total_count = total_count.filter(DBaudit.auditor == auditor).scalar()
     return total_count
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/detailed_finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/detailed_finding.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 from resc_backend.resc_web_service.schema import (
     detailed_finding as detailed_finding_schema,
 )
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 
 
-def _query_join_if_multiple_rule_pack(query: Query, rule_pack_versions: List[str]) -> Query:
+def _query_join_if_multiple_rule_pack(
+    query: Query, rule_pack_versions: List[str]
+) -> Query:
     """
     When we are working with rule pack it is sometimes necessary to use a join
     with a subquery (i.e. when there are 0 or > 1 rule pack selected).
 
     This takes care of the join of the sub query.
 
     Note that the filtering per rulepack is not applied here. We only search for the max
@@ -46,15 +48,17 @@
 
     Returns:
         Query: Updated query
     """
     if rule_pack_versions is not None and len(rule_pack_versions) == 1:
         return query
 
-    subquery: Query = query.session.query(DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id"))
+    subquery: Query = query.session.query(
+        DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id")
+    )
 
     # This contraint is not necessary, but it will make the table smaller.
     subquery = subquery.where(DBscan.is_latest == True)  # noqa: E712
     subquery = subquery.where(DBscan.scan_type == ScanType.BASE)
     if rule_pack_versions is not None and len(rule_pack_versions) > 0:
         subquery = subquery.where(DBscan.rule_pack.in_(rule_pack_versions))
     subquery = subquery.group_by(DBscan.repository_id)
@@ -89,21 +93,24 @@
     subquery = subquery.join(DBtag, DBruleTag.tag_id == DBtag.id_)
     subquery = subquery.where(DBtag.name.in_(rule_tags))
     subquery = subquery.group_by(DBruleTag.rule_id)
     subquery = subquery.subquery()
 
     query = query.join(
         DBrule,
-        (DBrule.rule_name == DBfinding.rule_name) & (DBrule.rule_pack == DBscan.rule_pack),
+        (DBrule.rule_name == DBfinding.rule_name)
+        & (DBrule.rule_pack == DBscan.rule_pack),
     )
     query = query.where(DBrule.id_.in_(subquery))
     return query
 
 
-def _query_apply_findings_filters(query: Query, findings_filter: FindingsFilter) -> Query:
+def _query_apply_findings_filters(
+    query: Query, findings_filter: FindingsFilter
+) -> Query:
     """
     Apply filtering on the query.
     This only applies filtering for:
         - rule_pack_versions
         - scan_ids
         - rule_names
         - start_date_time
@@ -146,26 +153,31 @@
     if findings_filter.event_sent is not None:
         if findings_filter.event_sent:
             query = query.where(DBfinding.event_sent_on != None)  # noqa: E711
         else:
             query = query.where(DBfinding.event_sent_on == None)  # noqa: E711
 
     if findings_filter.repository_name:
-        query = query.where(DBrepository.repository_name == findings_filter.repository_name)
+        query = query.where(
+            DBrepository.repository_name == findings_filter.repository_name
+        )
 
     if findings_filter.vcs_providers and findings_filter.vcs_providers is not None:
-        query = query.where(DBVcsInstance.provider_type.in_(findings_filter.vcs_providers))
+        query = query.where(
+            DBVcsInstance.provider_type.in_(findings_filter.vcs_providers)
+        )
 
     if findings_filter.project_name:
         query = query.where(DBrepository.project_key == findings_filter.project_name)
 
     if findings_filter.finding_statuses:
         if FindingStatus.NOT_ANALYZED.value in findings_filter.finding_statuses:
             query = query.where(
-                (DBaudit.status.in_(findings_filter.finding_statuses)) | (DBaudit.status == None)  # noqa: E711
+                (DBaudit.status.in_(findings_filter.finding_statuses))
+                | (DBaudit.status == None)  # noqa: E711
             )
         else:
             query = query.where(DBaudit.status.in_(findings_filter.finding_statuses))
     return query
 
 
 def get_detailed_findings(
@@ -186,15 +198,17 @@
     :param limit:
         integer amount of records to return, to support pagination
     :return: [DetailedFindingRead]
         The output will contain a list of DetailedFindingRead objects,
         or an empty list if no finding was found for the given findings_filter
     """
 
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
 
     query = db_connection.query(
         DBfinding.id_,
         DBfinding.file_path,
         DBfinding.line_number,
         DBfinding.column_start,
         DBfinding.column_end,
@@ -235,15 +249,17 @@
     query = query.order_by(DBfinding.id_)
     query = query.offset(skip).limit(limit_val)
     findings: List[detailed_finding_schema.DetailedFindingRead] = query.all()
 
     return findings
 
 
-def get_detailed_findings_count(db_connection: Session, findings_filter: FindingsFilter) -> int:
+def get_detailed_findings_count(
+    db_connection: Session, findings_filter: FindingsFilter
+) -> int:
     """
     Retrieve count of detailed findings objects matching the provided FindingsFilter
     :param findings_filter:
         Object of type FindingsFilter, only DetailedFindingRead objects matching the attributes in this filter will be
             fetched
     :param db_connection:
         Session of the database connection
@@ -268,15 +284,17 @@
         isouter=True,
     )
     query = _query_apply_findings_filters(query, findings_filter)
     findings_count = query.scalar()
     return findings_count
 
 
-def get_detailed_finding(db_connection: Session, finding_id: int) -> detailed_finding_schema.DetailedFindingRead:
+def get_detailed_finding(
+    db_connection: Session, finding_id: int
+) -> detailed_finding_schema.DetailedFindingRead:
     """
     Retrieve a detailed finding objects matching the provided finding_id
     :param db_connection:
         Session of the database connection
     :param finding_id:
         ID of the finding object for which a DetailedFinding is to be fetched
     :return: DetailedFindingRead
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,27 +33,31 @@
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 logger = logging.getLogger(__name__)
 
 
-def patch_finding(db_connection: Session, finding_id: int, finding_update: finding_schema.FindingPatch):
+def patch_finding(
+    db_connection: Session, finding_id: int, finding_update: finding_schema.FindingPatch
+):
     db_finding = db_connection.query(DBfinding).filter_by(id_=finding_id).first()
 
     finding_update_dict = finding_update.dict(exclude_unset=True)
     for key in finding_update_dict:
         setattr(db_finding, key, finding_update_dict[key])
 
     db_connection.commit()
     db_connection.refresh(db_finding)
     return db_finding
 
 
-def create_findings(db_connection: Session, findings: List[finding_schema.FindingCreate]) -> List[DBfinding]:
+def create_findings(
+    db_connection: Session, findings: List[finding_schema.FindingCreate]
+) -> List[DBfinding]:
     if len(findings) < 1:
         # Function is called with an empty list of findings
         return []
 
     repository_id = findings[0].repository_id
 
     # get a list of known / registered findings for this repository
@@ -104,16 +108,20 @@
 
 def get_finding(db_connection: Session, finding_id: int):
     finding = db_connection.query(DBfinding)
     finding = finding.where(DBfinding.id_ == finding_id).first()
     return finding
 
 
-def get_findings(db_connection: Session, skip: int = 0, limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT):
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+def get_findings(
+    db_connection: Session, skip: int = 0, limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT
+):
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
     findings = db_connection.query(DBfinding)
     findings = findings.order_by(DBfinding.id_).offset(skip).limit(limit_val).all()
     return findings
 
 
 def get_scans_findings(
     db_connection,
@@ -140,15 +148,17 @@
     :return: [DBfinding]
         The output will contain a list of DBfinding type objects,
         or an empty list if no finding was found for the given scan_ids
     """
     if len(scan_ids) == 0:
         return []
 
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
 
     query: Query = db_connection.query(DBfinding)
     query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
 
     if statuses_filter:
         query = query.join(
             DBaudit,
@@ -170,15 +180,17 @@
 
     query = query.order_by(DBfinding.id_)
     query = query.offset(skip).limit(limit_val)
     findings = query.all()
     return findings
 
 
-def get_total_findings_count(db_connection: Session, findings_filter: FindingsFilter = None) -> int:
+def get_total_findings_count(
+    db_connection: Session, findings_filter: FindingsFilter = None
+) -> int:
     """
         Retrieve count of finding records of a given scan
     :param findings_filter:
     :param db_connection:
         Session of the database connection
     :return: total_count
         count of findings
@@ -191,46 +203,60 @@
             query = query.join(
                 DBaudit,
                 (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
                 isouter=True,
             )
 
         if (
-            (findings_filter.vcs_providers and findings_filter.vcs_providers is not None)
+            (
+                findings_filter.vcs_providers
+                and findings_filter.vcs_providers is not None
+            )
             or findings_filter.project_name
             or findings_filter.repository_name
             or findings_filter.start_date_time
             or findings_filter.end_date_time
         ):
             query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
             query = query.join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
             query = query.join(DBrepository, DBrepository.id_ == DBscan.repository_id)
-            query = query.join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+            query = query.join(
+                DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+            )
 
         if findings_filter.start_date_time:
             query = query.where(DBscan.timestamp >= findings_filter.start_date_time)
         if findings_filter.end_date_time:
             query = query.where(DBscan.timestamp <= findings_filter.end_date_time)
 
         if findings_filter.repository_name:
-            query = query.where(DBrepository.repository_name == findings_filter.repository_name)
+            query = query.where(
+                DBrepository.repository_name == findings_filter.repository_name
+            )
 
         if findings_filter.vcs_providers and findings_filter.vcs_providers is not None:
-            query = query.where(DBVcsInstance.provider_type.in_(findings_filter.vcs_providers))
+            query = query.where(
+                DBVcsInstance.provider_type.in_(findings_filter.vcs_providers)
+            )
         if findings_filter.project_name:
-            query = query.where(DBrepository.project_key == findings_filter.project_name)
+            query = query.where(
+                DBrepository.project_key == findings_filter.project_name
+            )
         if findings_filter.rule_names:
             query = query.where(DBfinding.rule_name.in_(findings_filter.rule_names))
         if findings_filter.finding_statuses:
             if FindingStatus.NOT_ANALYZED.value in findings_filter.finding_statuses:
                 query = query.where(
-                    DBaudit.status.in_(findings_filter.finding_statuses) | (DBaudit.status == None)  # noqa: E711
+                    DBaudit.status.in_(findings_filter.finding_statuses)
+                    | (DBaudit.status == None)  # noqa: E711
                 )
             else:
-                query = query.where(DBaudit.status.in_(findings_filter.finding_statuses))
+                query = query.where(
+                    DBaudit.status.in_(findings_filter.finding_statuses)
+                )
         if findings_filter.scan_ids and len(findings_filter.scan_ids) == 1:
             query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
             query = query.where(DBscanFinding.scan_id == findings_filter.scan_ids[0])
 
         if findings_filter.scan_ids and len(findings_filter.scan_ids) >= 2:
             query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
             query = query.where(DBscanFinding.scan_id.in_(findings_filter.scan_ids))
@@ -241,15 +267,17 @@
 
 def get_findings_by_rule(
     db_connection: Session,
     skip: int = 0,
     limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
     rule_name: str = "",
 ):
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
     findings = db_connection.query(DBfinding)
     findings = findings.where(DBfinding.rule_name == rule_name)
     findings = findings.order_by(DBfinding.id_).offset(skip).limit(limit_val).all()
     return findings
 
 
 def get_distinct_rules_from_findings(
@@ -285,20 +313,27 @@
         optional, filter on rule pack version
     :return: rules
         List of unique rules
     """
     query = db_connection.query(DBfinding.rule_name)
 
     if (
-        vcs_providers or project_name or repository_name or start_date_time or end_date_time or rule_pack_versions
+        vcs_providers
+        or project_name
+        or repository_name
+        or start_date_time
+        or end_date_time
+        or rule_pack_versions
     ) and scan_id < 0:
         query = query.join(DBscanFinding, DBscanFinding.finding_id == DBfinding.id_)
         query = query.join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
         query = query.join(DBrepository, DBrepository.id_ == DBscan.repository_id)
-        query = query.join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
 
     if finding_statuses:
         query = query.join(
             DBaudit,
             (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
             isouter=True,
         )
@@ -352,15 +387,17 @@
     :param finding_statuses:
         finding statuses to filter, type FindingStatus
     :param rule_name:
         rule_name to filter on
     :return: findings_count
         count of findings
     """
-    query = db_connection.query(func.count(DBfinding.id_).label("status_count"), DBaudit.status)
+    query = db_connection.query(
+        func.count(DBfinding.id_).label("status_count"), DBaudit.status
+    )
     query = query.join(
         DBaudit,
         (DBaudit.finding_id == DBfinding.id_) & (DBaudit.is_latest == True),  # noqa: E712
         isouter=True,
     )
 
     if scan_ids and len(scan_ids) > 0:
@@ -395,44 +432,59 @@
     :param rule_pack_versions:
         optional, filter on rule pack version
     :param rule_tags:
         optional, filter on rule tag
     :return: findings_count
         per rulename and status the count of findings
     """
-    query = db_connection.query(DBfinding.rule_name, DBaudit.status, func.count(DBfinding.id_))
+    query = db_connection.query(
+        DBfinding.rule_name, DBaudit.status, func.count(DBfinding.id_)
+    )
 
     max_base_scan_subquery = db_connection.query(
         DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id")
     )
-    max_base_scan_subquery = max_base_scan_subquery.where(DBscan.scan_type == ScanType.BASE)
+    max_base_scan_subquery = max_base_scan_subquery.where(
+        DBscan.scan_type == ScanType.BASE
+    )
     if rule_pack_versions:
-        max_base_scan_subquery = max_base_scan_subquery.where(DBscan.rule_pack.in_(rule_pack_versions))
-    max_base_scan_subquery: Query = max_base_scan_subquery.group_by(DBscan.repository_id).subquery()
+        max_base_scan_subquery = max_base_scan_subquery.where(
+            DBscan.rule_pack.in_(rule_pack_versions)
+        )
+    max_base_scan_subquery: Query = max_base_scan_subquery.group_by(
+        DBscan.repository_id
+    ).subquery()
 
     query = query.join(DBscanFinding, DBfinding.id_ == DBscanFinding.finding_id)
     query = query.join(
         max_base_scan_subquery,
         DBfinding.repository_id == max_base_scan_subquery.c.repository_id,
     )
     query = query.join(DBscan, (DBscanFinding.scan_id == DBscan.id_))
     query = query.where(DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id)
 
     if rule_tags:
-        rule_tag_subquery: Query = db_connection.query(DBruleTag.rule_id).join(DBtag, DBruleTag.tag_id == DBtag.id_)
+        rule_tag_subquery: Query = db_connection.query(DBruleTag.rule_id).join(
+            DBtag, DBruleTag.tag_id == DBtag.id_
+        )
         if rule_pack_versions:
-            rule_tag_subquery = rule_tag_subquery.join(DBrule, DBrule.id_ == DBruleTag.rule_id)
-            rule_tag_subquery = rule_tag_subquery.where(DBrule.rule_pack.in_(rule_pack_versions))
+            rule_tag_subquery = rule_tag_subquery.join(
+                DBrule, DBrule.id_ == DBruleTag.rule_id
+            )
+            rule_tag_subquery = rule_tag_subquery.where(
+                DBrule.rule_pack.in_(rule_pack_versions)
+            )
 
         rule_tag_subquery = rule_tag_subquery.where(DBtag.name.in_(rule_tags))
         rule_tag_subquery = rule_tag_subquery.group_by(DBruleTag.rule_id).subquery()
 
         query = query.join(
             DBrule,
-            (DBrule.rule_name == DBfinding.rule_name) & (DBrule.rule_pack == DBscan.rule_pack),
+            (DBrule.rule_name == DBfinding.rule_name)
+            | (DBrule.rule_pack == DBscan.rule_pack),
         )
         query = query.join(rule_tag_subquery, DBrule.id_ == rule_tag_subquery.c.rule_id)
 
     if rule_pack_versions:
         query = query.where(DBscan.rule_pack.in_(rule_pack_versions))
 
     query = query.join(
@@ -462,15 +514,17 @@
         elif status_count[1] == FindingStatus.FALSE_POSITIVE.value:
             rule_count_dict[status_count[0]]["false_positive"] += status_count[2]
         elif status_count[1] == FindingStatus.TRUE_POSITIVE.value:
             rule_count_dict[status_count[0]]["true_positive"] += status_count[2]
         elif status_count[1] == FindingStatus.UNDER_REVIEW.value:
             rule_count_dict[status_count[0]]["under_review"] += status_count[2]
         elif status_count[1] == FindingStatus.CLARIFICATION_REQUIRED.value:
-            rule_count_dict[status_count[0]]["clarification_required"] += status_count[2]
+            rule_count_dict[status_count[0]]["clarification_required"] += status_count[
+                2
+            ]
 
     return rule_count_dict
 
 
 def get_findings_count_by_time(
     db_connection: Session,
     date_type: DateFilter,
@@ -518,19 +572,27 @@
 
     if start_date_time:
         query = query.where(DBscan.timestamp >= start_date_time)
     if end_date_time:
         query = query.where(DBscan.timestamp <= end_date_time)
 
     if date_type == DateFilter.MONTH:
-        query = query.group_by(extract("year", DBscan.timestamp), extract("month", DBscan.timestamp))
-        query = query.order_by(extract("year", DBscan.timestamp), extract("month", DBscan.timestamp))
+        query = query.group_by(
+            extract("year", DBscan.timestamp), extract("month", DBscan.timestamp)
+        )
+        query = query.order_by(
+            extract("year", DBscan.timestamp), extract("month", DBscan.timestamp)
+        )
     elif date_type == DateFilter.WEEK:
-        query = query.group_by(extract("year", DBscan.timestamp), extract("week", DBscan.timestamp))
-        query = query.order_by(extract("year", DBscan.timestamp), extract("week", DBscan.timestamp))
+        query = query.group_by(
+            extract("year", DBscan.timestamp), extract("week", DBscan.timestamp)
+        )
+        query = query.order_by(
+            extract("year", DBscan.timestamp), extract("week", DBscan.timestamp)
+        )
     elif date_type == DateFilter.DAY:
         query = query.group_by(
             extract("year", DBscan.timestamp),
             extract("month", DBscan.timestamp),
             extract("day", DBscan.timestamp),
         )
         query = query.order_by(
@@ -557,38 +619,44 @@
         required, filter on time_type
     :param start_date_time:
         optional, filter on start date
     :param end_date_time:
         optional, filter on end date
     """
     if date_type == DateFilter.MONTH:
-        query: Query = db_connection.query(extract("year", DBscan.timestamp), extract("month", DBscan.timestamp))
+        query: Query = db_connection.query(
+            extract("year", DBscan.timestamp), extract("month", DBscan.timestamp)
+        )
     elif date_type == DateFilter.WEEK:
-        query: Query = db_connection.query(extract("year", DBscan.timestamp), extract("week", DBscan.timestamp))
+        query: Query = db_connection.query(
+            extract("year", DBscan.timestamp), extract("week", DBscan.timestamp)
+        )
     elif date_type == DateFilter.DAY:
         query: Query = db_connection.query(
             extract("year", DBscan.timestamp),
             extract("month", DBscan.timestamp),
             extract("day", DBscan.timestamp),
         )
-
-    query = query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
+    # To check later if it fixes the bug.
+    # query = query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
 
     if start_date_time:
         query = query.where(DBscan.timestamp >= start_date_time)
     if end_date_time:
         query = query.where(DBscan.timestamp <= end_date_time)
 
     query = query.distinct()
 
     result = query.count()
     return result
 
 
-def get_distinct_rules_from_scans(db_connection: Session, scan_ids: List[int] = None) -> List[DBrule]:
+def get_distinct_rules_from_scans(
+    db_connection: Session, scan_ids: List[int] = None
+) -> List[DBrule]:
     """
         Retrieve distinct rules detected
     :param db_connection:
         Session of the database connection
     :param scan_ids:
         List of scan ids
     :return: rules
@@ -602,40 +670,46 @@
 
     query = query.distinct()
     query = query.order_by(DBfinding.rule_name)
     rules = query.all()
     return rules
 
 
-def delete_finding(db_connection: Session, finding_id: int, delete_related: bool = False):
+def delete_finding(
+    db_connection: Session, finding_id: int, delete_related: bool = False
+):
     """
         Delete a finding object
     :param db_connection:
         Session of the database connection
     :param finding_id:
         id of the finding to be deleted
     :param delete_related:
         if related records need to be deleted
     """
     if delete_related:
         scan_finding_crud.delete_scan_finding(db_connection, finding_id=finding_id)
 
-    db_connection.query(DBfinding).where(DBfinding.id_ == finding_id).delete(synchronize_session=False)
+    db_connection.query(DBfinding).where(DBfinding.id_ == finding_id).delete(
+        synchronize_session=False
+    )
     db_connection.commit()
 
 
 def delete_findings_by_repository_id(db_connection: Session, repository_id: int):
     """
         Delete findings for a given repository
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository
     """
-    db_connection.query(DBfinding).where(DBfinding.repository_id == repository_id).delete(synchronize_session=False)
+    db_connection.query(DBfinding).where(
+        DBfinding.repository_id == repository_id
+    ).delete(synchronize_session=False)
     db_connection.commit()
 
 
 def delete_findings_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
     """
         Delete findings for a given vcs instance
     :param db_connection:
@@ -664,94 +738,114 @@
     """
     current_utc_time = datetime.utcnow()
     current_iso = current_utc_time.isocalendar()
     current_iso_year = current_iso[0]
     current_iso_week = current_iso[1]
     # We use 6 (Saturday) to include the current week when 0
     # rather than doing a shift from current day.
-    last_nth_week_date_time = datetime.fromisocalendar(current_iso_year, current_iso_week, 6) - timedelta(weeks=week)
+    last_nth_week_date_time = datetime.fromisocalendar(
+        current_iso_year, current_iso_week, 6
+    ) - timedelta(weeks=week)
     return last_nth_week_date_time
 
 
-def _max_base_scan_subequery(db_connection: Session, last_nth_week_date_time: datetime) -> Query:
+def _max_base_scan_subequery(
+    db_connection: Session, last_nth_week_date_time: datetime
+) -> Query:
     """
         Creates a subquery given a cut-off date to have the max base scan
         per repository
 
     Args:
         db_connection (Session): Session to generate the subquery
         last_nth_week_date_time (datetime): max cut-off date
 
     Returns:
         Query: subquery to have the max base scan under a cut-off date
     """
-    subquery: Query = db_connection.query(func.max(DBscan.id_).label("scan_id"), DBscan.repository_id)
+    subquery: Query = db_connection.query(
+        func.max(DBscan.id_).label("scan_id"), DBscan.repository_id
+    )
     subquery = subquery.where(DBscan.timestamp <= last_nth_week_date_time)
     subquery = subquery.where(DBscan.scan_type == ScanType.BASE)
     subquery = subquery.group_by(DBscan.repository_id)
     return subquery.subquery()
 
 
-def _max_audit_subequery(db_connection: Session, last_nth_week_date_time: datetime) -> Query:
+def _max_audit_subequery(
+    db_connection: Session, last_nth_week_date_time: datetime
+) -> Query:
     """
         Creates a subquery given a cut-off date to have the last audit
         per finding
 
     Args:
         db_connection (Session): Session to generate the subquery
         last_nth_week_date_time (datetime): max cut-off date
 
     Returns:
         Query: subquery to have the last audit under a cut-off date
     """
-    subquery: Query = db_connection.query(func.max(DBaudit.id_).label("audit_id"), DBaudit.finding_id)
+    subquery: Query = db_connection.query(
+        func.max(DBaudit.id_).label("audit_id"), DBaudit.finding_id
+    )
     subquery = subquery.where(DBaudit.timestamp < last_nth_week_date_time)
     subquery = subquery.group_by(DBaudit.finding_id)
     return subquery.subquery()
 
 
-def get_finding_audit_status_count_over_time(db_connection: Session, status: FindingStatus, weeks: int = 13) -> dict:
+def get_finding_audit_status_count_over_time(
+    db_connection: Session, status: FindingStatus, weeks: int = 13
+) -> dict:
     """
         Retrieve count of true positive findings over time for given weeks
     :param db_connection:
         Session of the database connection
     :param status:
         mandatory, status for which to get the audit counts over time
     :param weeks:
         optional, filter on last n weeks, default 13
     :return: true_positive_count_over_time
         list of rows containing finding statuses count over time per week
     """
     all_tables = []
     for week in range(0, weeks):
         last_nth_week_date_time = _get_iso_date_now_diff_week(week)
-        max_audit_subquery = _max_audit_subequery(db_connection, last_nth_week_date_time)
+        max_audit_subquery = _max_audit_subequery(
+            db_connection, last_nth_week_date_time
+        )
 
         query = db_connection.query(
             literal_column(str(last_nth_week_date_time.isocalendar()[0])).label("year"),
             literal_column(str(last_nth_week_date_time.isocalendar()[1])).label("week"),
             DBVcsInstance.provider_type.label("provider_type"),
             func.count(DBaudit.id_).label("finding_count"),
         )
-        query = query.join(max_audit_subquery, max_audit_subquery.c.audit_id == DBaudit.id_)
+        query = query.join(
+            max_audit_subquery, max_audit_subquery.c.audit_id == DBaudit.id_
+        )
         query = query.join(DBfinding, DBfinding.id_ == DBaudit.finding_id)
         query = query.join(DBrepository, DBrepository.id_ == DBfinding.repository_id)
-        query = query.join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
         query = query.where(DBaudit.status == status)
         query = query.group_by(DBVcsInstance.provider_type)
 
         all_tables.append(query)
 
     # union
     unioned_query = union(*all_tables)
     status_count_over_time = db_connection.execute(unioned_query).all()
     return status_count_over_time
 
 
-def get_finding_count_by_vcs_provider_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
+def get_finding_count_by_vcs_provider_over_time(
+    db_connection: Session, weeks: int = 13
+) -> list[Row]:
     """
         Retrieve count findings over time for given weeks
     :param db_connection:
         Session of the database connection
     :param weeks:
         optional, filter on last n weeks, default 13
     :return: count_over_time
@@ -767,66 +861,79 @@
             literal_column(str(last_nth_week_date_time.isocalendar()[0])).label("year"),
             literal_column(str(last_nth_week_date_time.isocalendar()[1])).label("week"),
             DBVcsInstance.provider_type.label("provider_type"),
             func.count(DBfinding.id_).label("finding_count"),
         )
         query = query.join(DBscanFinding, DBfinding.id_ == DBscanFinding.finding_id)
         query = query.join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
-        query = query.join(max_base_scan, max_base_scan.c.repository_id == DBscan.repository_id)
+        query = query.join(
+            max_base_scan, max_base_scan.c.repository_id == DBscan.repository_id
+        )
         query = query.where(DBscan.id_ >= max_base_scan.c.scan_id)
         query = query.where(DBscan.timestamp <= last_nth_week_date_time)
         query = query.join(DBrepository, DBrepository.id_ == DBscan.repository_id)
-        query = query.join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
         query = query.group_by(DBVcsInstance.provider_type)
 
         all_tables.append(query)
 
     # union
     unioned_query = union(*all_tables)
     count_over_time = db_connection.execute(unioned_query).all()
     return count_over_time
 
 
-def get_un_triaged_finding_count_by_vcs_provider_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
+def get_un_triaged_finding_count_by_vcs_provider_over_time(
+    db_connection: Session, weeks: int = 13
+) -> list[Row]:
     """
         Retrieve count of un triaged findings over time for given weeks
     :param db_connection:
         Session of the database connection
     :param weeks:
         optional, filter on last n weeks, default 13
     :return: count_over_time
         list of rows containing un triaged findings count over time per week
     """
     all_tables = []
     for week in range(0, weeks):
         last_nth_week_date_time = _get_iso_date_now_diff_week(week)
         max_base_scan = _max_base_scan_subequery(db_connection, last_nth_week_date_time)
-        max_audit_subquery = _max_audit_subequery(db_connection, last_nth_week_date_time)
+        max_audit_subquery = _max_audit_subequery(
+            db_connection, last_nth_week_date_time
+        )
 
         query = db_connection.query(
             literal_column(str(last_nth_week_date_time.isocalendar()[0])).label("year"),
             literal_column(str(last_nth_week_date_time.isocalendar()[1])).label("week"),
             DBVcsInstance.provider_type.label("provider_type"),
             func.count(DBfinding.id_).label("finding_count"),
         )
         query = query.join(DBscanFinding, DBfinding.id_ == DBscanFinding.finding_id)
         query = query.join(DBscan, DBscan.id_ == DBscanFinding.scan_id)
         query = query.join(DBrepository, DBrepository.id_ == DBscan.repository_id)
-        query = query.join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
-        query = query.join(max_base_scan, max_base_scan.c.repository_id == DBscan.repository_id)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
+        query = query.join(
+            max_base_scan, max_base_scan.c.repository_id == DBscan.repository_id
+        )
         query = query.where(DBscan.id_ >= max_base_scan.c.scan_id)
         query = query.where(DBscan.timestamp <= last_nth_week_date_time)
         query = query.join(
             max_audit_subquery,
             max_audit_subquery.c.finding_id == DBfinding.id_,
             isouter=True,
         )
         query = query.join(
             DBaudit,
-            (DBaudit.finding_id == DBfinding.id_) & (DBaudit.id_ == max_audit_subquery.c.audit_id),
+            (DBaudit.finding_id == DBfinding.id_)
+            & (DBaudit.id_ == max_audit_subquery.c.audit_id),
             isouter=True,
         )
         query = query.where(
             (DBaudit.id_ == None) | (DBaudit.status == FindingStatus.NOT_ANALYZED.value)  # noqa: E711
         )
         query = query.group_by(DBVcsInstance.provider_type)
         all_tables.append(query)
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/repository.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 from resc_backend.resc_web_service.schema import repository as repository_schema
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 
 def _get_max_base_scan(db_connection: Session) -> Query:
-    subquery: Query = db_connection.query(DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id"))
+    subquery: Query = db_connection.query(
+        DBscan.repository_id, func.max(DBscan.id_).label("latest_base_scan_id")
+    )
     subquery = subquery.where(DBscan.scan_type == ScanType.BASE)
     subquery = subquery.where(DBscan.is_latest == True)  # noqa: E712
     subquery = subquery.group_by(DBscan.repository_id)
     return subquery.subquery()
 
 
 def get_repositories(
@@ -59,18 +61,22 @@
     :param repository_filter:
         optional, filter on repository name. Is used as a string contains filter
     :param only_if_has_findings:
         optional, filter on repositories with findings
     :return: repositories
         list of DBrepository objects
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
 
     # Get the latest scan for repository
-    sub_query: Query = db_connection.query(DBscan.repository_id, func.max(DBscan.timestamp).label("max_timestamp"))
+    sub_query: Query = db_connection.query(
+        DBscan.repository_id, func.max(DBscan.timestamp).label("max_timestamp")
+    )
     sub_query = sub_query.where(DBscan.is_latest == True)  # noqa: E712
     sub_query = sub_query.group_by(DBscan.repository_id)
     sub_query = sub_query.subquery()
 
     query = db_connection.query(
         DBrepository.id_,
         DBrepository.project_key,
@@ -86,15 +92,16 @@
     query = query.join(
         sub_query,
         DBrepository.id_ == sub_query.c.repository_id,
         isouter=True,
     )
     query = query.join(
         DBscan,
-        (DBscan.repository_id == sub_query.c.repository_id) & (DBscan.timestamp == sub_query.c.max_timestamp),
+        (DBscan.repository_id == sub_query.c.repository_id)
+        & (DBscan.timestamp == sub_query.c.max_timestamp),
         isouter=True,
     )
 
     if only_if_has_findings:
         last_scan_sub_query = _get_max_base_scan(db_connection)
 
         sub_query = db_connection.query(DBrepository.id_)
@@ -102,15 +109,17 @@
             last_scan_sub_query,
             DBrepository.id_ == last_scan_sub_query.c.repository_id,
         )
         sub_query = sub_query.join(
             DBscan,
             DBrepository.id_ == DBscan.repository_id,
         )
-        sub_query = sub_query.where(DBscan.id_ >= last_scan_sub_query.c.latest_base_scan_id)
+        sub_query = sub_query.where(
+            DBscan.id_ >= last_scan_sub_query.c.latest_base_scan_id
+        )
         sub_query = sub_query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
         sub_query = sub_query.distinct()
 
         # Filter on repositories that are in the selection
         query = query.where(DBrepository.id_.in_(sub_query))
 
     if vcs_providers and vcs_providers is not None:
@@ -159,71 +168,85 @@
             last_scan_sub_query,
             DBrepository.id_ == last_scan_sub_query.c.repository_id,
         )
         sub_query = sub_query.join(
             DBscan,
             DBrepository.id_ == DBscan.repository_id,
         )
-        sub_query = sub_query.where(DBscan.id_ >= last_scan_sub_query.c.latest_base_scan_id)
+        sub_query = sub_query.where(
+            DBscan.id_ >= last_scan_sub_query.c.latest_base_scan_id
+        )
         sub_query = sub_query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
         sub_query = sub_query.distinct()
 
         # Filter on repositories that are in the selection
         query = query.where(DBrepository.id_.in_(sub_query))
 
     if vcs_providers and vcs_providers is not None:
-        query = query.join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
         query = query.where(DBVcsInstance.provider_type.in_(vcs_providers))
 
     if project_filter:
         query = query.where(DBrepository.project_key == project_filter)
 
     if repository_filter:
         query = query.where(DBrepository.repository_name == repository_filter)
 
     total_count = query.scalar()
     return total_count
 
 
 def get_repository(db_connection: Session, repository_id: int):
-    repository = db_connection.query(DBrepository).where(DBrepository.id_ == repository_id).first()
+    repository = (
+        db_connection.query(DBrepository)
+        .where(DBrepository.id_ == repository_id)
+        .first()
+    )
     return repository
 
 
 def update_repository(
     db_connection: Session,
     repository_id: int,
     repository: repository_schema.RepositoryCreate,
 ):
-    db_repository = db_connection.query(DBrepository).filter_by(id_=repository_id).first()
+    db_repository = (
+        db_connection.query(DBrepository).filter_by(id_=repository_id).first()
+    )
 
     db_repository.repository_name = repository.repository_name
     db_repository.repository_url = repository.repository_url
     db_repository.vcs_instance = repository.vcs_instance
 
     db_connection.commit()
     db_connection.refresh(db_repository)
     return db_repository
 
 
-def create_repository(db_connection: Session, repository: repository_schema.RepositoryCreate):
+def create_repository(
+    db_connection: Session, repository: repository_schema.RepositoryCreate
+):
     db_repository = DBrepository(
         project_key=repository.project_key,
         repository_id=repository.repository_id,
         repository_name=repository.repository_name,
         repository_url=repository.repository_url,
         vcs_instance=repository.vcs_instance,
     )
     db_connection.add(db_repository)
     db_connection.commit()
     db_connection.refresh(db_repository)
     return db_repository
 
 
-def create_repository_if_not_exists(db_connection: Session, repository: repository_schema.RepositoryCreate):
+def create_repository_if_not_exists(
+    db_connection: Session, repository: repository_schema.RepositoryCreate
+):
     # Query the database to see if the repository object exists based on the unique constraint parameters
     query: Query = db_connection.query(DBrepository)
     query = query.where(DBrepository.project_key == repository.project_key)
     query = query.where(DBrepository.repository_id == repository.repository_id)
     query = query.where(DBrepository.vcs_instance == repository.vcs_instance)
     db_select_repository = query.first()
 
@@ -265,15 +288,17 @@
             DBscan,
             DBrepository.id_ == DBscan.repository_id,
         )
         query = query.where(DBscan.id_ >= last_scan_sub_query.c.latest_base_scan_id)
         query = query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
 
     if vcs_providers and vcs_providers is not None:
-        query = query.join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
         query = query.where(DBVcsInstance.provider_type.in_(vcs_providers))
 
     if repository_filter:
         query = query.where(DBrepository.repository_name == repository_filter)
 
     query = query.distinct()
     distinct_projects = query.all()
@@ -311,36 +336,42 @@
             DBscan,
             DBrepository.id_ == DBscan.repository_id,
         )
         query = query.where(DBscan.id_ >= last_scan_sub_query.c.latest_base_scan_id)
         query = query.join(DBscanFinding, DBscan.id_ == DBscanFinding.scan_id)
 
     if vcs_providers and vcs_providers is not None:
-        query = query.join(DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance)
+        query = query.join(
+            DBVcsInstance, DBVcsInstance.id_ == DBrepository.vcs_instance
+        )
         query = query.where(DBVcsInstance.provider_type.in_(vcs_providers))
 
     if project_name:
         query = query.where(DBrepository.project_key == project_name)
 
     query = query.distinct()
     distinct_repositories = query.all()
     return distinct_repositories
 
 
-def get_findings_metadata_by_repository_id(db_connection: Session, repository_ids: list[int]):
+def get_findings_metadata_by_repository_id(
+    db_connection: Session, repository_ids: list[int]
+):
     """
         Retrieves the finding metadata for a repository id from the database with most recent scan information
     :param db_connection:
         Session of the database connection
     :param repository_ids:
         ids of the repository for which findings metadata to be retrieved
     :return: findings_metadata
         findings_metadata containing the count for each status
     """
-    query = db_connection.query(DBrepository.id_, DBaudit.status, func.count(DBscanFinding.finding_id))
+    query = db_connection.query(
+        DBrepository.id_, DBaudit.status, func.count(DBscanFinding.finding_id)
+    )
 
     last_scan_sub_query = _get_max_base_scan(db_connection)
     query = query.join(
         last_scan_sub_query,
         DBrepository.id_ == last_scan_sub_query.c.repository_id,
     )
     query = query.join(
@@ -377,38 +408,52 @@
         elif status_count[1] == FindingStatus.FALSE_POSITIVE.value:
             repo_count_dict[status_count[0]]["false_positive"] += status_count[2]
         elif status_count[1] == FindingStatus.TRUE_POSITIVE.value:
             repo_count_dict[status_count[0]]["true_positive"] += status_count[2]
         elif status_count[1] == FindingStatus.UNDER_REVIEW.value:
             repo_count_dict[status_count[0]]["under_review"] += status_count[2]
         elif status_count[1] == FindingStatus.CLARIFICATION_REQUIRED.value:
-            repo_count_dict[status_count[0]]["clarification_required"] += status_count[2]
+            repo_count_dict[status_count[0]]["clarification_required"] += status_count[
+                2
+            ]
 
     return repo_count_dict
 
 
-def delete_repository(db_connection: Session, repository_id: int, delete_related: bool = False):
+def delete_repository(
+    db_connection: Session, repository_id: int, delete_related: bool = False
+):
     """
         Delete a repository object
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository to be deleted
     :param delete_related:
         if related records need to be deleted
     """
     if delete_related:
-        scan_finding_crud.delete_scan_finding_by_repository_id(db_connection, repository_id=repository_id)
-        finding_crud.delete_findings_by_repository_id(db_connection, repository_id=repository_id)
-        scan_crud.delete_scans_by_repository_id(db_connection, repository_id=repository_id)
-    db_connection.query(DBrepository).where(DBrepository.id_ == repository_id).delete(synchronize_session=False)
+        scan_finding_crud.delete_scan_finding_by_repository_id(
+            db_connection, repository_id=repository_id
+        )
+        finding_crud.delete_findings_by_repository_id(
+            db_connection, repository_id=repository_id
+        )
+        scan_crud.delete_scans_by_repository_id(
+            db_connection, repository_id=repository_id
+        )
+    db_connection.query(DBrepository).where(DBrepository.id_ == repository_id).delete(
+        synchronize_session=False
+    )
     db_connection.commit()
 
 
-def delete_repositories_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
+def delete_repositories_by_vcs_instance_id(
+    db_connection: Session, vcs_instance_id: int
+):
     """
         Delete repositories for a given vcs instance
     :param db_connection:
         Session of the database connection
     :param vcs_instance_id:
         id of the vcs instance
     """
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     rule_query = db_connection.query(DBrule)
     rule_query = rule_query.join(DBscan, DBscan.rule_pack == DBrule.rule_pack)
     rule_query = rule_query.where(DBscan.id_ == scan_id)
     rules: List[RuleRead] = rule_query.all()
     return rules
 
 
-def create_rule_allow_list(db_connection: Session, rule_allow_list: rule_allow_list_schema.RuleAllowList):
+def create_rule_allow_list(
+    db_connection: Session, rule_allow_list: rule_allow_list_schema.RuleAllowList
+):
     """
         Create rule allow list in database
     :param db_connection:
         Session of the database connection
     :param rule_allow_list:
         RuleAllowList object to be created
     """
@@ -75,15 +77,17 @@
     )
     db_connection.add(db_rule)
     db_connection.commit()
     db_connection.refresh(db_rule)
     return db_rule
 
 
-def get_rules_by_rule_pack_version(db_connection: Session, rule_pack_version: str) -> List[str]:
+def get_rules_by_rule_pack_version(
+    db_connection: Session, rule_pack_version: str
+) -> List[str]:
     """
         Fetch rules by rule pack version
     :param db_connection:
         Session of the database connection
     :param rule_pack_version:
         rule pack version
     :return: List[str]
@@ -102,23 +106,27 @@
         DBruleAllowList.regexes,
         DBruleAllowList.paths,
         DBruleAllowList.commits,
         DBruleAllowList.stop_words,
     )
 
     query = query.join(DBrulePack, DBrulePack.version == DBrule.rule_pack)
-    query = query.join(DBruleAllowList, DBruleAllowList.id_ == DBrule.allow_list, isouter=True)
+    query = query.join(
+        DBruleAllowList, DBruleAllowList.id_ == DBrule.allow_list, isouter=True
+    )
     query = query.where(DBrule.rule_pack == rule_pack_version)
     query = query.order_by(DBrule.id_)
     db_rules = query.all()
 
     return db_rules
 
 
-def get_global_allow_list_by_rule_pack_version(db_connection: Session, rule_pack_version: str) -> List[str]:
+def get_global_allow_list_by_rule_pack_version(
+    db_connection: Session, rule_pack_version: str
+) -> List[str]:
     """
         Retrieve global allow list by rule pack version
     :param db_connection:
         Session of the database connection
     :param rule_pack_version:
         rule pack version
     :return: List[str]
@@ -128,13 +136,15 @@
         DBrulePack.version,
         DBruleAllowList.description,
         DBruleAllowList.regexes,
         DBruleAllowList.paths,
         DBruleAllowList.commits,
         DBruleAllowList.stop_words,
     )
-    query = query.join(DBruleAllowList, DBruleAllowList.id_ == DBrulePack.global_allow_list)
+    query = query.join(
+        DBruleAllowList, DBruleAllowList.id_ == DBrulePack.global_allow_list
+    )
     query = query.where(DBrulePack.version == rule_pack_version)
     query = query.order_by(DBruleAllowList.id_)
     db_global_allow_list = query.first()
 
     return db_global_allow_list
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 )
 from resc_backend.db.model import DBrule, DBrulePack, DBruleTag, DBtag
 from resc_backend.resc_web_service.schema import rule_pack as rule_pack_schema
 
 logger = logging.getLogger(__name__)
 
 
-def get_rule_pack(db_connection: Session, version: Optional[str]) -> rule_pack_schema.RulePackRead:
+def get_rule_pack(
+    db_connection: Session, version: Optional[str]
+) -> rule_pack_schema.RulePackRead:
     """
         Get active rule pack from database
     :param db_connection:
         Session of the database connection
     :param version:
         optional, version of the rule pack to be fetched else latest rule pack version will be fetched
     :return: RulePackRead
@@ -36,15 +38,17 @@
     else:
         logger.debug("rule pack version not specified, fetching currently active one")
         query = query.where(DBrulePack.active == true())
     rule_pack = query.first()
     return rule_pack
 
 
-def create_rule_pack_version(db_connection: Session, rule_pack: rule_pack_schema.RulePackCreate):
+def create_rule_pack_version(
+    db_connection: Session, rule_pack: rule_pack_schema.RulePackCreate
+):
     """
         Create rule pack version in database
     :param db_connection:
         Session of the database connection
     :param rule_pack:
         RulePackCreate object to be created
     """
@@ -96,22 +100,26 @@
         integer amount of records to skip, to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [RulePackRead]
         The output will contain a PaginationModel containing the list of RulePackRead type objects,
         or an empty list if no rule pack was found
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
     query = db_connection.query(DBrulePack)
 
     if version:
         query = query.where(DBrulePack.version == version)
     if active is not None:
         query = query.where(DBrulePack.active == active)
-    rule_packs = query.order_by(DBrulePack.version.desc()).offset(skip).limit(limit_val).all()
+    rule_packs = (
+        query.order_by(DBrulePack.version.desc()).offset(skip).limit(limit_val).all()
+    )
     return rule_packs
 
 
 def get_current_active_rule_pack(
     db_connection: Session,
 ) -> Optional[DBrulePack]:
     """
@@ -142,15 +150,17 @@
     query = query.join(DBrule, DBrule.id_ == DBruleTag.rule_id)
     query = query.where(DBrule.rule_pack.in_(versions))
     rule_packs_tags = query.distinct().all()
     rule_packs_tags = [t for (t,) in rule_packs_tags]
     return rule_packs_tags
 
 
-def get_total_rule_packs_count(db_connection: Session, version: str = None, active: bool = None) -> int:
+def get_total_rule_packs_count(
+    db_connection: Session, version: str = None, active: bool = None
+) -> int:
     """
         Retrieve total count of rule packs from database
     :param db_connection:
         Session of the database connection
     :param version:
         optional, filter on rule pack version
     :param active:
@@ -164,17 +174,23 @@
     if active is not None:
         total_count_query = total_count_query.where(DBrulePack.active == active)
 
     total_count = total_count_query.scalar()
     return total_count
 
 
-def make_older_rule_packs_to_inactive(latest_rule_pack_version: str, db_connection: Session):
+def make_older_rule_packs_to_inactive(
+    latest_rule_pack_version: str, db_connection: Session
+):
     """
         Make older rule packs to inactive
     :param latest_rule_pack_version:
         latest rule pack version
     :param db_connection:
         Session of the database connection
     """
-    db_connection.execute(update(DBrulePack).where(DBrulePack.version != latest_rule_pack_version).values(active=False))
+    db_connection.execute(
+        update(DBrulePack)
+        .where(DBrulePack.version != latest_rule_pack_version)
+        .values(active=False)
+    )
     db_connection.commit()
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/rule_tag.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/rule_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from sqlalchemy.orm import Session
 from sqlalchemy.orm.query import Query
 
 # First Party
 from resc_backend.db.model import DBrule, DBruleTag, DBtag
 
 
-def create_rule_tag(db_connection: Session, rule_id: int, tags: List[str]) -> List[DBruleTag]:
+def create_rule_tag(
+    db_connection: Session, rule_id: int, tags: List[str]
+) -> List[DBruleTag]:
     """
     Create rule tag entries, linking / creating tag names to a rule
     :param db_connection:
         Session of the database connection
     :param rule_id:
         ID of the rule to link the tags to
     :param tags:
@@ -81,15 +83,17 @@
     if db_create_tags:
         db_connection.add_all(db_create_tags)
         db_connection.flush()
         db_connection.commit()
     return db_create_tags
 
 
-def get_rule_tag_names_by_rule_pack_version(db_connection: Session, rule_pack_version: str):
+def get_rule_tag_names_by_rule_pack_version(
+    db_connection: Session, rule_pack_version: str
+):
     """
     Get rule names and there tags based on the rule pack version
     :param db_connection:
         Session of the database connection
     :param rule_pack_version:
         Version of the rule pack for which to retrieve the rule tags
     :return: [rule.rule_name, tag.name]
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/scan.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 
 
 def get_scan(db_connection: Session, scan_id: int) -> DBscan:
     scan = db_connection.query(DBscan).where(DBscan.id_ == scan_id).first()
     return scan
 
 
-def get_latest_scan_for_repository(db_connection: Session, repository_id: int) -> DBscan:
+def get_latest_scan_for_repository(
+    db_connection: Session, repository_id: int
+) -> DBscan:
     """
         Retrieve the most recent scan of a given repository object
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository object for which to retrieve the most recent scan
     :return: scan
@@ -67,15 +69,17 @@
     :param skip:
         integer amount of records to skip to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [DBscan]
         List of DBScan objects
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
     query = db_connection.query(DBscan)
 
     if repository_id > 0:
         query = query.where(DBscan.repository_id == repository_id)
 
     scans = query.order_by(DBscan.id_).offset(skip).limit(limit_val).all()
     return scans
@@ -96,15 +100,17 @@
     if repository_id > 0:
         query = query.where(DBscan.repository_id == repository_id)
 
     total_count = query.scalar()
     return total_count
 
 
-def update_scan(db_connection: Session, scan_id: int, scan: scan_schema.ScanCreate) -> DBscan:
+def update_scan(
+    db_connection: Session, scan_id: int, scan: scan_schema.ScanCreate
+) -> DBscan:
     db_scan = db_connection.query(DBscan).filter_by(id_=scan_id).first()
     db_scan.scan_type = scan.scan_type
     db_scan.last_scanned_commit = scan.last_scanned_commit
     db_scan.timestamp = scan.timestamp
     db_scan.increment_number = scan.increment_number
     db_scan.rule_pack = scan.rule_pack
     db_connection.commit()
@@ -148,25 +154,27 @@
         repository id of the latest scan
     :param scan_timestamp:
         timestamp of the latest scan
     :return: findings_metadata
         findings_metadata containing the count for each status
     """
     scan_ids_latest_to_base = []
-    scans = get_scans(db_connection=db_connection, repository_id=repository_id, limit=1000000)
+    scans = get_scans(
+        db_connection=db_connection, repository_id=repository_id, limit=1000000
+    )
     scans.sort(key=lambda x: x.timestamp, reverse=True)
     for scan in scans:
         if scan.timestamp <= scan_timestamp:
             scan_ids_latest_to_base.append(scan.id_)
             if scan.scan_type == ScanType.BASE:
                 break
 
-    true_positive_count = false_positive_count = not_analyzed_count = under_review_count = (
-        clarification_required_count
-    ) = 0
+    true_positive_count = false_positive_count = not_analyzed_count = (
+        under_review_count
+    ) = clarification_required_count = 0
     if len(scan_ids_latest_to_base) > 0:
         findings_count_by_status = finding_crud.get_findings_count_by_status(
             db_connection,
             scan_ids=scan_ids_latest_to_base,
             finding_statuses=FindingStatus,
         )
         for finding in findings_count_by_status:
@@ -199,15 +207,17 @@
         "clarification_required": clarification_required_count,
         "total_findings_count": total_findings_count,
     }
 
     return findings_metadata
 
 
-def delete_repository_findings_not_linked_to_any_scan(db_connection: Session, repository_id: int):
+def delete_repository_findings_not_linked_to_any_scan(
+    db_connection: Session, repository_id: int
+):
     """
         Delete findings for a given repository which are not linked to any scans
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository
     """
@@ -240,26 +250,30 @@
         scan_finding_crud.delete_scan_finding(db_connection, scan_id=scan_id)
 
     query = db_connection.query(DBscan)
     query = query.where(DBscan.id_ == scan_id)
     query.delete(synchronize_session=False)
     db_connection.commit()
 
-    delete_repository_findings_not_linked_to_any_scan(db_connection, repository_id=repository_id)
+    delete_repository_findings_not_linked_to_any_scan(
+        db_connection, repository_id=repository_id
+    )
 
 
 def delete_scans_by_repository_id(db_connection: Session, repository_id: int):
     """
         Delete scans for a given repository
     :param db_connection:
         Session of the database connection
     :param repository_id:
         id of the repository
     """
-    db_connection.query(DBscan).where(DBscan.repository_id == repository_id).delete(synchronize_session=False)
+    db_connection.query(DBscan).where(DBscan.repository_id == repository_id).delete(
+        synchronize_session=False
+    )
     db_connection.commit()
 
 
 def delete_scans_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
     """
         Delete scans for a given vcs instance
     :param db_connection:
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/scan_finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/scan_finding.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     DBrepository,
     DBscan,
     DBscanFinding,
     DBVcsInstance,
 )
 
 
-def create_scan_findings(db_connection: Session, scan_findings: List[DBscanFinding]) -> int:
+def create_scan_findings(
+    db_connection: Session, scan_findings: List[DBscanFinding]
+) -> int:
     if len(scan_findings) < 1:
         # Function is called with an empty list of findings
         return 0
 
     # load existing scan findings for this scan into the session
     scan_id = scan_findings[0].scan_id
     _ = db_connection.query(DBscanFinding).where(DBscanFinding.scan_id == scan_id).all()
@@ -34,15 +36,17 @@
 
 def get_scan_findings(db_connection: Session, finding_id: int) -> List[DBscanFinding]:
     scan_findings = db_connection.query(DBscanFinding)
     scan_findings = scan_findings.where(DBscanFinding.finding_id == finding_id).all()
     return scan_findings
 
 
-def delete_scan_finding(db_connection: Session, finding_id: int = None, scan_id: int = None):
+def delete_scan_finding(
+    db_connection: Session, finding_id: int = None, scan_id: int = None
+):
     """
         Delete scan findings when finding id or scan id provided
     :param db_connection:
         Session of the database connection
     :param finding_id:
         optional, id of the finding
     :param scan_id:
@@ -71,15 +75,17 @@
         DBscanFinding.finding_id == DBfinding.id_,
         DBscan.repository_id == DBfinding.repository_id,
         DBscan.repository_id == repository_id,
     ).delete(synchronize_session=False)
     db_connection.commit()
 
 
-def delete_scan_finding_by_vcs_instance_id(db_connection: Session, vcs_instance_id: int):
+def delete_scan_finding_by_vcs_instance_id(
+    db_connection: Session, vcs_instance_id: int
+):
     """
         Delete scan findings for a given vcs instance
     :param db_connection:
         Session of the database connection
     :param vcs_instance_id:
         id of the vcs instance
     """
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 from resc_backend.resc_web_service.crud import scan as scan_crud
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.schema import vcs_instance as vcs_instance_schema
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 
 def get_vcs_instance(db_connection: Session, vcs_instance_id: int):
-    vcs_instance = db_connection.query(DBVcsInstance).filter(DBVcsInstance.id_ == vcs_instance_id).first()
+    vcs_instance = (
+        db_connection.query(DBVcsInstance)
+        .filter(DBVcsInstance.id_ == vcs_instance_id)
+        .first()
+    )
     return vcs_instance
 
 
 def get_vcs_instances(
     db_connection: Session,
     skip: int = 0,
     limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
@@ -42,24 +46,28 @@
     :param skip:
         integer amount of records to skip to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [DBVcsInstance]
         List of DBVcsInstance objects
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
     query = db_connection.query(DBVcsInstance)
 
     if vcs_provider_type:
         query = query.filter(DBVcsInstance.provider_type == vcs_provider_type)
 
     if vcs_instance_name:
         query = query.filter(DBVcsInstance.name == vcs_instance_name)
 
-    vcs_instances = query.order_by(DBVcsInstance.id_).offset(skip).limit(limit_val).all()
+    vcs_instances = (
+        query.order_by(DBVcsInstance.id_).offset(skip).limit(limit_val).all()
+    )
     return vcs_instances
 
 
 def get_vcs_instances_count(
     db_connection: Session,
     vcs_provider_type: VCSProviders = None,
     vcs_instance_name: str = None,
@@ -88,30 +96,34 @@
 
 
 def update_vcs_instance(
     db_connection: Session,
     vcs_instance_id: int,
     vcs_instance: vcs_instance_schema.VCSInstanceCreate,
 ) -> DBVcsInstance:
-    db_vcs_instance: DBVcsInstance = db_connection.query(DBVcsInstance).filter_by(id_=vcs_instance_id).first()
+    db_vcs_instance: DBVcsInstance = (
+        db_connection.query(DBVcsInstance).filter_by(id_=vcs_instance_id).first()
+    )
     db_vcs_instance.name = vcs_instance.name
     db_vcs_instance.provider_type = vcs_instance.provider_type
     db_vcs_instance.port = vcs_instance.port
     db_vcs_instance.scheme = vcs_instance.scheme
     db_vcs_instance.organization = vcs_instance.organization
     db_vcs_instance.hostname = vcs_instance.hostname
     db_vcs_instance.scope = ",".join(vcs_instance.scope)
     db_vcs_instance.exceptions = ",".join(vcs_instance.exceptions)
 
     db_connection.commit()
     db_connection.refresh(db_vcs_instance)
     return db_vcs_instance
 
 
-def create_vcs_instance(db_connection: Session, vcs_instance: vcs_instance_schema.VCSInstanceCreate) -> DBVcsInstance:
+def create_vcs_instance(
+    db_connection: Session, vcs_instance: vcs_instance_schema.VCSInstanceCreate
+) -> DBVcsInstance:
     db_vcs_instance = DBVcsInstance(
         name=vcs_instance.name,
         provider_type=vcs_instance.provider_type,
         port=vcs_instance.port,
         scheme=vcs_instance.scheme,
         organization=vcs_instance.organization,
         hostname=vcs_instance.hostname,
@@ -120,15 +132,17 @@
     )
     db_connection.add(db_vcs_instance)
     db_connection.commit()
     db_connection.refresh(db_vcs_instance)
     return db_vcs_instance
 
 
-def create_vcs_instance_if_not_exists(db_connection: Session, vcs_instance: vcs_instance_schema.VCSInstanceCreate):
+def create_vcs_instance_if_not_exists(
+    db_connection: Session, vcs_instance: vcs_instance_schema.VCSInstanceCreate
+):
     # Query the database to see if the vcs_instance object exists based on the unique constraint parameters
     db_select_vcs_instance = (
         db_connection.query(DBVcsInstance)
         .filter(
             DBVcsInstance.provider_type == vcs_instance.provider_type,
             DBVcsInstance.scheme == vcs_instance.scheme,
             DBVcsInstance.hostname == vcs_instance.hostname,
@@ -140,25 +154,37 @@
     if db_select_vcs_instance is not None:
         return db_select_vcs_instance
 
     # Create non-existing vcs_instance object
     return create_vcs_instance(db_connection, vcs_instance)
 
 
-def delete_vcs_instance(db_connection: Session, vcs_instance_id: int, delete_related: bool = False):
+def delete_vcs_instance(
+    db_connection: Session, vcs_instance_id: int, delete_related: bool = False
+):
     """
         Delete a vcs instance object
     :param db_connection:
         Session of the database connection
     :param vcs_instance_id:
         id of the vcs instance to be deleted
     :param delete_related:
         if related records need to be deleted
     """
     if delete_related:
-        scan_finding_crud.delete_scan_finding_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
-        finding_crud.delete_findings_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
-        scan_crud.delete_scans_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
-        repository_crud.delete_repositories_by_vcs_instance_id(db_connection, vcs_instance_id=vcs_instance_id)
-    db_vcs_instance = db_connection.query(DBVcsInstance).filter_by(id_=vcs_instance_id).first()
+        scan_finding_crud.delete_scan_finding_by_vcs_instance_id(
+            db_connection, vcs_instance_id=vcs_instance_id
+        )
+        finding_crud.delete_findings_by_vcs_instance_id(
+            db_connection, vcs_instance_id=vcs_instance_id
+        )
+        scan_crud.delete_scans_by_vcs_instance_id(
+            db_connection, vcs_instance_id=vcs_instance_id
+        )
+        repository_crud.delete_repositories_by_vcs_instance_id(
+            db_connection, vcs_instance_id=vcs_instance_id
+        )
+    db_vcs_instance = (
+        db_connection.query(DBVcsInstance).filter_by(id_=vcs_instance_id).first()
+    )
     db_connection.delete(db_vcs_instance)
     db_connection.commit()
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/dependencies.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     SSO_JWT_SIGN_ALGORITHM,
 )
 
 security = HTTPBearer()
 logger = logging.getLogger(__name__)
 
 
-async def requires_auth(request: Request, credentials: HTTPBasicCredentials = Depends(security)):
+async def requires_auth(
+    request: Request, credentials: HTTPBasicCredentials = Depends(security)
+):
     """
     Function that is used to validate the JWT access token
     """
     # Check and load environment variables
     env_variables = validate_environment(CONDITIONAL_SSO_ENV_VARS)
 
     access_token = credentials.credentials
@@ -74,15 +76,17 @@
             logger.error(f"Invalid login attempt for user {user_id}")
             raise HTTPException(
                 status_code=status.HTTP_403_FORBIDDEN,
                 detail="You don't have permission to access this resource.",
             )
         request.scope["user"] = user_id
     except urllib.error.URLError as error:
-        logger.error(f"Unable to contact server for token validation {jwks_url} Message: {error}")
+        logger.error(
+            f"Unable to contact server for token validation {jwks_url} Message: {error}"
+        )
         raise HTTPException(
             status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
             detail="Unable to contact server for token validation",
         ) from error
 
     except jwt.InvalidAlgorithmError as error:
         raise HTTPException(
@@ -196,11 +200,14 @@
         not_found_tables = []
         for table_name in required_table_names:
             table_exists = inspector.has_table(table_name)
             if not table_exists:
                 not_found_tables.append(table_name)
 
         if len(not_found_tables) > 0:
-            raise RuntimeError(f"Unable to determine existence of required table(s) " f"{', '.join(not_found_tables)}")
+            raise RuntimeError(
+                f"Unable to determine existence of required table(s) "
+                f"{', '.join(not_found_tables)}"
+            )
     except Exception as ex:
         logger.error(f"Database is NOT connected or initialized | {ex} | Retrying...")
         raise
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,40 +98,46 @@
         The output will contain a PaginationModel containing the list of DetailedFinding type objects,
         or an empty list if no finding was found
     """
 
     parsed_query_string_params = dict(urllib.parse.parse_qsl(query_string))
 
     if parsed_query_string_params.get("scan_ids"):
-        parsed_query_string_params["scan_ids"] = json.loads(parsed_query_string_params["scan_ids"])
+        parsed_query_string_params["scan_ids"] = json.loads(
+            parsed_query_string_params["scan_ids"]
+        )
     if parsed_query_string_params.get("vcs_providers"):
         parsed_query_string_params["vcs_providers"] = json.loads(
             parsed_query_string_params["vcs_providers"].replace("'", '"')
         )
     if parsed_query_string_params.get("finding_statuses"):
         parsed_query_string_params["finding_statuses"] = json.loads(
             parsed_query_string_params["finding_statuses"].replace("'", '"')
         )
     if parsed_query_string_params.get("rule_names"):
         parsed_query_string_params["rule_names"] = json.loads(
             parsed_query_string_params["rule_names"].replace("'", '"')
         )
     if parsed_query_string_params.get("rule_tags"):
-        parsed_query_string_params["rule_tags"] = json.loads(parsed_query_string_params["rule_tags"].replace("'", '"'))
+        parsed_query_string_params["rule_tags"] = json.loads(
+            parsed_query_string_params["rule_tags"].replace("'", '"')
+        )
     if parsed_query_string_params.get("rule_pack_versions"):
         parsed_query_string_params["rule_pack_versions"] = json.loads(
             parsed_query_string_params["rule_pack_versions"].replace("'", '"')
         )
 
     findings_filter = FindingsFilter(**parsed_query_string_params)
 
     findings = detailed_finding_crud.get_detailed_findings(
         db_connection, findings_filter=findings_filter, skip=skip, limit=limit
     )
-    total_findings = detailed_finding_crud.get_detailed_findings_count(db_connection, findings_filter=findings_filter)
+    total_findings = detailed_finding_crud.get_detailed_findings_count(
+        db_connection, findings_filter=findings_filter
+    )
 
     return PaginationModel[detailed_finding_schema.DetailedFindingRead](
         data=findings, total=total_findings, limit=limit, skip=skip
     )
 
 
 @router.get(
@@ -154,11 +160,13 @@
         Retrieve detailed finding by its ID
 
     - **db_connection**: Session of the database connection
     - **finding_id**: ID of the finding for which details need to be fetched
     - **return**: [DetailedFindingRead]
         The output will contain the details of a finding
     """
-    db_finding = detailed_finding_crud.get_detailed_finding(db_connection, finding_id=finding_id)
+    db_finding = detailed_finding_crud.get_detailed_finding(
+        db_connection, finding_id=finding_id
+    )
     if db_finding is None:
         raise HTTPException(status_code=404, detail="Finding not found")
     return db_finding
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,17 @@
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no finding was found
     """
     findings = finding_crud.get_findings(db_connection, skip=skip, limit=limit)
 
     total_findings = finding_crud.get_total_findings_count(db_connection)
 
-    return PaginationModel[finding_schema.FindingRead](data=findings, total=total_findings, limit=limit, skip=skip)
+    return PaginationModel[finding_schema.FindingRead](
+        data=findings, total=total_findings, limit=limit, skip=skip
+    )
 
 
 @router.post(
     "",
     response_model=int,
     summary="Create a finding",
     status_code=status.HTTP_201_CREATED,
@@ -106,15 +108,17 @@
     - **event_sent_on**: event sent timestamp
     - **rule_name**: rule name
     - **repository_id**: repository id of the finding
     - **return**: int
           The output will contain the number of successful created findings
     """
     try:
-        created_findings = finding_crud.create_findings(db_connection=db_connection, findings=findings)
+        created_findings = finding_crud.create_findings(
+            db_connection=db_connection, findings=findings
+        )
 
         # Clear cache related to findings
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE)
     except KeyError as err:
         raise HTTPException(status_code=400, detail=str(err)) from err
     return len(created_findings)
@@ -139,15 +143,17 @@
 
     - **db_connection**: Session of the database connection
     - **finding_id**: ID of the finding for which details need to be fetched
     """
     db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
     if db_finding is None:
         raise HTTPException(status_code=404, detail="Finding not found")
-    db_scan_findings = scan_finding_crud.get_scan_findings(db_connection, finding_id=finding_id)
+    db_scan_findings = scan_finding_crud.get_scan_findings(
+        db_connection, finding_id=finding_id
+    )
     scan_ids = [x.scan_id for x in db_scan_findings]
     return FindingRead.create_from_db_entities(db_finding=db_finding, scan_ids=scan_ids)
 
 
 @router.patch(
     "/{finding_id}",
     response_model=finding_schema.FindingRead,
@@ -169,23 +175,27 @@
         Partially update a finding by ID
 
     - **db_connection**: Session of the database connection
     - **finding_id**: ID of the finding for which details need to be updated
     - **event_sent_on**: Event sent timestamp
     """
     db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
-    db_sca_findings = scan_finding_crud.get_scan_findings(db_connection, finding_id=finding_id)
+    db_sca_findings = scan_finding_crud.get_scan_findings(
+        db_connection, finding_id=finding_id
+    )
     scan_ids = [x.scan_id for x in db_sca_findings]
 
     # Clear cache related to findings
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     if db_finding is None:
         raise HTTPException(status_code=404, detail="Finding not found")
     return FindingRead.create_from_db_entities(
-        finding_crud.patch_finding(db_connection, finding_id=finding_id, finding_update=finding_update),
+        finding_crud.patch_finding(
+            db_connection, finding_id=finding_id, finding_update=finding_update
+        ),
         scan_ids,
     )
 
 
 @router.delete(
     "/{finding_id}",
     summary="Delete a finding",
@@ -193,26 +203,30 @@
     responses={
         200: {"description": "Delete finding <finding_id>"},
         404: {"model": Model404, "description": "Finding <finding_id> not found"},
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
-async def delete_finding(finding_id: int, db_connection: Session = Depends(get_db_connection)):
+async def delete_finding(
+    finding_id: int, db_connection: Session = Depends(get_db_connection)
+):
     """
         Delete a finding object
 
     - **db_connection**: Session of the database connection
     - **finding_id**: ID of the finding to delete
     - **return**: The output will contain a success or error message based on the success of the deletion
     """
     db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
     if db_finding is None:
         raise HTTPException(status_code=404, detail="Finding not found")
-    finding_crud.delete_finding(db_connection, finding_id=finding_id, delete_related=True)
+    finding_crud.delete_finding(
+        db_connection, finding_id=finding_id, delete_related=True
+    )
 
     # Clear cache related to findings
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     return {"ok": True}
 
 
 @router.get(
@@ -222,23 +236,27 @@
     responses={
         200: {"description": "Retrieve total findings count of rule <rule_name>"},
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
-def get_total_findings_count_by_rule(rule_name: str, db_connection: Session = Depends(get_db_connection)):
+def get_total_findings_count_by_rule(
+    rule_name: str, db_connection: Session = Depends(get_db_connection)
+):
     """
         Retrieve total findings count for a given rule
 
     - **db_connection**: Session of the database connection
     - **rule_name**: name of the rule
     """
     findings_filter = FindingsFilter(rule_names=[rule_name])
-    return finding_crud.get_total_findings_count(db_connection, findings_filter=findings_filter)
+    return finding_crud.get_total_findings_count(
+        db_connection, findings_filter=findings_filter
+    )
 
 
 @router.get(
     f"{RWS_ROUTE_BY_RULE}" "/{rule_name}",
     response_model=PaginationModel[finding_schema.FindingRead],
     summary="Get findings by rule",
     status_code=status.HTTP_200_OK,
@@ -262,19 +280,23 @@
     - **rule_name**: Name of the rule to filter the findings by
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **return**: [FindingRead]
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no finding was found for the given rule
     """
-    findings = finding_crud.get_findings_by_rule(db_connection, skip=skip, limit=limit, rule_name=rule_name)
+    findings = finding_crud.get_findings_by_rule(
+        db_connection, skip=skip, limit=limit, rule_name=rule_name
+    )
     total_findings = finding_crud.get_total_findings_count(
         db_connection, findings_filter=FindingsFilter(rule_names=[rule_name])
     )
-    return PaginationModel[finding_schema.FindingRead](data=findings, total=total_findings, limit=limit, skip=skip)
+    return PaginationModel[finding_schema.FindingRead](
+        data=findings, total=total_findings, limit=limit, skip=skip
+    )
 
 
 @router.post(
     f"{RWS_ROUTE_AUDIT}/",
     response_model=int,
     summary="audit single/multiple findings",
     status_code=status.HTTP_201_CREATED,
@@ -301,15 +323,17 @@
     - **return**: int
         The output will contain count of successful saved audits
     """
     audits = []
     for finding_id in audit.finding_ids:
         db_finding = finding_crud.get_finding(db_connection, finding_id=finding_id)
         if db_finding is None:
-            raise HTTPException(status_code=404, detail=f"Finding {finding_id} not found")
+            raise HTTPException(
+                status_code=404, detail=f"Finding {finding_id} not found"
+            )
         audits.append(
             audit_crud.create_audit(
                 db_connection=db_connection,
                 finding_id=db_finding.id_,
                 auditor=request.user,
                 status=audit.status,
                 comment=audit.comment,
@@ -346,17 +370,23 @@
     - **finding_id**: id of the finding to get the audit for
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **return**: [AuditRead]
         The output will contain a PaginationModel containing the list of AuditRead type objects,
         or an empty list if no audit info was found
     """
-    audits = audit_crud.get_finding_audits(db_connection, skip=skip, limit=limit, finding_id=finding_id)
-    total_audits = audit_crud.get_finding_audits_count(db_connection, finding_id=finding_id)
-    return PaginationModel[audit_schema.AuditRead](data=audits, total=total_audits, limit=limit, skip=skip)
+    audits = audit_crud.get_finding_audits(
+        db_connection, skip=skip, limit=limit, finding_id=finding_id
+    )
+    total_audits = audit_crud.get_finding_audits_count(
+        db_connection, finding_id=finding_id
+    )
+    return PaginationModel[audit_schema.AuditRead](
+        data=audits, total=total_audits, limit=limit, skip=skip
+    )
 
 
 @router.get(
     f"{RWS_ROUTE_SUPPORTED_STATUSES}/",
     response_model=List[str],
     summary="Get all supported statuses for findings",
     status_code=status.HTTP_200_OK,
@@ -370,15 +400,17 @@
 def get_supported_statuses() -> List[str]:
     """
         Retrieve all supported statuses for findings
 
     - **return**: List[str]
         The output will contain a list of strings of unique statuses supported
     """
-    supported_finding_statuses = [finding_status for finding_status in FindingStatus if finding_status]
+    supported_finding_statuses = [
+        finding_status for finding_status in FindingStatus if finding_status
+    ]
     return supported_finding_statuses
 
 
 @router.get(
     f"{RWS_ROUTE_COUNT_BY_TIME}/" "{time_type}",
     response_model=PaginationModel[DateCountModel],
     summary="Get all the findings by time period",
@@ -423,19 +455,25 @@
         db_connection=db_connection,
         date_type=time_type,
         start_date_time=start_date_time,
         end_date_time=end_date_time,
     )
     for finding in findings:
         if time_type == DateFilter.MONTH:
-            date_count = DateCountModel(finding_count=finding[2], date_lable=f"{finding[0]}-{finding[1]}")
+            date_count = DateCountModel(
+                finding_count=finding[2], date_lable=f"{finding[0]}-{finding[1]}"
+            )
         elif time_type == DateFilter.WEEK:
-            date_count = DateCountModel(finding_count=finding[2], date_lable=f"{finding[0]}-W{finding[1]}")
+            date_count = DateCountModel(
+                finding_count=finding[2], date_lable=f"{finding[0]}-W{finding[1]}"
+            )
         elif time_type == DateFilter.DAY:
             date_count = DateCountModel(
                 finding_count=finding[3],
                 date_lable=f"{finding[0]}-{finding[1]}-{finding[2]}",
             )
 
         date_counts.append(date_count)
 
-    return PaginationModel[DateCountModel](data=date_counts, total=total_findings, limit=limit, skip=skip)
+    return PaginationModel[DateCountModel](
+        data=date_counts, total=total_findings, limit=limit, skip=skip
+    )
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/metrics.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 
 @router.get(
     f"{RWS_ROUTE_AUDITED_COUNT_OVER_TIME}",
     response_model=list[FindingCountOverTime],
     summary="Get count of audit status over time for given weeks per vcs provider",
     status_code=status.HTTP_200_OK,
     responses={
-        200: {"description": "Retrieve count of audit status over time for given weeks per vcs provider"},
+        200: {
+            "description": "Retrieve count of audit status over time for given weeks per vcs provider"
+        },
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def get_finding_audit_count_over_time(
     db_connection: Session = Depends(get_db_connection),
@@ -67,25 +69,29 @@
     - **audit_status**: audit status for which to retrieve the counts, defaults to True positive
     - **return**: [DateCountModel]
         The output will contain a list of DateCountModel type objects
     """
     audit_counts = finding_crud.get_finding_audit_status_count_over_time(
         db_connection=db_connection, status=audit_status, weeks=weeks
     )
-    output = convert_rows_to_finding_count_over_time(count_over_time=audit_counts, weeks=weeks)
+    output = convert_rows_to_finding_count_over_time(
+        count_over_time=audit_counts, weeks=weeks
+    )
     return output
 
 
 @router.get(
     f"{RWS_ROUTE_COUNT_PER_VCS_PROVIDER_BY_WEEK}",
     response_model=list[FindingCountOverTime],
     summary="Get count of findings over time for given weeks per vcs provider",
     status_code=status.HTTP_200_OK,
     responses={
-        200: {"description": "Retrieve count of findings over time for given weeks per vcs provider"},
+        200: {
+            "description": "Retrieve count of findings over time for given weeks per vcs provider"
+        },
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def get_finding_total_count_over_time(
     db_connection: Session = Depends(get_db_connection),
@@ -95,26 +101,32 @@
         Retrieve count of findings over time for given weeks per vcs provider
     - **db_connection**: Session of the database connection
     - **weeks**: Nr of weeks for which to retrieve the audit status count
     - **audit_status**: audit status for which to retrieve the counts, defaults to True positive
     - **return**: [DateCountModel]
         The output will contain a list of DateCountModel type objects
     """
-    audit_counts = finding_crud.get_finding_count_by_vcs_provider_over_time(db_connection=db_connection, weeks=weeks)
-    output = convert_rows_to_finding_count_over_time(count_over_time=audit_counts, weeks=weeks)
+    audit_counts = finding_crud.get_finding_count_by_vcs_provider_over_time(
+        db_connection=db_connection, weeks=weeks
+    )
+    output = convert_rows_to_finding_count_over_time(
+        count_over_time=audit_counts, weeks=weeks
+    )
     return output
 
 
 @router.get(
     f"{RWS_ROUTE_UN_TRIAGED_COUNT_OVER_TIME}",
     response_model=list[FindingCountOverTime],
     summary="Get count of UnTriaged findings over time for given weeks per vcs provider",
     status_code=status.HTTP_200_OK,
     responses={
-        200: {"description": "Retrieve count of UnTriaged findings over time for given weeks per vcs provider"},
+        200: {
+            "description": "Retrieve count of UnTriaged findings over time for given weeks per vcs provider"
+        },
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def get_finding_un_triaged_count_over_time(
     db_connection: Session = Depends(get_db_connection),
@@ -127,19 +139,23 @@
     - **audit_status**: audit status for which to retrieve the counts, defaults to True positive
     - **return**: [DateCountModel]
         The output will contain a list of DateCountModel type objects
     """
     audit_counts = finding_crud.get_un_triaged_finding_count_by_vcs_provider_over_time(
         db_connection=db_connection, weeks=weeks
     )
-    output = convert_rows_to_finding_count_over_time(count_over_time=audit_counts, weeks=weeks)
+    output = convert_rows_to_finding_count_over_time(
+        count_over_time=audit_counts, weeks=weeks
+    )
     return output
 
 
-def convert_rows_to_finding_count_over_time(count_over_time: dict, weeks: int) -> list[FindingCountOverTime]:
+def convert_rows_to_finding_count_over_time(
+    count_over_time: dict, weeks: int
+) -> list[FindingCountOverTime]:
     """
         Convert the rows from the database to the format of list[FindingCountOverTime]
     :param count_over_time:
         rows from the database
     :param weeks:
         number fo weeks that are in the data
     :return: output
@@ -149,28 +165,32 @@
     vcs_provider_types = list(VCSProviders)
 
     # create defaults with 0 value
     week_groups = {}
     for week in range(0, weeks):
         nth_week = datetime.utcnow() - timedelta(weeks=week)
         week = f"{nth_week.isocalendar().year} W{nth_week.isocalendar().week:02d}"
-        week_groups[week] = {vcs_provider_type: 0 for vcs_provider_type in vcs_provider_types + ["total"]}
+        week_groups[week] = {
+            vcs_provider_type: 0 for vcs_provider_type in vcs_provider_types + ["total"]
+        }
 
     # loop over the counts from the database
     for data in count_over_time:
         week = f"{getattr(data, 'year')} W{getattr(data, 'week'):02d}"
         finding_count = getattr(data, "finding_count")
 
         week_groups[week][getattr(data, "provider_type")] += finding_count
         week_groups[week]["total"] += finding_count
 
     # Convert to the output format
     output = []
     for week in sorted(week_groups.keys()):
-        week_data = FindingCountOverTime(time_period=week, total=week_groups[week]["total"])
+        week_data = FindingCountOverTime(
+            time_period=week, total=week_groups[week]["total"]
+        )
         for vcs_provider_type in vcs_provider_types:
             setattr(
                 week_data.vcs_provider_finding_count,
                 vcs_provider_type,
                 week_groups[week][vcs_provider_type],
             )
 
@@ -180,15 +200,17 @@
 
 @router.get(
     f"{RWS_ROUTE_AUDIT_COUNT_BY_AUDITOR_OVER_TIME}",
     response_model=list[AuditCountOverTime],
     summary="Get count of Audits by Auditor over time for given weeks",
     status_code=status.HTTP_200_OK,
     responses={
-        200: {"description": "Retrieve count of Audits by Auditor over time for given weeks"},
+        200: {
+            "description": "Retrieve count of Audits by Auditor over time for given weeks"
+        },
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def get_audit_count_by_auditor_over_time(
     db_connection: Session = Depends(get_db_connection),
@@ -197,36 +219,40 @@
     """
         Retrieve count of Audits by Auditor over time for given weeks
     - **db_connection**: Session of the database connection
     - **weeks**: Nr of weeks for which to retrieve the audit counts
     - **return**: [AuditCountOverTime]
         The output will contain a list of AuditCountOverTime type objects
     """
-    audit_counts = audit_crud.get_audit_count_by_auditor_over_time(db_connection=db_connection, weeks=weeks)
+    audit_counts = audit_crud.get_audit_count_by_auditor_over_time(
+        db_connection=db_connection, weeks=weeks
+    )
 
     # get the unique auditors from the data
     auditors_default = {}
     for audit in audit_counts:
         auditors_default[getattr(audit, "auditor")] = 0
 
     # default to 0 per auditor for all weeks in range
     weekly_audit_counts = {}
     for week in range(0, weeks):
         nth_week = datetime.utcnow() - timedelta(weeks=week)
         week = f"{nth_week.isocalendar().year} W{nth_week.isocalendar().week:02d}"
-        weekly_audit_counts[week] = AuditCountOverTime(time_period=week, audit_by_auditor_count=dict(auditors_default))
+        weekly_audit_counts[week] = AuditCountOverTime(
+            time_period=week, audit_by_auditor_count=dict(auditors_default)
+        )
     weekly_audit_counts = dict(sorted(weekly_audit_counts.items()))
 
     # set the counts based on the data from the database
     for audit in audit_counts:
         audit_week = f"{getattr(audit, 'year')} W{getattr(audit, 'week'):02d}"
         if audit_week in weekly_audit_counts:
-            weekly_audit_counts.get(audit_week).audit_by_auditor_count[getattr(audit, "auditor")] = getattr(
-                audit, "audit_count"
-            )
+            weekly_audit_counts.get(audit_week).audit_by_auditor_count[
+                getattr(audit, "auditor")
+            ] = getattr(audit, "audit_count")
             weekly_audit_counts.get(audit_week).total += getattr(audit, "audit_count")
 
     sorted_weekly_audit_counts = dict(sorted(weekly_audit_counts.items()))
     output = list(sorted_weekly_audit_counts.values())
     return output
 
 
@@ -290,19 +316,23 @@
         Retrieve personal audit ranking this week, compared to other auditors
     - **db_connection**: Session of the database connection
     - **auditor**: id of the auditor
     - **return**: int
         The output will be an integer nr of the ranking this week, defaulting to 0 if no audit was done by the auditor
     """
     audit_rank = 0
-    audit_counts_db = audit_crud.get_audit_count_by_auditor_over_time(db_connection=db_connection, weeks=0)
+    audit_counts_db = audit_crud.get_audit_count_by_auditor_over_time(
+        db_connection=db_connection, weeks=0
+    )
 
     auditor_counts = {}
     for audit in audit_counts_db:
         auditor_counts[getattr(audit, "auditor")] = getattr(audit, "audit_count")
 
-    sorted_auditor_counts = sorted(auditor_counts.items(), key=lambda x: x[1], reverse=True)
+    sorted_auditor_counts = sorted(
+        auditor_counts.items(), key=lambda x: x[1], reverse=True
+    )
     for auditor_count in dict(sorted_auditor_counts):
         audit_rank += 1
         if auditor_count == auditor:
             return audit_rank
     return 0
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,17 @@
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 def get_all_repositories(
     skip: int = Query(default=0, ge=0),
     limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-    vcsproviders: List[VCSProviders] = Query(None, alias="vcsprovider", title="VCSProviders"),
+    vcsproviders: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
     projectfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
     repositoryfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
     db_connection: Session = Depends(get_db_connection),
 ) -> PaginationModel[repository_schema.RepositoryRead]:
     """
         Retrieve all repository objects paginated
 
@@ -114,15 +116,17 @@
     - **db_connection**: Session of the database connection
     - **project_key**: each repository must have a project name or key
     - **repository_id**: repository id
     - **repository_name**: repository name
     - **repository_url**: repository url
     - **vcs_instance**: vcs instance id
     """
-    repository = repository_crud.create_repository_if_not_exists(db_connection=db_connection, repository=repository)
+    repository = repository_crud.create_repository_if_not_exists(
+        db_connection=db_connection, repository=repository
+    )
 
     # Clear cache related to repository
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_REPOSITORY)
     return repository
 
 
 @router.get(
@@ -133,22 +137,26 @@
     responses={
         200: {"description": "Retrieve repository <repository_id>"},
         404: {"model": Model404, "description": "Repository <repository_id> not found"},
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
-def read_repository(repository_id: int, db_connection: Session = Depends(get_db_connection)):
+def read_repository(
+    repository_id: int, db_connection: Session = Depends(get_db_connection)
+):
     """
         Read a repository by ID
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the repository for which details need to be fetched
     """
-    db_repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
+    db_repository = repository_crud.get_repository(
+        db_connection, repository_id=repository_id
+    )
     if db_repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
     return db_repository
 
 
 @router.put(
     "/{repository_id}",
@@ -174,15 +182,17 @@
     - **repository_id**: ID of the repository
     - **project_key**: project name that needs to be updated
     - **repository_id**: repository id that needs to be updated
     - **repository_name**: repository name that needs to be updated
     - **repository_url**: repository url that needs to be updated
     - **vcs_instance**: vcs instance id that needs to be updated
     """
-    db_repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
+    db_repository = repository_crud.get_repository(
+        db_connection, repository_id=repository_id
+    )
     if db_repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
 
     updated_repository = repository_crud.update_repository(
         db_connection=db_connection, repository_id=repository_id, repository=repository
     )
 
@@ -198,26 +208,32 @@
     responses={
         200: {"description": "Delete repository <repository_id>"},
         404: {"model": Model404, "description": "Repository <repository_id> not found"},
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
-async def delete_repository(repository_id: int, db_connection: Session = Depends(get_db_connection)):
+async def delete_repository(
+    repository_id: int, db_connection: Session = Depends(get_db_connection)
+):
     """
         Delete a repository
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the repository to delete
     - **return**: The output will contain a success or error message based on the success of the deletion
     """
-    db_repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
+    db_repository = repository_crud.get_repository(
+        db_connection, repository_id=repository_id
+    )
     if db_repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
-    repository_crud.delete_repository(db_connection, repository_id=repository_id, delete_related=True)
+    repository_crud.delete_repository(
+        db_connection, repository_id=repository_id, delete_related=True
+    )
 
     # Clear cache related to repository
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_REPOSITORY)
     return {"ok": True}
 
 
 @router.get(
@@ -229,15 +245,17 @@
         200: {"description": "Retrieve all the unique project-names"},
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_REPOSITORY, expire=REDIS_CACHE_EXPIRE)
 def get_distinct_projects(
-    vcsproviders: List[VCSProviders] = Query(None, alias="vcsprovider", title="VCSProviders"),
+    vcsproviders: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
     repositoryfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
     onlyifhasfindings: bool = Query(default=False),
     db_connection: Session = Depends(get_db_connection),
 ) -> List[str]:
     """
         Retrieve all unique project names
 
@@ -268,15 +286,17 @@
         200: {"description": "Retrieve all the unique repository names"},
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_REPOSITORY, expire=REDIS_CACHE_EXPIRE)
 def get_distinct_repositories(
-    vcsproviders: List[VCSProviders] = Query(None, alias="vcsprovider", title="VCSProviders"),
+    vcsproviders: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
     projectname: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
     onlyifhasfindings: bool = Query(default=False),
     db_connection: Session = Depends(get_db_connection),
 ) -> List[str]:
     """
         Retrieve all unique repository names
 
@@ -300,15 +320,17 @@
 
 @router.get(
     "/{repository_id}" f"{RWS_ROUTE_FINDINGS_METADATA}",
     response_model=FindingCountModel[repository_schema.RepositoryRead],
     summary="Get findings metadata for a repository",
     status_code=status.HTTP_200_OK,
     responses={
-        200: {"description": "Retrieve findings metadata for repository <repository_id>"},
+        200: {
+            "description": "Retrieve findings metadata for repository <repository_id>"
+        },
         404: {"model": Model404, "description": "Repository <repository_id> not found"},
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 def get_findings_metadata_for_repository(
     repository_id: int, db_connection: Session = Depends(get_db_connection)
@@ -318,49 +340,57 @@
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the repository object for which findings metadata to be retrieved
     - **return**: RepositoryRead, findings count per status
         The output will contain a RepositoryRead type object along with findings count per status,
         or empty if no scan was found
     """
-    repository = repository_crud.get_repository(db_connection, repository_id=repository_id)
+    repository = repository_crud.get_repository(
+        db_connection, repository_id=repository_id
+    )
     if repository is None:
         raise HTTPException(status_code=404, detail="Repository not found")
 
     findings_meta_data = repository_crud.get_findings_metadata_by_repository_id(
         db_connection, repository_ids=[repository_id]
     )
 
     return FindingCountModel[repository_schema.RepositoryRead](
         data=repository,
         true_positive=findings_meta_data[repository_id]["true_positive"],
         false_positive=findings_meta_data[repository_id]["false_positive"],
         not_analyzed=findings_meta_data[repository_id]["not_analyzed"],
         under_review=findings_meta_data[repository_id]["under_review"],
-        clarification_required=findings_meta_data[repository_id]["clarification_required"],
+        clarification_required=findings_meta_data[repository_id][
+            "clarification_required"
+        ],
         total_findings_count=findings_meta_data[repository_id]["total_findings_count"],
     )
 
 
 @router.get(
     f"{RWS_ROUTE_FINDINGS_METADATA}/",
     response_model=PaginationModel[repository_enriched_schema.RepositoryEnrichedRead],
     summary="Get all repositories with findings metadata",
     status_code=status.HTTP_200_OK,
     responses={
-        200: {"description": "Retrieve all the findings metadata for all the repositories"},
+        200: {
+            "description": "Retrieve all the findings metadata for all the repositories"
+        },
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def get_all_repositories_with_findings_metadata(
     skip: int = Query(default=0, ge=0),
     limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-    vcsproviders: List[VCSProviders] = Query(None, alias="vcsprovider", title="VCSProviders"),
+    vcsproviders: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
     projectfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
     repositoryfilter: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
     onlyifhasfindings: bool = Query(default=False),
     db_connection: Session = Depends(get_db_connection),
 ) -> PaginationModel[repository_enriched_schema.RepositoryEnrichedRead]:
     """
         Retrieve all repository objects paginated
@@ -409,16 +439,20 @@
             vcs_provider=repo.provider_type,
             last_scan_id=repo.last_scan_id,
             last_scan_timestamp=repo.last_scan_timestamp,
             true_positive=repo_findings_meta_data[repo.id_]["true_positive"],
             false_positive=repo_findings_meta_data[repo.id_]["false_positive"],
             not_analyzed=repo_findings_meta_data[repo.id_]["not_analyzed"],
             under_review=repo_findings_meta_data[repo.id_]["under_review"],
-            clarification_required=repo_findings_meta_data[repo.id_]["clarification_required"],
-            total_findings_count=repo_findings_meta_data[repo.id_]["total_findings_count"],
+            clarification_required=repo_findings_meta_data[repo.id_][
+                "clarification_required"
+            ],
+            total_findings_count=repo_findings_meta_data[repo.id_][
+                "total_findings_count"
+            ],
         )
         repository_list.append(enriched_repository)
 
     return PaginationModel[repository_enriched_schema.RepositoryEnrichedRead](
         data=repository_list, total=total_repositories, limit=limit, skip=skip
     )
 
@@ -443,15 +477,17 @@
 
     - **db_connection**: Session of the database connection
     - **repository_id**: ID of the parent repository object for which scan objects to be retrieved
     - **return**: ScanRead
         The output will contain a ScanRead type object,
         or empty if no scan was found
     """
-    last_scan = scan_crud.get_latest_scan_for_repository(db_connection, repository_id=repository_id)
+    last_scan = scan_crud.get_latest_scan_for_repository(
+        db_connection, repository_id=repository_id
+    )
     if last_scan is None:
         raise HTTPException(status_code=404, detail="Scan not found")
     return last_scan
 
 
 @router.get(
     "/{repository_id}" f"{RWS_ROUTE_SCANS}",
@@ -477,12 +513,16 @@
     - **repository_id**: ID of the parent repository object for which scan objects to be retrieved
     - **skip**: Integer amount of records to skip to support pagination
     - **limit**: Integer amount of records to return, to support pagination
     - **return**: [ScanRead]
         The output will contain a PaginationModel containing the list of ScanRead type objects,
         or an empty list if no scan was found
     """
-    scans = scan_crud.get_scans(db_connection, skip=skip, limit=limit, repository_id=repository_id)
+    scans = scan_crud.get_scans(
+        db_connection, skip=skip, limit=limit, repository_id=repository_id
+    )
 
     total_scans = scan_crud.get_scans_count(db_connection, repository_id=repository_id)
 
-    return PaginationModel[scan_schema.ScanRead](data=scans, total=total_scans, limit=limit, skip=skip)
+    return PaginationModel[scan_schema.ScanRead](
+        data=scans, total=total_scans, limit=limit, skip=skip
+    )
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,17 @@
         active=active,
         skip=skip,
         limit=limit,
     )
     total_rule_packs_count = rule_pack_crud.get_total_rule_packs_count(
         db_connection=db_connection, version=version, active=active
     )
-    return PaginationModel[RulePackRead](data=rule_packs, total=total_rule_packs_count, limit=limit, skip=skip)
+    return PaginationModel[RulePackRead](
+        data=rule_packs, total=total_rule_packs_count, limit=limit, skip=skip
+    )
 
 
 @router.get(
     "",
     summary="Download rule pack in TOML format",
     status_code=status.HTTP_200_OK,
     responses={
@@ -122,28 +124,36 @@
         Download rule pack in TOML format
 
     - **db_connection**: Session of the database connection
     - **version**: Optional, filter on rule pack version
     - **return**: [FileResponse] The output returns rule pack file downloaded in TOML format
     """
     if not version:
-        logger.info("rule pack version not specified, downloading the currently active version")
+        logger.info(
+            "rule pack version not specified, downloading the currently active version"
+        )
     rule_pack_from_db = read_rule_pack(version=version, db_connection=db_connection)
     if rule_pack_from_db:
         version = rule_pack_from_db.version
-        rules = rule_crud.get_rules_by_rule_pack_version(db_connection=db_connection, rule_pack_version=version)
+        rules = rule_crud.get_rules_by_rule_pack_version(
+            db_connection=db_connection, rule_pack_version=version
+        )
         rule_tag_names = rule_tag_crud.get_rule_tag_names_by_rule_pack_version(
             db_connection=db_connection, rule_pack_version=version
         )
         global_allow_list = rule_crud.get_global_allow_list_by_rule_pack_version(
             db_connection=db_connection, rule_pack_version=version
         )
-        generated_toml_dict = create_toml_dictionary(version, rules, global_allow_list, rule_tag_names)
+        generated_toml_dict = create_toml_dictionary(
+            version, rules, global_allow_list, rule_tag_names
+        )
     else:
-        raise HTTPException(status_code=404, detail=f"No rule pack found with version {version}")
+        raise HTTPException(
+            status_code=404, detail=f"No rule pack found with version {version}"
+        )
 
     toml_file = create_toml_rule_file(generated_toml_dict)
     return FileResponse(toml_file.name, filename="RESC-SECRETS-RULE.toml")
 
 
 @router.post(
     "",
@@ -184,20 +194,23 @@
     toml_rule_dictionary = tomlkit.loads(content)
 
     # Check if rule pack version exists
     rule_pack_from_db = read_rule_pack(version=version, db_connection=db_connection)
     if rule_pack_from_db:
         raise HTTPException(
             status_code=409,
-            detail=f"Unable to process rules. Rule pack version " f"{version} already exists",
+            detail=f"Unable to process rules. Rule pack version "
+            f"{version} already exists",
         )
 
     # Insert in to RULE_ALLOW_LIST for storing global allow list
     created_global_rule_allow_list = None
-    global_allow_list: RuleAllowList = get_mapped_global_allow_list_obj(toml_rule_dictionary)
+    global_allow_list: RuleAllowList = get_mapped_global_allow_list_obj(
+        toml_rule_dictionary
+    )
     if global_allow_list:
         created_global_rule_allow_list = create_rule_allow_list(
             rule_allow_list=global_allow_list, db_connection=db_connection
         )
         if not created_global_rule_allow_list.id_:
             logger.warning("Creating global rule allow list failed with an error")
 
@@ -206,25 +219,31 @@
         created_global_rule_allow_list.id_
         if created_global_rule_allow_list and created_global_rule_allow_list.id_
         else None
     )
 
     # Determine if uploaded rule pack needs to be activated
     current_newest_rule_pack = rule_pack_crud.get_newest_rule_pack(db_connection)
-    activate_uploaded_rule_pack = determine_uploaded_rule_pack_activation(version, current_newest_rule_pack)
+    activate_uploaded_rule_pack = determine_uploaded_rule_pack_activation(
+        version, current_newest_rule_pack
+    )
 
     rule_pack = RulePackCreate(
         version=version,
         active=activate_uploaded_rule_pack,
         global_allow_list=global_allow_list_id,
     )
-    created_rule_pack_version = create_rule_pack_version(rule_pack=rule_pack, db_connection=db_connection)
+    created_rule_pack_version = create_rule_pack_version(
+        rule_pack=rule_pack, db_connection=db_connection
+    )
     if created_rule_pack_version.version and activate_uploaded_rule_pack:
         # Update older rule packs to inactive
-        rule_pack_crud.make_older_rule_packs_to_inactive(latest_rule_pack_version=version, db_connection=db_connection)
+        rule_pack_crud.make_older_rule_packs_to_inactive(
+            latest_rule_pack_version=version, db_connection=db_connection
+        )
     else:
         logger.warning("Creating rule pack failed with an error")
 
     # Insert in to RULES
     if created_rule_pack_version and created_rule_pack_version.version:
         insert_rules(
             version=version,
@@ -235,15 +254,17 @@
         # Clear cache related to rule-pack
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE)
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE_PACK)
         await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     return {"filename": rule_file.filename}
 
 
-def read_rule_pack(version: Optional[str] = None, db_connection: Session = Depends(get_db_connection)) -> RulePackRead:
+def read_rule_pack(
+    version: Optional[str] = None, db_connection: Session = Depends(get_db_connection)
+) -> RulePackRead:
     """
         Read active rule pack from database
     :param version:
         optional, version of the rule pack to be fetched else latest rule pack version will be fetched
     :param db_connection:
         Session of the database connection
     :return: RulePackRead
@@ -252,46 +273,58 @@
     if version:
         regex = re.compile(r"^\d+(?:\.\d+){2}$")
         if not re.fullmatch(regex, version):
             raise HTTPException(
                 status_code=422,
                 detail=f"Version {version} is not a valid semantic version",
             )
-    db_rule_pack = rule_pack_crud.get_rule_pack(db_connection=db_connection, version=version)
+    db_rule_pack = rule_pack_crud.get_rule_pack(
+        db_connection=db_connection, version=version
+    )
     return db_rule_pack
 
 
-def create_rule_pack_version(rule_pack: RulePackCreate, db_connection: Session = Depends(get_db_connection)):
+def create_rule_pack_version(
+    rule_pack: RulePackCreate, db_connection: Session = Depends(get_db_connection)
+):
     """
         Create rule pack version in database
     :param rule_pack:
         RulePackCreate object to be created
     :param db_connection:
         Session of the database connection
     """
-    return rule_pack_crud.create_rule_pack_version(db_connection=db_connection, rule_pack=rule_pack)
+    return rule_pack_crud.create_rule_pack_version(
+        db_connection=db_connection, rule_pack=rule_pack
+    )
 
 
-def create_rule_allow_list(rule_allow_list: RuleAllowList, db_connection: Session = Depends(get_db_connection)):
+def create_rule_allow_list(
+    rule_allow_list: RuleAllowList, db_connection: Session = Depends(get_db_connection)
+):
     """
         Create rule allow list in database
     :param rule_allow_list:
         RuleAllowList object to be created
     :param db_connection:
         Session of the database connection
     """
     if (
         rule_allow_list.paths
         or rule_allow_list.commits
         or rule_allow_list.stop_words
         or rule_allow_list.description
         or rule_allow_list.regexes
     ):
-        return rule_crud.create_rule_allow_list(db_connection=db_connection, rule_allow_list=rule_allow_list)
-    raise HTTPException(status_code=400, detail="No properties defined for rule allow list")
+        return rule_crud.create_rule_allow_list(
+            db_connection=db_connection, rule_allow_list=rule_allow_list
+        )
+    raise HTTPException(
+        status_code=400, detail="No properties defined for rule allow list"
+    )
 
 
 def insert_rules(
     version: str,
     toml_rule_dictionary: dict,
     db_connection: Session = Depends(get_db_connection),
 ):
@@ -340,15 +373,17 @@
                 description=description,
                 entropy=entropy,
                 secret_group=secret_group,
                 regex=regex,
                 path=path,
                 keywords=keywords,
             )
-            created_rule = rule_crud.create_rule(rule=rule_obj, db_connection=db_connection)
+            created_rule = rule_crud.create_rule(
+                rule=rule_obj, db_connection=db_connection
+            )
             if not created_rule.id_:
                 logger.warning(f"Creating rule failed for Rule: {rule_name}")
             if "tags" in rule:
                 _ = rule_tag_crud.create_rule_tag(
                     db_connection=db_connection,
                     rule_id=created_rule.id_,
                     tags=rule["tags"],
@@ -376,19 +411,25 @@
 
     :param db_connection: Session of the database connection
     :param versions: Optional, filter on rule pack version, if not provided filter on active.
     :return: List[str]
         The output will contain a list of tags related to one or more rule-packs.
     """
     if not versions:
-        active_rule_pack = rule_pack_crud.get_current_active_rule_pack(db_connection=db_connection)
+        active_rule_pack = rule_pack_crud.get_current_active_rule_pack(
+            db_connection=db_connection
+        )
         if not active_rule_pack:
-            raise HTTPException(status_code=500, detail="No currently active rule pack.")
+            raise HTTPException(
+                status_code=500, detail="No currently active rule pack."
+            )
         versions = [active_rule_pack.version]
-    rule_packs_tags = rule_pack_crud.get_rule_packs_tags(db_connection=db_connection, versions=versions)
+    rule_packs_tags = rule_pack_crud.get_rule_packs_tags(
+        db_connection=db_connection, versions=versions
+    )
     return rule_packs_tags
 
 
 def determine_uploaded_rule_pack_activation(
     requested_rule_pack_version: str, latest_rule_pack_from_db: RulePackRead
 ) -> bool:
     """
@@ -397,15 +438,17 @@
         version of the rule pack uploaded
     :param latest_rule_pack_from_db:
         latest rule pack in RulePackRead object
     :return: boolean
         The output returns true if rule pack needs to be activated else returns false
     """
     if latest_rule_pack_from_db:
-        if Version(latest_rule_pack_from_db.version) < Version(requested_rule_pack_version):
+        if Version(latest_rule_pack_from_db.version) < Version(
+            requested_rule_pack_version
+        ):
             logger.info(
                 f"Uploaded rule pack is of version '{requested_rule_pack_version}', using it to replace "
                 f"'{latest_rule_pack_from_db.version}' as the active one."
             )
             activate_uploaded_rule_pack = True
         else:
             if not latest_rule_pack_from_db.active:
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,28 +34,36 @@
 
 @router.get(
     f"{RWS_ROUTE_DETECTED_RULES}",
     response_model=List[str],
     summary="Get unique rules from findings",
     status_code=status.HTTP_200_OK,
     responses={
-        200: {"description": "Retrieve all the unique detected rules across all the findings"},
+        200: {
+            "description": "Retrieve all the unique detected rules across all the findings"
+        },
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_RULE, expire=REDIS_CACHE_EXPIRE)
 def get_distinct_rules_from_findings(
-    finding_statuses: List[FindingStatus] = Query(None, alias="findingstatus", title="FindingStatuses"),
-    vcs_providers: List[VCSProviders] = Query(None, alias="vcsprovider", title="VCSProviders"),
+    finding_statuses: List[FindingStatus] = Query(
+        None, alias="findingstatus", title="FindingStatuses"
+    ),
+    vcs_providers: List[VCSProviders] = Query(
+        None, alias="vcsprovider", title="VCSProviders"
+    ),
     project_name: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
     repository_name: Optional[str] = Query("", pattern=r"^[A-z0-9 .\-_%]*$"),
     start_date_time: Optional[datetime] = Query(None),
     end_date_time: Optional[datetime] = Query(None),
-    rule_pack_versions: Optional[List[str]] = Query(None, alias="rule_pack_version", title="RulePackVersion"),
+    rule_pack_versions: Optional[List[str]] = Query(
+        None, alias="rule_pack_version", title="RulePackVersion"
+    ),
     db_connection: Session = Depends(get_db_connection),
 ) -> List[str]:
     """
         Retrieve all uniquely detected rules across all findings in the database
 
     - **db_connection**: Session of the database connection
     - **finding_statuses**: Optional, filter on supported finding statuses
@@ -90,15 +98,17 @@
         200: {"description": "Retrieve all the detected rules with counts per status"},
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 @cache(namespace=CACHE_NAMESPACE_FINDING, expire=REDIS_CACHE_EXPIRE)
 def get_rules_finding_status_count(
-    rule_pack_versions: Optional[List[str]] = Query(None, alias="rule_pack_version", title="RulePackVersion"),
+    rule_pack_versions: Optional[List[str]] = Query(
+        None, alias="rule_pack_version", title="RulePackVersion"
+    ),
     rule_tags: Optional[List[str]] = Query(None, alias="rule_tag", title="RuleTag"),
     db_connection: Session = Depends(get_db_connection),
 ) -> List[RuleFindingCountModel]:
     """
         Retrieve all detected rules with finding counts per supported status
 
     - **rule_pack_version**: Optional, filter on rule pack version
@@ -112,24 +122,32 @@
     rule_findings_counts = []
 
     for rule_name, rule_counts in rule_finding_counts.items():
         rule_finding_count = RuleFindingCountModel(
             rule_name=rule_name, finding_count=rule_counts["total_findings_count"]
         )
         rule_finding_count.finding_statuses_count.append(
-            StatusCount(status=FindingStatus.TRUE_POSITIVE.value, count=rule_counts["true_positive"])
+            StatusCount(
+                status=FindingStatus.TRUE_POSITIVE.value, count=rule_counts["true_positive"]
+            )
         )
         rule_finding_count.finding_statuses_count.append(
-            StatusCount(status=FindingStatus.FALSE_POSITIVE.value, count=rule_counts["false_positive"])
+            StatusCount(
+                status=FindingStatus.FALSE_POSITIVE.value, count=rule_counts["false_positive"]
+            )
         )
         rule_finding_count.finding_statuses_count.append(
-            StatusCount(status=FindingStatus.NOT_ANALYZED.value, count=rule_counts["not_analyzed"])
+            StatusCount(
+                status=FindingStatus.NOT_ANALYZED.value, count=rule_counts["not_analyzed"]
+            )
         )
         rule_finding_count.finding_statuses_count.append(
-            StatusCount(status=FindingStatus.UNDER_REVIEW.value, count=rule_counts["under_review"])
+            StatusCount(
+                status=FindingStatus.UNDER_REVIEW.value, count=rule_counts["under_review"]
+            )
         )
         rule_finding_count.finding_statuses_count.append(
             StatusCount(
                 status=FindingStatus.CLARIFICATION_REQUIRED.value,
                 count=rule_counts["clarification_required"],
             )
         )
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,52 +63,62 @@
         The output will contain a PaginationModel containing the list of ScanRead type objects,
         or an empty list if no scan was found
     """
     scans = scan_crud.get_scans(db_connection, skip=skip, limit=limit)
 
     total_scans = scan_crud.get_scans_count(db_connection)
 
-    return PaginationModel[scan_schema.ScanRead](data=scans, total=total_scans, limit=limit, skip=skip)
+    return PaginationModel[scan_schema.ScanRead](
+        data=scans, total=total_scans, limit=limit, skip=skip
+    )
 
 
 @router.post(
     "",
     response_model=scan_schema.ScanRead,
     summary="Create a scan",
     status_code=status.HTTP_201_CREATED,
     responses={
         201: {"description": "Create a new scan"},
         400: {"model": Model400, "description": "Error creating a new scan"},
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
-def create_scan(scan: scan_schema.ScanCreate, db_connection: Session = Depends(get_db_connection)):
+def create_scan(
+    scan: scan_schema.ScanCreate, db_connection: Session = Depends(get_db_connection)
+):
     """
         Create a scan with all the information
 
     - **db_connection**: Session of the database connection
     - **scan_type**: scan type, supported values are BASE or INCREMENTAL
     - **last_scanned_commit**: last scanned commit hash
     - **timestamp**: creation timestamp
     - **increment_number**: scan increment number
     - **rule_pack**: rule pack version
     - **repository_id**: repository id
     """
     # Determine the increment number if needed and not supplied
-    if scan.scan_type == ScanType.INCREMENTAL and (not scan.increment_number or scan.increment_number <= 0):
-        last_scan = scan_crud.get_latest_scan_for_repository(db_connection, repository_id=scan.repository_id)
+    if scan.scan_type == ScanType.INCREMENTAL and (
+        not scan.increment_number or scan.increment_number <= 0
+    ):
+        last_scan = scan_crud.get_latest_scan_for_repository(
+            db_connection, repository_id=scan.repository_id
+        )
         new_increment = last_scan.increment_number + 1
         scan.increment_number = new_increment
 
     try:
         created_scan = scan_crud.create_scan(db_connection=db_connection, scan=scan)
     except IntegrityError as err:
         logger.debug(f"Error creating new scan object: {err}")
-        raise HTTPException(status_code=400, detail="Error creating new scan object") from err
+        raise HTTPException(
+            status_code=400, detail="Error creating new scan object"
+        ) from err
     return created_scan
 
 
 @router.get(
     "/{scan_id}",
     response_model=scan_schema.ScanRead,
     summary="Fetch a scan by ID",
@@ -161,15 +171,17 @@
     - **rule_pack**: rule pack version
     - **repository_id**: repository id
 
     """
     db_scan = scan_crud.get_scan(db_connection, scan_id=scan_id)
     if db_scan is None:
         raise HTTPException(status_code=404, detail="Scan not found")
-    return scan_crud.update_scan(db_connection=db_connection, scan_id=scan_id, scan=scan)
+    return scan_crud.update_scan(
+        db_connection=db_connection, scan_id=scan_id, scan=scan
+    )
 
 
 @router.delete(
     "/{scan_id}",
     summary="Delete a scan",
     status_code=status.HTTP_200_OK,
     responses={
@@ -201,15 +213,17 @@
 
 @router.post(
     "/{scan_id}" f"{RWS_ROUTE_FINDINGS}",
     response_model=int,
     summary="Create scan findings",
     status_code=status.HTTP_201_CREATED,
     responses={
-        201: {"description": "Create findings and their associated scan_findings for scan <scan_id>"},
+        201: {
+            "description": "Create findings and their associated scan_findings for scan <scan_id>"
+        },
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 async def create_scan_findings(
     scan_id: int,
     findings: List[finding_schema.FindingCreate],
@@ -236,21 +250,25 @@
     - **rule_name**: rule name
     - **repository_id**: repository id of the finding
     - **return**: [FindingRead]
         The output will contain a PaginationModel containing the list of FindingRead type objects,
         or an empty list if no scan was found
     """
 
-    created_findings = finding_crud.create_findings(db_connection=db_connection, findings=findings)
+    created_findings = finding_crud.create_findings(
+        db_connection=db_connection, findings=findings
+    )
     scan_findings = []
     for finding in created_findings:
         scan_finding = DBscanFinding(finding_id=finding.id_, scan_id=scan_id)
         scan_findings.append(scan_finding)
 
-    _ = scan_finding_crud.create_scan_findings(db_connection=db_connection, scan_findings=scan_findings)
+    _ = scan_finding_crud.create_scan_findings(
+        db_connection=db_connection, scan_findings=scan_findings
+    )
 
     # Clear cache related to findings
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_FINDING)
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_RULE)
 
     return len(created_findings)
 
@@ -266,15 +284,17 @@
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 def get_scan_findings(
     scan_id: int,
     skip: int = Query(default=0, ge=0),
     limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-    rules: List[str] = Query([], pattern=r"^[A-z0-9 .\-_%]*$", alias="rule", title="rule"),
+    rules: List[str] = Query(
+        [], pattern=r"^[A-z0-9 .\-_%]*$", alias="rule", title="rule"
+    ),
     statuses: List[FindingStatus] = Query(None, alias="status", title="status"),
     db_connection: Session = Depends(get_db_connection),
 ) -> PaginationModel[finding_schema.FindingRead]:
     """
         Retrieve all finding objects paginated related to a scan_id
 
     - **db_connection**: Session of the database connection
@@ -292,18 +312,24 @@
         scan_ids=[scan_id],
         skip=skip,
         limit=limit,
         rules_filter=rules,
         statuses_filter=statuses,
     )
 
-    findings_filter = FindingsFilter(scan_ids=[scan_id], rule_names=rules, finding_statuses=statuses)
-    total_findings = finding_crud.get_total_findings_count(db_connection, findings_filter=findings_filter)
+    findings_filter = FindingsFilter(
+        scan_ids=[scan_id], rule_names=rules, finding_statuses=statuses
+    )
+    total_findings = finding_crud.get_total_findings_count(
+        db_connection, findings_filter=findings_filter
+    )
 
-    return PaginationModel[finding_schema.FindingRead](data=findings, total=total_findings, limit=limit, skip=skip)
+    return PaginationModel[finding_schema.FindingRead](
+        data=findings, total=total_findings, limit=limit, skip=skip
+    )
 
 
 @router.get(
     f"{RWS_ROUTE_FINDINGS}/",
     response_model=PaginationModel[finding_schema.FindingRead],
     summary="Get scan findings",
     status_code=status.HTTP_200_OK,
@@ -313,15 +339,17 @@
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 def get_scans_findings(
     scan_ids: List[int] = Query([], alias="scan_id", title="Scan ids"),
     skip: int = Query(default=0, ge=0),
     limit: int = Query(default=DEFAULT_RECORDS_PER_PAGE_LIMIT, ge=1),
-    rules: List[str] = Query([], pattern=r"^[A-z0-9 .\-_%]*$", alias="rule", title="rule"),
+    rules: List[str] = Query(
+        [], pattern=r"^[A-z0-9 .\-_%]*$", alias="rule", title="rule"
+    ),
     statuses: List[FindingStatus] = Query(None, alias="status", title="status"),
     db_connection: Session = Depends(get_db_connection),
 ) -> PaginationModel[finding_schema.FindingRead]:
     """
         Retrieve all finding objects paginated related to a scan_id
 
     - **db_connection**: Session of the database connection
@@ -339,27 +367,35 @@
         scan_ids=scan_ids,
         skip=skip,
         limit=limit,
         rules_filter=rules,
         statuses_filter=statuses,
     )
 
-    findings_filter = FindingsFilter(scan_ids=scan_ids, rule_names=rules, finding_statuses=statuses)
-    total_findings = finding_crud.get_total_findings_count(db_connection, findings_filter=findings_filter)
+    findings_filter = FindingsFilter(
+        scan_ids=scan_ids, rule_names=rules, finding_statuses=statuses
+    )
+    total_findings = finding_crud.get_total_findings_count(
+        db_connection, findings_filter=findings_filter
+    )
 
-    return PaginationModel[finding_schema.FindingRead](data=findings, total=total_findings, limit=limit, skip=skip)
+    return PaginationModel[finding_schema.FindingRead](
+        data=findings, total=total_findings, limit=limit, skip=skip
+    )
 
 
 @router.get(
     f"{RWS_ROUTE_DETECTED_RULES}/",
     response_model=List[str],
     summary="Get unique rules from scans",
     status_code=status.HTTP_200_OK,
     responses={
-        200: {"description": "Retrieve all the unique rules associated with specified scans"},
+        200: {
+            "description": "Retrieve all the unique rules associated with specified scans"
+        },
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
 def get_distinct_rules_from_scans(
     scan_ids: List[int] = Query([], alias="scan_id", title="Scan ids"),
     db_connection: Session = Depends(get_db_connection),
@@ -370,11 +406,13 @@
     - **db_connection**: Session of the database connection
     - **scan_ids**: scan ids for which to retrieve the unique rules
     - **return**: List[str]
         The output will contain a list of strings of unique rules for given scan ids
     """
     return_rules = []
     if scan_ids:
-        rules = finding_crud.get_distinct_rules_from_scans(db_connection, scan_ids=scan_ids)
+        rules = finding_crud.get_distinct_rules_from_scans(
+            db_connection, scan_ids=scan_ids
+        )
         for rule in rules:
             return_rules.append(rule.rule_name)
     return return_rules
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,16 +54,20 @@
     """
     try:
         created_vcs_instance = vcs_instance_crud.create_vcs_instance_if_not_exists(
             db_connection=db_connection, vcs_instance=vcs_instance
         )
     except IntegrityError as err:
         logger.debug(f"Error creating new vcs_instance object: {err}")
-        raise HTTPException(status_code=400, detail="Error creating new vcs_instance object") from err
-    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(created_vcs_instance)
+        raise HTTPException(
+            status_code=400, detail="Error creating new vcs_instance object"
+        ) from err
+    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(
+        created_vcs_instance
+    )
 
     # Clear cache related to VCS instances
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_VCS_INSTANCE)
     return vcs_instance
 
 
 @router.get(
@@ -88,18 +92,22 @@
         Retrieve a VCS instance object based on the provided id
 
     - **db_connection**: Session of the database connection
     - **vcs_instance_id**: ID of the VCS instance for which details need to be fetched
     - **return**: VCSInstanceRead
         The output will contain a VCSInstanceRead type object from the requested ID
     """
-    db_vcs_instance = vcs_instance_crud.get_vcs_instance(db_connection, vcs_instance_id=vcs_instance_id)
+    db_vcs_instance = vcs_instance_crud.get_vcs_instance(
+        db_connection, vcs_instance_id=vcs_instance_id
+    )
     if db_vcs_instance is None:
         raise HTTPException(status_code=404, detail="VCS Instance not found")
-    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(db_vcs_instance)
+    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(
+        db_vcs_instance
+    )
     return vcs_instance
 
 
 @router.get(
     "",
     response_model=PaginationModel[vcs_instance_schema.VCSInstanceRead],
     summary="Get all VCS instances",
@@ -134,15 +142,19 @@
         skip=skip,
         limit=limit,
         vcs_provider_type=vcs_provider_type,
         vcs_instance_name=vcs_instance_name,
     )
     vcs_instances = []
     for db_vcs_instance in db_vcs_instances:
-        vcs_instances.append(vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(db_vcs_instance))
+        vcs_instances.append(
+            vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(
+                db_vcs_instance
+            )
+        )
 
     total_vcs_instances = vcs_instance_crud.get_vcs_instances_count(
         db_connection,
         vcs_provider_type=vcs_provider_type,
         vcs_instance_name=vcs_instance_name,
     )
 
@@ -182,23 +194,27 @@
     - **scheme**: Scheme of the VCS instance that needs to be updated. Allowed values http or https
     - **exceptions**: List of projects which needs to be updated to exception list, default empty list
     - **scope**: List of projects which needs to be updated to scope
     - **organization**: Name of organization to be updated, default is empty
     - **return**: VCSInstanceRead
         The output will contain a VCSInstanceRead type object with the new properties
     """
-    db_vcs_instance = vcs_instance_crud.get_vcs_instance(db_connection, vcs_instance_id=vcs_instance_id)
+    db_vcs_instance = vcs_instance_crud.get_vcs_instance(
+        db_connection, vcs_instance_id=vcs_instance_id
+    )
     if db_vcs_instance is None:
         raise HTTPException(status_code=404, detail="VCS instance not found")
     db_vcs_instance = vcs_instance_crud.update_vcs_instance(
         db_connection=db_connection,
         vcs_instance_id=vcs_instance_id,
         vcs_instance=vcs_instance,
     )
-    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(db_vcs_instance)
+    vcs_instance = vcs_instance_schema.VCSInstanceRead.create_from_db_vcs_instance(
+        db_vcs_instance
+    )
 
     # Clear cache related to VCS instances
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_VCS_INSTANCE)
     return vcs_instance
 
 
 @router.delete(
@@ -211,23 +227,29 @@
             "model": Model404,
             "description": "VCS Instance <vcs_instance_id> not found",
         },
         500: {"description": ERROR_MESSAGE_500},
         503: {"description": ERROR_MESSAGE_503},
     },
 )
-async def delete_vcs_instance(vcs_instance_id: int, db_connection: Session = Depends(get_db_connection)):
+async def delete_vcs_instance(
+    vcs_instance_id: int, db_connection: Session = Depends(get_db_connection)
+):
     """
         Delete a VCS instance by ID
 
     - **db_connection**: Session of the database connection
     - **vcs_instance_id**: ID of the VCS instance to delete
     - **return**: The output will contain a success or error message based on the success of the deletion
     """
-    db_vcs_instance = vcs_instance_crud.get_vcs_instance(db_connection, vcs_instance_id=vcs_instance_id)
+    db_vcs_instance = vcs_instance_crud.get_vcs_instance(
+        db_connection, vcs_instance_id=vcs_instance_id
+    )
     if db_vcs_instance is None:
         raise HTTPException(status_code=404, detail="VCS instance not found")
-    vcs_instance_crud.delete_vcs_instance(db_connection, vcs_instance_id=vcs_instance_id, delete_related=True)
+    vcs_instance_crud.delete_vcs_instance(
+        db_connection, vcs_instance_id=vcs_instance_id, delete_related=True
+    )
 
     # Clear cache related to VCS instances
     await CacheManager.clear_cache_by_namespace(namespace=CACHE_NAMESPACE_VCS_INSTANCE)
     return {"ok": True}
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/filters.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,10 +26,12 @@
     rule_pack_versions: List[str] = None
 
     @validator("end_date_time")
     @classmethod
     def date_range_check(cls, end_date_time: datetime, values: dict):
         if end_date_time and values["start_date_time"]:
             if values["start_date_time"] >= end_date_time:
-                raise ValueError("the start of the date range needs to be prior to the end of it.")
+                raise ValueError(
+                    "the start of the date range needs to be prior to the end of it."
+                )
 
         return end_date_time
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 # First Party
 from resc_backend.constants import ERROR_MESSAGE_500, ERROR_MESSAGE_503
 
 
 def add_exception_handlers(app: FastAPI):
     @app.exception_handler(RequestValidationError)
-    async def validation_exception_handler(request: Request, exc: RequestValidationError):
+    async def validation_exception_handler(
+        request: Request, exc: RequestValidationError
+    ):
         log_warning(request, exc, "422 Unprocessable Entity")
         return JSONResponse(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             content=jsonable_encoder({"detail": exc.errors(), "body": exc.body}),
         )
 
     @app.exception_handler(ValueError)
@@ -36,15 +38,17 @@
         log_error(request, exc, "500 Internal Server Error")
         return JSONResponse(
             status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
             content={"detail": ERROR_MESSAGE_500},
         )
 
     @app.exception_handler(OperationalError)
-    async def service_unavailable_exception_handler(request: Request, exc: OperationalError):
+    async def service_unavailable_exception_handler(
+        request: Request, exc: OperationalError
+    ):
         log_error(request, exc, "503 Service Unavailable")
         return JSONResponse(
             status_code=status.HTTP_503_SERVICE_UNAVAILABLE,
             content={"detail": ERROR_MESSAGE_503},
         )
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 
 class Model409(RescResponseModel):
     """
     Response schema to be used for a 409 CONFLICT.
     """
 
     class Config:
-        schema_extra = {"example": {"detail": "Unable to process entity due to conflict"}}
+        schema_extra = {
+            "example": {"detail": "Unable to process entity due to conflict"}
+        }
 
 
 class Model422(RescResponseModel):
     """
     Response schema to be used for a 422 UNPROCESSABLE ENTITY.
     """
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,17 @@
         TOML rule dictionary
     :return: RuleAllowList
         The output will contain an object of RuleAllowList
     """
     global_allow_list_obj = None
     if "allowlist" in toml_rule_dictionary:
         global_allow_list = toml_rule_dictionary.get("allowlist")
-        global_allow_list_obj = map_dictionary_to_rule_allow_list_object(global_allow_list)
+        global_allow_list_obj = map_dictionary_to_rule_allow_list_object(
+            global_allow_list
+        )
     else:
         logger.info("No global allow list is present in the toml file!")
     return global_allow_list_obj
 
 
 def map_dictionary_to_rule_allow_list_object(
     allow_list_dictionary: dict,
@@ -146,15 +148,19 @@
     :param allow_list_dictionary:
         AllowList dictionary
     :return: RuleAllowList
         The output will contain an object of RuleAllowList
     """
     rule_allow_list = None
     if allow_list_dictionary:
-        description = allow_list_dictionary["description"] if "description" in allow_list_dictionary else None
+        description = (
+            allow_list_dictionary["description"]
+            if "description" in allow_list_dictionary
+            else None
+        )
         regexes = None
         paths = None
         commits = None
         stopwords = None
 
         if "regexes" in allow_list_dictionary:
             regexes = ""
@@ -200,32 +206,38 @@
     :return: toml_file
         Returns toml file
     """
     doc = document()
     doc.add(comment("This is a gitleaks configuration file."))
     doc.add(comment("Rules and allowlists are defined within this file."))
     doc.add(comment("Rules instruct gitleaks on what should be considered a secret."))
-    doc.add(comment("Allowlists instruct gitleaks on what is allowed, i.e. not a secret."))
+    doc.add(
+        comment("Allowlists instruct gitleaks on what is allowed, i.e. not a secret.")
+    )
     doc.add(nl())
 
     if "title" in parsed_toml_dictionary:
         doc.add("title", parsed_toml_dictionary["title"])
     doc.add(nl())
     if "version" in parsed_toml_dictionary:
         doc.add("version", parsed_toml_dictionary["version"])
     doc.add(nl())
 
     # Global allow list table
-    global_allow_list_table = create_allow_list_toml_table(input_dictionary=parsed_toml_dictionary, key="allowlist")
+    global_allow_list_table = create_allow_list_toml_table(
+        input_dictionary=parsed_toml_dictionary, key="allowlist"
+    )
     if global_allow_list_table:
         doc.add("allowlist", global_allow_list_table)
         doc.add(nl())
 
     # Rules table
-    rule_array_table = create_rule_array_toml_table(rule_dictionary=parsed_toml_dictionary)
+    rule_array_table = create_rule_array_toml_table(
+        rule_dictionary=parsed_toml_dictionary
+    )
     doc.add("rules", rule_array_table)
 
     toml_string = tomlkit.dumps(doc)
     with open(TEMP_RULE_FILE, "w", encoding="utf-8") as toml_file:
         toml_file.write(toml_string)
         toml_file.close()
     return toml_file
@@ -325,17 +337,21 @@
             if "description" in rule_dict:
                 rule_table.add("description", rule_dict["description"])
             if "entropy" in rule_dict:
                 rule_table.add("entropy", rule_dict["entropy"])
             if "secret_group" in rule_dict:
                 rule_table.add("secretGroup", rule_dict["secret_group"])
             if "regex" in rule_dict:
-                rule_table.add("regex", String.from_raw(rule_dict["regex"], StringType.MLL))
+                rule_table.add(
+                    "regex", String.from_raw(rule_dict["regex"], StringType.MLL)
+                )
             if "path" in rule_dict:
-                rule_table.add("path", String.from_raw(rule_dict["path"], StringType.MLL))
+                rule_table.add(
+                    "path", String.from_raw(rule_dict["path"], StringType.MLL)
+                )
             if "tags" in rule_dict:
                 multiline_tag_array = get_multiline_array_for_toml_file(
                     input_dictionary=rule_dict,
                     key="tags",
                     string_type=StringType.SLB,
                     delimiter=",",
                 )
@@ -347,15 +363,17 @@
                     string_type=StringType.SLB,
                     delimiter=",",
                 )
                 rule_table.add("keywords", multiline_keyword_array)
 
             # Rule Allow List Table
             if "allow_list" in rule_dict:
-                allow_list_table = create_allow_list_toml_table(input_dictionary=rule_dict, key="allow_list")
+                allow_list_table = create_allow_list_toml_table(
+                    input_dictionary=rule_dict, key="allow_list"
+                )
                 rule_table.append("allowlist", allow_list_table)
 
             rule_array_table.append(rule_table)
     return rule_array_table
 
 
 def validate_uploaded_file_and_read_content(rule_file: File) -> str:
@@ -367,25 +385,32 @@
         Return file content
     """
     file_name = os.path.splitext(rule_file.filename)[0]
 
     # File name validation
     is_valid_file_name = bool(re.match(FILE_NAME_REGEX, file_name))
     if not is_valid_file_name:
-        raise HTTPException(500, detail=f"Invalid characters in File name - {file_name}")
+        raise HTTPException(
+            500, detail=f"Invalid characters in File name - {file_name}"
+        )
 
     # File name max length validation
     if len(file_name) > 255:
-        raise HTTPException(500, detail="File name value exceeds maximum length of 255 characters")
+        raise HTTPException(
+            500, detail="File name value exceeds maximum length of 255 characters"
+        )
 
     # File extension validation
-    if rule_file.content_type != "application/octet-stream" or not rule_file.filename.lower().endswith(
-        ALLOWED_EXTENSION
+    if (
+        rule_file.content_type != "application/octet-stream"
+        or not rule_file.filename.lower().endswith(ALLOWED_EXTENSION)
     ):
-        raise HTTPException(500, detail="Invalid document type, only TOML file is supported")
+        raise HTTPException(
+            500, detail="Invalid document type, only TOML file is supported"
+        )
 
     # File size validation
     max_size: int = 1000000
     content = rule_file.file.read()
     file_size = len(content)
     if file_size > max_size:
         raise HTTPException(500, detail="File size exceeds the maximum limit 1 MB")
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/audit.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,31 @@
     ) -> str:
         arr = repository_url.split("/")
         if len(arr) >= 3:
             repo_base_url = arr[0] + "//" + arr[2]
         else:
             repo_base_url = repository_url
         bitbucket_commit_url = (
-            f"{repo_base_url}/projects/{project_key}/repos/" f"{repository_name}/browse/{file_path}?at={commit_id}"
+            f"{repo_base_url}/projects/{project_key}/repos/"
+            f"{repository_name}/browse/{file_path}?at={commit_id}"
         )
         commit_url = bitbucket_commit_url
         return commit_url
 
     @staticmethod
-    def build_ado_commit_url(repository_url: str, file_path: str, commit_id: str) -> str:
+    def build_ado_commit_url(
+        repository_url: str, file_path: str, commit_id: str
+    ) -> str:
         ado_commit_url = f"{repository_url}/commit/{commit_id}?path=/{file_path}"
         return ado_commit_url
 
     @staticmethod
-    def build_github_commit_url(repository_url: str, file_path: str, commit_id: str) -> str:
+    def build_github_commit_url(
+        repository_url: str, file_path: str, commit_id: str
+    ) -> str:
         github_commit_url = f"{repository_url}/commit/{commit_id}?path=/{file_path}"
         return github_commit_url
 
     @root_validator
     def build_commit_url(cls, values) -> Dict:
         if values["status"] is None:
             values["status"] = FindingStatus.NOT_ANALYZED.value
@@ -95,12 +100,14 @@
         elif values["vcs_provider"] == VCSProviders.GITHUB_PUBLIC:
             values["commit_url"] = cls.build_github_commit_url(
                 repository_url=values["repository_url"],
                 file_path=values["file_path"],
                 commit_id=values["commit_id"],
             )
         else:
-            raise NotImplementedError(f"Unsupported VCSProvider: {values['vcs_provider']}")
+            raise NotImplementedError(
+                f"Unsupported VCSProvider: {values['vcs_provider']}"
+            )
         return values
 
     class Config:
         orm_mode = True
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/repository.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/repository_enriched.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/repository_enriched.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 
 class RuleCreate(RuleBase):
     rule_pack: constr(regex=r"^(\d+\.)?(\d+\.)?(\*|\d+)$")
     allow_list: Optional[conint(gt=0)] = None
 
     @classmethod
-    def create_from_base_class(cls, base_object: RuleBase, rule_pack: str, allow_list=int):
+    def create_from_base_class(
+        cls, base_object: RuleBase, rule_pack: str, allow_list=int
+    ):
         return cls(**(dict(base_object)), rule_pack=rule_pack, allow_list=allow_list)
 
 
 class Rule(RuleBase):
     pass
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,30 +20,35 @@
     organization: Optional[constr(max_length=200)]
 
     @validator("scheme", pre=True)
     @classmethod
     def check_scheme(cls, value):
         allowed_schemes = ["http", "https"]
         if value not in allowed_schemes:
-            raise ValueError(f"The scheme '{value}' must be one of the following {', '.join(allowed_schemes)}")
+            raise ValueError(
+                f"The scheme '{value}' must be one of the following {', '.join(allowed_schemes)}"
+            )
         return value
 
     @validator("organization", pre=True)
     @classmethod
     def check_organization(cls, value, values):
         if not value and values.get("provider_type", None) == AZURE_DEVOPS:
-            raise ValueError("The organization field needs to be specified for Azure devops vcs instances")
+            raise ValueError(
+                "The organization field needs to be specified for Azure devops vcs instances"
+            )
         return value
 
     @validator("scope", pre=True)
     @classmethod
     def check_scope_and_exceptions(cls, value, values):
         if value and values.get("exceptions", None):
             raise ValueError(
-                "You cannot specify bot the scope and exceptions to the scan, only one setting" " is supported."
+                "You cannot specify bot the scope and exceptions to the scan, only one setting"
+                " is supported."
             )
         return value
 
 
 class VCSInstanceCreate(VCSInstanceBase):
     pass
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,20 +20,28 @@
 def create_findings(url: str, findings: List[FindingCreate]) -> requests.Response:
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_FINDINGS}"
 
     findings_json = []
     for finding in findings:
         findings_json.append(json.loads(finding.json()))
 
-    response = requests.post(api_url, json=findings_json, proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.post(
+        api_url, json=findings_json, proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
 
 
-def create_findings_with_scan_id(url: str, findings: List[FindingCreate], scan_id: int) -> requests.Response:
-    api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_SCANS}/{scan_id}{RWS_ROUTE_FINDINGS}"
+def create_findings_with_scan_id(
+    url: str, findings: List[FindingCreate], scan_id: int
+) -> requests.Response:
+    api_url = (
+        f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_SCANS}/{scan_id}{RWS_ROUTE_FINDINGS}"
+    )
 
     findings_json = []
     for finding in findings:
         findings_json.append(json.loads(finding.json()))
 
-    response = requests.post(api_url, json=findings_json, proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.post(
+        api_url, json=findings_json, proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/repositories.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/repositories.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from resc_backend.resc_web_service.schema.repository import Repository
 
 logger = logging.getLogger(__name__)
 
 
 def create_repository(url: str, repository: Repository):
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_REPOSITORIES}"
-    response = requests.post(api_url, data=repository.json(), proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.post(
+        api_url, data=repository.json(), proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
 
 
 def get_last_scan_for_repository(url: str, repository_id: int):
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_REPOSITORIES}/{repository_id}{RWS_ROUTE_LAST_SCAN}"
     response = requests.get(api_url, proxies={"http": "", "https": ""}, timeout=10)
     return response
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,31 +21,37 @@
         files = {
             "rule_file": (
                 "RESC-SECRETS-RULE.toml",
                 toml_file,
                 "application/octet-stream",
             )
         }
-        response = requests.post(url=url, files=files, proxies={"http": "", "https": ""}, timeout=10)
+        response = requests.post(
+            url=url, files=files, proxies={"http": "", "https": ""}, timeout=10
+        )
         toml_file.close()
     return response
 
 
-def download_rule_pack_toml_file(rws_url: str, rule_pack_version: Optional[str] = "") -> Response:
+def download_rule_pack_toml_file(
+    rws_url: str, rule_pack_version: Optional[str] = ""
+) -> Response:
     params = {}
     if rule_pack_version:
         params = {"rule_pack_version": rule_pack_version}
     response = requests.get(
         url=f"{rws_url}{RWS_VERSION_PREFIX}{RWS_ROUTE_RULE_PACKS}",
         params=params,
         timeout=10,
     )
 
     if response.status_code == 200:
-        logger.debug(f"Rule pack version: {rule_pack_version} has been successfully downloaded")
+        logger.debug(
+            f"Rule pack version: {rule_pack_version} has been successfully downloaded"
+        )
     else:
         logger.error(
             f"Downloading rule pack version {rule_pack_version} failed with "
             f"error: {response.status_code}->{response.text}"
         )
     return response
 
@@ -57,9 +63,11 @@
     skip: Optional[int] = 0,
     limit: Optional[int] = DEFAULT_RECORDS_PER_PAGE_LIMIT,
 ):
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_RULE_PACKS}/versions"
     params = {"active": active, "skip": skip, "limit": limit}
     if version:
         params["version"] = version
-    response = requests.get(api_url, params=params, proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.get(
+        api_url, params=params, proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
```

### Comparing `resc_backend-3.1.2/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-4.0.0/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,9 +9,11 @@
 from resc_backend.resc_web_service.schema.vcs_instance import VCSInstanceCreate
 
 logger = logging.getLogger(__name__)
 
 
 def create_vcs_instance(url: str, vcs_instance: VCSInstanceCreate):
     api_url = f"{url}{RWS_VERSION_PREFIX}{RWS_ROUTE_VCS}"
-    response = requests.post(api_url, data=vcs_instance.json(), proxies={"http": "", "https": ""}, timeout=10)
+    response = requests.post(
+        api_url, data=vcs_instance.json(), proxies={"http": "", "https": ""}, timeout=10
+    )
     return response
```

### Comparing `resc_backend-3.1.2/src/resc_backend.egg-info/PKG-INFO` & `resc_backend-4.0.0/src/resc_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 3.1.2
+Version: 4.0.0
 Summary: Repository Scanner - Backend
-Home-page: https://github.com/abnamro/resc-backend
+Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: celery==5.3.1
@@ -19,15 +19,15 @@
 Requires-Dist: pydantic==1.10.15
 Requires-Dist: uvicorn==0.17.6
 Requires-Dist: waitress==2.1.2
 Requires-Dist: pyjwt[crypto]==2.8.0
 Requires-Dist: cryptography==42.0.4
 Requires-Dist: tenacity==8.2.2
 Requires-Dist: tomlkit==0.12.1
-Requires-Dist: python-multipart==0.0.9
+Requires-Dist: python-multipart==0.0.7
 Requires-Dist: aiofiles==0.8.0
 Requires-Dist: packaging==23.1
 Requires-Dist: fastapi-cache2==0.2.1
 Requires-Dist: redis==4.6.0
 Requires-Dist: azure-identity==1.15.0
 Requires-Dist: setuptools==69.5.1
```

### Comparing `resc_backend-3.1.2/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-4.0.0/src/resc_backend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE.md
 README.md
-pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 src/resc_backend/__init__.py
 src/resc_backend/common.py
 src/resc_backend/constants.py
 src/resc_backend.egg-info/PKG-INFO
```

