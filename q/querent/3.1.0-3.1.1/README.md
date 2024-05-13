# Comparing `tmp/querent-3.1.0.tar.gz` & `tmp/querent-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querent-3.1.0.tar", last modified: Mon May  6 16:58:17 2024, max compression
+gzip compressed data, was "querent-3.1.1.tar", last modified: Mon May 13 07:21:15 2024, max compression
```

## Comparing `querent-3.1.0.tar` & `querent-3.1.1.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-06 16:53:38.000000 querent-3.1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-06 16:58:17.601502 querent-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-06 16:53:38.000000 querent-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.533502 querent-3.1.0/querent/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-06 16:53:38.000000 querent-3.1.0/querent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.533502 querent-3.1.0/querent/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-06 16:53:38.000000 querent-3.1.0/querent/callback/event_callback_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 16:53:38.000000 querent-3.1.0/querent/callback/event_callback_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.533502 querent-3.1.0/querent/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-06 16:53:38.000000 querent-3.1.0/querent/channel/channel_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/collectors/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/aws/aws_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/collectors/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/azure/azure_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/collector_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/collector_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/collector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/collector_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.537502 querent-3.1.0/querent/collectors/drive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/drive/google_drive_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/dropbox/dropbox_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/email/email_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/email/imap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/fs/fs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/gcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/gcs/gcs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/github/github_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.541502 querent-3.1.0/querent/collectors/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/jira/jira_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/collectors/news/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/news/news_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/collectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/slack/slack_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/collectors/webscaper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/webscaper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-06 16:53:38.000000 querent-3.1.0/querent/collectors/webscaper/web_scraper_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/common_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.545502 querent-3.1.0/querent/common/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/errors/metric_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.553502 querent-3.1.0/querent/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/collected_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/collector_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/engine_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/file_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/ingested_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/querent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/querent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/resource_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/types/workflow_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-06 16:53:38.000000 querent-3.1.0/querent/common/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.553502 querent-3.1.0/querent/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.553502 querent-3.1.0/querent/config/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/collector/collector_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/core/gpt_llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/core/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/core/opensource_llm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/engine/engine_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/graph_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/ingestor/ingestor_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/logger/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/metric/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.557502 querent-3.1.0/querent/config/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/resource/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/config/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-06 16:53:38.000000 querent-3.1.0/querent/config/workflow/workflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12319 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/bert_ner_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/fixed_entities_set_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/gpt_llm_gpt_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-06 16:53:38.000000 querent-3.1.0/querent/core/transformers/relationship_extraction_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.561502 querent-3.1.0/querent/dal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/dal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.565502 querent-3.1.0/querent/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/gnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.565502 querent-3.1.0/querent/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/graph_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-06 16:53:38.000000 querent-3.1.0/querent/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/audio/audio_ingestors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/base_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/code/code_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/csv/csv_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.569502 querent-3.1.0/querent/ingestors/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/doc/doc_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.573502 querent-3.1.0/querent/ingestors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/email/email_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/email/email_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.573502 querent-3.1.0/querent/ingestors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/github/github_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.573502 querent-3.1.0/querent/ingestors/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/html/html_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.573502 querent-3.1.0/querent/ingestors/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/images/image_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/ingestor_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/ingestor_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/json/json_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/pdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/pdfs/pdf_ingestor_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/ppt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/ppt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/ppt/ppt_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/texts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/texts/text_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/video/video_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.577502 querent-3.1.0/querent/ingestors/xlsx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/xlsx/xlsx_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.581502 querent-3.1.0/querent/ingestors/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-06 16:53:38.000000 querent-3.1.0/querent/ingestors/xml/xml_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.581502 querent-3.1.0/querent/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.585502 querent-3.1.0/querent/kg/ner_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/attn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/contextual_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/dependency_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/filter_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/fixed_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/fixed_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18269 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/ner_helperfunctions/ner_llm_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/querent_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.589502 querent-3.1.0/querent/kg/rel_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/contextual_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/fixed_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/openai_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/openllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/questionanswer_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/rel_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-06 16:53:38.000000 querent-3.1.0/querent/kg/rel_helperfunctions/triple_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.593502 querent-3.1.0/querent/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/custom_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-06 16:53:38.000000 querent-3.1.0/querent/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.593502 querent-3.1.0/querent/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.593502 querent-3.1.0/querent/metric/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/adapters/promethus_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/base_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/metric_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 16:53:38.000000 querent-3.1.0/querent/metric/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.597502 querent-3.1.0/querent/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-06 16:53:38.000000 querent-3.1.0/querent/processors/async_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 16:53:38.000000 querent-3.1.0/querent/processors/text_cleanup_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-06 16:53:38.000000 querent-3.1.0/querent/processors/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.597502 querent-3.1.0/querent/querent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/querent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/querent/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.597502 querent-3.1.0/querent/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/gcs_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/milvus_vectorevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/neo4j_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-06 16:53:38.000000 querent-3.1.0/querent/storage/postgres_graphevent_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/querent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-06 16:53:38.000000 querent-3.1.0/querent/tools/web_page_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/querent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:38.000000 querent-3.1.0/querent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-06 16:53:38.000000 querent-3.1.0/querent/utils/webpage_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/querent/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 16:53:38.000000 querent-3.1.0/querent/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-06 16:53:38.000000 querent-3.1.0/querent/workflow/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-06 16:53:38.000000 querent-3.1.0/querent/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:58:17.601502 querent-3.1.0/querent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 16:58:17.000000 querent-3.1.0/querent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:58:17.601502 querent-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-06 16:53:38.000000 querent-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.603400 querent-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-13 07:16:31.000000 querent-3.1.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-13 07:21:15.603400 querent-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-13 07:16:31.000000 querent-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.519399 querent-3.1.1/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-13 07:16:31.000000 querent-3.1.1/querent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.523399 querent-3.1.1/querent/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-13 07:16:31.000000 querent-3.1.1/querent/callback/event_callback_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-13 07:16:31.000000 querent-3.1.1/querent/callback/event_callback_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.523399 querent-3.1.1/querent/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-13 07:16:31.000000 querent-3.1.1/querent/channel/channel_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.523399 querent-3.1.1/querent/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.527399 querent-3.1.1/querent/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.531399 querent-3.1.1/querent/collectors/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/aws/aws_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.531399 querent-3.1.1/querent/collectors/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/azure/azure_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/collector_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/collector_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/collector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/collector_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.531399 querent-3.1.1/querent/collectors/drive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/drive/google_drive_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.531399 querent-3.1.1/querent/collectors/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/dropbox/dropbox_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.535399 querent-3.1.1/querent/collectors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/email/email_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/email/imap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.535399 querent-3.1.1/querent/collectors/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/fs/fs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.535399 querent-3.1.1/querent/collectors/gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/gcs/gcs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.535399 querent-3.1.1/querent/collectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/github/github_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.535399 querent-3.1.1/querent/collectors/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/jira/jira_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.535399 querent-3.1.1/querent/collectors/news/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/news/news_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.539399 querent-3.1.1/querent/collectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/slack/slack_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.539399 querent-3.1.1/querent/collectors/webscaper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/webscaper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-13 07:16:31.000000 querent-3.1.1/querent/collectors/webscaper/web_scraper_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.539399 querent-3.1.1/querent/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/common_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.539399 querent-3.1.1/querent/common/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/errors/metric_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.547399 querent-3.1.1/querent/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/collected_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/collector_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/engine_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/file_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/ingested_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/ingested_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/ingested_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/ingested_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/ingested_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/querent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/querent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/resource_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/types/workflow_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-13 07:16:31.000000 querent-3.1.1/querent/common/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.547399 querent-3.1.1/querent/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.547399 querent-3.1.1/querent/config/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/collector/collector_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.551399 querent-3.1.1/querent/config/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/core/gpt_llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/core/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/core/opensource_llm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.551399 querent-3.1.1/querent/config/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/engine/engine_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/graph_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.551399 querent-3.1.1/querent/config/ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/ingestor/ingestor_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.551399 querent-3.1.1/querent/config/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/logger/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.555399 querent-3.1.1/querent/config/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/metric/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.555399 querent-3.1.1/querent/config/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/resource/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.555399 querent-3.1.1/querent/config/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-13 07:16:31.000000 querent-3.1.1/querent/config/workflow/workflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.555399 querent-3.1.1/querent/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.555399 querent-3.1.1/querent/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12319 2024-05-13 07:16:31.000000 querent-3.1.1/querent/core/base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.559399 querent-3.1.1/querent/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/core/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17687 2024-05-13 07:16:31.000000 querent-3.1.1/querent/core/transformers/bert_ner_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-13 07:16:31.000000 querent-3.1.1/querent/core/transformers/fixed_entities_set_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-05-13 07:16:31.000000 querent-3.1.1/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-05-13 07:16:31.000000 querent-3.1.1/querent/core/transformers/gpt_llm_gpt_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-13 07:16:31.000000 querent-3.1.1/querent/core/transformers/relationship_extraction_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.559399 querent-3.1.1/querent/dal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/dal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.559399 querent-3.1.1/querent/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/gnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.563399 querent-3.1.1/querent/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-13 07:16:31.000000 querent-3.1.1/querent/graph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-13 07:16:31.000000 querent-3.1.1/querent/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-13 07:16:31.000000 querent-3.1.1/querent/graph/graph_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 07:16:31.000000 querent-3.1.1/querent/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-13 07:16:31.000000 querent-3.1.1/querent/graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-05-13 07:16:31.000000 querent-3.1.1/querent/graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-13 07:16:31.000000 querent-3.1.1/querent/graph/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-13 07:16:31.000000 querent-3.1.1/querent/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.563399 querent-3.1.1/querent/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.567399 querent-3.1.1/querent/ingestors/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/audio/audio_ingestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/base_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.567399 querent-3.1.1/querent/ingestors/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/code/code_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.567399 querent-3.1.1/querent/ingestors/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/csv/csv_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.567399 querent-3.1.1/querent/ingestors/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/doc/doc_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.571399 querent-3.1.1/querent/ingestors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/email/email_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/email/email_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.571399 querent-3.1.1/querent/ingestors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/github/github_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.571399 querent-3.1.1/querent/ingestors/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/html/html_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.571399 querent-3.1.1/querent/ingestors/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/images/image_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/ingestor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/ingestor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.571399 querent-3.1.1/querent/ingestors/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/json/json_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.575399 querent-3.1.1/querent/ingestors/pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/pdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/pdfs/pdf_ingestor_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.575399 querent-3.1.1/querent/ingestors/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/ppt/ppt_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.575399 querent-3.1.1/querent/ingestors/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/texts/text_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.575399 querent-3.1.1/querent/ingestors/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/video/video_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.575399 querent-3.1.1/querent/ingestors/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/xlsx/xlsx_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.575399 querent-3.1.1/querent/ingestors/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-13 07:16:31.000000 querent-3.1.1/querent/ingestors/xml/xml_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.579399 querent-3.1.1/querent/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.583399 querent-3.1.1/querent/kg/ner_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/ner_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/ner_helperfunctions/attn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/ner_helperfunctions/contextual_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/ner_helperfunctions/dependency_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/ner_helperfunctions/filter_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/ner_helperfunctions/fixed_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/ner_helperfunctions/fixed_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18269 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/ner_helperfunctions/ner_llm_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/querent_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.587399 querent-3.1.1/querent/kg/rel_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/contextual_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/fixed_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/openai_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/openllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/questionanswer_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/rel_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-13 07:16:31.000000 querent-3.1.1/querent/kg/rel_helperfunctions/triple_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.591399 querent-3.1.1/querent/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 07:16:31.000000 querent-3.1.1/querent/logging/custom_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 07:16:31.000000 querent-3.1.1/querent/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-13 07:16:31.000000 querent-3.1.1/querent/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-13 07:16:31.000000 querent-3.1.1/querent/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.591399 querent-3.1.1/querent/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.591399 querent-3.1.1/querent/metric/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/metric/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-13 07:16:31.000000 querent-3.1.1/querent/metric/adapters/promethus_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-13 07:16:31.000000 querent-3.1.1/querent/metric/base_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-13 07:16:31.000000 querent-3.1.1/querent/metric/metric_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-13 07:16:31.000000 querent-3.1.1/querent/metric/metric_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.595399 querent-3.1.1/querent/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-13 07:16:31.000000 querent-3.1.1/querent/processors/async_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-13 07:16:31.000000 querent-3.1.1/querent/processors/text_cleanup_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-13 07:16:31.000000 querent-3.1.1/querent/processors/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.595399 querent-3.1.1/querent/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/querent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-13 07:16:31.000000 querent-3.1.1/querent/querent/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-13 07:16:31.000000 querent-3.1.1/querent/querent/querent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-13 07:16:31.000000 querent-3.1.1/querent/querent/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/querent/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.599399 querent-3.1.1/querent/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-13 07:16:31.000000 querent-3.1.1/querent/storage/gcs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-13 07:16:31.000000 querent-3.1.1/querent/storage/milvus_vectorevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-13 07:16:31.000000 querent-3.1.1/querent/storage/neo4j_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-13 07:16:31.000000 querent-3.1.1/querent/storage/postgres_graphevent_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.599399 querent-3.1.1/querent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-13 07:16:31.000000 querent-3.1.1/querent/tools/web_page_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.599399 querent-3.1.1/querent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:16:31.000000 querent-3.1.1/querent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-13 07:16:31.000000 querent-3.1.1/querent/utils/webpage_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.603400 querent-3.1.1/querent/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 07:16:31.000000 querent-3.1.1/querent/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-13 07:16:31.000000 querent-3.1.1/querent/workflow/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-13 07:16:31.000000 querent-3.1.1/querent/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:21:15.603400 querent-3.1.1/querent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-13 07:21:15.000000 querent-3.1.1/querent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-13 07:21:15.000000 querent-3.1.1/querent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:21:15.000000 querent-3.1.1/querent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-13 07:21:15.000000 querent-3.1.1/querent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 07:21:15.000000 querent-3.1.1/querent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:21:15.603400 querent-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-13 07:16:31.000000 querent-3.1.1/setup.py
```

### Comparing `querent-3.1.0/LICENCE` & `querent-3.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/PKG-INFO` & `querent-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.1.0
+Version: 3.1.1
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
```

### Comparing `querent-3.1.0/README.md` & `querent-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/__init__.py` & `querent-3.1.1/querent/__init__.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/callback/event_callback_dispatcher.py` & `querent-3.1.1/querent/callback/event_callback_dispatcher.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/callback/event_callback_interface.py` & `querent-3.1.1/querent/callback/event_callback_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/channel/channel_interface.py` & `querent-3.1.1/querent/channel/channel_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/aws/aws_collector.py` & `querent-3.1.1/querent/collectors/aws/aws_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/azure/azure_collector.py` & `querent-3.1.1/querent/collectors/azure/azure_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/collector_errors.py` & `querent-3.1.1/querent/collectors/collector_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/collector_factory.py` & `querent-3.1.1/querent/collectors/collector_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/collector_resolver.py` & `querent-3.1.1/querent/collectors/collector_resolver.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/drive/google_drive_collector.py` & `querent-3.1.1/querent/collectors/drive/google_drive_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/dropbox/dropbox_collector.py` & `querent-3.1.1/querent/collectors/dropbox/dropbox_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/email/email_collector.py` & `querent-3.1.1/querent/collectors/email/email_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/email/imap.py` & `querent-3.1.1/querent/collectors/email/imap.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/fs/fs_collector.py` & `querent-3.1.1/querent/collectors/fs/fs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/gcs/gcs_collector.py` & `querent-3.1.1/querent/collectors/gcs/gcs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/github/github_collector.py` & `querent-3.1.1/querent/collectors/github/github_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/jira/jira_collector.py` & `querent-3.1.1/querent/collectors/jira/jira_collector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from typing import AsyncGenerator
+import requests
 
 from querent.collectors.collector_base import Collector
 from querent.collectors.collector_factory import CollectorFactory
 from querent.common import common_errors
 from querent.common.types.collected_bytes import CollectedBytes
 from querent.common.uri import Uri
 from querent.config.collector.collector_config import (
@@ -84,24 +85,45 @@
                 yield CollectedBytes(
                     data=json_issue, file=f"jira_issue_{issue.key}.json.jira", doc_source=f"jira://{self.config.jira_server}/{self.config.jira_project}"
                 )
                 yield CollectedBytes(
                     data=None, file=f"jira_issue_{issue.key}.json.jira", eof=True, doc_source=f"jira://{self.config.jira_server}/{self.config.jira_project}"
                 )
 
+                if hasattr(issue.fields, 'attachment') and isinstance(issue.fields.attachment, list):
+                    for attachment in issue.fields.attachment:
+                        try:
+                            attachment_bytes = self.download_attachment(attachment.content, self.auth)
+                            yield CollectedBytes(
+                                data=attachment_bytes, file=f"jira_attachment_{attachment.filename}", doc_source=f"jira://{self.config.jira_server}/{self.config.jira_project}"
+                            )
+                            yield CollectedBytes(
+                                data=None, file=f"jira_attachment_{attachment.filename}", eof=True, doc_source=f"jira://{self.config.jira_server}/{self.config.jira_project}"
+                            )
+                        except Exception as e:
+                            self.logger.error(f"Error downloading attachment {attachment.filename}: {str(e)}")
+                
+
         except common_errors.ConnectionError as e:
             self.logger.error(f"Error polling Jira issues: {e}")
             raise  # Re-raise ConnectionError without adding additional information
         except Exception as e:
             raise common_errors.ConnectionError(
                 f"Failed to poll Jira issues: {str(e)}"
             ) from e
         finally:
             await self.disconnect()
 
+    async def download_attachment(self, attachment_url, auth):
+        response = requests.get(attachment_url, auth=auth)
+        if response.status_code == 200:
+            return response.content
+        else:
+            self.logger.error("Failed to download file: HTTP {}".format(response.status_code))
+
 
 class JiraCollectorFactory(CollectorFactory):
     def backend(self) -> CollectorBackend:
         return CollectorBackend.Jira
 
     def resolve(self, uri: Uri, config: JiraCollectorConfig) -> Collector:
         return JiraCollector(config)
```

### Comparing `querent-3.1.0/querent/collectors/news/news_collector.py` & `querent-3.1.1/querent/collectors/news/news_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/collectors/webscaper/web_scraper_collector.py` & `querent-3.1.1/querent/collectors/webscaper/web_scraper_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/common_errors.py` & `querent-3.1.1/querent/common/common_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/errors/metric_errors.py` & `querent-3.1.1/querent/common/errors/metric_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/types/collected_bytes.py` & `querent-3.1.1/querent/common/types/collected_bytes.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/types/file_buffer.py` & `querent-3.1.1/querent/common/types/file_buffer.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/types/ingested_code.py` & `querent-3.1.1/querent/common/types/ingested_code.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/types/ingested_images.py` & `querent-3.1.1/querent/common/types/ingested_images.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/types/ingested_messages.py` & `querent-3.1.1/querent/common/types/ingested_messages.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/types/ingested_table.py` & `querent-3.1.1/querent/common/types/ingested_table.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/types/ingested_tokens.py` & `querent-3.1.1/querent/common/types/ingested_tokens.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/types/querent_queue.py` & `querent-3.1.1/querent/common/types/querent_queue.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/common/uri.py` & `querent-3.1.1/querent/common/uri.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/collector/collector_config.py` & `querent-3.1.1/querent/config/collector/collector_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/config.py` & `querent-3.1.1/querent/config/config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/core/gpt_llm_config.py` & `querent-3.1.1/querent/config/core/gpt_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/core/llm_config.py` & `querent-3.1.1/querent/config/core/llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/core/opensource_llm_config.py` & `querent-3.1.1/querent/config/core/opensource_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/engine/engine_config.py` & `querent-3.1.1/querent/config/engine/engine_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/graph_config.py` & `querent-3.1.1/querent/config/graph_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/ingestor/ingestor_config.py` & `querent-3.1.1/querent/config/ingestor/ingestor_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/metric/prometheus.py` & `querent-3.1.1/querent/config/metric/prometheus.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/resource/resource_config.py` & `querent-3.1.1/querent/config/resource/resource_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/config/workflow/workflow_config.py` & `querent-3.1.1/querent/config/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/core/base_engine.py` & `querent-3.1.1/querent/core/base_engine.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/core/transformers/bert_ner_opensourcellm.py` & `querent-3.1.1/querent/core/transformers/bert_ner_opensourcellm.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,25 +136,26 @@
                 (entity_ocr, doc_entity_pairs_ocr) = self.ner_llm_instance.get_entity_pairs(isConfinedSearch= self.isConfinedSearch, 
                                                                                                   content=ocr_content,
                                                                                                   fixed_entities=self.fixed_entities,
                                                                                                   sample_entities=self.sample_entities)
                 if len(doc_entity_pairs_ocr) >= 1:
                     results = doc_entity_pairs_ocr
                 elif len(doc_entity_pairs_ocr) == 0:
-                    if content:
+                    if content and len(entity_ocr) >=1:
                         if self.fixed_entities:
                             content = self.entity_context_extractor.find_entity_sentences(content)
                         (_, doc_entity_pairs) = self.ner_llm_instance.get_entity_pairs(isConfinedSearch= self.isConfinedSearch, 
                                                                                                   content=content,
                                                                                                   fixed_entities=self.fixed_entities,
                                                                                                   sample_entities=self.sample_entities)
                         if len(doc_entity_pairs) > 0 and len(entity_ocr) >=1:
                             results = [self.ner_llm_instance.filter_matching_entities(doc_entity_pairs, entity_ocr)]
                         elif len(doc_entity_pairs) > 0 and len(entity_ocr) == 0:
-                            results = doc_entity_pairs
+                            # results = doc_entity_pairs
+                            pass
                     else:
                         return        
                 if len(results) > 0:
                     doc_entity_pairs = self.ner_llm_instance.remove_duplicates(results)
                     filtered_triples = process_data(doc_entity_pairs, file)
                     if self.skip_inferences:
                         return filtered_triples, file, self.ner_llm_instance
```

### Comparing `querent-3.1.0/querent/core/transformers/fixed_entities_set_opensourcellm.py` & `querent-3.1.1/querent/core/transformers/fixed_entities_set_opensourcellm.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py` & `querent-3.1.1/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/core/transformers/gpt_llm_gpt_ner.py` & `querent-3.1.1/querent/core/transformers/gpt_llm_gpt_ner.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/core/transformers/relationship_extraction_llm.py` & `querent-3.1.1/querent/core/transformers/relationship_extraction_llm.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/graph/errors.py` & `querent-3.1.1/querent/graph/errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/graph/graph.py` & `querent-3.1.1/querent/graph/graph.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/graph/graph_namespace.py` & `querent-3.1.1/querent/graph/graph_namespace.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/graph/ontology.py` & `querent-3.1.1/querent/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/graph/schema.py` & `querent-3.1.1/querent/graph/schema.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/graph/shacl.py` & `querent-3.1.1/querent/graph/shacl.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/graph/subject.py` & `querent-3.1.1/querent/graph/subject.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/graph/utils.py` & `querent-3.1.1/querent/graph/utils.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/audio/audio_ingestors.py` & `querent-3.1.1/querent/ingestors/audio/audio_ingestors.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/base_ingestor.py` & `querent-3.1.1/querent/ingestors/base_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/code/code_ingestor.py` & `querent-3.1.1/querent/ingestors/code/code_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/csv/csv_ingestor.py` & `querent-3.1.1/querent/ingestors/csv/csv_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/doc/doc_ingestor.py` & `querent-3.1.1/querent/ingestors/doc/doc_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/email/email_ingestor.py` & `querent-3.1.1/querent/ingestors/email/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/email/email_reader.py` & `querent-3.1.1/querent/ingestors/email/email_reader.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/github/github_ingestor.py` & `querent-3.1.1/querent/ingestors/github/github_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/html/html_ingestor.py` & `querent-3.1.1/querent/ingestors/html/html_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/images/image_ingestor.py` & `querent-3.1.1/querent/ingestors/images/image_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/ingestor_factory.py` & `querent-3.1.1/querent/ingestors/ingestor_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/ingestor_manager.py` & `querent-3.1.1/querent/ingestors/ingestor_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/json/json_ingestor.py` & `querent-3.1.1/querent/ingestors/json/json_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/pdfs/pdf_ingestor_v1.py` & `querent-3.1.1/querent/ingestors/pdfs/pdf_ingestor_v1.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/ppt/ppt_ingestor.py` & `querent-3.1.1/querent/ingestors/ppt/ppt_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/texts/text_ingestor.py` & `querent-3.1.1/querent/ingestors/texts/text_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/video/video_ingestor.py` & `querent-3.1.1/querent/ingestors/video/video_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/ingestors/xlsx/xlsx_ingestor.py` & `querent-3.1.1/querent/ingestors/xml/xml_ingestor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,99 +1,94 @@
 from typing import List, AsyncGenerator
-import io
-import pandas as pd
+import xml.etree.ElementTree as ET
+from io import BytesIO
 
-from querent.ingestors.ingestor_factory import IngestorFactory
-from querent.ingestors.base_ingestor import BaseIngestor
 from querent.processors.async_processor import AsyncProcessor
+from querent.ingestors.ingestor_factory import IngestorFactory
 from querent.config.ingestor.ingestor_config import IngestorBackend
+from querent.ingestors.base_ingestor import BaseIngestor
 from querent.common.types.collected_bytes import CollectedBytes
 from querent.common.types.ingested_tokens import (
     IngestedTokens,
 )  # Added import for the return type
 from querent.logging.logger import setup_logger
 
 
-class XlsxIngestorFactory(IngestorFactory):
-    SUPPORTED_EXTENSIONS = {"xlsx"}
+class XmlIngestorFactory(IngestorFactory):
+    """Ingestor factory for xlsx files"""
+
+    SUPPORTED_EXTENSIONS = {"xml"}
 
     async def supports(self, file_extension: str) -> bool:
         return file_extension.lower() in self.SUPPORTED_EXTENSIONS
 
     async def create(
         self, file_extension: str, processors: List[AsyncProcessor]
     ) -> BaseIngestor:
         if not await self.supports(file_extension):
             return None
-        return XlsxIngestor(processors)
+        return XmlIngestor(processors)
+
 
+class XmlIngestor(BaseIngestor):
+    """Ingestor for xml"""
 
-class XlsxIngestor(BaseIngestor):
     def __init__(self, processors: List[AsyncProcessor]):
-        super().__init__(IngestorBackend.XLSX)
+        super().__init__(IngestorBackend.XML)
         self.processors = processors
-        self.logger = setup_logger(__name__, "XlsxIngestor")
+        self.logger = setup_logger(__name__, "XmlIngestor")
 
     async def ingest(
         self, poll_function: AsyncGenerator[CollectedBytes, None]
     ) -> AsyncGenerator[IngestedTokens, None]:
+        """Ingesting bytes of xml file"""
         current_file = None
         collected_bytes = b""
         try:
             async for chunk_bytes in poll_function:
                 if chunk_bytes.is_error() or chunk_bytes.is_eof():
                     continue
                 if current_file is None:
                     current_file = chunk_bytes.file
                 elif current_file != chunk_bytes.file:
-                    async for data in self.extract_and_process_xlsx(
+                    async for text in self.extract_and_process_xml(
                         CollectedBytes(file=current_file, data=collected_bytes)
                     ):
-                        yield IngestedTokens(
-                            file=current_file,
-                            data=[data],
-                            error=None,
-                            doc_source=chunk_bytes.doc_source
-                        )
+                        yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
                     yield IngestedTokens(
                         file=current_file,
                         data=None,
                         error=None,
                         doc_source=chunk_bytes.doc_source
                     )
                     collected_bytes = b""
                     current_file = chunk_bytes.file
                 collected_bytes += chunk_bytes.data
         except Exception as e:
             yield IngestedTokens(file=current_file, data=None, error=f"Exception: {e}", doc_source=chunk_bytes.doc_source)
         finally:
-            async for data in self.extract_and_process_xlsx(
+            async for text in self.extract_and_process_xml(
                 CollectedBytes(file=current_file, data=collected_bytes)
             ):
-                yield IngestedTokens(
-                    file=current_file,
-                    data=[data],
-                    error=None,
-                    doc_source=chunk_bytes.doc_source
-                )
+                yield IngestedTokens(file=current_file, data=[text], error=None, doc_source=chunk_bytes.doc_source)
+
             yield IngestedTokens(file=current_file, data=None, error=None, doc_source=chunk_bytes.doc_source)
 
-    async def extract_and_process_xlsx(
+    async def extract_and_process_xml(
         self, collected_bytes: CollectedBytes
-    ) -> AsyncGenerator[pd.DataFrame, None]:
-        df = await self.extract_text_from_xlsx(collected_bytes)
-        processed_text = await self.process_data(df.to_string())
+    ) -> AsyncGenerator[str, None]:
+        """Function to extract and process xml files"""
+        text = await self.extract_text_from_xml(collected_bytes)
+        processed_text = await self.process_data(text)
         yield processed_text
 
-    async def extract_text_from_xlsx(
-        self, collected_bytes: CollectedBytes
-    ) -> pd.DataFrame:
-        excel_buffer = io.BytesIO(collected_bytes.data)
-        dataframe = pd.read_excel(excel_buffer)
-        return dataframe
+    async def extract_text_from_xml(self, collected_bytes: CollectedBytes) -> str:
+        """Function to extract text from xml"""
+        text = collected_bytes.data.decode("UTF-8")
+        return text
 
     async def process_data(self, text: str) -> str:
         if self.processors is None or len(self.processors) == 0:
             return text
         try:
             processed_data = text
             for processor in self.processors:
```

### Comparing `querent-3.1.0/querent/kg/ner_helperfunctions/attn_scores.py` & `querent-3.1.1/querent/kg/ner_helperfunctions/attn_scores.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/ner_helperfunctions/contextual_embeddings.py` & `querent-3.1.1/querent/kg/ner_helperfunctions/contextual_embeddings.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/ner_helperfunctions/dependency_parsing.py` & `querent-3.1.1/querent/kg/ner_helperfunctions/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/ner_helperfunctions/filter_triples.py` & `querent-3.1.1/querent/kg/ner_helperfunctions/filter_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/ner_helperfunctions/fixed_entities.py` & `querent-3.1.1/querent/kg/ner_helperfunctions/fixed_entities.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/ner_helperfunctions/fixed_predicate.py` & `querent-3.1.1/querent/kg/ner_helperfunctions/fixed_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/ner_helperfunctions/ner_llm_transformer.py` & `querent-3.1.1/querent/kg/ner_helperfunctions/ner_llm_transformer.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/querent_kg.py` & `querent-3.1.1/querent/kg/querent_kg.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/rel_helperfunctions/contextual_predicate.py` & `querent-3.1.1/querent/kg/rel_helperfunctions/contextual_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/rel_helperfunctions/embedding_store.py` & `querent-3.1.1/querent/kg/rel_helperfunctions/embedding_store.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/rel_helperfunctions/fixed_relationships.py` & `querent-3.1.1/querent/kg/rel_helperfunctions/fixed_relationships.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py` & `querent-3.1.1/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/rel_helperfunctions/openai_functions.py` & `querent-3.1.1/querent/kg/rel_helperfunctions/openai_functions.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/rel_helperfunctions/questionanswer_llama2.py` & `querent-3.1.1/querent/kg/rel_helperfunctions/questionanswer_llama2.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/rel_helperfunctions/rel_normalize.py` & `querent-3.1.1/querent/kg/rel_helperfunctions/rel_normalize.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/kg/rel_helperfunctions/triple_to_json.py` & `querent-3.1.1/querent/kg/rel_helperfunctions/triple_to_json.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/logging/filters.py` & `querent-3.1.1/querent/logging/filters.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/logging/handlers.py` & `querent-3.1.1/querent/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/logging/logger.py` & `querent-3.1.1/querent/logging/logger.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/metric/adapters/promethus_adapter.py` & `querent-3.1.1/querent/metric/adapters/promethus_adapter.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/metric/metric_logging_handler.py` & `querent-3.1.1/querent/metric/metric_logging_handler.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/metric/metric_registry.py` & `querent-3.1.1/querent/metric/metric_registry.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/processors/text_cleanup_processor.py` & `querent-3.1.1/querent/processors/text_cleanup_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/processors/text_processor.py` & `querent-3.1.1/querent/processors/text_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/querent/auto_scaler.py` & `querent-3.1.1/querent/querent/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/querent/querent.py` & `querent-3.1.1/querent/querent/querent.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/querent/resource_manager.py` & `querent-3.1.1/querent/querent/resource_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/storage/gcs_query.py` & `querent-3.1.1/querent/storage/gcs_query.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/storage/milvus_vectorevent_storage.py` & `querent-3.1.1/querent/storage/milvus_vectorevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/storage/neo4j_graphevent_storage.py` & `querent-3.1.1/querent/storage/neo4j_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/storage/postgres_graphevent_storage.py` & `querent-3.1.1/querent/storage/postgres_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/tools/web_page_extractor.py` & `querent-3.1.1/querent/tools/web_page_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/utils/webpage_extractor.py` & `querent-3.1.1/querent/utils/webpage_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/workflow/_helpers.py` & `querent-3.1.1/querent/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent/workflow/workflow.py` & `querent-3.1.1/querent/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent.egg-info/PKG-INFO` & `querent-3.1.1/querent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.1.0
+Version: 3.1.1
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
```

### Comparing `querent-3.1.0/querent.egg-info/SOURCES.txt` & `querent-3.1.1/querent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/querent.egg-info/requires.txt` & `querent-3.1.1/querent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `querent-3.1.0/setup.py` & `querent-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="querent",
-    version="3.1.0",
+    version="3.1.1",
     author="Querent AI",
     description="The Asynchronous Data Dynamo and Graph Neural Network Catalyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Querent-ai/querent-ai",
     project_urls={
         "Documentation": "https://github.com/Querent-ai/querent-ai/docs",
```

