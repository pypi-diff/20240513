# Comparing `tmp/consoleme-1.3.0.tar.gz` & `tmp/consoleme-1.3.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consoleme-1.3.0.tar", last modified: Thu Jul 21 14:27:25 2022, max compression
+gzip compressed data, was "consoleme-1.3.1.dev3.tar", last modified: Mon May 13 17:19:53 2024, max compression
```

## Comparing `consoleme-1.3.0.tar` & `consoleme-1.3.1.dev3.tar`

### file list

```diff
@@ -1,302 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.884013 consoleme-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11343 2022-07-21 14:25:13.000000 consoleme-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-07-21 14:25:13.000000 consoleme-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-07-21 14:27:25.884013 consoleme-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-07-21 14:25:13.000000 consoleme-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.832012 consoleme-1.3.0/cdk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.832012 consoleme-1.3.0/cdk/consoleme_ecs_cdk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.832012 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/consoleme_ecs_service_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/consoleme_spoke_accounts_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/alb_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     4343 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/auth_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/cache_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     6887 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/compute_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     7345 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/config_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     3595 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/db_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     3748 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/domain_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     8910 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/iam_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/shared_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/vpc_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/consoleme_ecs_cdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/cdk/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-07-21 14:25:13.000000 consoleme-1.3.0/cdk/tests/test_cdk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/babel.config.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/celery_tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/celery_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    86894 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/celery_tasks/celery_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14652 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/default_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/default_plugins/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/default_plugins/plugins/auth/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12702 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/default_plugins/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27051 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/aws/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/default_plugins/plugins/celery_tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/celery_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/celery_tasks/celery_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/default_plugins/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/default_plugins/plugins/group_mapping/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/group_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7028 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/group_mapping/group_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme/default_plugins/plugins/internal_routes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/internal_routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.840012 consoleme-1.3.0/consoleme/default_plugins/plugins/internal_routes/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/internal_routes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/internal_routes/handlers/internal_demo_route.py
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/internal_routes/internal_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.840012 consoleme-1.3.0/consoleme/default_plugins/plugins/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/metrics/base_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.840012 consoleme-1.3.0/consoleme/default_plugins/plugins/metrics/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/metrics/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/metrics/default_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.840012 consoleme-1.3.0/consoleme/default_plugins/plugins/policies/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/plugins/policies/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/default_plugins/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.840012 consoleme-1.3.0/consoleme/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10377 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.840012 consoleme-1.3.0/consoleme/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    26952 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.840012 consoleme-1.3.0/consoleme/handlers/v1/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23260 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v1/credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v1/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v1/health.py
--rw-r--r--   0 runner    (1001) docker     (121)    11978 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v1/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v1/roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     3203 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v1/saml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.844012 consoleme-1.3.0/consoleme/handlers/v2/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/audit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5260 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/aws_iam_users.py
--rw-r--r--   0 runner    (1001) docker     (121)    13422 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/challenge.py
--rw-r--r--   0 runner    (1001) docker     (121)     4946 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/dynamic_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/generate_changes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/generate_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5986 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/logout.py
--rw-r--r--   0 runner    (1001) docker     (121)     6005 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/managed_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     5944 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     6804 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    33629 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)     8644 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)    25989 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/self_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/service_control_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/templated_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     6164 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/typeahead.py
--rw-r--r--   0 runner    (1001) docker     (121)    13172 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     5046 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/handlers/v2/user_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.848013 consoleme-1.3.0/consoleme/lib/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.848013 consoleme-1.3.0/consoleme/lib/account_indexers/
--rw-r--r--   0 runner    (1001) docker     (121)     4980 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/account_indexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9554 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/account_indexers/aws_organizations.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/account_indexers/current_account.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/account_indexers/local_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/account_indexers/swag.py
--rw-r--r--   0 runner    (1001) docker     (121)     6453 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/alb_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)    11566 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    81605 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.848013 consoleme-1.3.0/consoleme/lib/aws_config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/aws_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4204 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/aws_config/aws_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/aws_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     8548 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/challenge.py
--rw-r--r--   0 runner    (1001) docker     (121)    18225 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/change_request.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.848013 consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/
--rw-r--r--   0 runner    (1001) docker     (121)    11918 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/dynamic_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/internal_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3833 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/role_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)    10464 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/cookie-py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/credential_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)    13539 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/duo.py
--rw-r--r--   0 runner    (1001) docker     (121)    49019 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.848013 consoleme-1.3.0/consoleme/lib/event_bridge/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/event_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9914 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/event_bridge/access_denies.py
--rw-r--r--   0 runner    (1001) docker     (121)     4277 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/event_bridge/role_updates.py
--rw-r--r--   0 runner    (1001) docker     (121)    11368 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/git.py
--rw-r--r--   0 runner    (1001) docker     (121)    22017 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/google.py
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/handler_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.848013 consoleme-1.3.0/consoleme/lib/notifications/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4139 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    12720 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/oidc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/password.py
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)    35445 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (121)    15893 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)     9202 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.852012 consoleme-1.3.0/consoleme/lib/role_updater/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/role_updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/role_updater/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6381 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/role_updater/handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/role_updater/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     7559 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/s3_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3832 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/saml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.852012 consoleme-1.3.0/consoleme/lib/scm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/scm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.852012 consoleme-1.3.0/consoleme/lib/scm/git/
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/scm/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/scm/git/bitbucket.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.852012 consoleme-1.3.0/consoleme/lib/self_service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/self_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/self_service/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6221 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/self_service/typeahead.py
--rw-r--r--   0 runner    (1001) docker     (121)    13702 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/ses.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/singleton.py
--rw-r--r--   0 runner    (1001) docker     (121)     4820 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.852012 consoleme-1.3.0/consoleme/lib/templated_resources/
--rw-r--r--   0 runner    (1001) docker     (121)     9330 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/templated_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/templated_resources/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8861 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/templated_resources/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/timeout.py
--rw-r--r--   0 runner    (1001) docker     (121)     6710 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.852012 consoleme-1.3.0/consoleme/lib/v2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9280 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/v2/aws_principals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/v2/notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)   121179 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/v2/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/v2/user_profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/web.py
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/lib/yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)    26089 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9064 2022-07-21 14:25:13.000000 consoleme-1.3.0/consoleme/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.852012 consoleme-1.3.0/consoleme/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)    15086 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.832012 consoleme-1.3.0/consoleme/templates/images/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.852012 consoleme-1.3.0/consoleme/templates/images/logos/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.856013 consoleme-1.3.0/consoleme/templates/images/logos/infrasec/
--rw-r--r--   0 runner    (1001) docker     (121)  1780372 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/infrasec/DifferentGradient.png
--rw-r--r--   0 runner    (1001) docker     (121)   784262 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/infrasec/Honeybee.png
--rw-r--r--   0 runner    (1001) docker     (121)  1401997 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/infrasec/MikeCloudNoGradientWithFace.png
--rw-r--r--   0 runner    (1001) docker     (121)    32211 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/logo192.png
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/netflix-security-dark-bg-tight.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.860013 consoleme-1.3.0/consoleme/templates/images/logos/nosunglasses/
--rw-r--r--   0 runner    (1001) docker     (121)   353657 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/nosunglasses/1.png
--rw-r--r--   0 runner    (1001) docker     (121)   230322 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/nosunglasses/2.png
--rw-r--r--   0 runner    (1001) docker     (121)   243749 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/nosunglasses/3.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.860013 consoleme-1.3.0/consoleme/templates/images/logos/quarantine/
--rw-r--r--   0 runner    (1001) docker     (121)   374928 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/quarantine/1.png
--rw-r--r--   0 runner    (1001) docker     (121)   387350 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/quarantine/2.png
--rw-r--r--   0 runner    (1001) docker     (121)   359457 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/quarantine/3.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.860013 consoleme-1.3.0/consoleme/templates/images/logos/sunglasses/
--rw-r--r--   0 runner    (1001) docker     (121)   375501 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/sunglasses/1.png
--rw-r--r--   0 runner    (1001) docker     (121)   347136 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/sunglasses/2.png
--rw-r--r--   0 runner    (1001) docker     (121)   362390 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/images/logos/sunglasses/3.png
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-07-21 14:26:14.000000 consoleme-1.3.0/consoleme/templates/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.832012 consoleme-1.3.0/consoleme/templates/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.864013 consoleme-1.3.0/consoleme/templates/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)   609522 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/css/main.463a8800.css
--rw-r--r--   0 runner    (1001) docker     (121)   904718 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/css/main.463a8800.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.868013 consoleme-1.3.0/consoleme/templates/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)  2669634 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/js/main.903555c6.js
--rw-r--r--   0 runner    (1001) docker     (121)    68532 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/js/main.903555c6.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)  8284688 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/js/main.903555c6.js.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.884013 consoleme-1.3.0/consoleme/templates/static/media/
--rw-r--r--   0 runner    (1001) docker     (121)    54488 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/brand-icons.278156e41e0ad908cf7f.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    98404 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/brand-icons.65a2fb6d9aaa164b41a0.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   507628 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/brand-icons.6729d29753e000c17489.svg
--rw-r--r--   0 runner    (1001) docker     (121)    63728 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/brand-icons.cac87dc00c87a5d74711.woff
--rw-r--r--   0 runner    (1001) docker     (121)    98640 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/brand-icons.d68fa3e67dbb653a13ce.eot
--rw-r--r--   0 runner    (1001) docker     (121)    28123 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/flags.99f63ae7a743f21ab308.png
--rw-r--r--   0 runner    (1001) docker     (121)    40148 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/icons.38c6d8bab26db77d8c80.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    50524 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/icons.425399f81e4ce7cbd967.woff
--rw-r--r--   0 runner    (1001) docker     (121)   390837 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/icons.62d9dae4e0040e81c980.svg
--rw-r--r--   0 runner    (1001) docker     (121)   106004 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/icons.a01e3f2d6c83dc3aee17.eot
--rw-r--r--   0 runner    (1001) docker     (121)   105784 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/icons.c656b8caa454ed19b9a2.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    30928 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/outline-icons.5367103510b27b784827.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    12240 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/outline-icons.687a4990ea22bb1a49d4.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    31156 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/outline-icons.752905fa5edf21fc52a1.eot
--rw-r--r--   0 runner    (1001) docker     (121)   107201 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/outline-icons.9c4845b4b41ef40a22fa.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14712 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/outline-icons.ddae9b1ba9b0b42f5880.woff
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/stepper1Active.9866ff3a1ea1cc7a93fa.svg
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/stepper1Complete.6222088c914dcaffd0e4.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/stepper2Active.b5befeb514c5ec2f9815.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/stepper2Complete.47bfe6ee0ee7b0da663a.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/stepper2Pending.3aac534f4c215708e3eb.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/stepper3Active.45f15c88d73d2a09105e.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/stepper3Pending.b72269cdc74f6782c021.svg
--rw-r--r--   0 runner    (1001) docker     (121)    15246 2022-07-21 14:27:14.000000 consoleme-1.3.0/consoleme/templates/static/media/warning.5b4ee25d2b57cd9f461e.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.836012 consoleme-1.3.0/consoleme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-07-21 14:27:25.000000 consoleme-1.3.0/consoleme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10219 2022-07-21 14:27:25.000000 consoleme-1.3.0/consoleme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 14:27:25.000000 consoleme-1.3.0/consoleme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-07-21 14:27:25.000000 consoleme-1.3.0/consoleme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 14:27:25.000000 consoleme-1.3.0/consoleme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-07-21 14:27:25.000000 consoleme-1.3.0/consoleme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-21 14:27:25.000000 consoleme-1.3.0/consoleme.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.884013 consoleme-1.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8776 2022-07-21 14:25:13.000000 consoleme-1.3.0/scripts/initialize_dynamodb_oss.py
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-07-21 14:25:13.000000 consoleme-1.3.0/scripts/initialize_redis_oss.py
--rw-r--r--   0 runner    (1001) docker     (121)     3158 2022-07-21 14:25:13.000000 consoleme-1.3.0/scripts/retrieve_or_decode_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-21 14:27:25.884013 consoleme-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-07-21 14:25:13.000000 consoleme-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.832012 consoleme-1.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.884013 consoleme-1.3.0/tests/celery/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7785 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/celery/test_celery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.884013 consoleme-1.3.0/tests/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/test_accessui.py
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/test_role_login_api.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 14:27:25.884013 consoleme-1.3.0/tests/handlers/v2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4912 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/test_aws_iam_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    25135 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/test_generate_changes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    38224 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)    14007 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     8553 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/test_typeahead.py
--rw-r--r--   0 runner    (1001) docker     (121)    10131 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/test_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-07-21 14:25:13.000000 consoleme-1.3.0/tests/handlers/v2/test_user_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.301189 consoleme-1.3.1.dev3/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.301189 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.301189 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/consoleme_ecs_service_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/consoleme_spoke_accounts_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.305189 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/alb_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/auth_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/cache_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/compute_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/config_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/db_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/domain_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/iam_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/shared_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/vpc_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.305189 consoleme-1.3.1.dev3/cdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/tests/test_cdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.305189 consoleme-1.3.1.dev3/consoleme/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/babel.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/celery_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/celery_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86894 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/celery_tasks/celery_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27051 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/aws/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/celery_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/celery_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/celery_tasks/celery_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/group_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/group_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/group_mapping/group_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/handlers/internal_demo_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/internal_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/base_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/default_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/policies/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26952 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/handlers/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/saml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.317190 consoleme-1.3.1.dev3/consoleme/handlers/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/aws_iam_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/dynamic_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/generate_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/generate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/managed_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33629 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25989 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/self_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/service_control_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/templated_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/typeahead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/user_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/aws_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/current_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/swag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/alb_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81605 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/aws_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/aws_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/aws_config/aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/aws_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/change_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/dynamic_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/internal_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/role_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cookie-py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/credential_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49019 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/event_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/event_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/event_bridge/access_denies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/event_bridge/role_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22017 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/handler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35445 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15893 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/role_updater/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/role_updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/role_updater/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/role_updater/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/role_updater/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/s3_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/saml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/scm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/scm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/scm/git/
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/scm/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/scm/git/bitbucket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/self_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/self_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/self_service/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/self_service/typeahead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/ses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/templated_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/templated_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/templated_resources/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/templated_resources/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/aws_principals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121179 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26089 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.297189 consoleme-1.3.1.dev3/consoleme/templates/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.333190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/
+-rw-r--r--   0 runner    (1001) docker     (127)  1780372 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/DifferentGradient.png
+-rw-r--r--   0 runner    (1001) docker     (127)   784262 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/Honeybee.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1401997 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/MikeCloudNoGradientWithFace.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32211 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/netflix-security-dark-bg-tight.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.337190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/
+-rw-r--r--   0 runner    (1001) docker     (127)   353657 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   230322 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   243749 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.337190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/
+-rw-r--r--   0 runner    (1001) docker     (127)   374928 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   387350 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   359457 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.341190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/
+-rw-r--r--   0 runner    (1001) docker     (127)   375501 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   347136 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   362390 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.301189 consoleme-1.3.1.dev3/consoleme/templates/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.341190 consoleme-1.3.1.dev3/consoleme/templates/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   609522 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/css/main.463a8800.css
+-rw-r--r--   0 runner    (1001) docker     (127)   904718 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/css/main.463a8800.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.349190 consoleme-1.3.1.dev3/consoleme/templates/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  2669634 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68532 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  8284688 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/consoleme/templates/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    54488 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.278156e41e0ad908cf7f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    98404 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.65a2fb6d9aaa164b41a0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   507628 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.6729d29753e000c17489.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    63728 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.cac87dc00c87a5d74711.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    98640 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.d68fa3e67dbb653a13ce.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/flags.99f63ae7a743f21ab308.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40148 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.38c6d8bab26db77d8c80.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    50524 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.425399f81e4ce7cbd967.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   390837 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.62d9dae4e0040e81c980.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   106004 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.a01e3f2d6c83dc3aee17.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   105784 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.c656b8caa454ed19b9a2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    30928 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.5367103510b27b784827.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.687a4990ea22bb1a49d4.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31156 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.752905fa5edf21fc52a1.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   107201 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.9c4845b4b41ef40a22fa.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.ddae9b1ba9b0b42f5880.woff
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper1Active.9866ff3a1ea1cc7a93fa.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper1Complete.6222088c914dcaffd0e4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Active.b5befeb514c5ec2f9815.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Complete.47bfe6ee0ee7b0da663a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Pending.3aac534f4c215708e3eb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper3Active.45f15c88d73d2a09105e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper3Pending.b72269cdc74f6782c021.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/warning.5b4ee25d2b57cd9f461e.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/consoleme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/scripts/initialize_dynamodb_oss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/scripts/initialize_redis_oss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/scripts/retrieve_or_decode_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/tests/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/celery/test_celery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/tests/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_accessui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_role_login_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/tests/handlers/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_aws_iam_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_generate_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38224 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_typeahead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/test_main.py
```

### Comparing `consoleme-1.3.0/LICENSE` & `consoleme-1.3.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/PKG-INFO` & `consoleme-1.3.1.dev3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: consoleme
-Version: 1.3.0
-Summary: A central control plane for AWS permissions and access
-Home-page: https://github.com/Netflix/ConsoleMe
-Author: Netflix Security
-Author-email: consoleme-maintainers@netflix.com
-License: Apache 2.0
-Keywords: consoleme
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3105/)
 [![Discord](https://img.shields.io/discord/730908778299523072?label=Discord&logo=discord&style=flat-square)](https://discord.gg/nQVpNGGkYu)
 
 # ConsoleMe
 
 Check out our [quick start guide](https://hawkins.gitbook.io/consoleme/quick-start)
 , [documentation](https://hawkins.gitbook.io/consoleme/)
@@ -72,14 +59,14 @@
 - [Improving database security at FollowAnalytics with AWS IAM database authentication and ConsoleMe](https://medium.com/followanalytics/improving-database-security-at-followanalytics-with-aws-iam-database-authentication-and-consoleme-d00ea8a6edef)
 - [Awesome IAM Policy Tools](https://github.com/kdeldycke/awesome-iam#aws-policy-tools)
 - [Netflix on AWS Case Study](https://aws.amazon.com/solutions/case-studies/netflix/)
 - [Netflix Open Sources ConsoleMe to Manage Permissions and Access on AWS](infoq.com/news/2021/04/netflix-consoleme-aws/)
 
 ## Companies that use ConsoleMe (alphabetically sorted)
 
-- [AB180](https://en.ab180.co/)
+- [AB180](https://www.ab180.co/en)
 - [Calm](https://www.calm.com/)
 - [FollowAnalytics](https://followanalytics.com/)
 - [myKaarma](https://mykaarma.com/)
 - [National Center for Biotechnology Information](https://www.ncbi.nlm.nih.gov/)
 - Feel free to submit a PR or let us know in an [Issue](https://github.com/Netflix/consoleme/issues) if you'd like to
   add your company to this list.
```

### Comparing `consoleme-1.3.0/cdk/app.py` & `consoleme-1.3.1.dev3/cdk/app.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/consoleme_ecs_service_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/consoleme_ecs_service_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/consoleme_spoke_accounts_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/consoleme_spoke_accounts_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/constants.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/constants.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/helpers.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/helpers.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/alb_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/auth_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/auth_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/cache_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/cache_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/compute_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/compute_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/config_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/config_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/db_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/db_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/domain_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/domain_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/iam_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/iam_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/shared_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/shared_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/service/nested_stacks/vpc_stack.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/vpc_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/consoleme_ecs_cdk/setup.py` & `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/setup.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/cdk/tests/test_cdk.py` & `consoleme-1.3.1.dev3/cdk/tests/test_cdk.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/__main__.py` & `consoleme-1.3.1.dev3/consoleme/__main__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/celery_tasks/celery_tasks.py` & `consoleme-1.3.1.dev3/consoleme/celery_tasks/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/config/config.py` & `consoleme-1.3.1.dev3/consoleme/config/config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/auth/auth.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/auth/auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/aws/aws.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/aws/aws.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/celery_tasks/celery_tasks.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/celery_tasks/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/config/config.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/config/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 class Config:
     @staticmethod
     def get_config_location():
         config_location = os.environ.get("CONFIG_LOCATION")
         default_save_location = f"{os.curdir}/consoleme.yaml"
         if config_location:
+            # Pull config from S3 if an S3 URL is provided
             if config_location.startswith("s3://"):
                 import boto3
 
                 client = boto3.client("s3")
                 bucket, key = split_s3_path(config_location)
                 obj = client.get_object(Bucket=bucket, Key=key)
                 config_data = obj["Body"].read()
@@ -39,14 +40,15 @@
                 return config_location
         config_locations: List[str] = [
             default_save_location,
             os.path.expanduser("~/.config/consoleme/config.yaml"),
             "/etc/consoleme/config/config.yaml",
             "example_config/example_config_development.yaml",
         ]
+        # Use the first config location that exists from the above list.
         for loc in config_locations:
             if os.path.exists(loc):
                 return loc
         raise Exception(
             "Unable to find ConsoleMe's configuration. It either doesn't exist, or "
             "ConsoleMe doesn't have permission to access it. Please set the CONFIG_LOCATION environment variable "
             "to the path of the configuration, or to an s3 location with your configuration"
```

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/group_mapping/group_mapping.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/group_mapping/group_mapping.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/internal_routes/handlers/internal_demo_route.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/handlers/internal_demo_route.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/internal_routes/internal_routes.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/internal_routes.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/metrics/cloudwatch/__init__.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/metrics/default_metrics.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/default_metrics.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/plugins/policies/policies.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/policies/policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/default_plugins/setup.py` & `consoleme-1.3.1.dev3/consoleme/default_plugins/setup.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/exceptions/exceptions.py` & `consoleme-1.3.1.dev3/consoleme/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/auth.py` & `consoleme-1.3.1.dev3/consoleme/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/base.py` & `consoleme-1.3.1.dev3/consoleme/handlers/base.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v1/credentials.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v1/credentials.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v1/headers.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v1/headers.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v1/policies.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v1/policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v1/roles.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v1/roles.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v1/saml.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v1/saml.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/audit.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/audit.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/aws_iam_users.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/aws_iam_users.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/challenge.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/challenge.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/dynamic_config.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/errors.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/errors.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/generate_changes.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/generate_changes.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/generate_policy.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/generate_policy.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/index.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/index.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/logout.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/logout.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/managed_policies.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/managed_policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/notifications.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/notifications.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/policies.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/requests.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/requests.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/resources.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/resources.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/roles.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/roles.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/self_service.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/self_service.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/service_control_policy.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/service_control_policy.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/templated_resources.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/templated_resources.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/typeahead.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/typeahead.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/user.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/user.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/handlers/v2/user_profile.py` & `consoleme-1.3.1.dev3/consoleme/handlers/v2/user_profile.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/account_indexers/__init__.py` & `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/account_indexers/aws_organizations.py` & `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/aws_organizations.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/account_indexers/current_account.py` & `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/current_account.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/account_indexers/local_config.py` & `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/local_config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/account_indexers/swag.py` & `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/swag.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/alb_auth.py` & `consoleme-1.3.1.dev3/consoleme/lib/alb_auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/asyncio.py` & `consoleme-1.3.1.dev3/consoleme/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/auth.py` & `consoleme-1.3.1.dev3/consoleme/lib/auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/aws.py` & `consoleme-1.3.1.dev3/consoleme/lib/aws.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/aws_config/aws_config.py` & `consoleme-1.3.1.dev3/consoleme/lib/aws_config/aws_config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/cache.py` & `consoleme-1.3.1.dev3/consoleme/lib/cache.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/challenge.py` & `consoleme-1.3.1.dev3/consoleme/lib/challenge.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/change_request.py` & `consoleme-1.3.1.dev3/consoleme/lib/change_request.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/__init__.py` & `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/dynamic_config.py` & `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/internal_plugin.py` & `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/internal_plugin.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/models.py` & `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/cloud_credential_authorization_mapping/role_tags.py` & `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/role_tags.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/cloudtrail.py` & `consoleme-1.3.1.dev3/consoleme/lib/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/credential_auth.py` & `consoleme-1.3.1.dev3/consoleme/lib/credential_auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/crypto.py` & `consoleme-1.3.1.dev3/consoleme/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/defaults.py` & `consoleme-1.3.1.dev3/consoleme/lib/defaults.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/duo.py` & `consoleme-1.3.1.dev3/consoleme/lib/duo.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/dynamo.py` & `consoleme-1.3.1.dev3/consoleme/lib/dynamo.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/elasticsearch.py` & `consoleme-1.3.1.dev3/consoleme/lib/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/event_bridge/access_denies.py` & `consoleme-1.3.1.dev3/consoleme/lib/event_bridge/access_denies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/event_bridge/role_updates.py` & `consoleme-1.3.1.dev3/consoleme/lib/event_bridge/role_updates.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/generic.py` & `consoleme-1.3.1.dev3/consoleme/lib/generic.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/git.py` & `consoleme-1.3.1.dev3/consoleme/lib/git.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/google.py` & `consoleme-1.3.1.dev3/consoleme/lib/google.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/groups.py` & `consoleme-1.3.1.dev3/consoleme/lib/groups.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/handler_utils.py` & `consoleme-1.3.1.dev3/consoleme/lib/handler_utils.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/json_encoder.py` & `consoleme-1.3.1.dev3/consoleme/lib/json_encoder.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/jwt.py` & `consoleme-1.3.1.dev3/consoleme/lib/jwt.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/loader.py` & `consoleme-1.3.1.dev3/consoleme/lib/loader.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/notifications/models.py` & `consoleme-1.3.1.dev3/consoleme/lib/notifications/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/oidc.py` & `consoleme-1.3.1.dev3/consoleme/lib/oidc.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/password.py` & `consoleme-1.3.1.dev3/consoleme/lib/password.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/plugins.py` & `consoleme-1.3.1.dev3/consoleme/lib/plugins.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/policies.py` & `consoleme-1.3.1.dev3/consoleme/lib/policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/redis.py` & `consoleme-1.3.1.dev3/consoleme/lib/redis.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/requests.py` & `consoleme-1.3.1.dev3/consoleme/lib/requests.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/role_updater/cli.py` & `consoleme-1.3.1.dev3/consoleme/lib/role_updater/cli.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/role_updater/handler.py` & `consoleme-1.3.1.dev3/consoleme/lib/role_updater/handler.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/role_updater/schemas.py` & `consoleme-1.3.1.dev3/consoleme/lib/role_updater/schemas.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/s3_helpers.py` & `consoleme-1.3.1.dev3/consoleme/lib/s3_helpers.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/saml.py` & `consoleme-1.3.1.dev3/consoleme/lib/saml.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/scm/git/__init__.py` & `consoleme-1.3.1.dev3/consoleme/lib/scm/git/__init__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/scm/git/bitbucket.py` & `consoleme-1.3.1.dev3/consoleme/lib/scm/git/bitbucket.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/self_service/models.py` & `consoleme-1.3.1.dev3/consoleme/lib/self_service/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/self_service/typeahead.py` & `consoleme-1.3.1.dev3/consoleme/lib/self_service/typeahead.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/ses.py` & `consoleme-1.3.1.dev3/consoleme/lib/ses.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/slack.py` & `consoleme-1.3.1.dev3/consoleme/lib/slack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/templated_resources/__init__.py` & `consoleme-1.3.1.dev3/consoleme/lib/templated_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/templated_resources/models.py` & `consoleme-1.3.1.dev3/consoleme/lib/templated_resources/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/templated_resources/requests.py` & `consoleme-1.3.1.dev3/consoleme/lib/templated_resources/requests.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/timeout.py` & `consoleme-1.3.1.dev3/consoleme/lib/timeout.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/tracing.py` & `consoleme-1.3.1.dev3/consoleme/lib/tracing.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/v2/aws_principals.py` & `consoleme-1.3.1.dev3/consoleme/lib/v2/aws_principals.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/v2/notifications.py` & `consoleme-1.3.1.dev3/consoleme/lib/v2/notifications.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/v2/requests.py` & `consoleme-1.3.1.dev3/consoleme/lib/v2/requests.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/v2/user_profile.py` & `consoleme-1.3.1.dev3/consoleme/lib/v2/user_profile.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/lib/web.py` & `consoleme-1.3.1.dev3/consoleme/lib/web.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/models.py` & `consoleme-1.3.1.dev3/consoleme/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/routes.py` & `consoleme-1.3.1.dev3/consoleme/routes.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/asset-manifest.json` & `consoleme-1.3.1.dev3/consoleme/templates/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/favicon.ico` & `consoleme-1.3.1.dev3/consoleme/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/infrasec/DifferentGradient.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/DifferentGradient.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/infrasec/Honeybee.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/Honeybee.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/infrasec/MikeCloudNoGradientWithFace.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/MikeCloudNoGradientWithFace.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/logo192.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/logo192.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/netflix-security-dark-bg-tight.svg` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/netflix-security-dark-bg-tight.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/nosunglasses/1.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/1.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/nosunglasses/2.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/2.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/nosunglasses/3.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/3.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/quarantine/1.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/1.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/quarantine/2.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/2.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/quarantine/3.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/3.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/sunglasses/1.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/1.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/sunglasses/2.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/2.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/images/logos/sunglasses/3.png` & `consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/3.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/index.html` & `consoleme-1.3.1.dev3/consoleme/templates/index.html`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/css/main.463a8800.css` & `consoleme-1.3.1.dev3/consoleme/templates/static/css/main.463a8800.css`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/css/main.463a8800.css.map` & `consoleme-1.3.1.dev3/consoleme/templates/static/css/main.463a8800.css.map`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/js/main.903555c6.js` & `consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/js/main.903555c6.js.LICENSE.txt` & `consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/js/main.903555c6.js.map` & `consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js.map`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/brand-icons.278156e41e0ad908cf7f.woff2` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.278156e41e0ad908cf7f.woff2`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/brand-icons.65a2fb6d9aaa164b41a0.ttf` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.65a2fb6d9aaa164b41a0.ttf`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/brand-icons.6729d29753e000c17489.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.6729d29753e000c17489.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/brand-icons.cac87dc00c87a5d74711.woff` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.cac87dc00c87a5d74711.woff`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/brand-icons.d68fa3e67dbb653a13ce.eot` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.d68fa3e67dbb653a13ce.eot`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/flags.99f63ae7a743f21ab308.png` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/flags.99f63ae7a743f21ab308.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/icons.38c6d8bab26db77d8c80.woff2` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.38c6d8bab26db77d8c80.woff2`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/icons.425399f81e4ce7cbd967.woff` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.425399f81e4ce7cbd967.woff`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/icons.62d9dae4e0040e81c980.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.62d9dae4e0040e81c980.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/icons.a01e3f2d6c83dc3aee17.eot` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.a01e3f2d6c83dc3aee17.eot`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/icons.c656b8caa454ed19b9a2.ttf` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.c656b8caa454ed19b9a2.ttf`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/outline-icons.5367103510b27b784827.ttf` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.5367103510b27b784827.ttf`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/outline-icons.687a4990ea22bb1a49d4.woff2` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.687a4990ea22bb1a49d4.woff2`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/outline-icons.752905fa5edf21fc52a1.eot` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.752905fa5edf21fc52a1.eot`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/outline-icons.9c4845b4b41ef40a22fa.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.9c4845b4b41ef40a22fa.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/outline-icons.ddae9b1ba9b0b42f5880.woff` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.ddae9b1ba9b0b42f5880.woff`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/stepper1Active.9866ff3a1ea1cc7a93fa.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper1Active.9866ff3a1ea1cc7a93fa.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/stepper1Complete.6222088c914dcaffd0e4.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper1Complete.6222088c914dcaffd0e4.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/stepper2Active.b5befeb514c5ec2f9815.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Active.b5befeb514c5ec2f9815.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/stepper2Complete.47bfe6ee0ee7b0da663a.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Complete.47bfe6ee0ee7b0da663a.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/stepper2Pending.3aac534f4c215708e3eb.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Pending.3aac534f4c215708e3eb.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/stepper3Active.45f15c88d73d2a09105e.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper3Active.45f15c88d73d2a09105e.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/stepper3Pending.b72269cdc74f6782c021.svg` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper3Pending.b72269cdc74f6782c021.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme/templates/static/media/warning.5b4ee25d2b57cd9f461e.png` & `consoleme-1.3.1.dev3/consoleme/templates/static/media/warning.5b4ee25d2b57cd9f461e.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme.egg-info/SOURCES.txt` & `consoleme-1.3.1.dev3/consoleme.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,15 @@
 consoleme/templates/static/media/stepper3Active.45f15c88d73d2a09105e.svg
 consoleme/templates/static/media/stepper3Pending.b72269cdc74f6782c021.svg
 consoleme/templates/static/media/warning.5b4ee25d2b57cd9f461e.png
 scripts/__init__.py
 scripts/initialize_dynamodb_oss.py
 scripts/initialize_redis_oss.py
 scripts/retrieve_or_decode_configuration.py
+tests/test_main.py
 tests/celery/__init__.py
 tests/celery/test_celery.py
 tests/handlers/__init__.py
 tests/handlers/test_accessui.py
 tests/handlers/test_base.py
 tests/handlers/test_policies.py
 tests/handlers/test_role_login_api.py
```

### Comparing `consoleme-1.3.0/consoleme.egg-info/entry_points.txt` & `consoleme-1.3.1.dev3/consoleme.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/consoleme.egg-info/requires.txt` & `consoleme-1.3.1.dev3/consoleme.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/scripts/initialize_dynamodb_oss.py` & `consoleme-1.3.1.dev3/scripts/initialize_dynamodb_oss.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/scripts/initialize_redis_oss.py` & `consoleme-1.3.1.dev3/scripts/initialize_redis_oss.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/scripts/retrieve_or_decode_configuration.py` & `consoleme-1.3.1.dev3/scripts/retrieve_or_decode_configuration.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/setup.py` & `consoleme-1.3.1.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/celery/test_celery.py` & `consoleme-1.3.1.dev3/tests/celery/test_celery.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/test_base.py` & `consoleme-1.3.1.dev3/tests/handlers/test_base.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/test_policies.py` & `consoleme-1.3.1.dev3/tests/handlers/test_policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/test_role_login_api.py` & `consoleme-1.3.1.dev3/tests/handlers/test_role_login_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Docstring in public module."""
+
 import os
 import sys
+from unittest.mock import patch
 
 import ujson as json
 from tornado.testing import AsyncHTTPTestCase
 
 APP_ROOT = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(os.path.join(APP_ROOT, ".."))
 
@@ -48,25 +50,40 @@
             response_j["message"],
             "You have more than one role matching your query. Please select one.",
         )
         self.assertEqual(response_j["reason"], "multiple_roles")
         self.assertEqual(response_j["type"], "redirect")
         self.assertIn("/?arn=role&warningMessage=", response_j["redirect_url"])
 
-    def test_role_api_success(self):
+    @patch("consoleme.default_plugins.plugins.aws.aws.AsyncHTTPClient")
+    def test_role_api_success(self, mock_client):
         from consoleme.config import config
 
+        class TestResp:
+            def __init__(self, code, body):
+                self.code = code
+                self.body = body
+
+        class TestClient:
+            async def fetch(
+                self, url, method="GET", body=None, headers=None, ssl_options=None
+            ):
+                return TestResp(
+                    code=200, body='{"SigninToken": "testTokenSignin456223"}'
+                )
+
+        mock_client.return_value = TestClient()
         headers = {
             config.get("auth.user_header_name"): "userwithrole@example.com",
             config.get("auth.groups_header_name"): "groupa@example.com",
         }
 
         response = self.fetch("/api/v2/role_login/roleA", headers=headers)
         self.assertEqual(response.code, 200)
         response_j = json.loads(response.body)
         self.assertEqual(response_j["type"], "redirect")
         self.assertEqual(response_j["reason"], "console_login")
         self.assertEqual(response_j["role"], "arn:aws:iam::123456789012:role/roleA")
         self.assertIn(
-            "https://signin.aws.amazon.com/federation?Action=login&Issuer=YourCompany&Destination=https%3A%2F%2Fus-east-1.console.aws.amazon.com&SigninToken=",
+            "https://signin.aws.amazon.com/federation?Action=login&Issuer=YourCompany&Destination=https%3A%2F%2Fus-east-1.console.aws.amazon.com&SigninToken=testTokenSignin456223",
             response_j["redirect_url"],
         )
```

### Comparing `consoleme-1.3.0/tests/handlers/v2/test_aws_iam_users.py` & `consoleme-1.3.1.dev3/tests/handlers/v2/test_aws_iam_users.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/v2/test_errors.py` & `consoleme-1.3.1.dev3/tests/handlers/v2/test_errors.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/v2/test_generate_changes.py` & `consoleme-1.3.1.dev3/tests/handlers/v2/test_generate_changes.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/v2/test_policies.py` & `consoleme-1.3.1.dev3/tests/handlers/v2/test_policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/v2/test_requests.py` & `consoleme-1.3.1.dev3/tests/handlers/v2/test_requests.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/v2/test_roles.py` & `consoleme-1.3.1.dev3/tests/handlers/v2/test_roles.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/v2/test_typeahead.py` & `consoleme-1.3.1.dev3/tests/handlers/v2/test_typeahead.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/v2/test_user.py` & `consoleme-1.3.1.dev3/tests/handlers/v2/test_user.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.0/tests/handlers/v2/test_user_profile.py` & `consoleme-1.3.1.dev3/tests/handlers/v2/test_user_profile.py`

 * *Files identical despite different names*

