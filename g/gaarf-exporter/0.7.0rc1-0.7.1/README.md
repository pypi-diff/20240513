# Comparing `tmp/gaarf-exporter-0.7.0rc1.tar.gz` & `tmp/gaarf-exporter-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaarf-exporter-0.7.0rc1.tar", last modified: Mon Mar 25 13:31:25 2024, max compression
+gzip compressed data, was "gaarf-exporter-0.7.1.tar", last modified: Mon May 13 11:19:49 2024, max compression
```

## Comparing `gaarf-exporter-0.7.0rc1.tar` & `gaarf-exporter-0.7.1.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5742 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5270 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/gaarf_exporter/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1287 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/alert.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/alert_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1971 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/bootstrap.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    28882 2024-03-24 05:05:19.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3687 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/config.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7548 2024-03-24 07:22:06.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/main.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2799 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/query_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      908 2024-03-15 19:34:24.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/search_collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     8745 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/target.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/util.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5742 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      775 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       56 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1556 2024-03-25 13:18:51.000000 gaarf-exporter-0.7.0rc1/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-0.7.0rc1/tests/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3950 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/conftest.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_alerts.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2670 2024-03-21 10:06:54.000000 gaarf-exporter-0.7.0rc1/tests/test_collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2349 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_config.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3525 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_query_element.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    12589 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_target.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.139074 gaarf-exporter-0.7.1/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6912 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6443 2024-03-26 12:03:46.000000 gaarf-exporter-0.7.1/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/gaarf_exporter/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1287 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/alert.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/alert_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2395 2024-05-02 16:45:02.000000 gaarf-exporter-0.7.1/gaarf_exporter/bootstrap.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    35232 2024-05-13 11:14:49.000000 gaarf-exporter-0.7.1/gaarf_exporter/collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4093 2024-05-09 20:50:51.000000 gaarf-exporter-0.7.1/gaarf_exporter/config.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7971 2024-05-13 11:13:48.000000 gaarf-exporter-0.7.1/gaarf_exporter/main.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2825 2024-05-08 08:46:57.000000 gaarf-exporter-0.7.1/gaarf_exporter/query_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      908 2024-03-15 19:34:24.000000 gaarf-exporter-0.7.1/gaarf_exporter/search_collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    13737 2024-05-13 11:13:48.000000 gaarf-exporter-0.7.1/gaarf_exporter/target.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6912 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      885 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       56 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-05-13 11:19:49.139074 gaarf-exporter-0.7.1/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1552 2024-05-10 05:03:01.000000 gaarf-exporter-0.7.1/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:38:01.000000 gaarf-exporter-0.7.1/tests/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/tests/end-to-end/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/end-to-end/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      504 2024-05-13 11:14:49.000000 gaarf-exporter-0.7.1/tests/end-to-end/test_gaarf_exporter.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/tests/unit/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/unit/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/unit/test_alerts.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3854 2024-05-13 11:13:48.000000 gaarf-exporter-0.7.1/tests/unit/test_collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3724 2024-05-08 13:54:33.000000 gaarf-exporter-0.7.1/tests/unit/test_config.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/unit/test_exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3525 2024-05-08 08:46:57.000000 gaarf-exporter-0.7.1/tests/unit/test_query_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    20353 2024-05-09 20:50:51.000000 gaarf-exporter-0.7.1/tests/unit/test_target.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/unit/test_util.py
```

### Comparing `gaarf-exporter-0.7.0rc1/PKG-INFO` & `gaarf-exporter-0.7.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: gaarf-exporter
-Version: 0.7.0rc1
-Author: Google Inc. (gTech gPS CSE team)
-Author-email: no-reply@google.com
-License: Apache 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-
 # gaarf exporter
 
 Prometheus exporter for Google Ads metrics with customizable metrics collectors.
 
 ## Installation and usage
 
 ### Locally
@@ -46,15 +33,18 @@
 
 ```
 By default it will start http_server on `localhost:8000` and will push some basic metrics to it.
 
 ### Customization
 
 * `--ads-config` - path to `google-ads.yaml`
+  >  `ads-config` can be taken from local storage or remote storage (gs, s3, azure, ssh, stfp, scrp, hdfs, webhdfs).
 * `--config` - path to `gaarf_exporter.yaml`
+  >  `config` can be taken from local storage or remote storage (same as `--ads-config`).
+* `--collectors` - names of one or more [collectors](#collectors) (separated by comma).
 * `--http_server.address` - address of your http server (`localhost` by default)
 * `--http_server.port` - port of your http server (`8000` by default)
 * `--pushgateway.address` - address of your pushgateway service (`None` by default)
 * `--pushgateway.port` - port of your pushgateway (`None` by default)
 * `--delay-minutes` - delay in minutes between scrapings (`15` by default)
 
 #### Customizing with macros:
@@ -67,38 +57,43 @@
 * `--macro.end_date=:YYYYMMDD-M`, where `N` is number of days starting from today
 
 It will add an additional metric to be exposed to Prometheus `*_n_days` (i.e.
 `googleads_clicks_n_days`.
 
 ### Collectors
 
-You can specify collectors with `--collectors <collector_name>` CLI argument. Some collectors available by default, other you need to specify explicitly.
+You can specify collectors with `--collectors <collector_name>` CLI argument. Some collectors available by default, other you need to specify explicitly.\
+There are two types of collectors - *registry* (contains other collectors grouped logically) and *collectors* themselves.
 
 #### `default` registry.
 
 * `performance` - extracts *clicks*, *impressions*, *cost*, *conversions* on by *ad_network* and *ad_group_id*
 * `disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *ad_group_id* and *ad_id* only for not approved ads
 * `conversion_action` - extracts *all_conversions* by *conversion_id* and *account_id*
 * `mapping` - performance mapping between *ad_group_id*, *ad_group_name*, *campaign_id*, *campaign_name,* *campaign_status*, *account_id*, *account_name*
 
 #### *disapprovals* registry.
 
 * `ad_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *ad_group_id* and *ad_id* only for not approved ads
 * `ad_group_ad_asset_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *ad_group_id* and *asset_id* only for enabled assets.
 * `sitelink_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *asset_id*,   *sitelink_title* and both sitelink descriptions only for not approved sitelinks.
+* `pmax_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *asset_id*,   *asset_group_id* for active asset group assets.
 
 #### *app* registry.
 
 * `app_campaign_mapping` - performs mapping between *campaign_id*, *app_id*, *app_store*, *and bidding_strategy* only for active campaigns.
+* `app_asset_mapping` - performs mapping between *asset_id* and its type, source, and content (*name*, *text*, *video_id*) only for app assets (HTML5, TEXT, IMAGE, VIDEO).
 * `asset_performance` - extracts *clicks*, *impressions*, *cost*, *installs*, *inapps*, and *conversions_value* by *ad_group_id*, *ad_network* and *asset_id*
 * `asset_perf_label` - extracts *performance_label* by *ad_group_id* and *asset_id*
 
 #### *pmax* registry.
 
 * `pmax_mapping` - performs mapping between *asset_group_id*, *asset_group_name*, and meta information on campaign and account only for active campaigns and enabled asset groups.
+* `pmax_performance` - extracts *clicks*, *impressions*, *cost*, *installs*, *inapps*, and *conversions_value* by *asset_group_id*.
+* `pmax_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *asset_id*,   *asset_group_id* for active asset group assets.
 
 #### *search* registry.
 
 * `search_terms` - extracts *clicks*, *impressions*, *cost*, *conversions* on by *search_term* and *ad_group_id*
 * `search_terms_conversion_split` - extracts *all_conversions* by *search_term* and *conversion_id* on *ad_group_id* level
 * `keywords` - extracts *clicks*, *impressions*, *cost*, *conversions*, and *historical auality_score*  by *keyword* and *match_type* on ad_group level.
 * `keywords_conversion_split` - extracts *all_conversions* by *keyword* and *match_type* on ad_group level.
@@ -118,10 +113,12 @@
 #### *geo* registry.
 
 * `user_location` - extracts *clicks*, *impressions*, *cost*, *conversions* by *country_id* and *campaign_id* only for active campaigns.
 * `user_location_conversion_split` - extracts *all_conversions* by *country_id*  and *campaign_id*only for active campaigns.
 
 #### collectors without registry.
 
-* `bid_budgets` - extracts current values of bid (target_cpa, target_roas) and budget
+* `bid_budgets` - extracts current values of bid (target_cpa, target_roas) and campaign budgets.
+* `bids` - extracts current values of bid (target_cpa, target_roas).
+* `budgets` - extracts current values of campaign budgets.
 * `account_status` - extracts *customer_status* for each account.
 * `campaign_service_status` - extracts *primary_status* for each campaign.
```

### Comparing `gaarf-exporter-0.7.0rc1/README.md` & `gaarf-exporter-0.7.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: gaarf-exporter
+Version: 0.7.1
+Author: Google Inc. (gTech gPS CSE team)
+Author-email: no-reply@google.com
+License: Apache 2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Description-Content-Type: text/markdown
+
 # gaarf exporter
 
 Prometheus exporter for Google Ads metrics with customizable metrics collectors.
 
 ## Installation and usage
 
 ### Locally
@@ -33,15 +46,18 @@
 
 ```
 By default it will start http_server on `localhost:8000` and will push some basic metrics to it.
 
 ### Customization
 
 * `--ads-config` - path to `google-ads.yaml`
+  >  `ads-config` can be taken from local storage or remote storage (gs, s3, azure, ssh, stfp, scrp, hdfs, webhdfs).
 * `--config` - path to `gaarf_exporter.yaml`
+  >  `config` can be taken from local storage or remote storage (same as `--ads-config`).
+* `--collectors` - names of one or more [collectors](#collectors) (separated by comma).
 * `--http_server.address` - address of your http server (`localhost` by default)
 * `--http_server.port` - port of your http server (`8000` by default)
 * `--pushgateway.address` - address of your pushgateway service (`None` by default)
 * `--pushgateway.port` - port of your pushgateway (`None` by default)
 * `--delay-minutes` - delay in minutes between scrapings (`15` by default)
 
 #### Customizing with macros:
@@ -54,38 +70,43 @@
 * `--macro.end_date=:YYYYMMDD-M`, where `N` is number of days starting from today
 
 It will add an additional metric to be exposed to Prometheus `*_n_days` (i.e.
 `googleads_clicks_n_days`.
 
 ### Collectors
 
-You can specify collectors with `--collectors <collector_name>` CLI argument. Some collectors available by default, other you need to specify explicitly.
+You can specify collectors with `--collectors <collector_name>` CLI argument. Some collectors available by default, other you need to specify explicitly.\
+There are two types of collectors - *registry* (contains other collectors grouped logically) and *collectors* themselves.
 
 #### `default` registry.
 
 * `performance` - extracts *clicks*, *impressions*, *cost*, *conversions* on by *ad_network* and *ad_group_id*
 * `disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *ad_group_id* and *ad_id* only for not approved ads
 * `conversion_action` - extracts *all_conversions* by *conversion_id* and *account_id*
 * `mapping` - performance mapping between *ad_group_id*, *ad_group_name*, *campaign_id*, *campaign_name,* *campaign_status*, *account_id*, *account_name*
 
 #### *disapprovals* registry.
 
 * `ad_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *ad_group_id* and *ad_id* only for not approved ads
 * `ad_group_ad_asset_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *ad_group_id* and *asset_id* only for enabled assets.
 * `sitelink_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *asset_id*,   *sitelink_title* and both sitelink descriptions only for not approved sitelinks.
+* `pmax_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *asset_id*,   *asset_group_id* for active asset group assets.
 
 #### *app* registry.
 
 * `app_campaign_mapping` - performs mapping between *campaign_id*, *app_id*, *app_store*, *and bidding_strategy* only for active campaigns.
+* `app_asset_mapping` - performs mapping between *asset_id* and its type, source, and content (*name*, *text*, *video_id*) only for app assets (HTML5, TEXT, IMAGE, VIDEO).
 * `asset_performance` - extracts *clicks*, *impressions*, *cost*, *installs*, *inapps*, and *conversions_value* by *ad_group_id*, *ad_network* and *asset_id*
 * `asset_perf_label` - extracts *performance_label* by *ad_group_id* and *asset_id*
 
 #### *pmax* registry.
 
 * `pmax_mapping` - performs mapping between *asset_group_id*, *asset_group_name*, and meta information on campaign and account only for active campaigns and enabled asset groups.
+* `pmax_performance` - extracts *clicks*, *impressions*, *cost*, *installs*, *inapps*, and *conversions_value* by *asset_group_id*.
+* `pmax_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *asset_id*,   *asset_group_id* for active asset group assets.
 
 #### *search* registry.
 
 * `search_terms` - extracts *clicks*, *impressions*, *cost*, *conversions* on by *search_term* and *ad_group_id*
 * `search_terms_conversion_split` - extracts *all_conversions* by *search_term* and *conversion_id* on *ad_group_id* level
 * `keywords` - extracts *clicks*, *impressions*, *cost*, *conversions*, and *historical auality_score*  by *keyword* and *match_type* on ad_group level.
 * `keywords_conversion_split` - extracts *all_conversions* by *keyword* and *match_type* on ad_group level.
@@ -105,10 +126,12 @@
 #### *geo* registry.
 
 * `user_location` - extracts *clicks*, *impressions*, *cost*, *conversions* by *country_id* and *campaign_id* only for active campaigns.
 * `user_location_conversion_split` - extracts *all_conversions* by *country_id*  and *campaign_id*only for active campaigns.
 
 #### collectors without registry.
 
-* `bid_budgets` - extracts current values of bid (target_cpa, target_roas) and budget
+* `bid_budgets` - extracts current values of bid (target_cpa, target_roas) and campaign budgets.
+* `bids` - extracts current values of bid (target_cpa, target_roas).
+* `budgets` - extracts current values of campaign budgets.
 * `account_status` - extracts *customer_status* for each account.
 * `campaign_service_status` - extracts *primary_status* for each campaign.
```

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter/alert.py` & `gaarf-exporter-0.7.1/gaarf_exporter/alert.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter/alert_elements.py` & `gaarf-exporter-0.7.1/gaarf_exporter/alert_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter/bootstrap.py` & `gaarf-exporter-0.7.1/gaarf_exporter/bootstrap.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,47 +7,60 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-'''Module for building necessary dependencies to run Gaarf Exporter.'''
+"""Module for building necessary dependencies to run Gaarf Exporter."""
 from __future__ import annotations
 
+import smart_open
 import yaml
-from gaarf.api_clients import BaseClient
-from gaarf.api_clients import GoogleAdsApiClient
-from gaarf.query_executor import AdsReportFetcher
-from smart_open import open
+from gaarf import api_clients
+from gaarf import query_executor
 
 
 def inject_dependencies(
-    api_version: str,
+    api_version: str | None = None,
     ads_config_path: str | None = None,
     account: str | None = None
-) -> dict[str, AdsReportFetcher | list[str] | bool | None]:
+) -> dict[str, query_executor.AdsReportFetcher | list[str] | bool | None]:
+  """Creates necessary dependencies to run export data.
+
+  Args:
+    api_version: Version of Google Ads API.
+    ads_config_path: Path to google-ads.yaml file.
+    account: Google Ads manager or child account.
+
+  Returns:
+    A dictionary with injected dependencies.
+
+  Raises:
+    ValueError: If there's no Google Ads account to get data from.
+  """
+  api_version = api_version or api_clients.GOOGLE_ADS_API_VERSION
   if not account or not ads_config_path:
-    client = BaseClient(api_version)
-    report_fetcher = AdsReportFetcher(client)
+    client = api_clients.BaseClient(api_version)
+    report_fetcher = query_executor.AdsReportFetcher(client)
     accounts = None
     return {
         'report_fetcher': report_fetcher,
         'accounts': accounts,
         'convert_fake_report': True
     }
-  with open(ads_config_path, 'r', encoding='utf-8') as f:
+  with smart_open.open(ads_config_path, 'r', encoding='utf-8') as f:
     google_ads_config_dict = yaml.safe_load(f)
   if not account:
     account = google_ads_config_dict.get('login_customer_id')
   if not account:
     raise ValueError('No account found, please specify via --account CLI flag'
                      'or add as login_customer_id in google-ads.yaml')
-  client = GoogleAdsApiClient(
+  client = api_clients.GoogleAdsApiClient(
       config_dict=google_ads_config_dict, version=api_version)
-  report_fetcher = AdsReportFetcher(client)
+  report_fetcher = query_executor.AdsReportFetcher(client)
   accounts = report_fetcher.expand_mcc(account)
   return {
       'report_fetcher': report_fetcher,
       'accounts': accounts,
       'convert_fake_report': False
   }
```

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter/config.py` & `gaarf-exporter-0.7.1/gaarf_exporter/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-'''Module for defining gaarf GaarfExporter config to hold queries.'''
+"""Module for defining gaarf GaarfExporter config to hold queries."""
 from __future__ import annotations
 
 import functools
 from collections.abc import Sequence
 
 import yaml
 
@@ -41,31 +41,46 @@
   @functools.cached_property
   def targets(self):
     """Converts targets passed during init to regular and service targets."""
     targets = target.targets_similarity_check(self._targets)
     has_service_target = any(
         [isinstance(target_, target.ServiceTarget) for target_ in targets])
     if not has_service_target:
-      min_level = target.TargetLevel(
-          min([target_.level.value for target_ in targets]))
-      default_service_target = target.create_default_service_target(min_level)
-      targets.append(default_service_target)
+      valid_target_levels = [
+          target_.level
+          for target_ in targets
+          if target_.level != target.TargetLevel.UNKNOWN
+      ]
+      if valid_target_levels:
+        default_service_target = target.create_default_service_target(
+            min(valid_target_levels))
+        targets.append(default_service_target)
     return targets
 
   @property
+  def queries(self) -> dict[str, dict[str, str]]:
+    """Mapping between all target name to its text and suffix."""
+    return {
+        target_.name: {
+            'query': target_.query,
+            'suffix': target_.suffix
+        } for target_ in self.targets
+    }
+
+  @property
   def regular_targets(self) -> dict[str, target.Target]:
     """Mapping between name of non-service target to itself."""
     return {
         target_.name: target_
         for target_ in self.targets
         if not isinstance(target_, target.ServiceTarget)
     }
 
   @property
-  def queries(self) -> dict[str, dict[str, str]]:
+  def regular_queries(self) -> dict[str, dict[str, str]]:
     """Mapping between regular target name to its text and suffix."""
     return {
         name: {
             'query': target_.query,
             'suffix': target_.suffix
         } for name, target_ in self.regular_targets.items()
     }
```

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter/exporter.py` & `gaarf-exporter-0.7.1/gaarf_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter/main.py` & `gaarf-exporter-0.7.1/gaarf_exporter/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,134 +5,149 @@
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and limitations under the License.
-'''Entrypoint for running GaarfExporter.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""Entrypoint for running GaarfExporter.
 
 Defines GaarfExporter collectors, fetches data from Google Ads API
 and expose them to Prometheus.
-
-'''
+"""
 from __future__ import annotations
 
 import argparse
 import logging
 from concurrent import futures
 from time import sleep
 from time import time
 
+import prometheus_client
+import smart_open
 import yaml
-from gaarf.cli.utils import init_logging
-from gaarf.cli.utils import ParamsParser
-from prometheus_client import start_http_server
-from smart_open import open
+from gaarf.cli import utils as gaarf_utils
 
+from gaarf_exporter import bootstrap
 from gaarf_exporter import collectors
-from gaarf_exporter.bootstrap import inject_dependencies
-from gaarf_exporter.config import Config
-from gaarf_exporter.exporter import GaarfExporter
-from gaarf_exporter.util import find_relative_metrics
+from gaarf_exporter import config as exporter_config
+from gaarf_exporter import exporter
+from gaarf_exporter import util
 
 
 def main() -> None:
   parser = argparse.ArgumentParser()
   parser.add_argument('--account', dest='account', default=None)
   parser.add_argument('-c', dest='config', default=None)
   parser.add_argument('--ads-config', dest='ads_config', default=None)
-  parser.add_argument('--api-version', dest='api_version', default=14)
+  parser.add_argument('--api-version', dest='api_version', default=None)
   parser.add_argument('--queries.exclude', dest='exclude_queries', default=None)
   parser.add_argument('--queries.include', dest='include_queries', default=None)
   parser.add_argument('--log', '--loglevel', dest='loglevel', default='info')
   parser.add_argument(
       '--http_server.address', dest='address', default='0.0.0.0')
   parser.add_argument('--http_server.port', dest='port', type=int, default=8000)
   parser.add_argument(
       '--pushgateway.address', dest='pushgateway_address', default=None)
   parser.add_argument(
       '--pushgateway.port', dest='pushgateway_port', default=None)
   parser.add_argument('--logger', dest='logger', default='local')
   parser.add_argument('--iterations', dest='iterations', default=None, type=int)
+  parser.add_argument(
+      '--update-accounts-every-n-iterations',
+      dest='iterations_left',
+      default=4 * 24,
+      type=int)
   parser.add_argument('--delay-minutes', dest='delay', type=int, default=15)
   parser.add_argument(
       '--expose-metrics-with-zero-values',
       dest='zero_value_metrics',
       action='store_true')
   parser.add_argument('--namespace', dest='namespace', default='googleads')
   parser.add_argument('--collectors', dest='collectors', default='default')
   args_bag = parser.parse_known_args()
   args = args_bag[0]
 
-  logger = init_logging(loglevel=args.loglevel.upper(), logger_type=args.logger)
+  logger = gaarf_utils.init_logging(
+      loglevel=args.loglevel.upper(), logger_type=args.logger)
 
-  params = ParamsParser(['macro', 'sql', 'template']).parse(args_bag[1])
+  params = gaarf_utils.ParamsParser([
+      'macro',
+      'sql',
+      'template',
+  ]).parse(args_bag[1])
   collectors_registry = collectors.Registry()
   macros = params.get('macro', {})
   if config_file := args.config:
-    with open(config_file, encoding='utf-8') as f:
+    with smart_open.open(config_file, encoding='utf-8') as f:
       config = yaml.safe_load(f)
       queries = config.get('queries')
   else:
     if not (active_collectors := collectors_registry.find_collectors(
         args.collectors)):
       logger.warning('Failed to get "%s" collectors, using default ones',
                      args.collectors)
       active_collectors = collectors_registry.default_collectors
     if macros:
       active_collectors.customize(macros)
-    config = Config(active_collectors.targets)
+    config = exporter_config.Config(active_collectors.targets)
     queries = config.queries
   for query_name, query in queries.items():
-    if relative_metrics := find_relative_metrics(query['query']):
+    if relative_metrics := util.find_relative_metrics(query['query']):
       logger.warning(
           'In query %s, relative metrics: [%s] are found, which might '
           'not be useful.', query_name, ', '.join(relative_metrics))
   runtime_options = {
       'exclude_queries':
           args.exclude_queries.split(',') if args.exclude_queries else None,
       'include_queries':
           args.include_queries.split(',') if args.include_queries else None,
   }
 
-  dependencies = inject_dependencies(
+  dependencies = bootstrap.inject_dependencies(
       ads_config_path=args.ads_config,
       api_version=args.api_version,
       account=args.account)
   report_fetcher, accounts = dependencies.get(
       'report_fetcher'), dependencies.get('accounts')
   gaarf_exporter_options = {
       'expose_metrics_with_zero_values': args.zero_value_metrics,
       'namespace': args.namespace
   }
 
   if args.pushgateway_address and args.pushgateway_port:
-    gaarf_exporter = GaarfExporter(
+    gaarf_exporter = exporter.GaarfExporter(
         pushgateway_url=f'{args.pushgateway_address}:{args.pushgateway_port}',
         **gaarf_exporter_options)
   elif (args.address and args.port):
-    gaarf_exporter = GaarfExporter(
+    gaarf_exporter = exporter.GaarfExporter(
         http_server_url=f'{args.address}:{args.port}', **gaarf_exporter_options)
   else:
     raise ValueError('Specify option for exposing data to Prometheus '
                      '- either http_server or pushgateway')
 
   if gaarf_exporter.http_server_url and not gaarf_exporter.pushgateway_url:
-    start_http_server(
+    prometheus_client.start_http_server(
         port=args.port, addr=args.address, registry=gaarf_exporter.registry)
     logger.info('Started http_server at http://%s',
                 gaarf_exporter.http_server_url)
   while True:
+    if iterations_left := args.iterations_left:
+      iterations_left -= 1
+    if accounts and iterations_left == 0:
+      accounts = report_fetcher.expand_mcc(args.account)
+      iterations_left = args.iterations_left
     start_export_time = time()
-    if macros:
-      active_collectors.customize(macros)
-    config = Config(active_collectors.targets)
-    queries = config.queries
+    if not args.config:
+      if macros:
+        active_collectors.customize(macros)
+      config = exporter_config.Config(active_collectors.targets)
+      queries = config.queries
     for name, content in queries.items():
       if not (query_text := content.get('query')):
         raise ValueError(f'Missing query text for query "{name}"')
       if include_queries := runtime_options.get('include_queries'):
         if name not in include_queries:
           continue
       if exclude_queries := runtime_options.get('exclude_queries'):
```

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter/query_elements.py` & `gaarf-exporter-0.7.1/gaarf_exporter/query_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 class Field:
 
   def __init__(self,
                name: str,
                alias: str | None = None,
                customizer: Customizer | None = None) -> None:
     self.name = name
-    self.alias = alias
+    self.alias = alias or name.replace('.', '_')
     self.customizer = customizer
 
   def to_query_field(self) -> str:
     name = self.name
 
     if self.customizer:
       name = f'{name}{self.customizer.to_raw_string()}'
```

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter/search_collectors.py` & `gaarf-exporter-0.7.1/gaarf_exporter/search_collectors.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter/util.py` & `gaarf-exporter-0.7.1/gaarf_exporter/util.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/PKG-INFO` & `gaarf-exporter-0.7.1/gaarf_exporter.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaarf-exporter
-Version: 0.7.0rc1
+Version: 0.7.1
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
@@ -46,15 +46,18 @@
 
 ```
 By default it will start http_server on `localhost:8000` and will push some basic metrics to it.
 
 ### Customization
 
 * `--ads-config` - path to `google-ads.yaml`
+  >  `ads-config` can be taken from local storage or remote storage (gs, s3, azure, ssh, stfp, scrp, hdfs, webhdfs).
 * `--config` - path to `gaarf_exporter.yaml`
+  >  `config` can be taken from local storage or remote storage (same as `--ads-config`).
+* `--collectors` - names of one or more [collectors](#collectors) (separated by comma).
 * `--http_server.address` - address of your http server (`localhost` by default)
 * `--http_server.port` - port of your http server (`8000` by default)
 * `--pushgateway.address` - address of your pushgateway service (`None` by default)
 * `--pushgateway.port` - port of your pushgateway (`None` by default)
 * `--delay-minutes` - delay in minutes between scrapings (`15` by default)
 
 #### Customizing with macros:
@@ -67,38 +70,43 @@
 * `--macro.end_date=:YYYYMMDD-M`, where `N` is number of days starting from today
 
 It will add an additional metric to be exposed to Prometheus `*_n_days` (i.e.
 `googleads_clicks_n_days`.
 
 ### Collectors
 
-You can specify collectors with `--collectors <collector_name>` CLI argument. Some collectors available by default, other you need to specify explicitly.
+You can specify collectors with `--collectors <collector_name>` CLI argument. Some collectors available by default, other you need to specify explicitly.\
+There are two types of collectors - *registry* (contains other collectors grouped logically) and *collectors* themselves.
 
 #### `default` registry.
 
 * `performance` - extracts *clicks*, *impressions*, *cost*, *conversions* on by *ad_network* and *ad_group_id*
 * `disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *ad_group_id* and *ad_id* only for not approved ads
 * `conversion_action` - extracts *all_conversions* by *conversion_id* and *account_id*
 * `mapping` - performance mapping between *ad_group_id*, *ad_group_name*, *campaign_id*, *campaign_name,* *campaign_status*, *account_id*, *account_name*
 
 #### *disapprovals* registry.
 
 * `ad_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *ad_group_id* and *ad_id* only for not approved ads
 * `ad_group_ad_asset_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *ad_group_id* and *asset_id* only for enabled assets.
 * `sitelink_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *asset_id*,   *sitelink_title* and both sitelink descriptions only for not approved sitelinks.
+* `pmax_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *asset_id*,   *asset_group_id* for active asset group assets.
 
 #### *app* registry.
 
 * `app_campaign_mapping` - performs mapping between *campaign_id*, *app_id*, *app_store*, *and bidding_strategy* only for active campaigns.
+* `app_asset_mapping` - performs mapping between *asset_id* and its type, source, and content (*name*, *text*, *video_id*) only for app assets (HTML5, TEXT, IMAGE, VIDEO).
 * `asset_performance` - extracts *clicks*, *impressions*, *cost*, *installs*, *inapps*, and *conversions_value* by *ad_group_id*, *ad_network* and *asset_id*
 * `asset_perf_label` - extracts *performance_label* by *ad_group_id* and *asset_id*
 
 #### *pmax* registry.
 
 * `pmax_mapping` - performs mapping between *asset_group_id*, *asset_group_name*, and meta information on campaign and account only for active campaigns and enabled asset groups.
+* `pmax_performance` - extracts *clicks*, *impressions*, *cost*, *installs*, *inapps*, and *conversions_value* by *asset_group_id*.
+* `pmax_disapprovals` - extracts *approval_status*, *review_status*, *topic*, *topic_type* by *asset_id*,   *asset_group_id* for active asset group assets.
 
 #### *search* registry.
 
 * `search_terms` - extracts *clicks*, *impressions*, *cost*, *conversions* on by *search_term* and *ad_group_id*
 * `search_terms_conversion_split` - extracts *all_conversions* by *search_term* and *conversion_id* on *ad_group_id* level
 * `keywords` - extracts *clicks*, *impressions*, *cost*, *conversions*, and *historical auality_score*  by *keyword* and *match_type* on ad_group level.
 * `keywords_conversion_split` - extracts *all_conversions* by *keyword* and *match_type* on ad_group level.
@@ -118,10 +126,12 @@
 #### *geo* registry.
 
 * `user_location` - extracts *clicks*, *impressions*, *cost*, *conversions* by *country_id* and *campaign_id* only for active campaigns.
 * `user_location_conversion_split` - extracts *all_conversions* by *country_id*  and *campaign_id*only for active campaigns.
 
 #### collectors without registry.
 
-* `bid_budgets` - extracts current values of bid (target_cpa, target_roas) and budget
+* `bid_budgets` - extracts current values of bid (target_cpa, target_roas) and campaign budgets.
+* `bids` - extracts current values of bid (target_cpa, target_roas).
+* `budgets` - extracts current values of campaign budgets.
 * `account_status` - extracts *customer_status* for each account.
 * `campaign_service_status` - extracts *primary_status* for each campaign.
```

### Comparing `gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/SOURCES.txt` & `gaarf-exporter-0.7.1/gaarf_exporter.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 gaarf_exporter.egg-info/PKG-INFO
 gaarf_exporter.egg-info/SOURCES.txt
 gaarf_exporter.egg-info/dependency_links.txt
 gaarf_exporter.egg-info/entry_points.txt
 gaarf_exporter.egg-info/requires.txt
 gaarf_exporter.egg-info/top_level.txt
 tests/__init__.py
-tests/conftest.py
-tests/test_alerts.py
-tests/test_collectors.py
-tests/test_config.py
-tests/test_exporter.py
-tests/test_query_element.py
-tests/test_target.py
-tests/test_util.py
+tests/end-to-end/__init__.py
+tests/end-to-end/test_gaarf_exporter.py
+tests/unit/__init__.py
+tests/unit/test_alerts.py
+tests/unit/test_collectors.py
+tests/unit/test_config.py
+tests/unit/test_exporter.py
+tests/unit/test_query_elements.py
+tests/unit/test_target.py
+tests/unit/test_util.py
```

### Comparing `gaarf-exporter-0.7.0rc1/setup.py` & `gaarf-exporter-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / 'README.md').read_text()
 
 setup(
   name='gaarf-exporter',
-  version='0.7.0.rc1',
+  version='0.7.1',
   long_description=README,
   long_description_content_type='text/markdown',
   author='Google Inc. (gTech gPS CSE team)',
   author_email='no-reply@google.com',
   license='Apache 2.0',
   classifiers=[
     'Programming Language :: Python :: 3',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: Apache Software License'
   ],
   packages=find_packages(),
   install_requires=[
-    'prometheus-client', 'google-ads-api-report-fetcher>=1.12.0'
+    'prometheus-client', 'google-ads-api-report-fetcher==1.13.4'
   ],
   setup_requires=['pytest-runner'],
   tests_requires=['pytest'],
   entry_points={
     'console_scripts': ['gaarf-exporter=gaarf_exporter.main:main',]
   })
```

### Comparing `gaarf-exporter-0.7.0rc1/tests/test_alerts.py` & `gaarf-exporter-0.7.1/tests/unit/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0rc1/tests/test_exporter.py` & `gaarf-exporter-0.7.1/tests/unit/test_exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0rc1/tests/test_query_element.py` & `gaarf-exporter-0.7.1/tests/unit/test_query_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0rc1/tests/test_util.py` & `gaarf-exporter-0.7.1/tests/unit/test_util.py`

 * *Files identical despite different names*

