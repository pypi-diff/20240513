# Comparing `tmp/pycti-6.0.9.tar.gz` & `tmp/pycti-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-6.0.9.tar", last modified: Wed Apr  3 11:21:10 2024, max compression
+gzip compressed data, was "pycti-6.1.0.tar", last modified: Mon May 13 08:06:32 2024, max compression
```

## Comparing `pycti-6.0.9.tar` & `pycti-6.1.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.684364 pycti-6.0.9/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-04-03 11:20:58.000000 pycti-6.0.9/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-04-03 11:21:10.684364 pycti-6.0.9/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-04-03 11:20:58.000000 pycti-6.0.9/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.672364 pycti-6.0.9/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4691 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.676365 pycti-6.0.9/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28980 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/opencti_api_playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7109 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.676365 pycti-6.0.9/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    55835 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/connector/opencti_connector_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/connector/opencti_metric_handler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.684364 pycti-6.0.9/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18331 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27005 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17392 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20904 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33037 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    48728 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   103971 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    77998 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14610 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.684364 pycti-6.0.9/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7915 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   112190 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-04-03 11:20:58.000000 pycti-6.0.9/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-03 11:21:10.684364 pycti-6.0.9/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-03 11:21:10.000000 pycti-6.0.9/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-04-03 11:20:58.000000 pycti-6.0.9/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-04-03 11:21:10.688365 pycti-6.0.9/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.225975 pycti-6.1.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-13 08:06:17.000000 pycti-6.1.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-13 08:06:32.225975 pycti-6.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-13 08:06:17.000000 pycti-6.1.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.213975 pycti-6.1.0/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.213975 pycti-6.1.0/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/opencti_api_playbook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.213975 pycti-6.1.0/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    60538 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/connector/opencti_connector_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/connector/opencti_metric_handler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.221975 pycti-6.1.0/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18990 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    78434 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16641 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.225975 pycti-6.1.0/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   120458 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.225975 pycti-6.1.0/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-13 08:06:17.000000 pycti-6.1.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-13 08:06:32.229975 pycti-6.1.0/setup.cfg
```

### Comparing `pycti-6.0.9/LICENSE` & `pycti-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/PKG-INFO` & `pycti-6.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.0.9
+Version: 6.1.0
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,33 +25,33 @@
 Requires-Dist: pika~=1.3.1
 Requires-Dist: python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
 Requires-Dist: prometheus-client~=0.20.0
 Requires-Dist: python-magic-bin~=0.4.14; sys_platform == "win32"
 Requires-Dist: python_json_logger~=2.0.4
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: requests~=2.31.0
-Requires-Dist: setuptools~=69.2.0
+Requires-Dist: setuptools~=69.5.1
 Requires-Dist: filigran-sseclient~=1.0.0
 Requires-Dist: stix2~=3.0.1
 Requires-Dist: cachetools~=5.3.0
 Provides-Extra: dev
-Requires-Dist: black~=24.3.0; extra == "dev"
+Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
 Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 Requires-Dist: pytest-cases~=3.8.0; extra == "dev"
 Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
 Requires-Dist: pytest_randomly~=3.15.0; extra == "dev"
-Requires-Dist: pytest~=8.1.1; extra == "dev"
+Requires-Dist: pytest~=8.2.0; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
 Requires-Dist: wheel~=0.43.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: autoapi~=2.0.1; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints~=2.0.0; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints~=2.1.0; extra == "doc"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "doc"
 
 # OpenCTI client for Python
 
 [![Website](https://img.shields.io/badge/website-opencti.io-blue.svg)](https://opencti.io)
 [![CircleCI](https://circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://circleci.com/gh/OpenCTI-Platform/client-python/tree/master)
 [![readthedocs](https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)](https://opencti-client-for-python.readthedocs.io/en/latest/)
```

### Comparing `pycti-6.0.9/README.md` & `pycti-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/__init__.py` & `pycti-6.1.0/pycti/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "6.0.9"
+__version__ = "6.1.0"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
@@ -49,17 +49,22 @@
 from .entities.opencti_threat_actor_group import ThreatActorGroup
 from .entities.opencti_threat_actor_individual import ThreatActorIndividual
 from .entities.opencti_tool import Tool
 from .entities.opencti_vulnerability import Vulnerability
 from .utils.constants import (
     CustomObjectCaseIncident,
     CustomObjectTask,
+    CustomObservableBankAccount,
+    CustomObservableCredential,
     CustomObservableCryptocurrencyWallet,
     CustomObservableHostname,
+    CustomObservablePaymentCard,
+    CustomObservablePhoneNumber,
     CustomObservableText,
+    CustomObservableTrackingNumber,
     CustomObservableUserAgent,
     MultipleRefRelationship,
     StixCyberObservableTypes,
     StixMetaTypes,
 )
 from .utils.opencti_stix2 import (
     STIX_EXT_MITRE,
@@ -124,15 +129,20 @@
     "ThreatActorIndividual",
     "Tool",
     "Vulnerability",
     "get_config_variable",
     "CustomObjectCaseIncident",
     "CustomObjectTask",
     "StixCyberObservableTypes",
+    "CustomObservableCredential",
     "CustomObservableHostname",
     "CustomObservableUserAgent",
+    "CustomObservableBankAccount",
     "CustomObservableCryptocurrencyWallet",
+    "CustomObservablePaymentCard",
+    "CustomObservablePhoneNumber",
+    "CustomObservableTrackingNumber",
     "CustomObservableText",
     "STIX_EXT_MITRE",
     "STIX_EXT_OCTI_SCO",
     "STIX_EXT_OCTI",
 ]
```

### Comparing `pycti-6.0.9/pycti/api/opencti_api_client.py` & `pycti-6.1.0/pycti/api/opencti_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,21 +104,23 @@
         self,
         url,
         token,
         log_level="info",
         ssl_verify=False,
         proxies=None,
         json_logging=False,
+        bundle_send_to_queue=True,
         cert=None,
         auth=None,
         perform_health_check=True,
     ):
         """Constructor method"""
 
         # Check configuration
+        self.bundle_send_to_queue = bundle_send_to_queue
         self.ssl_verify = ssl_verify
         self.cert = cert
         self.proxies = proxies
         if url is None or len(url) == 0:
             raise ValueError("An URL must be set")
         if token is None or len(token) == 0 or token == "ChangeMe":
             raise ValueError("A TOKEN must be set")
@@ -201,14 +203,20 @@
             raise ValueError(
                 "OpenCTI API is not reachable. Waiting for OpenCTI API to start or check your configuration..."
             )
 
     def set_applicant_id_header(self, applicant_id):
         self.request_headers["opencti-applicant-id"] = applicant_id
 
+    def set_playbook_id_header(self, playbook_id):
+        self.request_headers["opencti-playbook-id"] = playbook_id
+
+    def set_event_id(self, event_id):
+        self.request_headers["opencti-event-id"] = event_id
+
     def set_synchronized_upsert_header(self, synchronized):
         self.request_headers["synchronized-upsert"] = (
             "true" if synchronized is True else "false"
         )
 
     def set_previous_standard_header(self, previous_standard):
         self.request_headers["previous-standard"] = previous_standard
@@ -610,39 +618,43 @@
             del data["content_alt"]
         return data
 
     def upload_file(self, **kwargs):
         """upload a file to OpenCTI API
 
         :param `**kwargs`: arguments for file upload (required: `file_name` and `data`)
-        :return: returns the query respons for the file upload
+        :return: returns the query response for the file upload
         :rtype: dict
         """
 
         file_name = kwargs.get("file_name", None)
+        file_markings = kwargs.get("file_markings", None)
         data = kwargs.get("data", None)
         mime_type = kwargs.get("mime_type", "text/plain")
         if file_name is not None:
             self.app_logger.info("Uploading a file.")
             query = """
-                mutation UploadImport($file: Upload!) {
-                    uploadImport(file: $file) {
+                mutation UploadImport($file: Upload!, $fileMarkings: [String]) {
+                    uploadImport(file: $file, fileMarkings: $fileMarkings) {
                         id
                         name
                     }
                 }
              """
             if data is None:
                 data = open(file_name, "rb")
                 if file_name.endswith(".json"):
                     mime_type = "application/json"
                 else:
                     mime_type = magic.from_file(file_name, mime=True)
-
-            return self.query(query, {"file": (File(file_name, data, mime_type))})
+            query_vars = {"file": (File(file_name, data, mime_type))}
+            # optional file markings
+            if file_markings is not None:
+                query_vars["fileMarkings"] = file_markings
+            return self.query(query, query_vars)
         else:
             self.app_logger.error("[upload] Missing parameter: file_name")
             return None
 
     def upload_pending_file(self, **kwargs):
         """upload a file to OpenCTI API
```

### Comparing `pycti-6.0.9/pycti/api/opencti_api_connector.py` & `pycti-6.1.0/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/api/opencti_api_playbook.py` & `pycti-6.1.0/pycti/api/opencti_api_playbook.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,23 @@
         self.api = api
 
     def playbook_step_execution(self, playbook: dict, bundle: str):
         self.api.app_logger.info(
             "Executing playbook step", {"playbook_id": playbook["playbook_id"]}
         )
         query = """
-            mutation PlaybookStepExecution($execution_id: ID!, $execution_start: DateTime!, $data_instance_id: ID!, $playbook_id: ID!, $previous_step_id: ID!, $step_id: ID!, $previous_bundle: String!, $bundle: String!) {
-                playbookStepExecution(execution_id: $execution_id, execution_start: $execution_start, data_instance_id: $data_instance_id, playbook_id: $playbook_id, previous_step_id: $previous_step_id, step_id: $step_id, previous_bundle: $previous_bundle, bundle: $bundle)
+            mutation PlaybookStepExecution($execution_id: ID!, $event_id: ID!, $execution_start: DateTime!, $data_instance_id: ID!, $playbook_id: ID!, $previous_step_id: ID!, $step_id: ID!, $previous_bundle: String!, $bundle: String!) {
+                playbookStepExecution(execution_id: $execution_id, event_id: $event_id, execution_start: $execution_start, data_instance_id: $data_instance_id, playbook_id: $playbook_id, previous_step_id: $previous_step_id, step_id: $step_id, previous_bundle: $previous_bundle, bundle: $bundle)
             }
            """
         self.api.query(
             query,
             {
                 "execution_id": playbook["execution_id"],
+                "event_id": playbook["event_id"],
                 "execution_start": playbook["execution_start"],
                 "playbook_id": playbook["playbook_id"],
                 "data_instance_id": playbook["data_instance_id"],
                 "step_id": playbook["step_id"],
                 "previous_step_id": playbook["previous_step_id"],
                 "previous_bundle": playbook["previous_bundle"],
                 "bundle": bundle,
```

### Comparing `pycti-6.0.9/pycti/api/opencti_api_work.py` & `pycti-6.1.0/pycti/api/opencti_api_work.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,92 +5,101 @@
 class OpenCTIApiWork:
     """OpenCTIApiJob"""
 
     def __init__(self, api):
         self.api = api
 
     def to_received(self, work_id: str, message: str):
-        self.api.app_logger.info("Reporting work update_received", {"work_id": work_id})
-        query = """
-            mutation workToReceived($id: ID!, $message: String) {
-                workEdit(id: $id) {
-                    toReceived (message: $message)
+        if self.api.bundle_send_to_queue:
+            self.api.app_logger.info(
+                "Reporting work update_received", {"work_id": work_id}
+            )
+            query = """
+                mutation workToReceived($id: ID!, $message: String) {
+                    workEdit(id: $id) {
+                        toReceived (message: $message)
+                    }
                 }
-            }
-           """
-        self.api.query(query, {"id": work_id, "message": message})
+               """
+            self.api.query(query, {"id": work_id, "message": message})
 
     def to_processed(self, work_id: str, message: str, in_error: bool = False):
-        self.api.app_logger.info(
-            "Reporting work update_processed", {"work_id": work_id}
-        )
-        query = """
-            mutation workToProcessed($id: ID!, $message: String, $inError: Boolean) {
-                workEdit(id: $id) {
-                    toProcessed (message: $message, inError: $inError)
-                }
-            }
-           """
-        self.api.query(query, {"id": work_id, "message": message, "inError": in_error})
+        if self.api.bundle_send_to_queue:
+            self.api.app_logger.info(
+                "Reporting work update_processed", {"work_id": work_id}
+            )
+            query = """
+                mutation workToProcessed($id: ID!, $message: String, $inError: Boolean) {
+                    workEdit(id: $id) {
+                        toProcessed (message: $message, inError: $inError)
+                    }
+                }
+               """
+            self.api.query(
+                query, {"id": work_id, "message": message, "inError": in_error}
+            )
 
     def ping(self, work_id: str):
         self.api.app_logger.info("Ping work", {"work_id": work_id})
         query = """
             mutation pingWork($id: ID!) {
                 workEdit(id: $id) {
                     ping
                 }
             }
            """
         self.api.query(query, {"id": work_id})
 
     def report_expectation(self, work_id: str, error):
-        self.api.app_logger.info("Report expectation", {"work_id": work_id})
-        query = """
-            mutation reportExpectation($id: ID!, $error: WorkErrorInput) {
-                workEdit(id: $id) {
-                    reportExpectation(error: $error)
-                }
-            }
-           """
-        try:
-            self.api.query(query, {"id": work_id, "error": error})
-        except:
-            self.api.app_logger.error("Cannot report expectation")
+        if self.api.bundle_send_to_queue:
+            self.api.app_logger.info("Report expectation", {"work_id": work_id})
+            query = """
+                mutation reportExpectation($id: ID!, $error: WorkErrorInput) {
+                    workEdit(id: $id) {
+                        reportExpectation(error: $error)
+                    }
+                }
+               """
+            try:
+                self.api.query(query, {"id": work_id, "error": error})
+            except:
+                self.api.app_logger.error("Cannot report expectation")
 
     def add_expectations(self, work_id: str, expectations: int):
-        self.api.app_logger.info(
-            "Update action expectations",
-            {"work_id": work_id, "expectations": expectations},
-        )
-        query = """
-            mutation addExpectations($id: ID!, $expectations: Int) {
-                workEdit(id: $id) {
-                    addExpectations(expectations: $expectations)
-                }
-            }
-           """
-        try:
-            self.api.query(query, {"id": work_id, "expectations": expectations})
-        except:
-            self.api.app_logger.error("Cannot report expectation")
+        if self.api.bundle_send_to_queue:
+            self.api.app_logger.info(
+                "Update action expectations",
+                {"work_id": work_id, "expectations": expectations},
+            )
+            query = """
+                mutation addExpectations($id: ID!, $expectations: Int) {
+                    workEdit(id: $id) {
+                        addExpectations(expectations: $expectations)
+                    }
+                }
+               """
+            try:
+                self.api.query(query, {"id": work_id, "expectations": expectations})
+            except:
+                self.api.app_logger.error("Cannot report expectation")
 
     def initiate_work(self, connector_id: str, friendly_name: str) -> str:
-        self.api.app_logger.info("Initiate work", {"connector_id": connector_id})
-        query = """
-            mutation workAdd($connectorId: String!, $friendlyName: String) {
-                workAdd(connectorId: $connectorId, friendlyName: $friendlyName) {
-                  id
-                }
-            }
-           """
-        work = self.api.query(
-            query, {"connectorId": connector_id, "friendlyName": friendly_name}
-        )
-        return work["data"]["workAdd"]["id"]
+        if self.api.bundle_send_to_queue:
+            self.api.app_logger.info("Initiate work", {"connector_id": connector_id})
+            query = """
+                mutation workAdd($connectorId: String!, $friendlyName: String) {
+                    workAdd(connectorId: $connectorId, friendlyName: $friendlyName) {
+                      id
+                    }
+                }
+               """
+            work = self.api.query(
+                query, {"connectorId": connector_id, "friendlyName": friendly_name}
+            )
+            return work["data"]["workAdd"]["id"]
 
     def delete_work(self, work_id: str):
         query = """
         mutation ConnectorWorksMutation($workId: ID!) {
             workEdit(id: $workId) {
                 delete
             }
```

### Comparing `pycti-6.0.9/pycti/connector/opencti_connector.py` & `pycti-6.1.0/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/connector/opencti_connector_helper.py` & `pycti-6.1.0/pycti/connector/opencti_connector_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -278,26 +278,28 @@
                         "Unable to read/access to the entity, please check that the connector permission"
                     )
                 event_data["enrichment_entity"] = opencti_entity
                 # Handle action vs playbook behavior
                 is_playbook = "playbook" in json_data["internal"]
                 # If playbook, compute object on data bundle
                 if is_playbook:
-                    execution_id = json_data["internal"]["playbook"]["execution_id"]
                     execution_start = self.helper.date_now()
-                    playbook_id = json_data["internal"]["playbook"]["playbook_id"]
-                    data_instance_id = json_data["internal"]["playbook"][
+                    event_id = json_data["internal"]["playbook"].get("event_id")
+                    execution_id = json_data["internal"]["playbook"].get("execution_id")
+                    playbook_id = json_data["internal"]["playbook"].get("playbook_id")
+                    data_instance_id = json_data["internal"]["playbook"].get(
                         "data_instance_id"
-                    ]
+                    )
                     previous_bundle = json.dumps((json_data["event"]["bundle"]))
                     step_id = json_data["internal"]["playbook"]["step_id"]
                     previous_step_id = json_data["internal"]["playbook"][
                         "previous_step_id"
                     ]
                     playbook_data = {
+                        "event_id": event_id,
                         "execution_id": execution_id,
                         "execution_start": execution_start,
                         "playbook_id": playbook_id,
                         "data_instance_id": data_instance_id,
                         "previous_step_id": previous_step_id,
                         "previous_bundle": previous_bundle,
                         "step_id": step_id,
@@ -724,14 +726,40 @@
         self.connect_confidence_level = None  # Deprecated since OpenCTI version >= 6.0
         self.connect_scope = get_config_variable(
             "CONNECTOR_SCOPE", ["connector", "scope"], config
         )
         self.connect_auto = get_config_variable(
             "CONNECTOR_AUTO", ["connector", "auto"], config, False, False
         )
+        self.bundle_send_to_queue = get_config_variable(
+            "CONNECTOR_SEND_TO_QUEUE",
+            ["connector", "send_to_queue"],
+            config,
+            False,
+            True,
+        )
+        self.bundle_send_to_directory = get_config_variable(
+            "CONNECTOR_SEND_TO_DIRECTORY",
+            ["connector", "send_to_directory"],
+            config,
+            False,
+            False,
+        )
+        self.bundle_send_to_directory_path = get_config_variable(
+            "CONNECTOR_SEND_TO_DIRECTORY_PATH",
+            ["connector", "send_to_directory_path"],
+            config,
+        )
+        self.bundle_send_to_directory_retention = get_config_variable(
+            "CONNECTOR_SEND_TO_DIRECTORY_RETENTION",
+            ["connector", "send_to_directory_retention"],
+            config,
+            True,
+            7,
+        )
         self.connect_only_contextual = get_config_variable(
             "CONNECTOR_ONLY_CONTEXTUAL",
             ["connector", "only_contextual"],
             config,
             False,
             False,
         )
@@ -745,14 +773,16 @@
             False,
             False,
         )
         self.connect_validate_before_import = get_config_variable(
             "CONNECTOR_VALIDATE_BEFORE_IMPORT",
             ["connector", "validate_before_import"],
             config,
+            False,
+            False,
         )
         # Start up the server to expose the metrics.
         expose_metrics = get_config_variable(
             "CONNECTOR_EXPOSE_METRICS",
             ["connector", "expose_metrics"],
             config,
             False,
@@ -765,22 +795,24 @@
         # Initialize configuration
         # - Classic API that will be directly attached to the connector rights
         self.api = OpenCTIApiClient(
             self.opencti_url,
             self.opencti_token,
             self.log_level,
             json_logging=self.opencti_json_logging,
+            bundle_send_to_queue=self.bundle_send_to_queue,
         )
         # - Impersonate API that will use applicant id
         # Behave like standard api if applicant not found
         self.api_impersonate = OpenCTIApiClient(
             self.opencti_url,
             self.opencti_token,
             self.log_level,
             json_logging=self.opencti_json_logging,
+            bundle_send_to_queue=self.bundle_send_to_queue,
         )
         self.connector_logger = self.api.logger_class(self.connect_name)
         # For retro compatibility
         self.log_debug = self.connector_logger.debug
         self.log_info = self.connector_logger.info
         self.log_warning = self.connector_logger.warning
         self.log_error = self.connector_logger.error
@@ -1071,14 +1103,24 @@
         entities_types = kwargs.get("entities_types", None)
         update = kwargs.get("update", False)
         event_version = kwargs.get("event_version", None)
         bypass_split = kwargs.get("bypass_split", False)
         bypass_validation = kwargs.get("bypass_validation", False)
         entity_id = kwargs.get("entity_id", None)
         file_name = kwargs.get("file_name", None)
+        bundle_send_to_queue = kwargs.get("send_to_queue", self.bundle_send_to_queue)
+        bundle_send_to_directory = kwargs.get(
+            "send_to_directory", self.bundle_send_to_directory
+        )
+        bundle_send_to_directory_path = kwargs.get(
+            "send_to_directory_path", self.bundle_send_to_directory_path
+        )
+        bundle_send_to_directory_retention = kwargs.get(
+            "send_to_directory_retention", self.bundle_send_to_directory_retention
+        )
 
         # In case of enrichment ingestion, ensure the sharing if needed
         if self.enrichment_shared_organizations is not None:
             # Every element of the bundle must be enriched with the same organizations
             bundle_data = json.loads(bundle)
             for item in bundle_data["objects"]:
                 if (
@@ -1110,81 +1152,139 @@
                         )
                     else:
                         item["x_opencti_granted_refs"] = (
                             self.enrichment_shared_organizations
                         )
             bundle = json.dumps(bundle_data)
 
+        # If execution in playbook, callback the api
         if self.playbook is not None:
             self.api.playbook.playbook_step_execution(self.playbook, bundle)
             return [bundle]
 
+        # Upload workbench in case of pending validation
         if not file_name and work_id:
             file_name = f"{work_id}.json"
-
         if self.connect_validate_before_import and not bypass_validation and file_name:
             self.api.upload_pending_file(
                 file_name=file_name,
                 data=bundle,
                 mime_type="application/json",
                 entity_id=entity_id,
             )
             return []
 
-        if entities_types is None:
-            entities_types = []
+        # If directory setup, write the bundle to the target directory
+        if bundle_send_to_directory and bundle_send_to_directory_path is not None:
+            self.connector_logger.info(
+                "The connector sending bundle to directory",
+                {
+                    "connector": self.connect_name,
+                    "directory": bundle_send_to_directory_path,
+                    "also_queuing": bundle_send_to_queue,
+                },
+            )
+            bundle_file = (
+                self.connect_name.lower().replace(" ", "_")
+                + "-"
+                + time.strftime("%Y%m%d-%H%M%S-")
+                + str(time.time())
+                + ".json"
+            )
+            write_file = os.path.join(
+                bundle_send_to_directory_path, bundle_file + ".tmp"
+            )
+            message_bundle = {
+                "bundle_type": "DIRECTORY_BUNDLE",
+                "applicant_id": self.applicant_id,
+                "connector": {
+                    "id": self.connect_id,
+                    "name": self.connect_name,
+                    "type": self.connect_type,
+                    "scope": self.connect_scope,
+                    "auto": self.connect_auto,
+                    "validate_before_import": self.connect_validate_before_import,
+                },
+                "entities_types": entities_types,
+                "bundle": json.loads(bundle),
+                "update": update,
+            }
+            # Maintains the list of files under control
+            if bundle_send_to_directory_retention > 0:  # If 0, disable the auto remove
+                current_time = time.time()
+                for f in os.listdir(bundle_send_to_directory_path):
+                    if f.endswith(".json"):
+                        file_location = os.path.join(bundle_send_to_directory_path, f)
+                        file_time = os.stat(file_location).st_mtime
+                        is_expired_file = (
+                            file_time
+                            < current_time - 86400 * bundle_send_to_directory_retention
+                        )  # 86400 = 1 day
+                        if is_expired_file:
+                            os.remove(file_location)
+            # Write the bundle to target directory
+            with open(write_file, "w") as f:
+                str_bundle = json.dumps(message_bundle)
+                f.write(str_bundle)
+            # Rename the file after full write
+            final_write_file = os.path.join(bundle_send_to_directory_path, bundle_file)
+            os.rename(write_file, final_write_file)
 
         if bypass_split:
             bundles = [bundle]
         else:
             stix2_splitter = OpenCTIStix2Splitter()
             bundles = stix2_splitter.split_bundle(bundle, True, event_version)
 
         if len(bundles) == 0:
             self.metric.inc("error_count")
             raise ValueError("Nothing to import")
 
-        if work_id:
-            self.api.work.add_expectations(work_id, len(bundles))
-
-        pika_credentials = pika.PlainCredentials(
-            self.connector_config["connection"]["user"],
-            self.connector_config["connection"]["pass"],
-        )
-        pika_parameters = pika.ConnectionParameters(
-            host=self.connector_config["connection"]["host"],
-            port=self.connector_config["connection"]["port"],
-            virtual_host=self.connector_config["connection"]["vhost"],
-            credentials=pika_credentials,
-            ssl_options=(
-                pika.SSLOptions(
-                    create_mq_ssl_context(self.config),
-                    self.connector_config["connection"]["host"],
-                )
-                if self.connector_config["connection"]["use_ssl"]
-                else None
-            ),
-        )
-        pika_connection = pika.BlockingConnection(pika_parameters)
-        channel = pika_connection.channel()
-        try:
-            channel.confirm_delivery()
-        except Exception as err:  # pylint: disable=broad-except
-            self.connector_logger.warning(str(err))
-        for sequence, bundle in enumerate(bundles, start=1):
-            self._send_bundle(
-                channel,
-                bundle,
-                work_id=work_id,
-                entities_types=entities_types,
-                sequence=sequence,
-                update=update,
+        if bundle_send_to_queue:
+            if work_id:
+                self.api.work.add_expectations(work_id, len(bundles))
+            if entities_types is None:
+                entities_types = []
+            pika_credentials = pika.PlainCredentials(
+                self.connector_config["connection"]["user"],
+                self.connector_config["connection"]["pass"],
+            )
+            pika_parameters = pika.ConnectionParameters(
+                host=self.connector_config["connection"]["host"],
+                port=self.connector_config["connection"]["port"],
+                virtual_host=self.connector_config["connection"]["vhost"],
+                credentials=pika_credentials,
+                ssl_options=(
+                    pika.SSLOptions(
+                        create_mq_ssl_context(self.config),
+                        self.connector_config["connection"]["host"],
+                    )
+                    if self.connector_config["connection"]["use_ssl"]
+                    else None
+                ),
             )
-        channel.close()
-        pika_connection.close()
+            pika_connection = pika.BlockingConnection(pika_parameters)
+            channel = pika_connection.channel()
+            try:
+                channel.confirm_delivery()
+            except Exception as err:  # pylint: disable=broad-except
+                self.connector_logger.warning(str(err))
+            self.connector_logger.info(self.connect_name + " sending bundle to queue")
+            for sequence, bundle in enumerate(bundles, start=1):
+                self._send_bundle(
+                    channel,
+                    bundle,
+                    work_id=work_id,
+                    entities_types=entities_types,
+                    sequence=sequence,
+                    update=update,
+                )
+            channel.close()
+            pika_connection.close()
+
         return bundles
 
     def _send_bundle(self, channel, bundle, **kwargs) -> None:
         """send a STIX2 bundle to RabbitMQ to be consumed by workers
 
         :param channel: RabbitMQ channel
         :type channel: callable
@@ -1208,14 +1308,15 @@
         # if not validation.is_valid:
         # raise ValueError('The bundle is not a valid STIX2 JSON')
 
         # Prepare the message
         # if self.current_work_id is None:
         #    raise ValueError('The job id must be specified')
         message = {
+            "bundle_type": "QUEUE_BUNDLE",
             "applicant_id": self.applicant_id,
             "action_sequence": sequence,
             "entities_types": entities_types,
             "content": base64.b64encode(bundle.encode("utf-8", "escape")).decode(
                 "utf-8"
             ),
             "update": update,
```

### Comparing `pycti-6.0.9/pycti/connector/opencti_metric_handler.py` & `pycti-6.1.0/pycti/connector/opencti_metric_handler.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_attack_pattern.py` & `pycti-6.1.0/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_campaign.py` & `pycti-6.1.0/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_case_incident.py` & `pycti-6.1.0/pycti/entities/opencti_case_incident.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
             },
         )
         if get_all:
             final_data = []
             data = self.opencti.process_multiple(result["data"]["caseIncidents"])
             final_data = final_data + data
             while result["data"]["caseIncidents"]["pageInfo"]["hasNextPage"]:
-                after = result["date"]["caseIncidents"]["pageInfo"]["endCursor"]
+                after = result["data"]["caseIncidents"]["pageInfo"]["endCursor"]
                 self.opencti.app_logger.info("Listing Case Incidents", {"after": after})
                 result = self.opencti.query(
                     query,
                     {
                         "filters": filters,
                         "search": search,
                         "first": first,
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_case_rfi.py` & `pycti-6.1.0/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_case_rft.py` & `pycti-6.1.0/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_channel.py` & `pycti-6.1.0/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_course_of_action.py` & `pycti-6.1.0/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_data_component.py` & `pycti-6.1.0/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_data_source.py` & `pycti-6.1.0/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_event.py` & `pycti-6.1.0/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_external_reference.py` & `pycti-6.1.0/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_feedback.py` & `pycti-6.1.0/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_grouping.py` & `pycti-6.1.0/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_identity.py` & `pycti-6.1.0/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_incident.py` & `pycti-6.1.0/pycti/entities/opencti_incident.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,14 +454,18 @@
                 stix_object["x_opencti_stix_ids"] = (
                     self.opencti.get_attribute_in_extension("stix_ids", stix_object)
                 )
             if "x_opencti_granted_refs" not in stix_object:
                 stix_object["x_opencti_granted_refs"] = (
                     self.opencti.get_attribute_in_extension("granted_refs", stix_object)
                 )
+            if "x_opencti_workflow_id" not in stix_object:
+                stix_object["x_opencti_workflow_id"] = (
+                    self.opencti.get_attribute_in_extension("workflow_id", stix_object)
+                )
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=(
                     extras["created_by_id"] if "created_by_id" in extras else None
                 ),
                 objectMarking=(
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_indicator.py` & `pycti-6.1.0/pycti/entities/opencti_indicator.py`

 * *Files 4% similar despite different names*

```diff
@@ -464,14 +464,15 @@
             "x_opencti_main_observable_type", None
         )
         x_mitre_platforms = kwargs.get("x_mitre_platforms", None)
         kill_chain_phases = kwargs.get("killChainPhases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         create_observables = kwargs.get("x_opencti_create_observables", False)
         granted_refs = kwargs.get("objectOrganization", None)
+        x_opencti_workflow_id = kwargs.get("x_opencti_workflow_id", None)
         update = kwargs.get("update", False)
 
         if (
             name is not None
             and pattern is not None
             and pattern_type is not None
             and x_opencti_main_observable_type is not None
@@ -524,14 +525,15 @@
                         "x_opencti_score": x_opencti_score,
                         "x_opencti_detection": x_opencti_detection,
                         "x_opencti_main_observable_type": x_opencti_main_observable_type,
                         "x_mitre_platforms": x_mitre_platforms,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
                         "killChainPhases": kill_chain_phases,
                         "createObservables": create_observables,
+                        "x_opencti_workflow_id": x_opencti_workflow_id,
                         "update": update,
                     }
                 },
             )
             return self.opencti.process_multiple_fields(result["data"]["indicatorAdd"])
         else:
             self.opencti.app_logger.error(
@@ -638,14 +640,18 @@
                 stix_object["x_opencti_stix_ids"] = (
                     self.opencti.get_attribute_in_extension("stix_ids", stix_object)
                 )
             if "x_opencti_granted_refs" not in stix_object:
                 stix_object["x_opencti_granted_refs"] = (
                     self.opencti.get_attribute_in_extension("granted_refs", stix_object)
                 )
+            if "x_opencti_workflow_id" not in stix_object:
+                stix_object["x_opencti_workflow_id"] = (
+                    self.opencti.get_attribute_in_extension("workflow_id", stix_object)
+                )
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=(
                     extras["created_by_id"] if "created_by_id" in extras else None
                 ),
                 objectMarking=(
@@ -736,13 +742,18 @@
                     else False
                 ),
                 objectOrganization=(
                     stix_object["x_opencti_granted_refs"]
                     if "x_opencti_granted_refs" in stix_object
                     else None
                 ),
+                x_opencti_workflow_id=(
+                    stix_object["x_opencti_workflow_id"]
+                    if "x_opencti_workflow_id" in stix_object
+                    else None
+                ),
                 update=update,
             )
         else:
             self.opencti.app_logger.error(
                 "[opencti_indicator] Missing parameters: stixObject"
             )
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_infrastructure.py` & `pycti-6.1.0/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_intrusion_set.py` & `pycti-6.1.0/pycti/entities/opencti_intrusion_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -282,17 +282,39 @@
                 "search": search,
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
-        return self.opencti.process_multiple(
-            result["data"]["intrusionSets"], with_pagination
-        )
+        if get_all:
+            final_data = []
+            data = self.opencti.process_multiple(result["data"]["intrusionSets"])
+            final_data = final_data + data
+            while result["data"]["intrusionSets"]["pageInfo"]["hasNextPage"]:
+                after = result["data"]["intrusionSets"]["pageInfo"]["endCursor"]
+                self.opencti.app_logger.info("Listing Intrusion-Sets", {"after": after})
+                result = self.opencti.query(
+                    query,
+                    {
+                        "filters": filters,
+                        "search": search,
+                        "first": first,
+                        "after": after,
+                        "orderBy": order_by,
+                        "orderMode": order_mode,
+                    },
+                )
+                data = self.opencti.process_multiple(result["data"]["intrusionSets"])
+                final_data = final_data + data
+            return final_data
+        else:
+            return self.opencti.process_multiple(
+                result["data"]["intrusionSets"], with_pagination
+            )
 
     """
         Read a Intrusion-Set object
 
         :param id: the id of the Intrusion-Set
         :param filters: the filters to apply if no id provided
         :return Intrusion-Set object
@@ -359,14 +381,15 @@
         last_seen = kwargs.get("last_seen", None)
         goals = kwargs.get("goals", None)
         resource_level = kwargs.get("resource_level", None)
         primary_motivation = kwargs.get("primary_motivation", None)
         secondary_motivations = kwargs.get("secondary_motivations", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
+        x_opencti_workflow_id = kwargs.get("x_opencti_workflow_id", None)
         update = kwargs.get("update", False)
 
         if name is not None:
             self.opencti.app_logger.info("Creating Intrusion-Set", {"name": name})
             query = """
                 mutation IntrusionSetAdd($input: IntrusionSetAddInput!) {
                     intrusionSetAdd(input: $input) {
@@ -398,14 +421,15 @@
                         "first_seen": first_seen,
                         "last_seen": last_seen,
                         "goals": goals,
                         "resource_level": resource_level,
                         "primary_motivation": primary_motivation,
                         "secondary_motivations": secondary_motivations,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
+                        "x_opencti_workflow_id": x_opencti_workflow_id,
                         "update": update,
                     }
                 },
             )
             return self.opencti.process_multiple_fields(
                 result["data"]["intrusionSetAdd"]
             )
@@ -431,15 +455,19 @@
                 stix_object["x_opencti_stix_ids"] = (
                     self.opencti.get_attribute_in_extension("stix_ids", stix_object)
                 )
             if "x_opencti_granted_refs" not in stix_object:
                 stix_object["x_opencti_granted_refs"] = (
                     self.opencti.get_attribute_in_extension("granted_refs", stix_object)
                 )
-
+            if "x_opencti_workflow_id" not in stix_object:
+                stix_object["x_opencti_workflow_id"] = (
+                    self.opencti.get_attribute_in_extension("workflow_id", stix_object)
+                )
+                7
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=(
                     extras["created_by_id"] if "created_by_id" in extras else None
                 ),
                 objectMarking=(
                     extras["object_marking_ids"]
@@ -496,13 +524,18 @@
                     else None
                 ),
                 objectOrganization=(
                     stix_object["x_opencti_granted_refs"]
                     if "x_opencti_granted_refs" in stix_object
                     else None
                 ),
+                x_opencti_workflow_id=(
+                    stix_object["x_opencti_workflow_id"]
+                    if "x_opencti_workflow_id" in stix_object
+                    else None
+                ),
                 update=update,
             )
         else:
             self.opencti.app_logger.error(
                 "[opencti_intrusion_set] Missing parameters: stixObject"
             )
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_kill_chain_phase.py` & `pycti-6.1.0/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_label.py` & `pycti-6.1.0/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_language.py` & `pycti-6.1.0/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_location.py` & `pycti-6.1.0/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_malware.py` & `pycti-6.1.0/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_malware_analysis.py` & `pycti-6.1.0/pycti/entities/opencti_malware_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,14 +397,15 @@
         hostVm = kwargs.get("hostVm", None)
         operatingSystem = kwargs.get("operatingSystem", None)
         installedSoftware = kwargs.get("installedSoftware", None)
         sample = kwargs.get("sample", None)
         analysisSco = kwargs.get("analysisSco", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
+        x_opencti_workflow_id = kwargs.get("x_opencti_workflow_id", None)
         update = kwargs.get("update", False)
 
         if product is not None and result_name is not None:
             self.opencti.app_logger.info(
                 "Creating Malware analysis", {"product": product}
             )
             query = """
@@ -445,14 +446,15 @@
                         "modules": modules,
                         "hostVm": hostVm,
                         "operatingSystem": operatingSystem,
                         "installedSoftware": installedSoftware,
                         "analysisSample": sample,
                         "analysisSco": analysisSco,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
+                        "x_opencti_workflow_id": x_opencti_workflow_id,
                         "update": update,
                     }
                 },
             )
             return self.opencti.process_multiple_fields(
                 result["data"]["malwareAnalysisAdd"]
             )
@@ -478,14 +480,18 @@
                 stix_object["x_opencti_stix_ids"] = (
                     self.opencti.get_attribute_in_extension("stix_ids", stix_object)
                 )
             if "x_opencti_granted_refs" not in stix_object:
                 stix_object["x_opencti_granted_refs"] = (
                     self.opencti.get_attribute_in_extension("granted_refs", stix_object)
                 )
+            if "x_opencti_workflow_id" not in stix_object:
+                stix_object["x_opencti_workflow_id"] = (
+                    self.opencti.get_attribute_in_extension("workflow_id", stix_object)
+                )
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=(
                     extras["created_by_id"] if "created_by_id" in extras else None
                 ),
                 objectMarking=(
@@ -570,13 +576,18 @@
                     else None
                 ),
                 objectOrganization=(
                     stix_object["x_opencti_granted_refs"]
                     if "x_opencti_granted_refs" in stix_object
                     else None
                 ),
+                x_opencti_workflow_id=(
+                    stix_object["x_opencti_workflow_id"]
+                    if "x_opencti_workflow_id" in stix_object
+                    else None
+                ),
                 update=update,
             )
         else:
             self.opencti.app_logger.error(
                 "[opencti_malware_analysis] Missing parameters: stixObject"
             )
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_marking_definition.py` & `pycti-6.1.0/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_narrative.py` & `pycti-6.1.0/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_note.py` & `pycti-6.1.0/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_observed_data.py` & `pycti-6.1.0/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_opinion.py` & `pycti-6.1.0/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_report.py` & `pycti-6.1.0/pycti/entities/opencti_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,14 +462,27 @@
         if isinstance(published, datetime.datetime):
             published = published.isoformat()
         data = {"name": name, "published": published}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
         return "report--" + id
 
+    @staticmethod
+    def generate_fixed_fake_id(name, published=None):
+        name = name.lower().strip()
+        if isinstance(published, datetime.datetime):
+            published = published.isoformat()
+        if published is not None:
+            data = {"name": name, "published": published, "fake": "fake"}
+        else:
+            data = {"name": name, "fake": "fake"}
+        data = canonicalize(data, utf8=False)
+        id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
+        return "report--" + id
+
     """
         List Report objects
 
         :param filters: the filters to apply
         :param search: the search keyword
         :param first: return the first n rows from the after ID (or the beginning if not set)
         :param after: ID of the first row for pagination
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_stix.py` & `pycti-6.1.0/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_stix_core_object.py` & `pycti-6.1.0/pycti/entities/opencti_stix_core_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,17 +431,26 @@
                                 id
                                 entity_type
                                 standard_id
                             }
                         }
                     }
                 }
-            }      
+            }
             ... on StixCyberObservable {
                 observable_value
+                indicators {
+                    edges {
+                        node {
+                            id
+                            pattern
+                            pattern_type
+                        }
+                    }
+                }
             }
             ... on AutonomousSystem {
                 number
                 name_alt: name
                 rir
             }
             ... on Directory {
@@ -611,14 +620,20 @@
                 iban
                 bic
                 account_number
             }
             ... on PhoneNumber {
                 value
             }
+            ... on TrackingNumber {
+                value
+            }
+            ... on Credential {
+                value
+            }
             ... on PaymentCard {
                 card_number
                 expiration_date
                 cvv
                 holder_name
             }
             ... on MediaContent {
@@ -1080,17 +1095,26 @@
                                 id
                                 entity_type
                                 standard_id
                             }
                         }
                     }
                 }
-            }      
+            }
             ... on StixCyberObservable {
                 observable_value
+                indicators {
+                    edges {
+                        node {
+                            id
+                            pattern
+                            pattern_type
+                        }
+                    }
+                }
             }
             ... on AutonomousSystem {
                 number
                 name_alt: name
                 rir
             }
             ... on Directory {
@@ -1449,31 +1473,40 @@
                     }
                 """
         result = self.opencti.query(query, {"id": id})
         entity = self.opencti.process_multiple_fields(result["data"]["stixCoreObject"])
         return entity["importFiles"]
 
     def push_list_export(
-        self, entity_id, entity_type, file_name, data, list_filters="", mime_type=None
+        self,
+        entity_id,
+        entity_type,
+        file_name,
+        file_markings,
+        data,
+        list_filters="",
+        mime_type=None,
     ):
         query = """
-            mutation StixCoreObjectsExportPush($entity_id: String, $entity_type: String!, $file: Upload!, $listFilters: String) {
-                stixCoreObjectsExportPush(entity_id: $entity_id, entity_type: $entity_type, file: $file, listFilters: $listFilters)
+            mutation StixCoreObjectsExportPush($entity_id: String, $entity_type: String!, $file: Upload!, $file_markings: [String]!, $listFilters: String) {
+                stixCoreObjectsExportPush(entity_id: $entity_id, entity_type: $entity_type, file: $file, file_markings: $file_markings, listFilters: $listFilters)
             }
         """
+
         if mime_type is None:
             file = self.file(file_name, data)
         else:
             file = self.file(file_name, data, mime_type)
         self.opencti.query(
             query,
             {
                 "entity_id": entity_id,
                 "entity_type": entity_type,
                 "file": file,
+                "file_markings": file_markings,
                 "listFilters": list_filters,
             },
         )
 
     """
         Get the reports about a Stix-Core-Object object
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_stix_core_relationship.py` & `pycti-6.1.0/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-6.1.0/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,20 @@
                 iban
                 bic
                 account_number
             }
             ... on PhoneNumber {
                 value
             }
+            ... on TrackingNumber {
+                value
+            }
+            ... on Credential {
+                value
+            }
             ... on PaymentCard {
                 card_number
                 expiration_date
                 cvv
                 holder_name
             }
             ... on MediaContent {
@@ -572,14 +578,20 @@
                 iban
                 bic
                 account_number
             }
             ... on PhoneNumber {
                 value
             }
+            ... on TrackingNumber {
+                value
+            }
+            ... on Credential {
+                value
+            }
             ... on PaymentCard {
                 card_number
                 expiration_date
                 cvv
                 holder_name
             }
             ... on MediaContent {
@@ -853,14 +865,23 @@
             type = "StixFile"
         elif type.lower() == "ipv4-addr":
             type = "IPv4-Addr"
         elif type.lower() == "ipv6-addr":
             type = "IPv6-Addr"
         elif type.lower() == "hostname" or type.lower() == "x-opencti-hostname":
             type = "Hostname"
+        elif type.lower() == "payment-card" or type.lower() == "x-opencti-payment-card":
+            type = "Payment-Card"
+        elif type.lower() == "credential" or type.lower() == "x-opencti-credential":
+            type = "Credential"
+        elif (
+            type.lower() == "tracking-number"
+            or type.lower() == "x-opencti-tracking-number"
+        ):
+            type = "Tracking-Number"
         elif (
             type.lower() == "cryptocurrency-wallet"
             or type.lower() == "x-opencti-cryptocurrency-wallet"
         ):
             type = "Cryptocurrency-Wallet"
         elif type.lower() == "user-agent" or type.lower() == "x-opencti-user-agent":
             type = "User-Agent"
@@ -970,14 +991,16 @@
                     $CryptographicKey: CryptographicKeyAddInput,
                     $CryptocurrencyWallet: CryptocurrencyWalletAddInput,
                     $Hostname: HostnameAddInput
                     $Text: TextAddInput,
                     $UserAgent: UserAgentAddInput
                     $BankAccount: BankAccountAddInput
                     $PhoneNumber: PhoneNumberAddInput
+                    $Credential: CredentialAddInput
+                    $TrackingNumber: TrackingNumberAddInput
                     $PaymentCard: PaymentCardAddInput
                     $MediaContent: MediaContentAddInput
                 ) {
                     stixCyberObservableAdd(
                         type: $type,
                         stix_id: $stix_id,
                         x_opencti_score: $x_opencti_score,
@@ -1012,14 +1035,16 @@
                         CryptographicKey: $CryptographicKey,
                         CryptocurrencyWallet: $CryptocurrencyWallet,
                         Hostname: $Hostname,
                         Text: $Text,
                         UserAgent: $UserAgent
                         BankAccount: $BankAccount
                         PhoneNumber: $PhoneNumber
+                        Credential: $Credential
+                        TrackingNumber: $TrackingNumber
                         PaymentCard: $PaymentCard
                         MediaContent: $MediaContent
                     ) {
                         id
                         standard_id
                         entity_type
                         parent_types
@@ -1504,23 +1529,14 @@
                 }
             elif type == "Cryptographic-Key":
                 input_variables["CryptographicKey"] = {
                     "value": (
                         observable_data["value"] if "value" in observable_data else None
                     ),
                 }
-            elif (
-                type == "Cryptocurrency-Wallet"
-                or type == "X-OpenCTI-Cryptocurrency-Wallet"
-            ):
-                input_variables["CryptocurrencyWallet"] = {
-                    "value": (
-                        observable_data["value"] if "value" in observable_data else None
-                    ),
-                }
             elif type == "Hostname":
                 input_variables["Hostname"] = {
                     "value": (
                         observable_data["value"] if "value" in observable_data else None
                     ),
                 }
             elif type == "Text":
@@ -1584,16 +1600,58 @@
                     "url": observable_data["url"] if "url" in observable_data else None,
                     "publication_date": (
                         observable_data["publication_date"]
                         if "publication_date" in observable_data
                         else None
                     ),
                 }
+            elif type == "Payment-Card" or type.lower() == "x-opencti-payment-card":
+                input_variables["PaymentCard"] = {
+                    "card_number": (
+                        observable_data["card_number"]
+                        if "card_number" in observable_data
+                        else None
+                    ),
+                    "expiration_date": (
+                        observable_data["expiration_date"]
+                        if "expiration_date" in observable_data
+                        else None
+                    ),
+                    "cvv": observable_data["cvv"] if "cvv" in observable_data else None,
+                    "holder_name": (
+                        observable_data["holder_name"]
+                        if "holder_name" in observable_data
+                        else None
+                    ),
+                }
+            elif (
+                type == "Cryptocurrency-Wallet"
+                or type.lower() == "x-opencti-cryptocurrency-wallet"
+            ):
+                input_variables["CryptocurrencyWallet"] = {
+                    "value": (
+                        observable_data["value"] if "value" in observable_data else None
+                    ),
+                }
+            elif type == "Credential" or type.lower() == "x-opencti-credential":
+                input_variables["Credential"] = {
+                    "value": (
+                        observable_data["value"] if "value" in observable_data else None
+                    ),
+                }
+            elif (
+                type == "Tracking-Number" or type.lower() == "x-opencti-tracking-number"
+            ):
+                input_variables["TrackingNumber"] = {
+                    "value": (
+                        observable_data["value"] if "value" in observable_data else None
+                    ),
+                }
             result = self.opencti.query(query, input_variables)
-            if "payload_bin" in observable_data and "mime/type" in observable_data:
+            if "payload_bin" in observable_data and "mime_type" in observable_data:
                 self.add_file(
                     id=result["data"]["stixCyberObservableAdd"]["id"],
                     file_name=(
                         observable_data["x_opencti_additional_names"][0]
                         if "x_opencti_additional_names" in observable_data
                         and len(observable_data["x_opencti_additional_names"]) > 0
                         else "artifact.bin"
@@ -2254,31 +2312,51 @@
             )
             return True
         else:
             self.opencti.app_logger.error("Missing parameters: id and label_id")
             return False
 
     def push_list_export(
-        self, entity_id, entity_type, file_name, data, list_filters="", mime_type=None
+        self,
+        entity_id,
+        entity_type,
+        file_name,
+        file_markings,
+        data,
+        list_filters="",
+        mime_type=None,
     ):
         query = """
-            mutation StixCyberObservablesExportPush($entity_id: String, $entity_type: String!, $file: Upload!, $listFilters: String) {
-                stixCyberObservablesExportPush(entity_id: $entity_id, entity_type: $entity_type, file: $file, listFilters: $listFilters)
+            mutation StixCyberObservablesExportPush(
+                $entity_id: String,
+                $entity_type: String!,
+                $file: Upload!,
+                $file_markings: [String]!,
+                $listFilters: String
+            ) {
+                stixCyberObservablesExportPush(
+                    entity_id: $entity_id,
+                    entity_type: $entity_type,
+                    file: $file,
+                    file_markings: $file_markings,
+                    listFilters: $listFilters
+                )
             }
         """
         if mime_type is None:
             file = self.file(file_name, data)
         else:
             file = self.file(file_name, data, mime_type)
         self.opencti.query(
             query,
             {
                 "entity_id": entity_id,
                 "entity_type": entity_type,
                 "file": file,
+                "file_markings": file_markings,
                 "listFilters": list_filters,
             },
         )
 
     def ask_for_enrichment(self, **kwargs) -> str:
         id = kwargs.get("id", None)
         connector_id = kwargs.get("connector_id", None)
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_stix_domain_object.py` & `pycti-6.1.0/pycti/entities/opencti_stix_domain_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1321,48 +1321,66 @@
         else:
             self.opencti.app_logger.error(
                 "[opencti_stix_domain_object] Missing parameters: id or file_name"
             )
             return None
 
     def push_list_export(
-        self, entity_id, entity_type, file_name, data, list_filters="", mime_type=None
+        self,
+        entity_id,
+        entity_type,
+        file_name,
+        file_markings,
+        data,
+        list_filters="",
+        mime_type=None,
     ):
         query = """
-            mutation StixDomainObjectsExportPush($entity_id: String, $entity_type: String!, $file: Upload!, $listFilters: String) {
-                stixDomainObjectsExportPush(entity_id: $entity_id, entity_type: $entity_type, file: $file, listFilters: $listFilters)
+            mutation StixDomainObjectsExportPush($entity_id: String, $entity_type: String!, $file: Upload!, $file_markings: [String]!, $listFilters: String) {
+                stixDomainObjectsExportPush(entity_id: $entity_id, entity_type: $entity_type, file: $file,  file_markings: $file_markings, listFilters: $listFilters)
             }
         """
         if mime_type is None:
             file = self.file(file_name, data)
         else:
             file = self.file(file_name, data, mime_type)
         self.opencti.query(
             query,
             {
                 "entity_id": entity_id,
                 "entity_type": entity_type,
                 "file": file,
+                "file_markings": file_markings,
                 "listFilters": list_filters,
             },
         )
 
-    def push_entity_export(self, entity_id, file_name, data, mime_type=None):
+    def push_entity_export(
+        self, entity_id, file_name, data, file_markings, mime_type=None
+    ):
         query = """
-            mutation StixDomainObjectEdit($id: ID!, $file: Upload!) {
+            mutation StixDomainObjectEdit(
+                $id: ID!, $file: Upload!,
+                $file_markings: [String]!
+            ) {
                 stixDomainObjectEdit(id: $id) {
-                    exportPush(file: $file)
+                    exportPush(
+                        file: $file,
+                        file_markings: $file_markings
+                    )
                 }
             }
         """
         if mime_type is None:
             file = self.file(file_name, data)
         else:
             file = self.file(file_name, data, mime_type)
-        self.opencti.query(query, {"id": entity_id, "file": file})
+        self.opencti.query(
+            query, {"id": entity_id, "file": file, "file_markings": file_markings}
+        )
 
     """
         Update the Identity author of a Stix-Domain-Object object (created_by)
 
         :param id: the id of the Stix-Domain-Object
         :param identity_id: the id of the Identity
         :return Boolean
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-6.1.0/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-6.1.0/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import json
+
+
 class StixObjectOrStixRelationship:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             ... on StixObject {
                 id
                 standard_id
@@ -325,19 +328,23 @@
             }
             ... on DataSource {
                 name
                 description
             }
             ... on Case {
                 name
-            }            
+            }
             ... on StixCyberObservable {
                 observable_value
             }
             ... on StixCoreRelationship {
+                id
+                standard_id
+                entity_type
+                parent_types
                 createdBy {
                     ... on Identity {
                         id
                         standard_id
                         entity_type
                         parent_types
                         name
@@ -392,14 +399,18 @@
                 created
                 modified
                 description
                 start_time
                 stop_time
             }
             ... on StixSightingRelationship {
+                id
+                standard_id
+                entity_type
+                parent_types
                 createdBy {
                     ... on Identity {
                         id
                         standard_id
                         entity_type
                         parent_types
                         name
@@ -472,17 +483,17 @@
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
             self.opencti.app_logger.info(
                 "Reading StixObjectOrStixRelationship", {"id": id}
             )
             query = (
                 """
-                query StixObjectOrStixRelationship($id: String!) {
-                    stixObjectOrStixRelationship(id: $id) {
-                        """
+                    query StixObjectOrStixRelationship($id: String!) {
+                        stixObjectOrStixRelationship(id: $id) {
+                            """
                 + (
                     custom_attributes
                     if custom_attributes is not None
                     else self.properties
                 )
                 + """
                     }
@@ -492,7 +503,55 @@
             result = self.opencti.query(query, {"id": id})
             return self.opencti.process_multiple_fields(
                 result["data"]["stixObjectOrStixRelationship"]
             )
         else:
             self.opencti.app_logger.error("Missing parameters: id")
             return None
+
+    def list(self, **kwargs):
+        filters = kwargs.get("filters", None)
+        search = kwargs.get("search", None)
+        first = kwargs.get("first", 100)
+        after = kwargs.get("after", None)
+        with_pagination = kwargs.get("with_pagination", False)
+        custom_attributes = kwargs.get("customAttributes", None)
+
+        self.opencti.app_logger.info(
+            "Listing StixObjectOrStixRelationships with filters",
+            {"filters": json.dumps(filters)},
+        )
+        query = (
+            """
+                        query StixObjectOrStixRelationships($filters: FilterGroup, $search: String, $first: Int, $after: ID) {
+                            stixObjectOrStixRelationships(filters: $filters, search: $search, first: $first, after: $after) {
+                                edges {
+                                    node {
+                                        """
+            + (custom_attributes if custom_attributes is not None else self.properties)
+            + """
+                                }
+                            }
+                            pageInfo {
+                                startCursor
+                                endCursor
+                                hasNextPage
+                                hasPreviousPage
+                                globalCount
+                            }
+                        }
+                    }
+                """
+        )
+        result = self.opencti.query(
+            query,
+            {
+                "filters": filters,
+                "search": search,
+                "first": first,
+                "after": after,
+            },
+        )
+
+        return self.opencti.process_multiple(
+            result["data"]["stixObjectOrStixRelationships"], with_pagination
+        )
```

### Comparing `pycti-6.0.9/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-6.1.0/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_task.py` & `pycti-6.1.0/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_threat_actor.py` & `pycti-6.1.0/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_threat_actor_group.py` & `pycti-6.1.0/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_threat_actor_individual.py` & `pycti-6.1.0/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_tool.py` & `pycti-6.1.0/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_vocabulary.py` & `pycti-6.1.0/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/entities/opencti_vulnerability.py` & `pycti-6.1.0/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/utils/constants.py` & `pycti-6.1.0/pycti/utils/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     HOSTNAME = "Hostname"
     CRYPTOGRAPHIC_KEY = "Cryptographic-Key"
     CRYPTOCURRENCY_WALLET = "Cryptocurrency-Wallet"
     TEXT = "Text"
     USER_AGENT = "User-Agent"
     BANK_ACCOUNT = "Bank-Account"
     PHONE_NUMBER = "Phone-Number"
+    CREDENTIAL = "Credential"
+    TRACKING_NUMBER = "Tracking-Number"
     PAYMENT_CARD = "Payment-Card"
     MEDIA_CONTENT = "Media-Content"
     SIMPLE_OBSERVABLE = "Simple-Observable"
 
     @classmethod
     def has_value(cls, value):
         lower_attr = list(map(lambda x: x.lower(), cls._value2member_map_))
@@ -62,14 +64,15 @@
     def has_value(cls, value):
         lower_attr = list(map(lambda x: x.lower(), cls._value2member_map_))
         return value.lower() in lower_attr
 
 
 class ThreatActorTypes(Enum):
     THREAT_ACTOR_GROUP = "Threat-Actor-Group"
+    THREAT_ACTOR_INDIVIDUAL = "Threat-Actor-Individual"
 
     @classmethod
     def has_value(cls, value):
         lower_attr = list(map(lambda x: x.lower(), cls._value2member_map_))
         return value.lower() in lower_attr
 
 
@@ -122,15 +125,14 @@
     CC = "cc"
     BCC = "bcc"
     ENCAPSULATES = "encapsulates"
     OPENED_CONNECTION = "opened-connection"
     CHILD = "child"
     BODY_MULTIPART = "body-multipart"
     VALUES = "values"
-    LINKED = "x_opencti_linked-to"
     SERVICE_DDL = "service-dll"
     INSTALLED_SOFTWARE = "installed-software"
     RELATION_ANALYSIS_SCO = "analysis-sco"
 
     @classmethod
     def has_value(cls, value):
         lower_attr = list(map(lambda x: x.lower(), cls._value2member_map_))
@@ -260,14 +262,81 @@
 class CustomObservableText:
     """Text observable."""
 
     pass
 
 
 @CustomObservable(
+    "payment-card",
+    [
+        ("value", StringProperty(required=True)),
+        ("card_number", StringProperty(required=True)),
+        ("expiration_date", StringProperty(required=False)),
+        ("cvv", StringProperty(required=False)),
+        ("holder_name", StringProperty(required=False)),
+        ("spec_version", StringProperty(fixed="2.1")),
+        (
+            "object_marking_refs",
+            ListProperty(
+                ReferenceProperty(valid_types="marking-definition", spec_version="2.1")
+            ),
+        ),
+    ],
+    ["card_number"],
+)
+class CustomObservablePaymentCard:
+    """Payment card observable."""
+
+    pass
+
+
+@CustomObservable(
+    "bank-account",
+    [
+        ("value", StringProperty(required=True)),
+        ("iban", StringProperty(required=True)),
+        ("bic", StringProperty(required=False)),
+        ("account_number", StringProperty(required=False)),
+        ("spec_version", StringProperty(fixed="2.1")),
+        (
+            "object_marking_refs",
+            ListProperty(
+                ReferenceProperty(valid_types="marking-definition", spec_version="2.1")
+            ),
+        ),
+    ],
+    ["iban"],
+)
+class CustomObservableBankAccount:
+    """Bank Account observable."""
+
+    pass
+
+
+@CustomObservable(
+    "credential",
+    [
+        ("value", StringProperty(required=True)),
+        ("spec_version", StringProperty(fixed="2.1")),
+        (
+            "object_marking_refs",
+            ListProperty(
+                ReferenceProperty(valid_types="marking-definition", spec_version="2.1")
+            ),
+        ),
+    ],
+    ["value"],
+)
+class CustomObservableCredential:
+    """Credential observable."""
+
+    pass
+
+
+@CustomObservable(
     "cryptocurrency-wallet",
     [
         ("value", StringProperty(required=True)),
         ("spec_version", StringProperty(fixed="2.1")),
         (
             "object_marking_refs",
             ListProperty(
@@ -280,14 +349,54 @@
 class CustomObservableCryptocurrencyWallet:
     """Cryptocurrency wallet observable."""
 
     pass
 
 
 @CustomObservable(
+    "phone-number",
+    [
+        ("value", StringProperty(required=True)),
+        ("spec_version", StringProperty(fixed="2.1")),
+        (
+            "object_marking_refs",
+            ListProperty(
+                ReferenceProperty(valid_types="marking-definition", spec_version="2.1")
+            ),
+        ),
+    ],
+    ["value"],
+)
+class CustomObservablePhoneNumber:
+    """Phone number observable."""
+
+    pass
+
+
+@CustomObservable(
+    "tracking-number",
+    [
+        ("value", StringProperty(required=True)),
+        ("spec_version", StringProperty(fixed="2.1")),
+        (
+            "object_marking_refs",
+            ListProperty(
+                ReferenceProperty(valid_types="marking-definition", spec_version="2.1")
+            ),
+        ),
+    ],
+    ["value"],
+)
+class CustomObservableTrackingNumber:
+    """Tracking number observable."""
+
+    pass
+
+
+@CustomObservable(
     "user-agent",
     [
         ("value", StringProperty(required=True)),
         ("spec_version", StringProperty(fixed="2.1")),
         (
             "object_marking_refs",
             ListProperty(
```

### Comparing `pycti-6.0.9/pycti/utils/opencti_logger.py` & `pycti-6.1.0/pycti/utils/opencti_logger.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/utils/opencti_stix2.py` & `pycti-6.1.0/pycti/utils/opencti_stix2.py`

 * *Files 2% similar despite different names*

```diff
@@ -676,14 +676,17 @@
                             )
                             self.mapping_cache["marking_tlpclear"] = {
                                 "id": object_marking_ref_result["id"]
                             }
 
                         author = self.resolve_author(title)
                         report = self.opencti.report.create(
+                            id=self.opencti.report.generate_fixed_fake_id(
+                                title, published
+                            ),
                             name=title,
                             createdBy=author["id"] if author is not None else None,
                             objectMarking=[object_marking_ref_result["id"]],
                             externalReferences=[external_reference_id],
                             description=(
                                 external_reference["description"]
                                 if "description" in external_reference
@@ -784,14 +787,56 @@
             "object_refs": object_refs_ids,
             "granted_refs": granted_refs_ids,
             "sample_refs": sample_refs_ids,
             "external_references": external_references_ids,
             "reports": reports,
         }
 
+    def get_listers(self):
+        return {
+            "Stix-Core-Object": self.opencti.stix_core_object.list,
+            "Stix-Domain-Object": self.opencti.stix_domain_object.list,
+            "Administrative-Area": self.opencti.location.list,
+            "Attack-Pattern": self.opencti.attack_pattern.list,
+            "Campaign": self.opencti.campaign.list,
+            "Channel": self.opencti.channel.list,
+            "Event": self.opencti.event.list,
+            "Note": self.opencti.note.list,
+            "Observed-Data": self.opencti.observed_data.list,
+            "Opinion": self.opencti.opinion.list,
+            "Report": self.opencti.report.list,
+            "Grouping": self.opencti.grouping.list,
+            "Case-Incident": self.opencti.case_incident.list,
+            "Feedback": self.opencti.feedback.list,
+            "Case-Rfi": self.opencti.case_rfi.list,
+            "Case-Rft": self.opencti.case_rft.list,
+            "Task": self.opencti.task.list,
+            "Course-Of-Action": self.opencti.course_of_action.list,
+            "Data-Component": self.opencti.data_component.list,
+            "Data-Source": self.opencti.data_source.list,
+            "Identity": self.opencti.identity.list,
+            "Indicator": self.opencti.indicator.list,
+            "Infrastructure": self.opencti.infrastructure.list,
+            "Intrusion-Set": self.opencti.intrusion_set.list,
+            "Location": self.opencti.location.list,
+            "Language": self.opencti.language.list,
+            "Malware": self.opencti.malware.list,
+            "Malware-Analysis": self.opencti.malware_analysis.list,
+            "Threat-Actor": self.opencti.threat_actor_group.list,
+            "Threat-Actor-Group": self.opencti.threat_actor_group.list,
+            "Threat-Actor-Individual": self.opencti.threat_actor_individual.list,
+            "Tool": self.opencti.tool.list,
+            "Narrative": self.opencti.narrative.list,
+            "Vulnerability": self.opencti.vulnerability.list,
+            "Incident": self.opencti.incident.list,
+            "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.list,
+            "stix-sighting-relationship": self.opencti.stix_sighting_relationship.list,
+            "stix-core-relationship": self.opencti.stix_core_relationship.list,
+        }
+
     def get_readers(self):
         return {
             "Attack-Pattern": self.opencti.attack_pattern.read,
             "Campaign": self.opencti.campaign.read,
             "Case-Incident": self.opencti.case_incident.read,
             "Case-Rfi": self.opencti.case_rfi.read,
             "Case-Rft": self.opencti.case_rft.read,
@@ -831,14 +876,29 @@
             "Threat-Actor-Group": self.opencti.threat_actor_group.read,
             "Threat-Actor-Individual": self.opencti.threat_actor_individual.read,
             "Tool": self.opencti.tool.read,
             "Vocabulary": self.opencti.vocabulary.read,
             "Vulnerability": self.opencti.vulnerability.read,
         }
 
+    def get_reader(self, entity_type: str):
+        # Map types
+        if entity_type == "StixFile":
+            entity_type = "File"
+        if IdentityTypes.has_value(entity_type):
+            entity_type = "Identity"
+        if LocationTypes.has_value(entity_type):
+            entity_type = "Location"
+        if StixCyberObservableTypes.has_value(entity_type):
+            entity_type = "Stix-Cyber-Observable"
+        readers = self.get_readers()
+        return readers.get(
+            entity_type, lambda **kwargs: self.unknown_type({"type": entity_type})
+        )
+
     # endregion
 
     # region import
     def import_object(
         self, stix_object: Dict, update: bool = False, types: List = None
     ) -> Optional[List]:
         """import a stix2 object
@@ -1493,15 +1553,15 @@
         ):
             del entity["valid_from"]
 
         # Flatten
         if "tasks" in entity:
             del entity["tasks"]
 
-        if "status" in entity:
+        if "status" in entity and entity["status"] is not None:
             entity["x_opencti_workflow_id"] = entity["status"].get("id")
         if "status" in entity:
             del entity["status"]
 
         if "objectLabel" in entity and len(entity["objectLabel"]) > 0:
             entity["labels"] = []
             for object_label in entity["objectLabel"]:
@@ -1595,36 +1655,98 @@
         if "created_at" in entity:
             del entity["created_at"]
         if "updated_at" in entity:
             del entity["updated_at"]
 
         return {k: v for k, v in entity.items() if self.opencti.not_empty(v)}
 
+    def prepare_filters_export(self, id: str, access_filter: Dict = None) -> Dict:
+        if access_filter is not None:
+            return {
+                "mode": "and",
+                "filterGroups": [
+                    {
+                        "mode": "or",
+                        "filters": [
+                            {
+                                "key": "id",
+                                "values": [id],
+                            }
+                        ],
+                        "filterGroups": [],
+                    },
+                    access_filter,
+                ],
+                "filters": [],
+            }
+        else:
+            return {
+                "mode": "and",
+                "filterGroups": [
+                    {
+                        "mode": "or",
+                        "filters": [
+                            {
+                                "key": "id",
+                                "values": [id],
+                            }
+                        ],
+                        "filterGroups": [],
+                    },
+                ],
+                "filters": [],
+            }
+
     def prepare_export(
         self,
         entity: Dict,
         mode: str = "simple",
         max_marking_definition_entity: Dict = None,
+        main_filter: Dict = None,
+        access_filter: Dict = None,
         no_custom_attributes: bool = False,
     ) -> List:
-        if (
-            self.check_max_marking_definition(
-                max_marking_definition_entity,
-                entity["objectMarking"] if "objectMarking" in entity else [],
-            )
-            is False
-        ):
-            self.opencti.app_logger.info(
-                "Marking definitions are less than max definition, not exporting.",
-                {"type": entity["type"]},
-            )
-            return []
         result = []
         objects_to_get = []
         relations_to_get = []
+
+        # Container
+        if "objects" in entity and len(entity["objects"]) > 0:
+            del entity["objects"]
+            regarding_of_filter = {
+                "mode": "and",
+                "filterGroups": [],
+                "filters": [
+                    {
+                        "key": "regardingOf",
+                        "mode": "and",
+                        "operator": "eq",
+                        "values": [
+                            {"key": "id", "values": [entity["x_opencti_id"]]},
+                            {"key": "relationship_type", "values": ["object"]},
+                        ],
+                    }
+                ],
+            }
+            filter_groups = []
+            if regarding_of_filter is not None:
+                filter_groups.append(regarding_of_filter)
+            if access_filter is not None:
+                filter_groups.append(access_filter)
+            export_query_filter = {
+                "mode": "and",
+                "filterGroups": filter_groups,
+                "filters": [],
+            }
+            entity["objects"] = (
+                self.opencti.opencti_stix_object_or_stix_relationship.list(
+                    filters=export_query_filter
+                )
+            )
+
         # CreatedByRef
         if (
             not no_custom_attributes
             and "createdBy" in entity
             and entity["createdBy"] is not None
         ):
             created_by = self.generate_export(entity["createdBy"])
@@ -1728,15 +1850,15 @@
         # ObjectRefs
         if (
             not no_custom_attributes
             and "objects" in entity
             and len(entity["objects"]) > 0
         ):
             entity["object_refs"] = []
-            objects_to_get = entity["objects"]
+            objects_to_get = entity["objects"]  # To do differently
             for entity_object in entity["objects"]:
                 if (
                     entity["type"] == "report"
                     and entity_object["entity_type"]
                     not in [
                         "Note",
                         "Report",
@@ -1800,30 +1922,70 @@
             del entity["objects"]
             del entity["objectsIds"]
         # Stix Sighting Relationship
         if entity["type"] == "stix-sighting-relationship":
             entity["type"] = "sighting"
             entity["count"] = entity["attribute_count"]
             del entity["attribute_count"]
-            entity["sighting_of_ref"] = entity["from"]["standard_id"]
-            objects_to_get.append(entity["from"])
-            entity["where_sighted_refs"] = [entity["to"]["standard_id"]]
-            objects_to_get.append(entity["to"])
+            from_to_check = entity["from"]["id"]
+            relationships_from_filter = self.prepare_filters_export(
+                id=from_to_check, access_filter=access_filter
+            )
+            x = self.opencti.opencti_stix_object_or_stix_relationship.list(
+                filters=relationships_from_filter
+            )
+            if len(x) > 0:
+                entity["sighting_of_ref"] = entity["from"]["id"]
+                # handle from and to separately like Stix Core Relationship and call 2 requests
+                objects_to_get.append(
+                    entity["from"]
+                )  # what happen with unauthorized objects ?
+
+            to_to_check = [entity["to"]["id"]]
+            relationships_to_filter = self.prepare_filters_export(
+                id=to_to_check, access_filter=access_filter
+            )
+            y = self.opencti.opencti_stix_object_or_stix_relationship.list(
+                filters=relationships_to_filter
+            )
+            if len(y) > 0:
+                entity["where_sighted_refs"] = [entity["to"]["id"]]
+                objects_to_get.append(entity["to"])
+
             del entity["from"]
             del entity["to"]
         # Stix Core Relationship
         if "from" in entity or "to" in entity:
             entity["type"] = "relationship"
         if "from" in entity:
-            entity["source_ref"] = entity["from"]["standard_id"]
-            objects_to_get.append(entity["from"])
+            from_to_check = entity["from"]["id"]
+            relationships_from_filter = self.prepare_filters_export(
+                id=from_to_check, access_filter=access_filter
+            )
+            x = self.opencti.opencti_stix_object_or_stix_relationship.list(
+                filters=relationships_from_filter
+            )
+            if len(x) > 0:
+                entity["source_ref"] = entity["from"]["id"]
+                # handle from and to separately like Stix Core Relationship and call 2 requests
+                objects_to_get.append(
+                    entity["from"]
+                )  # what happen with unauthorized objects ?
             del entity["from"]
         if "to" in entity:
-            entity["target_ref"] = entity["to"]["standard_id"]
-            objects_to_get.append(entity["to"])
+            to_to_check = [entity["to"]["id"]]
+            relationships_to_filter = self.prepare_filters_export(
+                id=to_to_check, access_filter=access_filter
+            )
+            y = self.opencti.opencti_stix_object_or_stix_relationship.list(
+                filters=relationships_to_filter
+            )
+            if len(y) > 0:
+                entity["target_ref"] = entity["to"]["id"]
+                objects_to_get.append(entity["to"])
             del entity["to"]
         # Stix Domain Object
         if "attribute_abstract" in entity:
             entity["abstract"] = entity["attribute_abstract"]
             del entity["attribute_abstract"]
         # Stix Cyber Observable
         if "observable_value" in entity:
@@ -1858,15 +2020,15 @@
                     }
                 )
             del entity["importFiles"]
             del entity["importFilesIds"]
 
         # StixRefRelationship
         stix_nested_ref_relationships = self.opencti.stix_nested_ref_relationship.list(
-            fromId=entity["x_opencti_id"]
+            fromId=entity["x_opencti_id"], filters=access_filter
         )
         for stix_nested_ref_relationship in stix_nested_ref_relationships:
             if "standard_id" in stix_nested_ref_relationship["to"]:
                 # dirty fix because the sample and operating-system ref are not multiple for a Malware Analysis
                 # will be replaced by a proper toStix converter in the back
                 if not MultipleRefRelationship.has_value(
                     stix_nested_ref_relationship["relationship_type"]
@@ -1902,16 +2064,16 @@
 
         if mode == "simple":
             if no_custom_attributes:
                 del entity["x_opencti_id"]
             return result
         elif mode == "full":
             uuids = [entity["id"]]
-            for x in result:
-                uuids.append(x["id"])
+            for y in result:
+                uuids.append(y["id"])
             # Get extra refs
             for key in entity.keys():
                 if key.endswith("_ref"):
                     type = entity[key].split("--")[0]
                     if type in STIX_CYBER_OBSERVABLE_MAPPING:
                         objects_to_get.append(
                             {
@@ -1945,15 +2107,15 @@
                                     "id": value,
                                     "entity_type": "Stix-Domain-Object",
                                     "parent_types": ["Stix-Domain-Object"],
                                 }
                             )
             # Get extra relations (from AND to)
             stix_core_relationships = self.opencti.stix_core_relationship.list(
-                fromOrToId=entity["x_opencti_id"], getAll=True
+                fromOrToId=entity["x_opencti_id"], getAll=True, filters=access_filter
             )
             for stix_core_relationship in stix_core_relationships:
                 if self.check_max_marking_definition(
                     max_marking_definition_entity,
                     (
                         stix_core_relationship["objectMarking"]
                         if "objectMarking" in stix_core_relationship
@@ -1961,18 +2123,22 @@
                     ),
                 ):
                     objects_to_get.append(
                         stix_core_relationship["to"]
                         if stix_core_relationship["to"]["id"] != entity["x_opencti_id"]
                         else stix_core_relationship["from"]
                     )
-                    relation_object_data = self.prepare_export(
-                        self.generate_export(stix_core_relationship),
-                        "simple",
-                        max_marking_definition_entity,
+                    relation_object_data = (
+                        self.prepare_export(  # ICI -> remove max marking ?
+                            self.generate_export(stix_core_relationship),
+                            "simple",
+                            max_marking_definition_entity,
+                            main_filter,
+                            access_filter,
+                        )
                     )
                     relation_object_bundle = self.filter_objects(
                         uuids, relation_object_data
                     )
                     uuids = uuids + [x["id"] for x in relation_object_bundle]
                     result = result + relation_object_bundle
                 else:
@@ -1982,16 +2148,15 @@
                         {
                             "type": stix_core_relationship["entity_type"],
                             "id": stix_core_relationship["id"],
                         },
                     )
             # Get sighting
             stix_sighting_relationships = self.opencti.stix_sighting_relationship.list(
-                fromOrToId=entity["x_opencti_id"],
-                getAll=True,
+                fromOrToId=entity["x_opencti_id"], getAll=True, filters=access_filter
             )
             for stix_sighting_relationship in stix_sighting_relationships:
                 if self.check_max_marking_definition(
                     max_marking_definition_entity,
                     (
                         stix_sighting_relationship["objectMarking"]
                         if "objectMarking" in stix_sighting_relationship
@@ -2000,18 +2165,22 @@
                 ):
                     objects_to_get.append(
                         stix_sighting_relationship["to"]
                         if stix_sighting_relationship["to"]["id"]
                         != entity["x_opencti_id"]
                         else stix_sighting_relationship["from"]
                     )
-                    relation_object_data = self.prepare_export(
-                        self.generate_export(stix_sighting_relationship),
-                        "simple",
-                        max_marking_definition_entity,
+                    relation_object_data = (
+                        self.prepare_export(  # ICI -> remove max marking ?
+                            self.generate_export(stix_sighting_relationship),
+                            "simple",
+                            max_marking_definition_entity,
+                            main_filter,
+                            access_filter,
+                        )
                     )
                     relation_object_bundle = self.filter_objects(
                         uuids, relation_object_data
                     )
                     uuids = uuids + [x["id"] for x in relation_object_bundle]
                     result = result + relation_object_bundle
                 else:
@@ -2046,30 +2215,43 @@
 
                 do_read = reader.get(
                     entity_object["entity_type"],
                     lambda **kwargs: self.unknown_type(
                         {"type": entity_object["entity_type"]}
                     ),
                 )
-                entity_object_data = do_read(id=entity_object["id"])
+                entity_object_data = do_read(
+                    id=entity_object["id"], filters=access_filter
+                )
                 if entity_object_data is not None:
                     stix_entity_object = self.prepare_export(
                         self.generate_export(entity_object_data),
                         "simple",
                         max_marking_definition_entity,
+                        main_filter,
+                        access_filter,
                     )
                     # Add to result
                     entity_object_bundle = self.filter_objects(
                         uuids, stix_entity_object
                     )
                     uuids = uuids + [x["id"] for x in entity_object_bundle]
                     result = result + entity_object_bundle
-            for relation_object in relations_to_get:
+            for (
+                relation_object
+            ) in relations_to_get:  # never appended after initialization
+
+                def find_relation_object_data(current_relation_object):
+                    return current_relation_object.id == relation_object["id"]
+
                 relation_object_data = self.prepare_export(
-                    self.opencti.stix_core_relationship.read(id=relation_object["id"])
+                    filter(
+                        find_relation_object_data,
+                        self.opencti.stix_core_relationship.list(filters=access_filter),
+                    )
                 )
                 relation_object_bundle = self.filter_objects(
                     uuids, relation_object_data
                 )
                 uuids = uuids + [x["id"] for x in relation_object_bundle]
                 result = result + relation_object_bundle
 
@@ -2131,23 +2313,20 @@
             return []
 
     def export_entity(
         self,
         entity_type: str,
         entity_id: str,
         mode: str = "simple",
+        main_filter: Dict = None,
+        access_filter: Dict = None,
         max_marking_definition: Dict = None,
         no_custom_attributes: bool = False,
         only_entity: bool = False,
     ) -> Dict:
-        max_marking_definition_entity = (
-            self.opencti.marking_definition.read(id=max_marking_definition)
-            if max_marking_definition is not None
-            else None
-        )
         bundle = {
             "type": "bundle",
             "id": "bundle--" + str(uuid.uuid4()),
             "objects": [],
         }
 
         if entity_type == "StixFile":
@@ -2155,47 +2334,47 @@
 
         # Map types
         if IdentityTypes.has_value(entity_type):
             entity_type = "Identity"
         if LocationTypes.has_value(entity_type):
             entity_type = "Location"
 
-        # Reader
-        reader = self.get_readers()
-        if StixCyberObservableTypes.has_value(entity_type):
-            entity_type = "Stix-Cyber-Observable"
-        do_read = reader.get(
+        # Lister
+        listers = self.get_listers()
+        do_list = listers.get(
             entity_type, lambda **kwargs: self.unknown_type({"type": entity_type})
         )
-        entity = do_read(id=entity_id)
+        entity = do_list(filters=main_filter)[0]
         if entity is None:
             self.opencti.app_logger.error(
                 "Cannot export entity (not found)", {"id": entity_id}
             )
             return bundle
         entity_standard_id = entity["standard_id"]
         stix_objects = self.prepare_export(
             self.generate_export(entity, no_custom_attributes),
             mode,
-            max_marking_definition_entity,
+            None,
+            main_filter,
+            access_filter,
             no_custom_attributes,
         )
         if stix_objects is not None:
             bundle["objects"].extend(stix_objects)
         if only_entity:
             return [e for e in bundle["objects"] if e.get("id") == entity_standard_id][
                 0
             ]
         return bundle
 
     def export_entities_list(
         self,
         entity_type: str,
         search: Dict = None,
-        filters: List = None,
+        filters: Dict = None,
         orderBy: str = None,
         orderMode: str = None,
         getAll: bool = True,
     ) -> Dict:
         if IdentityTypes.has_value(entity_type):
             entity_type = "Identity"
 
@@ -2260,82 +2439,103 @@
             getAll=getAll,
         )
 
     def export_list(
         self,
         entity_type: str,
         search: Dict = None,
-        filters: List = None,
+        filters: Dict = None,
         order_by: str = None,
         order_mode: str = None,
         mode: str = "simple",
-        max_marking_definition: Dict = None,
+        main_filter: Dict = None,
+        access_filter: Dict = None,
     ) -> Dict:
-        max_marking_definition_entity = (
-            self.opencti.marking_definition.read(id=max_marking_definition)
-            if max_marking_definition is not None
-            else None
-        )
         bundle = {
             "type": "bundle",
             "id": "bundle--" + str(uuid.uuid4()),
             "objects": [],
         }
+        filterGroups = []
+        if filters is not None:
+            filterGroups.append(filters)
+        if access_filter is not None:
+            filterGroups.append(access_filter)
+        export_query_filter = {
+            "mode": "and",
+            "filterGroups": filterGroups,
+            "filters": [],
+        }
         entities_list = self.export_entities_list(
             entity_type=entity_type,
             search=search,
-            filters=filters,
+            filters=export_query_filter,
             orderBy=order_by,
             orderMode=order_mode,
             getAll=True,
         )
         if entities_list is not None:
             uuids = []
             for entity in entities_list:
                 entity_bundle = self.prepare_export(
                     self.generate_export(entity),
                     mode,
-                    max_marking_definition_entity,
+                    None,
+                    main_filter,
+                    access_filter,
                 )
                 if entity_bundle is not None:
                     entity_bundle_filtered = self.filter_objects(uuids, entity_bundle)
                     for x in entity_bundle_filtered:
                         uuids.append(x["id"])
                     bundle["objects"] = bundle["objects"] + entity_bundle_filtered
         return bundle
 
     def export_selected(
         self,
         entities_list: [str],
         mode: str = "simple",
-        max_marking_definition: Dict = None,
+        main_filter: Dict = None,
+        access_filter: Dict = None,
     ) -> Dict:
-        max_marking_definition_entity = (
-            self.opencti.marking_definition.read(id=max_marking_definition)
-            if max_marking_definition is not None
-            else None
+
+        entity_data_sdo = self.opencti.stix_domain_object.list(filters=main_filter)
+        entity_data_sco = self.opencti.stix_cyber_observable.list(filters=main_filter)
+        entity_data_scr = self.opencti.stix_core_relationship.list(filters=main_filter)
+        entity_data_ssr = self.opencti.stix_sighting_relationship.list(
+            filters=main_filter
+        )
+
+        entities_list = (
+            entity_data_sdo + entity_data_sco + entity_data_scr + entity_data_ssr
         )
         bundle = {
             "type": "bundle",
             "id": "bundle--" + str(uuid.uuid4()),
             "objects": [],
         }
+
         if entities_list is not None:
             uuids = []
             for entity in entities_list:
                 entity_bundle = self.prepare_export(
                     self.generate_export(entity),
                     mode,
-                    max_marking_definition_entity,
+                    None,
+                    main_filter,
+                    access_filter,
                 )
                 if entity_bundle is not None:
                     entity_bundle_filtered = self.filter_objects(uuids, entity_bundle)
                     for x in entity_bundle_filtered:
                         uuids.append(x["id"])
-                    bundle["objects"] = bundle["objects"] + entity_bundle_filtered
+                    bundle["objects"] = (
+                        bundle["objects"] + entity_bundle_filtered
+                    )  # unsupported operand type(s) for +: 'dict' and 'list'
+
         return bundle
 
     def import_bundle(
         self,
         stix_bundle: Dict,
         update: bool = False,
         types: List = None,
```

### Comparing `pycti-6.0.9/pycti/utils/opencti_stix2_splitter.py` & `pycti-6.1.0/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/utils/opencti_stix2_update.py` & `pycti-6.1.0/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti/utils/opencti_stix2_utils.py` & `pycti-6.1.0/pycti/utils/opencti_stix2_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,30 +3,39 @@
 from stix2 import EqualityComparisonExpression, ObjectPath, ObservationExpression
 
 STIX_CYBER_OBSERVABLE_MAPPING = {
     "autonomous-system": "Autonomous-System",
     "directory": "Directory",
     "domain-name": "Domain-Name",
     "email-addr": "Email-Addr",
-    "file": "StixFile",
     "email-message": "Email-Message",
+    "email-mime-part-type": "Email-Mime-Part-Type",
+    "artifact": "Artifact",
+    "file": "StixFile",
+    "x509-certificate": "X509-Certificate",
     "ipv4-addr": "IPv4-Addr",
     "ipv6-addr": "IPv6-Addr",
     "mac-addr": "Mac-Addr",
     "mutex": "Mutex",
     "network-traffic": "Network-Traffic",
     "process": "Process",
     "software": "Software",
     "url": "Url",
     "user-account": "User-Account",
     "windows-registry-key": "Windows-Registry-Key",
     "windows-registry-value-type": "Windows-Registry-Value-Type",
     "hostname": "Hostname",
+    "cryptographic-key": "Cryptographic-Key",
+    "cryptocurrency-wallet": "Cryptocurrency-Wallet",
+    "text": "Text",
+    "user-agent": "User-Agent",
     "bank-account": "Bank-Account",
     "phone-number": "Phone-Number",
+    "credential": "Credential",
+    "tracking-number": "Tracking-Number",
     "payment-card": "Payment-Card",
     "media-content": "Media-Content",
 }
 
 PATTERN_MAPPING = {
     "Autonomous-System": ["number"],
     "Directory": ["path"],
@@ -50,14 +59,16 @@
     "User-Account": ["acount_login"],
     "Windows-Registry-Key": ["key"],
     "Windows-Registry-Value-Type": ["name"],
     "Hostname": ["value"],
     "Bank-Account": ["iban"],
     "Phone-Number": ["value"],
     "Payment-Card": ["card_number"],
+    "Tracking-Number": ["value"],
+    "Credential": ["value"],
     "Media-Content": ["url"],
 }
 
 OBSERVABLES_VALUE_INT = [
     "Autonomous-System.number",
     "Network-Traffic.dst_port",
     "Process.pid",
```

### Comparing `pycti-6.0.9/pycti.egg-info/PKG-INFO` & `pycti-6.1.0/pycti.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.0.9
+Version: 6.1.0
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,33 +25,33 @@
 Requires-Dist: pika~=1.3.1
 Requires-Dist: python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
 Requires-Dist: prometheus-client~=0.20.0
 Requires-Dist: python-magic-bin~=0.4.14; sys_platform == "win32"
 Requires-Dist: python_json_logger~=2.0.4
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: requests~=2.31.0
-Requires-Dist: setuptools~=69.2.0
+Requires-Dist: setuptools~=69.5.1
 Requires-Dist: filigran-sseclient~=1.0.0
 Requires-Dist: stix2~=3.0.1
 Requires-Dist: cachetools~=5.3.0
 Provides-Extra: dev
-Requires-Dist: black~=24.3.0; extra == "dev"
+Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
 Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 Requires-Dist: pytest-cases~=3.8.0; extra == "dev"
 Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
 Requires-Dist: pytest_randomly~=3.15.0; extra == "dev"
-Requires-Dist: pytest~=8.1.1; extra == "dev"
+Requires-Dist: pytest~=8.2.0; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
 Requires-Dist: wheel~=0.43.0; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: autoapi~=2.0.1; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints~=2.0.0; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints~=2.1.0; extra == "doc"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "doc"
 
 # OpenCTI client for Python
 
 [![Website](https://img.shields.io/badge/website-opencti.io-blue.svg)](https://opencti.io)
 [![CircleCI](https://circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://circleci.com/gh/OpenCTI-Platform/client-python/tree/master)
 [![readthedocs](https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)](https://opencti-client-for-python.readthedocs.io/en/latest/)
```

### Comparing `pycti-6.0.9/pycti.egg-info/SOURCES.txt` & `pycti-6.1.0/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/pycti.egg-info/requires.txt` & `pycti-6.1.0/pycti.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 datefinder~=0.7.3
 pika~=1.3.1
 prometheus-client~=0.20.0
 python_json_logger~=2.0.4
 pyyaml~=6.0
 requests~=2.31.0
-setuptools~=69.2.0
+setuptools~=69.5.1
 filigran-sseclient~=1.0.0
 stix2~=3.0.1
 cachetools~=5.3.0
 
 [:sys_platform == "linux" or sys_platform == "darwin"]
 python-magic~=0.4.27
 
 [:sys_platform == "win32"]
 python-magic-bin~=0.4.14
 
 [dev]
-black~=24.3.0
+black~=24.4.0
 build~=1.2.1
 isort~=5.13.0
 types-pytz~=2024.1.0.20240203
 pre-commit~=3.7.0
 pytest-cases~=3.8.0
 pytest-cov~=5.0.0
 pytest_randomly~=3.15.0
-pytest~=8.1.1
+pytest~=8.2.0
 types-python-dateutil~=2.9.0
 wheel~=0.43.0
 
 [doc]
 autoapi~=2.0.1
-sphinx-autodoc-typehints~=2.0.0
+sphinx-autodoc-typehints~=2.1.0
 sphinx-rtd-theme~=2.0.0
```

### Comparing `pycti-6.0.9/pyproject.toml` & `pycti-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-6.0.9/setup.cfg` & `pycti-6.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -36,34 +36,34 @@
 	pika~=1.3.1
 	python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
 	prometheus-client~=0.20.0
 	python-magic-bin~=0.4.14; sys_platform == "win32"
 	python_json_logger~=2.0.4
 	pyyaml~=6.0
 	requests~=2.31.0
-	setuptools~=69.2.0
+	setuptools~=69.5.1
 	filigran-sseclient~=1.0.0
 	stix2~=3.0.1
 	cachetools~=5.3.0
 
 [options.extras_require]
 dev = 
-	black~=24.3.0
+	black~=24.4.0
 	build~=1.2.1
 	isort~=5.13.0
 	types-pytz~=2024.1.0.20240203
 	pre-commit~=3.7.0
 	pytest-cases~=3.8.0
 	pytest-cov~=5.0.0
 	pytest_randomly~=3.15.0
-	pytest~=8.1.1
+	pytest~=8.2.0
 	types-python-dateutil~=2.9.0
 	wheel~=0.43.0
 doc = 
 	autoapi~=2.0.1
-	sphinx-autodoc-typehints~=2.0.0
+	sphinx-autodoc-typehints~=2.1.0
 	sphinx-rtd-theme~=2.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

