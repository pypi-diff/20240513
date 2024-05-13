# Comparing `tmp/therix-0.1.4.tar.gz` & `tmp/therix-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "therix-0.1.4.tar", max compression
+gzip compressed data, was "therix-0.1.5.tar", max compression
```

## Comparing `therix-0.1.4.tar` & `therix-0.1.5.tar`

### file list

```diff
@@ -1,105 +1,114 @@
--rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.4/LICENSE
--rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.4/README.md
--rw-r--r--   0        0        0     1023 2024-05-09 12:13:10.309807 therix-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.4/therix/__init__.py
--rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.4/therix/alembic/README
--rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.4/therix/alembic/env.py
--rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.4/therix/alembic/script.py.mako
--rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.4/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
--rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.4/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
--rw-r--r--   0        0        0      880 2024-05-08 11:24:55.867083 therix-0.1.4/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py
--rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.4/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
--rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.4/therix/alembic.ini
--rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.4/therix/core/JSONLoader.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.4/therix/core/__init__.py
--rw-r--r--   0        0        0     2371 2024-05-08 11:24:55.868083 therix-0.1.4/therix/core/cache.py
--rw-r--r--   0        0        0     1408 2024-05-03 12:50:17.295817 therix-0.1.4/therix/core/chat_history/base_chat_history.py
--rw-r--r--   0        0        0     1649 2024-05-03 12:50:17.296463 therix-0.1.4/therix/core/constants.py
--rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.4/therix/core/data_sources.py
--rw-r--r--   0        0        0     1676 2024-04-16 12:12:31.276049 therix-0.1.4/therix/core/embedding_models.py
--rw-r--r--   0        0        0     2374 2024-05-03 13:10:49.072728 therix-0.1.4/therix/core/inference_models.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.4/therix/core/output_source.py
--rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.4/therix/core/pii_filter_config.py
--rw-r--r--   0        0        0     5653 2024-05-09 12:03:13.869241 therix-0.1.4/therix/core/pipeline.py
--rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.4/therix/core/pipeline_component.py
--rw-r--r--   0        0        0      238 2024-05-08 11:24:55.868662 therix-0.1.4/therix/core/response.py
--rw-r--r--   0        0        0      588 2024-04-26 09:41:57.772788 therix-0.1.4/therix/core/summarizer_config.py
--rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.4/therix/core/trace.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.4/therix/db/__init__.py
--rw-r--r--   0        0        0     3757 2024-04-29 11:17:18.463868 therix-0.1.4/therix/db/db_manager.py
--rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.4/therix/db/session.py
--rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.4/therix/db/tests/__init__.py
--rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.4/therix/db/tests/test_db_manager.py
--rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.4/therix/docs/.gitignore
--rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.4/therix/docs/README.md
--rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.4/therix/docs/babel.config.js
--rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.4/therix/docs/blog/2019-05-28-first-blog-post.md
--rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.4/therix/docs/blog/2019-05-29-long-blog-post.md
--rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.4/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
--rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.4/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.4/therix/docs/blog/2021-08-26-welcome/index.md
--rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.4/therix/docs/blog/authors.yml
--rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.4/therix/docs/docs/LLM-Proxy/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.4/therix/docs/docs/LLM-Proxy/index.md
--rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.4/therix/docs/docs/core-components/_category_.json
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/_category_.json
--rw-r--r--   0        0        0     3533 2024-05-08 11:24:55.869158 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/caching.md
--rw-r--r--   0        0        0     1288 2024-05-08 11:24:55.869292 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
--rw-r--r--   0        0        0     3959 2024-05-08 11:24:55.869587 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
--rw-r--r--   0        0        0       81 2024-05-03 05:53:02.649008 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/index.md
--rw-r--r--   0        0        0     5496 2024-05-08 11:24:55.869807 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
--rw-r--r--   0        0        0   101843 2024-05-08 11:24:55.870971 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG
--rw-r--r--   0        0        0    87594 2024-05-08 11:24:55.871966 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG
--rw-r--r--   0        0        0     1835 2024-05-08 11:24:55.872168 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/trace.md
--rw-r--r--   0        0        0     1377 2024-05-08 11:24:55.868823 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations.md
--rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.4/therix/docs/docs/core-components/pipeline-templates.md
--rw-r--r--   0        0        0     3488 2024-05-08 11:24:55.872304 therix-0.1.4/therix/docs/docs/core-components/pipeline.md
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.4/therix/docs/docs/introduction/_category_.json
--rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.4/therix/docs/docs/introduction/getting-started.md
--rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.4/therix/docs/docs/introduction/index.md
--rw-r--r--   0        0        0     1813 2024-05-08 11:24:55.872443 therix-0.1.4/therix/docs/docs/introduction/installation.md
--rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.4/therix/docs/docs/observability/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.4/therix/docs/docs/observability/index.md
--rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.4/therix/docs/docs/squad/_category_.json
--rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.4/therix/docs/docs/squad/index.md
--rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.4/therix/docs/docs/usage/_category_.json
--rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.4/therix/docs/docs/usage/index.md
--rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.4/therix/docs/docs/use-cases/_category_.json
--rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.4/therix/docs/docs/use-cases/faq.md
--rw-r--r--   0        0        0     4156 2024-05-08 11:24:55.872787 therix-0.1.4/therix/docs/docs/use-cases/summarizer.md
--rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.4/therix/docs/docusaurus.config.js
--rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.4/therix/docs/package-lock.json
--rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.4/therix/docs/package.json
--rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.4/therix/docs/sidebars.js
--rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.4/therix/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.4/therix/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.4/therix/docs/src/css/custom.css
--rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.4/therix/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.4/therix/docs/src/pages/markdown-page.md
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.4/therix/docs/static/.nojekyll
--rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.4/therix/docs/static/img/coditas.png
--rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.4/therix/docs/static/img/coditasLogo.svg
--rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.4/therix/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.4/therix/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.4/therix/docs/static/img/favicon.ico
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.4/therix/docs/static/img/icon.svg
--rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.4/therix/docs/static/img/logo.png
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.4/therix/docs/static/img/logo.svg
--rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.4/therix/docs/static/img/therix-logo.png
--rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.4/therix/docs/static/img/undraw_docusaurus_mountain.svg
--rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.4/therix/docs/static/img/undraw_docusaurus_react.svg
--rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.4/therix/docs/static/img/undraw_docusaurus_tree.svg
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.4/therix/entities/__init__.py
--rw-r--r--   0        0        0     2535 2024-05-03 12:50:17.297755 therix-0.1.4/therix/entities/models.py
--rw-r--r--   0        0        0     2490 2024-05-08 11:24:55.873082 therix-0.1.4/therix/examples/cache_config_example.py
--rw-r--r--   0        0        0     1745 2024-05-08 11:24:55.873332 therix-0.1.4/therix/examples/pii_filter_example.py
--rw-r--r--   0        0        0     6206 2024-05-08 11:24:55.873927 therix-0.1.4/therix/examples/summarizer_example.py
--rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.4/therix/pylintrc
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.4/therix/services/__init__.py
--rw-r--r--   0        0        0     4434 2024-05-09 12:03:21.346863 therix-0.1.4/therix/services/pipeline_service.py
--rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.4/therix/services/web_crawling.py
--rw-r--r--   0        0        0      602 2024-05-08 11:24:55.874269 therix-0.1.4/therix/tests/test_pii_filter.py
--rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.4/therix/utils/pii_filter.py
--rw-r--r--   0        0        0    10916 2024-05-09 12:03:21.347328 therix-0.1.4/therix/utils/rag.py
--rw-r--r--   0        0        0     4074 2024-05-08 11:24:55.875542 therix-0.1.4/therix/utils/summarizer.py
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 therix-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.5/README.md
+-rw-r--r--   0        0        0     1048 2024-05-13 10:00:57.830665 therix-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.5/therix/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.5/therix/alembic/README
+-rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.5/therix/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.5/therix/alembic/script.py.mako
+-rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.5/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
+-rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.5/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
+-rw-r--r--   0        0        0      880 2024-05-08 11:24:55.867083 therix-0.1.5/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py
+-rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.5/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
+-rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.5/therix/alembic.ini
+-rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.5/therix/core/JSONLoader.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.5/therix/core/__init__.py
+-rw-r--r--   0        0        0     2737 2024-05-13 10:00:13.299373 therix-0.1.5/therix/core/cache.py
+-rw-r--r--   0        0        0     1399 2024-05-13 10:00:13.301278 therix-0.1.5/therix/core/chat_history/base_chat_history.py
+-rw-r--r--   0        0        0     1649 2024-05-13 10:00:13.301411 therix-0.1.5/therix/core/constants.py
+-rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.5/therix/core/data_sources.py
+-rw-r--r--   0        0        0     1676 2024-04-16 12:12:31.276049 therix-0.1.5/therix/core/embedding_models.py
+-rw-r--r--   0        0        0     2374 2024-05-13 10:00:13.301910 therix-0.1.5/therix/core/inference_models.py
+-rw-r--r--   0        0        0      317 2024-05-13 10:00:13.302010 therix-0.1.5/therix/core/output_parser.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.5/therix/core/output_source.py
+-rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.5/therix/core/pii_filter_config.py
+-rw-r--r--   0        0        0     6171 2024-05-13 10:00:13.302291 therix-0.1.5/therix/core/pipeline.py
+-rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.5/therix/core/pipeline_component.py
+-rw-r--r--   0        0        0      238 2024-05-08 11:24:55.868662 therix-0.1.5/therix/core/response.py
+-rw-r--r--   0        0        0      594 2024-05-13 10:00:13.302774 therix-0.1.5/therix/core/summarizer_config.py
+-rw-r--r--   0        0        0       98 2024-05-13 10:00:13.302847 therix-0.1.5/therix/core/summarizer_output_model.py
+-rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.5/therix/core/trace.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.5/therix/db/__init__.py
+-rw-r--r--   0        0        0     3757 2024-04-29 11:17:18.463868 therix-0.1.5/therix/db/db_manager.py
+-rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.5/therix/db/session.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.5/therix/db/tests/__init__.py
+-rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.5/therix/db/tests/test_db_manager.py
+-rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.5/therix/docs/.gitignore
+-rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.5/therix/docs/README.md
+-rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.5/therix/docs/babel.config.js
+-rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.5/therix/docs/blog/2019-05-28-first-blog-post.md
+-rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.5/therix/docs/blog/2019-05-29-long-blog-post.md
+-rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.5/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
+-rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.5/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.5/therix/docs/blog/2021-08-26-welcome/index.md
+-rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.5/therix/docs/blog/authors.yml
+-rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.5/therix/docs/docs/LLM-Proxy/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.5/therix/docs/docs/LLM-Proxy/index.md
+-rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.5/therix/docs/docs/core-components/_category_.json
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/_category_.json
+-rw-r--r--   0        0        0     3533 2024-05-08 11:24:55.869158 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/caching.md
+-rw-r--r--   0        0        0     1288 2024-05-08 11:24:55.869292 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
+-rw-r--r--   0        0        0     3959 2024-05-08 11:24:55.869587 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
+-rw-r--r--   0        0        0     5428 2024-05-13 10:00:13.303279 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
+-rw-r--r--   0        0        0   101843 2024-05-08 11:24:55.870971 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG
+-rw-r--r--   0        0        0    87594 2024-05-08 11:24:55.871966 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG
+-rw-r--r--   0        0        0     1835 2024-05-08 11:24:55.872168 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/trace.md
+-rw-r--r--   0        0        0     1377 2024-05-08 11:24:55.868823 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations.md
+-rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.5/therix/docs/docs/core-components/pipeline-templates.md
+-rw-r--r--   0        0        0     3488 2024-05-08 11:24:55.872304 therix-0.1.5/therix/docs/docs/core-components/pipeline.md
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.5/therix/docs/docs/introduction/_category_.json
+-rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.5/therix/docs/docs/introduction/getting-started.md
+-rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.5/therix/docs/docs/introduction/index.md
+-rw-r--r--   0        0        0     1813 2024-05-08 11:24:55.872443 therix-0.1.5/therix/docs/docs/introduction/installation.md
+-rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.5/therix/docs/docs/observability/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.5/therix/docs/docs/observability/index.md
+-rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.5/therix/docs/docs/squad/_category_.json
+-rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.5/therix/docs/docs/squad/index.md
+-rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.5/therix/docs/docs/usage/_category_.json
+-rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.5/therix/docs/docs/usage/index.md
+-rw-r--r--   0        0        0     3717 2024-05-13 10:00:13.303378 therix-0.1.5/therix/docs/docs/use-cases/Keyword Search.md
+-rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.5/therix/docs/docs/use-cases/_category_.json
+-rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.5/therix/docs/docs/use-cases/faq.md
+-rw-r--r--   0        0        0     3579 2024-05-13 10:00:13.303497 therix-0.1.5/therix/docs/docs/use-cases/pii_filer.md
+-rw-r--r--   0        0        0     4177 2024-05-13 10:00:13.303673 therix-0.1.5/therix/docs/docs/use-cases/summarizer.md
+-rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.5/therix/docs/docusaurus.config.js
+-rw-r--r--   0        0        0      133 2024-05-13 10:00:13.303753 therix-0.1.5/therix/docs/firebase.json
+-rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.5/therix/docs/package-lock.json
+-rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.5/therix/docs/package.json
+-rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.5/therix/docs/sidebars.js
+-rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.5/therix/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.5/therix/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.5/therix/docs/src/css/custom.css
+-rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.5/therix/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.5/therix/docs/src/pages/markdown-page.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.5/therix/docs/static/.nojekyll
+-rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.5/therix/docs/static/img/coditas.png
+-rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.5/therix/docs/static/img/coditasLogo.svg
+-rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.5/therix/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.5/therix/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.5/therix/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.5/therix/docs/static/img/icon.svg
+-rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.5/therix/docs/static/img/logo.png
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.5/therix/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.5/therix/docs/static/img/therix-logo.png
+-rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.5/therix/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.5/therix/docs/static/img/undraw_docusaurus_react.svg
+-rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.5/therix/docs/static/img/undraw_docusaurus_tree.svg
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.5/therix/entities/__init__.py
+-rw-r--r--   0        0        0     2535 2024-05-03 12:50:17.297755 therix-0.1.5/therix/entities/models.py
+-rw-r--r--   0        0        0     2489 2024-05-13 10:00:13.304041 therix-0.1.5/therix/examples/cache_config_example.py
+-rw-r--r--   0        0        0     2720 2024-05-13 10:00:13.304169 therix-0.1.5/therix/examples/keyword_search_examples.py
+-rw-r--r--   0        0        0     3231 2024-05-13 10:00:13.304273 therix-0.1.5/therix/examples/main.py
+-rw-r--r--   0        0        0     1839 2024-05-13 10:00:13.304440 therix-0.1.5/therix/examples/pii_filter_example.py
+-rw-r--r--   0        0        0     6424 2024-05-13 10:00:13.304598 therix-0.1.5/therix/examples/summarizer_example.py
+-rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.5/therix/pylintrc
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.5/therix/services/__init__.py
+-rw-r--r--   0        0        0     7209 2024-05-13 10:00:13.304760 therix-0.1.5/therix/services/pipeline_service.py
+-rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.5/therix/services/web_crawling.py
+-rw-r--r--   0        0        0     2077 2024-05-13 10:00:13.304865 therix-0.1.5/therix/tests/test_cache.py
+-rw-r--r--   0        0        0      602 2024-05-08 11:24:55.874269 therix-0.1.5/therix/tests/test_pii_filter.py
+-rw-r--r--   0        0        0     8197 2024-05-13 10:00:13.305133 therix-0.1.5/therix/tests/test_summarizer.py
+-rw-r--r--   0        0        0     3304 2024-05-13 10:00:13.305224 therix-0.1.5/therix/utils/keyword_search.py
+-rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.5/therix/utils/pii_filter.py
+-rw-r--r--   0        0        0    10981 2024-05-13 10:00:13.305523 therix-0.1.5/therix/utils/rag.py
+-rw-r--r--   0        0        0     4591 2024-05-13 10:00:13.305701 therix-0.1.5/therix/utils/summarizer.py
+-rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 therix-0.1.5/PKG-INFO
```

### Comparing `therix-0.1.4/LICENSE` & `therix-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/README.md` & `therix-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/pyproject.toml` & `therix-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "therix"
-version = "0.1.4"
+version = "0.1.5"
 description = "Therix is the SDK for langchain based applications."
 authors = ["Ajinath"]
 license = "MIT"
 readme = "README.md"
 include = ["alembic/**/*", "alembic.ini"]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.10"
 wheel = "^0.43.0"
 alembic = "1.13.1"
 psycopg2-binary = "2.9.9"
 sqlalchemy = "2.0.28"
 pgvector = "0.2.5"
 langchain = "0.1.13"
 langchain-openai = "0.1.1"
@@ -29,14 +29,15 @@
 psycopg = {extras = ["binary", "pool"], version = "^3.1.18"}
 langchain-groq = "^0.1.0"
 boto3 = "^1.34.81"
 pylint = "^3.1.0"
 coverage = "^7.4.4"
 pytest-cov = "^5.0.0"
 langchain-postgres = "^0.0.3"
+transformers = "^4.40.2"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 pytest = "^8.1.1"
 pytest-mock = "^3.14.0"
 
 [build-system]
```

### Comparing `therix-0.1.4/therix/alembic/env.py` & `therix-0.1.5/therix/alembic/env.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/alembic/script.py.mako` & `therix-0.1.5/therix/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py` & `therix-0.1.5/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py` & `therix-0.1.5/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py` & `therix-0.1.5/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py` & `therix-0.1.5/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/alembic.ini` & `therix-0.1.5/therix/alembic.ini`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/core/JSONLoader.py` & `therix-0.1.5/therix/core/JSONLoader.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/core/cache.py` & `therix-0.1.5/therix/core/cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import uuid
 from sqlalchemy.ext.declarative import declarative_base
 from therix.core.pipeline_component import PipelineComponent
 from therix.entities.models import ConfigType
 import logging
 from sqlalchemy.dialects.postgresql import UUID
 from therix.db.db_manager import DatabaseManager
 from typing import Type
@@ -45,27 +46,37 @@
     def __init__(self, engine: Engine, cache_schema: Type[FulltextLLMCache] = FulltextLLMCache):
         self.engine = engine
         self.cache_schema = cache_schema
         self.cache_schema.metadata.create_all(self.engine)
 
 
     def lookup(self, question: str, llm_string: str, pipeline_id):
-        """Update cache based on prompt, llm_string, and pipeline_id."""
+        if not isinstance(pipeline_id, uuid.UUID):
+            try:
+                pipeline_id = uuid.UUID(pipeline_id)
+            except ValueError:
+                raise ValueError("pipeline_id is not a valid UUID")
         session = db_manager.get_session()
         query = session.query(FulltextLLMCache).filter(
             FulltextLLMCache.question == question,
             FulltextLLMCache.pipeline_id == pipeline_id
         )
         result = query.first()
         session.close()
-        return result.response
+        return result
         
     
     
-    def update(self, prompt: str, llm_string: str, answer, pipeline_id: str) -> None:
+    def update(self, prompt: str, llm_string: str, answer, pipeline_id) -> None:
+
+        if not isinstance(pipeline_id, uuid.UUID):
+            try:
+                pipeline_id = uuid.UUID(pipeline_id)
+            except ValueError:
+                raise ValueError("pipeline_id is not a valid UUID")
         session = db_manager.get_session()
         cache_entry = FulltextLLMCache(
             question=prompt,
             llm=llm_string,
             response=answer,
             pipeline_id=pipeline_id
         )
```

### Comparing `therix-0.1.4/therix/core/chat_history/base_chat_history.py` & `therix-0.1.5/therix/core/chat_history/base_chat_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
    
     def __init__(
         self,
         session_id,
         pipeline_id:str,
         engine,
         table_name: str,
-        
     ): 
          self.sync_connection = psycopg.connect(SQLALCHEMY_DATABASE_URL)
          super().__init__(table_name,session_id,sync_connection=self.sync_connection)
          self.session_id = session_id
          self.table_name = table_name
          self.pipeline_id=pipeline_id
```

### Comparing `therix-0.1.4/therix/core/constants.py` & `therix-0.1.5/therix/core/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     OPENAI_GPT_3_5_TURBO = 'gpt-3.5-turbo'
     OPENAI_GPT_3_5_TURBO_INSTRUCT = 'gpt-3.5-turbo-instruct'
     AZURE_GPT_4_TURBO_PREVIEW = 'gpt-4-turbo-preview'
     AZURE_GPT_4 = 'gpt-4'
     AZURE_GPT_3_5_TURBO = 'gpt-3.5-turbo'
     AZURE_GPT_3_5_TURBO_INSTRUCT = 'gpt-3.5-turbo-instruct'
     GROQ_LLM_MIXTRAL_8_7_B='mixtral-8x7b-32768'
-    GROQ_LLM_LLAMA2_70B= 'llama2-70b-4096'
+    GROQ_LLM_LLAMA3_70B= 'llama3-70b-8192'
     GROQ_LLM_GEMMA7B= 'gemma-7b-it'
     BEDROCK_TEXT_EXPRES_V1='amazon.titan-text-express-v1'
     BEDROCK_TEXT_LITE_G1='amazon.titan-text-lite-v1'
 
 class OutputSourceMaster:
     S3 = "S3"
     LOCAL = "LOCAL"
```

### Comparing `therix-0.1.4/therix/core/data_sources.py` & `therix-0.1.5/therix/core/data_sources.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/core/embedding_models.py` & `therix-0.1.5/therix/core/embedding_models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/core/inference_models.py` & `therix-0.1.5/therix/core/inference_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 
 
 class GroqGemma7B(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.GROQ_LLM_GEMMA7B, config=config)
 
 
-class GroqLlama270b(InferenceModel):
+class GroqLlama370b(InferenceModel):
     def __init__(self, config: dict):
-        super().__init__(name=InferenceModelMaster.GROQ_LLM_LLAMA2_70B, config=config)
+        super().__init__(name=InferenceModelMaster.GROQ_LLM_LLAMA3_70B, config=config)
 
 
 class BedrockTextExpressV1(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(
             name=InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1, config=config
         )
```

### Comparing `therix-0.1.4/therix/core/pipeline.py` & `therix-0.1.5/therix/core/pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -89,40 +89,46 @@
         self.id = self.pipeline_data.id
         self.name = self.pipeline_data.name
         return self.pipeline_data
 
     def preprocess_data(self):
        return self.pipeline_service.preprocess_data(self.pipeline_data.id)
 
-    def invoke(self, question, session_id=None):
+    def invoke(self, question=None, session_id=None , keyword_search_params=None):
             cached_response = None
             therix_cache = TherixCache(engine)
             inference_model = self.pipeline_service.get_pipeline_configuraitons_by_type(self.pipeline_data.id, ConfigType.INFERENCE_MODEL)
 
             if session_id is None:
                 session_id = uuid4()
             add_cache = self.pipeline_service.get_pipeline_configuraitons_by_type(self.pipeline_data.id, ConfigType.CACHE_CONFIG)
             
+            if(question == None and keyword_search_params == None):
+                return "Please provide the required Parameters to invoke the pipeline"
 
             pipeline_trace_config = self.pipeline_service.get_pipeline_configuraitons_by_type(
                 self.pipeline_data.id, ConfigType.TRACE_DETAILS
             )
             trace_details = pipeline_trace_config[0].config if pipeline_trace_config else None
 
             pipeline_type = self.pipeline_service.get_pipeline(self.pipeline_data.id).type.value
-            model_response = ModelResponse()
 
             if pipeline_type == PipelineTypeMaster.RAG.value:
                 if add_cache:
                     cached_response = therix_cache.lookup(question, inference_model[0].name, self.pipeline_data.id)
                 if cached_response:
                     return ModelResponse(cached_response, session_id).create_response()
-                answer = self.pipeline_service.invoke_pipeline(
-                    self.pipeline_data.id, question, session_id, trace_details
-                )
+                if (keyword_search_params and question == None):
+                    keyword_search_params['pipeline_id'] = self.pipeline_data.id
+                    keyword_search_params['trace_details'] = trace_details
+                    answer = self.pipeline_service.search_keywords(keyword_search_params)
+                else:
+                    answer = self.pipeline_service.invoke_pipeline(
+                        self.pipeline_data.id, question, session_id, trace_details
+                    )
                 if add_cache:
                     therix_cache.update(question, inference_model[0].name, answer, self.pipeline_data.id)
             elif pipeline_type == PipelineTypeMaster.SUMMARIZER.value:
-                answer = self.pipeline_service.invoke_summarizer_pipeline(self.pipeline_data.id, text=question)
+                answer = self.pipeline_service.invoke_summarizer_pipeline(self.pipeline_data.id, text=question, trace_details=trace_details)
             
             return ModelResponse(answer, session_id).create_response()
```

### Comparing `therix-0.1.4/therix/core/pipeline_component.py` & `therix-0.1.5/therix/core/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/core/summarizer_config.py` & `therix-0.1.5/therix/core/summarizer_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 
 class SummarizerConfig(PipelineComponent):
     def __init__(self, summarization_type, pydantic_model = None):
         parser = JsonOutputParser(pydantic_object=pydantic_model)
         json_prompt = parser.get_format_instructions()
         config = {
         'pydantic_model' : json_prompt,
-        'summarization_type' : summarization_type
+        'summarization_type' : summarization_type.value
         }
         super().__init__(ConfigType.SUMMARIZER, 'SUMMARIZER', config)
```

### Comparing `therix-0.1.4/therix/db/db_manager.py` & `therix-0.1.5/therix/db/db_manager.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/db/tests/test_db_manager.py` & `therix-0.1.5/therix/db/tests/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/README.md` & `therix-0.1.5/therix/docs/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/blog/2019-05-29-long-blog-post.md` & `therix-0.1.5/therix/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `therix-0.1.5/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/blog/2021-08-26-welcome/index.md` & `therix-0.1.5/therix/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/caching.md` & `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/caching.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/data-sources.md` & `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/data-sources.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md` & `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/inference-model.md` & `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/inference-model.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,155 +7,155 @@
 
 Inference models are neural network architectures designed for natural language processing tasks. They analyze input text to generate responses, answer questions, make predections, or summarize content. 
 
 In Therix, we make it easy to use many popular inference models. You can choose the best one for your needs, depending on what you're trying to do. Whether you're analyzing data, recognizing patterns, or making predictions, we've got you covered with simple integration and a variety of options to suit your specific use case.
 
 
 
-## 1. OpenAIGPT35TurboInferenceModel
+## 1. OpenAI GPT3.5 Turbo
 
 - Import the OpenAIGPT35TurboInferenceModel model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import OpenAIGPT35TurboInferenceModel
 ```
 
 - Add the model to pipeline configurations using the add method
 
 ```python
 .add(OpenAIGPT35TurboInferenceModel(config={'api_key': // Your openAi API key here}))
 ```
 
-## 2. OpenAIGPT4InferenceModel
+## 2. OpenAI GPT4 
 
 - Import the OpenAIGPT4InferenceModel model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import OpenAIGPT4InferenceModel
 ```
 
 - Add the model to pipeline configurations using the add method.
 
 ```python
 .add(OpenAIGPT4InferenceModel(config={'api_key': // Your openAi API key here}))
 ```
 
-## 3. OpenAIGPT4TurboPreviewInferenceModel
+## 3. OpenAI GPT4 Turbo Preview
 
 - Import the OpenAIGPT4TurboPreviewInferenceModel model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import OpenAIGPT4TurboPreviewInferenceModel
 ```
 
 - Add the model to pipeline configurations using the add method.
 
 ```python
 .add(OpenAIGPT4TurboPreviewInferenceModel(config={'api_key': // Your openAi API key here}))
 ```
 
-## 4. AzureOpenAIGPT3TurboPreviewInferenceModel
+## 4. Azure OpenAI GPT3 Turbo Preview
 
 - Import the AzureOpenAIGPT3TurboPreviewInferenceModel model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import AzureOpenAIGPT3TurboPreviewInferenceModel
 ```
 
 - Add the model to pipeline configurations using the add method.
 
 ```python
 .add(AzureOpenAIGPT3TurboPreviewInferenceModel(config={'azure_api_key': // Your azure API key here}))
 ```
 
-## 5. AzureOpenAIGPT3TurboInstructnferenceModel
+## 5. Azure OpenAI GPT3 Turbo Instructnference Model
 
 - Import the AzureOpenAIGPT3TurboInstructnferenceModel model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import AzureOpenAIGPT3TurboInstructnferenceModel
 ```
 
 - Add the model to pipeline configurations using the add method.
 
 ```python
 .add(AzureOpenAIGPT3TurboInstructnferenceModel(config={'azure_api_key': // Your azure API key here}))
 ```
 
-## 6. AzureOpenAIGPT4InferenceModel
+## 6. Azure OpenAI GPT4 
 
 - Import the AzureOpenAIGPT4InferenceModel model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import AzureOpenAIGPT4InferenceModel
 ```
 
 - Add the model to pipeline configurations using the add method.
 
 ```python
 .add(AzureOpenAIGPT4InferenceModel(config={'azure_api_key': // Your azure API key here}))
 ```
 
-## 7. AzureOpenAIGPT4TurboPreviewInferenceModel
+## 7. Azure OpenAI GPT4 Turbo Preview
 
 - Import the AzureOpenAIGPT4TurboPreviewInferenceModel model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import AzureOpenAIGPT4TurboPreviewInferenceModel
 ```
 
 - Add the model to pipeline configurations using the add method.
 
 ```python
 .add(AzureOpenAIGPT4TurboPreviewInferenceModel(config={'azure_api_key': // Your azure API key here}))
 ```
 
-## 8. GroqMixtral87bInferenceModel
+## 8. Groq Mixtral87b
 
 - Import the GroqMixtral87bInferenceModel model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import GroqMixtral87bInferenceModel
 ```
 
 - Add the model to pipeline configurations using the add method.
 
 ```python
 .add(GroqMixtral87bInferenceModel(config={'groq_api_key': // Your groq API key here}))
 ```
 
-## 9. GroqGemma7B
+## 9. Groq Gemma7B
 
 - Import the GroqGemma7B model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import GroqGemma7B
 ```
 
 - Add the model to pipeline configurations using the add method.
 
 ```python
 .add(GroqGemma7B(config={'groq_api_key': // Your groq API key here}))
 ```
 
-## 10. GroqLlama270b
+## 10. Groq Llama3x70b
 
-- Import the GroqLlama270b model from therix.core.inference_models
+- Import the GroqLlama370b model from therix.core.inference_models
 
 ```python
-from therix.core.inference_models import GroqLlama270b
+from therix.core.inference_models import GroqLlama370b
 ```
 
 - Add the model to pipeline configurations using the add method.
 
 ```python
-.add(GroqLlama270b(config={'groq_api_key': // Your groq API key here}))
+.add(GroqLlama370b(config={'groq_api_key': // Your groq API key here}))
 ```
 
-## 11. BedrockTextExpressV1
+## 11. Bedrock Text ExpressV1
 
 - Import the BedrockTextExpressV1 model from therix.core.inference_models
 
 ```python
 from therix.core.inference_models import BedrockTextExpressV1
 ```
```

### Comparing `therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG` & `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG` & `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/trace.md` & `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/trace.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations.md` & `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/core-components/pipeline.md` & `therix-0.1.5/therix/docs/docs/core-components/pipeline.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/introduction/getting-started.md` & `therix-0.1.5/therix/docs/docs/introduction/getting-started.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/introduction/index.md` & `therix-0.1.5/therix/docs/docs/introduction/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/introduction/installation.md` & `therix-0.1.5/therix/docs/docs/introduction/installation.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/docs/use-cases/summarizer.md` & `therix-0.1.5/therix/docs/docs/use-cases/summarizer.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 {'answer': '\nBeets are a root vegetable rich in fiber, folate, manganese, and antioxidants, and can improve athletic performance and reduce blood pressure. More research is needed to fully understand their health benefits.', 'session_id': UUID('b9548328-6982-40e9-9cea-06208090f25f')}
 ```
 
 ## Summarizer - Extractive
 
 In the Extractive Summarizer of Therix, the aim is to make a brief summary of a text in a JSON format. It picks out important sentences or phrases from the text and puts them in a structured way in JSON.
 
-If you don't specify a Pydantic model, the system itself decides how to organize the summary in JSON, making sure it's clear and concise.
-But users can also give a Pydantic model to customize how the information is organized in the JSON. This gives more control over how the summary looks.
+Users can also give a custom model to customize how the information is organized in the JSON. This gives more control over how the summary looks.
+If you don't specify a custom model, the system itself decides how to organize the summary in JSON, making sure it's clear and concise.
 
-Whether using the default JSON setup or a customized Pydantic model, the result is a neat and informative summary in JSON. This helps in understanding big chunks of text quickly and making decisions based on them in different fields.
+Whether using the default JSON setup or a custom model, the result is a neat and informative summary in JSON. This helps in understanding big chunks of text quickly and making decisions based on them in different fields.
 
-The sample model used here is extended from the BaseModel of Pydantic.
+Custom model is made by extending from the SummarizerOutputModel of therix.
 ```python
-from langchain_core.pydantic_v1 import BaseModel
+from therix.core.summarizer_output_model import SummarizerOutputModel
 
-class TopicModel(BaseModel):
+class TopicModel(SummarizerOutputModel):
     mainTopic: str
     subTopic1: str
     subTopic2: str
 ```
 
 **Sample Output:**
 ```python
@@ -46,44 +46,44 @@
 
 ## How you can integrate summarizer in your code:
 
 - Import Necessary Modules: Begin by importing the required modules for configuring the Summarizer.
 
 ```python
 from therix.summarizer import SummarizerConfig, SummarizerTypeMaster
-from your_model_module import TopicModel  # Import your Pydantic model if needed
+from therix.core.summarizer_output_model import SummarizerOutputModel  # Import SummarizerOutputModel if needed
 ```
 
 - Instantiate SummarizerConfig:
 
 Create an instance of the SummarizerConfig class by specifying the type of summarizer and, optionally, the Pydantic model for structuring the JSON output.
 
 - **For Extractive Summarizer with custom Pydantic model**
 ```python
-summarizer_config = SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE.value, TopicModel)
+summarizer_config = SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE, TopicModel)
 ```
 
 - **For Abstractive Summarizer**
 ```python
-summarizer_config = SummarizerConfig(SummarizerTypeMaster.ABSTRACTIVE.value)
+summarizer_config = SummarizerConfig(SummarizerTypeMaster.ABSTRACTIVE)
 ```
 
 - Add Summarizer Configuration to Pipeline: Use the .add() method to add the SummarizerConfig to your Therix pipeline.
 
 ```python
 pipeline.add(summarizer_config)
 ```
 
 ## Example
 
 ```python
 pipeline = Pipeline(name="Summarizer Pipeline")
     (pipeline
-    .add(SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE.value,TopicModel))
+    .add(SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE,TopicModel))
     .add(// Any other configuration you want to add)
     .save())
 
     pipeline.publish()
     answer = pipeline.invoke(text)
 ```
 
-By following these steps and adjusting the parameters as needed, you can seamlessly integrate the Summarizer into your Therix pipeline. Whether you require Extractive or Abstractive summarization, with or without a custom Pydantic model, Therix provides the flexibility and functionality to meet your summarization needs effectively.
+By following these steps and adjusting the parameters as needed, you can seamlessly integrate the Summarizer into your Therix pipeline. Whether you require Extractive or Abstractive summarization, with or without a custom model, Therix provides the flexibility and functionality to meet your summarization needs effectively.
```

### Comparing `therix-0.1.4/therix/docs/docusaurus.config.js` & `therix-0.1.5/therix/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/package-lock.json` & `therix-0.1.5/therix/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/package.json` & `therix-0.1.5/therix/docs/package.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/sidebars.js` & `therix-0.1.5/therix/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/src/components/HomepageFeatures/index.js` & `therix-0.1.5/therix/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/src/css/custom.css` & `therix-0.1.5/therix/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/coditas.png` & `therix-0.1.5/therix/docs/static/img/coditas.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/coditasLogo.svg` & `therix-0.1.5/therix/docs/static/img/coditasLogo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/docusaurus-social-card.jpg` & `therix-0.1.5/therix/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/docusaurus.png` & `therix-0.1.5/therix/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/favicon.ico` & `therix-0.1.5/therix/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/icon.svg` & `therix-0.1.5/therix/docs/static/img/icon.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/logo.png` & `therix-0.1.5/therix/docs/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/logo.svg` & `therix-0.1.5/therix/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/therix-logo.png` & `therix-0.1.5/therix/docs/static/img/therix-logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/undraw_docusaurus_mountain.svg` & `therix-0.1.5/therix/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/undraw_docusaurus_react.svg` & `therix-0.1.5/therix/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/docs/static/img/undraw_docusaurus_tree.svg` & `therix-0.1.5/therix/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/entities/models.py` & `therix-0.1.5/therix/entities/models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/examples/cache_config_example.py` & `therix-0.1.5/therix/examples/cache_config_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     }))
     .add(CacheConfig(config={}))
     .save())
 
     pipeline.publish()
     pipeline.preprocess_data()
     print(pipeline.id)
-    ans = pipeline.invoke("What are some use cases of RAT?",)
+    ans = pipeline.invoke("What are some use cases of RAT?")
 
     print(ans)
 
 
     end_time = time.process_time()
```

### Comparing `therix-0.1.4/therix/examples/pii_filter_example.py` & `therix-0.1.5/therix/examples/pii_filter_example.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from therix.core.data_sources import PDFDataSource
-from therix.core.embedding_models import AzureOpenAIEmbedding3SmallEmbeddingModel, OpenAITextAdaEmbeddingModel
-from therix.core.inference_models import AzureOpenAIGPT3TurboPreviewInferenceModel, GroqMixtral87bInferenceModel, OpenAIGPT4TurboPreviewInferenceModel
-from therix.core.inference_models import AzureOpenAIGPT3TurboPreviewInferenceModel, OpenAIGPT4TurboPreviewInferenceModel
-from therix.core.embedding_models import BedrockTitanEmbedding, OpenAITextAdaEmbeddingModel
-from therix.core.inference_models import BedrockTextExpressV1, OpenAIGPT4TurboPreviewInferenceModel
+from therix.core.inference_models import GroqMixtral87bInferenceModel
+from therix.core.embedding_models import BedrockTitanEmbedding
 from therix.core.pii_filter_config import PIIFilterConfig
 from therix.core.pipeline import Pipeline
 import sys
+from therix.core.trace import Trace
 
 
 
 # TODO: Init therix with DB details, and license key
 
 
 ## Usage:
@@ -22,20 +20,29 @@
     pipeline = Pipeline.from_id(sys.argv[1])
     question = sys.argv[2]
     ans = pipeline.invoke(question)
     print(ans)
 else:
     pipeline = Pipeline(name="My New Published Pipeline")
     (pipeline
-    .add(PDFDataSource(config={'files': ['./test-data/Essay-on-Lata-Mangeshkar-final.pdf']}))
-    .add(OpenAITextAdaEmbeddingModel(config={'api_key': OPENAI_API_KEY}))
-    .add(OpenAIGPT4TurboPreviewInferenceModel(config={'api_key': OPENAI_API_KEY}))
+    .add(PDFDataSource(config={'files': ['../../test-data/Essay-on-Lata-Mangeshkar-final.pdf']}))
+    .add(BedrockTitanEmbedding(config={ "bedrock_aws_access_key_id":"",
+                                            "bedrock_aws_secret_access_key" : "",
+                                            "bedrock_aws_session_token" : "",
+                                            "bedrock_region_name" : "us-east-1"
+                                            }))
+    .add(GroqMixtral87bInferenceModel(config={"groq_api_key": 'your groq api key'}))
     .add(PIIFilterConfig(config={
         'entities': ['PERSON','PHONE_NUMBER','EMAIL_ADDRESS']
     }))
+    .add(Trace(config={
+        'secret_key': 'sk-lf-e62aa7ce-c4c8-4c77-ad7d-9d76dfd96db1',
+        'public_key': 'pk-lf-282ad728-c1d6-4247-b6cd-8022198591a9',
+        'identifier': 'my own pipeline'
+    }))
     .save())
 
     pipeline.publish()
     pipeline.preprocess_data()
     print(pipeline.id)
     ans = pipeline.invoke("Whom is the data about? And what are their personal details?")
```

### Comparing `therix-0.1.4/therix/examples/summarizer_example.py` & `therix-0.1.5/therix/examples/summarizer_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from therix.core.inference_models import GroqMixtral87bInferenceModel, OpenAIGPT4TurboPreviewInferenceModel
+from therix.core.inference_models import GroqMixtral87bInferenceModel
 from therix.core.pipeline import Pipeline
 import sys
+from therix.core.summarizer_output_model import SummarizerOutputModel
 from therix.core.summarizer_config import SummarizerConfig
+from therix.core.trace import Trace
 from therix.utils.summarizer import SummarizerTypeMaster
 
 
-
-# TODO: Init therix with DB details, and license key
-
-from langchain_core.pydantic_v1 import BaseModel
-
-class TopicModel(BaseModel):
+class TopicModel(SummarizerOutputModel):
     mainTopic: str
     subTopic1: str
     subTopic2: str
 
 ## Usage:
 # python main.py ad11128d-d2ec-4f7c-8d87-15c1a5dfe1a9 "how does it help in reasoning?"
 
@@ -98,16 +95,21 @@
     question = sys.argv[2]
     ans = pipeline.invoke(question)
     print(ans)
 else:
     pipeline = Pipeline(name="Summarizer Pipeline")
 
     (pipeline
-    .add(OpenAIGPT4TurboPreviewInferenceModel(config={'api_key': OPENAI_API_KEY}))
-    .add(SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE.value,TopicModel))
+    .add(GroqMixtral87bInferenceModel(config={"groq_api_key": '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'}))
+    .add(SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE,TopicModel))
+    .add(Trace(config={
+        'secret_key': 'sk-lf-e62aa7ce-c4c8-4c77-ad7d-9d76dfd96db1',
+        'public_key': 'pk-lf-282ad728-c1d6-4247-b6cd-8022198591a9',
+        'identifier': 'my own pipeline'
+    }))
     .save())
 
     pipeline.publish()
     print(pipeline.id)
     ans = pipeline.invoke(text)
 
     print(ans)
```

### Comparing `therix-0.1.4/therix/pylintrc` & `therix-0.1.5/therix/pylintrc`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/services/web_crawling.py` & `therix-0.1.5/therix/services/web_crawling.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/tests/test_pii_filter.py` & `therix-0.1.5/therix/tests/test_pii_filter.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/utils/pii_filter.py` & `therix-0.1.5/therix/utils/pii_filter.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.4/therix/utils/rag.py` & `therix-0.1.5/therix/utils/rag.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from operator import itemgetter
 from pathlib import Path
 from urllib import response
 from langchain.docstore.document import Document
 from langchain_community.document_loaders import TextLoader, PyPDFLoader
 from langchain_community.vectorstores.pgvector import PGVector
 from langchain_openai import OpenAIEmbeddings, ChatOpenAI
-from langchain_openai import AzureOpenAI
+from langchain_openai import AzureChatOpenAI
 from langchain_groq import ChatGroq
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_community.document_loaders.youtube import YoutubeLoader
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_openai import AzureOpenAIEmbeddings
 from therix.core.JSONLoader import JSONLoader
@@ -59,15 +59,14 @@
     elif file_type == DataSourceMaster.WEBSITE:
         return JSONLoader(file_path)
     else:
         raise ValueError(f"Unknown data source type: {file_type}")
 
 
 def get_embedding_model(embedding_model_name, config):
-    print(embedding_model_name, config)
     if (
         embedding_model_name == EmbeddingModelMaster.OPENAI_TEXT_ADA
         or embedding_model_name == EmbeddingModelMaster.OPENAI_TEXT_EMBEDDING_3_SMALL
         or embedding_model_name == EmbeddingModelMaster.OPENAI_TEXT_EMBEDDING_3_LARGE
     ) and ("api_key" in config):
         return OpenAIEmbeddings(
             openai_api_key=config["api_key"], model=embedding_model_name
@@ -118,24 +117,24 @@
         return ChatOpenAI(openai_api_key=config["api_key"], model=inference_model_name)
     elif (
         inference_model_name == InferenceModelMaster.OPENAI_GPT_3_5_TURBO
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_3_5_TURBO_INSTRUCT
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_4
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_4_TURBO_PREVIEW
     ) and ("azure_api_key" in config):
-        return AzureOpenAI(
+        return AzureChatOpenAI(
             api_key=config["azure_api_key"],
             model=inference_model_name,
-            deployment_name=config["deployment_name"],
+            deployment_name=config["azure_deployment"],
             azure_endpoint=config["azure_endpoint"],
             api_version=config["openai_api_version"],
         )
     elif (
         inference_model_name == InferenceModelMaster.GROQ_LLM_MIXTRAL_8_7_B
-        or inference_model_name == InferenceModelMaster.GROQ_LLM_LLAMA2_70B
+        or inference_model_name == InferenceModelMaster.GROQ_LLM_LLAMA3_70B
         or inference_model_name == InferenceModelMaster.GROQ_LLM_GEMMA7B
     ) and ("groq_api_key" in config):
         return ChatGroq(groq_api_key=config["groq_api_key"], model=inference_model_name)
 
     elif (
         inference_model_name == InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1
         or inference_model_name == InferenceModelMaster.BEDROCK_TEXT_LITE_G1
@@ -156,30 +155,32 @@
     else:
         raise ValueError(f"Unknown inference model: {inference_model_name}")
 
 
 def create_embeddings(data_sources, embedding_model, collection_name):
 
     store = get_vectorstore(embedding_model, collection_name)
-    doc_id = uuid.uuid4()
+    config_id = []
     for data_source in data_sources:
+        config_id.append(uuid.uuid4())
         # data_source = {'name': 'PDF', 'config': {'files': ['path/to/file', 'path/to/file']}}
         for file_path in data_source.config["files"]:
             loader = get_loader(data_source.name, file_path, data_source.config)
             extra_metadata = [
-                ("configId", str(doc_id)),
+                ("configId", str(config_id)),
             ]
             pages = loader.load_and_split()
             for page_content in pages:
                 for key, value in extra_metadata:
                     page_content.metadata[key] = value
             # document.text = mask_data(document.text)
             # text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
             store.add_documents(pages)
-            return {"message" : "embedding created" , "config_id" : str(doc_id)}
+    # config_id is a list, due to possibility of multiple data_source.
+    return {"message" : "embedding created" , "config_id" : config_id}
 
 
 def get_vectorstore(embedding_model, collection_name):
     embeddings = get_embedding_model(embedding_model.name, embedding_model.config)
     store = PGVector(
         collection_name=collection_name,
         connection_string=SQLALCHEMY_DATABASE_URL,
```

### Comparing `therix-0.1.4/therix/utils/summarizer.py` & `therix-0.1.5/therix/utils/summarizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from langchain.text_splitter import CharacterTextSplitter
 from langchain.docstore.document import Document
 from langchain.chains import (
     MapReduceDocumentsChain,
     ReduceDocumentsChain,
 )
 from langchain_core.output_parsers import JsonOutputParser
+from langfuse.callback import CallbackHandler
+
        
 class SummarizerTypeMaster(Enum): 
     EXTRACTIVE = 'EXTRACTIVE'
     ABSTRACTIVE = 'ABSTRACTIVE'
         
 PROMPT_TEMPLATE = {
     "EXTRACTIVE" : """
@@ -29,15 +31,26 @@
 
         Please structure your response in the following JSON format:
         {response_schema_json}
         """,
     "ABSTRACTIVE": "Provide a concise summary for the following text using abstractive summarization:\n\n{context}."
 }
         
-def summarizer(summarizer_config,inference_model_details,text):
+def summarizer(summarizer_config,inference_model_details,text, trace_details):
+    
+    chain_callbacks = []
+    if trace_details is not None:
+        langfuse_handler = CallbackHandler(
+            secret_key=trace_details["secret_key"],
+            public_key=trace_details["public_key"],
+            host=trace_details["host"],
+            trace_name=trace_details["identifier"],
+        )
+        chain_callbacks.append(langfuse_handler)
+        
     pydantic_prompt = summarizer_config['pydantic_model']
     summarization_type = summarizer_config['summarization_type']
     inference_model_name = inference_model_details.name
     inference_model_config = inference_model_details.config
     llm = get_inference_model(inference_model_name, inference_model_config)
 
     map_template = PromptTemplate.from_template(
@@ -100,11 +113,11 @@
         template=PROMPT_TEMPLATE[summarization_type],
         input_variables=["context"],
         partial_variables={"response_schema_json": pydantic_prompt},
     )
     
     if summarization_type == SummarizerTypeMaster.EXTRACTIVE.value:
         chain = prompt | llm | parser
-        return json.dumps(chain.invoke({"context": summary}))
+        return json.dumps(chain.invoke({"context": summary},config={"callbacks": [langfuse_handler]}))
     else:
         chain = prompt | llm
-        return  chain.invoke({"context": summary}).content
+        return  chain.invoke({"context": summary}, config={"callbacks": [langfuse_handler]}).content
```

### Comparing `therix-0.1.4/PKG-INFO` & `therix-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: therix
-Version: 0.1.4
+Version: 0.1.5
 Summary: Therix is the SDK for langchain based applications.
 License: MIT
 Author: Ajinath
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (==1.13.1)
 Requires-Dist: alembic-postgresql-enum (==1.1.2)
 Requires-Dist: boto3 (>=1.34.81,<2.0.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: coverage (>=7.4.4,<8.0.0)
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
@@ -26,14 +28,15 @@
 Requires-Dist: pylint (>=3.1.0,<4.0.0)
 Requires-Dist: pypdf (==4.1.0)
 Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: selenium (>=4.19.0,<5.0.0)
 Requires-Dist: sqlalchemy (==2.0.28)
 Requires-Dist: tiktoken (==0.6.0)
+Requires-Dist: transformers (>=4.40.2,<5.0.0)
 Requires-Dist: wheel (>=0.43.0,<0.44.0)
 Requires-Dist: youtube-transcript-api (>=0.6.2,<0.7.0)
 Description-Content-Type: text/markdown
 
 # Therix
 
 `therix` is a Python library designed to enhance and simplify your development experience. With a focus on ease of use and extensibility, `therix` provides a solid foundation for building more complex functionalities.
```

