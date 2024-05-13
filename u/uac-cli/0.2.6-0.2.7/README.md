# Comparing `tmp/uac-cli-0.2.6.tar.gz` & `tmp/uac-cli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-cli-0.2.6.tar", last modified: Fri May 10 17:14:44 2024, max compression
+gzip compressed data, was "uac-cli-0.2.7.tar", last modified: Mon May 13 18:27:21 2024, max compression
```

## Comparing `uac-cli-0.2.6.tar` & `uac-cli-0.2.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.237628 uac-cli-0.2.6/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-10 17:14:44.237279 uac-cli-0.2.6/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9041 2024-05-07 21:43:44.000000 uac-cli-0.2.6/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      405 2024-05-07 21:45:43.000000 uac-cli-0.2.6/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-10 17:14:44.237684 uac-cli-0.2.6/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1185 2024-05-08 02:51:37.000000 uac-cli-0.2.6/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.213675 uac-cli-0.2.6/uac_cli/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      145 2024-05-10 17:10:20.000000 uac-cli-0.2.6/uac_cli/__init__.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.234890 uac-cli-0.2.6/uac_cli/commands/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.2.6/uac_cli/commands/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5545 2024-05-07 20:59:24.000000 uac-cli-0.2.6/uac_cli/commands/agent.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6346 2024-05-07 21:00:04.000000 uac-cli-0.2.6/uac_cli/commands/agent_cluster.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      918 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/audit.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9331 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/bundle.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2994 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/business_service.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5357 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/calendar.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1188 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/cluster_node.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2891 2024-05-10 16:40:07.000000 uac-cli-0.2.6/uac_cli/commands/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11836 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/connection.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3875 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/credential.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3434 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/custom_day.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2929 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/email_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1491 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/ldap.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      756 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/metric.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2954 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/oauth_client.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3023 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/oms_server.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1616 2024-05-08 03:23:56.000000 uac-cli-0.2.6/uac_cli/commands/property.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      958 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/report.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2527 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/script.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3134 2024-05-08 03:49:16.000000 uac-cli-0.2.6/uac_cli/commands/server_operation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2993 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/simulation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      726 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/system.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9664 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/task.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    19049 2024-05-08 04:47:43.000000 uac-cli-0.2.6/uac_cli/commands/task_instance.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6392 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/trigger.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1499 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/universal_event.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3084 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/universal_event_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6950 2024-05-08 05:29:26.000000 uac-cli-0.2.6/uac_cli/commands/universal_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4716 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/user.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2678 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/user_group.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3495 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/variable.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3691 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/virtual_resource.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4208 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/webhook.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5716 2024-05-08 04:31:39.000000 uac-cli-0.2.6/uac_cli/commands/workflow.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6719 2024-05-10 17:08:47.000000 uac-cli-0.2.6/uac_cli/main.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.236755 uac-cli-0.2.6/uac_cli/utils/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.2.6/uac_cli/utils/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2970 2024-05-10 16:44:39.000000 uac-cli-0.2.6/uac_cli/utils/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      573 2024-05-08 05:25:10.000000 uac-cli-0.2.6/uac_cli/utils/options.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2736 2024-05-10 16:09:14.000000 uac-cli-0.2.6/uac_cli/utils/process.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.216435 uac-cli-0.2.6/uac_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       66 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/top_level.txt
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 18:27:21.805607 uac-cli-0.2.7/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9671 2024-05-13 18:27:21.805297 uac-cli-0.2.7/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9041 2024-05-07 21:43:44.000000 uac-cli-0.2.7/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      405 2024-05-07 21:45:43.000000 uac-cli-0.2.7/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-13 18:27:21.805658 uac-cli-0.2.7/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1193 2024-05-10 17:16:23.000000 uac-cli-0.2.7/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 18:27:21.788999 uac-cli-0.2.7/uac_cli/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      145 2024-05-10 18:36:37.000000 uac-cli-0.2.7/uac_cli/__init__.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 18:27:21.803534 uac-cli-0.2.7/uac_cli/commands/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.2.7/uac_cli/commands/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5545 2024-05-07 20:59:24.000000 uac-cli-0.2.7/uac_cli/commands/agent.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6346 2024-05-07 21:00:04.000000 uac-cli-0.2.7/uac_cli/commands/agent_cluster.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      918 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/audit.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9331 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/bundle.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2994 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/business_service.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5357 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/calendar.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1188 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/cluster_node.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2891 2024-05-10 16:40:07.000000 uac-cli-0.2.7/uac_cli/commands/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11836 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/connection.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3875 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/credential.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3434 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/custom_day.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2929 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/email_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1491 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      756 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/metric.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2954 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/oauth_client.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3023 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/oms_server.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1616 2024-05-08 03:23:56.000000 uac-cli-0.2.7/uac_cli/commands/property.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      958 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/report.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2527 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/script.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3134 2024-05-08 03:49:16.000000 uac-cli-0.2.7/uac_cli/commands/server_operation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2993 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/simulation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      726 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9664 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/task.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    19049 2024-05-08 04:47:43.000000 uac-cli-0.2.7/uac_cli/commands/task_instance.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6392 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/trigger.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1499 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/universal_event.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3084 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/universal_event_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6950 2024-05-08 05:29:26.000000 uac-cli-0.2.7/uac_cli/commands/universal_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4716 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/user.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2678 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/user_group.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3495 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/variable.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3691 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/virtual_resource.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4208 2024-05-07 15:20:53.000000 uac-cli-0.2.7/uac_cli/commands/webhook.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5716 2024-05-08 04:31:39.000000 uac-cli-0.2.7/uac_cli/commands/workflow.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6868 2024-05-10 18:49:31.000000 uac-cli-0.2.7/uac_cli/main.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 18:27:21.804945 uac-cli-0.2.7/uac_cli/utils/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.2.7/uac_cli/utils/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2970 2024-05-10 16:44:39.000000 uac-cli-0.2.7/uac_cli/utils/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      573 2024-05-08 05:25:10.000000 uac-cli-0.2.7/uac_cli/utils/options.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2736 2024-05-10 16:09:14.000000 uac-cli-0.2.7/uac_cli/utils/process.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-13 18:27:21.790701 uac-cli-0.2.7/uac_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9671 2024-05-13 18:27:21.000000 uac-cli-0.2.7/uac_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-13 18:27:21.000000 uac-cli-0.2.7/uac_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-13 18:27:21.000000 uac-cli-0.2.7/uac_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-13 18:27:21.000000 uac-cli-0.2.7/uac_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       73 2024-05-13 18:27:21.000000 uac-cli-0.2.7/uac_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-13 18:27:21.000000 uac-cli-0.2.7/uac_cli.egg-info/top_level.txt
```

### Comparing `uac-cli-0.2.6/PKG-INFO` & `uac-cli-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: uac-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: A CLI tool for executing commands against the Stonebranch UAC API
-Author: Stonebranch
+Author: Huseyin G.
 Author-email: "Huseyin G." <huseyim@gmail.com>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://github.com/gomleksiz/uac-cli
 Project-URL: Issues, https://github.com/gomleksiz/uac-cli/issues
 Project-URL: Documentation, https://uac-cli.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uac-cli-0.2.6/README.md` & `uac-cli-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/setup.py` & `uac-cli-0.2.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,21 +9,21 @@
         name='uac-cli',
         version=version,
         author_email="huseyim@gmail.com",
         license="CC BY-NC 4.0",
         packages=find_packages(),
         include_package_data=True,
         install_requires=[
-            "uac-api",
+            "uac-api >= 0.4.5",
             "setuptools >= 44.1.1",
             "click == 8.1.6",
             "jsonpath-ng == 1.5.3",
             "PyYAML"
         ],
-        author='Stonebranch',
+        author='Huseyin G.',
         description='A CLI tool for executing commands against the Stonebranch UAC API',
         entry_points={
             'console_scripts': [
                 'uac=uac_cli.main:run'
             ]
         },
         python_requires='>=3.7',
```

### Comparing `uac-cli-0.2.6/uac_cli/commands/agent.py` & `uac-cli-0.2.7/uac_cli/commands/agent.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/agent_cluster.py` & `uac-cli-0.2.7/uac_cli/commands/agent_cluster.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/audit.py` & `uac-cli-0.2.7/uac_cli/commands/audit.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/bundle.py` & `uac-cli-0.2.7/uac_cli/commands/bundle.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/business_service.py` & `uac-cli-0.2.7/uac_cli/commands/business_service.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/calendar.py` & `uac-cli-0.2.7/uac_cli/commands/calendar.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/cluster_node.py` & `uac-cli-0.2.7/uac_cli/commands/cluster_node.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/config.py` & `uac-cli-0.2.7/uac_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/connection.py` & `uac-cli-0.2.7/uac_cli/commands/connection.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/credential.py` & `uac-cli-0.2.7/uac_cli/commands/credential.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/custom_day.py` & `uac-cli-0.2.7/uac_cli/commands/custom_day.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/email_template.py` & `uac-cli-0.2.7/uac_cli/commands/email_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/ldap.py` & `uac-cli-0.2.7/uac_cli/commands/ldap.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/metric.py` & `uac-cli-0.2.7/uac_cli/commands/metric.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/oauth_client.py` & `uac-cli-0.2.7/uac_cli/commands/oauth_client.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/oms_server.py` & `uac-cli-0.2.7/uac_cli/commands/oms_server.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/property.py` & `uac-cli-0.2.7/uac_cli/commands/property.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/report.py` & `uac-cli-0.2.7/uac_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/script.py` & `uac-cli-0.2.7/uac_cli/commands/script.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/server_operation.py` & `uac-cli-0.2.7/uac_cli/commands/server_operation.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/simulation.py` & `uac-cli-0.2.7/uac_cli/commands/simulation.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/system.py` & `uac-cli-0.2.7/uac_cli/commands/system.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/task.py` & `uac-cli-0.2.7/uac_cli/commands/task.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/task_instance.py` & `uac-cli-0.2.7/uac_cli/commands/task_instance.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/trigger.py` & `uac-cli-0.2.7/uac_cli/commands/trigger.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/universal_event.py` & `uac-cli-0.2.7/uac_cli/commands/universal_event.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/universal_event_template.py` & `uac-cli-0.2.7/uac_cli/commands/universal_event_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/universal_template.py` & `uac-cli-0.2.7/uac_cli/commands/universal_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/user.py` & `uac-cli-0.2.7/uac_cli/commands/user.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/user_group.py` & `uac-cli-0.2.7/uac_cli/commands/user_group.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/variable.py` & `uac-cli-0.2.7/uac_cli/commands/variable.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/virtual_resource.py` & `uac-cli-0.2.7/uac_cli/commands/virtual_resource.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/webhook.py` & `uac-cli-0.2.7/uac_cli/commands/webhook.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/commands/workflow.py` & `uac-cli-0.2.7/uac_cli/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/main.py` & `uac-cli-0.2.7/uac_cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     def __init__(self, profile_name='default', log_level='ERROR', temp_profile=None):
         self.log_level = log_level
         if temp_profile:
             self.profile = temp_profile
         else:
             self.profile = read_profile(profile_name)
         self.setup_logging()
-        self.log.debug(f'Profile URL: {self.profile.get("url")}')
+        if self.profile:
+            self.log.debug(f'Profile URL: {self.profile.get("url")}')
 
 
     def setup_logging(self):
         if self.log_level != "DEBUG":
             sys.tracebacklimit = 0
         logging.basicConfig(level=self.log_level)
         logging.info(f'UAC CLI is running... (Version: {__version__})')
@@ -124,14 +125,17 @@
         }
     else:
         temp_profile = None
 
 
     cli = UacCli(log_level=log_level, profile_name=profile, temp_profile=temp_profile)
     ctx.obj = cli.main()
+    if ctx.obj is None and ctx.invoked_subcommand != "config": 
+        click.echo("No profile found.")
+        exit(1)
 
 
 main.add_command(config)
 main.add_command(agent)
 main.add_command(agent_cluster)
 main.add_command(audit)
 main.add_command(bundle)
```

### Comparing `uac-cli-0.2.6/uac_cli/utils/config.py` & `uac-cli-0.2.7/uac_cli/utils/config.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/utils/options.py` & `uac-cli-0.2.7/uac_cli/utils/options.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli/utils/process.py` & `uac-cli-0.2.7/uac_cli/utils/process.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.6/uac_cli.egg-info/PKG-INFO` & `uac-cli-0.2.7/uac_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: uac-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: A CLI tool for executing commands against the Stonebranch UAC API
-Author: Stonebranch
+Author: Huseyin G.
 Author-email: "Huseyin G." <huseyim@gmail.com>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://github.com/gomleksiz/uac-cli
 Project-URL: Issues, https://github.com/gomleksiz/uac-cli/issues
 Project-URL: Documentation, https://uac-cli.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uac-cli-0.2.6/uac_cli.egg-info/SOURCES.txt` & `uac-cli-0.2.7/uac_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

