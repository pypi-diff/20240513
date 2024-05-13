# Comparing `tmp/datarobot_early_access-3.5.0.2024.5.13.tar.gz` & `tmp/datarobot_early_access-3.5.0.2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.5.0.2024.5.13.tar", last modified: Mon May 13 16:47:56 2024, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.5.0.2024.5.6.tar", last modified: Mon May  6 16:47:31 2024, max compression
```

## Comparing `datarobot_early_access-3.5.0.2024.5.13.tar` & `datarobot_early_access-3.5.0.2024.5.6.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   232061 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4235 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5852 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2527 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:46:34.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26398 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/chunking_service.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/data_matching.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5808 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/enums.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:46:34.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      379 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/chat.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14799 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/chat_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      390 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/comparison_chat.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4404 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/comparison_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5620 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/cost_metric_configurations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      402 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/custom_model_llm_validation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9890 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/evaluation_dataset_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7350 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12541 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/insights_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      378 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/llm.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      388 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/llm_blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      385 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/playground.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7445 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/prompt_trace.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12780 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/sidecar_model_metric.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3237 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      386 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/user_limits.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9278 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/vector_database.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5416 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/incremental_learning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6392 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20913 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    31504 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54156 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/recipe_operations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8966 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/recipes.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7408 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/analytics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14682 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12682 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/config.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40267 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27055 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8744 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      200 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9380 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/base.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3057 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1770 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1986 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/shap_preview.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:46:34.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4339 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9076 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15457 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20521 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/batch_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    86467 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11451 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4889 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7244 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20307 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    33710 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12041 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    63366 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22991 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17068 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/data_slice.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17063 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20149 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    75540 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      544 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16779 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5698 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/bias_and_fairness.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7095 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/challenger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6170 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/champion_model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57732 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/custom_metrics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24249 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/data_exports.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   121466 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/mixins.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/sharing.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:46:34.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27024 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8427 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5376 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7052 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18312 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/featurelist.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      455 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5647 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/chat.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18148 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/chat_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5925 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/comparison_chat.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12080 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/comparison_prompt.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2168 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/custom_model_llm_validation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16900 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/custom_model_validation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10350 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/llm.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23244 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/llm_blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7303 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/playground.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/user_limits.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26873 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/vector_database.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21315 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13141 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/key_values.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6516 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   303355 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model_registry/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      204 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model_registry/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      408 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model_registry/common.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3453 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model_registry/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26475 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model_registry/registered_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22985 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model_registry/registered_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10918 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prediction_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39753 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   224363 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57175 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/recommended_model.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/registry/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      345 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/registry/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16789 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/registry/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10379 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/registry/job_run.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19108 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6645 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11692 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5008 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/runtime_parameters.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4722 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8216 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2676 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7314 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6267 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/status_check_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2029 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24813 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/use_cases/use_case.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13496 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/use_cases/utils.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:46:34.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2024-05-13 16:46:32.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4235 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8344 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1235 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2024-05-13 16:47:55.000000 datarobot_early_access-3.5.0.2024.5.13/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2024-05-13 16:46:34.000000 datarobot_early_access-3.5.0.2024.5.13/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2024-05-13 16:47:56.000000 datarobot_early_access-3.5.0.2024.5.13/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2024-05-13 16:46:34.000000 datarobot_early_access-3.5.0.2024.5.13/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2498 2024-05-13 16:46:34.000000 datarobot_early_access-3.5.0.2024.5.13/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   231328 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5852 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2527 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26398 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/chunking_service.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/data_matching.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5808 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/enums.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      379 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14680 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/chat_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      390 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/comparison_chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4400 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/comparison_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5620 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/cost_metric_configurations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      402 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/custom_model_llm_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9890 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7350 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12541 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/insights_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      378 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/llm.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      388 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/llm_blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      385 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/playground.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7305 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/prompt_trace.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12780 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/sidecar_model_metric.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3237 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      386 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/user_limits.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9278 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/vector_database.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5416 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/incremental_learning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6392 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20913 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    31504 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54156 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipe_operations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8966 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipes.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7408 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/analytics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14682 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12682 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/config.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40318 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27055 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8744 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      200 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9380 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/base.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3057 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1770 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1986 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_preview.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4339 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9076 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15457 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20521 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    86467 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11451 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4889 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7244 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20307 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34090 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    63934 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22991 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17068 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_slice.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17063 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20149 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    75540 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      544 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16779 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5698 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7095 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/challenger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6170 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/champion_model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57732 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/custom_metrics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24249 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_exports.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   121466 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/mixins.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/sharing.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27024 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8427 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5376 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7052 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18312 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/featurelist.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      455 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5647 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18029 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5925 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_chat.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12076 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_prompt.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2168 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_llm_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16900 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_validation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10350 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22899 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm_blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7299 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/playground.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/user_limits.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26873 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/vector_database.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21315 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13141 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/key_values.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6516 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   303355 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      204 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      408 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/common.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3453 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26475 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22985 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10918 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39753 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   224363 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    57175 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/recommended_model.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      345 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16789 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10379 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job_run.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6645 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11692 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5008 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/runtime_parameters.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4722 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8216 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2676 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7314 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6267 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/status_check_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2029 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24890 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13496 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2024-05-06 16:46:21.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4234 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8344 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1235 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2024-05-06 16:47:31.000000 datarobot_early_access-3.5.0.2024.5.6/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2498 2024-05-06 16:46:22.000000 datarobot_early_access-3.5.0.2024.5.6/setup_weekly.py
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/CHANGES.rst` & `datarobot_early_access-3.5.0.2024.5.6/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 #########
 Changelog
 #########
 3.5.0b0
 =======
 
-New features
-************
-- Added attribute `creation_user_name` to :class:`LLMBlueprint <datarobot.models.genai.llm_blueprint.LLMBlueprint>`.
-
 Documentation changes
 *********************
-- Added usage of `external_llm_context_size` in `llm_settings` in `genai_example.rst`.
-- Updated doc string for `llm_settings` to include attribute `external_llm_context_size` for external LLMs.
 - Updated `genai_example.rst` to link to DataRobot doc pages for external vector database and external LLM deployment creation.
 
-API changes
-***********
-- Remove an unsupported `NETWORK_EGRESS_POLICY.DR_API_ACCESS` value for custom models. This value
-  was used by a feature that was never released as a GA and is not supported in the current API.
-
 3.4.0b0
 =======
 
 New features
 ************
 - Added a new class :class: `EvaluationDatasetConfiguration <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration>` for configuration of evaluation datasets.
   :meth:`EvaluationDatasetConfiguration.get <datarobot._experimental.models.genai.evaluation_dataset_configuration.EvaluationDatasetConfiguration.get>` to get an evaluation dataset configuration.
@@ -53,30 +42,27 @@
 
 
 Enhancements
 ************
 
 Bugfixes
 ********
-- Updated the validation logic of `RelationshipsConfiguration` to work with native database connections
 
 API changes
 ***********
 - Remove `ImportedModel` object since it was API for SSE (standalone scoring engine) which is not part of DataRobot anymore.
 
 Deprecation summary
 *******************
 
 Configuration changes
 *********************
 
 Documentation changes
 *********************
-- Removed incorrect can_share parameters in Use Case sharing example
-
 
 Experimental changes
 ********************
 
 3.4.0
 =====
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/LICENSE.txt` & `datarobot_early_access-3.5.0.2024.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/PKG-INFO` & `datarobot_early_access-3.5.0.2024.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.5.0.2024.5.13
+Version: 3.5.0.2024.5.6
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/README.md` & `datarobot_early_access-3.5.0.2024.5.6/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/common_setup.py` & `datarobot_early_access-3.5.0.2024.5.6/common_setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_compat.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/chunking_service.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/chunking_service.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/enums.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/enums.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/chat_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/chat_prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -293,25 +293,24 @@
     llm_blueprint_id : str
         ID of the LLM blueprint associated with the chat prompt.
     llm_id : str
         ID of the LLM type. This must be one of the IDs returned by `LLMDefinition.list`
         for this user.
     llm_settings : dict or None
         The LLM settings for the LLM blueprint. The specific keys allowed and the
-        constraints on the values are defined in the response from `LLMDefinition.list`,
-        but this typically has dict fields. Either:
-        - system_prompt - The system prompt that influences the LLM responses.
-        - max_completion_length - The maximum number of tokens in the completion.
-        - temperature - Controls the variability in the LLM response.
-        - top_p - Sets whether the model considers next tokens with top_p probability mass.
+        constraints on the values are defined in the response from `LLMDefinition.list`
+        but this typically has dict fields:
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - max_completion_length - The maximum number of token in the completion.
+        - temperature - controls the variability in the LLM response.
+        - top_p - the model considers next tokens with top_p probability mass
         or
-        - system_prompt - The system prompt that influences the LLM responses.
-        - validation_id - The ID of the external model LLM validation.
-        - external_llm_context_size - The external LLM's context size, in tokens,
-        for external model-based LLM blueprints.
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - validation_id - The ID of the custom model LLM validation
+        for custom model LLM blueprints.
     creation_date : str
         The date the chat prompt was created.
     creation_user_id : str
         ID of the creating user.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
     vector_database_settings : VectorDatabaseSettings or None
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/comparison_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/comparison_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     id : str
         Comparison prompt ID.
     text : str
         The prompt text.
     results : list[ComparisonPromptResult]
         The list of results for individual LLM blueprints that are part of the comparison prompt.
     creation_date : str
-        The date when the playground was created.
+        Date when the playground was created.
     creation_user_id : str
         ID of the creating user.
     comparison_chat_id : str
         The ID of the comparison chat this comparison prompt is associated with.
     """
 
     def update(
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/cost_metric_configurations.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/cost_metric_configurations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/evaluation_dataset_configuration.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/evaluation_dataset_metric_aggregation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/insights_configuration.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/insights_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/prompt_trace.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/prompt_trace.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,27 +77,25 @@
         The ID of the LLM blueprint that the prompt was submitted to.
     llm_name : str
         The name of the LLM in the LLM blueprint.
     llm_vendor : str
         The vendor name of the LLM.
     llm_license : str
         What type of license the LLM has.
-    llm_settings : dict or None
+    llm_settings : dict
         The LLM settings for the LLM blueprint. The specific keys allowed and the
-        constraints on the values are defined in the response from `LLMDefinition.list`,
-        but this typically has dict fields. Either:
-        - system_prompt - The system prompt that influences the LLM responses.
-        - max_completion_length - The maximum number of tokens in the completion.
+        constraints on the values are defined in the response from LLMDefinition.list
+        but this typically has dict fields:
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - max_completion_length - The maximum number of token in the completion.
         - temperature - Controls the variability in the LLM response.
-        - top_p - Sets whether the model considers next tokens with top_p probability mass.
-        or
-        - system_prompt - The system prompt that influences the LLM responses.
-        - validation_id - The ID of the external model LLM validation.
-        - external_llm_context_size - The external LLM's context size, in tokens,
-        for external model-based LLM blueprints.
+        - top_p - The model considers next tokens with top_p probability mass
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - validation_id - The ID of the custom model LLM validation
+        for custom model LLM blueprints.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
     vector_database_settings : VectorDatabaseSettings or None
         The settings for the vector database associated with the LLM blueprint, if any.
     result_metadata : ResultMetadata or None
         Metadata for the result of the prompt submission.
     result_text: str or None
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/sidecar_model_metric.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/sidecar_model_metric.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/synthetic_evaluation_dataset_generation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/genai/vector_database.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/genai/vector_database.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/incremental_learning.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/incremental_learning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/notebooks.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/notebooks.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/recipe_operations.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipe_operations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/recipes.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/recipes.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/analytics.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/analytics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/client.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/config.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/config.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/context.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/enums.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,17 +570,18 @@
     ALL = _SHARED_TARGET_TYPE.ALL + [TRANSFORM]
 
 
 class NETWORK_EGRESS_POLICY:
     """Enum of valid network egress policy"""
 
     NONE = "NONE"
+    DR_API_ACCESS = "DR_API_ACCESS"
     PUBLIC = "PUBLIC"
 
-    ALL = [NONE, PUBLIC]
+    ALL = [NONE, DR_API_ACCESS, PUBLIC]
 
 
 @use_all
 class SOURCE_TYPE(StrEnum):
     """Enum of backtest source types"""
 
     TRAINING = "training"
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/errors.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/base.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/base.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/shap_impact.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/shap_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/insights/shap_preview.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/insights/shap_preview.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/api_object.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/application.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/batch_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/blueprint.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/calendar_file.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/change_request.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/cluster.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/connector.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/credential.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -430,15 +430,18 @@
         The username of a user who created the custom model.
     updated_at: str
         ISO-8601 formatted timestamp of when the custom model was updated
     created_at: str
         ISO-8601 formatted timestamp of when the custom model was created
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+        `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+        is only supported by the SaaS (cloud) environment.
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
         If exceeded, the custom-model will be killed by k8s.
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster
     is_training_data_for_versions_permanently_enabled: bool, optional
         Whether training data assignment on the version level is permanently enabled for the model.
@@ -645,15 +648,18 @@
             Custom inference model class labels for multiclass classification.
             Cannot be used with class_labels_file.
         class_labels_file: str, optional
             Path to file containing newline separated class labels for multiclass classification.
             Cannot be used with class_labels.
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`]
+            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`]
+            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+            is only supported by the SaaS (cloud) environment.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s.
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster.
         is_training_data_for_versions_permanently_enabled: bool, optional
             Permanently enable training data assignment on the version level for the current model,
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,17 @@
         id of a dataset version used for testing
     completed_at: str, optional
         ISO-8601 formatted timestamp of when the test has completed
     created_at: str, optional
         ISO-8601 formatted timestamp of when the version was created
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+        `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value is only supported by the SaaS (cloud) environment.
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
         If exceeded, the custom-model will be killed by k8s
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster
     """
 
@@ -163,15 +165,18 @@
             The id of the testing dataset for non-unstructured custom models.
             Ignored and not required for unstructured models.
         max_wait: int, optional
             max time to wait for a test completion.
             If set to None - method will return without waiting.
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+            is only supported by the SaaS (cloud) environment.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster
 
         Returns
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_model_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -524,15 +524,17 @@
     created_at: str, optional
         ISO-8601 formatted timestamp of when the version was created.
     dependencies: List[CustomDependency]
         The parsed dependencies of the custom model version if the
         version has a valid requirements.txt file.
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+        `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+        Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value is only supported by the SaaS (cloud) environment.
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
         If exceeded, the custom-model will be killed by k8s.
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster.
     required_metadata_values: List[RequiredMetadataValue]
         Additional parameters required by the execution environment. The required keys are
@@ -705,15 +707,18 @@
             [("/home/user/Documents/myModel/file1.txt", "file1.txt"),
             ("/home/user/Documents/myModel/folder/file2.txt", "folder/file2.txt")]
             or
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+            is only supported by the SaaS (cloud) environment.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s.
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster.
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
@@ -889,15 +894,18 @@
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         files_to_delete: list, optional
             The list of a file items ids to be deleted.
             Example: ["5ea95f7a4024030aba48e4f9", "5ea6b5da402403181895cc51"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Values: [`datarobot.NETWORK_EGRESS_POLICY.NONE`, `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS`,
+            `datarobot.NETWORK_EGRESS_POLICY.PUBLIC`].
+            Note: `datarobot.NETWORK_EGRESS_POLICY.DR_API_ACCESS` value
+            is only supported by the SaaS (cloud) environment.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_task.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/data_slice.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_slice.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/data_source.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/data_store.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/challenger.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/challenger.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/champion_model_package.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/champion_model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/custom_metrics.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/data_exports.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/data_exports.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/documentai/document.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/driver.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/execution_environment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_effect.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/feature_impact.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/feature_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/featurelist.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/chat.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/chat_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/chat_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,25 +231,24 @@
     llm_blueprint_id : str
         ID of the LLM blueprint associated with the chat prompt.
     llm_id : str
         ID of the LLM type. This must be one of the IDs returned by `LLMDefinition.list`
         for this user.
     llm_settings : dict or None
         The LLM settings for the LLM blueprint. The specific keys allowed and the
-        constraints on the values are defined in the response from `LLMDefinition.list`,
-        but this typically has dict fields. Either:
-        - system_prompt - The system prompt that influences the LLM responses.
-        - max_completion_length - The maximum number of tokens in the completion.
-        - temperature - Controls the variability in the LLM response.
-        - top_p - Sets whether the model considers next tokens with top_p probability mass.
+        constraints on the values are defined in the response from `LLMDefinition.list`
+        but this typically has dict fields:
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - max_completion_length - The maximum number of token in the completion.
+        - temperature - controls the variability in the LLM response.
+        - top_p - the model considers next tokens with top_p probability mass
         or
-        - system_prompt - The system prompt that influences the LLM responses.
-        - validation_id - The ID of the external model LLM validation.
-        - external_llm_context_size - The external LLM's context size, in tokens,
-        for external model-based LLM blueprints.
+        - system_prompt - The system prompt that tells the LLM how to behave.
+        - validation_id - The ID of the custom model LLM validation
+        for custom model LLM blueprints.
     creation_date : str
         The date the chat prompt was created.
     creation_user_id : str
         ID of the creating user.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
     vector_database_settings : VectorDatabaseSettings or None
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/comparison_chat.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_chat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/comparison_prompt.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/comparison_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     id : str
         Comparison prompt ID.
     text : str
         The prompt text.
     results : list[ComparisonPromptResult]
         The list of results for individual LLM blueprints that are part of the comparison prompt.
     creation_date : str
-        The date when the playground was created.
+        Date when the playground was created.
     creation_user_id : str
         ID of the creating user.
     comparison_chat_id : str
         The ID of the comparison chat this comparison prompt is associated with.
     """
 
     _path = "api/v2/genai/comparisonPrompts"
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/custom_model_llm_validation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_llm_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/custom_model_validation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/custom_model_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/llm.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/llm_blueprint.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/llm_blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         t.Key("is_starred"): t.Bool,
         t.Key("playground_id"): t.String,
         t.Key("llm_id", optional=True): t.Or(t.String, t.Null),
         t.Key("llm_settings", optional=True): t.Or(t.Dict().allow_extra("*"), t.Null),
         t.Key("llm_name", optional=True): t.Or(t.String, t.Null),
         t.Key("creation_date"): t.String,
         t.Key("creation_user_id"): t.String,
-        t.Key("creation_user_name"): t.String(allow_blank=True),
         t.Key("last_update_date"): t.String,
         t.Key("last_update_user_id"): t.String,
         t.Key("prompt_type"): t.Enum(*enum_to_list(PromptType)),
         t.Key("vector_database_id", optional=True): t.Or(t.String, t.Null),
         t.Key("vector_database_settings", optional=True): t.Or(
             vector_database_settings_trafaret, t.Null
         ),
@@ -164,25 +163,22 @@
         but this typically has dict fields:
         - system_prompt - The system prompt that tells the LLM how to behave.
         - max_completion_length - The maximum number of token in the completion.
         - temperature - controls the variability in the LLM response.
         - top_p - the model considers next tokens with top_p probability mass
         or
         - system_prompt - The system prompt that tells the LLM how to behave.
-        - validation_id - The ID of the external model LLM validation
-        - external_llm_context_size - The external LLM's context size in tokens
-        for external model LLM blueprints.
+        - validation_id - The ID of the custom model LLM validation
+        for custom model LLM blueprints.
     creation_date : str
-        The date when the playground was created.
+        Date when the playground was created.
     creation_user_id : str
-        The ID of the user creating the playground.
-    creation_user_name : str
-        The name of the user creating the playground.
+        ID of the creating user.
     last_update_date : str
-        The date when the playground was most recently updated.
+        Date when the playground was most recently updated.
     last_update_user_id : str
         ID of the user who most recently updated the playground.
     prompt_type : PromptType
         The prompting strategy for the LLM Blueprint.
         Currently supported options are listed in PromptType.
     vector_database_id : str or None
         ID of the vector database associated with the LLM blueprint, if any.
@@ -214,15 +210,14 @@
         name: str,
         description: str,
         is_saved: bool,
         is_starred: bool,
         playground_id: str,
         creation_date: str,
         creation_user_id: str,
-        creation_user_name: str,
         last_update_date: str,
         last_update_user_id: str,
         prompt_type: PromptType,
         llm_id: Optional[str] = None,
         llm_name: Optional[str] = None,
         llm_settings: Optional[LLMSettingsCommonDict | LLMSettingsCustomModelDict] = None,
         vector_database_id: Optional[str] = None,
@@ -242,15 +237,14 @@
         self.is_starred = is_starred
         self.playground_id = playground_id
         self.llm_id = llm_id
         self.llm_name = llm_name
         self.llm_settings = llm_settings
         self.creation_date = creation_date
         self.creation_user_id = creation_user_id
-        self.creation_user_name = creation_user_name
         self.last_update_date = last_update_date
         self.last_update_user_id = last_update_user_id
         self.prompt_type = prompt_type
         self.vector_database_id = vector_database_id
         self.vector_database_settings = (
             VectorDatabaseSettings.from_server_data(vector_database_settings)
             if vector_database_settings
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/playground.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/playground.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     name : str
         Playground name.
     description : str
         Description of the playground.
     use_case_id : str
         Linked use case ID.
     creation_date : str
-        The date when the playground was created.
+        Date when the playground was created.
     creation_user_id : str
         ID of the creating user.
     last_update_date : str
         Date when the playground was most recently updated.
     last_update_user_id : str
         ID of the user who most recently updated the playground.
     saved_llm_blueprints_count : int
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/user_limits.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/user_limits.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/genai/vector_database.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/genai/vector_database.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/key_values.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/key_values.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/lift_chart.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/missing_report.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model_registry/deployment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model_registry/registered_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/model_registry/registered_model_version.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/model_registry/registered_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/modeljob.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/pareto_front.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/predict_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prediction_environment.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prediction_server.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/predictions.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/prime_file.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/project.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/project_options.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/rating_table.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/recommended_model.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/registry/job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/registry/job_run.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/registry/job_run.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/relationships_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,16 +175,16 @@
     """
 
     _path = "relationshipsConfigurations/"
     data_source_trafaret = t.Dict(
         {
             t.Key("data_store_name"): String,
             t.Key("data_store_id"): String,
-            t.Key("url", optional=True): t.Or(String, t.Null),
-            t.Key("dbtable", optional=True): t.Or(String, t.Null),
+            t.Key("url"): String,
+            t.Key("dbtable"): t.Or(String, t.Null),
             t.Key("schema", optional=True): t.Or(String(allow_blank=True), t.Null),
             t.Key("catalog", optional=True): t.Or(String(allow_blank=True), t.Null),
             t.Key("data_source_id", optional=True): t.Or(String, t.Null),
         }
     ).ignore_extra("*")
     feature_list_info = t.Dict(
         {
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/residuals.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/roc_curve.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/ruleset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/runtime_parameters.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/segmentation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/shap_impact.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/sharing.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/status_check_job.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/status_check_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/trafarets.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/training_predictions.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/types.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/use_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,14 +575,15 @@
             >>> user_ids = ["60912e09fd1f04e832a575c1", "639ce542862e9b1b1bfa8f1b", "63e185e7cd3a5f8e190c6393"]
             >>> sharing_roles = []
             >>> for user_id in user_ids:
             ...     new_sharing_role = SharingRole(
             ...         role=SHARING_ROLE.CONSUMER,
             ...         share_recipient_type=SHARING_RECIPIENT_TYPE.USER,
             ...         id=user_id,
+            ...         can_share=True,
             ...     )
             ...     sharing_roles.append(new_sharing_role)
             >>> use_case = UseCase.get(use_case_id="5f33f1fd9071ae13568237b2")
             >>> use_case.share(roles=sharing_roles)
 
         Similarly, a :class:`SharingRole <datarobot.models.sharing.SharingRole>` instance can be used to
         remove a user's access if the ``role`` is set to ``SHARING_ROLE.NO_ROLE``, like in this example:
@@ -594,14 +595,15 @@
             >>> from datarobot.enums import SHARING_ROLE, SHARING_RECIPIENT_TYPE
             >>>
             >>> user_to_remove = "foo.bar@datarobot.com"
             ... remove_sharing_role = SharingRole(
             ...     role=SHARING_ROLE.NO_ROLE,
             ...     share_recipient_type=SHARING_RECIPIENT_TYPE.USER,
             ...     username=user_to_remove,
+            ...     can_share=False,
             ... )
             >>> use_case = UseCase.get(use_case_id="5f33f1fd9071ae13568237b2")
             >>> use_case.share(roles=[remove_sharing_role])
         """
         if any(
             role.role
             not in [
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/use_cases/utils.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/use_cases/utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/validators.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/visualai/images.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/models/word_cloud.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/rest.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/__init__.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/deprecation.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/pagination.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/retry.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/source.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot/utils/waiters.py` & `datarobot_early_access-3.5.0.2024.5.6/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.5.0.2024.5.13
+Version: 3.5.0.2024.5.6
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.5.0.2024.5.6/datarobot_early_access.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/pyproject.toml` & `datarobot_early_access-3.5.0.2024.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/setup.py` & `datarobot_early_access-3.5.0.2024.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.5.0.2024.5.13/setup_weekly.py` & `datarobot_early_access-3.5.0.2024.5.6/setup_weekly.py`

 * *Files identical despite different names*

