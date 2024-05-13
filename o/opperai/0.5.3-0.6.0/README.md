# Comparing `tmp/opperai-0.5.3.tar.gz` & `tmp/opperai-0.6.0.tar.gz`

## Comparing `opperai-0.5.3.tar` & `opperai-0.6.0.tar`

### file list

```diff
@@ -1,88 +1,92 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.5.3/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.5.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/__init__.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/_client.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/functions/__init__.py
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/functions/_async_functions.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/indexes/__init__.py
--rw-r--r--   0        0        0    12400 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/indexes/_async_indexes.py
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/spans/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/spans/_async_spans.py
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/spans/_decorator.py
--rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/spans/_spans.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/utils/__init__.py
--rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/async_functions.py
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/decorator/__init__.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/decorator/_schemas.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/indexes/async_indexes.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/indexes/indexes.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/spans/async_spans.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/spans/spans.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/validators.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/conftest.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_async_functions.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_async_indexes.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_async_spans.py
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_fn_decorator.py
--rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_functions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_indexes.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_spans.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_types.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.5.3/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.5.3/LICENSE
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 opperai-0.5.3/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 opperai-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.6.0/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/__init__.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/_client.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/functions/__init__.py
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/functions/_async_functions.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/indexes/__init__.py
+-rw-r--r--   0        0        0    12400 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/indexes/_async_indexes.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/spans/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/spans/_async_spans.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/spans/_decorator.py
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/spans/_spans.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/core/utils/__init__.py
+-rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/async_functions.py
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/indexes/async_indexes.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/indexes/indexes.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/spans/async_spans.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/spans/spans.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.6.0/src/opperai/types/validators.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_async_spans.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_fn_decorator.py
+-rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_indexes.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/test_types.py
+-rw-r--r--   0        0        0   173874 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/images/fossil.jpg
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0   236306 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_file.yaml
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_image_url.yaml
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0   237017 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_image_file.yaml
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_image_url.yaml
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.6.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 opperai-0.6.0/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 opperai-0.6.0/PKG-INFO
```

### Comparing `opperai-0.5.3/.github/workflows/publish.yml` & `opperai-0.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/__init__.py` & `opperai-0.6.0/src/opperai/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/_client.py` & `opperai-0.6.0/src/opperai/_client.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/core/_http_clients.py` & `opperai-0.6.0/src/opperai/core/_http_clients.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/core/functions/_async_functions.py` & `opperai-0.6.0/src/opperai/core/functions/_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/core/functions/_functions.py` & `opperai-0.6.0/src/opperai/core/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/core/indexes/_async_indexes.py` & `opperai-0.6.0/src/opperai/core/indexes/_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/core/indexes/_indexes.py` & `opperai-0.6.0/src/opperai/core/indexes/_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/core/spans/_async_spans.py` & `opperai-0.6.0/src/opperai/core/spans/_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/core/spans/_decorator.py` & `opperai-0.6.0/src/opperai/core/spans/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/core/spans/_spans.py` & `opperai-0.6.0/src/opperai/core/spans/_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/core/utils/__init__.py` & `opperai-0.6.0/src/opperai/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/functions/async_functions.py` & `opperai-0.6.0/src/opperai/functions/async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/functions/functions.py` & `opperai-0.6.0/src/opperai/functions/functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/functions/decorator/_decorator.py` & `opperai-0.6.0/src/opperai/functions/decorator/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/functions/decorator/_schemas.py` & `opperai-0.6.0/src/opperai/functions/decorator/_schemas.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/indexes/async_indexes.py` & `opperai-0.6.0/src/opperai/indexes/async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/indexes/indexes.py` & `opperai-0.6.0/src/opperai/indexes/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/spans/async_spans.py` & `opperai-0.6.0/src/opperai/spans/async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/spans/spans.py` & `opperai-0.6.0/src/opperai/spans/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/types/indexes.py` & `opperai-0.6.0/src/opperai/types/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/types/spans.py` & `opperai-0.6.0/src/opperai/types/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/src/opperai/types/validators.py` & `opperai-0.6.0/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/conftest.py` & `opperai-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/test_async_functions.py` & `opperai-0.6.0/tests/test_async_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+from contextlib import asynccontextmanager
+
 import pytest
 from opperai import AsyncClient
-from opperai.types import CacheConfiguration, ChatPayload, Function, Message
+from opperai.types import (
+    CacheConfiguration,
+    ChatPayload,
+    Function,
+    Message,
+    MessageContent,
+)
 from opperai.types.exceptions import StructuredGenerationError
-from contextlib import asynccontextmanager
 
 
 @asynccontextmanager
 async def _function(desc: Function, c: AsyncClient):
     function = await c.functions.create(desc)
     yield function
     await c.functions.delete(id=function.id)
@@ -97,14 +104,74 @@
     )
     await aclient.functions.delete(id=function.id)
     f = await aclient.functions.get(id=function.id)
     assert f is None
 
 
 @pytest.mark.asyncio(scope="module")
+async def test_image_url(aclient: AsyncClient, vcr_cassette):
+    async with _function(
+        Function(
+            path="test/sdk/test_image",
+            instructions="describe the image",
+            model="openai/gpt4-turbo",
+        ),
+        aclient,
+    ) as function:
+        f = await aclient.functions.get(id=function.id)
+        resp = await aclient.functions.chat(
+            f.path,
+            ChatPayload(
+                messages=[
+                    Message(
+                        role="user",
+                        content=[
+                            MessageContent.image_url(
+                                url="https://tf-cmsv2-smithsonianmag-media.s3.amazonaws.com/filer/e1/d3/e1d3fee9-9aaa-4599-ba67-1c71a6d0ed03/1200px-seymouria_fossil.jpg"
+                            )
+                        ],
+                    )
+                ]
+            ),
+        )
+
+        assert "fossil" in resp.message.lower()
+
+
+@pytest.mark.asyncio(scope="module")
+async def test_image_file(aclient: AsyncClient, vcr_cassette):
+    async with _function(
+        Function(
+            path="test/sdk/test_image",
+            instructions="describe the image",
+            model="openai/gpt4-turbo",
+        ),
+        aclient,
+    ) as function:
+        f = await aclient.functions.get(id=function.id)
+        resp = await aclient.functions.chat(
+            f.path,
+            ChatPayload(
+                messages=[
+                    Message(
+                        role="user",
+                        content=[
+                            MessageContent.image(
+                                path="tests/fixtures/images/fossil.jpg"
+                            )
+                        ],
+                    )
+                ]
+            ),
+        )
+
+        assert "fossil" in resp.message.lower()
+
+
+@pytest.mark.asyncio(scope="module")
 async def test_async_chat(aclient: AsyncClient, vcr_cassette):
     async with _function(
         Function(
             path="test/sdk/test_async_chat",
             description="Translate to French",
             instructions="Translate to French",
         ),
```

### Comparing `opperai-0.5.3/tests/test_async_indexes.py` & `opperai-0.6.0/tests/test_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/test_async_spans.py` & `opperai-0.6.0/tests/test_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/test_fn_decorator.py` & `opperai-0.6.0/tests/test_fn_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/test_functions.py` & `opperai-0.6.0/tests/test_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from contextlib import contextmanager
 
 import pytest
 from opperai import Client
-from opperai.types import CacheConfiguration, ChatPayload, Function, Message
+from opperai.types import (
+    CacheConfiguration,
+    ChatPayload,
+    Function,
+    Message,
+    MessageContent,
+)
 from opperai.types.exceptions import StructuredGenerationError
 
 
 @contextmanager
 def _function(desc: Function, c: Client):
     function = c.functions.create(desc)
     yield function
@@ -92,14 +98,72 @@
     )
     assert function is not None
     client.functions.delete(path=function.path)
     f = client.functions.get(path=function.path)
     assert f is None
 
 
+def test_image_url(client: Client, vcr_cassette):
+    with _function(
+        Function(
+            path="test/sdk/test_image",
+            instructions="describe the image",
+            model="openai/gpt4-turbo",
+        ),
+        client,
+    ) as function:
+        f = client.functions.get(id=function.id)
+        resp = client.functions.chat(
+            f.path,
+            ChatPayload(
+                messages=[
+                    Message(
+                        role="user",
+                        content=[
+                            MessageContent.image_url(
+                                url="https://tf-cmsv2-smithsonianmag-media.s3.amazonaws.com/filer/e1/d3/e1d3fee9-9aaa-4599-ba67-1c71a6d0ed03/1200px-seymouria_fossil.jpg"
+                            )
+                        ],
+                    )
+                ]
+            ),
+        )
+
+        assert "fossil" in resp.message.lower()
+
+
+def test_image_file(client: Client, vcr_cassette):
+    with _function(
+        Function(
+            path="test/sdk/test_image",
+            instructions="describe the image",
+            model="openai/gpt4-turbo",
+        ),
+        client,
+    ) as function:
+        f = client.functions.get(id=function.id)
+        resp = client.functions.chat(
+            f.path,
+            ChatPayload(
+                messages=[
+                    Message(
+                        role="user",
+                        content=[
+                            MessageContent.image(
+                                path="tests/fixtures/images/fossil.jpg"
+                            )
+                        ],
+                    )
+                ]
+            ),
+        )
+
+        assert "fossil" in resp.message.lower()
+
+
 def test_chat(client: Client, vcr_cassette):
     with _function(
         Function(
             path="test/sdk/test_chat",
             description="Translate to French",
             instructions="Translate to French",
         ),
```

### Comparing `opperai-0.5.3/tests/test_indexes.py` & `opperai-0.6.0/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/test_trace_decorator.py` & `opperai-0.6.0/tests/test_trace_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/test_types.py` & `opperai-0.6.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml` & `opperai-0.6.0/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/LICENSE` & `opperai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opperai-0.5.3/README.md` & `opperai-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Opper Python SDK
 
+This is the Opper Python SDK. See below for getting started, and the [docs](https://docs.opper.ai) for more information. The SDK has builtin documentation and examples in function docstrings, which should be visible in your code editor as you are using the functions.
+
 ## Install
 
 ```bash
 pip install opperai
 ```
 
 ## Configuration
```

### Comparing `opperai-0.5.3/pyproject.toml` & `opperai-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.5.3"
+version = "0.6.0"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `opperai-0.5.3/PKG-INFO` & `opperai-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.5.3
+Version: 0.6.0
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,16 @@
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: vcrpy; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Opper Python SDK
 
+This is the Opper Python SDK. See below for getting started, and the [docs](https://docs.opper.ai) for more information. The SDK has builtin documentation and examples in function docstrings, which should be visible in your code editor as you are using the functions.
+
 ## Install
 
 ```bash
 pip install opperai
 ```
 
 ## Configuration
```

