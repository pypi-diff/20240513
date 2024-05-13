# Comparing `tmp/logfire-0.30.0.tar.gz` & `tmp/logfire-0.31.0.tar.gz`

## Comparing `logfire-0.30.0.tar` & `logfire-0.31.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.30.0/Makefile
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18526 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    55143 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/config.py
--rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/constants.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    12892 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    54139 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/main.py
--rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/openai.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    18716 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 logfire-0.30.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/__init__.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    18741 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_backfill.py
--rw-r--r--   0        0        0    44869 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    51315 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_configure.py
--rw-r--r--   0        0        0    24810 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_formatter.py
--rw-r--r--   0        0        0    45555 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0    67482 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_logfire.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_loguru.py
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_no_production.py
--rw-r--r--   0        0        0    53680 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_structlog.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    40300 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    43085 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7332 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.30.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.30.0/LICENSE
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 logfire-0.30.0/README.md
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 logfire-0.30.0/pyproject.toml
--rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 logfire-0.30.0/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.31.0/Makefile
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18526 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    55953 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    55300 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0     9959 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/openai.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    18537 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 logfire-0.31.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    45014 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_configure.py
+-rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_loguru.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    40637 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    43190 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.31.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.31.0/LICENSE
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.31.0/README.md
+-rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 logfire-0.31.0/pyproject.toml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.31.0/PKG-INFO
```

### Comparing `logfire-0.30.0/Makefile` & `logfire-0.31.0/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/__init__.py` & `logfire-0.31.0/logfire/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 fatal = DEFAULT_LOGFIRE_INSTANCE.fatal
 exception = DEFAULT_LOGFIRE_INSTANCE.exception
 
 # Metrics
 metric_counter = DEFAULT_LOGFIRE_INSTANCE.metric_counter
 metric_histogram = DEFAULT_LOGFIRE_INSTANCE.metric_histogram
 metric_up_down_counter = DEFAULT_LOGFIRE_INSTANCE.metric_up_down_counter
+metric_gauge = DEFAULT_LOGFIRE_INSTANCE.metric_gauge
 metric_counter_callback = DEFAULT_LOGFIRE_INSTANCE.metric_counter_callback
 metric_gauge_callback = DEFAULT_LOGFIRE_INSTANCE.metric_gauge_callback
 metric_up_down_counter_callback = DEFAULT_LOGFIRE_INSTANCE.metric_up_down_counter_callback
 
 
 def loguru_handler() -> dict[str, Any]:
     """Create a **Logfire** handler for Loguru.
```

### Comparing `logfire-0.30.0/logfire/propagate.py` & `logfire-0.31.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/testing.py` & `logfire-0.31.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/ast_utils.py` & `logfire-0.31.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/async_.py` & `logfire-0.31.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/auth.py` & `logfire-0.31.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/backfill.py` & `logfire-0.31.0/logfire/_internal/backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                     is_remote=False,
                 )
             else:
                 parent_context = None  # pragma: no cover
             otlp_attributes = user_attributes(data.attributes)
 
             if data.formatted_msg is None:  # pragma: no cover
-                formatted_message = logfire_format(data.msg_template, data.attributes, self.scrubber, stack_offset=2)
+                formatted_message = logfire_format(data.msg_template, data.attributes, self.scrubber)
             else:
                 formatted_message = data.formatted_msg
             otlp_attributes: dict[str, Any] = {
                 ATTRIBUTES_SPAN_TYPE_KEY: 'log',
                 ATTRIBUTES_LOG_LEVEL_NUM_KEY: LEVEL_NUMBERS[data.level],
                 ATTRIBUTES_MESSAGE_TEMPLATE_KEY: data.msg_template,
                 ATTRIBUTES_MESSAGE_KEY: formatted_message,
@@ -194,17 +194,15 @@
             if end_timestamp.tzinfo is None:  # pragma: no branch
                 end_timestamp = end_timestamp.replace(tzinfo=timezone.utc)
             start_timestamp = data.start_timestamp
             if start_timestamp.tzinfo is None:  # pragma: no branch
                 start_timestamp = start_timestamp.replace(tzinfo=timezone.utc)
             otlp_attributes = user_attributes(data.log_attributes)
             if data.formatted_msg is None:  # pragma: no branch
-                formatted_message = logfire_format(
-                    data.msg_template, data.log_attributes, self.scrubber, stack_offset=2
-                )
+                formatted_message = logfire_format(data.msg_template, data.log_attributes, self.scrubber)
             else:  # pragma: no cover
                 formatted_message = data.formatted_msg
             otlp_attributes: dict[str, Any] = {
                 ATTRIBUTES_SPAN_TYPE_KEY: 'log',
                 ATTRIBUTES_MESSAGE_TEMPLATE_KEY: data.msg_template,
                 ATTRIBUTES_MESSAGE_KEY: formatted_message,
                 **otlp_attributes,
```

### Comparing `logfire-0.30.0/logfire/_internal/cli.py` & `logfire-0.31.0/logfire/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/config.py` & `logfire-0.31.0/logfire/_internal/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,15 @@
     default_span_processor: Callable[[SpanExporter], SpanProcessor] | None = None,
     metric_readers: Sequence[MetricReader] | None = None,
     logfire_api_session: requests.Session | None = None,
     pydantic_plugin: PydanticPlugin | None = None,
     fast_shutdown: bool = False,
     scrubbing_patterns: Sequence[str] | None = None,
     scrubbing_callback: ScrubCallback | None = None,
+    inspect_arguments: bool | None = None,
 ) -> None:
     """Configure the logfire SDK.
 
     Args:
         send_to_logfire: Whether to send logs to logfire.dev. Defaults to the `LOGFIRE_SEND_TO_LOGFIRE` environment
             variable if set, otherwise defaults to `True`. If `if-token-present` is provided, logs will only be sent if
             a token is present.
@@ -206,14 +207,17 @@
         scrubbing_patterns: A sequence of regular expressions to detect sensitive data that should be redacted.
             For example, the default includes `'password'`, `'secret'`, and `'api[._ -]?key'`.
             The specified patterns are combined with the default patterns.
         scrubbing_callback: A function that is called for each match found by the scrubber.
             If it returns `None`, the value is redacted.
             Otherwise, the returned value replaces the matched value.
             The function accepts a single argument of type [`logfire.ScrubMatch`][logfire.ScrubMatch].
+        inspect_arguments: Whether to enable f-string magic.
+            If `None` uses the `LOGFIRE_INSPECT_ARGUMENTS` environment variable.
+            Defaults to `True` if and only if the Python version is at least 3.11.
     """
     GLOBAL_CONFIG.configure(
         base_url=base_url,
         send_to_logfire=send_to_logfire,
         token=token,
         project_name=project_name,
         service_name=service_name,
@@ -230,14 +234,15 @@
         default_span_processor=default_span_processor,
         metric_readers=metric_readers,
         logfire_api_session=logfire_api_session,
         pydantic_plugin=pydantic_plugin,
         fast_shutdown=fast_shutdown,
         scrubbing_patterns=scrubbing_patterns,
         scrubbing_callback=scrubbing_callback,
+        inspect_arguments=inspect_arguments,
     )
 
 
 def _get_int_from_env(env_var: str) -> int | None:
     value = os.getenv(env_var)
     if not value:
         return None
@@ -333,17 +338,18 @@
         id_generator: IdGenerator | None,
         ns_timestamp_generator: Callable[[], int] | None,
         processors: Sequence[SpanProcessor] | None,
         default_span_processor: Callable[[SpanExporter], SpanProcessor] | None,
         metric_readers: Sequence[MetricReader] | None,
         logfire_api_session: requests.Session | None,
         pydantic_plugin: PydanticPlugin | None,
-        fast_shutdown: bool = False,
-        scrubbing_patterns: Sequence[str] | None = None,
-        scrubbing_callback: ScrubCallback | None = None,
+        fast_shutdown: bool,
+        scrubbing_patterns: Sequence[str] | None,
+        scrubbing_callback: ScrubCallback | None,
+        inspect_arguments: bool | None,
     ) -> None:
         """Merge the given parameters with the environment variables file configurations."""
         param_manager = ParamManager.create(config_dir)
 
         self.base_url = param_manager.load_param('base_url', base_url)
         self.metrics_endpoint = os.getenv(OTEL_EXPORTER_OTLP_METRICS_ENDPOINT) or urljoin(self.base_url, '/v1/metrics')
         self.traces_endpoint = os.getenv(OTEL_EXPORTER_OTLP_TRACES_ENDPOINT) or urljoin(self.base_url, '/v1/traces')
@@ -353,14 +359,19 @@
         self.project_name = param_manager.load_param('project_name', project_name)
         self.service_name = param_manager.load_param('service_name', service_name)
         self.service_version = param_manager.load_param('service_version', service_version)
         self.trace_sample_rate = param_manager.load_param('trace_sample_rate', trace_sample_rate)
         self.show_summary = param_manager.load_param('show_summary', show_summary)
         self.data_dir = param_manager.load_param('data_dir', data_dir)
         self.collect_system_metrics = param_manager.load_param('collect_system_metrics', collect_system_metrics)
+        self.inspect_arguments = param_manager.load_param('inspect_arguments', inspect_arguments)
+        if self.inspect_arguments and sys.version_info[:2] <= (3, 8):
+            raise LogfireConfigError(
+                'Inspecting arguments is only supported in Python 3.9+ and only recommended in Python 3.11+.'
+            )
 
         # We save `scrubbing_patterns` and `scrubbing_callback` just so that they can be serialized and deserialized.
         self.scrubbing_patterns = scrubbing_patterns
         self.scrubbing_callback = scrubbing_callback
         self.scrubber = Scrubber(scrubbing_patterns, scrubbing_callback)
 
         if isinstance(console, dict):
@@ -421,14 +432,15 @@
         default_span_processor: Callable[[SpanExporter], SpanProcessor] | None = None,
         metric_readers: Sequence[MetricReader] | None = None,
         logfire_api_session: requests.Session | None = None,
         pydantic_plugin: PydanticPlugin | None = None,
         fast_shutdown: bool = False,
         scrubbing_patterns: Sequence[str] | None = None,
         scrubbing_callback: ScrubCallback | None = None,
+        inspect_arguments: bool | None = None,
     ) -> None:
         """Create a new LogfireConfig.
 
         Users should never need to call this directly, instead use `logfire.configure`.
 
         See `_LogfireConfigData` for parameter documentation.
         """
@@ -453,14 +465,15 @@
             default_span_processor=default_span_processor,
             metric_readers=metric_readers,
             logfire_api_session=logfire_api_session,
             pydantic_plugin=pydantic_plugin,
             fast_shutdown=fast_shutdown,
             scrubbing_patterns=scrubbing_patterns,
             scrubbing_callback=scrubbing_callback,
+            inspect_arguments=inspect_arguments,
         )
         # initialize with no-ops so that we don't impact OTEL's global config just because logfire is installed
         # that is, we defer setting logfire as the otel global config until `configure` is called
         self._tracer_provider = ProxyTracerProvider(trace.NoOpTracerProvider(), self)
         # note: this reference is important because the MeterProvider runs things in background threads
         # thus it "shuts down" when it's gc'ed
         self._meter_provider = ProxyMeterProvider(metrics.NoOpMeterProvider())
@@ -486,17 +499,18 @@
         id_generator: IdGenerator | None,
         ns_timestamp_generator: Callable[[], int] | None,
         processors: Sequence[SpanProcessor] | None,
         default_span_processor: Callable[[SpanExporter], SpanProcessor] | None,
         metric_readers: Sequence[MetricReader] | None,
         logfire_api_session: requests.Session | None,
         pydantic_plugin: PydanticPlugin | None,
-        fast_shutdown: bool = False,
-        scrubbing_patterns: Sequence[str] | None = None,
-        scrubbing_callback: ScrubCallback | None = None,
+        fast_shutdown: bool,
+        scrubbing_patterns: Sequence[str] | None,
+        scrubbing_callback: ScrubCallback | None,
+        inspect_arguments: bool | None,
     ) -> None:
         with self._lock:
             self._initialized = False
             self._load_configuration(
                 base_url,
                 send_to_logfire,
                 token,
@@ -515,14 +529,15 @@
                 default_span_processor,
                 metric_readers,
                 logfire_api_session,
                 pydantic_plugin,
                 fast_shutdown,
                 scrubbing_patterns,
                 scrubbing_callback,
+                inspect_arguments,
             )
             self.initialize()
 
     def initialize(self) -> ProxyTracerProvider:
         """Configure internals to start exporting traces and metrics."""
         with self._lock:
             return self._initialize()
```

### Comparing `logfire-0.30.0/logfire/_internal/config_params.py` & `logfire-0.31.0/logfire/_internal/config_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations as _annotations
 
 import os
 import sys
 from dataclasses import dataclass
 from functools import cached_property, lru_cache
 from pathlib import Path
-from typing import Any, Literal, Set, TypeVar
+from typing import Any, Callable, Literal, Set, TypeVar
 
 from opentelemetry.sdk.environment_variables import OTEL_EXPORTER_OTLP_ENDPOINT, OTEL_SERVICE_NAME
 from typing_extensions import get_args, get_origin
 
 from logfire.exceptions import LogfireConfigError
 
 from . import config
@@ -43,18 +43,31 @@
     """Whether the parameter can be set in the config file."""
     default: Any = None
     """Default value if no other value is found."""
     tp: Any = str
     """Type of the parameter."""
 
 
+@dataclass
+class _DefaultCallback:
+    """A default value that is computed at runtime.
+
+    A good example is when we want to check if we are running under pytest and set a default value based on that.
+    """
+
+    callback: Callable[[], Any]
+
+
+_send_to_logfire_default = _DefaultCallback(lambda: 'PYTEST_CURRENT_TEST' not in os.environ)
+"""When running under pytest, don't send spans to Logfire by default."""
+
 # fmt: off
 BASE_URL = ConfigParam(env_vars=['LOGFIRE_BASE_URL', OTEL_EXPORTER_OTLP_ENDPOINT], allow_file_config=True, default=LOGFIRE_BASE_URL)
 """Use to set the base URL of the Logfire backend."""
-SEND_TO_LOGFIRE = ConfigParam(env_vars=['LOGFIRE_SEND_TO_LOGFIRE'], allow_file_config=True, default=True, tp=bool)
+SEND_TO_LOGFIRE = ConfigParam(env_vars=['LOGFIRE_SEND_TO_LOGFIRE'], allow_file_config=True, default=_send_to_logfire_default, tp=bool)
 """Whether to send spans to Logfire."""
 TOKEN = ConfigParam(env_vars=['LOGFIRE_TOKEN'])
 """Token for the Logfire API."""
 PROJECT_NAME = ConfigParam(env_vars=['LOGFIRE_PROJECT_NAME'], allow_file_config=True)
 """Name of the project. Project name accepts a string value containing alphanumeric characters and hyphens (-). The hyphen character must not be located at the beginning or end of the string and should appear in between alphanumeric characters."""
 SERVICE_NAME = ConfigParam(env_vars=['LOGFIRE_SERVICE_NAME', OTEL_SERVICE_NAME], allow_file_config=True, default='')
 """Name of the service emitting spans. For further details, please refer to the [Service section](https://opentelemetry.io/docs/specs/semconv/resource/#service)."""
@@ -87,14 +100,16 @@
 """Whether instrument Pydantic validation.."""
 PYDANTIC_PLUGIN_INCLUDE = ConfigParam(env_vars=['LOGFIRE_PYDANTIC_PLUGIN_INCLUDE'], allow_file_config=True, default=set(), tp=Set[str])
 """Set of items that should be included in Logfire Pydantic plugin instrumentation."""
 PYDANTIC_PLUGIN_EXCLUDE = ConfigParam(env_vars=['LOGFIRE_PYDANTIC_PLUGIN_EXCLUDE'], allow_file_config=True, default=set(), tp=Set[str])
 """Set of items that should be excluded from Logfire Pydantic plugin instrumentation."""
 TRACE_SAMPLE_RATE = ConfigParam(env_vars=['LOGFIRE_TRACE_SAMPLE_RATE', 'OTEL_TRACES_SAMPLER_ARG'], allow_file_config=True, default=1.0, tp=float)
 """Default sampling ratio for traces. Can be overridden by the `logfire.sample_rate` attribute of a span."""
+INSPECT_ARGUMENTS = ConfigParam(env_vars=['LOGFIRE_INSPECT_ARGUMENTS'], allow_file_config=True, default=sys.version_info[:2] >= (3, 11), tp=bool)
+"""Whether to enable the f-string magic feature. On by default for Python 3.11 and above."""
 # fmt: on
 
 CONFIG_PARAMS = {
     'base_url': BASE_URL,
     'send_to_logfire': SEND_TO_LOGFIRE,
     'token': TOKEN,
     'project_name': PROJECT_NAME,
@@ -109,14 +124,15 @@
     'console_span_style': CONSOLE_SPAN_STYLE,
     'console_include_timestamp': CONSOLE_INCLUDE_TIMESTAMP,
     'console_verbose': CONSOLE_VERBOSE,
     'console_min_log_level': CONSOLE_MIN_LOG_LEVEL,
     'pydantic_plugin_record': PYDANTIC_PLUGIN_RECORD,
     'pydantic_plugin_include': PYDANTIC_PLUGIN_INCLUDE,
     'pydantic_plugin_exclude': PYDANTIC_PLUGIN_EXCLUDE,
+    'inspect_arguments': INSPECT_ARGUMENTS,
 }
 
 
 @dataclass
 class ParamManager:
     """Manage parameters for a Logfire instance."""
 
@@ -157,14 +173,16 @@
                 return self._cast(value, name, param.tp)
 
         if param.allow_file_config:
             value = self.config_from_file.get(name)
             if value is not None:
                 return self._cast(value, name, param.tp)
 
+        if isinstance(param.default, _DefaultCallback):
+            return self._cast(param.default.callback(), name, param.tp)
         return self._cast(param.default, name, param.tp)
 
     @cached_property
     def pydantic_plugin(self):
         return config.PydanticPlugin(
             record=self.load_param('pydantic_plugin_record'),
             include=self.load_param('pydantic_plugin_include'),
```

### Comparing `logfire-0.30.0/logfire/_internal/constants.py` & `logfire-0.31.0/logfire/_internal/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,29 +22,87 @@
     'warn': 13,
     'error': 17,
     'fatal': 21,
 }
 
 NUMBER_TO_LEVEL = {v: k for k, v in LEVEL_NUMBERS.items()}
 
+LOGGING_TO_OTEL_LEVEL_NUMBERS = {
+    0: 9,  # logging.NOTSET: default to info
+    1: 1,  # OTEL trace
+    2: 1,
+    3: 2,
+    4: 2,
+    5: 3,
+    6: 3,
+    7: 4,
+    8: 4,
+    9: 5,
+    10: 5,  # debug
+    11: 5,
+    12: 5,
+    13: 6,
+    14: 6,
+    15: 7,
+    16: 7,
+    17: 8,
+    18: 8,
+    19: 9,
+    20: 9,  # info
+    21: 9,
+    22: 9,
+    23: 10,  # notice
+    24: 10,
+    25: 11,  # 25 = success in loguru
+    26: 11,
+    27: 12,
+    28: 12,
+    29: 13,
+    30: 13,  # warning
+    31: 13,
+    32: 13,
+    33: 14,
+    34: 14,
+    35: 15,
+    36: 15,
+    37: 16,
+    38: 16,
+    39: 17,
+    40: 17,  # error
+    41: 17,
+    42: 17,
+    43: 18,
+    44: 18,
+    45: 19,
+    46: 19,
+    47: 20,
+    48: 20,
+    49: 21,
+    50: 21,  # fatal/critical
+}
+"""Mapping from standard library logging level numbers to OTEL/logfire level numbers.
+Based on feeling rather than hard maths."""
+
 ATTRIBUTES_LOG_LEVEL_NAME_KEY = f'{LOGFIRE_ATTRIBUTES_NAMESPACE}.level_name'
 """Deprecated, use only ATTRIBUTES_LOG_LEVEL_NUM_KEY."""
 
 ATTRIBUTES_LOG_LEVEL_NUM_KEY = f'{LOGFIRE_ATTRIBUTES_NAMESPACE}.level_num'
 """The key within OTEL attributes where logfire puts the log level number."""
 
 
 # This is in this file to encourage using it instead of setting these attributes manually.
-def log_level_attributes(level: LevelName) -> dict[str, otel_types.AttributeValue]:
-    if level not in LEVEL_NUMBERS:
-        warnings.warn(f'Invalid log level name: {level!r}')
-        level = 'error'
+def log_level_attributes(level: LevelName | int) -> dict[str, otel_types.AttributeValue]:
+    if isinstance(level, str):
+        if level not in LEVEL_NUMBERS:
+            warnings.warn(f'Invalid log level name: {level!r}')
+            level = 'error'
+        level = LEVEL_NUMBERS[level]
 
     return {
-        ATTRIBUTES_LOG_LEVEL_NUM_KEY: LEVEL_NUMBERS[level],
+        ATTRIBUTES_LOG_LEVEL_NUM_KEY: level,
     }
 
 
 SpanTypeType = Literal['log', 'pending_span', 'span']
 
 ATTRIBUTES_SPAN_TYPE_KEY = f'{LOGFIRE_ATTRIBUTES_NAMESPACE}.span_type'
 """Used to differentiate logs, pending spans and regular spans. Absences should be interpreted as a real span."""
```

### Comparing `logfire-0.30.0/logfire/_internal/instrument.py` & `logfire-0.31.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/json_encoder.py` & `logfire-0.31.0/logfire/_internal/json_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,20 @@
     return to_json_value(o.tolist(), seen)
 
 
 def _pydantic_model_encoder(o: Any, seen: set[int]) -> JsonValue:
     import pydantic
 
     assert isinstance(o, pydantic.BaseModel)
-    return to_json_value(o.model_dump(), seen)
+    try:
+        dump = o.model_dump()
+    except AttributeError:  # pragma: no cover
+        # pydantic v1
+        dump = o.dict()  # type: ignore
+    return to_json_value(dump, seen)
 
 
 def _get_sqlalchemy_data(o: Any, seen: set[int]) -> JsonValue:
     try:
         from sqlalchemy import inspect as sa_inspect
 
         state = sa_inspect(o)
@@ -167,15 +172,15 @@
 
     return to_json_value(
         {field: getattr(o, field) if field not in deferred else '<deferred>' for field in o.__mapper__.attrs.keys()},
         seen,
     )
 
 
-EncoderFunction = Callable[[Any, set[int]], JsonValue]
+EncoderFunction = Callable[[Any, 'set[int]'], JsonValue]
 
 
 @lru_cache(maxsize=None)
 def encoder_by_type() -> dict[type[Any], EncoderFunction]:
     lookup: dict[type[Any], EncoderFunction] = {
         set: _set_encoder,
         frozenset: _set_encoder,
```

### Comparing `logfire-0.30.0/logfire/_internal/json_formatter.py` & `logfire-0.31.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/json_schema.py` & `logfire-0.31.0/logfire/_internal/json_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,15 +264,22 @@
     return {'type': 'object', 'title': obj.__class__.__name__, 'x-python-datatype': 'Exception'}
 
 
 def _pydantic_model_schema(obj: Any, seen: set[int]) -> JsonDict:
     import pydantic
 
     assert isinstance(obj, pydantic.BaseModel)
-    return _custom_object_schema(obj, 'PydanticModel', [*obj.model_fields, *(obj.model_extra or {})], seen)
+    try:
+        fields = obj.model_fields
+        extra = obj.model_extra or {}
+    except AttributeError:  # pragma: no cover
+        # pydantic v1
+        fields = obj.__fields__  # type: ignore
+        extra = {}
+    return _custom_object_schema(obj, 'PydanticModel', [*fields, *extra], seen)
 
 
 def _pandas_schema(obj: Any, _seen: set[int]) -> JsonDict:
     import pandas
 
     assert isinstance(obj, pandas.DataFrame)
```

### Comparing `logfire-0.30.0/logfire/_internal/json_types.py` & `logfire-0.31.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/main.py` & `logfire-0.31.0/logfire/_internal/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import atexit
+import inspect
 import sys
 import traceback
 import typing
 import warnings
 from functools import cached_property, partial
 from time import time
 from types import TracebackType
@@ -33,31 +34,32 @@
     ATTRIBUTES_VALIDATION_ERROR_KEY,
     DISABLE_CONSOLE_KEY,
     NULL_ARGS_KEY,
     OTLP_MAX_INT_SIZE,
     LevelName,
     log_level_attributes,
 )
-from .formatter import logfire_format
+from .formatter import logfire_format, logfire_format_with_magic
 from .instrument import LogfireArgs, instrument
 from .json_encoder import logfire_json_dumps
 from .json_schema import (
     JsonSchemaProperties,
     attributes_json_schema,
     attributes_json_schema_properties,
     create_json_schema,
 )
 from .metrics import ProxyMeterProvider
-from .stack_info import get_caller_stack_info
+from .stack_info import get_user_stack_info
 from .tracer import ProxyTracerProvider
 from .utils import uniquify_sequence
 
 if TYPE_CHECKING:
     import openai
     from fastapi import FastAPI
+    from opentelemetry.metrics import _Gauge as Gauge
     from starlette.requests import Request
     from starlette.websockets import WebSocket
 
 try:
     from pydantic import ValidationError
 except ImportError:  # pragma: no cover
     ValidationError = None
@@ -83,22 +85,20 @@
 
     def __init__(
         self,
         *,
         config: LogfireConfig = GLOBAL_CONFIG,
         sample_rate: float | None = None,
         tags: Sequence[str] = (),
-        stack_offset: int = 0,
         console_log: bool = True,
         otel_scope: str = 'logfire',
     ) -> None:
         self._tags = tuple(tags)
         self._config = config
         self._sample_rate = sample_rate
-        self._stack_offset = stack_offset
         self._console_log = console_log
         self._otel_scope = otel_scope
 
     @property
     def config(self) -> LogfireConfig:
         return self._config
 
@@ -124,28 +124,37 @@
             VERSION,
             is_span_tracer=is_span_tracer,
         )
 
     # If any changes are made to this method, they may need to be reflected in `_fast_span` as well.
     def _span(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         attributes: dict[str, Any],
         *,
         _tags: Sequence[str] | None = None,
         _span_name: str | None = None,
-        _level: LevelName | None = None,
-        _stack_offset: int = 3,
+        _level: LevelName | int | None = None,
     ) -> LogfireSpan:
-        stack_info = get_caller_stack_info(_stack_offset)
+        stack_info = get_user_stack_info()
         merged_attributes = {**stack_info, **attributes}
 
-        log_message = logfire_format(
-            msg_template, merged_attributes, self._config.scrubber, stack_offset=_stack_offset + 2
+        if self._config.inspect_arguments:
+            fstring_frame = inspect.currentframe().f_back  # type: ignore
+        else:
+            fstring_frame = None
+
+        log_message, extra_attrs, msg_template = logfire_format_with_magic(
+            msg_template,
+            merged_attributes,
+            self._config.scrubber,
+            fstring_frame=fstring_frame,
         )
+        merged_attributes.update(extra_attrs)
+        attributes.update(extra_attrs)  # for the JSON schema
         merged_attributes[ATTRIBUTES_MESSAGE_TEMPLATE_KEY] = msg_template
         merged_attributes[ATTRIBUTES_MESSAGE_KEY] = log_message
 
         otlp_attributes = user_attributes(merged_attributes)
 
         if json_schema_properties := attributes_json_schema_properties(attributes):
             otlp_attributes[ATTRIBUTES_JSON_SCHEMA_KEY] = attributes_json_schema(json_schema_properties)
@@ -185,25 +194,23 @@
     ) -> FastLogfireSpan:
         """A version of `_span` used by `@instrument` with `extract_args=True`.
 
         This is a bit faster than `_span` but not as fast as `_fast_span` because it supports message formatting
         and arbitrary types of attributes.
         """
         msg_template: str = attributes[ATTRIBUTES_MESSAGE_TEMPLATE_KEY]  # type: ignore
-        attributes[ATTRIBUTES_MESSAGE_KEY] = logfire_format(
-            msg_template, function_args, self._config.scrubber, stack_offset=4
-        )
+        attributes[ATTRIBUTES_MESSAGE_KEY] = logfire_format(msg_template, function_args, self._config.scrubber)
         if json_schema_properties := attributes_json_schema_properties(function_args):
             attributes[ATTRIBUTES_JSON_SCHEMA_KEY] = attributes_json_schema(json_schema_properties)
         attributes.update(user_attributes(function_args))
         return self._fast_span(name, attributes)
 
     def trace(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         /,
         *,
         _tags: Sequence[str] | None = None,
         _exc_info: ExcInfo = False,
         **attributes: Any,
     ) -> None:
         """Log a trace message.
@@ -221,19 +228,19 @@
             _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
 
                 Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
-        self.log('trace', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
+        self.log('trace', msg_template, attributes, tags=_tags, exc_info=_exc_info)
 
     def debug(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         /,
         *,
         _tags: Sequence[str] | None = None,
         _exc_info: ExcInfo = False,
         **attributes: Any,
     ) -> None:
         """Log a debug message.
@@ -251,19 +258,19 @@
             _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
 
                 Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
-        self.log('debug', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
+        self.log('debug', msg_template, attributes, tags=_tags, exc_info=_exc_info)
 
     def info(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         /,
         *,
         _tags: Sequence[str] | None = None,
         _exc_info: ExcInfo = False,
         **attributes: Any,
     ) -> None:
         """Log an info message.
@@ -281,19 +288,19 @@
             _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
 
                 Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
-        self.log('info', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
+        self.log('info', msg_template, attributes, tags=_tags, exc_info=_exc_info)
 
     def notice(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         /,
         *,
         _tags: Sequence[str] | None = None,
         _exc_info: ExcInfo = False,
         **attributes: Any,
     ) -> None:
         """Log a notice message.
@@ -311,19 +318,19 @@
             _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
 
                 Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
-        self.log('notice', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
+        self.log('notice', msg_template, attributes, tags=_tags, exc_info=_exc_info)
 
     def warn(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         /,
         *,
         _tags: Sequence[str] | None = None,
         _exc_info: ExcInfo = False,
         **attributes: Any,
     ) -> None:
         """Log a warning message.
@@ -341,19 +348,19 @@
             _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
 
                 Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
-        self.log('warn', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
+        self.log('warn', msg_template, attributes, tags=_tags, exc_info=_exc_info)
 
     def error(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         /,
         *,
         _tags: Sequence[str] | None = None,
         _exc_info: ExcInfo = False,
         **attributes: Any,
     ) -> None:
         """Log an error message.
@@ -371,19 +378,19 @@
             _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
 
                 Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
-        self.log('error', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
+        self.log('error', msg_template, attributes, tags=_tags, exc_info=_exc_info)
 
     def fatal(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         /,
         *,
         _tags: Sequence[str] | None = None,
         _exc_info: ExcInfo = False,
         **attributes: Any,
     ) -> None:
         """Log a fatal message.
@@ -401,19 +408,19 @@
             _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
 
                 Set to `True` to use the currently handled exception.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
-        self.log('fatal', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
+        self.log('fatal', msg_template, attributes, tags=_tags, exc_info=_exc_info)
 
     def exception(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         /,
         *,
         _tags: Sequence[str] | None = None,
         _exc_info: ExcInfo = True,
         **attributes: Any,
     ) -> None:
         """The same as `error` but with `_exc_info=True` by default.
@@ -425,25 +432,24 @@
             attributes: The attributes to bind to the log.
             _tags: An optional sequence of tags to include in the log.
             _exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
         """
         if any(k.startswith('_') for k in attributes):  # pragma: no cover
             raise ValueError('Attribute keys cannot start with an underscore.')
-        self.log('error', msg_template, attributes, stack_offset=1, tags=_tags, exc_info=_exc_info)
+        self.log('error', msg_template, attributes, tags=_tags, exc_info=_exc_info)
 
     def span(
         self,
-        msg_template: LiteralString,
+        msg_template: str,
         /,
         *,
         _tags: Sequence[str] | None = None,
         _span_name: str | None = None,
         _level: LevelName | None = None,
-        _stack_offset: int = 3,
         **attributes: Any,
     ) -> LogfireSpan:
         """Context manager for creating a span.
 
         ```py
         import logfire
 
@@ -452,27 +458,25 @@
         ```
 
         Args:
             msg_template: The template for the span message.
             _span_name: The span name. If not provided, the `msg_template` will be used.
             _tags: An optional sequence of tags to include in the span.
             _level: An optional log level name.
-            _stack_offset: The stack level offset to use when collecting stack info, defaults to `3`.
             attributes: The arguments to include in the span and format the message template with.
                 Attributes starting with an underscore are not allowed.
         """
         if any(k.startswith('_') for k in attributes):
             raise ValueError('Attribute keys cannot start with an underscore.')
         return self._span(
             msg_template,
             attributes,
             _tags=_tags,
             _span_name=_span_name,
             _level=_level,
-            _stack_offset=_stack_offset,
         )
 
     def instrument(
         self,
         msg_template: LiteralString | None = None,
         *,
         span_name: str | None = None,
@@ -499,20 +503,19 @@
             extract_args: Whether to extract arguments from the function signature and log them as span attributes.
         """
         args = LogfireArgs(tuple(self._tags), self._sample_rate, msg_template, span_name, extract_args)
         return instrument(self, args)
 
     def log(
         self,
-        level: LevelName,
-        msg_template: LiteralString,
+        level: LevelName | int,
+        msg_template: str,
         attributes: dict[str, Any] | None = None,
         tags: Sequence[str] | None = None,
         exc_info: ExcInfo = False,
-        stack_offset: int | None = None,
         console_log: bool | None = None,
         custom_scope_suffix: str | None = None,
     ) -> None:
         """Log a message.
 
         ```py
         import logfire
@@ -525,32 +528,47 @@
             msg_template: The message to log.
             attributes: The attributes to bind to the log.
             tags: An optional sequence of tags to include in the log.
             exc_info: Set to an exception or a tuple as returned by [`sys.exc_info()`][sys.exc_info]
                 to record a traceback with the log message.
 
                 Set to `True` to use the currently handled exception.
-            stack_offset: The stack level offset to use when collecting stack info, also affects the warning which
-                message formatting might emit, defaults to `0` which means the stack info will be collected from the
-                position where [`logfire.log`][logfire.Logfire.log] was called.
             console_log: Whether to log to the console, defaults to `True`.
             custom_scope_suffix: A custom suffix to append to `logfire.` e.g. `logfire.loguru`.
 
                 It should only be used when instrumenting another library with Logfire, such as structlog or loguru.
 
                 See the `instrumenting_module_name` parameter on
                 [TracerProvider.get_tracer][opentelemetry.sdk.trace.TracerProvider.get_tracer] for more info.
         """
-        stack_offset = (self._stack_offset if stack_offset is None else stack_offset) + 2
-        stack_info = get_caller_stack_info(stack_offset)
+        stack_info = get_user_stack_info()
 
         attributes = attributes or {}
         merged_attributes = {**stack_info, **attributes}
         if (msg := attributes.pop(ATTRIBUTES_MESSAGE_KEY, None)) is None:
-            msg = logfire_format(msg_template, merged_attributes, self._config.scrubber, stack_offset=stack_offset + 2)
+            fstring_frame = None
+            if self._config.inspect_arguments:
+                fstring_frame = inspect.currentframe()
+                if fstring_frame.f_back.f_code.co_filename == Logfire.log.__code__.co_filename:  # type: ignore
+                    # fstring_frame.f_back should be the user's frame.
+                    # The user called logfire.info or a similar method rather than calling logfire.log directly.
+                    fstring_frame = fstring_frame.f_back  # type: ignore
+
+            msg, extra_attrs, msg_template = logfire_format_with_magic(
+                msg_template,
+                merged_attributes,
+                self._config.scrubber,
+                fstring_frame=fstring_frame,
+            )
+            if extra_attrs:
+                merged_attributes.update(extra_attrs)
+                # Only do this if extra_attrs is not empty since the copy of `attributes` might be expensive.
+                # We update both because attributes_json_schema_properties looks at `attributes`.
+                attributes = {**attributes, **extra_attrs}
+
         otlp_attributes = user_attributes(merged_attributes)
         otlp_attributes = {
             ATTRIBUTES_SPAN_TYPE_KEY: 'log',
             **log_level_attributes(level),
             ATTRIBUTES_MESSAGE_TEMPLATE_KEY: msg_template,
             ATTRIBUTES_MESSAGE_KEY: msg,
             **otlp_attributes,
@@ -662,15 +680,14 @@
             A new Logfire instance with the given settings applied.
         """
         # TODO add sample_rate once it's more stable
         return Logfire(
             config=self._config,
             tags=self._tags + tuple(tags),
             sample_rate=self._sample_rate,
-            stack_offset=self._stack_offset if stack_offset is None else stack_offset,
             console_log=self._console_log if console_log is None else console_log,
             otel_scope=self._otel_scope if custom_scope_suffix is None else f'logfire.{custom_scope_suffix}',
         )
 
     def force_flush(self, timeout_millis: int = 3_000) -> bool:  # pragma: no cover
         """Force flush all spans.
 
@@ -799,15 +816,15 @@
         )
 
     def instrument_openai(
         self, openai_client: openai.OpenAI | openai.AsyncOpenAI, *, suppress_other_instrumentation: bool = True
     ) -> ContextManager[None]:
         """Instrument an OpenAI client so that spans are automatically created for each request.
 
-        The following methods are instrumented for both the sync the async clients:
+        The following methods are instrumented for both the sync and the async clients:
 
         - [`client.chat.completions.create`](https://platform.openai.com/docs/guides/text-generation/chat-completions-api) — with and without `stream=True`
         - [`client.completions.create`](https://platform.openai.com/docs/guides/text-generation/completions-api) — with and without `stream=True`
         - [`client.embeddings.create`](https://platform.openai.com/docs/guides/embeddings/how-to-get-embeddings)
         - [`client.images.generate`](https://platform.openai.com/docs/guides/images/generations)
 
         When `stream=True` a second span is created to instrument the streamed response.
@@ -926,14 +943,41 @@
             description: The description of the metric.
 
         Returns:
             The histogram metric.
         """
         return self._config.meter.create_histogram(name, unit, description)
 
+    def metric_gauge(self, name: str, *, unit: str = '', description: str = '') -> Gauge:
+        """Create a gauge metric.
+
+        Gauge is a synchronous instrument which can be used to record non-additive measurements.
+
+        ```py
+        import logfire
+
+        gauge = logfire.metric_gauge('system.cpu_usage', unit='%', description='CPU usage')
+
+
+        def update_cpu_usage(cpu_percent):
+            gauge.set(cpu_percent)
+        ```
+
+        See the [Opentelemetry documentation](https://opentelemetry.io/docs/specs/otel/metrics/api/#gauge) about gauges.
+
+        Args:
+            name: The name of the metric.
+            unit: The unit of the metric.
+            description: The description of the metric.
+
+        Returns:
+            The gauge metric.
+        """
+        return self._config.meter.create_gauge(name, unit, description)
+
     def metric_up_down_counter(self, name: str, *, unit: str = '', description: str = '') -> UpDownCounter:
         """Create an up-down counter metric.
 
         An up-down counter is a cumulative metric that represents a single numerical value that can be adjusted up or
         down.
 
         ```py
@@ -1279,17 +1323,17 @@
             timestamp=timestamp,
             escaped=escaped,
         )
 
     def is_recording(self) -> bool:
         return self._span is not None and self._span.is_recording()
 
-    def set_level(self, level_name: LevelName):
+    def set_level(self, level: LevelName | int):
         """Set the log level of this span."""
-        attributes = log_level_attributes(level_name)
+        attributes = log_level_attributes(level)
         if self._span is None:
             self._otlp_attributes.update(attributes)
         else:
             self._span.set_attributes(attributes)
 
     def _get_attribute(self, key: str, default: Any) -> Any:
         attributes = getattr(self._span, 'attributes', self._otlp_attributes)
```

### Comparing `logfire-0.30.0/logfire/_internal/metrics.py` & `logfire-0.31.0/logfire/_internal/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
     UpDownCounter,
 )
 from opentelemetry.sdk.metrics import MeterProvider as SDKMeterProvider
 from opentelemetry.util.types import Attributes
 
 try:
     # This only exists in opentelemetry-sdk>=1.23.0
-    from opentelemetry.metrics import _Gauge as Gauge
+    from opentelemetry.metrics import _Gauge
+
+    Gauge = _Gauge
 except ImportError:  # pragma: no cover
     Gauge = None
 
 # All the cpu_times fields provided by psutil (used by system_metrics) across all platforms,
 # except for 'guest' and 'guest_nice' which are included in 'user' and 'nice' in Linux (see psutil._cpu_tot_time).
 # Docs: https://psutil.readthedocs.io/en/latest/#psutil.cpu_times
 CPU_FIELDS = 'idle user system irq softirq nice iowait steal interrupt dpc'.split()
@@ -202,21 +204,27 @@
         description: str = '',
     ) -> Histogram:
         with self._lock:
             proxy = _ProxyHistogram(self._meter.create_histogram(name, unit, description), name, unit, description)
             self._instruments.add(proxy)
             return proxy
 
-    # TODO(Marcelo): We should test this method.
     def create_gauge(
         self,
         name: str,
         unit: str = '',
         description: str = '',
-    ):  # pragma: no cover
+    ) -> _Gauge:
+        if Gauge is None:
+            # This only exists in opentelemetry-sdk>=1.23.0
+            raise RuntimeError(
+                'Gauge is not available in this version of OpenTelemetry SDK.\n'
+                'You should upgrade to 1.23.0 or newer:\n'
+                '   pip install opentelemetry-sdk>=1.23.0'
+            )
         with self._lock:
             proxy = _ProxyGauge(self._meter.create_gauge(name, unit, description), name, unit, description)
             self._instruments.add(proxy)
             return proxy
 
     def create_observable_gauge(
         self,
```

### Comparing `logfire-0.30.0/logfire/_internal/scrubbing.py` & `logfire-0.31.0/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/tracer.py` & `logfire-0.31.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/utils.py` & `logfire-0.31.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/auto_trace/__init__.py` & `logfire-0.31.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.31.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.31.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/auto_trace/types.py` & `logfire-0.31.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/exporters/console.py` & `logfire-0.31.0/logfire/_internal/exporters/console.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from __future__ import annotations
 
 import json
 import os
 import sys
 from collections.abc import Sequence
 from datetime import datetime, timezone
+from textwrap import indent as indent_text
 from typing import Any, List, Literal, Mapping, TextIO, Tuple, cast
 
-from opentelemetry.sdk.trace import ReadableSpan
+from opentelemetry.sdk.trace import Event, ReadableSpan
 from opentelemetry.sdk.trace.export import SpanExporter, SpanExportResult
 from opentelemetry.util import types as otel_types
 from rich.columns import Columns
 from rich.console import Console, Group
 from rich.syntax import Syntax
 from rich.text import Text
 
@@ -121,14 +122,17 @@
         else:
             print(''.join(text for text, _style in parts), file=self._output)
 
         # This uses a separate system for color vs no-color because it's not simple text:
         # in the rich case it uses syntax highlighting and columns for layout.
         self._print_arguments(span, indent_str)
 
+        exc_event = next((event for event in span.events or [] if event.name == 'exception'), None)
+        self._print_exc_info(exc_event, indent_str)
+
     def _span_text_parts(self, span: ReadableSpan, indent: int) -> tuple[str, TextParts]:
         """Return the formatted message or span name and parts containing basic span information.
 
         The following information is included:
         * timestamp
         * message (maybe indented)
         * tags
@@ -251,14 +255,35 @@
             value_lines = value_code.splitlines()
             out += [f'{indent_str}│ {k}={value_lines[0]}']
             prefix = f'{indent_str}│ {" " * len(k)} '
             for line in value_lines[1:]:
                 out += [f'{prefix}{line}']
         print('\n'.join(out), file=self._output)
 
+    def _print_exc_info(self, exc_event: Event | None, indent_str: str) -> None:
+        """Print exception information if an exception event is present."""
+        if exc_event is None or not exc_event.attributes:
+            return
+
+        exc_type = cast(str, exc_event.attributes.get('exception.type'))
+        exc_msg = cast(str, exc_event.attributes.get('exception.message'))
+        exc_tb = cast(str, exc_event.attributes.get('exception.stacktrace'))
+
+        if self._console:
+            barrier = Text(indent_str + '│ ', style='blue', end='')
+            exc_type = Text(f'{exc_type}: ', end='', style='bold red')
+            exc_msg = Text(exc_msg)
+            indented_code = indent_text(exc_tb, indent_str + '│ ')
+            exc_tb = Syntax(indented_code, 'python', background_color='default')
+            self._console.print(Group(barrier, exc_type, exc_msg), exc_tb)
+        else:
+            out = [f'{indent_str}│ {exc_type}: {exc_msg}']
+            out += [indent_text(exc_tb, indent_str + '│ ')]
+            print('\n'.join(out), file=self._output)
+
     def force_flush(self, timeout_millis: int = 0) -> bool:  # pragma: no cover
         """Force flush all spans, does nothing for this exporter."""
         return True
 
 
 class IndentedConsoleSpanExporter(SimpleConsoleSpanExporter):
     """The ConsoleSpanExporter exports spans to the console, indented.
```

### Comparing `logfire-0.30.0/logfire/_internal/exporters/fallback.py` & `logfire-0.31.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/exporters/file.py` & `logfire-0.31.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/exporters/otlp.py` & `logfire-0.31.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.31.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/exporters/remove_pending.py` & `logfire-0.31.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/exporters/wrapper.py` & `logfire-0.31.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/integrations/executors.py` & `logfire-0.31.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/integrations/fastapi.py` & `logfire-0.31.0/logfire/_internal/integrations/fastapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,36 @@
 import inspect
 from contextlib import contextmanager
 from functools import lru_cache
 from typing import Any, Callable, ContextManager, Iterable, Literal, cast
 from weakref import WeakKeyDictionary
 
 import fastapi.routing
-from fastapi import BackgroundTasks, FastAPI, Response
+from fastapi import BackgroundTasks, FastAPI
 from fastapi.routing import APIRoute, APIWebSocketRoute
 from fastapi.security import SecurityScopes
-from opentelemetry.instrumentation.asgi import get_host_port_url_tuple  # type: ignore
-from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
-from opentelemetry.semconv.trace import SpanAttributes
-from opentelemetry.util.http import get_excluded_urls, parse_excluded_urls
 from starlette.requests import Request
+from starlette.responses import Response
 from starlette.websockets import WebSocket
 
-from logfire import Logfire
-
+from ..main import Logfire
 from ..stack_info import StackInfo, get_code_object_info
 
+try:
+    from opentelemetry.instrumentation.asgi import get_host_port_url_tuple  # type: ignore
+    from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
+    from opentelemetry.semconv.trace import SpanAttributes
+    from opentelemetry.util.http import get_excluded_urls, parse_excluded_urls
+except ModuleNotFoundError:
+    raise RuntimeError(
+        'The `logfire.instrument_fastapi()` requires the `opentelemetry-instrumentation-fastapi` package.\n'
+        'You can install this with:\n'
+        "    pip install 'logfire[fastapi]'"
+    )
+
 
 def instrument_fastapi(
     logfire_instance: Logfire,
     app: FastAPI,
     *,
     request_attributes_mapper: Callable[
         [
```

### Comparing `logfire-0.30.0/logfire/_internal/integrations/openai.py` & `logfire-0.31.0/logfire/_internal/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/_internal/integrations/psycopg.py` & `logfire-0.31.0/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/integrations/logging.py` & `logfire-0.31.0/logfire/integrations/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 
 import inspect
 from logging import NOTSET, Handler as LoggingHandler, LogRecord, StreamHandler
 from typing import Any, ClassVar, Mapping, cast
 
 from logfire import log
 
-from .._internal.constants import ATTRIBUTES_LOGGING_ARGS_KEY, ATTRIBUTES_MESSAGE_KEY, ATTRIBUTES_MESSAGE_TEMPLATE_KEY
+from .._internal.constants import (
+    ATTRIBUTES_LOGGING_ARGS_KEY,
+    ATTRIBUTES_MESSAGE_KEY,
+    ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
+    LOGGING_TO_OTEL_LEVEL_NUMBERS,
+)
 
 # skip natural LogRecord attributes
 # http://docs.python.org/library/logging.html#logrecord-attributes
 RESERVED_ATTRS: frozenset[str] = frozenset(
     [
         'args',
         'asctime',
@@ -71,15 +76,15 @@
                     return
                 frame = frame.f_back
 
         attributes = self.fill_attributes(record)
 
         log(
             msg_template=attributes.pop(ATTRIBUTES_MESSAGE_TEMPLATE_KEY, record.msg),
-            level=record.levelname.lower(),  # type: ignore
+            level=LOGGING_TO_OTEL_LEVEL_NUMBERS.get(record.levelno, record.levelno),
             attributes=attributes,
             custom_scope_suffix=self.custom_scope_suffix,
             exc_info=record.exc_info,
         )
 
     def fill_attributes(self, record: LogRecord) -> dict[str, Any]:
         """Fill the attributes to send to Logfire.
```

### Comparing `logfire-0.30.0/logfire/integrations/loguru.py` & `logfire-0.31.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/logfire/integrations/pydantic.py` & `logfire-0.31.0/logfire/integrations/pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,18 +64,14 @@
 
     * `all`: Record all validation events.
     * `failure`: Record only validation failures.
     * `metrics`: Record only validation metrics.
     """
 
 
-_USER_STACK_OFFSET = 3
-"""The number of frames to skip when logging from user code."""
-
-
 class _ValidateWrapper:
     """Decorator factory for one schema validator method."""
 
     __slots__ = (
         'validation_method',
         'schema_name',
         '_record',
@@ -211,15 +207,14 @@
             level='warn',
             msg_template='Validation on {schema_name} failed',
             attributes={
                 'schema_name': self.schema_name,
                 'error_count': error.error_count(),
                 'errors': error.errors(include_url=False),
             },
-            stack_offset=_USER_STACK_OFFSET,
         )
 
     def _on_error_span(self, span: LogfireSpan, error: ValidationError):
         self._set_span_attributes(
             span,
             success=False,
             status='failed',
@@ -233,15 +228,14 @@
         self._logfire.log(
             level='error',
             msg_template='Validation on {schema_name} raised {exception_type}',
             attributes={
                 'schema_name': self.schema_name,
                 'exception_type': type(exception).__name__,
             },
-            stack_offset=_USER_STACK_OFFSET,
             exc_info=exception,
         )
 
     def _on_exception_span(self, span: LogfireSpan, exception: Exception):
         self._set_span_attributes(
             span,
             success=False,
```

### Comparing `logfire-0.30.0/tests/conftest.py` & `logfire-0.31.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Import this anyio backend early to prevent weird bug caused by concurrent calls to ast.parse
+from __future__ import annotations
+
 import os
+import sys
 from pathlib import Path
+from typing import Any
 
 import anyio._backends._asyncio  # noqa  # type: ignore
 import pytest
 from opentelemetry import trace
 from opentelemetry.sdk.metrics.export import InMemoryMetricReader
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 
@@ -34,29 +38,43 @@
 
 
 @pytest.fixture
 def metrics_reader() -> InMemoryMetricReader:
     return InMemoryMetricReader(preferred_temporality=METRICS_PREFERRED_TEMPORALITY)
 
 
-@pytest.fixture(autouse=True)
-def config(
+@pytest.fixture
+def config_kwargs(
     exporter: TestExporter,
-    metrics_reader: InMemoryMetricReader,
     id_generator: IncrementalIdGenerator,
     time_generator: TimeGenerator,
-) -> None:
-    configure(
+) -> dict[str, Any]:
+    """
+    Use this when you want to `logfire.configure()` with a variation of the default configuration.
+
+    Note that this doesn't set `metric_readers` because `metrics_reader` can't be used twice.
+    """
+    return dict(
         send_to_logfire=False,
         console=False,
         id_generator=id_generator,
         ns_timestamp_generator=time_generator,
         processors=[SimpleSpanProcessor(exporter)],
-        metric_readers=[metrics_reader],
         collect_system_metrics=False,
+        # Ensure that inspect_arguments doesn't break things in most versions
+        # (it's off by default for <3.11) but it's completely forbidden for 3.8.
+        inspect_arguments=sys.version_info[:2] >= (3, 9),
+    )
+
+
+@pytest.fixture(autouse=True)
+def config(config_kwargs: dict[str, Any], metrics_reader: InMemoryMetricReader) -> None:
+    configure(
+        **config_kwargs,
+        metric_readers=[metrics_reader],
     )
     # sanity check: there are no active spans
     # if there are, it means that some test forgot to close them
     # which may mess with other tests
     span = trace.get_current_span()
     assert span is trace.INVALID_SPAN
```

### Comparing `logfire-0.30.0/tests/test_auto_trace.py` & `logfire-0.31.0/tests/test_auto_trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,127 +43,128 @@
     # The exact plain loader here isn't that essential.
     assert isinstance(loader.plain_spec.loader, SourceFileLoader)
     assert loader.plain_spec.name == foo.__name__ == foo.__spec__.name == 'tests.auto_trace_samples.foo'
 
     with pytest.raises(IndexError):  # foo.bar intentionally raises an error to test that it's recorded below
         asyncio.run(foo.bar())
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'Calling tests.auto_trace_samples.foo.bar (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'foo.py',
-                'code.lineno': 123,
-                'code.function': 'bar',
-                'logfire.msg_template': 'Calling tests.auto_trace_samples.foo.bar',
-                'logfire.msg': 'Calling tests.auto_trace_samples.foo.bar',
-                'logfire.span_type': 'pending_span',
-                'logfire.tags': ('auto-trace',),
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'Calling tests.auto_trace_samples.foo.bar (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'foo.py',
+                    'code.lineno': 123,
+                    'code.function': 'bar',
+                    'logfire.msg_template': 'Calling tests.auto_trace_samples.foo.bar',
+                    'logfire.msg': 'Calling tests.auto_trace_samples.foo.bar',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.tags': ('auto-trace',),
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'Calling async_gen via @instrument (pending)',
-            'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'foo.py',
-                'code.lineno': 123,
-                'code.function': 'async_gen',
-                'logfire.msg_template': 'Calling async_gen via @instrument',
-                'logfire.span_type': 'pending_span',
-                'logfire.msg': 'Calling async_gen via @instrument',
-                'logfire.pending_parent_id': '0000000000000001',
+            {
+                'name': 'Calling async_gen via @instrument (pending)',
+                'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'foo.py',
+                    'code.lineno': 123,
+                    'code.function': 'async_gen',
+                    'logfire.msg_template': 'Calling async_gen via @instrument',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.msg': 'Calling async_gen via @instrument',
+                    'logfire.pending_parent_id': '0000000000000001',
+                },
             },
-        },
-        {
-            'name': 'Calling tests.auto_trace_samples.foo.gen (pending)',
-            'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
-            'start_time': 3000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'code.filepath': 'foo.py',
-                'code.lineno': 123,
-                'code.function': 'gen',
-                'logfire.msg_template': 'Calling tests.auto_trace_samples.foo.gen',
-                'logfire.msg': 'Calling tests.auto_trace_samples.foo.gen',
-                'logfire.span_type': 'pending_span',
-                'logfire.tags': ('auto-trace',),
-                'logfire.pending_parent_id': '0000000000000003',
+            {
+                'name': 'Calling tests.auto_trace_samples.foo.gen (pending)',
+                'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'start_time': 3000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'code.filepath': 'foo.py',
+                    'code.lineno': 123,
+                    'code.function': 'gen',
+                    'logfire.msg_template': 'Calling tests.auto_trace_samples.foo.gen',
+                    'logfire.msg': 'Calling tests.auto_trace_samples.foo.gen',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.tags': ('auto-trace',),
+                    'logfire.pending_parent_id': '0000000000000003',
+                },
             },
-        },
-        {
-            'name': 'Calling tests.auto_trace_samples.foo.gen',
-            'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 3000000000,
-            'end_time': 4000000000,
-            'attributes': {
-                'code.filepath': 'foo.py',
-                'code.lineno': 123,
-                'code.function': 'gen',
-                'logfire.msg_template': 'Calling tests.auto_trace_samples.foo.gen',
-                'logfire.span_type': 'span',
-                'logfire.tags': ('auto-trace',),
-                'logfire.msg': 'Calling tests.auto_trace_samples.foo.gen',
+            {
+                'name': 'Calling tests.auto_trace_samples.foo.gen',
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 3000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'code.filepath': 'foo.py',
+                    'code.lineno': 123,
+                    'code.function': 'gen',
+                    'logfire.msg_template': 'Calling tests.auto_trace_samples.foo.gen',
+                    'logfire.span_type': 'span',
+                    'logfire.tags': ('auto-trace',),
+                    'logfire.msg': 'Calling tests.auto_trace_samples.foo.gen',
+                },
             },
-        },
-        {
-            'name': 'Calling async_gen via @instrument',
-            'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 5000000000,
-            'attributes': {
-                'code.filepath': 'foo.py',
-                'code.lineno': 123,
-                'code.function': 'async_gen',
-                'logfire.msg_template': 'Calling async_gen via @instrument',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'Calling async_gen via @instrument',
+            {
+                'name': 'Calling async_gen via @instrument',
+                'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 5000000000,
+                'attributes': {
+                    'code.filepath': 'foo.py',
+                    'code.lineno': 123,
+                    'code.function': 'async_gen',
+                    'logfire.msg_template': 'Calling async_gen via @instrument',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'Calling async_gen via @instrument',
+                },
             },
-        },
-        {
-            'name': 'Calling tests.auto_trace_samples.foo.bar',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 7000000000,
-            'attributes': {
-                'code.filepath': 'foo.py',
-                'code.lineno': 123,
-                'code.function': 'bar',
-                'logfire.msg_template': 'Calling tests.auto_trace_samples.foo.bar',
-                'logfire.span_type': 'span',
-                'logfire.tags': ('auto-trace',),
-                'logfire.msg': 'Calling tests.auto_trace_samples.foo.bar',
-                'logfire.level_num': 17,
+            {
+                'name': 'Calling tests.auto_trace_samples.foo.bar',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 7000000000,
+                'attributes': {
+                    'code.filepath': 'foo.py',
+                    'code.lineno': 123,
+                    'code.function': 'bar',
+                    'logfire.msg_template': 'Calling tests.auto_trace_samples.foo.bar',
+                    'logfire.span_type': 'span',
+                    'logfire.tags': ('auto-trace',),
+                    'logfire.msg': 'Calling tests.auto_trace_samples.foo.bar',
+                    'logfire.level_num': 17,
+                },
+                'events': [
+                    {
+                        'name': 'exception',
+                        'timestamp': 6000000000,
+                        'attributes': {
+                            'exception.type': 'IndexError',
+                            'exception.message': 'list index out of range',
+                            'exception.stacktrace': 'IndexError: list index out of range',
+                            'exception.escaped': 'True',
+                        },
+                    }
+                ],
             },
-            'events': [
-                {
-                    'name': 'exception',
-                    'timestamp': 6000000000,
-                    'attributes': {
-                        'exception.type': 'IndexError',
-                        'exception.message': 'list index out of range',
-                        'exception.stacktrace': 'IndexError: list index out of range',
-                        'exception.escaped': 'True',
-                    },
-                }
-            ],
-        },
-    ]
+        ]
+    )
 
 
 def test_default_modules() -> None:
     # Check that nothing gets imported during this test,
     # because we don't want anything to get auto-traced here.
     imported_modules = set(sys.modules.items())
 
@@ -427,15 +428,14 @@
 def test_no_auto_trace():
     filtered_calling_strings = {
         'Calling module.name.traced_func',
         'Calling module.name.traced_func.<locals>.inner',
         'Calling module.name.TracedClass.traced_method',
     }
 
-    # insert_assert(get_calling_strings(no_auto_trace_sample.replace('@no_auto_trace', '')))
     all_calling_strings = {
         'Calling module.name.not_traced_func',
         'Calling module.name.TracedClass.traced_method',
         'Calling module.name.NotTracedClass.would_be_traced_method',
         'Calling module.name.not_traced_func.<locals>.inner',
         'Calling module.name.traced_func',
         'Calling module.name.NotTracedClass.would_be_traced_method.<locals>.inner',
```

### Comparing `logfire-0.30.0/tests/test_backfill.py` & `logfire-0.31.0/tests/test_backfill.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 from datetime import datetime
 from io import BytesIO
 
 import pytest
+from inline_snapshot import snapshot
 from opentelemetry.proto.collector.trace.v1.trace_service_pb2 import ExportTraceServiceRequest
 
 from logfire._internal.backfill import Log, PrepareBackfill, StartSpan
 from logfire._internal.exporters.file import FileParser, to_json_lines
 
 
 def test_write_spans_and_logs() -> None:
@@ -37,137 +38,138 @@
             otel_resource_attributes={'telemetry.sdk.version': '1.0.0'},  # to make output deterministic
         )
         prep_backfill.write(log)
         prep_backfill.write(span.end(datetime(2023, 1, 2, 0, 0, 1)))
 
     output.seek(0)
     lines = [json.loads(line) for line in to_json_lines(output)]
-    # insert_assert(lines)
-    assert lines == [
-        {
-            'resourceSpans': [
-                {
-                    'resource': {
-                        'attributes': [
-                            {
-                                'key': 'telemetry.sdk.language',
-                                'value': {'stringValue': 'python'},
-                            },
-                            {
-                                'key': 'telemetry.sdk.name',
-                                'value': {'stringValue': 'opentelemetry'},
-                            },
-                            {
-                                'key': 'telemetry.sdk.version',
-                                'value': {'stringValue': '1.0.0'},
-                            },
-                            {
-                                'key': 'service.name',
-                                'value': {'stringValue': 'docs.pydantic.dev'},
-                            },
-                        ]
-                    },
-                    'scopeSpans': [
-                        {
-                            'scope': {'name': 'logfire'},
-                            'spans': [
-                                {
-                                    'traceId': 'AAAAAAAAAAAAAAAAAAAAAg==',
-                                    'spanId': 'AAAAAAAAAAM=',
-                                    'parentSpanId': 'AAAAAAAAAAE=',
-                                    'name': 'GET {path=}',
-                                    'kind': 'SPAN_KIND_INTERNAL',
-                                    'startTimeUnixNano': '1672531200000000000',
-                                    'endTimeUnixNano': '1672531200000000000',
-                                    'attributes': [
-                                        {
-                                            'key': 'logfire.span_type',
-                                            'value': {'stringValue': 'log'},
-                                        },
-                                        {
-                                            'key': 'logfire.level_num',
-                                            'value': {'intValue': '9'},
-                                        },
-                                        {
-                                            'key': 'logfire.msg_template',
-                                            'value': {'stringValue': 'GET {path=}'},
-                                        },
-                                        {
-                                            'key': 'logfire.msg',
-                                            'value': {'stringValue': 'GET /test'},
-                                        },
-                                        {'key': 'path', 'value': {'stringValue': '/test'}},
-                                    ],
-                                    'status': {'code': 'STATUS_CODE_OK'},
-                                }
-                            ],
-                        }
-                    ],
-                }
-            ]
-        },
-        {
-            'resourceSpans': [
-                {
-                    'resource': {
-                        'attributes': [
-                            {
-                                'key': 'telemetry.sdk.language',
-                                'value': {'stringValue': 'python'},
-                            },
-                            {
-                                'key': 'telemetry.sdk.name',
-                                'value': {'stringValue': 'opentelemetry'},
-                            },
-                            {
-                                'key': 'telemetry.sdk.version',
-                                'value': {'stringValue': '1.0.0'},
-                            },
-                            {
-                                'key': 'service.name',
-                                'value': {'stringValue': 'docs.pydantic.dev'},
-                            },
-                        ]
-                    },
-                    'scopeSpans': [
-                        {
-                            'scope': {'name': 'logfire'},
-                            'spans': [
-                                {
-                                    'traceId': 'AAAAAAAAAAAAAAAAAAAAAg==',
-                                    'spanId': 'AAAAAAAAAAE=',
-                                    'name': 'session',
-                                    'kind': 'SPAN_KIND_INTERNAL',
-                                    'startTimeUnixNano': '1672531200000000000',
-                                    'endTimeUnixNano': '1672617601000000000',
-                                    'attributes': [
-                                        {
-                                            'key': 'logfire.span_type',
-                                            'value': {'stringValue': 'log'},
-                                        },
-                                        {
-                                            'key': 'logfire.msg_template',
-                                            'value': {'stringValue': 'session {user_id=} {path=}'},
-                                        },
-                                        {
-                                            'key': 'logfire.msg',
-                                            'value': {'stringValue': 'session user_id=123 path=/test'},
-                                        },
-                                        {'key': 'user_id', 'value': {'stringValue': '123'}},
-                                        {'key': 'path', 'value': {'stringValue': '/test'}},
-                                    ],
-                                    'status': {'code': 'STATUS_CODE_OK'},
-                                }
-                            ],
-                        }
-                    ],
-                }
-            ]
-        },
-    ]
+    assert lines == snapshot(
+        [
+            {
+                'resourceSpans': [
+                    {
+                        'resource': {
+                            'attributes': [
+                                {
+                                    'key': 'telemetry.sdk.language',
+                                    'value': {'stringValue': 'python'},
+                                },
+                                {
+                                    'key': 'telemetry.sdk.name',
+                                    'value': {'stringValue': 'opentelemetry'},
+                                },
+                                {
+                                    'key': 'telemetry.sdk.version',
+                                    'value': {'stringValue': '1.0.0'},
+                                },
+                                {
+                                    'key': 'service.name',
+                                    'value': {'stringValue': 'docs.pydantic.dev'},
+                                },
+                            ]
+                        },
+                        'scopeSpans': [
+                            {
+                                'scope': {'name': 'logfire'},
+                                'spans': [
+                                    {
+                                        'traceId': 'AAAAAAAAAAAAAAAAAAAAAg==',
+                                        'spanId': 'AAAAAAAAAAM=',
+                                        'parentSpanId': 'AAAAAAAAAAE=',
+                                        'name': 'GET {path=}',
+                                        'kind': 'SPAN_KIND_INTERNAL',
+                                        'startTimeUnixNano': '1672531200000000000',
+                                        'endTimeUnixNano': '1672531200000000000',
+                                        'attributes': [
+                                            {
+                                                'key': 'logfire.span_type',
+                                                'value': {'stringValue': 'log'},
+                                            },
+                                            {
+                                                'key': 'logfire.level_num',
+                                                'value': {'intValue': '9'},
+                                            },
+                                            {
+                                                'key': 'logfire.msg_template',
+                                                'value': {'stringValue': 'GET {path=}'},
+                                            },
+                                            {
+                                                'key': 'logfire.msg',
+                                                'value': {'stringValue': 'GET /test'},
+                                            },
+                                            {'key': 'path', 'value': {'stringValue': '/test'}},
+                                        ],
+                                        'status': {'code': 'STATUS_CODE_OK'},
+                                    }
+                                ],
+                            }
+                        ],
+                    }
+                ]
+            },
+            {
+                'resourceSpans': [
+                    {
+                        'resource': {
+                            'attributes': [
+                                {
+                                    'key': 'telemetry.sdk.language',
+                                    'value': {'stringValue': 'python'},
+                                },
+                                {
+                                    'key': 'telemetry.sdk.name',
+                                    'value': {'stringValue': 'opentelemetry'},
+                                },
+                                {
+                                    'key': 'telemetry.sdk.version',
+                                    'value': {'stringValue': '1.0.0'},
+                                },
+                                {
+                                    'key': 'service.name',
+                                    'value': {'stringValue': 'docs.pydantic.dev'},
+                                },
+                            ]
+                        },
+                        'scopeSpans': [
+                            {
+                                'scope': {'name': 'logfire'},
+                                'spans': [
+                                    {
+                                        'traceId': 'AAAAAAAAAAAAAAAAAAAAAg==',
+                                        'spanId': 'AAAAAAAAAAE=',
+                                        'name': 'session',
+                                        'kind': 'SPAN_KIND_INTERNAL',
+                                        'startTimeUnixNano': '1672531200000000000',
+                                        'endTimeUnixNano': '1672617601000000000',
+                                        'attributes': [
+                                            {
+                                                'key': 'logfire.span_type',
+                                                'value': {'stringValue': 'log'},
+                                            },
+                                            {
+                                                'key': 'logfire.msg_template',
+                                                'value': {'stringValue': 'session {user_id=} {path=}'},
+                                            },
+                                            {
+                                                'key': 'logfire.msg',
+                                                'value': {'stringValue': 'session user_id=123 path=/test'},
+                                            },
+                                            {'key': 'user_id', 'value': {'stringValue': '123'}},
+                                            {'key': 'path', 'value': {'stringValue': '/test'}},
+                                        ],
+                                        'status': {'code': 'STATUS_CODE_OK'},
+                                    }
+                                ],
+                            }
+                        ],
+                    }
+                ]
+            },
+        ]
+    )
 
 
 @pytest.mark.parametrize('read_chunk_size', [1, 10, 100, 1_000, 10_000])
 def test_parser(read_chunk_size: int) -> None:
     data = BytesIO()
     with PrepareBackfill(data) as prep_backfill:
         spans: list[StartSpan] = []
```

### Comparing `logfire-0.30.0/tests/test_cli.py` & `logfire-0.31.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,34 +49,37 @@
             pass
         assert capsys.readouterr().err == 'User cancelled.\n'
 
 
 def test_whoami(tmp_dir_cwd: Path, logfire_credentials: LogfireCredentials, capsys: pytest.CaptureFixture[str]) -> None:
     logfire_credentials.write_creds_file(tmp_dir_cwd)
     main(shlex.split(f'--logfire-url=http://localhost:0 whoami --data-dir {tmp_dir_cwd}'))
-    # insert_assert(capsys.readouterr().err)
-    assert capsys.readouterr().err == (
-        'Not logged in. Run `logfire auth` to log in.\n'
-        f'Credentials loaded from data dir: {tmp_dir_cwd}\n'
-        '\n'
-        'Logfire project URL: https://dashboard.logfire.dev\n'
+    assert capsys.readouterr().err.splitlines() == snapshot(
+        [
+            'Not logged in. Run `logfire auth` to log in.',
+            IsStr(regex=rf'^Credentials loaded from data dir: {tmp_dir_cwd}'),
+            '',
+            'Logfire project URL: https://dashboard.logfire.dev',
+        ]
     )
 
 
 def test_whoami_without_data(tmp_dir_cwd: Path, capsys: pytest.CaptureFixture[str]) -> None:
     # Change to the temp dir so the test doesn't fail if executed from a folder containing logfire credentials.
     current_dir = os.getcwd()
     os.chdir(tmp_dir_cwd)
     try:
         main(['--logfire-url=http://localhost:0', 'whoami'])
     except SystemExit as e:
         assert e.code == 1
-        # insert_assert(capsys.readouterr().err)
-        assert capsys.readouterr().err == (
-            'Not logged in. Run `logfire auth` to log in.\n' f'No Logfire credentials found in {tmp_dir_cwd}/.logfire\n'
+        assert capsys.readouterr().err.splitlines() == snapshot(
+            [
+                'Not logged in. Run `logfire auth` to log in.',
+                IsStr(regex=r'No Logfire credentials found in .*/\.logfire'),
+            ]
         )
     finally:
         os.chdir(current_dir)
 
 
 def test_whoami_logged_in(
     tmp_dir_cwd: Path, logfire_credentials: LogfireCredentials, capsys: pytest.CaptureFixture[str]
@@ -87,34 +90,36 @@
 
         m = requests_mock.Mocker()
         stack.enter_context(m)
 
         m.get('http://localhost/v1/account/me', json={'name': 'test-user'})
 
         main(shlex.split(f'--logfire-url=http://localhost:0 whoami --data-dir {tmp_dir_cwd}'))
-    # insert_assert(capsys.readouterr().err)
-    assert capsys.readouterr().err == (
-        'Logged in as: test-user\n'
-        f'Credentials loaded from data dir: {tmp_dir_cwd}\n'
-        '\n'
-        'Logfire project URL: https://dashboard.logfire.dev\n'
+    assert capsys.readouterr().err.splitlines() == snapshot(
+        [
+            'Logged in as: test-user',
+            IsStr(regex=rf'^Credentials loaded from data dir: {tmp_dir_cwd}'),
+            '',
+            'Logfire project URL: https://dashboard.logfire.dev',
+        ]
     )
 
 
 def test_whoami_default_dir(
     tmp_dir_cwd: Path, logfire_credentials: LogfireCredentials, capsys: pytest.CaptureFixture[str]
 ) -> None:
     logfire_credentials.write_creds_file(tmp_dir_cwd / '.logfire')
     main(['--logfire-url=http://localhost:0', 'whoami'])
-    # insert_assert(capsys.readouterr().err)
-    assert capsys.readouterr().err == (
-        'Not logged in. Run `logfire auth` to log in.\n'
-        f'Credentials loaded from data dir: {tmp_dir_cwd}/.logfire\n'
-        '\n'
-        'Logfire project URL: https://dashboard.logfire.dev\n'
+    assert capsys.readouterr().err.splitlines() == snapshot(
+        [
+            'Not logged in. Run `logfire auth` to log in.',
+            IsStr(regex=r'^Credentials loaded from data dir: .*/\.logfire$'),
+            '',
+            'Logfire project URL: https://dashboard.logfire.dev',
+        ]
     )
 
 
 @pytest.mark.parametrize(
     'confirm,output',
     [
         ('y', 'Cleaned Logfire data.\n'),
@@ -210,28 +215,29 @@
 [tokens."https://logfire-api.pydantic.dev"]
 token = "fake_token"
 expiration = "fake_exp"
 """
         )
 
         console_calls = [re.sub(r'^call(\(\).)?', '', str(call)) for call in console.mock_calls]
-        # insert_assert(console_calls)
-        assert console_calls == [
-            IsStr(regex=r'^\(file=.*'),
-            'print()',
-            "print('Welcome to Logfire! :fire:')",
-            "print('Before you can send data to Logfire, we need to authenticate you.')",
-            'print()',
-            "input('Press [bold]Enter[/] to open example.com in your browser...')",
-            'print("Please open [bold]http://example.com/auth[/] in your browser to authenticate if it hasn\'t already.")',
-            "print('Waiting for you to authenticate with Logfire...')",
-            "print('Successfully authenticated!')",
-            'print()',
-            f"print('Your Logfire credentials are stored in [bold]{auth_file}[/]')",
-        ]
+        assert console_calls == snapshot(
+            [
+                IsStr(regex=r'^\(file=.*'),
+                'print()',
+                "print('Welcome to Logfire! :fire:')",
+                "print('Before you can send data to Logfire, we need to authenticate you.')",
+                'print()',
+                "input('Press [bold]Enter[/] to open example.com in your browser...')",
+                'print("Please open [bold]http://example.com/auth[/] in your browser to authenticate if it hasn\'t already.")',
+                "print('Waiting for you to authenticate with Logfire...')",
+                "print('Successfully authenticated!')",
+                'print()',
+                IsStr(regex=r"^print\('Your Logfire credentials are stored in \[bold\].*/default.toml\[/\]'\)"),
+            ]
+        )
 
         webbrowser_open.assert_called_once_with('http://example.com/auth', new=2)
 
 
 def test_auth_temp_failure(tmp_path: Path) -> None:
     auth_file = tmp_path / 'default.toml'
     with ExitStack() as stack:
```

### Comparing `logfire-0.30.0/tests/test_collect_package_resources.py` & `logfire-0.31.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/test_configure.py` & `logfire-0.31.0/tests/test_configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import dataclasses
 import json
 import os
+import sys
 from contextlib import ExitStack
 from pathlib import Path
 from typing import Any, Sequence
 from unittest import mock
 from unittest.mock import call, patch
 
 import pytest
 import requests_mock
+from inline_snapshot import snapshot
 from opentelemetry.sdk.metrics.export import InMemoryMetricReader
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor, SpanExporter, SpanExportResult
 from pytest import LogCaptureFixture
 
 import logfire
 from logfire import configure
@@ -53,361 +55,362 @@
     for lf in (logfire, tags1, tags2):
         with lf.span('root'):
             with lf.span('child'):
                 logfire.info('test1')
                 tags1.info('test2')
                 tags2.info('test3')
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'root (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'root',
-                'logfire.msg': 'root',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
-            },
-        },
-        {
-            'name': 'child (pending)',
-            'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'child',
-                'logfire.msg': 'child',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000001',
-            },
-        },
-        {
-            'name': 'test1',
-            'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 3000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test1',
-                'logfire.msg': 'test1',
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-            },
-        },
-        {
-            'name': 'test2',
-            'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 4000000000,
-            'end_time': 4000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test2',
-                'logfire.msg': 'test2',
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.tags': ('tag1', 'tag2'),
-            },
-        },
-        {
-            'name': 'test3',
-            'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 5000000000,
-            'end_time': 5000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test3',
-                'logfire.msg': 'test3',
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.tags': ('tag3', 'tag4'),
-            },
-        },
-        {
-            'name': 'child',
-            'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 6000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'child',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'child',
-            },
-        },
-        {
-            'name': 'root',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 7000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'root',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'root',
-            },
-        },
-        {
-            'name': 'root (pending)',
-            'context': {'trace_id': 2, 'span_id': 9, 'is_remote': False},
-            'parent': {'trace_id': 2, 'span_id': 8, 'is_remote': False},
-            'start_time': 8000000000,
-            'end_time': 8000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'root',
-                'logfire.msg': 'root',
-                'logfire.tags': ('tag1', 'tag2'),
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
-            },
-        },
-        {
-            'name': 'child (pending)',
-            'context': {'trace_id': 2, 'span_id': 11, 'is_remote': False},
-            'parent': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
-            'start_time': 9000000000,
-            'end_time': 9000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'child',
-                'logfire.msg': 'child',
-                'logfire.tags': ('tag1', 'tag2'),
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000008',
-            },
-        },
-        {
-            'name': 'test1',
-            'context': {'trace_id': 2, 'span_id': 12, 'is_remote': False},
-            'parent': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
-            'start_time': 10000000000,
-            'end_time': 10000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test1',
-                'logfire.msg': 'test1',
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-            },
-        },
-        {
-            'name': 'test2',
-            'context': {'trace_id': 2, 'span_id': 13, 'is_remote': False},
-            'parent': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
-            'start_time': 11000000000,
-            'end_time': 11000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test2',
-                'logfire.msg': 'test2',
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.tags': ('tag1', 'tag2'),
-            },
-        },
-        {
-            'name': 'test3',
-            'context': {'trace_id': 2, 'span_id': 14, 'is_remote': False},
-            'parent': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
-            'start_time': 12000000000,
-            'end_time': 12000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test3',
-                'logfire.msg': 'test3',
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.tags': ('tag3', 'tag4'),
-            },
-        },
-        {
-            'name': 'child',
-            'context': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
-            'parent': {'trace_id': 2, 'span_id': 8, 'is_remote': False},
-            'start_time': 9000000000,
-            'end_time': 13000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'child',
-                'logfire.tags': ('tag1', 'tag2'),
-                'logfire.span_type': 'span',
-                'logfire.msg': 'child',
-            },
-        },
-        {
-            'name': 'root',
-            'context': {'trace_id': 2, 'span_id': 8, 'is_remote': False},
-            'parent': None,
-            'start_time': 8000000000,
-            'end_time': 14000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'root',
-                'logfire.tags': ('tag1', 'tag2'),
-                'logfire.span_type': 'span',
-                'logfire.msg': 'root',
-            },
-        },
-        {
-            'name': 'root (pending)',
-            'context': {'trace_id': 3, 'span_id': 16, 'is_remote': False},
-            'parent': {'trace_id': 3, 'span_id': 15, 'is_remote': False},
-            'start_time': 15000000000,
-            'end_time': 15000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'root',
-                'logfire.msg': 'root',
-                'logfire.tags': ('tag3', 'tag4'),
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
-            },
-        },
-        {
-            'name': 'child (pending)',
-            'context': {'trace_id': 3, 'span_id': 18, 'is_remote': False},
-            'parent': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
-            'start_time': 16000000000,
-            'end_time': 16000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'child',
-                'logfire.msg': 'child',
-                'logfire.tags': ('tag3', 'tag4'),
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '000000000000000f',
-            },
-        },
-        {
-            'name': 'test1',
-            'context': {'trace_id': 3, 'span_id': 19, 'is_remote': False},
-            'parent': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
-            'start_time': 17000000000,
-            'end_time': 17000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test1',
-                'logfire.msg': 'test1',
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-            },
-        },
-        {
-            'name': 'test2',
-            'context': {'trace_id': 3, 'span_id': 20, 'is_remote': False},
-            'parent': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
-            'start_time': 18000000000,
-            'end_time': 18000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test2',
-                'logfire.msg': 'test2',
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.tags': ('tag1', 'tag2'),
-            },
-        },
-        {
-            'name': 'test3',
-            'context': {'trace_id': 3, 'span_id': 21, 'is_remote': False},
-            'parent': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
-            'start_time': 19000000000,
-            'end_time': 19000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test3',
-                'logfire.msg': 'test3',
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.tags': ('tag3', 'tag4'),
-            },
-        },
-        {
-            'name': 'child',
-            'context': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
-            'parent': {'trace_id': 3, 'span_id': 15, 'is_remote': False},
-            'start_time': 16000000000,
-            'end_time': 20000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'child',
-                'logfire.tags': ('tag3', 'tag4'),
-                'logfire.span_type': 'span',
-                'logfire.msg': 'child',
-            },
-        },
-        {
-            'name': 'root',
-            'context': {'trace_id': 3, 'span_id': 15, 'is_remote': False},
-            'parent': None,
-            'start_time': 15000000000,
-            'end_time': 21000000000,
-            'attributes': {
-                'code.filepath': 'test_configure.py',
-                'code.lineno': 123,
-                'code.function': 'test_propagate_config_to_tags',
-                'logfire.msg_template': 'root',
-                'logfire.tags': ('tag3', 'tag4'),
-                'logfire.span_type': 'span',
-                'logfire.msg': 'root',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'root (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'root',
+                    'logfire.msg': 'root',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
+            },
+            {
+                'name': 'child (pending)',
+                'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'child',
+                    'logfire.msg': 'child',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000001',
+                },
+            },
+            {
+                'name': 'test1',
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 3000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test1',
+                    'logfire.msg': 'test1',
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                },
+            },
+            {
+                'name': 'test2',
+                'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 4000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test2',
+                    'logfire.msg': 'test2',
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.tags': ('tag1', 'tag2'),
+                },
+            },
+            {
+                'name': 'test3',
+                'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 5000000000,
+                'end_time': 5000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test3',
+                    'logfire.msg': 'test3',
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.tags': ('tag3', 'tag4'),
+                },
+            },
+            {
+                'name': 'child',
+                'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 6000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'child',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'child',
+                },
+            },
+            {
+                'name': 'root',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 7000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'root',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'root',
+                },
+            },
+            {
+                'name': 'root (pending)',
+                'context': {'trace_id': 2, 'span_id': 9, 'is_remote': False},
+                'parent': {'trace_id': 2, 'span_id': 8, 'is_remote': False},
+                'start_time': 8000000000,
+                'end_time': 8000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'root',
+                    'logfire.msg': 'root',
+                    'logfire.tags': ('tag1', 'tag2'),
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
+            },
+            {
+                'name': 'child (pending)',
+                'context': {'trace_id': 2, 'span_id': 11, 'is_remote': False},
+                'parent': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
+                'start_time': 9000000000,
+                'end_time': 9000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'child',
+                    'logfire.msg': 'child',
+                    'logfire.tags': ('tag1', 'tag2'),
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000008',
+                },
+            },
+            {
+                'name': 'test1',
+                'context': {'trace_id': 2, 'span_id': 12, 'is_remote': False},
+                'parent': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
+                'start_time': 10000000000,
+                'end_time': 10000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test1',
+                    'logfire.msg': 'test1',
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                },
+            },
+            {
+                'name': 'test2',
+                'context': {'trace_id': 2, 'span_id': 13, 'is_remote': False},
+                'parent': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
+                'start_time': 11000000000,
+                'end_time': 11000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test2',
+                    'logfire.msg': 'test2',
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.tags': ('tag1', 'tag2'),
+                },
+            },
+            {
+                'name': 'test3',
+                'context': {'trace_id': 2, 'span_id': 14, 'is_remote': False},
+                'parent': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
+                'start_time': 12000000000,
+                'end_time': 12000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test3',
+                    'logfire.msg': 'test3',
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.tags': ('tag3', 'tag4'),
+                },
+            },
+            {
+                'name': 'child',
+                'context': {'trace_id': 2, 'span_id': 10, 'is_remote': False},
+                'parent': {'trace_id': 2, 'span_id': 8, 'is_remote': False},
+                'start_time': 9000000000,
+                'end_time': 13000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'child',
+                    'logfire.tags': ('tag1', 'tag2'),
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'child',
+                },
+            },
+            {
+                'name': 'root',
+                'context': {'trace_id': 2, 'span_id': 8, 'is_remote': False},
+                'parent': None,
+                'start_time': 8000000000,
+                'end_time': 14000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'root',
+                    'logfire.tags': ('tag1', 'tag2'),
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'root',
+                },
+            },
+            {
+                'name': 'root (pending)',
+                'context': {'trace_id': 3, 'span_id': 16, 'is_remote': False},
+                'parent': {'trace_id': 3, 'span_id': 15, 'is_remote': False},
+                'start_time': 15000000000,
+                'end_time': 15000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'root',
+                    'logfire.msg': 'root',
+                    'logfire.tags': ('tag3', 'tag4'),
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
+            },
+            {
+                'name': 'child (pending)',
+                'context': {'trace_id': 3, 'span_id': 18, 'is_remote': False},
+                'parent': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
+                'start_time': 16000000000,
+                'end_time': 16000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'child',
+                    'logfire.msg': 'child',
+                    'logfire.tags': ('tag3', 'tag4'),
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '000000000000000f',
+                },
+            },
+            {
+                'name': 'test1',
+                'context': {'trace_id': 3, 'span_id': 19, 'is_remote': False},
+                'parent': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
+                'start_time': 17000000000,
+                'end_time': 17000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test1',
+                    'logfire.msg': 'test1',
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                },
+            },
+            {
+                'name': 'test2',
+                'context': {'trace_id': 3, 'span_id': 20, 'is_remote': False},
+                'parent': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
+                'start_time': 18000000000,
+                'end_time': 18000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test2',
+                    'logfire.msg': 'test2',
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.tags': ('tag1', 'tag2'),
+                },
+            },
+            {
+                'name': 'test3',
+                'context': {'trace_id': 3, 'span_id': 21, 'is_remote': False},
+                'parent': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
+                'start_time': 19000000000,
+                'end_time': 19000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test3',
+                    'logfire.msg': 'test3',
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.tags': ('tag3', 'tag4'),
+                },
+            },
+            {
+                'name': 'child',
+                'context': {'trace_id': 3, 'span_id': 17, 'is_remote': False},
+                'parent': {'trace_id': 3, 'span_id': 15, 'is_remote': False},
+                'start_time': 16000000000,
+                'end_time': 20000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'child',
+                    'logfire.tags': ('tag3', 'tag4'),
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'child',
+                },
+            },
+            {
+                'name': 'root',
+                'context': {'trace_id': 3, 'span_id': 15, 'is_remote': False},
+                'parent': None,
+                'start_time': 15000000000,
+                'end_time': 21000000000,
+                'attributes': {
+                    'code.filepath': 'test_configure.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_propagate_config_to_tags',
+                    'logfire.msg_template': 'root',
+                    'logfire.tags': ('tag3', 'tag4'),
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'root',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_read_config_from_environment_variables() -> None:
     assert LogfireConfig().pydantic_plugin.record == 'off'
 
     with patch.dict(os.environ, {'LOGFIRE_PYDANTIC_PLUGIN_RECORD': 'all'}):
         assert LogfireConfig().pydantic_plugin.record == 'all'
@@ -524,14 +527,15 @@
         fallback_exporter.exporter = FailureExporter()
 
         return SimpleSpanProcessor(exporter)
 
     with request_mocker:
         data_dir = Path(tmp_path) / 'logfire_data'
         logfire.configure(
+            send_to_logfire=True,
             data_dir=data_dir,
             token='abc',
             default_span_processor=default_span_processor,
             metric_readers=[InMemoryMetricReader()],
         )
 
     assert not data_dir.exists()
@@ -597,44 +601,45 @@
             id_generator=IncrementalIdGenerator(),
             processors=[SimpleSpanProcessor(exporter)],
             metric_readers=[InMemoryMetricReader()],
         )
 
     logfire.info('test1')
 
-    # insert_assert(exporter.exported_spans_as_dict(include_resources=True))
-    assert exporter.exported_spans_as_dict(include_resources=True) == [
-        {
-            'name': 'test1',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test1',
-                'logfire.msg': 'test1',
-                'code.filepath': 'test_configure.py',
-                'code.function': 'test_otel_service_name_env_var',
-                'code.lineno': 123,
-            },
-            'resource': {
-                'attributes': {
-                    'telemetry.sdk.language': 'python',
-                    'telemetry.sdk.name': 'opentelemetry',
-                    'telemetry.sdk.version': '0.0.0',
-                    'service.name': 'potato',
-                    'service.version': '1.2.3',
-                    'service.instance.id': '00000000000000000000000000000000',
-                    'process.pid': 1234,
-                }
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(include_resources=True) == snapshot(
+        [
+            {
+                'name': 'test1',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test1',
+                    'logfire.msg': 'test1',
+                    'code.filepath': 'test_configure.py',
+                    'code.function': 'test_otel_service_name_env_var',
+                    'code.lineno': 123,
+                },
+                'resource': {
+                    'attributes': {
+                        'telemetry.sdk.language': 'python',
+                        'telemetry.sdk.name': 'opentelemetry',
+                        'telemetry.sdk.version': '0.0.0',
+                        'service.name': 'potato',
+                        'service.version': '1.2.3',
+                        'service.instance.id': '00000000000000000000000000000000',
+                        'process.pid': 1234,
+                    }
+                },
+            }
+        ]
+    )
 
 
 def test_otel_otel_resource_attributes_env_var() -> None:
     time_generator = TimeGenerator()
     exporter = TestExporter()
 
     with patch.dict(
@@ -648,44 +653,45 @@
             id_generator=IncrementalIdGenerator(),
             processors=[SimpleSpanProcessor(exporter)],
             metric_readers=[InMemoryMetricReader()],
         )
 
     logfire.info('test1')
 
-    # insert_assert(exporter.exported_spans_as_dict(include_resources=True))
-    assert exporter.exported_spans_as_dict(include_resources=True) == [
-        {
-            'name': 'test1',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test1',
-                'logfire.msg': 'test1',
-                'code.filepath': 'test_configure.py',
-                'code.function': 'test_otel_otel_resource_attributes_env_var',
-                'code.lineno': 123,
-            },
-            'resource': {
-                'attributes': {
-                    'telemetry.sdk.language': 'python',
-                    'telemetry.sdk.name': 'opentelemetry',
-                    'telemetry.sdk.version': '0.0.0',
-                    'service.name': 'banana',
-                    'service.version': '1.2.3',
-                    'service.instance.id': 'instance_id',
-                    'process.pid': 1234,
-                }
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(include_resources=True) == snapshot(
+        [
+            {
+                'name': 'test1',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test1',
+                    'logfire.msg': 'test1',
+                    'code.filepath': 'test_configure.py',
+                    'code.function': 'test_otel_otel_resource_attributes_env_var',
+                    'code.lineno': 123,
+                },
+                'resource': {
+                    'attributes': {
+                        'telemetry.sdk.language': 'python',
+                        'telemetry.sdk.name': 'opentelemetry',
+                        'telemetry.sdk.version': '0.0.0',
+                        'service.name': 'banana',
+                        'service.version': '1.2.3',
+                        'service.instance.id': 'instance_id',
+                        'process.pid': 1234,
+                    }
+                },
+            }
+        ]
+    )
 
 
 def test_otel_service_name_has_priority_on_otel_resource_attributes_service_name_env_var() -> None:
     time_generator = TimeGenerator()
     exporter = TestExporter()
 
     with patch.dict(
@@ -699,44 +705,45 @@
             id_generator=IncrementalIdGenerator(),
             processors=[SimpleSpanProcessor(exporter)],
             metric_readers=[InMemoryMetricReader()],
         )
 
     logfire.info('test1')
 
-    # insert_assert(exporter.exported_spans_as_dict(include_resources=True))
-    assert exporter.exported_spans_as_dict(include_resources=True) == [
-        {
-            'name': 'test1',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test1',
-                'logfire.msg': 'test1',
-                'code.filepath': 'test_configure.py',
-                'code.function': 'test_otel_service_name_has_priority_on_otel_resource_attributes_service_name_env_var',
-                'code.lineno': 123,
-            },
-            'resource': {
-                'attributes': {
-                    'telemetry.sdk.language': 'python',
-                    'telemetry.sdk.name': 'opentelemetry',
-                    'telemetry.sdk.version': '0.0.0',
-                    'service.name': 'banana',
-                    'service.version': '1.2.3',
-                    'service.instance.id': '00000000000000000000000000000000',
-                    'process.pid': 1234,
-                }
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(include_resources=True) == snapshot(
+        [
+            {
+                'name': 'test1',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test1',
+                    'logfire.msg': 'test1',
+                    'code.filepath': 'test_configure.py',
+                    'code.function': 'test_otel_service_name_has_priority_on_otel_resource_attributes_service_name_env_var',
+                    'code.lineno': 123,
+                },
+                'resource': {
+                    'attributes': {
+                        'telemetry.sdk.language': 'python',
+                        'telemetry.sdk.name': 'opentelemetry',
+                        'telemetry.sdk.version': '0.0.0',
+                        'service.name': 'banana',
+                        'service.version': '1.2.3',
+                        'service.instance.id': '00000000000000000000000000000000',
+                        'process.pid': 1234,
+                    }
+                },
+            }
+        ]
+    )
 
 
 def test_config_serializable():
     """
     Tests that by default, the logfire config can be serialized in the way that we do when sending it to another process.
 
     Here's an example of a configuration that (as of writing) fails to serialize:
@@ -827,15 +834,15 @@
                 'project_name': 'myproject',
                 'token': 'fake_token',
                 'project_url': 'fake_project_url',
             }
         }
         request_mocker.post('https://logfire-api.pydantic.dev/v1/projects/fake_org', [create_project_response])
 
-        logfire.configure()
+        logfire.configure(send_to_logfire=True)
 
         assert confirm_mock.mock_calls == [
             call('The project will be created in the organization "fake_org". Continue?', default=True),
         ]
 
 
 def test_initialize_project_use_existing_project(tmp_dir_cwd: Path, tmp_path: Path, capsys: pytest.CaptureFixture[str]):
@@ -862,15 +869,15 @@
             }
         }
         request_mocker.post(
             'https://logfire-api.pydantic.dev/v1/organizations/fake_org/projects/fake_project/write-tokens/',
             [create_project_response],
         )
 
-        logfire.configure()
+        logfire.configure(send_to_logfire=True)
 
         assert confirm_mock.mock_calls == [
             call('Do you want to use one of your existing projects? ', default=True),
         ]
         assert prompt_mock.mock_calls == [
             call(
                 'Please select one of the following projects by number:\n1. fake_org/fake_project\n',
@@ -919,15 +926,15 @@
         }
         request_mocker.post('https://logfire-api.pydantic.dev/v1/projects/fake_org', [create_project_response])
         request_mocker.post(
             'https://logfire-api.pydantic.dev/v1/organizations/fake_org/projects/fake_project/write-tokens/',
             [create_project_response],
         )
 
-        logfire.configure()
+        logfire.configure(send_to_logfire=True)
 
         assert confirm_mock.mock_calls == [
             call('Do you want to use one of your existing projects? ', default=True),
             call('The project will be created in the organization "fake_org". Continue?', default=True),
         ]
         assert prompt_mock.mock_calls == [
             call('Enter the project name', default='testinitializeprojectnotus0'),
@@ -959,15 +966,15 @@
         )
         request_mocker.get(
             'https://logfire-api.pydantic.dev/v1/projects/',
             json=[{'organization_name': 'fake_org', 'project_name': 'fake_project'}],
         )
 
         with pytest.raises(SystemExit):
-            logfire.configure(data_dir=tmp_path)
+            logfire.configure(data_dir=tmp_path, send_to_logfire=True)
 
         assert confirm_mock.mock_calls == [
             call('Do you want to use one of your existing projects? ', default=True),
             call('The project will be created in the organization "fake_org". Continue?', default=True),
         ]
 
 
@@ -1036,15 +1043,15 @@
             [
                 create_existing_project_response,
                 create_reserved_project_response,
                 create_project_response,
             ],
         )
 
-        logfire.configure()
+        logfire.configure(send_to_logfire=True)
 
         for request in request_mocker.request_history:
             assert request.headers['Authorization'] == 'fake_user_token'
 
         assert request_mocker.request_history[2].json() == create_existing_project_request_json
         assert request_mocker.request_history[3].json() == create_reserved_project_request_json
         assert request_mocker.request_history[4].json() == create_project_request_json
@@ -1119,15 +1126,15 @@
             }
         }
         request_mocker.post(
             'https://logfire-api.pydantic.dev/v1/projects/fake_org',
             [create_project_response],
         )
 
-        logfire.configure()
+        logfire.configure(send_to_logfire=True)
 
         assert prompt_mock.mock_calls == [
             call(
                 '\nTo create and use a new project, please provide the following information:\nSelect the organization to create the project in',
                 choices=['fake_org', 'fake_org1'],
                 default='fake_org1',
             ),
@@ -1269,7 +1276,25 @@
         ):
             LogfireConfig()._initialize_credentials_from_token('some-token')  # type: ignore
 
 
 def test_configure_twice_no_warning(caplog: LogCaptureFixture):
     logfire.configure(send_to_logfire=False)
     assert not caplog.messages
+
+
+def test_send_to_logfire_under_pytest():
+    """
+    Test that the `send_to_logfire` parameter is set to False when running under pytest.
+    """
+    assert 'PYTEST_CURRENT_TEST' in os.environ
+    logfire.configure()
+    assert GLOBAL_CONFIG.send_to_logfire is False
+
+
+@pytest.mark.skipif(sys.version_info[:2] >= (3, 9), reason='Testing an error only raised in Python 3.8+')
+def test_configure_fstring_python_38():
+    with pytest.raises(  # pragma: no branch
+        LogfireConfigError,
+        match=r'Inspecting arguments is only supported in Python 3.9\+ and only recommended in Python 3.11\+.',
+    ):
+        logfire.configure(send_to_logfire=False, inspect_arguments=True)
```

### Comparing `logfire-0.30.0/tests/test_console_exporter.py` & `logfire-0.31.0/tests/test_console_exporter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # pyright: reportPrivateUsage=false
 from __future__ import annotations
 
 import io
+import sys
 
 import pytest
+from dirty_equals import IsStr
 from inline_snapshot import snapshot
 from opentelemetry import trace
 from opentelemetry.sdk.trace import ReadableSpan
 
 import logfire
 from logfire import ConsoleOptions
 from logfire._internal.exporters.console import (
@@ -73,42 +75,45 @@
     ]
 
 
 def test_simple_console_exporter_no_colors_concise(simple_spans: list[ReadableSpan]) -> None:
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, verbose=False, colors='never').export(simple_spans)
 
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '00:00:01.000 rootSpan',
-        '00:00:02.000 childSpan 1',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 rootSpan',
+            '00:00:02.000 childSpan 1',
+        ]
+    )
 
 
 def test_simple_console_exporter_colors_concise(simple_spans: list[ReadableSpan]) -> None:
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, verbose=False, colors='always').export(simple_spans)
 
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '\x1b[32m00:00:01.000\x1b[0m rootSpan',
-        '\x1b[32m00:00:02.000\x1b[0m childSpan 1',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '\x1b[32m00:00:01.000\x1b[0m rootSpan',
+            '\x1b[32m00:00:02.000\x1b[0m childSpan 1',
+        ]
+    )
 
 
 def test_simple_console_exporter_no_colors_verbose(simple_spans: list[ReadableSpan]) -> None:
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, verbose=True, colors='never').export(simple_spans)
 
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '00:00:01.000 rootSpan',
-        '00:00:02.000 childSpan 1',
-        '             │ testing.py:42 ',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 rootSpan',
+            '00:00:02.000 childSpan 1',
+            '             │ testing.py:42 ',
+        ]
+    )
 
 
 def pending_span(
     msg_template: str, timestamp: int, trace_id: int, span_id: int, parent_id: int, grand_parent_id: int | None = None
 ) -> ReadableSpan:
     extra_attributes: dict[str, str] = {}
     if grand_parent_id is not None:
@@ -190,19 +195,20 @@
         [
             log_span('logSpan', 2, trace_id, log_span_id, root_span_id),
             span_span('rootSpan', 1, 3, trace_id, root_span_id),
         ]
     )
     assert exporter._indent_level == {}
 
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '00:00:01.000 rootSpan',
-        '00:00:02.000   logSpan',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 rootSpan',
+            '00:00:02.000   logSpan',
+        ]
+    )
 
 
 def test_indented_console_exporter_nested() -> None:
     trace_id = 0
     root_span_id = 1
     root_pending_span_id = 2
     nested_span_id = 3
@@ -220,21 +226,22 @@
 
     out = io.StringIO()
     exporter = IndentedConsoleSpanExporter(output=out, verbose=False, colors='never')
     assert exporter._indent_level == {}
     exporter.export(spans)
     assert exporter._indent_level == {}
 
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '00:00:01.000 rootSpan',
-        '00:00:02.000   nestedSpan',
-        '00:00:03.000     logSpan 1',
-        '00:00:05.000   logSpan 2',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 rootSpan',
+            '00:00:02.000   nestedSpan',
+            '00:00:03.000     logSpan 1',
+            '00:00:05.000   logSpan 2',
+        ]
+    )
 
 
 def test_show_parents_console_exporter() -> None:
     trace_id = 0
     root_span_id = 1
     pending_span_id = 2
     log_span_id = 3
@@ -251,19 +258,20 @@
             log_span('logSpan', 2, trace_id, log_span_id, root_span_id),
             span_span('rootSpan', 1, 3, trace_id, root_span_id),
         ]
     )
     assert exporter._span_history == {}
     assert exporter._span_stack == []
 
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '00:00:01.000 rootSpan',
-        '00:00:02.000   logSpan',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 rootSpan',
+            '00:00:02.000   logSpan',
+        ]
+    )
 
 
 def test_show_parents_console_exporter_nested() -> None:
     trace_id = 0
     root_span_id = 1
     root_pending_span_id = 2
     nested_span_id = 3
@@ -278,46 +286,43 @@
         [
             pending_span('rootSpan', 1, trace_id, root_pending_span_id, root_span_id),
             pending_span('nestedSpan', 2, trace_id, nested_pending_span_id, nested_span_id, root_span_id),
             log_span('logSpan 1', 3, trace_id, log_1_span_id, nested_span_id),
         ]
     )
 
-    # insert_assert(exporter._span_history)
-    assert exporter._span_history == {1: (0, 'rootSpan', 0), 3: (1, 'nestedSpan', 1)}
-    # insert_assert(exporter._span_stack)
-    assert exporter._span_stack == [1, 3]
+    assert exporter._span_history == snapshot({1: (0, 'rootSpan', 0), 3: (1, 'nestedSpan', 1)})
+    assert exporter._span_stack == snapshot([1, 3])
 
     exporter.export(
         [
             span_span('nestedSpan', 2, 4, trace_id, nested_span_id, root_span_id),
         ]
     )
 
-    # insert_assert(exporter._span_history)
-    assert exporter._span_history == {1: (0, 'rootSpan', 0)}
-    # insert_assert(exporter._span_stack)
-    assert exporter._span_stack == [1]
+    assert exporter._span_history == snapshot({1: (0, 'rootSpan', 0)})
+    assert exporter._span_stack == snapshot([1])
 
     exporter.export(
         [
             log_span('logSpan 2', 5, trace_id, log_2_span_id, root_span_id),
             span_span('rootSpan', 1, 5, trace_id, root_span_id),
         ]
     )
     assert exporter._span_history == {}
     assert exporter._span_stack == []
 
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '00:00:01.000 rootSpan',
-        '00:00:02.000   nestedSpan',
-        '00:00:03.000     logSpan 1',
-        '00:00:05.000   logSpan 2',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 rootSpan',
+            '00:00:02.000   nestedSpan',
+            '00:00:03.000     logSpan 1',
+            '00:00:05.000   logSpan 2',
+        ]
+    )
 
 
 def test_show_parents_console_exporter_interleaved() -> None:
     a_trace_id = 0
     a_span_id = 1
     a_pending_span_id = 2
     a_log_id = 3
@@ -339,53 +344,55 @@
             span_span('span b', 1, 6, b_trace_id, b_span_id),
         ]
     )
 
     assert exporter._span_history == {}
     assert exporter._span_stack == []
 
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '00:00:01.000 span a',
-        '00:00:02.000 span b',
-        '             span a',
-        '00:00:03.000   log a',
-        '             span b',
-        '00:00:04.000   log b',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 span a',
+            '00:00:02.000 span b',
+            '             span a',
+            '00:00:03.000   log a',
+            '             span b',
+            '00:00:04.000   log b',
+        ]
+    )
 
 
 def test_verbose_attributes(exporter: TestExporter) -> None:
     d = {'a': 1, 'b': 2}
     logfire.info('Hello {name}!', name='world', d=d)
     spans = exported_spans_as_models(exporter)
-    # insert_assert(spans)
-    assert spans == [
-        ReadableSpanModel(
-            name='Hello {name}!',
-            context=SpanContextModel(trace_id=1, span_id=1, is_remote=False),
-            parent=None,
-            start_time=1000000000,
-            end_time=1000000000,
-            attributes={
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'Hello {name}!',
-                'logfire.msg': 'Hello world!',
-                'code.lineno': 123,
-                'code.filepath': 'test_console_exporter.py',
-                'code.function': 'test_verbose_attributes',
-                'name': 'world',
-                'd': '{"a":1,"b":2}',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"d":{"type":"object"}}}',
-            },
-            events=None,
-            resource=None,
-        )
-    ]
+    assert spans == snapshot(
+        [
+            ReadableSpanModel(
+                name='Hello {name}!',
+                context=SpanContextModel(trace_id=1, span_id=1, is_remote=False),
+                parent=None,
+                start_time=1000000000,
+                end_time=1000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'Hello {name}!',
+                    'logfire.msg': 'Hello world!',
+                    'code.lineno': 123,
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_verbose_attributes',
+                    'name': 'world',
+                    'd': '{"a":1,"b":2}',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"d":{"type":"object"}}}',
+                },
+                events=None,
+                resource=None,
+            )
+        ]
+    )
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, verbose=True, colors='never').export(spans)  # type: ignore
     lines = [line.rstrip(' ') for line in out.getvalue().splitlines()]
     assert lines == [
         '00:00:01.000 Hello world!',
         '             │ test_console_exporter.py:123 info',
         "             │ name='world'",
@@ -406,247 +413,251 @@
         "│       'a': 1,",
         "│       'b': 2,",
         '│   }',
     ]
 
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, verbose=True, colors='always').export(spans)  # type: ignore
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '\x1b[32m00:00:01.000\x1b[0m Hello world!',
-        '             \x1b[34m│\x1b[0m \x1b[36mtest_console_exporter.py:123\x1b[0m info',
-        "             \x1b[34m│ \x1b[0m\x1b[34mname=\x1b[0m\x1b[93;49m'\x1b[0m\x1b[93;49mworld\x1b[0m\x1b[93;49m'\x1b[0m",
-        '             \x1b[34m│ \x1b[0m\x1b[34md=\x1b[0m\x1b[97;49m{\x1b[0m          ',
-        "             \x1b[34m│ \x1b[0m  \x1b[97;49m    \x1b[0m\x1b[93;49m'\x1b[0m\x1b[93;49ma\x1b[0m\x1b[93;49m'\x1b[0m\x1b[97;49m:\x1b[0m\x1b[97;49m \x1b[0m\x1b[37;49m1\x1b[0m\x1b[97;49m,\x1b[0m",
-        "             \x1b[34m│ \x1b[0m  \x1b[97;49m    \x1b[0m\x1b[93;49m'\x1b[0m\x1b[93;49mb\x1b[0m\x1b[93;49m'\x1b[0m\x1b[97;49m:\x1b[0m\x1b[97;49m \x1b[0m\x1b[37;49m2\x1b[0m\x1b[97;49m,\x1b[0m",
-        '             \x1b[34m│ \x1b[0m  \x1b[97;49m}\x1b[0m          ',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '\x1b[32m00:00:01.000\x1b[0m Hello world!',
+            '             \x1b[34m│\x1b[0m \x1b[36mtest_console_exporter.py:123\x1b[0m info',
+            "             \x1b[34m│ \x1b[0m\x1b[34mname=\x1b[0m\x1b[93;49m'\x1b[0m\x1b[93;49mworld\x1b[0m\x1b[93;49m'\x1b[0m",
+            '             \x1b[34m│ \x1b[0m\x1b[34md=\x1b[0m\x1b[97;49m{\x1b[0m          ',
+            "             \x1b[34m│ \x1b[0m  \x1b[97;49m    \x1b[0m\x1b[93;49m'\x1b[0m\x1b[93;49ma\x1b[0m\x1b[93;49m'\x1b[0m\x1b[97;49m:\x1b[0m\x1b[97;49m \x1b[0m\x1b[37;49m1\x1b[0m\x1b[97;49m,\x1b[0m",
+            "             \x1b[34m│ \x1b[0m  \x1b[97;49m    \x1b[0m\x1b[93;49m'\x1b[0m\x1b[93;49mb\x1b[0m\x1b[93;49m'\x1b[0m\x1b[97;49m:\x1b[0m\x1b[97;49m \x1b[0m\x1b[37;49m2\x1b[0m\x1b[97;49m,\x1b[0m",
+            '             \x1b[34m│ \x1b[0m  \x1b[97;49m}\x1b[0m          ',
+        ]
+    )
 
 
 def test_tags(exporter: TestExporter):
     logfire.with_tags('tag1', 'tag2').info('Hello')
     spans = exported_spans_as_models(exporter)
-    # insert_assert(spans)
-    assert spans == [
-        ReadableSpanModel(
-            name='Hello',
-            context=SpanContextModel(trace_id=1, span_id=1, is_remote=False),
-            parent=None,
-            start_time=1000000000,
-            end_time=1000000000,
-            attributes={
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'Hello',
-                'logfire.msg': 'Hello',
-                'code.lineno': 123,
-                'code.filepath': 'test_console_exporter.py',
-                'code.function': 'test_tags',
-                'logfire.tags': ('tag1', 'tag2'),
-            },
-            events=None,
-            resource=None,
-        )
-    ]
+    assert spans == snapshot(
+        [
+            ReadableSpanModel(
+                name='Hello',
+                context=SpanContextModel(trace_id=1, span_id=1, is_remote=False),
+                parent=None,
+                start_time=1000000000,
+                end_time=1000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'Hello',
+                    'logfire.msg': 'Hello',
+                    'code.lineno': 123,
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_tags',
+                    'logfire.tags': ('tag1', 'tag2'),
+                },
+                events=None,
+                resource=None,
+            )
+        ]
+    )
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, colors='never').export(spans)  # type: ignore
-    # insert_assert(out.getvalue())
-    assert out.getvalue() == '00:00:01.000 Hello [tag1,tag2]\n'
+    assert out.getvalue() == snapshot('00:00:01.000 Hello [tag1,tag2]\n')
 
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, colors='always').export(spans)  # type: ignore
-    # insert_assert(out.getvalue())
-    assert out.getvalue() == '\x1b[32m00:00:01.000\x1b[0m Hello \x1b[36m[tag1,tag2]\x1b[0m\n'
+    assert out.getvalue() == snapshot('\x1b[32m00:00:01.000\x1b[0m Hello \x1b[36m[tag1,tag2]\x1b[0m\n')
 
 
 def test_levels(exporter: TestExporter):
     logfire.trace('trace message')
     logfire.debug('debug message')
     logfire.info('info message')
     logfire.notice('notice message')
     logfire.warn('warn message')
     logfire.error('error message')
     logfire.fatal('fatal message')
 
     spans = exported_spans_as_models(exporter)
-    # insert_assert(spans)
-    assert spans == [
-        ReadableSpanModel(
-            name='trace message',
-            context=SpanContextModel(trace_id=1, span_id=1, is_remote=False),
-            parent=None,
-            start_time=1000000000,
-            end_time=1000000000,
-            attributes={
-                'logfire.span_type': 'log',
-                'logfire.level_num': 1,
-                'logfire.msg_template': 'trace message',
-                'logfire.msg': 'trace message',
-                'code.lineno': 123,
-                'code.filepath': 'test_console_exporter.py',
-                'code.function': 'test_levels',
-            },
-            events=None,
-            resource=None,
-        ),
-        ReadableSpanModel(
-            name='debug message',
-            context=SpanContextModel(trace_id=2, span_id=2, is_remote=False),
-            parent=None,
-            start_time=2000000000,
-            end_time=2000000000,
-            attributes={
-                'logfire.span_type': 'log',
-                'logfire.level_num': 5,
-                'logfire.msg_template': 'debug message',
-                'logfire.msg': 'debug message',
-                'code.lineno': 123,
-                'code.filepath': 'test_console_exporter.py',
-                'code.function': 'test_levels',
-            },
-            events=None,
-            resource=None,
-        ),
-        ReadableSpanModel(
-            name='info message',
-            context=SpanContextModel(trace_id=3, span_id=3, is_remote=False),
-            parent=None,
-            start_time=3000000000,
-            end_time=3000000000,
-            attributes={
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'info message',
-                'logfire.msg': 'info message',
-                'code.lineno': 123,
-                'code.filepath': 'test_console_exporter.py',
-                'code.function': 'test_levels',
-            },
-            events=None,
-            resource=None,
-        ),
-        ReadableSpanModel(
-            name='notice message',
-            context=SpanContextModel(trace_id=4, span_id=4, is_remote=False),
-            parent=None,
-            start_time=4000000000,
-            end_time=4000000000,
-            attributes={
-                'logfire.span_type': 'log',
-                'logfire.level_num': 10,
-                'logfire.msg_template': 'notice message',
-                'logfire.msg': 'notice message',
-                'code.lineno': 123,
-                'code.filepath': 'test_console_exporter.py',
-                'code.function': 'test_levels',
-            },
-            events=None,
-            resource=None,
-        ),
-        ReadableSpanModel(
-            name='warn message',
-            context=SpanContextModel(trace_id=5, span_id=5, is_remote=False),
-            parent=None,
-            start_time=5000000000,
-            end_time=5000000000,
-            attributes={
-                'logfire.span_type': 'log',
-                'logfire.level_num': 13,
-                'logfire.msg_template': 'warn message',
-                'logfire.msg': 'warn message',
-                'code.lineno': 123,
-                'code.filepath': 'test_console_exporter.py',
-                'code.function': 'test_levels',
-            },
-            events=None,
-            resource=None,
-        ),
-        ReadableSpanModel(
-            name='error message',
-            context=SpanContextModel(trace_id=6, span_id=6, is_remote=False),
-            parent=None,
-            start_time=6000000000,
-            end_time=6000000000,
-            attributes={
-                'logfire.span_type': 'log',
-                'logfire.level_num': 17,
-                'logfire.msg_template': 'error message',
-                'logfire.msg': 'error message',
-                'code.lineno': 123,
-                'code.filepath': 'test_console_exporter.py',
-                'code.function': 'test_levels',
-            },
-            events=None,
-            resource=None,
-        ),
-        ReadableSpanModel(
-            name='fatal message',
-            context=SpanContextModel(trace_id=7, span_id=7, is_remote=False),
-            parent=None,
-            start_time=7000000000,
-            end_time=7000000000,
-            attributes={
-                'logfire.span_type': 'log',
-                'logfire.level_num': 21,
-                'logfire.msg_template': 'fatal message',
-                'logfire.msg': 'fatal message',
-                'code.lineno': 123,
-                'code.filepath': 'test_console_exporter.py',
-                'code.function': 'test_levels',
-            },
-            events=None,
-            resource=None,
-        ),
-    ]
+    assert spans == snapshot(
+        [
+            ReadableSpanModel(
+                name='trace message',
+                context=SpanContextModel(trace_id=1, span_id=1, is_remote=False),
+                parent=None,
+                start_time=1000000000,
+                end_time=1000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 1,
+                    'logfire.msg_template': 'trace message',
+                    'logfire.msg': 'trace message',
+                    'code.lineno': 123,
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_levels',
+                },
+                events=None,
+                resource=None,
+            ),
+            ReadableSpanModel(
+                name='debug message',
+                context=SpanContextModel(trace_id=2, span_id=2, is_remote=False),
+                parent=None,
+                start_time=2000000000,
+                end_time=2000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 5,
+                    'logfire.msg_template': 'debug message',
+                    'logfire.msg': 'debug message',
+                    'code.lineno': 123,
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_levels',
+                },
+                events=None,
+                resource=None,
+            ),
+            ReadableSpanModel(
+                name='info message',
+                context=SpanContextModel(trace_id=3, span_id=3, is_remote=False),
+                parent=None,
+                start_time=3000000000,
+                end_time=3000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'info message',
+                    'logfire.msg': 'info message',
+                    'code.lineno': 123,
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_levels',
+                },
+                events=None,
+                resource=None,
+            ),
+            ReadableSpanModel(
+                name='notice message',
+                context=SpanContextModel(trace_id=4, span_id=4, is_remote=False),
+                parent=None,
+                start_time=4000000000,
+                end_time=4000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 10,
+                    'logfire.msg_template': 'notice message',
+                    'logfire.msg': 'notice message',
+                    'code.lineno': 123,
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_levels',
+                },
+                events=None,
+                resource=None,
+            ),
+            ReadableSpanModel(
+                name='warn message',
+                context=SpanContextModel(trace_id=5, span_id=5, is_remote=False),
+                parent=None,
+                start_time=5000000000,
+                end_time=5000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': 'warn message',
+                    'logfire.msg': 'warn message',
+                    'code.lineno': 123,
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_levels',
+                },
+                events=None,
+                resource=None,
+            ),
+            ReadableSpanModel(
+                name='error message',
+                context=SpanContextModel(trace_id=6, span_id=6, is_remote=False),
+                parent=None,
+                start_time=6000000000,
+                end_time=6000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': 'error message',
+                    'logfire.msg': 'error message',
+                    'code.lineno': 123,
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_levels',
+                },
+                events=None,
+                resource=None,
+            ),
+            ReadableSpanModel(
+                name='fatal message',
+                context=SpanContextModel(trace_id=7, span_id=7, is_remote=False),
+                parent=None,
+                start_time=7000000000,
+                end_time=7000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 21,
+                    'logfire.msg_template': 'fatal message',
+                    'logfire.msg': 'fatal message',
+                    'code.lineno': 123,
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_levels',
+                },
+                events=None,
+                resource=None,
+            ),
+        ]
+    )
 
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, colors='never', min_log_level='trace').export(spans)  # type: ignore
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '00:00:01.000 trace message',
-        '00:00:02.000 debug message',
-        '00:00:03.000 info message',
-        '00:00:04.000 notice message',
-        '00:00:05.000 warn message',
-        '00:00:06.000 error message',
-        '00:00:07.000 fatal message',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 trace message',
+            '00:00:02.000 debug message',
+            '00:00:03.000 info message',
+            '00:00:04.000 notice message',
+            '00:00:05.000 warn message',
+            '00:00:06.000 error message',
+            '00:00:07.000 fatal message',
+        ]
+    )
 
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, colors='never', verbose=True, min_log_level='trace').export(spans)  # type: ignore
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '00:00:01.000 trace message',
-        '             │ test_console_exporter.py:123 trace',
-        '00:00:02.000 debug message',
-        '             │ test_console_exporter.py:123 debug',
-        '00:00:03.000 info message',
-        '             │ test_console_exporter.py:123 info',
-        '00:00:04.000 notice message',
-        '             │ test_console_exporter.py:123 notice',
-        '00:00:05.000 warn message',
-        '             │ test_console_exporter.py:123 warn',
-        '00:00:06.000 error message',
-        '             │ test_console_exporter.py:123 error',
-        '00:00:07.000 fatal message',
-        '             │ test_console_exporter.py:123 fatal',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 trace message',
+            '             │ test_console_exporter.py:123 trace',
+            '00:00:02.000 debug message',
+            '             │ test_console_exporter.py:123 debug',
+            '00:00:03.000 info message',
+            '             │ test_console_exporter.py:123 info',
+            '00:00:04.000 notice message',
+            '             │ test_console_exporter.py:123 notice',
+            '00:00:05.000 warn message',
+            '             │ test_console_exporter.py:123 warn',
+            '00:00:06.000 error message',
+            '             │ test_console_exporter.py:123 error',
+            '00:00:07.000 fatal message',
+            '             │ test_console_exporter.py:123 fatal',
+        ]
+    )
 
     out = io.StringIO()
     SimpleConsoleSpanExporter(output=out, colors='always', min_log_level='trace').export(spans)  # type: ignore
-    # insert_assert(out.getvalue().splitlines())
-    assert out.getvalue().splitlines() == [
-        '\x1b[32m00:00:01.000\x1b[0m trace message',
-        '\x1b[32m00:00:02.000\x1b[0m debug message',
-        '\x1b[32m00:00:03.000\x1b[0m info message',
-        '\x1b[32m00:00:04.000\x1b[0m notice message',
-        '\x1b[32m00:00:05.000\x1b[0m \x1b[33mwarn message\x1b[0m',
-        '\x1b[32m00:00:06.000\x1b[0m \x1b[31merror message\x1b[0m',
-        '\x1b[32m00:00:07.000\x1b[0m \x1b[31mfatal message\x1b[0m',
-    ]
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '\x1b[32m00:00:01.000\x1b[0m trace message',
+            '\x1b[32m00:00:02.000\x1b[0m debug message',
+            '\x1b[32m00:00:03.000\x1b[0m info message',
+            '\x1b[32m00:00:04.000\x1b[0m notice message',
+            '\x1b[32m00:00:05.000\x1b[0m \x1b[33mwarn message\x1b[0m',
+            '\x1b[32m00:00:06.000\x1b[0m \x1b[31merror message\x1b[0m',
+            '\x1b[32m00:00:07.000\x1b[0m \x1b[31mfatal message\x1b[0m',
+        ]
+    )
 
     out = io.StringIO()
     # The `min_log_level` is set to 'info' by default, so only 'info' and higher levels are logged.
     SimpleConsoleSpanExporter(output=out).export(spans)  # type: ignore
     assert out.getvalue().splitlines() == snapshot(
         [
             '00:00:03.000 info message',
@@ -668,14 +679,112 @@
     )
 
     with logfire.span('outer span'):
         with logfire.span('inner span'):
             logfire.info('inner span log message')
         logfire.info('outer span log message')
 
-    # insert_assert(capsys.readouterr().out.splitlines())
-    assert capsys.readouterr().out.splitlines() == [
-        'outer span',
-        '  inner span',
-        '    inner span log message',
-        '  outer span log message',
+    assert capsys.readouterr().out.splitlines() == snapshot(
+        [
+            'outer span',
+            '  inner span',
+            '    inner span log message',
+            '  outer span log message',
+        ]
+    )
+
+
+def test_exception(exporter: TestExporter) -> None:
+    try:
+        1 / 0  # type: ignore
+    except ZeroDivisionError:
+        logfire.exception('error!!! {a}', a='test')
+
+    spans = exported_spans_as_models(exporter)
+    assert spans == snapshot(
+        [
+            ReadableSpanModel(
+                name='error!!! {a}',
+                context=SpanContextModel(trace_id=1, span_id=1, is_remote=False),
+                parent=None,
+                start_time=1000000000,
+                end_time=1000000000,
+                attributes={
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': 'error!!! {a}',
+                    'logfire.msg': 'error!!! test',
+                    'code.filepath': 'test_console_exporter.py',
+                    'code.function': 'test_exception',
+                    'code.lineno': 123,
+                    'a': 'test',
+                    'logfire.json_schema': '{"type":"object","properties":{"a":{}}}',
+                },
+                events=[
+                    {
+                        'name': 'exception',
+                        'timestamp': 2000000000,
+                        'attributes': {
+                            'exception.type': 'ZeroDivisionError',
+                            'exception.message': 'division by zero',
+                            'exception.stacktrace': 'ZeroDivisionError: division by zero',
+                            'exception.escaped': 'False',
+                        },
+                    }
+                ],
+                resource=None,
+            )
+        ]
+    )
+
+    issue_lines = (
+        ['             │     1 / 0  # type: ignore', '             │     ~~^~~']
+        if sys.version_info >= (3, 11)
+        else ['             │     1 / 0  # type: ignore']
+    )
+    out = io.StringIO()
+    SimpleConsoleSpanExporter(output=out, colors='never').export(exporter.exported_spans)
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:01.000 error!!! test',
+            '             │ ZeroDivisionError: division by zero',
+            '             │ Traceback (most recent call last):',
+            IsStr(regex=rf'             │   File "{__file__}", line \d+, in test_exception'),
+            *issue_lines,
+            '             │ ZeroDivisionError: division by zero',
+            '',
+        ]
+    )
+
+    issue_lines = (
+        [
+            '\x1b[97;49m             \x1b[0m\x1b[35;49m│\x1b[0m\x1b[97;49m     '
+            '\x1b[0m\x1b[91;49m~\x1b[0m\x1b[91;49m~\x1b[0m\x1b[91;49m^\x1b[0m\x1b[91;49m~\x1b[0m\x1b[91;49m~\x1b[0m',
+        ]
+        if sys.version_info >= (3, 11)
+        else []
+    )
+
+    out = io.StringIO()
+    SimpleConsoleSpanExporter(output=out, colors='always').export(exporter.exported_spans)
+    assert out.getvalue().splitlines() == [
+        '\x1b[32m00:00:01.000\x1b[0m \x1b[31merror!!! test\x1b[0m',
+        '\x1b[34m             │ \x1b[0m\x1b[1;31mZeroDivisionError: ' '\x1b[0mdivision by zero',
+        '\x1b[97;49m             \x1b[0m\x1b[35;49m│\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[97;49mTraceback\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[97;49m(\x1b[0m\x1b[97;49mmost\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[97;49mrecent\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[97;49mcall\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[97;49mlast\x1b[0m\x1b[97;49m)\x1b[0m\x1b[97;49m:\x1b[0m',
+        IsStr(),
+        '\x1b[97;49m             \x1b[0m\x1b[35;49m│\x1b[0m\x1b[97;49m     '
+        '\x1b[0m\x1b[37;49m1\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[91;49m/\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[37;49m0\x1b[0m\x1b[97;49m  \x1b[0m\x1b[37;49m# type: '
+        'ignore\x1b[0m',
+        *issue_lines,
+        '\x1b[97;49m             \x1b[0m\x1b[35;49m│\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[92;49mZeroDivisionError\x1b[0m\x1b[97;49m:\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[97;49mdivision\x1b[0m\x1b[97;49m '
+        '\x1b[0m\x1b[97;49mby\x1b[0m\x1b[97;49m \x1b[0m\x1b[97;49mzero\x1b[0m',
+        '',
     ]
```

### Comparing `logfire-0.30.0/tests/test_formatter.py` & `logfire-0.31.0/tests/test_formatter.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,68 +4,64 @@
 from inline_snapshot import snapshot
 
 from logfire._internal.formatter import chunks_formatter, logfire_format
 from logfire._internal.scrubbing import Scrubber
 
 
 def chunks(format_string: str, kwargs: Mapping[str, Any]):
-    return chunks_formatter.chunks(format_string, kwargs, scrubber=Scrubber([]))
+    result, _extra_attrs, _span_name = chunks_formatter.chunks(format_string, kwargs, scrubber=Scrubber([]))
+    return result
 
 
 def test_simple_render():
     v = chunks('foo {bar}', {'bar': 'span'})
     assert v == [{'v': 'foo ', 't': 'lit'}, {'v': 'span', 't': 'arg'}]
 
 
 def test_spec():
     v = chunks('foo {bar:0.2f}', ChainMap({}, {'bar': 123.456}))
-    # insert_assert(v)
-    assert v == [{'t': 'lit', 'v': 'foo '}, {'t': 'arg', 'v': '123.46', 'spec': '0.2f'}]
+    assert v == snapshot([{'t': 'lit', 'v': 'foo '}, {'t': 'arg', 'v': '123.46', 'spec': '0.2f'}])
 
 
 def test_insert_name():
     v = chunks('foo {bar=}', {'bar': 42})
-    # insert_assert(v)
-    assert v == [{'t': 'lit', 'v': 'foo bar='}, {'t': 'arg', 'v': '42'}]
+    assert v == snapshot([{'t': 'lit', 'v': 'foo bar='}, {'t': 'arg', 'v': '42'}])
 
 
 def test_insert_name_spec():
     v = chunks('foo {bar=:d}', {'bar': 42})
-    # insert_assert(v)
-    assert v == [{'t': 'lit', 'v': 'foo bar='}, {'t': 'arg', 'v': '42', 'spec': 'd'}]
+    assert v == snapshot([{'t': 'lit', 'v': 'foo bar='}, {'t': 'arg', 'v': '42', 'spec': 'd'}])
 
 
 def test_first():
     v = chunks('{bar}', {'bar': 42})
-    # insert_assert(v)
-    assert v == [{'t': 'arg', 'v': '42'}]
+    assert v == snapshot([{'t': 'arg', 'v': '42'}])
 
 
 def test_insert_first():
     v = chunks('{bar=}', {'bar': 42})
-    # insert_assert(v)
-    assert v == [{'t': 'lit', 'v': 'bar='}, {'t': 'arg', 'v': '42'}]
+    assert v == snapshot([{'t': 'lit', 'v': 'bar='}, {'t': 'arg', 'v': '42'}])
 
 
 def test_three():
     v = chunks('{foo} {bar} {spam}', ChainMap({'foo': 1, 'bar': 2}, {'spam': '3'}))
-    # insert_assert(v)
-    assert v == [
-        {'t': 'arg', 'v': '1'},
-        {'t': 'lit', 'v': ' '},
-        {'t': 'arg', 'v': '2'},
-        {'t': 'lit', 'v': ' '},
-        {'t': 'arg', 'v': '3'},
-    ]
+    assert v == snapshot(
+        [
+            {'t': 'arg', 'v': '1'},
+            {'t': 'lit', 'v': ' '},
+            {'t': 'arg', 'v': '2'},
+            {'t': 'lit', 'v': ' '},
+            {'t': 'arg', 'v': '3'},
+        ]
+    )
 
 
 def test_dict():
     v = chunks('{foo[bar]}', {'foo': {'bar': 42}})
-    # insert_assert(v)
-    assert v == [{'t': 'arg', 'v': '42'}]
+    assert v == snapshot([{'t': 'arg', 'v': '42'}])
 
 
 def test_truncate():
     message = logfire_format(
         '1 {a} 2 {b} 3',
         dict(
             a='a' * 1000,
```

### Comparing `logfire-0.30.0/tests/test_json_args.py` & `logfire-0.31.0/tests/test_json_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections.abc import Sequence
 from dataclasses import dataclass
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from enum import Enum
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from pathlib import Path
-from typing import Any, Iterator, Mapping
+from typing import Any, Iterator, List, Mapping
 from uuid import UUID
 
 import numpy
 import pandas
 import pytest
 from attrs import define
 from dirty_equals import IsJson
@@ -848,15 +848,15 @@
 
 
 class SAModel(SABase):
     __tablename__ = 'model'
 
     id: Mapped[int] = mapped_column(primary_key=True)
     name: Mapped[str] = mapped_column(String(30))
-    models2: Mapped[list[SAModel2]] = relationship(back_populates='model', lazy='dynamic')
+    models2: Mapped[List[SAModel2]] = relationship(back_populates='model', lazy='dynamic')  # noqa
 
 
 class SAModel2(SABase):
     __tablename__ = 'model2'
 
     id: Mapped[int] = mapped_column(primary_key=True)
     model_id: Mapped[int] = mapped_column(ForeignKey('model.id'))
@@ -980,61 +980,66 @@
         list_of_objects=[
             Model(values=[1, 2]),
             Dataclass(values={'a': 1, 'b': 2}),
             PydanticDataclass(values=[{'a': 1, 'b': 2}, {'c': 3, 'd': 4}]),
         ],
     )
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict() == [
-        {
-            'name': 'hi',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'hi',
-                'logfire.msg': 'hi',
-                'code.filepath': 'test_json_args.py',
-                'code.function': 'test_log_dicts_and_lists',
-                'code.lineno': 123,
-                'list_of_lists': '[[1,2],[3,4]]',
-                'list_of_dicts': '[{"a":1},{"b":2}]',
-                'dict_of_lists': '{"a":[1,2],"b":[3,4]}',
-                'dict_of_dicts': '{"a":{"a":1},"b":{"b":2}}',
-                'complex_list': '[1,2,{"a":{"b":{"c":["d"]}}},{"b":[2]},true,false,null,"a","b",[1,2]]',
-                'complex_dict': '{"a":1,"b":{"c":{"d":[1,2]}}}',
-                'list_of_objects': '[{"values":[1,2]},{"values":{"a":1,"b":2}},{"values":[{"a":1,"b":2},{"c":3,"d":4}]}]',
-                'logfire.json_schema': IsJson(
-                    {
-                        'type': 'object',
-                        'properties': {
-                            'list_of_lists': {'type': 'array'},
-                            'list_of_dicts': {'type': 'array'},
-                            'dict_of_lists': {'type': 'object'},
-                            'dict_of_dicts': {'type': 'object'},
-                            'complex_list': {'type': 'array'},
-                            'complex_dict': {'type': 'object'},
-                            'list_of_objects': {
-                                'type': 'array',
-                                'prefixItems': [
-                                    {'type': 'object', 'title': 'Model', 'x-python-datatype': 'PydanticModel'},
-                                    {'type': 'object', 'title': 'Dataclass', 'x-python-datatype': 'dataclass'},
-                                    {'type': 'object', 'title': 'PydanticDataclass', 'x-python-datatype': 'dataclass'},
-                                ],
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'hi',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'hi',
+                    'logfire.msg': 'hi',
+                    'code.filepath': 'test_json_args.py',
+                    'code.function': 'test_log_dicts_and_lists',
+                    'code.lineno': 123,
+                    'list_of_lists': '[[1,2],[3,4]]',
+                    'list_of_dicts': '[{"a":1},{"b":2}]',
+                    'dict_of_lists': '{"a":[1,2],"b":[3,4]}',
+                    'dict_of_dicts': '{"a":{"a":1},"b":{"b":2}}',
+                    'complex_list': '[1,2,{"a":{"b":{"c":["d"]}}},{"b":[2]},true,false,null,"a","b",[1,2]]',
+                    'complex_dict': '{"a":1,"b":{"c":{"d":[1,2]}}}',
+                    'list_of_objects': '[{"values":[1,2]},{"values":{"a":1,"b":2}},{"values":[{"a":1,"b":2},{"c":3,"d":4}]}]',
+                    'logfire.json_schema': IsJson(
+                        {
+                            'type': 'object',
+                            'properties': {
+                                'list_of_lists': {'type': 'array'},
+                                'list_of_dicts': {'type': 'array'},
+                                'dict_of_lists': {'type': 'object'},
+                                'dict_of_dicts': {'type': 'object'},
+                                'complex_list': {'type': 'array'},
+                                'complex_dict': {'type': 'object'},
+                                'list_of_objects': {
+                                    'type': 'array',
+                                    'prefixItems': [
+                                        {'type': 'object', 'title': 'Model', 'x-python-datatype': 'PydanticModel'},
+                                        {'type': 'object', 'title': 'Dataclass', 'x-python-datatype': 'dataclass'},
+                                        {
+                                            'type': 'object',
+                                            'title': 'PydanticDataclass',
+                                            'x-python-datatype': 'dataclass',
+                                        },
+                                    ],
+                                },
                             },
-                        },
-                    }
-                ),
-            },
-        }
-    ]
+                        }
+                    ),
+                },
+            }
+        ]
+    )
 
 
 def test_recursive_objects(exporter: TestExporter) -> None:
     class Model(BaseModel):
         lst: list[Any]
 
     @dataclass
```

### Comparing `logfire-0.30.0/tests/test_json_args_formatting.py` & `logfire-0.31.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/test_logfire.py` & `logfire-0.31.0/tests/test_logfire.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import inspect
 import re
 import sys
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from dataclasses import dataclass
+from functools import partial
 from logging import getLogger
 from typing import Callable
 
 import pytest
 from dirty_equals import IsJson, IsStr
 from inline_snapshot import snapshot
 from opentelemetry.proto.common.v1.common_pb2 import AnyValue
@@ -25,14 +26,15 @@
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     ATTRIBUTES_TAGS_KEY,
     LEVEL_NUMBERS,
     NULL_ARGS_KEY,
 )
+from logfire._internal.formatter import InspectArgumentsFailedWarning
 from logfire.integrations.logging import LogfireLoggingHandler
 from logfire.testing import IncrementalIdGenerator, TestExporter, TimeGenerator
 
 
 @pytest.mark.parametrize('method', ['trace', 'info', 'debug', 'warn', 'error', 'fatal'])
 def test_log_methods_without_kwargs(method: str):
     with pytest.warns(UserWarning, match="The field 'foo' is not defined.") as warnings:
@@ -44,34 +46,35 @@
 
 def test_instrument_with_no_args(exporter: TestExporter) -> None:
     @logfire.instrument()
     def foo(x: int):
         return x * 2
 
     assert foo(2) == 4
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict(_strip_function_qualname=False) == [
-        {
-            'name': 'Calling tests.test_logfire.test_instrument_with_no_args.<locals>.foo',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_instrument_with_no_args.<locals>.foo',
-                'logfire.msg_template': 'Calling tests.test_logfire.test_instrument_with_no_args.<locals>.foo',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'Calling tests.test_logfire.test_instrument_with_no_args.<locals>.foo',
-                'x': 2,
-                'logfire.json_schema': '{"type":"object","properties":{"x":{}}}',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(_strip_function_qualname=False) == snapshot(
+        [
+            {
+                'name': 'Calling tests.test_logfire.test_instrument_with_no_args.<locals>.foo',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_instrument_with_no_args.<locals>.foo',
+                    'logfire.msg_template': 'Calling tests.test_logfire.test_instrument_with_no_args.<locals>.foo',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'Calling tests.test_logfire.test_instrument_with_no_args.<locals>.foo',
+                    'x': 2,
+                    'logfire.json_schema': '{"type":"object","properties":{"x":{}}}',
+                },
+            }
+        ]
+    )
 
 
 def test_instrument_without_kwargs():
     with pytest.warns(UserWarning, match="The field 'foo' is not defined.") as warnings:
 
         @logfire.instrument('{foo}')
         def home() -> None: ...
@@ -98,56 +101,57 @@
     assert s.name == 'test span'
     assert s.parent is None
     assert s.start_time is not None
     assert s.end_time is not None
     assert s.start_time < s.end_time
     assert len(s.events) == 0
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test span (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_with_kwargs',
-                'name': 'foo',
-                'number': 3,
-                'extra': 'extra',
-                'logfire.msg_template': 'test {name=} {number}',
-                'logfire.msg': 'test name=foo 3',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test span (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_with_kwargs',
+                    'name': 'foo',
+                    'number': 3,
+                    'extra': 'extra',
+                    'logfire.msg_template': 'test {name=} {number}',
+                    'logfire.msg': 'test name=foo 3',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'test span',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_with_kwargs',
-                'name': 'foo',
-                'number': 3,
-                'extra': 'extra',
-                'logfire.msg_template': 'test {name=} {number}',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'test name=foo 3',
+            {
+                'name': 'test span',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_with_kwargs',
+                    'name': 'foo',
+                    'number': 3,
+                    'extra': 'extra',
+                    'logfire.msg_template': 'test {name=} {number}',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'test name=foo 3',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_span_with_parent(exporter: TestExporter) -> None:
     with logfire.span('{type} span', _span_name='test parent span', type='parent') as p:
         with logfire.span('{type} span', _span_name='test child span', type='child') as c:
             pass
 
@@ -159,87 +163,88 @@
 
     assert c.name == 'test child span'
     assert c.parent == p.context
     assert len(c.events) == 0
     assert c.attributes is not None
     assert ATTRIBUTES_TAGS_KEY not in c.attributes
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test parent span (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_with_parent',
-                'type': 'parent',
-                'logfire.msg_template': '{type} span',
-                'logfire.msg': 'parent span',
-                'logfire.json_schema': '{"type":"object","properties":{"type":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test parent span (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_with_parent',
+                    'type': 'parent',
+                    'logfire.msg_template': '{type} span',
+                    'logfire.msg': 'parent span',
+                    'logfire.json_schema': '{"type":"object","properties":{"type":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'test child span (pending)',
-            'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_with_parent',
-                'type': 'child',
-                'logfire.msg_template': '{type} span',
-                'logfire.msg': 'child span',
-                'logfire.json_schema': '{"type":"object","properties":{"type":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000001',
+            {
+                'name': 'test child span (pending)',
+                'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_with_parent',
+                    'type': 'child',
+                    'logfire.msg_template': '{type} span',
+                    'logfire.msg': 'child span',
+                    'logfire.json_schema': '{"type":"object","properties":{"type":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000001',
+                },
             },
-        },
-        {
-            'name': 'test child span',
-            'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_with_parent',
-                'type': 'child',
-                'logfire.msg_template': '{type} span',
-                'logfire.json_schema': '{"type":"object","properties":{"type":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'child span',
+            {
+                'name': 'test child span',
+                'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_with_parent',
+                    'type': 'child',
+                    'logfire.msg_template': '{type} span',
+                    'logfire.json_schema': '{"type":"object","properties":{"type":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'child span',
+                },
             },
-        },
-        {
-            'name': 'test parent span',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 4000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_with_parent',
-                'type': 'parent',
-                'logfire.msg_template': '{type} span',
-                'logfire.json_schema': '{"type":"object","properties":{"type":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'parent span',
+            {
+                'name': 'test parent span',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_with_parent',
+                    'type': 'parent',
+                    'logfire.msg_template': '{type} span',
+                    'logfire.json_schema': '{"type":"object","properties":{"type":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'parent span',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_span_with_tags(exporter: TestExporter) -> None:
     with logfire.with_tags('tag1', 'tag2').span(
         'test {name} {number}', _span_name='test span', name='foo', number=3, extra='extra'
     ) as s:
         pass
@@ -248,58 +253,59 @@
     assert s.parent is None
     assert s.start_time is not None and s.end_time is not None
     assert s.start_time < s.end_time
     assert s.attributes is not None
     assert s.attributes[ATTRIBUTES_TAGS_KEY] == ('tag1', 'tag2')
     assert len(s.events) == 0
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test span (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_with_tags',
-                'name': 'foo',
-                'number': 3,
-                'extra': 'extra',
-                'logfire.msg_template': 'test {name} {number}',
-                'logfire.msg': 'test foo 3',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
-                'logfire.tags': ('tag1', 'tag2'),
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test span (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_with_tags',
+                    'name': 'foo',
+                    'number': 3,
+                    'extra': 'extra',
+                    'logfire.msg_template': 'test {name} {number}',
+                    'logfire.msg': 'test foo 3',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
+                    'logfire.tags': ('tag1', 'tag2'),
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'test span',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_with_tags',
-                'name': 'foo',
-                'number': 3,
-                'extra': 'extra',
-                'logfire.msg_template': 'test {name} {number}',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
-                'logfire.tags': ('tag1', 'tag2'),
-                'logfire.span_type': 'span',
-                'logfire.msg': 'test foo 3',
+            {
+                'name': 'test span',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_with_tags',
+                    'name': 'foo',
+                    'number': 3,
+                    'extra': 'extra',
+                    'logfire.msg_template': 'test {name} {number}',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
+                    'logfire.tags': ('tag1', 'tag2'),
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'test foo 3',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_span_without_span_name(exporter: TestExporter) -> None:
     with logfire.span('test {name=} {number}', name='foo', number=3, extra='extra') as s:
         pass
 
     assert s.name == 'test {name=} {number}'
@@ -311,56 +317,57 @@
     assert ATTRIBUTES_TAGS_KEY not in s.attributes
     assert s.attributes[ATTRIBUTES_MESSAGE_KEY] == 'test name=foo 3'
     assert s.attributes[ATTRIBUTES_MESSAGE_TEMPLATE_KEY] == 'test {name=} {number}'
 
     assert len(exporter.exported_spans) == 2
     # # because both spans have been ended
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test {name=} {number} (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_without_span_name',
-                'name': 'foo',
-                'number': 3,
-                'extra': 'extra',
-                'logfire.msg_template': 'test {name=} {number}',
-                'logfire.msg': 'test name=foo 3',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test {name=} {number} (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_without_span_name',
+                    'name': 'foo',
+                    'number': 3,
+                    'extra': 'extra',
+                    'logfire.msg_template': 'test {name=} {number}',
+                    'logfire.msg': 'test name=foo 3',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'test {name=} {number}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_without_span_name',
-                'name': 'foo',
-                'number': 3,
-                'extra': 'extra',
-                'logfire.msg_template': 'test {name=} {number}',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'test name=foo 3',
+            {
+                'name': 'test {name=} {number}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_without_span_name',
+                    'name': 'foo',
+                    'number': 3,
+                    'extra': 'extra',
+                    'logfire.msg_template': 'test {name=} {number}',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'test name=foo 3',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_span_end_on_exit_false(exporter: TestExporter) -> None:
     with logfire.span('test {name=} {number}', name='foo', number=3, extra='extra') as s:
         s.end_on_exit = False
 
     assert s.name == 'test {name=} {number}'
@@ -373,90 +380,92 @@
 
     assert len(exporter.exported_spans) == 1
     span = exporter.exported_spans[0]
     assert span.attributes is not None
     assert span.attributes[ATTRIBUTES_SPAN_TYPE_KEY] == 'pending_span'
     # because the real span hasn't ended yet
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test {name=} {number} (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_end_on_exit_false',
-                'name': 'foo',
-                'number': 3,
-                'extra': 'extra',
-                'logfire.msg_template': 'test {name=} {number}',
-                'logfire.msg': 'test name=foo 3',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test {name=} {number} (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_end_on_exit_false',
+                    'name': 'foo',
+                    'number': 3,
+                    'extra': 'extra',
+                    'logfire.msg_template': 'test {name=} {number}',
+                    'logfire.msg': 'test name=foo 3',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
+            }
+        ]
+    )
 
     with s:
         pass
 
     assert isinstance(s.end_time, int)
     assert s.end_time > s.start_time
     assert len(exporter.exported_spans) == 2
     span = exporter.exported_spans[1]
     assert span.attributes is not None
     assert span.attributes[ATTRIBUTES_SPAN_TYPE_KEY] == 'span'
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test {name=} {number} (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_end_on_exit_false',
-                'name': 'foo',
-                'number': 3,
-                'extra': 'extra',
-                'logfire.msg_template': 'test {name=} {number}',
-                'logfire.msg': 'test name=foo 3',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test {name=} {number} (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_end_on_exit_false',
+                    'name': 'foo',
+                    'number': 3,
+                    'extra': 'extra',
+                    'logfire.msg_template': 'test {name=} {number}',
+                    'logfire.msg': 'test name=foo 3',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'test {name=} {number}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_end_on_exit_false',
-                'name': 'foo',
-                'number': 3,
-                'extra': 'extra',
-                'logfire.msg_template': 'test {name=} {number}',
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'test name=foo 3',
+            {
+                'name': 'test {name=} {number}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_end_on_exit_false',
+                    'name': 'foo',
+                    'number': 3,
+                    'extra': 'extra',
+                    'logfire.msg_template': 'test {name=} {number}',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{},"extra":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'test name=foo 3',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 @pytest.mark.parametrize('level', ('fatal', 'debug', 'error', 'info', 'notice', 'warn', 'trace'))
 def test_log(exporter: TestExporter, level: str):
     getattr(logfire, level)('test {name} {number} {none}', name='foo', number=2, none=None)
 
     s = exporter.exported_spans[0]
@@ -503,73 +512,75 @@
     assert s.attributes is not None
     assert s.attributes['logfire.msg'] == 'test message foo=foo bar=3'
     assert s.attributes['foo'] == 'foo'
     assert s.attributes['bar'] == 3
     assert s.attributes[ATTRIBUTES_MESSAGE_TEMPLATE_KEY] == 'test message {foo=} {bar=}'
     assert s.attributes[ATTRIBUTES_SPAN_TYPE_KEY] == 'log'
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test message {foo=} {bar=}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test message {foo=} {bar=}',
-                'logfire.msg': 'test message foo=foo bar=3',
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_log_equals',
-                'foo': 'foo',
-                'bar': 3,
-                'logfire.json_schema': '{"type":"object","properties":{"foo":{},"bar":{}}}',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test message {foo=} {bar=}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test message {foo=} {bar=}',
+                    'logfire.msg': 'test message foo=foo bar=3',
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_log_equals',
+                    'foo': 'foo',
+                    'bar': 3,
+                    'logfire.json_schema': '{"type":"object","properties":{"foo":{},"bar":{}}}',
+                },
+            }
+        ]
+    )
 
 
 def test_log_with_tags(exporter: TestExporter):
     logfire.with_tags('tag1', 'tag2').info('test {name} {number}', name='foo', number=2)
 
     s = exporter.exported_spans[0]
 
     assert s.attributes is not None
     assert s.attributes[ATTRIBUTES_MESSAGE_TEMPLATE_KEY] == 'test {name} {number}'
     assert s.attributes[ATTRIBUTES_SPAN_TYPE_KEY] == 'log'
     assert s.attributes['name'] == 'foo'
     assert s.attributes['number'] == 2
     assert s.attributes[ATTRIBUTES_TAGS_KEY] == ('tag1', 'tag2')
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test {name} {number}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test {name} {number}',
-                'logfire.msg': 'test foo 2',
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_log_with_tags',
-                'name': 'foo',
-                'number': 2,
-                'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{}}}',
-                'logfire.tags': ('tag1', 'tag2'),
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test {name} {number}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test {name} {number}',
+                    'logfire.msg': 'test foo 2',
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_log_with_tags',
+                    'name': 'foo',
+                    'number': 2,
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{},"number":{}}}',
+                    'logfire.tags': ('tag1', 'tag2'),
+                },
+            }
+        ]
+    )
 
 
 def test_log_with_multiple_tags(exporter: TestExporter):
     logfire_with_2_tags = logfire.with_tags('tag1').with_tags('tag2')
     logfire_with_2_tags.info('test {name} {number}', name='foo', number=2)
     assert len(exporter.exported_spans) == 1
     s = exporter.exported_spans[0]
@@ -587,250 +598,255 @@
 def test_instrument(exporter: TestExporter):
     @logfire.instrument('hello-world {a=}')
     def hello_world(a: int) -> str:
         return f'hello {a}'
 
     assert hello_world(123) == 'hello 123'
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True, _strip_function_qualname=False) == [
-        {
-            'name': 'hello-world {a=} (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_instrument.<locals>.hello_world',
-                'a': 123,
-                'logfire.msg_template': 'hello-world {a=}',
-                'logfire.msg': 'hello-world a=123',
-                'logfire.json_schema': '{"type":"object","properties":{"a":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True, _strip_function_qualname=False) == snapshot(
+        [
+            {
+                'name': 'hello-world {a=} (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_instrument.<locals>.hello_world',
+                    'a': 123,
+                    'logfire.msg_template': 'hello-world {a=}',
+                    'logfire.msg': 'hello-world a=123',
+                    'logfire.json_schema': '{"type":"object","properties":{"a":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'hello-world {a=}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_instrument.<locals>.hello_world',
-                'a': 123,
-                'logfire.msg_template': 'hello-world {a=}',
-                'logfire.json_schema': '{"type":"object","properties":{"a":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'hello-world a=123',
+            {
+                'name': 'hello-world {a=}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_instrument.<locals>.hello_world',
+                    'a': 123,
+                    'logfire.msg_template': 'hello-world {a=}',
+                    'logfire.json_schema': '{"type":"object","properties":{"a":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'hello-world a=123',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_instrument_extract_false(exporter: TestExporter):
     @logfire.instrument('hello {a}!', extract_args=False)
     def hello_world(a: int) -> str:
         return f'hello {a}'
 
     assert hello_world(123) == 'hello 123'
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict(_strip_function_qualname=False) == [
-        {
-            'name': 'hello {a}!',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_instrument_extract_false.<locals>.hello_world',
-                'logfire.msg_template': 'hello {a}!',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'hello {a}!',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(_strip_function_qualname=False) == snapshot(
+        [
+            {
+                'name': 'hello {a}!',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_instrument_extract_false.<locals>.hello_world',
+                    'logfire.msg_template': 'hello {a}!',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'hello {a}!',
+                },
+            }
+        ]
+    )
 
 
 def test_instrument_complex_args(exporter: TestExporter):
     @logfire.instrument('hello {thing}!')
     def hello_world(thing: dict[str, int]) -> str:
         return f'hello {thing}'
 
     assert hello_world({'a': 123}) == "hello {'a': 123}"
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict(_strip_function_qualname=False) == [
-        {
-            'name': 'hello {thing}!',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_instrument_complex_args.<locals>.hello_world',
-                'logfire.msg_template': 'hello {thing}!',
-                'logfire.msg': "hello {'a': 123}!",
-                'logfire.json_schema': '{"type":"object","properties":{"thing":{"type":"object"}}}',
-                'thing': '{"a":123}',
-                'logfire.span_type': 'span',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(_strip_function_qualname=False) == snapshot(
+        [
+            {
+                'name': 'hello {thing}!',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_instrument_complex_args.<locals>.hello_world',
+                    'logfire.msg_template': 'hello {thing}!',
+                    'logfire.msg': "hello {'a': 123}!",
+                    'logfire.json_schema': '{"type":"object","properties":{"thing":{"type":"object"}}}',
+                    'thing': '{"a":123}',
+                    'logfire.span_type': 'span',
+                },
+            }
+        ]
+    )
 
 
 def test_validation_error_on_instrument(exporter: TestExporter):
     class Model(BaseModel, plugin_settings={'logfire': {'record': 'off'}}):
         a: int
 
     @logfire.instrument('hello-world {a=}')
     def run(a: str) -> Model:
         return Model(a=a)  # type: ignore
 
     with pytest.raises(ValidationError):
         run('haha')
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict(_strip_function_qualname=False) == [
-        {
-            'name': 'hello-world {a=}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_validation_error_on_instrument.<locals>.run',
-                'logfire.msg_template': 'hello-world {a=}',
-                'logfire.msg': 'hello-world a=haha',
-                'logfire.json_schema': '{"type":"object","properties":{"a":{}}}',
-                'a': 'haha',
-                'logfire.span_type': 'span',
-                'logfire.level_num': 17,
-                'exception.logfire.data': IsJson(
-                    [
-                        {
-                            'type': 'int_parsing',
-                            'loc': ['a'],
-                            'msg': 'Input should be a valid integer, unable to parse string as an integer',
-                            'input': 'haha',
-                        }
-                    ]
-                ),
-            },
-            'events': [
-                {
-                    'name': 'exception',
-                    'timestamp': 2000000000,
-                    'attributes': {
-                        'exception.type': 'ValidationError',
-                        'exception.message': IsStr(
-                            regex='1 validation error for Model\na\n  '
-                            'Input should be a valid integer, unable to parse string as an integer .+',
-                            regex_flags=re.DOTALL,
-                        ),
-                        'exception.stacktrace': IsStr(
-                            regex='For further information visit https://errors.pydantic.dev/.+'
-                        ),
-                        'exception.escaped': 'True',
-                        'exception.logfire.data': IsJson(
-                            [
-                                {
-                                    'type': 'int_parsing',
-                                    'loc': ['a'],
-                                    'msg': 'Input should be a valid integer, unable to parse string as an integer',
-                                    'input': 'haha',
-                                }
-                            ]
-                        ),
-                    },
-                }
-            ],
-        }
-    ]
+    assert exporter.exported_spans_as_dict(_strip_function_qualname=False) == snapshot(
+        [
+            {
+                'name': 'hello-world {a=}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_validation_error_on_instrument.<locals>.run',
+                    'logfire.msg_template': 'hello-world {a=}',
+                    'logfire.msg': 'hello-world a=haha',
+                    'logfire.json_schema': '{"type":"object","properties":{"a":{}}}',
+                    'a': 'haha',
+                    'logfire.span_type': 'span',
+                    'logfire.level_num': 17,
+                    'exception.logfire.data': IsJson(
+                        [
+                            {
+                                'type': 'int_parsing',
+                                'loc': ['a'],
+                                'msg': 'Input should be a valid integer, unable to parse string as an integer',
+                                'input': 'haha',
+                            }
+                        ]
+                    ),
+                },
+                'events': [
+                    {
+                        'name': 'exception',
+                        'timestamp': 2000000000,
+                        'attributes': {
+                            'exception.type': 'ValidationError',
+                            'exception.message': IsStr(
+                                regex='1 validation error for Model\na\n  '
+                                'Input should be a valid integer, unable to parse string as an integer .+',
+                                regex_flags=re.DOTALL,
+                            ),
+                            'exception.stacktrace': IsStr(
+                                regex='For further information visit https://errors.pydantic.dev/.+'
+                            ),
+                            'exception.escaped': 'True',
+                            'exception.logfire.data': IsJson(
+                                [
+                                    {
+                                        'type': 'int_parsing',
+                                        'loc': ['a'],
+                                        'msg': 'Input should be a valid integer, unable to parse string as an integer',
+                                        'input': 'haha',
+                                    }
+                                ]
+                            ),
+                        },
+                    }
+                ],
+            }
+        ]
+    )
 
 
 def test_validation_error_on_span(exporter: TestExporter) -> None:
     class Model(BaseModel, plugin_settings={'logfire': {'record': 'off'}}):
         a: int
 
     def run(a: str) -> None:
         with logfire.span('test', _span_name='test span'):
             Model(a=a)  # type: ignore
 
     with pytest.raises(ValidationError):
         run('haha')
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict() == [
-        {
-            'name': 'test span',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.function': 'run',
-                'code.lineno': 123,
-                'logfire.msg_template': 'test',
-                'logfire.msg': 'test',
-                'logfire.span_type': 'span',
-                'logfire.level_num': 17,
-                'exception.logfire.data': IsJson(
-                    [
-                        {
-                            'type': 'int_parsing',
-                            'loc': ['a'],
-                            'msg': 'Input should be a valid integer, unable to parse string as an integer',
-                            'input': 'haha',
-                        }
-                    ]
-                ),
-            },
-            'events': [
-                {
-                    'name': 'exception',
-                    'timestamp': 2000000000,
-                    'attributes': {
-                        'exception.type': 'ValidationError',
-                        'exception.message': IsStr(
-                            regex='1 validation error for Model\na\n  '
-                            'Input should be a valid integer, unable to parse string as an integer .+',
-                            regex_flags=re.DOTALL,
-                        ),
-                        'exception.stacktrace': IsStr(
-                            regex='For further information visit https://errors.pydantic.dev/.+'
-                        ),
-                        'exception.escaped': 'True',
-                        'exception.logfire.data': IsJson(
-                            [
-                                {
-                                    'type': 'int_parsing',
-                                    'loc': ['a'],
-                                    'msg': 'Input should be a valid integer, unable to parse string as an integer',
-                                    'input': 'haha',
-                                }
-                            ]
-                        ),
-                    },
-                }
-            ],
-        }
-    ]
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'test span',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'run',
+                    'code.lineno': 123,
+                    'logfire.msg_template': 'test',
+                    'logfire.msg': 'test',
+                    'logfire.span_type': 'span',
+                    'logfire.level_num': 17,
+                    'exception.logfire.data': IsJson(
+                        [
+                            {
+                                'type': 'int_parsing',
+                                'loc': ['a'],
+                                'msg': 'Input should be a valid integer, unable to parse string as an integer',
+                                'input': 'haha',
+                            }
+                        ]
+                    ),
+                },
+                'events': [
+                    {
+                        'name': 'exception',
+                        'timestamp': 2000000000,
+                        'attributes': {
+                            'exception.type': 'ValidationError',
+                            'exception.message': IsStr(
+                                regex='1 validation error for Model\na\n  '
+                                'Input should be a valid integer, unable to parse string as an integer .+',
+                                regex_flags=re.DOTALL,
+                            ),
+                            'exception.stacktrace': IsStr(
+                                regex='For further information visit https://errors.pydantic.dev/.+'
+                            ),
+                            'exception.escaped': 'True',
+                            'exception.logfire.data': IsJson(
+                                [
+                                    {
+                                        'type': 'int_parsing',
+                                        'loc': ['a'],
+                                        'msg': 'Input should be a valid integer, unable to parse string as an integer',
+                                        'input': 'haha',
+                                    }
+                                ]
+                            ),
+                        },
+                    }
+                ],
+            }
+        ]
+    )
 
 
 @dataclass
 class Foo:
     x: int
     y: int
 
@@ -878,115 +894,115 @@
     logfire1 = logfire.with_tags('tag1', 'tag2')
 
     with logfire.span('root'):
         with logfire.span('child'):
             logfire.info('test1')
             logfire1.info('test2')
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == []
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot([])
 
-    # insert_assert(exporter1.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter1.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'root (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_logfire_with_its_own_config',
-                'logfire.msg_template': 'root',
-                'logfire.msg': 'root',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter1.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'root (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_logfire_with_its_own_config',
+                    'logfire.msg_template': 'root',
+                    'logfire.msg': 'root',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'child (pending)',
-            'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_logfire_with_its_own_config',
-                'logfire.msg_template': 'child',
-                'logfire.msg': 'child',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000001',
+            {
+                'name': 'child (pending)',
+                'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_logfire_with_its_own_config',
+                    'logfire.msg_template': 'child',
+                    'logfire.msg': 'child',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000001',
+                },
             },
-        },
-        {
-            'name': 'test1',
-            'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 3000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test1',
-                'logfire.msg': 'test1',
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_logfire_with_its_own_config',
+            {
+                'name': 'test1',
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 3000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test1',
+                    'logfire.msg': 'test1',
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_logfire_with_its_own_config',
+                },
             },
-        },
-        {
-            'name': 'test2',
-            'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 4000000000,
-            'end_time': 4000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test2',
-                'logfire.msg': 'test2',
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_logfire_with_its_own_config',
-                'logfire.tags': ('tag1', 'tag2'),
+            {
+                'name': 'test2',
+                'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 4000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test2',
+                    'logfire.msg': 'test2',
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_logfire_with_its_own_config',
+                    'logfire.tags': ('tag1', 'tag2'),
+                },
             },
-        },
-        {
-            'name': 'child',
-            'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 5000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_logfire_with_its_own_config',
-                'logfire.msg_template': 'child',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'child',
+            {
+                'name': 'child',
+                'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 5000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_logfire_with_its_own_config',
+                    'logfire.msg_template': 'child',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'child',
+                },
             },
-        },
-        {
-            'name': 'root',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 6000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_logfire_with_its_own_config',
-                'logfire.msg_template': 'root',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'root',
+            {
+                'name': 'root',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 6000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_logfire_with_its_own_config',
+                    'logfire.msg_template': 'root',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'root',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def do_work() -> None:
     with logfire.span('child'):
         pass
 
 
@@ -999,206 +1015,211 @@
     exporter: TestExporter,
 ) -> None:
     with logfire.span('main'):
         with ThreadPoolExecutor() as executor:
             executor.submit(do_work)
             executor.shutdown(wait=True)
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'main (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_in_executor',
-                'logfire.msg_template': 'main',
-                'logfire.msg': 'main',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'main (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_in_executor',
+                    'logfire.msg_template': 'main',
+                    'logfire.msg': 'main',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'child (pending)',
-            'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'do_work',
-                'logfire.msg_template': 'child',
-                'logfire.msg': 'child',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000001',
+            {
+                'name': 'child (pending)',
+                'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'do_work',
+                    'logfire.msg_template': 'child',
+                    'logfire.msg': 'child',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000001',
+                },
             },
-        },
-        {
-            'name': 'child',
-            'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': True},
-            'start_time': 2000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'do_work',
-                'logfire.msg_template': 'child',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'child',
+            {
+                'name': 'child',
+                'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': True},
+                'start_time': 2000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'do_work',
+                    'logfire.msg_template': 'child',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'child',
+                },
             },
-        },
-        {
-            'name': 'main',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 4000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_span_in_executor',
-                'logfire.msg_template': 'main',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'main',
+            {
+                'name': 'main',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_span_in_executor',
+                    'logfire.msg_template': 'main',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'main',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_span_in_executor_args(exporter: TestExporter) -> None:
     with ThreadPoolExecutor() as exec:
         exec.submit(do_work_with_arg, 'foo')
         exec.shutdown(wait=True)
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'child {within} (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'do_work_with_arg',
-                'within': 'foo',
-                'logfire.msg_template': 'child {within}',
-                'logfire.msg': 'child foo',
-                'logfire.json_schema': '{"type":"object","properties":{"within":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'child {within} (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'do_work_with_arg',
+                    'within': 'foo',
+                    'logfire.msg_template': 'child {within}',
+                    'logfire.msg': 'child foo',
+                    'logfire.json_schema': '{"type":"object","properties":{"within":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'child {within}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'do_work_with_arg',
-                'within': 'foo',
-                'logfire.msg_template': 'child {within}',
-                'logfire.json_schema': '{"type":"object","properties":{"within":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'child foo',
+            {
+                'name': 'child {within}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'do_work_with_arg',
+                    'within': 'foo',
+                    'logfire.msg_template': 'child {within}',
+                    'logfire.json_schema': '{"type":"object","properties":{"within":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'child foo',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_complex_attribute_added_after_span_started(exporter: TestExporter) -> None:
     with logfire.span('hi', a={'b': 1}) as span:
         span.set_attribute('c', {'d': 2})
         span.set_attribute('e', None)
         span.set_attribute('f', None)
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict() == [
-        {
-            'name': 'hi',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.function': 'test_complex_attribute_added_after_span_started',
-                'code.lineno': 123,
-                'a': '{"b":1}',
-                'logfire.msg_template': 'hi',
-                'logfire.msg': 'hi',
-                'logfire.span_type': 'span',
-                'c': '{"d":2}',
-                'logfire.null_args': ('e', 'f'),
-                'logfire.json_schema': '{"type":"object","properties":{"a":{"type":"object"},"c":{"type":"object"},"e":{},"f":{}}}',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'hi',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_complex_attribute_added_after_span_started',
+                    'code.lineno': 123,
+                    'a': '{"b":1}',
+                    'logfire.msg_template': 'hi',
+                    'logfire.msg': 'hi',
+                    'logfire.span_type': 'span',
+                    'c': '{"d":2}',
+                    'logfire.null_args': ('e', 'f'),
+                    'logfire.json_schema': '{"type":"object","properties":{"a":{"type":"object"},"c":{"type":"object"},"e":{},"f":{}}}',
+                },
+            }
+        ]
+    )
 
 
 def test_format_attribute_added_after_pending_span_sent(exporter: TestExporter) -> None:
     with pytest.warns(UserWarning, match=r'missing') as warnings:
         span = logfire.span('{present} {missing}', present='here')
 
     assert len(warnings) == 1
     assert warnings[0].filename == __file__
+    assert warnings[0].lineno == inspect.currentframe().f_lineno - 4  # type: ignore
 
     with span:
         # Previously the message was reformatted with this attribute, not any more
         span.set_attribute('missing', 'value')
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': '{present} {missing} (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_format_attribute_added_after_pending_span_sent',
-                'present': 'here',
-                'logfire.msg_template': '{present} {missing}',
-                'logfire.msg': 'here {missing}',
-                'logfire.json_schema': '{"type":"object","properties":{"present":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': '{present} {missing} (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_format_attribute_added_after_pending_span_sent',
+                    'present': 'here',
+                    'logfire.msg_template': '{present} {missing}',
+                    'logfire.msg': 'here {missing}',
+                    'logfire.json_schema': '{"type":"object","properties":{"present":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': '{present} {missing}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_format_attribute_added_after_pending_span_sent',
-                'present': 'here',
-                'logfire.msg_template': '{present} {missing}',
-                'logfire.msg': 'here {missing}',
-                'logfire.json_schema': '{"type":"object","properties":{"present":{},"missing":{}}}',
-                'logfire.span_type': 'span',
-                'missing': 'value',
+            {
+                'name': '{present} {missing}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_format_attribute_added_after_pending_span_sent',
+                    'present': 'here',
+                    'logfire.msg_template': '{present} {missing}',
+                    'logfire.msg': 'here {missing}',
+                    'logfire.json_schema': '{"type":"object","properties":{"present":{},"missing":{}}}',
+                    'logfire.span_type': 'span',
+                    'missing': 'value',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def check_project_name(expected_project_name: str) -> None:
     from logfire._internal.config import GLOBAL_CONFIG
 
     assert GLOBAL_CONFIG.project_name == expected_project_name
 
@@ -1225,246 +1246,252 @@
         executor.submit(check_project_name, 'foobar!')
         executor.shutdown(wait=True)
 
 
 def test_kwarg_with_dot_in_name(exporter: TestExporter) -> None:
     logfire.info('{http.status}', **{'http.status': 123})  # type: ignore
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': '{http.status}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': '{http.status}',
-                'logfire.msg': '123',
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_kwarg_with_dot_in_name',
-                'http.status': 123,
-                'logfire.json_schema': '{"type":"object","properties":{"http.status":{}}}',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': '{http.status}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': '{http.status}',
+                    'logfire.msg': '123',
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_kwarg_with_dot_in_name',
+                    'http.status': 123,
+                    'logfire.json_schema': '{"type":"object","properties":{"http.status":{}}}',
+                },
+            }
+        ]
+    )
 
     exporter.exported_spans.clear()
 
     with logfire.span('{http.status} - {code.lineno}', **{'http.status': 123}):  # type: ignore
         pass
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': '{http.status} - {code.lineno} (pending)',
-            'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
-            'parent': {'trace_id': 2, 'span_id': 2, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_kwarg_with_dot_in_name',
-                'http.status': 123,
-                'logfire.msg_template': '{http.status} - {code.lineno}',
-                'logfire.msg': IsStr(regex=r'123 - \d+'),
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
-                'logfire.json_schema': '{"type":"object","properties":{"http.status":{}}}',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': '{http.status} - {code.lineno} (pending)',
+                'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 2, 'span_id': 2, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_kwarg_with_dot_in_name',
+                    'http.status': 123,
+                    'logfire.msg_template': '{http.status} - {code.lineno}',
+                    'logfire.msg': IsStr(regex=r'123 - \d+'),
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                    'logfire.json_schema': '{"type":"object","properties":{"http.status":{}}}',
+                },
             },
-        },
-        {
-            'name': '{http.status} - {code.lineno}',
-            'context': {'trace_id': 2, 'span_id': 2, 'is_remote': False},
-            'parent': None,
-            'start_time': 2000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_kwarg_with_dot_in_name',
-                'http.status': 123,
-                'logfire.msg_template': '{http.status} - {code.lineno}',
-                'logfire.msg': IsStr(regex=r'123 - \d+'),
-                'logfire.span_type': 'span',
-                'logfire.json_schema': '{"type":"object","properties":{"http.status":{}}}',
+            {
+                'name': '{http.status} - {code.lineno}',
+                'context': {'trace_id': 2, 'span_id': 2, 'is_remote': False},
+                'parent': None,
+                'start_time': 2000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_kwarg_with_dot_in_name',
+                    'http.status': 123,
+                    'logfire.msg_template': '{http.status} - {code.lineno}',
+                    'logfire.msg': IsStr(regex=r'123 - \d+'),
+                    'logfire.span_type': 'span',
+                    'logfire.json_schema': '{"type":"object","properties":{"http.status":{}}}',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 @pytest.mark.parametrize('method', ('trace', 'debug', 'info', 'notice', 'warn', 'error', 'fatal', 'span'))
 def test_forbid_methods_with_leading_underscore_on_attributes(method: str) -> None:
     with pytest.raises(ValueError, match='Attribute keys cannot start with an underscore.'):
         getattr(logfire, method)('test {_foo=}', _foo='bar')
 
     with pytest.raises(ValueError, match='Attribute keys cannot start with an underscore.'):
         getattr(logfire, method)('test {__foo=}', __foo='bar')
 
 
 def test_log_with_leading_underscore_on_attributes(exporter: TestExporter) -> None:
     logfire.log('info', 'test {_foo=}', attributes={'_foo': 'bar'})
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test {_foo=}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'test {_foo=}',
-                'logfire.msg': 'test _foo=bar',
-                'code.filepath': 'test_logfire.py',
-                'code.function': 'test_log_with_leading_underscore_on_attributes',
-                'code.lineno': 123,
-                '_foo': 'bar',
-                'logfire.json_schema': '{"type":"object","properties":{"_foo":{}}}',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test {_foo=}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'test {_foo=}',
+                    'logfire.msg': 'test _foo=bar',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_log_with_leading_underscore_on_attributes',
+                    'code.lineno': 123,
+                    '_foo': 'bar',
+                    'logfire.json_schema': '{"type":"object","properties":{"_foo":{}}}',
+                },
+            }
+        ]
+    )
 
 
 def test_large_int(exporter: TestExporter) -> None:
     with pytest.warns(UserWarning, match='larger than the maximum OTLP integer size'):
         with logfire.span('test {value=}', value=2**63 + 1):
             pass
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test {value=} (pending)',
-            'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_large_int',
-                'value': '9223372036854775809',
-                'logfire.msg_template': 'test {value=}',
-                'logfire.msg': 'test value=9223372036854775809',
-                'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test {value=} (pending)',
+                'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_large_int',
+                    'value': '9223372036854775809',
+                    'logfire.msg_template': 'test {value=}',
+                    'logfire.msg': 'test value=9223372036854775809',
+                    'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'test {value=}',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_large_int',
-                'value': '9223372036854775809',
-                'logfire.msg_template': 'test {value=}',
-                'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'test value=9223372036854775809',
+            {
+                'name': 'test {value=}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_large_int',
+                    'value': '9223372036854775809',
+                    'logfire.msg_template': 'test {value=}',
+                    'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'test value=9223372036854775809',
+                },
             },
-        },
-    ]
+        ]
+    )
     exporter.exported_spans.clear()
 
     with pytest.warns(UserWarning, match='larger than the maximum OTLP integer size'):
         with logfire.span('test {value=}', value=2**63):
             pass
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test {value=} (pending)',
-            'context': {'trace_id': 2, 'span_id': 4, 'is_remote': False},
-            'parent': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
-            'start_time': 3000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_large_int',
-                'value': '9223372036854775808',
-                'logfire.msg_template': 'test {value=}',
-                'logfire.msg': 'test value=9223372036854775808',
-                'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test {value=} (pending)',
+                'context': {'trace_id': 2, 'span_id': 4, 'is_remote': False},
+                'parent': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
+                'start_time': 3000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_large_int',
+                    'value': '9223372036854775808',
+                    'logfire.msg_template': 'test {value=}',
+                    'logfire.msg': 'test value=9223372036854775808',
+                    'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'test {value=}',
-            'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
-            'parent': None,
-            'start_time': 3000000000,
-            'end_time': 4000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_large_int',
-                'value': '9223372036854775808',
-                'logfire.msg_template': 'test {value=}',
-                'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'test value=9223372036854775808',
+            {
+                'name': 'test {value=}',
+                'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
+                'parent': None,
+                'start_time': 3000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_large_int',
+                    'value': '9223372036854775808',
+                    'logfire.msg_template': 'test {value=}',
+                    'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'test value=9223372036854775808',
+                },
             },
-        },
-    ]
+        ]
+    )
     exporter.exported_spans.clear()
 
     with logfire.span('test {value=}', value=2**63 - 1):
         pass
 
-    # insert_assert(exporter.exported_spans_as_dict(_include_pending_spans=True))
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == [
-        {
-            'name': 'test {value=} (pending)',
-            'context': {'trace_id': 3, 'span_id': 6, 'is_remote': False},
-            'parent': {'trace_id': 3, 'span_id': 5, 'is_remote': False},
-            'start_time': 5000000000,
-            'end_time': 5000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_large_int',
-                'value': 9223372036854775807,
-                'logfire.msg_template': 'test {value=}',
-                'logfire.msg': 'test value=9223372036854775807',
-                'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
-                'logfire.span_type': 'pending_span',
-                'logfire.pending_parent_id': '0000000000000000',
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
+        [
+            {
+                'name': 'test {value=} (pending)',
+                'context': {'trace_id': 3, 'span_id': 6, 'is_remote': False},
+                'parent': {'trace_id': 3, 'span_id': 5, 'is_remote': False},
+                'start_time': 5000000000,
+                'end_time': 5000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_large_int',
+                    'value': 9223372036854775807,
+                    'logfire.msg_template': 'test {value=}',
+                    'logfire.msg': 'test value=9223372036854775807',
+                    'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
+                    'logfire.span_type': 'pending_span',
+                    'logfire.pending_parent_id': '0000000000000000',
+                },
             },
-        },
-        {
-            'name': 'test {value=}',
-            'context': {'trace_id': 3, 'span_id': 5, 'is_remote': False},
-            'parent': None,
-            'start_time': 5000000000,
-            'end_time': 6000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.lineno': 123,
-                'code.function': 'test_large_int',
-                'value': 9223372036854775807,
-                'logfire.msg_template': 'test {value=}',
-                'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
-                'logfire.span_type': 'span',
-                'logfire.msg': 'test value=9223372036854775807',
+            {
+                'name': 'test {value=}',
+                'context': {'trace_id': 3, 'span_id': 5, 'is_remote': False},
+                'parent': None,
+                'start_time': 5000000000,
+                'end_time': 6000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_large_int',
+                    'value': 9223372036854775807,
+                    'logfire.msg_template': 'test {value=}',
+                    'logfire.json_schema': '{"type":"object","properties":{"value":{}}}',
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'test value=9223372036854775807',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_readable_span_signature():
     # This is to test that we are providing all the arguments we can when
     # constructing ReadableSpans (e.g. in PendingSpanProcessor and SpanProcessorWrapper)
     # i.e. if this test fails it means that the OTEL SDK has been updated
     # and places in our code constructing ReadableSpans needs to be updated to add the new arguments.
@@ -1493,50 +1520,51 @@
 
 
 def test_tags(exporter: TestExporter) -> None:
     lf = logfire.with_tags('tag1', 'tag2')
     with lf.span('a span', _tags=('tag2', 'tag3')):
         lf.info('a log', _tags=('tag4', 'tag1'))
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict() == [
-        {
-            'name': 'a log',
-            'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'a log',
-                'logfire.msg': 'a log',
-                'code.filepath': 'test_logfire.py',
-                'code.function': 'test_tags',
-                'code.lineno': 123,
-                'logfire.tags': ('tag1', 'tag2', 'tag4'),
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'a log',
+                'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'a log',
+                    'logfire.msg': 'a log',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_tags',
+                    'code.lineno': 123,
+                    'logfire.tags': ('tag1', 'tag2', 'tag4'),
+                },
             },
-        },
-        {
-            'name': 'a span',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 3000000000,
-            'attributes': {
-                'code.filepath': 'test_logfire.py',
-                'code.function': 'test_tags',
-                'code.lineno': 123,
-                'logfire.msg_template': 'a span',
-                'logfire.msg': 'a span',
-                'logfire.tags': ('tag1', 'tag2', 'tag3'),
-                'logfire.span_type': 'span',
+            {
+                'name': 'a span',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_tags',
+                    'code.lineno': 123,
+                    'logfire.msg_template': 'a span',
+                    'logfire.msg': 'a span',
+                    'logfire.tags': ('tag1', 'tag2', 'tag3'),
+                    'logfire.span_type': 'span',
+                },
             },
-        },
-    ]
+        ]
+    )
 
 
 def test_exc_info(exporter: TestExporter):
     logger = getLogger(__name__)
     logger.addHandler(LogfireLoggingHandler())
 
     logfire.debug('no error', _exc_info=True)
@@ -1695,7 +1723,734 @@
                     'code.filepath': 'test_logfire.py',
                     'code.function': 'test_invalid_log_level',
                     'code.lineno': 123,
                 },
             }
         ]
     )
+
+
+GLOBAL_VAR = 1
+
+
+@pytest.mark.skipif(
+    sys.version_info < (3, 11), reason='f-string magic clashes with @logfire.instrument() in Python < 3.11'
+)
+def test_inspect_arguments(exporter: TestExporter):
+    local_var = 2
+    x = 1.2345
+
+    # Test that `executing` still works in instrumented functions for Python 3.11+.
+    @logfire.instrument()
+    def foo():
+        # Test some cases that require `executing` (i.e. the simple fallback heuristics can't handle)
+        # particularly two `span` calls in one line.
+        with logfire.span(f'span {GLOBAL_VAR} {local_var}'), logfire.span(f'span2 {local_var}'):
+            str(logfire.info(f'log {GLOBAL_VAR} {local_var}'))
+
+        with pytest.warns(UserWarning) as warnings:
+            logfire.info(f'log2 {local_var}', local_var=3, x=x)
+        assert str(warnings[0].message) == snapshot(
+            "The attribute 'local_var' has the same name as a variable with a different value. Using the attribute."
+        )
+        assert warnings[0].filename == __file__
+        frame = inspect.currentframe()
+        assert frame is not None
+        assert warnings[0].lineno == frame.f_lineno - 7
+
+        # Test the .log method which has the argument in a different place from the other methods.
+        logfire.log('error', f'log3 {GLOBAL_VAR}')
+        logfire.log(level='error', msg_template=f'log4 {GLOBAL_VAR}')
+
+        # Test putting exotic things inside braces.
+        # Note that the span name / message template differ slightly from the f-string in these cases.
+        logfire.info(f'log5 {local_var = }')
+        logfire.info(f'log6 {x:.{local_var}f}')
+        logfire.info(f'log7 {str(local_var)!r}')
+
+    foo()
+
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'log {GLOBAL_VAR} {local_var}',
+                'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'start_time': 4000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'log {GLOBAL_VAR} {local_var}',
+                    'logfire.msg': f'log {GLOBAL_VAR} {local_var}',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'GLOBAL_VAR': 1,
+                    'local_var': 2,
+                    'logfire.json_schema': '{"type":"object","properties":{"GLOBAL_VAR":{},"local_var":{}}}',
+                },
+            },
+            {
+                'name': 'span2 {local_var}',
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 3000000000,
+                'end_time': 5000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'local_var': 2,
+                    'logfire.msg_template': 'span2 {local_var}',
+                    'logfire.msg': f'span2 {local_var}',
+                    'logfire.json_schema': '{"type":"object","properties":{"local_var":{}}}',
+                    'logfire.span_type': 'span',
+                },
+            },
+            {
+                'name': 'span {GLOBAL_VAR} {local_var}',
+                'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 6000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg_template': 'span {GLOBAL_VAR} {local_var}',
+                    'GLOBAL_VAR': 1,
+                    'logfire.msg': f'span {GLOBAL_VAR} {local_var}',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'local_var': 2,
+                    'logfire.json_schema': '{"type":"object","properties":{"GLOBAL_VAR":{},"local_var":{}}}',
+                },
+            },
+            {
+                'name': 'log2 {local_var}',
+                'context': {'trace_id': 1, 'span_id': 8, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 7000000000,
+                'end_time': 7000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'logfire.level_num': 9,
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'local_var': 3,
+                    'logfire.msg_template': 'log2 {local_var}',
+                    'logfire.msg': 'log2 3',
+                    'logfire.json_schema': '{"type":"object","properties":{"local_var":{},"x":{}}}',
+                    'x': 1.2345,
+                    'logfire.span_type': 'log',
+                },
+            },
+            {
+                'name': 'log3 {GLOBAL_VAR}',
+                'context': {'trace_id': 1, 'span_id': 9, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 8000000000,
+                'end_time': 8000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': 'log3 {GLOBAL_VAR}',
+                    'logfire.msg': f'log3 {GLOBAL_VAR}',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'GLOBAL_VAR': 1,
+                    'logfire.json_schema': '{"type":"object","properties":{"GLOBAL_VAR":{}}}',
+                },
+            },
+            {
+                'name': 'log4 {GLOBAL_VAR}',
+                'context': {'trace_id': 1, 'span_id': 10, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 9000000000,
+                'end_time': 9000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': 'log4 {GLOBAL_VAR}',
+                    'logfire.msg': f'log4 {GLOBAL_VAR}',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'GLOBAL_VAR': 1,
+                    'logfire.json_schema': '{"type":"object","properties":{"GLOBAL_VAR":{}}}',
+                },
+            },
+            {
+                'name': 'log5 local_var = {local_var}',
+                'context': {'trace_id': 1, 'span_id': 11, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 10000000000,
+                'end_time': 10000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'log5 local_var = {local_var}',
+                    'logfire.msg': f'log5 {local_var = }',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'local_var': 2,
+                    'logfire.json_schema': '{"type":"object","properties":{"local_var":{}}}',
+                },
+            },
+            {
+                'name': 'log6 {x}',
+                'context': {'trace_id': 1, 'span_id': 12, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 11000000000,
+                'end_time': 11000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'log6 {x}',
+                    'logfire.msg': f'log6 {x:.{local_var}f}',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'x': 1.2345,
+                    'logfire.json_schema': '{"type":"object","properties":{"x":{}}}',
+                },
+            },
+            {
+                'name': 'log7 {str(local_var)}',
+                'context': {'trace_id': 1, 'span_id': 13, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 12000000000,
+                'end_time': 12000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'log7 {str(local_var)}',
+                    'logfire.msg': f'log7 {str(local_var)!r}',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'str(local_var)': '2',
+                    'logfire.json_schema': '{"type":"object","properties":{"str(local_var)":{}}}',
+                },
+            },
+            {
+                'name': 'Calling tests.test_logfire.test_inspect_arguments.<locals>.foo',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 13000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'foo',
+                    'logfire.msg_template': 'Calling tests.test_logfire.test_inspect_arguments.<locals>.foo',
+                    'logfire.msg': 'Calling tests.test_logfire.test_inspect_arguments.<locals>.foo',
+                    'logfire.span_type': 'span',
+                },
+            },
+        ]
+    )
+
+
+@pytest.mark.skipif(sys.version_info < (3, 11), reason='Testing behaviour in Python 3.11+')
+def test_executing_failure(exporter: TestExporter, monkeypatch: pytest.MonkeyPatch):
+    # We're about to 'disable' `executing` which `snapshot` also uses, so make the snapshot first.
+    expected_spans = snapshot(
+        [
+            {
+                'name': 'good log {local_var}',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'good log {local_var}',
+                    'logfire.msg': 'good log 3',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_executing_failure',
+                    'code.lineno': 123,
+                    'things': '[]',
+                    'local_var': 3,
+                    'logfire.json_schema': '{"type":"object","properties":{"things":{"type":"array","x-python-datatype":"set"},"local_var":{}}}',
+                },
+            },
+            {
+                'name': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node.\
+""",
+                'context': {'trace_id': 2, 'span_id': 2, 'is_remote': False},
+                'parent': None,
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node.\
+""",
+                    'logfire.msg': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node.\
+""",
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_executing_failure',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': 'bad log 3',
+                'context': {'trace_id': 3, 'span_id': 3, 'is_remote': False},
+                'parent': None,
+                'start_time': 3000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'bad log 3',
+                    'logfire.msg': 'bad log 3',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_executing_failure',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': 'good span {local_var}',
+                'context': {'trace_id': 4, 'span_id': 4, 'is_remote': False},
+                'parent': None,
+                'start_time': 4000000000,
+                'end_time': 5000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_executing_failure',
+                    'code.lineno': 123,
+                    'local_var': 3,
+                    'logfire.msg_template': 'good span {local_var}',
+                    'logfire.msg': 'good span 3',
+                    'logfire.json_schema': '{"type":"object","properties":{"local_var":{}}}',
+                    'logfire.span_type': 'span',
+                },
+            },
+            {
+                'name': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node.\
+""",
+                'context': {'trace_id': 5, 'span_id': 6, 'is_remote': False},
+                'parent': None,
+                'start_time': 6000000000,
+                'end_time': 6000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node.\
+""",
+                    'logfire.msg': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node.\
+""",
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_executing_failure',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node.\
+""",
+                'context': {'trace_id': 6, 'span_id': 9, 'is_remote': False},
+                'parent': {'trace_id': 6, 'span_id': 7, 'is_remote': False},
+                'start_time': 8000000000,
+                'end_time': 8000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node.\
+""",
+                    'logfire.msg': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node.\
+""",
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_executing_failure',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': 'bad span 2 3',
+                'context': {'trace_id': 6, 'span_id': 10, 'is_remote': False},
+                'parent': {'trace_id': 6, 'span_id': 7, 'is_remote': False},
+                'start_time': 9000000000,
+                'end_time': 10000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_executing_failure',
+                    'code.lineno': 123,
+                    'logfire.msg_template': 'bad span 2 3',
+                    'logfire.msg': 'bad span 2 3',
+                    'logfire.span_type': 'span',
+                },
+            },
+            {
+                'name': 'bad span 1 3',
+                'context': {'trace_id': 6, 'span_id': 7, 'is_remote': False},
+                'parent': None,
+                'start_time': 7000000000,
+                'end_time': 11000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_executing_failure',
+                    'code.lineno': 123,
+                    'logfire.msg_template': 'bad span 1 3',
+                    'logfire.msg': 'bad span 1 3',
+                    'logfire.span_type': 'span',
+                },
+            },
+        ]
+    )
+    import executing._position_node_finder
+
+    # Test what happens when `executing` fails.
+    monkeypatch.setattr(executing._position_node_finder.PositionNodeFinder, 'find_node', lambda _: None)  # type: ignore  # pragma: no cover  (coverage being weird)
+
+    local_var = 3
+    # The simple heuristic works when there's only one call with arguments in the whole statement.
+    logfire.info(f'good log {local_var}', things=set())
+
+    with pytest.warns(InspectArgumentsFailedWarning, match='`executing` failed to find a node.$'):
+        # Two calls with arguments breaks the heuristic
+        str(logfire.info(f'bad log {local_var}'))
+
+    # Works:
+    with logfire.span(f'good span {local_var}'):
+        pass
+
+    with pytest.warns(InspectArgumentsFailedWarning, match='`executing` failed to find a node.$'):
+        # Multiple calls break the heuristic.
+        with logfire.span(f'bad span 1 {local_var}'), logfire.span(f'bad span 2 {local_var}'):
+            pass
+
+    assert exporter.exported_spans_as_dict() == expected_spans
+
+
+@pytest.mark.skipif(
+    sys.version_info[:2] > (3, 10) or sys.version_info[:2] < (3, 9),
+    reason='Testing behaviour for Python < 3.11 but > 3.8',
+)
+def test_executing_failure_old_python(exporter: TestExporter):
+    local_var = 2
+
+    # For older versions, the AST modification done by `@instrument` interferes with `executing`.
+    @logfire.instrument()
+    def foo():  # pragma: no cover  (coverage being weird)
+        # For these cases, the simple heuristic still works.
+        with logfire.span(f'span {GLOBAL_VAR} {local_var}'):
+            logfire.info(f'log {GLOBAL_VAR} {local_var}')
+
+        # But here it doesn't, see the previous test.
+        with pytest.warns(InspectArgumentsFailedWarning, match='`executing` failed to find a node.'):
+            str(logfire.info(f'bad log {local_var}'))
+
+    foo()
+
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'log {GLOBAL_VAR} {local_var}',
+                'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'start_time': 3000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'log {GLOBAL_VAR} {local_var}',
+                    'logfire.msg': f'log {GLOBAL_VAR} {local_var}',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'GLOBAL_VAR': 1,
+                    'local_var': 2,
+                    'logfire.json_schema': '{"type":"object","properties":{"GLOBAL_VAR":{},"local_var":{}}}',
+                },
+            },
+            {
+                'name': 'span {GLOBAL_VAR} {local_var}',
+                'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                    'GLOBAL_VAR': 1,
+                    'local_var': 2,
+                    'logfire.msg_template': 'span {GLOBAL_VAR} {local_var}',
+                    'logfire.msg': f'span {GLOBAL_VAR} {local_var}',
+                    'logfire.json_schema': '{"type":"object","properties":{"GLOBAL_VAR":{},"local_var":{}}}',
+                    'logfire.span_type': 'span',
+                },
+            },
+            {
+                'name': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node. This may be caused by a combination of using Python < 3.11 and auto-tracing or @logfire.instrument.\
+""",
+                'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 5000000000,
+                'end_time': 5000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node. This may be caused by a combination of using Python < 3.11 and auto-tracing or @logfire.instrument.\
+""",
+                    'logfire.msg': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+`executing` failed to find a node. This may be caused by a combination of using Python < 3.11 and auto-tracing or @logfire.instrument.\
+""",
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': 'bad log 2',
+                'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 6000000000,
+                'end_time': 6000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'bad log 2',
+                    'logfire.msg': 'bad log 2',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'foo',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': 'Calling tests.test_logfire.test_executing_failure_old_python.<locals>.foo',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 7000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.lineno': 123,
+                    'code.function': 'test_executing_failure_old_python.<locals>.foo',
+                    'logfire.msg_template': 'Calling tests.test_logfire.test_executing_failure_old_python.<locals>.foo',
+                    'logfire.msg': 'Calling tests.test_logfire.test_executing_failure_old_python.<locals>.foo',
+                    'logfire.span_type': 'span',
+                },
+            },
+        ]
+    )
+
+
+@pytest.mark.skipif(
+    sys.version_info[:2] == (3, 8), reason='Warning is only raised in Python 3.9+ because f-string magic is enabled'
+)
+def test_find_arg_failure(exporter: TestExporter):
+    info = partial(logfire.info, 'info')
+    log = partial(logfire.log, 'error', 'log')
+    span = partial(logfire.span, 'span')
+    with pytest.warns(
+        InspectArgumentsFailedWarning, match="Couldn't identify the `msg_template` argument in the call."
+    ):
+        info()
+    with pytest.warns(
+        InspectArgumentsFailedWarning, match="Couldn't identify the `msg_template` argument in the call."
+    ):
+        log()
+    with pytest.warns(
+        InspectArgumentsFailedWarning, match="Couldn't identify the `msg_template` argument in the call."
+    ):
+        with span():
+            pass
+
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+Couldn't identify the `msg_template` argument in the call.\
+""",
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+Couldn't identify the `msg_template` argument in the call.\
+""",
+                    'logfire.msg': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+Couldn't identify the `msg_template` argument in the call.\
+""",
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_find_arg_failure',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': 'info',
+                'context': {'trace_id': 2, 'span_id': 2, 'is_remote': False},
+                'parent': None,
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'info',
+                    'logfire.msg': 'info',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_find_arg_failure',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+Couldn't identify the `msg_template` argument in the call.\
+""",
+                'context': {'trace_id': 3, 'span_id': 3, 'is_remote': False},
+                'parent': None,
+                'start_time': 3000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+Couldn't identify the `msg_template` argument in the call.\
+""",
+                    'logfire.msg': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+Couldn't identify the `msg_template` argument in the call.\
+""",
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_find_arg_failure',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': 'log',
+                'context': {'trace_id': 4, 'span_id': 4, 'is_remote': False},
+                'parent': None,
+                'start_time': 4000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': 'log',
+                    'logfire.msg': 'log',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_find_arg_failure',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+Couldn't identify the `msg_template` argument in the call.\
+""",
+                'context': {'trace_id': 5, 'span_id': 5, 'is_remote': False},
+                'parent': None,
+                'start_time': 5000000000,
+                'end_time': 5000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+Couldn't identify the `msg_template` argument in the call.\
+""",
+                    'logfire.msg': """\
+Failed to introspect calling code. Please report this issue to Logfire. Falling back to normal message formatting which may result in loss of information if using an f-string. Set inspect_arguments=False in logfire.configure() to suppress this warning. The problem was:
+Couldn't identify the `msg_template` argument in the call.\
+""",
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_find_arg_failure',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': 'span',
+                'context': {'trace_id': 6, 'span_id': 6, 'is_remote': False},
+                'parent': None,
+                'start_time': 6000000000,
+                'end_time': 7000000000,
+                'attributes': {
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_find_arg_failure',
+                    'code.lineno': 123,
+                    'logfire.msg_template': 'span',
+                    'logfire.msg': 'span',
+                    'logfire.span_type': 'span',
+                },
+            },
+        ]
+    )
+
+
+@pytest.mark.skipif(sys.version_info[:2] == (3, 8), reason='fstring magic is only for 3.9+')
+def test_wrong_fstring_source_segment(exporter: TestExporter):
+    name = 'me'
+    # This is a case where `ast.get_source_segment` returns an incorrect string for `{name}`
+    # in some Python versions, hence the fallback to `ast.unparse` (so this still works).
+    logfire.info(
+        f"""
+        Hello {name}
+        """
+    )
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': """\
+
+        Hello {name}
+        \
+""",
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': """\
+
+        Hello {name}
+        \
+""",
+                    'logfire.msg': """\
+
+        Hello me
+        \
+""",
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_wrong_fstring_source_segment',
+                    'code.lineno': 123,
+                    'name': 'me',
+                    'logfire.json_schema': '{"type":"object","properties":{"name":{}}}',
+                },
+            }
+        ]
+    )
```

### Comparing `logfire-0.30.0/tests/test_loguru.py` & `logfire-0.31.0/tests/test_loguru.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @pytest.fixture(scope='module', autouse=True)
 def configure_logger() -> Any:
     loguru.logger.configure(handlers=[loguru_handler()])
 
 
 def test_loguru(exporter: TestExporter) -> None:
-    logger.info('Positional arguments are merged to the message: {}', 'positional')
+    logger.success('Positional arguments are merged to the message: {}', 'positional')
     logger.info('Keyword arguments are stored in the "extra", we extra them from there: {name}', name='named')
 
     try:
         raise ValueError('This is a test exception')
     except ValueError:
         logger.exception('An exception was raised: {foo}', foo='bar')
 
@@ -31,15 +31,15 @@
                 'name': 'Positional arguments are merged to the message: {}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 1000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
-                    'logfire.level_num': 9,
+                    'logfire.level_num': 11,
                     'logfire.msg_template': 'Positional arguments are merged to the message: {}',
                     'logfire.msg': 'Positional arguments are merged to the message: positional',
                     'code.filepath': 'test_loguru.py',
                     'code.function': 'test_loguru',
                     'code.lineno': 20,
                     'logfire.logging_args': '["positional"]',
                     'logfire.json_schema': '{"type":"object","properties":{"logfire.logging_args":{"type":"array","x-python-datatype":"tuple"}}}',
```

### Comparing `logfire-0.30.0/tests/test_metrics.py` & `logfire-0.31.0/tests/test_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import json
 import subprocess
 from typing import Any, cast
 
+import pytest
 from dirty_equals._numeric import IsInt
 from inline_snapshot import snapshot
 from opentelemetry.metrics import CallbackOptions, Observation
 from opentelemetry.sdk.metrics.export import AggregationTemporality, InMemoryMetricReader, MetricsData
 
 import logfire
+import logfire._internal.metrics
 
 
 def test_system_metrics_collection() -> None:
     metrics_reader = InMemoryMetricReader()
     logfire.configure(
         send_to_logfire=False,
         metric_readers=[metrics_reader],
@@ -125,14 +127,72 @@
                     'aggregation_temporality': AggregationTemporality.DELTA,
                 },
             }
         ]
     )
 
 
+def test_create_metric_gauge(metrics_reader: InMemoryMetricReader) -> None:
+    temperature = logfire.metric_gauge('temperature')
+    temperature.set(1)
+    assert get_collected_metrics(metrics_reader) == snapshot(
+        [
+            {
+                'name': 'temperature',
+                'description': '',
+                'unit': '',
+                'data': {
+                    'data_points': [
+                        {
+                            'attributes': {},
+                            'start_time_unix_nano': 0,
+                            'time_unix_nano': IsInt(),
+                            'value': 1,
+                        }
+                    ]
+                },
+            }
+        ]
+    )
+
+    # The value is updated, not accumulated. The previous value is overwritten.
+    temperature.set(20)
+    temperature.set(24)
+    assert get_collected_metrics(metrics_reader) == snapshot(
+        [
+            {
+                'name': 'temperature',
+                'description': '',
+                'unit': '',
+                'data': {
+                    'data_points': [
+                        {
+                            'attributes': {},
+                            'start_time_unix_nano': 0,
+                            'time_unix_nano': IsInt(),
+                            'value': 24,
+                        }
+                    ]
+                },
+            }
+        ]
+    )
+
+
+def test_create_metric_gauge_old_opentelemetry_sdk(monkeypatch: pytest.MonkeyPatch) -> None:
+    monkeypatch.setattr(logfire._internal.metrics, 'Gauge', None)
+    with pytest.raises(RuntimeError) as exc_info:
+        logfire.metric_gauge('gauge')
+    assert str(exc_info.value) == snapshot("""\
+Gauge is not available in this version of OpenTelemetry SDK.
+You should upgrade to 1.23.0 or newer:
+   pip install opentelemetry-sdk>=1.23.0\
+""")
+
+
 def test_create_metric_up_down_counter(metrics_reader: InMemoryMetricReader) -> None:
     counter = logfire.metric_up_down_counter('up_down_counter')
     counter.add(1)
     counter.add(20)
     metrics_reader.collect()
     counter.add(300)
     counter.add(4000)
```

### Comparing `logfire-0.30.0/tests/test_no_production.py` & `logfire-0.31.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/test_pydantic_plugin.py` & `logfire-0.31.0/tests/test_pydantic_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,16 +285,16 @@
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic MyModel validate_python succeeded',
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_pydantic_plugin_python_success',
                     'code.lineno': 123,
                     'result': '{"x":1}',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{},"result":{"type":"object","title":"MyModel","x-python-datatype":"PydanticModel"}}}',
                     'success': True,
                     'input_data': '{"x":1}',
                     'schema_name': 'MyModel',
                     'validation_method': 'validate_python',
@@ -432,16 +432,16 @@
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic MyModel validate_python failed',
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_pydantic_plugin_python_error',
                     'code.lineno': 123,
                     'schema_name': 'MyModel',
                     'error_count': 1,
                     'errors': '[{"type":"int_parsing","loc":["x"],"msg":"Input should be a valid integer, unable to parse string as an integer","input":"a"}]',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{},"error_count":{},"errors":{"type":"array","items":{"type":"object","properties":{"loc":{"type":"array","x-python-datatype":"tuple"}}}}}}',
                     'success': False,
                     'validation_method': 'validate_python',
@@ -467,16 +467,16 @@
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic MyModel validate_json succeeded',
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_pydantic_plugin_json_success',
                     'code.lineno': 123,
                     'result': '{"x":1}',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{},"success":{},"result":{"type":"object","title":"MyModel","x-python-datatype":"PydanticModel"}}}',
                     'success': True,
                     'input_data': '{"x":1}',
                     'schema_name': 'MyModel',
                     'validation_method': 'validate_json',
@@ -502,16 +502,16 @@
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic MyModel validate_python failed',
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_pydantic_plugin_json_error',
                     'code.lineno': 123,
                     'schema_name': 'MyModel',
                     'error_count': 1,
                     'errors': '[{"type":"int_parsing","loc":["x"],"msg":"Input should be a valid integer, unable to parse string as an integer","input":"a"}]',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{},"error_count":{},"errors":{"type":"array","items":{"type":"object","properties":{"loc":{"type":"array","x-python-datatype":"tuple"}}}}}}',
                     'success': False,
                     'validation_method': 'validate_python',
@@ -537,16 +537,16 @@
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic MyModel validate_strings succeeded',
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_pydantic_plugin_strings_success',
                     'code.lineno': 123,
                     'result': '{"x":1}',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{},"result":{"type":"object","title":"MyModel","x-python-datatype":"PydanticModel"}}}',
                     'success': True,
                     'input_data': '{"x":"1"}',
                     'schema_name': 'MyModel',
                     'validation_method': 'validate_strings',
@@ -572,16 +572,16 @@
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic MyModel validate_strings failed',
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_pydantic_plugin_strings_error',
                     'code.lineno': 123,
                     'schema_name': 'MyModel',
                     'error_count': 1,
                     'errors': '[{"type":"int_parsing","loc":["x"],"msg":"Input should be a valid integer, unable to parse string as an integer","input":"a"}]',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{},"error_count":{},"errors":{"type":"array","items":{"type":"object","properties":{"loc":{"type":"array","x-python-datatype":"tuple"}}}}}}',
                     'success': False,
                     'validation_method': 'validate_strings',
@@ -725,16 +725,16 @@
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'start_time': 2000000000,
                 'end_time': 3000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic Model1 validate_python succeeded',
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'validate_m',
                     'code.lineno': 123,
                     'result': '{"x":10}',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{},"result":{"type":"object","title":"Model1","x-python-datatype":"PydanticModel"}}}',
                     'success': True,
                     'input_data': '{"x":10}',
                     'schema_name': 'Model1',
                     'validation_method': 'validate_python',
@@ -744,16 +744,16 @@
             {
                 'name': 'pydantic.validate_python',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 4000000000,
                 'attributes': {
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_pydantic_plugin_nested_model',
                     'code.lineno': 123,
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic Model2 validate_python succeeded',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{},"result":{"type":"object","title":"Model2","x-python-datatype":"PydanticModel","properties":{"m":{"type":"object","title":"Model1","x-python-datatype":"PydanticModel"}}}}}',
                     'logfire.span_type': 'span',
                     'schema_name': 'Model2',
                     'validation_method': 'validate_python',
@@ -769,16 +769,16 @@
                 'parent': {'trace_id': 2, 'span_id': 5, 'is_remote': False},
                 'start_time': 6000000000,
                 'end_time': 7000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic Model1 validate_python failed',
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'validate_m',
                     'code.lineno': 123,
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{},"error_count":{},"errors":{"type":"array","items":{"type":"object","properties":{"loc":{"type":"array","x-python-datatype":"tuple"}}}}}}',
                     'success': False,
                     'input_data': '{"x":"y"}',
                     'schema_name': 'Model1',
                     'validation_method': 'validate_python',
                     'error_count': 1,
@@ -789,16 +789,16 @@
             {
                 'name': 'pydantic.validate_python',
                 'context': {'trace_id': 2, 'span_id': 5, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
                 'end_time': 8000000000,
                 'attributes': {
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_pydantic_plugin_nested_model',
                     'code.lineno': 123,
                     'schema_name': 'Model2',
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic Model2 validate_python failed',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{},"error_count":{},"errors":{"type":"array","items":{"type":"object","properties":{"loc":{"type":"array","x-python-datatype":"tuple"}}}}}}',
                     'logfire.span_type': 'span',
                     'input_data': '{"m":{"x":"y"}}',
@@ -833,16 +833,16 @@
                 'start_time': 1000000000,
                 'end_time': 3000000000,
                 'attributes': {
                     'logfire.span_type': 'span',
                     'logfire.level_num': 17,
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.msg': 'Pydantic MyModel validate_python raised TypeError',
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_pydantic_plugin_python_exception',
                     'code.lineno': 123,
                     'schema_name': 'MyModel',
                     'logfire.json_schema': '{"type":"object","properties":{"schema_name":{},"validation_method":{},"input_data":{"type":"object"},"success":{}}}',
                     'validation_method': 'validate_python',
                     'input_data': '{"x":1}',
                     'success': False,
                 },
@@ -966,16 +966,16 @@
                 {
                     'name': 'pydantic.validate_python',
                     'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                     'parent': None,
                     'start_time': 1000000000,
                     'end_time': 2000000000,
                     'attributes': {
-                        'code.filepath': 'pydantic.py',
-                        'code.function': '_on_enter',
+                        'code.filepath': 'test_pydantic_plugin.py',
+                        'code.function': 'test_old_plugin_style',
                         'code.lineno': 123,
                         'schema_name': 'MyModel',
                         'validation_method': 'validate_python',
                         'input_data': '{"x":1}',
                         'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                         'logfire.level_num': 9,
                         'logfire.span_type': 'span',
@@ -988,16 +988,16 @@
                 {
                     'name': 'pydantic.validate_python',
                     'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                     'parent': None,
                     'start_time': 3000000000,
                     'end_time': 5000000000,
                     'attributes': {
-                        'code.filepath': 'pydantic.py',
-                        'code.function': '_on_enter',
+                        'code.filepath': 'test_pydantic_plugin.py',
+                        'code.function': 'test_old_plugin_style',
                         'code.lineno': 123,
                         'schema_name': 'MyModel',
                         'validation_method': 'validate_python',
                         'input_data': '{"x":2}',
                         'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                         'logfire.span_type': 'span',
                         'success': False,
@@ -1021,16 +1021,16 @@
                 {
                     'name': 'pydantic.validate_python',
                     'context': {'trace_id': 3, 'span_id': 5, 'is_remote': False},
                     'parent': None,
                     'start_time': 6000000000,
                     'end_time': 7000000000,
                     'attributes': {
-                        'code.filepath': 'pydantic.py',
-                        'code.function': '_on_enter',
+                        'code.filepath': 'test_pydantic_plugin.py',
+                        'code.function': 'test_old_plugin_style',
                         'code.lineno': 123,
                         'schema_name': 'MyModel',
                         'validation_method': 'validate_python',
                         'input_data': '{"x":"a"}',
                         'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                         'logfire.span_type': 'span',
                         'success': False,
@@ -1064,16 +1064,16 @@
             {
                 'name': 'pydantic.validate_python',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'pydantic.py',
-                    'code.function': '_on_enter',
+                    'code.filepath': 'test_pydantic_plugin.py',
+                    'code.function': 'test_function_validator',
                     'code.lineno': 123,
                     'schema_name': 'int',
                     'validation_method': 'validate_python',
                     'input_data': 3,
                     'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                     'logfire.level_num': 9,
                     'logfire.span_type': 'span',
@@ -1112,16 +1112,16 @@
                 {
                     'name': 'pydantic.validate_python',
                     'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                     'parent': None,
                     'start_time': 1000000000,
                     'end_time': 2000000000,
                     'attributes': {
-                        'code.filepath': 'pydantic.py',
-                        'code.function': '_on_enter',
+                        'code.filepath': 'test_pydantic_plugin.py',
+                        'code.function': 'test_record_all_env_var',
                         'code.lineno': 123,
                         'schema_name': 'MyModel',
                         'validation_method': 'validate_python',
                         'input_data': '{"x":2}',
                         'logfire.msg_template': 'Pydantic {schema_name} {validation_method}',
                         'logfire.level_num': 9,
                         'logfire.span_type': 'span',
```

### Comparing `logfire-0.30.0/tests/test_sampling.py` & `logfire-0.31.0/tests/test_sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Any
 
 import pytest
+from inline_snapshot import snapshot
 from opentelemetry.sdk.metrics.export import InMemoryMetricReader
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 
 import logfire
 from logfire.testing import SeededRandomIdGenerator, TestExporter, TimeGenerator
 
 
@@ -117,19 +118,20 @@
 
     for _ in range(10):
         with logfire.DEFAULT_LOGFIRE_INSTANCE.with_trace_sample_rate(0.1).span('1'):
             with logfire.span('2'):
                 with logfire.span('3'):
                     pass
 
-    # insert_assert(build_tree(exporter.exported_spans_as_dict()))
-    assert build_tree(exporter.exported_spans_as_dict()) == [
-        SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
-        SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
-    ]
+    assert build_tree(exporter.exported_spans_as_dict()) == snapshot(
+        [
+            SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
+            SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
+        ]
+    )
 
 
 @pytest.mark.skipif(
     not hasattr(logfire, 'with_trace_sample_rate'), reason='with_trace_sample_rate is hidden from public API'
 )
 def test_outer_and_inner_sampled() -> None:  # pragma: no cover
     exporter = TestExporter()
@@ -145,25 +147,26 @@
 
     for _ in range(10):
         with logfire.DEFAULT_LOGFIRE_INSTANCE.with_trace_sample_rate(0.75).span('1'):
             with logfire.DEFAULT_LOGFIRE_INSTANCE.with_trace_sample_rate(0.75).span('2'):
                 with logfire.DEFAULT_LOGFIRE_INSTANCE.with_trace_sample_rate(0.75).span('3'):
                     pass
 
-    # insert_assert(build_tree(exporter.exported_spans_as_dict()))
-    assert build_tree(exporter.exported_spans_as_dict()) == [
-        SpanNode(name='1', children=[SpanNode(name='2', children=[])]),
-        SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
-        SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
-        SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
-        SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
-        SpanNode(name='1', children=[]),
-        SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
-        SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
-    ]
+    assert build_tree(exporter.exported_spans_as_dict()) == snapshot(
+        [
+            SpanNode(name='1', children=[SpanNode(name='2', children=[])]),
+            SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
+            SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
+            SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
+            SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
+            SpanNode(name='1', children=[]),
+            SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
+            SpanNode(name='1', children=[SpanNode(name='2', children=[SpanNode(name='3', children=[])])]),
+        ]
+    )
 
 
 @pytest.mark.skipif(
     not hasattr(logfire, 'with_trace_sample_rate'), reason='with_trace_sample_rate is hidden from public API'
 )
 def test_sampling_rate_does_not_get_overwritten() -> None:  # pragma: no cover
     exporter = TestExporter()
@@ -179,9 +182,8 @@
 
     for _ in range(10):
         with logfire.DEFAULT_LOGFIRE_INSTANCE.with_trace_sample_rate(0).span('1'):
             for _ in range(100):
                 with logfire.DEFAULT_LOGFIRE_INSTANCE.with_trace_sample_rate(1).span('2'):
                     pass
 
-    # insert_assert(build_tree(exporter.exported_spans_as_dict()))
-    assert build_tree(exporter.exported_spans_as_dict()) == []
+    assert build_tree(exporter.exported_spans_as_dict()) == snapshot([])
```

### Comparing `logfire-0.30.0/tests/test_secret_scrubbing.py` & `logfire-0.31.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/test_slow_async_callbacks.py` & `logfire-0.31.0/tests/test_slow_async_callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 from asyncio.events import Handle
 
 import pytest
 from dirty_equals import IsInt
+from inline_snapshot import snapshot
 
 import logfire
 from logfire.testing import TestExporter
 from tests.import_used_for_tests.slow_async_callbacks_example import main
 
 
 def test_slow_async_callbacks(exporter: TestExporter) -> None:
@@ -22,130 +23,131 @@
 
         with pytest.raises(RuntimeError):
             asyncio.run(main())
 
     # Check that the patching is no longer in effect
     assert Handle._run.__qualname__ == 'Handle._run'
 
-    # insert_assert(exporter.exported_spans_as_dict(fixed_line_number=None))
-    assert exporter.exported_spans_as_dict(fixed_line_number=None) == [
-        {
-            'name': 'Async {name} blocked for {duration:.3f} seconds',
-            'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
-            'parent': None,
-            'start_time': IsInt,
-            'end_time': IsInt,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 13,
-                'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
-                'logfire.msg': 'Async callback mock_block blocked for 2.000 seconds',
-                'code.filepath': 'slow_async_callbacks_example.py',
-                'code.function': 'mock_block',
-                'code.lineno': 31,
-                'duration': 2.0,
-                'name': 'callback mock_block',
-                'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
-                'logfire.tags': ('slow-async',),
-            },
-        },
-        {
-            'name': 'Async {name} blocked for {duration:.3f} seconds',
-            'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
-            'parent': None,
-            'start_time': IsInt,
-            'end_time': IsInt,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 13,
-                'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
-                'logfire.msg': 'Async task foo 1 (foo) blocked for 2.000 seconds',
-                'code.filepath': 'slow_async_callbacks_example.py',
-                'code.function': 'foo',
-                'code.lineno': 28,
-                'duration': 2.0,
-                'name': 'task foo 1 (foo)',
-                'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
-                'logfire.tags': ('slow-async',),
-            },
-        },
-        {
-            'name': 'Async {name} blocked for {duration:.3f} seconds',
-            'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
-            'parent': None,
-            'start_time': IsInt,
-            'end_time': IsInt,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 13,
-                'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
-                'logfire.msg': 'Async task bar 1 (bar) blocked for 2.000 seconds',
-                'code.filepath': 'slow_async_callbacks_example.py',
-                'code.function': 'bar',
-                'code.lineno': 15,
-                'duration': 2.0,
-                'name': 'task bar 1 (bar)',
-                'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
-                'logfire.tags': ('slow-async',),
-            },
-        },
-        {
-            'name': 'Async {name} blocked for {duration:.3f} seconds',
-            'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
-            'parent': None,
-            'start_time': IsInt,
-            'end_time': IsInt,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 13,
-                'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
-                'logfire.msg': 'Async task bar 1 (bar) blocked for 3.000 seconds',
-                'code.filepath': 'slow_async_callbacks_example.py',
-                'code.function': 'bar',
-                'code.lineno': 18,
-                'duration': 3.0,
-                'name': 'task bar 1 (bar)',
-                'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
-                'logfire.tags': ('slow-async',),
-            },
-        },
-        {
-            'name': 'Async {name} blocked for {duration:.3f} seconds',
-            'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
-            'parent': None,
-            'start_time': IsInt,
-            'end_time': IsInt,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 13,
-                'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
-                'logfire.msg': 'Async task foo 2 (foo) blocked for 2.000 seconds',
-                'code.filepath': 'slow_async_callbacks_example.py',
-                'code.function': 'foo',
-                'code.lineno': 28,
-                'duration': 2.0,
-                'name': 'task foo 2 (foo)',
-                'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
-                'logfire.tags': ('slow-async',),
-            },
-        },
-        {
-            'name': 'Async {name} blocked for {duration:.3f} seconds',
-            'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
-            'parent': None,
-            'start_time': IsInt,
-            'end_time': IsInt,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 13,
-                'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
-                'logfire.msg': 'Async task bar 1 (bar) blocked for 4.000 seconds',
-                'code.filepath': 'slow_async_callbacks_example.py',
-                'code.function': 'bar',
-                'code.lineno': 14,
-                'duration': 4.0,
-                'name': 'task bar 1 (bar)',
-                'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
-                'logfire.tags': ('slow-async',),
+    assert exporter.exported_spans_as_dict(fixed_line_number=None) == snapshot(
+        [
+            {
+                'name': 'Async {name} blocked for {duration:.3f} seconds',
+                'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
+                'parent': None,
+                'start_time': IsInt,
+                'end_time': IsInt,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
+                    'logfire.msg': 'Async callback mock_block blocked for 2.000 seconds',
+                    'code.filepath': 'slow_async_callbacks_example.py',
+                    'code.function': 'mock_block',
+                    'code.lineno': 31,
+                    'duration': 2.0,
+                    'name': 'callback mock_block',
+                    'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
+                    'logfire.tags': ('slow-async',),
+                },
+            },
+            {
+                'name': 'Async {name} blocked for {duration:.3f} seconds',
+                'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
+                'parent': None,
+                'start_time': IsInt,
+                'end_time': IsInt,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
+                    'logfire.msg': 'Async task foo 1 (foo) blocked for 2.000 seconds',
+                    'code.filepath': 'slow_async_callbacks_example.py',
+                    'code.function': 'foo',
+                    'code.lineno': 28,
+                    'duration': 2.0,
+                    'name': 'task foo 1 (foo)',
+                    'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
+                    'logfire.tags': ('slow-async',),
+                },
+            },
+            {
+                'name': 'Async {name} blocked for {duration:.3f} seconds',
+                'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
+                'parent': None,
+                'start_time': IsInt,
+                'end_time': IsInt,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
+                    'logfire.msg': 'Async task bar 1 (bar) blocked for 2.000 seconds',
+                    'code.filepath': 'slow_async_callbacks_example.py',
+                    'code.function': 'bar',
+                    'code.lineno': 15,
+                    'duration': 2.0,
+                    'name': 'task bar 1 (bar)',
+                    'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
+                    'logfire.tags': ('slow-async',),
+                },
+            },
+            {
+                'name': 'Async {name} blocked for {duration:.3f} seconds',
+                'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
+                'parent': None,
+                'start_time': IsInt,
+                'end_time': IsInt,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
+                    'logfire.msg': 'Async task bar 1 (bar) blocked for 3.000 seconds',
+                    'code.filepath': 'slow_async_callbacks_example.py',
+                    'code.function': 'bar',
+                    'code.lineno': 18,
+                    'duration': 3.0,
+                    'name': 'task bar 1 (bar)',
+                    'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
+                    'logfire.tags': ('slow-async',),
+                },
+            },
+            {
+                'name': 'Async {name} blocked for {duration:.3f} seconds',
+                'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
+                'parent': None,
+                'start_time': IsInt,
+                'end_time': IsInt,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
+                    'logfire.msg': 'Async task foo 2 (foo) blocked for 2.000 seconds',
+                    'code.filepath': 'slow_async_callbacks_example.py',
+                    'code.function': 'foo',
+                    'code.lineno': 28,
+                    'duration': 2.0,
+                    'name': 'task foo 2 (foo)',
+                    'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
+                    'logfire.tags': ('slow-async',),
+                },
+            },
+            {
+                'name': 'Async {name} blocked for {duration:.3f} seconds',
+                'context': {'trace_id': IsInt, 'span_id': IsInt, 'is_remote': False},
+                'parent': None,
+                'start_time': IsInt,
+                'end_time': IsInt,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': 'Async {name} blocked for {duration:.3f} seconds',
+                    'logfire.msg': 'Async task bar 1 (bar) blocked for 4.000 seconds',
+                    'code.filepath': 'slow_async_callbacks_example.py',
+                    'code.function': 'bar',
+                    'code.lineno': 14,
+                    'duration': 4.0,
+                    'name': 'task bar 1 (bar)',
+                    'logfire.json_schema': '{"type":"object","properties":{"duration":{},"name":{}}}',
+                    'logfire.tags': ('slow-async',),
+                },
             },
-        },
-    ]
+        ]
+    )
```

### Comparing `logfire-0.30.0/tests/test_stdlib_logging.py` & `logfire-0.31.0/tests/test_stdlib_logging.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,61 +22,63 @@
     _logger.addHandler(LogfireLoggingHandler())
     return _logger
 
 
 def test_stdlib_logging(exporter: TestExporter, logger: Logger) -> None:
     logger.error('{first_name=} is in trouble!', extra={'first_name': 'Fred'})
 
-    # insert_assert(exporter.exported_spans_as_dict(fixed_line_number=None))
-    assert exporter.exported_spans_as_dict(fixed_line_number=None) == [
-        {
-            'name': '{first_name=} is in trouble!',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 17,
-                'logfire.msg_template': '{first_name=} is in trouble!',
-                'logfire.msg': '{first_name=} is in trouble!',
-                'code.filepath': 'test_stdlib_logging.py',
-                'code.function': 'test_stdlib_logging',
-                'code.lineno': IsPositiveInt(),
-                'first_name': 'Fred',
-                'logfire.json_schema': '{"type":"object","properties":{"first_name":{}}}',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(fixed_line_number=None) == snapshot(
+        [
+            {
+                'name': '{first_name=} is in trouble!',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': '{first_name=} is in trouble!',
+                    'logfire.msg': '{first_name=} is in trouble!',
+                    'code.filepath': 'test_stdlib_logging.py',
+                    'code.function': 'test_stdlib_logging',
+                    'code.lineno': IsPositiveInt(),
+                    'first_name': 'Fred',
+                    'logfire.json_schema': '{"type":"object","properties":{"first_name":{}}}',
+                },
+            }
+        ]
+    )
 
 
 def test_stdlib_logging_with_positional_params(exporter: TestExporter, logger: Logger) -> None:
     logger.error('This is a test message %s.', 'with a parameter')
 
-    # insert_assert(exporter.exported_spans_as_dict(fixed_line_number=None))
-    assert exporter.exported_spans_as_dict(fixed_line_number=None) == [
-        {
-            'name': 'This is a test message %s.',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 17,
-                'logfire.msg_template': 'This is a test message %s.',
-                'logfire.msg': 'This is a test message with a parameter.',
-                'code.filepath': 'test_stdlib_logging.py',
-                'code.function': 'test_stdlib_logging_with_positional_params',
-                'code.lineno': IsPositiveInt(),
-                'logfire.logging_args': '["with a parameter"]',
-                'logfire.json_schema': '{"type":"object","properties":{"logfire.logging_args":{"type":"array","x-python-datatype":"tuple"}}}',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(fixed_line_number=None) == snapshot(
+        [
+            {
+                'name': 'This is a test message %s.',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': 'This is a test message %s.',
+                    'logfire.msg': 'This is a test message with a parameter.',
+                    'code.filepath': 'test_stdlib_logging.py',
+                    'code.function': 'test_stdlib_logging_with_positional_params',
+                    'code.lineno': IsPositiveInt(),
+                    'logfire.logging_args': '["with a parameter"]',
+                    'logfire.json_schema': '{"type":"object","properties":{"logfire.logging_args":{"type":"array","x-python-datatype":"tuple"}}}',
+                },
+            }
+        ]
+    )
 
 
 def test_stdlib_logging_with_positional_dict_param(exporter: TestExporter, logger: Logger) -> None:
     logger.error('This is a test message %s.', {'param': 'with a parameter'})
 
     assert exporter.exported_spans_as_dict() == snapshot(
         [
@@ -101,90 +103,93 @@
         ]
     )
 
 
 def test_stdlib_logging_with_parenthesis_params(exporter: TestExporter, logger: Logger) -> None:
     logger.error('This is a test message %(module)s')
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict() == [
-        {
-            'name': 'This is a test message %(module)s',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 17,
-                'logfire.msg_template': 'This is a test message %(module)s',
-                'logfire.msg': 'This is a test message %(module)s',
-                'code.filepath': 'test_stdlib_logging.py',
-                'code.function': 'test_stdlib_logging_with_parenthesis_params',
-                'code.lineno': IsPositiveInt(),
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'This is a test message %(module)s',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': 'This is a test message %(module)s',
+                    'logfire.msg': 'This is a test message %(module)s',
+                    'code.filepath': 'test_stdlib_logging.py',
+                    'code.function': 'test_stdlib_logging_with_parenthesis_params',
+                    'code.lineno': IsPositiveInt(),
+                },
+            }
+        ]
+    )
 
 
 def test_stdlib_logging_with_custom_parenthesis_params(exporter: TestExporter, logger: Logger) -> None:
     logger.error('abc %(blah)s', {'blah': 'blah'})
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict() == [
-        {
-            'name': 'abc %(blah)s',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 17,
-                'logfire.msg_template': 'abc %(blah)s',
-                'logfire.msg': 'abc blah',
-                'code.filepath': 'test_stdlib_logging.py',
-                'code.function': 'test_stdlib_logging_with_custom_parenthesis_params',
-                'code.lineno': IsPositiveInt(),
-                'blah': 'blah',
-                'logfire.json_schema': '{"type":"object","properties":{"blah":{}}}',
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'abc %(blah)s',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': 'abc %(blah)s',
+                    'logfire.msg': 'abc blah',
+                    'code.filepath': 'test_stdlib_logging.py',
+                    'code.function': 'test_stdlib_logging_with_custom_parenthesis_params',
+                    'code.lineno': IsPositiveInt(),
+                    'blah': 'blah',
+                    'logfire.json_schema': '{"type":"object","properties":{"blah":{}}}',
+                },
+            }
+        ]
+    )
 
 
 def test_stdlib_logging_warning(exporter: TestExporter, logger: Logger) -> None:
     logger.warning('%s is in some trouble', 'Fred')
 
-    # insert_assert(exporter.exported_spans_as_dict(fixed_line_number=None))
-    assert exporter.exported_spans_as_dict(fixed_line_number=None) == [
-        {
-            'name': '%s is in some trouble',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 13,
-                'logfire.msg_template': '%s is in some trouble',
-                'logfire.msg': 'Fred is in some trouble',
-                'code.filepath': 'test_stdlib_logging.py',
-                'code.function': 'test_stdlib_logging_warning',
-                'code.lineno': IsPositiveInt(),
-                'logfire.logging_args': '["Fred"]',
-                'logfire.json_schema': IsJson(
-                    {
-                        'type': 'object',
-                        'properties': {'logfire.logging_args': {'type': 'array', 'x-python-datatype': 'tuple'}},
-                    }
-                ),
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(fixed_line_number=None) == snapshot(
+        [
+            {
+                'name': '%s is in some trouble',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': '%s is in some trouble',
+                    'logfire.msg': 'Fred is in some trouble',
+                    'code.filepath': 'test_stdlib_logging.py',
+                    'code.function': 'test_stdlib_logging_warning',
+                    'code.lineno': IsPositiveInt(),
+                    'logfire.logging_args': '["Fred"]',
+                    'logfire.json_schema': IsJson(
+                        {
+                            'type': 'object',
+                            'properties': {'logfire.logging_args': {'type': 'array', 'x-python-datatype': 'tuple'}},
+                        }
+                    ),
+                },
+            }
+        ]
+    )
 
 
 def test_recursive_logging_from_opentelemetry() -> None:
     class ExceptionExporter(SpanExporter):
         def export(self, spans: Sequence[ReadableSpan]):
             raise Exception()
```

### Comparing `logfire-0.30.0/tests/test_structlog.py` & `logfire-0.31.0/tests/test_structlog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from logging import Logger
 from typing import Any
 
 import pytest
 import structlog
+from inline_snapshot import snapshot
 
 from logfire.integrations.structlog import LogfireProcessor
 from logfire.testing import TestExporter
 
 
 @pytest.fixture(autouse=True, scope='module')
 def fixture_configure_structlog() -> None:
@@ -26,27 +27,28 @@
 @pytest.fixture(scope='module')
 def logger() -> Any:
     return structlog.get_logger()
 
 
 def test_structlog(exporter: TestExporter, logger: Logger) -> None:
     logger.info('This is now being logged.')
-    # insert_assert(exporter.exported_spans_as_dict(fixed_line_number=None))
-    assert exporter.exported_spans_as_dict(fixed_line_number=None) == [
-        {
-            'name': 'This is now being logged.',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 1000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'This is now being logged.',
-                'logfire.msg': 'This is now being logged.',
-                'code.filepath': 'python.py',
-                'code.function': 'pytest_pyfunc_call',
-                'code.lineno': 195,
-                'logfire.disable_console_log': True,
-            },
-        }
-    ]
+    assert exporter.exported_spans_as_dict(fixed_line_number=None) == snapshot(
+        [
+            {
+                'name': 'This is now being logged.',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'This is now being logged.',
+                    'logfire.msg': 'This is now being logged.',
+                    'code.filepath': 'test_structlog.py',
+                    'code.function': 'test_structlog',
+                    'code.lineno': 33,
+                    'logfire.disable_console_log': True,
+                },
+            }
+        ]
+    )
```

### Comparing `logfire-0.30.0/tests/test_testing.py` & `logfire-0.31.0/tests/test_testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+from inline_snapshot import snapshot
 
 import logfire
 from logfire.testing import CaptureLogfire, TestExporter, TimeGenerator
 
 
 def test_reset_exported_spans(exporter: TestExporter) -> None:
     assert len(exporter.exported_spans) == 0
@@ -26,61 +27,62 @@
 def test_capfire_fixture(capfire: CaptureLogfire) -> None:
     with pytest.raises(Exception):
         with logfire.span('a span!'):
             logfire.info('a log!')
             raise Exception('an exception!')
 
     exporter = capfire.exporter
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict() == [
-        {
-            'name': 'a log!',
-            'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-            'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'start_time': 2000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'logfire.span_type': 'log',
-                'logfire.level_num': 9,
-                'logfire.msg_template': 'a log!',
-                'logfire.msg': 'a log!',
-                'code.filepath': 'test_testing.py',
-                'code.function': 'test_capfire_fixture',
-                'code.lineno': 123,
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'a log!',
+                'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
+                'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'a log!',
+                    'logfire.msg': 'a log!',
+                    'code.filepath': 'test_testing.py',
+                    'code.function': 'test_capfire_fixture',
+                    'code.lineno': 123,
+                },
             },
-        },
-        {
-            'name': 'a span!',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 4000000000,
-            'attributes': {
-                'code.filepath': 'test_testing.py',
-                'code.function': 'test_capfire_fixture',
-                'code.lineno': 123,
-                'logfire.msg_template': 'a span!',
-                'logfire.msg': 'a span!',
-                'logfire.span_type': 'span',
-                'logfire.level_num': 17,
+            {
+                'name': 'a span!',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'code.filepath': 'test_testing.py',
+                    'code.function': 'test_capfire_fixture',
+                    'code.lineno': 123,
+                    'logfire.msg_template': 'a span!',
+                    'logfire.msg': 'a span!',
+                    'logfire.span_type': 'span',
+                    'logfire.level_num': 17,
+                },
+                'events': [
+                    {
+                        'name': 'exception',
+                        'timestamp': 3000000000,
+                        'attributes': {
+                            'exception.type': 'Exception',
+                            'exception.message': 'an exception!',
+                            'exception.stacktrace': 'Exception: an exception!',
+                            'exception.escaped': 'True',
+                        },
+                    }
+                ],
             },
-            'events': [
-                {
-                    'name': 'exception',
-                    'timestamp': 3000000000,
-                    'attributes': {
-                        'exception.type': 'Exception',
-                        'exception.message': 'an exception!',
-                        'exception.stacktrace': 'Exception: an exception!',
-                        'exception.escaped': 'True',
-                    },
-                }
-            ],
-        },
-    ]
+        ]
+    )
 
 
 def test_time_generator():
     t = TimeGenerator()
     assert t() == 1000000000
     assert t() == 2000000000
     assert repr(t) == 'TimeGenerator(ns_time=2000000000)'
```

### Comparing `logfire-0.30.0/tests/test_utils.py` & `logfire-0.31.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/utils.py` & `logfire-0.31.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/exporters/test_fallback_exporter.py` & `logfire-0.31.0/tests/exporters/test_fallback_exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import Sequence
 
 import pytest
+from inline_snapshot import snapshot
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SpanExporter, SpanExportResult
 from opentelemetry.sdk.util.instrumentation import (
     InstrumentationScope,
 )
 from opentelemetry.trace import SpanContext, SpanKind
@@ -51,38 +52,40 @@
 
     exporter = FallbackSpanExporter(ExceptionExporter(), test_exporter)
     with pytest.raises(Exception, match='Bad, bad exporter 😉'):
         exporter.export([TEST_SPAN])
 
     exporter.shutdown()
 
-    # insert_assert(test_exporter.exported_spans_as_dict())
-    assert test_exporter.exported_spans_as_dict() == [
-        {
-            'name': 'test',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 0,
-            'end_time': 1,
-            'attributes': {},
-        }
-    ]
+    assert test_exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'test',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 0,
+                'end_time': 1,
+                'attributes': {},
+            }
+        ]
+    )
 
 
 def test_fallback_on_failure() -> None:
     test_exporter = TestExporter()
 
     exporter = FallbackSpanExporter(FailureExporter(), test_exporter)
     exporter.export([TEST_SPAN])
     exporter.shutdown()
 
-    # insert_assert(test_exporter.exported_spans_as_dict())
-    assert test_exporter.exported_spans_as_dict() == [
-        {
-            'name': 'test',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 0,
-            'end_time': 1,
-            'attributes': {},
-        }
-    ]
+    assert test_exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'test',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 0,
+                'end_time': 1,
+                'attributes': {},
+            }
+        ]
+    )
```

### Comparing `logfire-0.30.0/tests/exporters/test_file_exporter.py` & `logfire-0.31.0/tests/exporters/test_file_exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import json
 from pathlib import Path
 
 from google.protobuf.json_format import MessageToJson
+from inline_snapshot import snapshot
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.util.instrumentation import (
     InstrumentationScope,
 )
 from opentelemetry.trace import SpanContext, SpanKind
 from opentelemetry.trace.status import Status, StatusCode
@@ -47,68 +48,16 @@
     assert path.exists()
 
     # the fact that we were able to read here means the file was closed
     messages = list(logfire.load_spans_from_file(path))
 
     parsed = [json.loads(MessageToJson(message)) for message in messages]
 
-    # insert_assert(parsed)
-    assert parsed == [
-        {
-            'resourceSpans': [
-                {
-                    'resource': {
-                        'attributes': [
-                            {'key': 'telemetry.sdk.language', 'value': {'stringValue': 'python'}},
-                            {'key': 'telemetry.sdk.name', 'value': {'stringValue': 'opentelemetry'}},
-                            {'key': 'telemetry.sdk.version', 'value': {'stringValue': '1.0.0'}},
-                            {'key': 'service.name', 'value': {'stringValue': 'test'}},
-                        ]
-                    },
-                    'scopeSpans': [
-                        {
-                            'scope': {'name': 'test'},
-                            'spans': [
-                                {
-                                    'traceId': 'AAAAAAAAAAAAAAAAAAAAAQ==',
-                                    'spanId': 'AAAAAAAAAAE=',
-                                    'name': 'test',
-                                    'kind': 'SPAN_KIND_INTERNAL',
-                                    'endTimeUnixNano': '1',
-                                    'status': {'code': 'STATUS_CODE_OK'},
-                                }
-                            ],
-                        }
-                    ],
-                }
-            ]
-        }
-    ]
-
-
-def test_dont_close_open_file(tmp_path: str) -> None:
-    path = Path(tmp_path) / 'spans.log'
-
-    with open(path, 'wb+') as file:
-        exporter = FileSpanExporter(file)
-
-        exporter.export([TEST_SPAN])
-
-        exporter.shutdown()
-
-        assert path.exists()
-
-        file.seek(0)
-
-        messages = list(logfire.load_spans_from_file(file))
-
-        parsed = [json.loads(MessageToJson(message)) for message in messages]
-
-        # insert_assert(parsed)
-        assert parsed == [
+    assert parsed == snapshot(
+        [
             {
                 'resourceSpans': [
                     {
                         'resource': {
                             'attributes': [
                                 {'key': 'telemetry.sdk.language', 'value': {'stringValue': 'python'}},
                                 {'key': 'telemetry.sdk.name', 'value': {'stringValue': 'opentelemetry'}},
@@ -131,14 +80,68 @@
                                 ],
                             }
                         ],
                     }
                 ]
             }
         ]
+    )
+
+
+def test_dont_close_open_file(tmp_path: str) -> None:
+    path = Path(tmp_path) / 'spans.log'
+
+    with open(path, 'wb+') as file:
+        exporter = FileSpanExporter(file)
+
+        exporter.export([TEST_SPAN])
+
+        exporter.shutdown()
+
+        assert path.exists()
+
+        file.seek(0)
+
+        messages = list(logfire.load_spans_from_file(file))
+
+        parsed = [json.loads(MessageToJson(message)) for message in messages]
+
+        assert parsed == snapshot(
+            [
+                {
+                    'resourceSpans': [
+                        {
+                            'resource': {
+                                'attributes': [
+                                    {'key': 'telemetry.sdk.language', 'value': {'stringValue': 'python'}},
+                                    {'key': 'telemetry.sdk.name', 'value': {'stringValue': 'opentelemetry'}},
+                                    {'key': 'telemetry.sdk.version', 'value': {'stringValue': '1.0.0'}},
+                                    {'key': 'service.name', 'value': {'stringValue': 'test'}},
+                                ]
+                            },
+                            'scopeSpans': [
+                                {
+                                    'scope': {'name': 'test'},
+                                    'spans': [
+                                        {
+                                            'traceId': 'AAAAAAAAAAAAAAAAAAAAAQ==',
+                                            'spanId': 'AAAAAAAAAAE=',
+                                            'name': 'test',
+                                            'kind': 'SPAN_KIND_INTERNAL',
+                                            'endTimeUnixNano': '1',
+                                            'status': {'code': 'STATUS_CODE_OK'},
+                                        }
+                                    ],
+                                }
+                            ],
+                        }
+                    ]
+                }
+            ]
+        )
 
 
 def test_export_existing_file(tmp_path: str) -> None:
     path = Path(tmp_path) / 'spans.log'
 
     exporter = FileSpanExporter(path)
     exporter.shutdown()
@@ -153,68 +156,69 @@
 
     assert path.exists()
 
     messages = list(logfire.load_spans_from_file(path))
 
     parsed = [json.loads(MessageToJson(message)) for message in messages]
 
-    # insert_assert(parsed)
-    assert parsed == [
-        {
-            'resourceSpans': [
-                {
-                    'resource': {
-                        'attributes': [
-                            {'key': 'telemetry.sdk.language', 'value': {'stringValue': 'python'}},
-                            {'key': 'telemetry.sdk.name', 'value': {'stringValue': 'opentelemetry'}},
-                            {'key': 'telemetry.sdk.version', 'value': {'stringValue': '1.0.0'}},
-                            {'key': 'service.name', 'value': {'stringValue': 'test'}},
-                        ]
-                    },
-                    'scopeSpans': [
-                        {
-                            'scope': {'name': 'test'},
-                            'spans': [
-                                {
-                                    'traceId': 'AAAAAAAAAAAAAAAAAAAAAQ==',
-                                    'spanId': 'AAAAAAAAAAE=',
-                                    'name': 'test',
-                                    'kind': 'SPAN_KIND_INTERNAL',
-                                    'endTimeUnixNano': '1',
-                                    'status': {'code': 'STATUS_CODE_OK'},
-                                }
-                            ],
-                        }
-                    ],
-                }
-            ]
-        },
-        {
-            'resourceSpans': [
-                {
-                    'resource': {
-                        'attributes': [
-                            {'key': 'telemetry.sdk.language', 'value': {'stringValue': 'python'}},
-                            {'key': 'telemetry.sdk.name', 'value': {'stringValue': 'opentelemetry'}},
-                            {'key': 'telemetry.sdk.version', 'value': {'stringValue': '1.0.0'}},
-                            {'key': 'service.name', 'value': {'stringValue': 'test'}},
-                        ]
-                    },
-                    'scopeSpans': [
-                        {
-                            'scope': {'name': 'test'},
-                            'spans': [
-                                {
-                                    'traceId': 'AAAAAAAAAAAAAAAAAAAAAQ==',
-                                    'spanId': 'AAAAAAAAAAE=',
-                                    'name': 'test',
-                                    'kind': 'SPAN_KIND_INTERNAL',
-                                    'endTimeUnixNano': '1',
-                                    'status': {'code': 'STATUS_CODE_OK'},
-                                }
-                            ],
-                        }
-                    ],
-                }
-            ]
-        },
-    ]
+    assert parsed == snapshot(
+        [
+            {
+                'resourceSpans': [
+                    {
+                        'resource': {
+                            'attributes': [
+                                {'key': 'telemetry.sdk.language', 'value': {'stringValue': 'python'}},
+                                {'key': 'telemetry.sdk.name', 'value': {'stringValue': 'opentelemetry'}},
+                                {'key': 'telemetry.sdk.version', 'value': {'stringValue': '1.0.0'}},
+                                {'key': 'service.name', 'value': {'stringValue': 'test'}},
+                            ]
+                        },
+                        'scopeSpans': [
+                            {
+                                'scope': {'name': 'test'},
+                                'spans': [
+                                    {
+                                        'traceId': 'AAAAAAAAAAAAAAAAAAAAAQ==',
+                                        'spanId': 'AAAAAAAAAAE=',
+                                        'name': 'test',
+                                        'kind': 'SPAN_KIND_INTERNAL',
+                                        'endTimeUnixNano': '1',
+                                        'status': {'code': 'STATUS_CODE_OK'},
+                                    }
+                                ],
+                            }
+                        ],
+                    }
+                ]
+            },
+            {
+                'resourceSpans': [
+                    {
+                        'resource': {
+                            'attributes': [
+                                {'key': 'telemetry.sdk.language', 'value': {'stringValue': 'python'}},
+                                {'key': 'telemetry.sdk.name', 'value': {'stringValue': 'opentelemetry'}},
+                                {'key': 'telemetry.sdk.version', 'value': {'stringValue': '1.0.0'}},
+                                {'key': 'service.name', 'value': {'stringValue': 'test'}},
+                            ]
+                        },
+                        'scopeSpans': [
+                            {
+                                'scope': {'name': 'test'},
+                                'spans': [
+                                    {
+                                        'traceId': 'AAAAAAAAAAAAAAAAAAAAAQ==',
+                                        'spanId': 'AAAAAAAAAAE=',
+                                        'name': 'test',
+                                        'kind': 'SPAN_KIND_INTERNAL',
+                                        'endTimeUnixNano': '1',
+                                        'status': {'code': 'STATUS_CODE_OK'},
+                                    }
+                                ],
+                            }
+                        ],
+                    }
+                ]
+            },
+        ]
+    )
```

### Comparing `logfire-0.30.0/tests/exporters/test_otlp_session.py` & `logfire-0.31.0/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/exporters/test_remove_pending.py` & `logfire-0.31.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.31.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.31.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/test_asgi.py` & `logfire-0.31.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/test_asyncpg.py` & `logfire-0.31.0/tests/otel_integrations/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/test_django.py` & `logfire-0.31.0/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/test_fastapi.py` & `logfire-0.31.0/tests/otel_integrations/test_fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
+import importlib
 import os
 from typing import Any
+from unittest import mock
 
 import pytest
 from dirty_equals import IsJson
 from fastapi import BackgroundTasks, FastAPI, Response, WebSocket
 from fastapi.exceptions import RequestValidationError
 from fastapi.params import Header
 from fastapi.security import SecurityScopes
@@ -13,17 +15,31 @@
 from opentelemetry.propagate import inject
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse
 from starlette.testclient import TestClient
 from typing_extensions import Annotated
 
 import logfire
+import logfire._internal
+import logfire._internal.integrations
+import logfire._internal.integrations.fastapi
 from logfire.testing import TestExporter
 
 
+def test_missing_opentelemetry_dependency() -> None:
+    with mock.patch.dict('sys.modules', {'opentelemetry.instrumentation.fastapi': None}):
+        with pytest.raises(RuntimeError) as exc_info:
+            importlib.reload(logfire._internal.integrations.fastapi)
+        assert str(exc_info.value) == snapshot("""\
+The `logfire.instrument_fastapi()` requires the `opentelemetry-instrumentation-fastapi` package.
+You can install this with:
+    pip install 'logfire[fastapi]'\
+""")
+
+
 async def homepage() -> PlainTextResponse:
     logfire.info('inside request handler')
     return PlainTextResponse('middleware test')
 
 
 async def other_route(
     foo: str,
@@ -523,17 +539,14 @@
                 'end_time': 2000000000,
                 'attributes': {
                     'custom_attr': 'custom_value',
                     'logfire.span_type': 'log',
                     'logfire.level_num': 17,
                     'logfire.msg_template': 'FastAPI arguments',
                     'logfire.msg': 'FastAPI arguments',
-                    'code.filepath': 'fastapi.py',
-                    'code.function': 'solve_dependencies',
-                    'code.lineno': 123,
                     'values': '{"foo":"foo_val"}',
                     'errors': '[{"type":"int_parsing","loc":["query","bar"],"msg":"Input should be a valid integer, unable to parse string as an integer","input":"bar_val"}]',
                     'http.method': 'GET',
                     'http.route': '/other',
                     'fastapi.route.name': 'other_route_name',
                     'fastapi.route.operation_id': 'other_route_operation_id',
                     'logfire.json_schema': IsJson(
@@ -805,17 +818,14 @@
                 'start_time': 2000000000,
                 'end_time': 2000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
                     'logfire.level_num': 5,
                     'logfire.msg_template': 'FastAPI arguments',
                     'logfire.msg': 'FastAPI arguments',
-                    'code.filepath': 'fastapi.py',
-                    'code.function': 'solve_dependencies',
-                    'code.lineno': 123,
                     'values': '{"path_param": "[Redacted due to \'auth\']", "foo": "foo_val", "password": "[Redacted due to \'password\']", "testauthorization": "[Redacted due to \'auth\']"}',
                     'errors': '[]',
                     'custom_attr': 'custom_value',
                     'http.method': 'GET',
                     'http.route': '/secret/{path_param}',
                     'fastapi.route.name': 'secret',
                     'logfire.null_args': ('fastapi.route.operation_id',),
```

### Comparing `logfire-0.30.0/tests/otel_integrations/test_flask.py` & `logfire-0.31.0/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/test_httpx.py` & `logfire-0.31.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/test_openai.py` & `logfire-0.31.0/tests/otel_integrations/test_openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -227,16 +227,16 @@
             {
                 'name': 'Chat Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_sync_chat_completions',
                     'code.lineno': 123,
                     'request_data': IsJson(
                         {
                             'messages': [
                                 {'role': 'system', 'content': 'You are a helpful assistant.'},
                                 {'role': 'user', 'content': 'What is four plus five?'},
                             ],
@@ -302,16 +302,16 @@
             {
                 'name': 'Chat Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_async_chat_completions',
                     'code.lineno': 123,
                     'request_data': IsJson(
                         {
                             'messages': [
                                 {'role': 'system', 'content': 'You are a helpful assistant.'},
                                 {'role': 'user', 'content': 'What is four plus five?'},
                             ],
@@ -376,16 +376,16 @@
             {
                 'name': 'Chat Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_sync_chat_empty_response_chunk',
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"empty response chunk"}],"model":"gpt-4","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
@@ -394,21 +394,21 @@
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
                 'end_time': 5000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
                     'logfire.level_num': 9,
-                    'code.function': 'record_streaming',
-                    'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"empty response chunk"}],"model":"gpt-4","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_sync_chat_empty_response_chunk',
+                    'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"","chunk_count":0}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
@@ -430,16 +430,16 @@
             {
                 'name': 'Chat Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_sync_chat_empty_response_choices',
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"empty choices in response chunk"}],"model":"gpt-4","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
@@ -448,21 +448,21 @@
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
                 'end_time': 5000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
                     'logfire.level_num': 9,
-                    'code.function': 'record_streaming',
-                    'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"empty choices in response chunk"}],"model":"gpt-4","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_sync_chat_empty_response_choices',
+                    'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"","chunk_count":0}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
@@ -486,16 +486,16 @@
             {
                 'name': 'Chat Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_sync_chat_completions_stream',
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"You are a helpful assistant."},{"role":"user","content":"What is four plus five?"}],"model":"gpt-4","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
@@ -504,21 +504,21 @@
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
                 'end_time': 5000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
                     'logfire.level_num': 9,
-                    'code.function': 'record_streaming',
-                    'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"You are a helpful assistant."},{"role":"user","content":"What is four plus five?"}],"model":"gpt-4","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': '<genexpr>',
+                    'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"The answer is Nine","chunk_count":2}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
@@ -545,16 +545,16 @@
             {
                 'name': 'Chat Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_async_chat_completions_stream',
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"You are a helpful assistant."},{"role":"user","content":"What is four plus five?"}],"model":"gpt-4","stream":true}',
                     'async': True,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
@@ -563,21 +563,21 @@
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
                 'end_time': 5000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
                     'logfire.level_num': 9,
-                    'code.function': 'record_streaming',
-                    'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"You are a helpful assistant."},{"role":"user","content":"What is four plus five?"}],"model":"gpt-4","stream":true}',
                     'async': True,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_async_chat_completions_stream',
+                    'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"The answer is Nine","chunk_count":2}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
@@ -596,16 +596,16 @@
             {
                 'name': 'Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_completions',
                     'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"What is four plus five?"}',
                     'async': False,
                     'logfire.msg_template': 'Completion with {request_data[model]!r}',
                     'logfire.msg': "Completion with 'gpt-3.5-turbo-instruct'",
                     'logfire.span_type': 'span',
                     'response_data': '{"finish_reason":"stop","text":"Nine","usage":null}',
@@ -629,16 +629,16 @@
             {
                 'name': 'Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_completions_stream',
                     'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"What is four plus five?","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'Completion with {request_data[model]!r}',
                     'logfire.msg': "Completion with 'gpt-3.5-turbo-instruct'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
@@ -647,21 +647,21 @@
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
                 'end_time': 5000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
                     'logfire.level_num': 9,
-                    'code.function': 'record_streaming',
-                    'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"What is four plus five?","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': '<genexpr>',
+                    'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-3.5-turbo-instruct' took 1.00s",
                     'logfire.span_type': 'log',
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"The answer is Nine","chunk_count":3}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
@@ -680,16 +680,16 @@
             {
                 'name': 'Embedding Creation with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_embeddings',
                     'code.lineno': 123,
                     'request_data': '{"input":"This is a sentence to embed.","model":"text-embedding-3-small","encoding_format":"base64"}',
                     'async': False,
                     'logfire.msg_template': 'Embedding Creation with {request_data[model]!r}',
                     'logfire.msg': "Embedding Creation with 'text-embedding-3-small'",
                     'logfire.span_type': 'span',
                     'response_data': '{"usage":{"prompt_tokens":1,"total_tokens":2}}',
@@ -712,16 +712,16 @@
             {
                 'name': 'Image Generation with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_images',
                     'code.lineno': 123,
                     'request_data': '{"prompt":"A picture of a cat.","model":"dall-e-3"}',
                     'async': False,
                     'logfire.msg_template': 'Image Generation with {request_data[model]!r}',
                     'logfire.msg': "Image Generation with 'dall-e-3'",
                     'logfire.span_type': 'span',
                     'response_data': '{"images":[{"b64_json":null,"revised_prompt":"revised prompt","url":"https://example.com/image.jpg"}]}',
@@ -764,16 +764,16 @@
                 'name': 'Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 4000000000,
                 'instrumentation_scope': 'logfire.openai',
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_dont_suppress_httpx',
                     'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"xxx"}',
                     'async': False,
                     'logfire.msg_template': 'Completion with {request_data[model]!r}',
                     'logfire.msg': "Completion with 'gpt-3.5-turbo-instruct'",
                     'logfire.span_type': 'span',
                     'response_data': '{"finish_reason":"stop","text":"Nine","usage":null}',
@@ -800,16 +800,16 @@
                 'name': 'Completion with {request_data[model]!r}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 2000000000,
                 'instrumentation_scope': 'logfire.openai',
                 'attributes': {
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_suppress_httpx',
                     'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"xxx"}',
                     'async': False,
                     'logfire.msg_template': 'Completion with {request_data[model]!r}',
                     'logfire.msg': "Completion with 'gpt-3.5-turbo-instruct'",
                     'logfire.span_type': 'span',
                     'response_data': '{"finish_reason":"stop","text":"Nine","usage":null}',
@@ -856,16 +856,16 @@
                 'start_time': 1000000000,
                 'end_time': 1000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
                     'logfire.level_num': 13,
                     'logfire.msg_template': 'Unable to instrument OpenAI API call: {error}',
                     'logfire.msg': 'Unable to instrument OpenAI API call: `model` not found in request data',
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_unknown_method',
                     'code.lineno': 123,
                     'error': '`model` not found in request data',
                     'kwargs': IsStr(),
                     'logfire.json_schema': IsStr(),
                 },
             }
         ]
@@ -884,16 +884,16 @@
                 'start_time': 1000000000,
                 'end_time': 1000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
                     'logfire.level_num': 13,
                     'logfire.msg_template': 'Unable to instrument OpenAI API call: {error}',
                     'logfire.msg': 'Unable to instrument OpenAI API call: `model` not found in request data',
-                    'code.filepath': 'openai.py',
-                    'code.function': 'instrumented_openai_request',
+                    'code.filepath': 'test_openai.py',
+                    'code.function': 'test_async_unknown_method',
                     'code.lineno': 123,
                     'error': '`model` not found in request data',
                     'kwargs': IsStr(),
                     'logfire.json_schema': IsStr(),
                 },
             }
         ]
```

### Comparing `logfire-0.30.0/tests/otel_integrations/test_psycopg.py` & `logfire-0.31.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/test_requests.py` & `logfire-0.31.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.31.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Iterator
 
+from inline_snapshot import snapshot
 from sqlalchemy.engine import Engine, create_engine
 from sqlalchemy.orm import DeclarativeBase, Mapped, Session, mapped_column
 from sqlalchemy.sql import text
 from sqlalchemy.types import Integer, String
 
 from logfire.testing import TestExporter
 
@@ -44,149 +45,150 @@
             record = AuthRecord(id=1, number=2, content='abc')
             session.execute(text('select * from auth_records'))
             session.add(record)
             session.commit()
             session.delete(record)
             session.commit()
 
-    # insert_assert(exporter.exported_spans_as_dict())
-    assert exporter.exported_spans_as_dict() == [
-        {
-            'name': 'connect',
-            'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-            'parent': None,
-            'start_time': 1000000000,
-            'end_time': 2000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'connect',
-                'db.name': 'example.db',
-                'db.system': 'sqlite',
-            },
-        },
-        {
-            'name': 'PRAGMA example.db',
-            'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
-            'parent': None,
-            'start_time': 3000000000,
-            'end_time': 4000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'PRAGMA example.db',
-                'db.statement': 'PRAGMA main.table_info("auth_records")',
-                'db.system': 'sqlite',
-                'db.name': 'example.db',
-            },
-        },
-        {
-            'name': 'PRAGMA example.db',
-            'context': {'trace_id': 3, 'span_id': 5, 'is_remote': False},
-            'parent': None,
-            'start_time': 5000000000,
-            'end_time': 6000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'PRAGMA example.db',
-                'db.statement': 'PRAGMA temp.table_info("auth_records")',
-                'db.system': 'sqlite',
-                'db.name': 'example.db',
-            },
-        },
-        {
-            'name': 'CREATE example.db',
-            'context': {'trace_id': 4, 'span_id': 7, 'is_remote': False},
-            'parent': None,
-            'start_time': 7000000000,
-            'end_time': 8000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'CREATE example.db',
-                'db.statement': '\nCREATE TABLE auth_records (\n\tid INTEGER NOT NULL, \n\tnumber INTEGER NOT NULL, \n\tcontent VARCHAR NOT NULL, \n\tPRIMARY KEY (id)\n)\n\n',
-                'db.system': 'sqlite',
-                'db.name': 'example.db',
-            },
-        },
-        {
-            'name': 'connect',
-            'context': {'trace_id': 5, 'span_id': 9, 'is_remote': False},
-            'parent': None,
-            'start_time': 9000000000,
-            'end_time': 10000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'connect',
-                'db.name': 'example.db',
-                'db.system': 'sqlite',
-            },
-        },
-        {
-            'name': 'select example.db',
-            'context': {'trace_id': 6, 'span_id': 11, 'is_remote': False},
-            'parent': None,
-            'start_time': 11000000000,
-            'end_time': 12000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'select example.db',
-                'db.statement': 'select * from auth_records',
-                'db.system': 'sqlite',
-                'db.name': 'example.db',
-            },
-        },
-        {
-            'name': 'INSERT example.db',
-            'context': {'trace_id': 7, 'span_id': 13, 'is_remote': False},
-            'parent': None,
-            'start_time': 13000000000,
-            'end_time': 14000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'INSERT example.db',
-                'db.statement': 'INSERT INTO auth_records (id, number, content) VALUES (?, ?, ?)',
-                'db.system': 'sqlite',
-                'db.name': 'example.db',
-            },
-        },
-        {
-            'name': 'connect',
-            'context': {'trace_id': 8, 'span_id': 15, 'is_remote': False},
-            'parent': None,
-            'start_time': 15000000000,
-            'end_time': 16000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'connect',
-                'db.name': 'example.db',
-                'db.system': 'sqlite',
-            },
-        },
-        {
-            'name': 'SELECT example.db',
-            'context': {'trace_id': 9, 'span_id': 17, 'is_remote': False},
-            'parent': None,
-            'start_time': 17000000000,
-            'end_time': 18000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'SELECT example.db',
-                'db.statement': 'SELECT auth_records.id AS auth_records_id, auth_records.number AS auth_records_number, auth_records.content AS auth_records_content \nFROM auth_records \nWHERE auth_records.id = ?',
-                'db.system': 'sqlite',
-                'db.name': 'example.db',
-            },
-        },
-        {
-            'name': 'DELETE example.db',
-            'context': {'trace_id': 10, 'span_id': 19, 'is_remote': False},
-            'parent': None,
-            'start_time': 19000000000,
-            'end_time': 20000000000,
-            'attributes': {
-                'logfire.span_type': 'span',
-                'logfire.msg': 'DELETE example.db',
-                'db.statement': 'DELETE FROM auth_records WHERE auth_records.id = ?',
-                'db.system': 'sqlite',
-                'db.name': 'example.db',
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'connect',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'connect',
+                    'db.name': 'example.db',
+                    'db.system': 'sqlite',
+                },
+            },
+            {
+                'name': 'PRAGMA example.db',
+                'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
+                'parent': None,
+                'start_time': 3000000000,
+                'end_time': 4000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'PRAGMA example.db',
+                    'db.statement': 'PRAGMA main.table_info("auth_records")',
+                    'db.system': 'sqlite',
+                    'db.name': 'example.db',
+                },
+            },
+            {
+                'name': 'PRAGMA example.db',
+                'context': {'trace_id': 3, 'span_id': 5, 'is_remote': False},
+                'parent': None,
+                'start_time': 5000000000,
+                'end_time': 6000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'PRAGMA example.db',
+                    'db.statement': 'PRAGMA temp.table_info("auth_records")',
+                    'db.system': 'sqlite',
+                    'db.name': 'example.db',
+                },
+            },
+            {
+                'name': 'CREATE example.db',
+                'context': {'trace_id': 4, 'span_id': 7, 'is_remote': False},
+                'parent': None,
+                'start_time': 7000000000,
+                'end_time': 8000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'CREATE example.db',
+                    'db.statement': '\nCREATE TABLE auth_records (\n\tid INTEGER NOT NULL, \n\tnumber INTEGER NOT NULL, \n\tcontent VARCHAR NOT NULL, \n\tPRIMARY KEY (id)\n)\n\n',
+                    'db.system': 'sqlite',
+                    'db.name': 'example.db',
+                },
+            },
+            {
+                'name': 'connect',
+                'context': {'trace_id': 5, 'span_id': 9, 'is_remote': False},
+                'parent': None,
+                'start_time': 9000000000,
+                'end_time': 10000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'connect',
+                    'db.name': 'example.db',
+                    'db.system': 'sqlite',
+                },
+            },
+            {
+                'name': 'select example.db',
+                'context': {'trace_id': 6, 'span_id': 11, 'is_remote': False},
+                'parent': None,
+                'start_time': 11000000000,
+                'end_time': 12000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'select example.db',
+                    'db.statement': 'select * from auth_records',
+                    'db.system': 'sqlite',
+                    'db.name': 'example.db',
+                },
+            },
+            {
+                'name': 'INSERT example.db',
+                'context': {'trace_id': 7, 'span_id': 13, 'is_remote': False},
+                'parent': None,
+                'start_time': 13000000000,
+                'end_time': 14000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'INSERT example.db',
+                    'db.statement': 'INSERT INTO auth_records (id, number, content) VALUES (?, ?, ?)',
+                    'db.system': 'sqlite',
+                    'db.name': 'example.db',
+                },
+            },
+            {
+                'name': 'connect',
+                'context': {'trace_id': 8, 'span_id': 15, 'is_remote': False},
+                'parent': None,
+                'start_time': 15000000000,
+                'end_time': 16000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'connect',
+                    'db.name': 'example.db',
+                    'db.system': 'sqlite',
+                },
+            },
+            {
+                'name': 'SELECT example.db',
+                'context': {'trace_id': 9, 'span_id': 17, 'is_remote': False},
+                'parent': None,
+                'start_time': 17000000000,
+                'end_time': 18000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'SELECT example.db',
+                    'db.statement': 'SELECT auth_records.id AS auth_records_id, auth_records.number AS auth_records_number, auth_records.content AS auth_records_content \nFROM auth_records \nWHERE auth_records.id = ?',
+                    'db.system': 'sqlite',
+                    'db.name': 'example.db',
+                },
+            },
+            {
+                'name': 'DELETE example.db',
+                'context': {'trace_id': 10, 'span_id': 19, 'is_remote': False},
+                'parent': None,
+                'start_time': 19000000000,
+                'end_time': 20000000000,
+                'attributes': {
+                    'logfire.span_type': 'span',
+                    'logfire.msg': 'DELETE example.db',
+                    'db.statement': 'DELETE FROM auth_records WHERE auth_records.id = ?',
+                    'db.system': 'sqlite',
+                    'db.name': 'example.db',
+                },
             },
-        },
-    ]
+        ]
+    )
 
     SQLAlchemyInstrumentor().uninstrument()  # type: ignore[reportUnknownMemberType]
```

### Comparing `logfire-0.30.0/tests/otel_integrations/test_starlette.py` & `logfire-0.31.0/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/test_wsgi.py` & `logfire-0.31.0/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.31.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.31.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/LICENSE` & `logfire-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.30.0/README.md` & `logfire-0.31.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 logfire.info('Hello, {name}!', name='world')
 
 with logfire.span('Asking the user their {question}', question='age'):
     user_input = input('How old are you [YYYY-mm-dd]? ')
     dob = date.fromisoformat(user_input)
     logfire.debug('{dob=} {age=!r}', dob=dob, age=date.today() - dob)
 ```
-[_(learn more)_](https://docs.pydantic.dev/logfire/guides/onboarding_checklist/03_add_manual_tracing/)
+[_(learn more)_](https://docs.pydantic.dev/logfire/guides/onboarding_checklist/add_manual_tracing/)
 
 ### Integration
 
 Or you can also avoid manual instrumentation and instead integrate with [lots of popular packages](https://docs.pydantic.dev/logfire/integrations/), here's an example of integrating with FastAPI:
 
 ```py
 import logfire
@@ -86,12 +86,12 @@
 
 Logfire gives you a view into how your code is running like this:
 
 ![Logfire screenshot](https://docs.pydantic.dev/logfire/images/index/logfire-screenshot-fastapi-200.png)
 
 ## Contributing
 
-We'd love anyone interested to contribute to the Logfire SDK and documentation, see the [contributing guide](./CONTRIBUTING.md).
+We'd love anyone interested to contribute to the Logfire SDK and documentation, see the [contributing guide](https://github.com/pydantic/logfire/blob/main/CONTRIBUTING.md).
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/logfire/security).
```

### Comparing `logfire-0.30.0/pyproject.toml` & `logfire-0.31.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.30.0"
+version = "0.31.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
@@ -43,14 +43,15 @@
     "opentelemetry-sdk >= 1.21.0",
     "opentelemetry-exporter-otlp-proto-http >= 1.21.0",
     "opentelemetry-instrumentation >= 0.41b0",
     "rich >= 13.4.2",
     "protobuf >= 4.23.4",
     "typing-extensions >= 4.1.0",
     "tomli >= 2.0.1; python_version < '3.11'",
+    "executing>=2.0.1",
 ]
 
 [project.optional-dependencies]
 system-metrics = ["opentelemetry-instrumentation-system-metrics >= 0.42b0"]
 aiohttp = ["opentelemetry-instrumentation-aiohttp-client >= 0.42b0"]
 celery = ["opentelemetry-instrumentation-celery >= 0.42b0"]
 django = ["opentelemetry-instrumentation-django >= 0.42b0"]
@@ -105,23 +106,22 @@
     "opentelemetry-instrumentation-requests",
     "opentelemetry-instrumentation-sqlalchemy",
     "opentelemetry-instrumentation-system-metrics",
     "opentelemetry-instrumentation-asyncpg",
     "opentelemetry-instrumentation-psycopg",
     "opentelemetry-instrumentation-psycopg2",
     "gitpython",
-    "devtools",
     "eval-type-backport",
     "requests-mock",
     "inline-snapshot",
     "structlog",
     "loguru",
     "ruff",
     "pyright>=1.1.360",
-    "pre-commit>=3.7.0",
+    "pre-commit>=3.5.0",
     "mkdocs>=1.5.0",
     "mkdocs-material>=9.5.17",
     "mkdocs-glightbox>=0.3.7",
     "mkdocstrings-python>=1.8.0",
     "coverage[toml]>=7.5.0",
     "psycopg[binary]",
     "psycopg2-binary",
@@ -180,15 +180,15 @@
 docstring-code-format = true
 quote-style = "single"
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportUnnecessaryTypeIgnoreComment = true
 reportMissingTypeStubs = false
-exclude = ["docs/**/*.py", "site/**/*.py", ".venv"]
+exclude = ["docs/**/*.py", "site/**/*.py", ".venv", "venv*"]
 venvPath = ".venv"
 
 [tool.pytest.ini_options]
 xfail_strict = true
 filterwarnings = [
     "error",
     # fastapi uses deprecated pydantic functions
```

### Comparing `logfire-0.30.0/PKG-INFO` & `logfire-0.31.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.30.0
+Version: 0.31.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: executing>=2.0.1
 Requires-Dist: opentelemetry-exporter-otlp-proto-http>=1.21.0
 Requires-Dist: opentelemetry-instrumentation>=0.41b0
 Requires-Dist: opentelemetry-sdk>=1.21.0
 Requires-Dist: protobuf>=4.23.4
 Requires-Dist: rich>=13.4.2
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Requires-Dist: typing-extensions>=4.1.0
@@ -119,15 +120,15 @@
 logfire.info('Hello, {name}!', name='world')
 
 with logfire.span('Asking the user their {question}', question='age'):
     user_input = input('How old are you [YYYY-mm-dd]? ')
     dob = date.fromisoformat(user_input)
     logfire.debug('{dob=} {age=!r}', dob=dob, age=date.today() - dob)
 ```
-[_(learn more)_](https://docs.pydantic.dev/logfire/guides/onboarding_checklist/03_add_manual_tracing/)
+[_(learn more)_](https://docs.pydantic.dev/logfire/guides/onboarding_checklist/add_manual_tracing/)
 
 ### Integration
 
 Or you can also avoid manual instrumentation and instead integrate with [lots of popular packages](https://docs.pydantic.dev/logfire/integrations/), here's an example of integrating with FastAPI:
 
 ```py
 import logfire
@@ -153,12 +154,12 @@
 
 Logfire gives you a view into how your code is running like this:
 
 ![Logfire screenshot](https://docs.pydantic.dev/logfire/images/index/logfire-screenshot-fastapi-200.png)
 
 ## Contributing
 
-We'd love anyone interested to contribute to the Logfire SDK and documentation, see the [contributing guide](./CONTRIBUTING.md).
+We'd love anyone interested to contribute to the Logfire SDK and documentation, see the [contributing guide](https://github.com/pydantic/logfire/blob/main/CONTRIBUTING.md).
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/logfire/security).
```

