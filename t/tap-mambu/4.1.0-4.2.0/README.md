# Comparing `tmp/tap-mambu-4.1.0.tar.gz` & `tmp/tap-mambu-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mambu-4.1.0.tar", last modified: Tue Feb 20 11:28:21 2024, max compression
+gzip compressed data, was "tap-mambu-4.2.0.tar", last modified: Mon May 13 12:37:13 2024, max compression
```

## Comparing `tap-mambu-4.1.0.tar` & `tap-mambu-4.2.0.tar`

### file list

```diff
@@ -1,161 +1,152 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.916558 tap-mambu-4.1.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       57 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      904 2024-02-20 11:28:21.916558 tap-mambu-4.1.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19063 2024-02-20 10:34:41.000000 tap-mambu-4.1.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.876557 tap-mambu-4.1.0/mambu_tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      953 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3873 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/helpers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.876557 tap-mambu-4.1.0/mambu_tests/multithreading/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/multithreading/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4418 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/multithreading/test_multithreaded_bookmark_daybyday_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13914 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/multithreading/test_multithreaded_bookmark_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16607 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/multithreading/test_multithreaded_offset_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4660 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/multithreading/test_requests_pool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.880557 tap-mambu-4.1.0/mambu_tests/tap_generators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1604 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_activities_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3245 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_audit_trail_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      537 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_branches_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      546 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_centres_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      669 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_clients_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      608 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_communications_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      565 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_credit_arrangements_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_custom_field_sets_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      688 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_deposit_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      376 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_deposit_cards_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      403 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_deposit_products_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      687 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_deposit_transactions_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9335 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_generators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      429 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_gl_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_gl_journal_entries_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_groups_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      602 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_index_rate_sources_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_installments_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_interest_accrual_breakdown_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1181 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_loan_accounts_generators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_loan_products_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      663 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_loan_transactions_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_no_pagination_generators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_repayments_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      528 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_tasks_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      514 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_generators/test_users_generator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.884557 tap-mambu-4.1.0/mambu_tests/tap_processors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1001 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_processors/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2669 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_processors/test_audit_trail_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_processors/test_deposit_accounts_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_processors/test_deposit_cards_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_processors/test_loan_accounts_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      269 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_processors/test_loan_repayments_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14265 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/tap_processors/test_processors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3453 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/test_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7154 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/mambu_tests/test_sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.884557 tap-mambu-4.1.0/schema_fetcher/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/schema_fetcher/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1725 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/schema_fetcher/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/schema_fetcher/converters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/schema_fetcher/custom_exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1090 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/schema_fetcher/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8223 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/schema_fetcher/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-02-20 11:28:21.916558 tap-mambu-4.1.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1167 2024-02-20 11:27:32.000000 tap-mambu-4.1.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.884557 tap-mambu-4.1.0/tap_mambu/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2024-01-30 07:04:59.000000 tap-mambu-4.1.0/tap_mambu/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.888557 tap-mambu-4.1.0/tap_mambu/helpers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4276 2024-01-30 09:07:22.000000 tap-mambu-4.1.0/tap_mambu/helpers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7711 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2024-01-25 06:28:28.000000 tap-mambu-4.1.0/tap_mambu/helpers/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2280 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/datetime_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      921 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      118 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4448 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/generator_processor_pairs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      982 2024-02-14 09:04:24.000000 tap-mambu-4.1.0/tap_mambu/helpers/hashable_dict.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1396 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/metrics_plotter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2045 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/multithreaded_requests.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2866 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/perf_metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4929 2024-02-20 10:34:41.000000 tap-mambu-4.1.0/tap_mambu/helpers/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.908558 tap-mambu-4.1.0/tap_mambu/helpers/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3896 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/activities.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/audit_trail.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4297 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/branches.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      203 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/cards.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3071 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/centres.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10100 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/clients.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/communications.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2303 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/credit_arrangements.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5596 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/custom_field_sets.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14675 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/deposit_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22353 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/deposit_products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18118 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/deposit_transactions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1783 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/gl_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5314 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/gl_journal_entries.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5425 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/groups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/index_rate_sources.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9559 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/installments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3670 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/interest_accrual_breakdown.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31314 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/loan_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43409 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/loan_products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5677 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/loan_repayments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12828 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/loan_transactions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1607 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/tasks.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4366 2024-02-14 09:04:24.000000 tap-mambu-4.1.0/tap_mambu/helpers/schemas/users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      537 2024-01-30 09:08:44.000000 tap-mambu-4.1.0/tap_mambu/helpers/transformer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5177 2024-01-17 09:02:20.000000 tap-mambu-4.1.0/tap_mambu/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.912558 tap-mambu-4.1.0/tap_mambu/tap_generators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1382 2024-02-20 04:29:46.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/activities_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2536 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/audit_trail_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      380 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/branches_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/centres_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/child_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      255 2024-02-20 10:34:41.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/clients_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1382 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/communications_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      406 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/credit_arrangements_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/custom_field_sets_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1237 2024-01-31 05:21:40.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/deposit_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/deposit_cards_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/deposit_products_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1187 2024-01-31 05:21:40.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/deposit_transactions_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4266 2024-02-20 10:16:44.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      375 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/gl_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1304 2024-01-31 05:21:40.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/gl_journal_entries_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1124 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/groups_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      443 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/index_rate_sources_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      991 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/installments_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1272 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/interest_accrual_breakdown_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1557 2024-02-15 07:46:37.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/loan_accounts_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      378 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/loan_products_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/loan_repayments_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1086 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/loan_transactions_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4971 2024-02-20 10:16:44.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/multithreaded_bookmark_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6834 2024-02-20 07:20:04.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/multithreaded_offset_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      344 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/no_pagination_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      521 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/tasks_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      410 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_generators/users_generator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.916558 tap-mambu-4.1.0/tap_mambu/tap_processors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2692 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/audit_trail_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/child_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/deduplication_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/deposit_accounts_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      260 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/deposit_cards_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      427 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/loan_accounts_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      217 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/loan_repayments_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1613 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/multithreaded_parent_processor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5648 2024-01-30 09:08:44.000000 tap-mambu-4.1.0/tap_mambu/tap_processors/processor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.916558 tap-mambu-4.1.0/tap_mambu.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      904 2024-02-20 11:28:21.000000 tap-mambu-4.1.0/tap_mambu.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6554 2024-02-20 11:28:21.000000 tap-mambu-4.1.0/tap_mambu.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-02-20 11:28:21.000000 tap-mambu-4.1.0/tap_mambu.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2024-02-20 11:28:21.000000 tap-mambu-4.1.0/tap_mambu.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      230 2024-02-20 11:28:21.000000 tap-mambu-4.1.0/tap_mambu.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2024-02-20 11:28:21.000000 tap-mambu-4.1.0/tap_mambu.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-20 11:28:21.916558 tap-mambu-4.1.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1929 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tests/test_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tests/test_bookmarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7060 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tests/test_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1684 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tests/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6464 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tests/test_start_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1198 2023-12-20 04:57:20.000000 tap-mambu-4.1.0/tests/test_sync_canary.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.343251 tap-mambu-4.2.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2024-03-18 08:10:16.000000 tap-mambu-4.2.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      332 2024-05-13 12:37:13.343251 tap-mambu-4.2.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19454 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.323251 tap-mambu-4.2.0/mambu_tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      953 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3873 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/helpers.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.323251 tap-mambu-4.2.0/mambu_tests/multithreading/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/multithreading/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4418 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/multithreading/test_multithreaded_bookmark_daybyday_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13914 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/multithreading/test_multithreaded_bookmark_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16607 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/multithreading/test_multithreaded_offset_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4660 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/multithreading/test_requests_pool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.327251 tap-mambu-4.2.0/mambu_tests/tap_generators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1541 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1604 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_activities_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3245 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_audit_trail_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      537 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_branches_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      546 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_centres_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      669 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_clients_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      608 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_communications_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      565 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_credit_arrangements_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_custom_field_sets_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      688 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_deposit_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      376 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_deposit_cards_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      403 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_deposit_products_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      687 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_deposit_transactions_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9335 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_generators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      429 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_gl_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_gl_journal_entries_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_groups_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      602 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_index_rate_sources_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_installments_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_interest_accrual_breakdown_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1181 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_loan_accounts_generators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_loan_products_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      663 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_loan_transactions_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_no_pagination_generators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_repayments_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      528 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_tasks_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      514 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_generators/test_users_generator.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.331251 tap-mambu-4.2.0/mambu_tests/tap_processors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1001 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_processors/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2669 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_processors/test_audit_trail_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_processors/test_deposit_accounts_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_processors/test_deposit_cards_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_processors/test_loan_accounts_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      269 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_processors/test_loan_repayments_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14265 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/tap_processors/test_processors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3453 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/test_helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7154 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/mambu_tests/test_sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.331251 tap-mambu-4.2.0/schema_fetcher/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/schema_fetcher/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1725 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/schema_fetcher/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/schema_fetcher/converters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      102 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/schema_fetcher/custom_exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1090 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/schema_fetcher/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8223 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/schema_fetcher/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-13 12:37:13.343251 tap-mambu-4.2.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1167 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.331251 tap-mambu-4.2.0/tap_mambu/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1605 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.331251 tap-mambu-4.2.0/tap_mambu/helpers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4276 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8307 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/helpers/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/helpers/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2280 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      921 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/helpers/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4448 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/generator_processor_pairs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      982 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/hashable_dict.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1906 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/helpers/multithreaded_requests.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4929 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.335251 tap-mambu-4.2.0/tap_mambu/helpers/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3896 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/activities.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/audit_trail.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4297 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/branches.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      203 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/cards.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3071 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/centres.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10100 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/clients.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/communications.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2303 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/credit_arrangements.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5596 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/custom_field_sets.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14675 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/deposit_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22353 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/deposit_products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18118 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/deposit_transactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1783 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/gl_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5314 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/gl_journal_entries.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5425 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/groups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/index_rate_sources.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9559 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/installments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3670 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/interest_accrual_breakdown.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31314 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/loan_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    43409 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/loan_products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5677 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/loan_repayments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12828 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/loan_transactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1607 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/tasks.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4366 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/schemas/users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      537 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/helpers/transformer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4006 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.339251 tap-mambu-4.2.0/tap_mambu/tap_generators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1273 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/activities_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2536 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/audit_trail_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      380 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/branches_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/centres_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      610 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/child_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/clients_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1479 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/communications_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      406 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/credit_arrangements_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/custom_field_sets_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      844 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/deposit_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      478 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/deposit_cards_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/deposit_products_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      709 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/deposit_transactions_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4655 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      375 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/gl_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      752 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/gl_journal_entries_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      729 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/groups_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      443 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/index_rate_sources_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1196 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/installments_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      878 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/interest_accrual_breakdown_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/loan_accounts_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      378 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/loan_products_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      402 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/loan_repayments_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      697 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/loan_transactions_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4971 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/multithreaded_bookmark_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10106 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/multithreaded_offset_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      344 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/no_pagination_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      521 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/tasks_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      608 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_generators/users_generator.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.343251 tap-mambu-4.2.0/tap_mambu/tap_processors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2692 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/audit_trail_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/child_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4647 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/deduplication_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/deposit_accounts_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      260 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/deposit_cards_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      427 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/loan_accounts_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      217 2024-05-02 09:00:53.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/loan_repayments_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1800 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/multithreaded_parent_processor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6370 2024-05-13 10:15:47.000000 tap-mambu-4.2.0/tap_mambu/tap_processors/processor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 12:37:13.331251 tap-mambu-4.2.0/tap_mambu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      332 2024-05-13 12:37:13.000000 tap-mambu-4.2.0/tap_mambu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6328 2024-05-13 12:37:13.000000 tap-mambu-4.2.0/tap_mambu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-13 12:37:13.000000 tap-mambu-4.2.0/tap_mambu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2024-05-13 12:37:13.000000 tap-mambu-4.2.0/tap_mambu.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      230 2024-05-13 12:37:13.000000 tap-mambu-4.2.0/tap_mambu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2024-05-13 12:37:13.000000 tap-mambu-4.2.0/tap_mambu.egg-info/top_level.txt
```

### Comparing `tap-mambu-4.1.0/LICENSE` & `tap-mambu-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/README.md` & `tap-mambu-4.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -250,18 +250,21 @@
         "password": "YOUR_PASSWORD",
         "apikey": "YOUR_APIKEY",
         "subdomain": "YOUR_SUBDOMAIN",
         "start_date": "2019-01-01T00:00:00Z",
         "lookback_window": 30,
         "user_agent": "tap-mambu <api_user_email@your_company.com>",
         "page_size": "500",
-        "apikey_audit": "AUDIT_TRAIL_APIKEY"
+        "apikey_audit": "AUDIT_TRAIL_APIKEY",
+        "window_size": 7
     }
     ```
-    
+
+    Note: The `window_size` parameter defaults to 1 day, which may cause slowdowns in historical sync for streams utilizing multi-threaded implementation. Conversely, using a larger `window_size` could lead to potential `out-of-memory` issues. It is advisable to select an optimal `window_size` based on the `start_date` and volume of data to mitigate these concerns.
+
     Optionally, also create a `state.json` file. `currently_syncing` is an optional attribute used for identifying the last object to be synced in case the job is interrupted mid-stream. The next run would begin where the last job left off.
 
     ```json
     {
         "currently_syncing": "tasks",
         "bookmarks": {
             "audit_trail":"2021-05-20T09:59:09.780213Z",
```

### Comparing `tap-mambu-4.1.0/mambu_tests/conftest.py` & `tap-mambu-4.2.0/mambu_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/helpers.py` & `tap-mambu-4.2.0/mambu_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/multithreading/test_multithreaded_bookmark_daybyday_generator.py` & `tap-mambu-4.2.0/mambu_tests/multithreading/test_multithreaded_bookmark_daybyday_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/multithreading/test_multithreaded_bookmark_generator.py` & `tap-mambu-4.2.0/mambu_tests/multithreading/test_multithreaded_bookmark_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/multithreading/test_multithreaded_offset_generator.py` & `tap-mambu-4.2.0/mambu_tests/multithreading/test_multithreaded_offset_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/multithreading/test_requests_pool.py` & `tap-mambu-4.2.0/mambu_tests/multithreading/test_requests_pool.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/__init__.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_activities_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_activities_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_audit_trail_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_audit_trail_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_branches_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_branches_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_centres_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_centres_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_clients_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_clients_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_communications_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_communications_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_credit_arrangements_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_credit_arrangements_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_deposit_accounts_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_deposit_accounts_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_deposit_transactions_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_deposit_transactions_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_generators.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_generators.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_gl_journal_entries_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_gl_journal_entries_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_groups_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_groups_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_index_rate_sources_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_index_rate_sources_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_installments_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_installments_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_interest_accrual_breakdown_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_interest_accrual_breakdown_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_loan_accounts_generators.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_loan_accounts_generators.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_loan_transactions_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_loan_transactions_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_no_pagination_generators.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_no_pagination_generators.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_tasks_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_tasks_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_generators/test_users_generator.py` & `tap-mambu-4.2.0/mambu_tests/tap_generators/test_users_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_processors/__init__.py` & `tap-mambu-4.2.0/mambu_tests/tap_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_processors/test_audit_trail_processor.py` & `tap-mambu-4.2.0/mambu_tests/tap_processors/test_audit_trail_processor.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/tap_processors/test_processors.py` & `tap-mambu-4.2.0/mambu_tests/tap_processors/test_processors.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/test_helpers.py` & `tap-mambu-4.2.0/mambu_tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/mambu_tests/test_sync.py` & `tap-mambu-4.2.0/mambu_tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/schema_fetcher/constants.py` & `tap-mambu-4.2.0/schema_fetcher/constants.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/schema_fetcher/helpers.py` & `tap-mambu-4.2.0/schema_fetcher/helpers.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/schema_fetcher/main.py` & `tap-mambu-4.2.0/schema_fetcher/main.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/setup.py` & `tap-mambu-4.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-mambu',
-      version='4.1.0',
+      version='4.2.0',
       description='Singer.io tap for extracting data from the Mambu 2.0 API',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mambu'],
       python_requires='>=3.9',
       install_requires=[
           'backoff==1.8.0',
```

### Comparing `tap-mambu-4.1.0/tap_mambu/__init__.py` & `tap-mambu-4.2.0/tap_mambu/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
     with MambuClient(parsed_args.config.get('username'),
                      parsed_args.config.get('password'),
                      parsed_args.config.get('apikey'),
                      parsed_args.config['subdomain'],
                      parsed_args.config.get('apikey_audit'),
                      int(parsed_args.config.get('page_size', DEFAULT_PAGE_SIZE)),
-                     user_agent=parsed_args.config['user_agent']) as client:
+                     user_agent=parsed_args.config['user_agent'],
+                     window_size=parsed_args.config.get('window_size')) as client:
 
         state = {}
         if parsed_args.state:
             state = parsed_args.state
 
         if parsed_args.discover:
             do_discover()
```

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/__init__.py` & `tap-mambu-4.2.0/tap_mambu/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/client.py` & `tap-mambu-4.2.0/tap_mambu/helpers/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import backoff
 import requests
 import requests.adapters
-from requests.exceptions import ConnectionError
+from requests.exceptions import ConnectionError, ChunkedEncodingError
 from singer import metrics, get_logger
 
+from urllib3.exceptions import ProtocolError
+from tap_mambu.helpers.constants import DEFAULT_DATE_WINDOW_SIZE
 
 LOGGER = get_logger()
 class ClientError(Exception):
     """class representing Generic Http error."""
 
     message = None
 
@@ -114,21 +116,29 @@
     def __init__(self,
                  username,
                  password,
                  apikey,
                  subdomain,
                  apikey_audit,
                  page_size,
-                 user_agent=''):
+                 user_agent='',
+                 window_size=DEFAULT_DATE_WINDOW_SIZE):
         self.__username = username
         self.__password = password
         self.__subdomain = subdomain
         base_url = "https://{}.mambu.com/api".format(subdomain)
         self.base_url = base_url
         self.page_size = page_size
+        try:
+            self.window_size = int(float(window_size)) if window_size else DEFAULT_DATE_WINDOW_SIZE
+            if self.window_size <= 0:
+                raise ValueError()
+        except ValueError:
+            raise Exception("The entered window size '{}' is invalid; it should be a valid non-zero integer.".format(window_size))
+
         self.__user_agent = f'MambuTap-{user_agent}' if user_agent else 'MambuTap'
         self.__apikey = apikey
         self.__session = requests.Session()
         self.__adapter = requests.adapters.HTTPAdapter(pool_maxsize=100)
         self.__session.mount("https://", self.__adapter)
         self.__verified = False
         self.__apikey_audit = apikey_audit
@@ -174,15 +184,16 @@
         if response.status_code != 200:
             LOGGER.error('Error status_code = {}'.format(response.status_code))
             raise_for_error(response)
         else:
             return True
 
     @backoff.on_exception(backoff.expo,
-                          (MambuInternalServiceError, ConnectionError, MambuApiLimitError),
+                          (MambuInternalServiceError, ConnectionError,
+                           ChunkedEncodingError, MambuApiLimitError, ProtocolError),
                           max_tries=7,
                           factor=3)
     def request(self, method, path=None, url=None, json=None, version=None, apikey_type=None, **kwargs):
         if not self.__verified:
             self.__verified = self.check_access()
 
         if not version:
```

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/datetime_utils.py` & `tap-mambu-4.2.0/tap_mambu/helpers/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/discover.py` & `tap-mambu-4.2.0/tap_mambu/helpers/discover.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/generator_processor_pairs.py` & `tap-mambu-4.2.0/tap_mambu/helpers/generator_processor_pairs.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/hashable_dict.py` & `tap-mambu-4.2.0/tap_mambu/helpers/hashable_dict.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/multithreaded_requests.py` & `tap-mambu-4.2.0/tap_mambu/helpers/multithreaded_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import singer
 from concurrent.futures import Future, ThreadPoolExecutor
 from typing import List
-from .perf_metrics import PerformanceMetrics
 
 
 LOGGER = singer.get_logger()
 
 
 class MultithreadedRequestsPool:
     _dispatcher = ThreadPoolExecutor(max_workers=20)
@@ -20,24 +19,23 @@
             endpoint_api_key_type, endpoint_body, endpoint_params) -> List[dict]:
         endpoint_querystring = '&'.join([f'{key}={value}' for (key, value) in endpoint_params.items()])
 
         LOGGER.info(f'(generator) Stream {stream_name} - URL for {stream_name} ({endpoint_api_method}, '
                     f'{endpoint_api_version}): {client.base_url}/{endpoint_path}?{endpoint_querystring}'
                     f' - body = {endpoint_body}')
 
-        with PerformanceMetrics(metric_name="generator"):
-            response = client.request(
-                method=endpoint_api_method,
-                path=endpoint_path,
-                version=endpoint_api_version,
-                apikey_type=endpoint_api_key_type,
-                params=endpoint_querystring,
-                endpoint=stream_name,
-                json=endpoint_body
-            )
+        response = client.request(
+            method=endpoint_api_method,
+            path=endpoint_path,
+            version=endpoint_api_version,
+            apikey_type=endpoint_api_key_type,
+            params=endpoint_querystring,
+            endpoint=stream_name,
+            json=endpoint_body
+        )
 
         LOGGER.info(f'(generator) Stream {stream_name} - extracted records: {len(response)}')
         return response
 
     @classmethod
     def queue_request(cls, client, stream_name,
                       endpoint_path, endpoint_api_method, endpoint_api_version,
```

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schema.py` & `tap-mambu-4.2.0/tap_mambu/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/activities.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/activities.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/audit_trail.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/audit_trail.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/branches.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/branches.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/centres.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/centres.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/clients.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/clients.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/communications.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/communications.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/credit_arrangements.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/credit_arrangements.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/custom_field_sets.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/custom_field_sets.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/deposit_accounts.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/deposit_accounts.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/deposit_products.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/deposit_products.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/deposit_transactions.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/deposit_transactions.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/gl_accounts.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/gl_accounts.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/gl_journal_entries.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/gl_journal_entries.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/groups.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/index_rate_sources.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/index_rate_sources.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/installments.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/installments.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/interest_accrual_breakdown.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/interest_accrual_breakdown.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/loan_accounts.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/loan_accounts.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/loan_products.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/loan_products.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/loan_repayments.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/loan_repayments.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/loan_transactions.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/loan_transactions.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/tasks.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/tasks.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/schemas/users.json` & `tap-mambu-4.2.0/tap_mambu/helpers/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/helpers/transformer.py` & `tap-mambu-4.2.0/tap_mambu/helpers/transformer.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/sync.py` & `tap-mambu-4.2.0/tap_mambu/sync.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import singer
 
 from .helpers.constants import DEFAULT_PAGE_SIZE
 from .helpers import get_selected_streams, should_sync_stream, update_currently_syncing
 from .helpers.datetime_utils import get_timezone_info
 from .helpers.generator_processor_pairs import get_generator_processor_for_stream, get_stream_subtypes
 from .helpers.multithreaded_requests import MultithreadedRequestsPool
-from .helpers.perf_metrics import PerformanceMetrics
 
 LOGGER = singer.get_logger()
 
 
 def sync_endpoint(client, catalog, state,
                   stream_name, sub_type, config, parent_id=None):
     generator_classes, processor_class = get_generator_processor_for_stream(stream_name)
@@ -34,16 +33,14 @@
 
 def sync_all_streams(client, config, catalog, state):
     from .tap_generators.child_generator import ChildGenerator
     from .tap_processors.child_processor import ChildProcessor
 
     get_timezone_info(client)
 
-    PerformanceMetrics.set_generator_batch_size(int(config.get("page_size", DEFAULT_PAGE_SIZE)))
-    
     selected_streams = get_selected_streams(catalog)
     LOGGER.info('selected_streams: {}'.format(selected_streams))
 
     if not selected_streams:
         return
 
     # last_stream = Previous currently synced stream, if the load was interrupted
@@ -71,15 +68,14 @@
         if should_stream:
             # loop through each sub type
             sub_types = get_stream_subtypes(stream_name)
             for sub_type in sub_types:
                 LOGGER.info('START Syncing: {}, Type: {}'.format(stream_name, sub_type))
 
                 update_currently_syncing(state, stream_name)
-                PerformanceMetrics.reset_metrics()
                 total_records = sync_endpoint(
                     client=client,
                     catalog=catalog,
                     state=state,
                     stream_name=stream_name,
                     sub_type=sub_type,
                     config=config
@@ -87,25 +83,8 @@
 
                 update_currently_syncing(state, None)
                 LOGGER.info('Synced: {}, total_records: {}'.format(
                                 stream_name,
                                 total_records))
                 LOGGER.info('FINISHED Syncing: {}'.format(stream_name))
 
-                statistics = PerformanceMetrics.get_statistics()
-
-                if statistics['generator'] and statistics['generator_98th']:
-                    LOGGER.info(f"Average Generator Records/s: {round(1/statistics['generator'])} "
-                                f"[98th percentile: {round(1/statistics['generator_98th'])}]")
-
-                if statistics['processor'] and statistics['processor_98th']:
-                    LOGGER.info(f"Average Processor Records/s: {round(1/statistics['processor'])} "
-                                f"[98th percentile: {round(1/statistics['processor_98th'])}]")
-
-                LOGGER.info(f"Total Generator Wait (s): {round(statistics['generator_wait'], 1)} ")
-
-                LOGGER.info(f"Total Processor Wait (s): {round(statistics['processor_wait'], 1)} ")
-
-                LOGGER.info(f"Average Records/s: {statistics['records']}")
-                LOGGER.info(f"Total Duration: {statistics['extraction']}")
-
     MultithreadedRequestsPool.shutdown()
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/activities_generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/activities_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from .multithreaded_bookmark_generator import MultithreadedBookmarkDayByDayGenerator
-from ..helpers import get_bookmark
-from ..helpers.datetime_utils import datetime_to_utc_str, str_to_localized_datetime, utc_now
+from ..helpers.datetime_utils import datetime_to_utc_str
+from datetime import datetime
 
 
 class ActivitiesGenerator(MultithreadedBookmarkDayByDayGenerator):
     def _init_endpoint_config(self):
         super(ActivitiesGenerator, self)._init_endpoint_config()
         self.endpoint_path = "activities"
         self.endpoint_api_method = "GET"
         self.endpoint_api_version = "v1"
-
-        self.endpoint_params["from"] = datetime_to_utc_str(str_to_localized_datetime(
-                    get_bookmark(self.state, self.stream_name, self.sub_type, self.start_date)))[:10]
-        self.endpoint_params["to"] = datetime_to_utc_str(utc_now())[:10]
         self.endpoint_bookmark_field = "timestamp"
 
+    def modify_request_params(self, start, end):
+        self.static_params["from"] = datetime.strftime(start, '%Y-%m-%d')
+        self.static_params["to"] = datetime.strftime(end, '%Y-%m-%d')
+
     @staticmethod
     def unpack_activity(record):
         record.update(record["activity"])
         del record["activity"]
         return record
 
     def transform_batch(self, batch):
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/audit_trail_generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/audit_trail_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/communications_generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/communications_generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 from .multithreaded_bookmark_generator import MultithreadedBookmarkGenerator
-from ..helpers import get_bookmark
-from ..helpers.datetime_utils import datetime_to_local_str, str_to_localized_datetime
+from ..helpers.datetime_utils import datetime_to_local_str, datetime_to_utc_str
+from datetime import datetime
 
 
 class CommunicationsGenerator(MultithreadedBookmarkGenerator):
     def _init_endpoint_config(self):
         super(CommunicationsGenerator, self)._init_endpoint_config()
         self.endpoint_path = "communications/messages:search"
         self.endpoint_params = {
             "detailsLevel": "FULL",
             "paginationDetails": "OFF"
         }
         self.endpoint_bookmark_field = "creationDate"
-        self.endpoint_filter_criteria = [
+
+    def modify_request_params(self, start, end):
+        self.endpoint_body = [
+            {
+                "field": self.endpoint_bookmark_field,
+                "operator": "AFTER",
+                "value": datetime_to_utc_str(start)
+            },
+            {
+                "field": self.endpoint_bookmark_field,
+                "operator": "BEFORE",
+                "value": datetime_to_utc_str(start)
+            },
             {
                 "field": "state",
                 "operator": "EQUALS",
                 "value": "SENT"
-            },
-            {
-                "field": "creationDate",
-                "operator": "AFTER",
-                "value": datetime_to_local_str(str_to_localized_datetime(
-                    get_bookmark(self.state, self.stream_name, self.sub_type, self.start_date)))
             }
         ]
 
     def _init_endpoint_body(self):
         self.endpoint_body = self.endpoint_filter_criteria
 
     def prepare_batch_params(self):
         super(CommunicationsGenerator, self).prepare_batch_params()
-        self.endpoint_filter_criteria[1]["value"] = datetime_to_local_str(self.endpoint_intermediary_bookmark_value)
+        self.endpoint_filter_criteria[0]["value"] = datetime_to_local_str(self.endpoint_intermediary_bookmark_value)
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/deposit_accounts_generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/interest_accrual_breakdown_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,18 @@
-from .multithreaded_bookmark_generator import MultithreadedBookmarkGenerator
-from ..helpers import get_bookmark
-from ..helpers.datetime_utils import datetime_to_utc_str, str_to_localized_datetime
+from .multithreaded_bookmark_generator import MultithreadedBookmarkDayByDayGenerator
+from ..helpers.datetime_utils import datetime_to_utc_str
 
 
-class DepositAccountsGenerator(MultithreadedBookmarkGenerator):
-    def _init_config(self):
-        super()._init_config()
-        self.max_threads = 25
-
+class InterestAccrualBreakdownGenerator(MultithreadedBookmarkDayByDayGenerator):
     def _init_endpoint_config(self):
-        super(DepositAccountsGenerator, self)._init_endpoint_config()
-        self.endpoint_path = "deposits:search"
+        super(InterestAccrualBreakdownGenerator, self)._init_endpoint_config()
+        self.endpoint_path = "accounting/interestaccrual:search"
+        self.endpoint_bookmark_field = "creationDate"
         self.endpoint_sorting_criteria = {
-            "field": "lastModifiedDate",
+            "field": "entryId",
             "order": "ASC"
         }
-        self.endpoint_filter_criteria = [
-            {
-                "field": "lastModifiedDate",
-                "operator": "AFTER",
-                "value": datetime_to_utc_str(str_to_localized_datetime(
-                    get_bookmark(self.state, self.stream_name, self.sub_type, self.start_date)))
-            }
-        ]
-        self.endpoint_bookmark_field = "lastModifiedDate"
 
     def prepare_batch_params(self):
-        super(DepositAccountsGenerator, self).prepare_batch_params()
-        self.endpoint_filter_criteria[0]["value"] = datetime_to_utc_str(self.endpoint_intermediary_bookmark_value)
+        super(InterestAccrualBreakdownGenerator, self).prepare_batch_params()
+        # look in db for the reason DateTimes don't work, but Dates do
+        self.endpoint_filter_criteria[0]["value"] = datetime_to_utc_str(self.endpoint_intermediary_bookmark_value)[:10]
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/deposit_transactions_generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/installments_generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from .multithreaded_bookmark_generator import MultithreadedBookmarkGenerator
-from ..helpers import get_bookmark
-from ..helpers.datetime_utils import datetime_to_utc_str, str_to_localized_datetime
+from .multithreaded_offset_generator import MultithreadedOffsetGenerator
+from ..helpers.datetime_utils import datetime_to_utc_str, str_to_localized_datetime, utc_now
 
 
-class DepositTransactionsGenerator(MultithreadedBookmarkGenerator):
-    def _init_config(self):
-        super()._init_config()
-        self.max_threads = 5
+class InstallmentsGenerator(MultithreadedOffsetGenerator):
+    def __init__(self, stream_name, client, config, state, sub_type):
+        super(InstallmentsGenerator, self).__init__(stream_name, client, config, state, sub_type)
+        self.date_windowing = False
 
     def _init_endpoint_config(self):
-        super(DepositTransactionsGenerator, self)._init_endpoint_config()
-        self.endpoint_path = "deposits/transactions:search"
-        self.endpoint_bookmark_field = "creationDate"
-        self.endpoint_sorting_criteria["field"] = "id"
-        self.endpoint_filter_criteria = [
-            {
-                "field": "creationDate",
-                "operator": "AFTER",
-                "value": datetime_to_utc_str(str_to_localized_datetime(
-                    get_bookmark(self.state, self.stream_name, self.sub_type, self.start_date)))
-            }
-        ]
+        super(InstallmentsGenerator, self)._init_endpoint_config()
+        self.endpoint_path = "installments"
+        self.endpoint_api_method = "GET"
+        self.endpoint_params = {
+            "dueFrom": datetime_to_utc_str(str_to_localized_datetime(self.start_date))[:10],
+            "dueTo": datetime_to_utc_str(utc_now())[:10],
+            "detailsLevel": "FULL",
+            "paginationDetails": "OFF"
+        }
+        self.endpoint_bookmark_field = "lastPaidDate"
 
-    def prepare_batch_params(self):
-        super(DepositTransactionsGenerator, self).prepare_batch_params()
-        self.endpoint_filter_criteria[0]["value"] = datetime_to_utc_str(self.endpoint_intermediary_bookmark_value)
+    def transform_batch(self, batch):
+        temp_batch = super(InstallmentsGenerator, self).transform_batch(batch)
+        for record in temp_batch:
+            if "number" in record:
+                record["number"] = "0"
+        return temp_batch
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from abc import ABC
 from typing import List
 from singer import utils, get_logger
 
 from ..helpers import transform_json
 from ..helpers.hashable_dict import HashableDict
-from ..helpers.perf_metrics import PerformanceMetrics
 
 LOGGER = get_logger()
 
 
 class TapGenerator(ABC):
     def __init__(self, stream_name, client, config, state, sub_type):
         self.stream_name = stream_name
         self.client = client
         self.config = config
         self.state = state
         self.sub_type = sub_type
+        self.date_windowing = False
+        self.date_window_size = client.window_size
+        self.start_windows_datetime_str = None
+        self.sub_stream_name = stream_name
 
         # Define parameters inside init
         self.params = dict()
         self.time_extracted = 0
         self.offset = 0
 
         # Initialize parameters
@@ -50,23 +53,29 @@
 
     def _init_endpoint_body(self):
         self.endpoint_body = {"sortingCriteria": self.endpoint_sorting_criteria,
                               "filterCriteria": self.endpoint_filter_criteria}
 
     def _init_buffers(self):
         self.buffer: List = list()
+        self.max_buffer_size = 10000
 
     def _init_params(self):
         self.time_extracted = None
         self.static_params = dict(self.endpoint_params)
         self.offset = 0
         self.limit = self.client.page_size
         self.params = self.static_params
 
     def _all_fetch_batch_steps(self):
+        # Large buffer size can impact memory utilization of connector
+        # so empty the buffer once it reaches default max limit
+        if len(self.buffer) > self.max_buffer_size:
+            return
+
         self.prepare_batch()
         raw_batch = self.fetch_batch()
         self.buffer = transform_json(raw_batch, self.stream_name)
         if not self.buffer:
             LOGGER.warning(f'(generator) Stream {self.stream_name} - NO TRANSFORMED DATA RESULTS')
         self.last_batch_size = len(self.buffer)
 
@@ -81,15 +90,14 @@
             self.offset += self.limit
             self._all_fetch_batch_steps()
             if not self.buffer:
                 raise StopIteration()
         return self.buffer.pop(0)
 
     def __next__(self):
-        # with PerformanceMetrics(metric_name="processor_wait"):
         return self.next()
 
     def prepare_batch(self):
         self.params = {
             "offset": self.offset,
             "limit": self.limit,
             **self.static_params
@@ -104,21 +112,29 @@
     def fetch_batch(self):
         endpoint_querystring = '&'.join([f'{key}={value}' for (key, value) in self.params.items()])
 
         LOGGER.info(f'(generator) Stream {self.stream_name} - URL for {self.stream_name} ({self.endpoint_api_method}, '
                     f'{self.endpoint_api_version}): {self.client.base_url}/{self.endpoint_path}?{endpoint_querystring}')
         LOGGER.info(f'(generator) Stream {self.stream_name} - body = {self.endpoint_body}')
 
-        with PerformanceMetrics(metric_name="generator"):
-            response = self.client.request(
-                method=self.endpoint_api_method,
-                path=self.endpoint_path,
-                version=self.endpoint_api_version,
-                apikey_type=self.endpoint_api_key_type,
-                params=endpoint_querystring,
-                endpoint=self.stream_name,
-                json=self.endpoint_body
-            )
+        response = self.client.request(
+            method=self.endpoint_api_method,
+            path=self.endpoint_path,
+            version=self.endpoint_api_version,
+            apikey_type=self.endpoint_api_key_type,
+            params=endpoint_querystring,
+            endpoint=self.stream_name,
+            json=self.endpoint_body
+        )
 
         self.time_extracted = utils.now()
         LOGGER.info(f'(generator) Stream {self.stream_name} - extracted records: {len(response)}')
         return self.transform_batch(response)
+
+    def get_default_start_value(self):
+        return None
+
+    def set_last_sync_completed(self, end_time):
+        pass
+
+    def wait_for_slibling_to_catchup(self):
+        pass
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/gl_journal_entries_generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/gl_journal_entries_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,17 @@
 from .multithreaded_bookmark_generator import MultithreadedBookmarkGenerator
-from ..helpers import get_bookmark
-from ..helpers.datetime_utils import datetime_to_utc_str, str_to_localized_datetime, utc_now
+from ..helpers.datetime_utils import datetime_to_utc_str
 
 
 class GlJournalEntriesGenerator(MultithreadedBookmarkGenerator):
-    def _init_config(self):
-        super()._init_config()
-        self.max_threads = 5
-
     def _init_endpoint_config(self):
         super(GlJournalEntriesGenerator, self)._init_endpoint_config()
         self.endpoint_path = "gljournalentries:search"
         self.endpoint_bookmark_field = "creationDate"
         self.endpoint_sorting_criteria = {
             "field": "entryId",
             "order": "ASC"
         }
-        self.endpoint_filter_criteria = [
-            {
-                "field": "creationDate",
-                "operator": "BETWEEN",
-                "value": datetime_to_utc_str(str_to_localized_datetime(
-                    get_bookmark(self.state, self.stream_name, self.sub_type, self.start_date))),
-                "secondValue": datetime_to_utc_str(utc_now())
-            }
-        ]
 
     def prepare_batch_params(self):
         super(GlJournalEntriesGenerator, self).prepare_batch_params()
         self.endpoint_filter_criteria[0]["value"] = datetime_to_utc_str(self.endpoint_intermediary_bookmark_value)
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/loan_transactions_generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/deposit_transactions_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 from .multithreaded_bookmark_generator import MultithreadedBookmarkGenerator
-from ..helpers import get_bookmark
-from ..helpers.datetime_utils import datetime_to_utc_str, str_to_localized_datetime
+from ..helpers.datetime_utils import datetime_to_utc_str
 
 
-class LoanTransactionsGenerator(MultithreadedBookmarkGenerator):
+class DepositTransactionsGenerator(MultithreadedBookmarkGenerator):
     def _init_endpoint_config(self):
-        super(LoanTransactionsGenerator, self)._init_endpoint_config()
-        self.endpoint_path = "loans/transactions:search"
+        super(DepositTransactionsGenerator, self)._init_endpoint_config()
+        self.endpoint_path = "deposits/transactions:search"
         self.endpoint_bookmark_field = "creationDate"
         self.endpoint_sorting_criteria["field"] = "id"
-        self.endpoint_filter_criteria = [
-            {
-                "field": "creationDate",
-                "operator": "AFTER",
-                "value": datetime_to_utc_str(str_to_localized_datetime(
-                    get_bookmark(self.state, self.stream_name, self.sub_type, self.start_date)))
-            }
-        ]
 
     def prepare_batch_params(self):
-        super(LoanTransactionsGenerator, self).prepare_batch_params()
+        super(DepositTransactionsGenerator, self).prepare_batch_params()
         self.endpoint_filter_criteria[0]["value"] = datetime_to_utc_str(self.endpoint_intermediary_bookmark_value)
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/multithreaded_bookmark_generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/multithreaded_bookmark_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_generators/tasks_generator.py` & `tap-mambu-4.2.0/tap_mambu/tap_generators/tasks_generator.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_processors/audit_trail_processor.py` & `tap-mambu-4.2.0/tap_mambu/tap_processors/audit_trail_processor.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_processors/child_processor.py` & `tap-mambu-4.2.0/tap_mambu/tap_processors/child_processor.py`

 * *Files identical despite different names*

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_processors/deduplication_processor.py` & `tap-mambu-4.2.0/tap_mambu/tap_processors/deduplication_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from singer import get_logger, metrics
 from singer.utils import strptime_to_utc
 
 from .processor import TapProcessor
 from ..helpers import convert
 from ..helpers.exceptions import NoDeduplicationCapabilityException, NoDeduplicationKeyException
-from ..helpers.perf_metrics import PerformanceMetrics
 
 LOGGER = get_logger()
 
 
 class DeduplicationProcessor(TapProcessor):
     def _init_endpoint_config(self):
         try:
@@ -82,17 +81,16 @@
                     break
 
                 record_key, record_value = self._choose_next_record(self.generator_values)
 
                 # Process the record
                 record = self.generator_values[record_key]
 
-                with PerformanceMetrics(metric_name="processor"):
-                    is_processed = self.process_record(record, record_key.time_extracted,
-                                                       record_key.endpoint_bookmark_field)
+                is_processed = self.process_record(record, record_key.time_extracted,
+                                                    record_key.endpoint_bookmark_field)
 
                 if is_processed:
                     record_count += 1
                     self._process_child_records(record)
                     counter.increment()
 
                 self.remove_same_key_values_from_generators(record_value)
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_processors/multithreaded_parent_processor.py` & `tap-mambu-4.2.0/tap_mambu/tap_processors/multithreaded_parent_processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,18 @@
         self.futures = list()
 
     def process_records(self):
         record_count = super(MultithreadedParentProcessor, self).process_records()
 
         for future in futures.as_completed(self.futures):
             record_count += future.result()
+
+        for generator in self.generators:
+            generator.set_last_sync_completed(self.generators[0].start_windows_datetime_str)
+            generator.remove_sub_stream_bookmark()
         return record_count
 
     def _process_child_records(self, record):
         from ..sync import sync_endpoint
 
         super(MultithreadedParentProcessor, self)._process_child_records(record)
         for child_stream_name in self.endpoint_child_streams:
```

### Comparing `tap-mambu-4.1.0/tap_mambu/tap_processors/processor.py` & `tap-mambu-4.2.0/tap_mambu/tap_processors/processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABC
 
 from singer import write_record, metadata, write_schema, get_logger, metrics, utils
 
 from ..helpers import convert, get_bookmark, write_bookmark
 from ..helpers.transformer import Transformer
 from ..helpers.exceptions import NoDeduplicationCapabilityException
-from ..helpers.perf_metrics import PerformanceMetrics
 from ..helpers.datetime_utils import utc_now, str_to_datetime, datetime_to_utc_str, str_to_localized_datetime
+from ..helpers.schema import STREAMS
 
 LOGGER = get_logger()
 
 
 class TapProcessor(ABC):
     def __init__(self, catalog, stream_name, client, config, state, sub_type, generators):
         self.start_time = utc_now()
@@ -40,15 +40,22 @@
         self.endpoint_id_field = "id"
 
         if len(self.generators) > 1:
             raise NoDeduplicationCapabilityException("In order to merge streams in the processor, "
                                                      "you need to use the deduplication processor")
 
     def _init_bookmarks(self):
-        self.last_bookmark_value = get_bookmark(self.state, self.stream_name, self.sub_type, self.start_date)
+        # Since we have date window implementation in multithreaded genrators,
+        # we can't rely on bookmark value since if case of interruption we may miss some of the records
+        # lesser bookmark value record by lagging threads than bookmark written by faster thread
+        # Because of which in next sync we will miss parent as well as corresponding child records.
+        # In such scenario we should resume extraction from the last date window where extration interrupted
+        last_bookmark = self.generators[0].get_default_start_value()
+
+        self.last_bookmark_value = last_bookmark or get_bookmark(self.state, self.stream_name, self.sub_type, self.start_date)
         self.max_bookmark_value = self.last_bookmark_value
 
     def write_schema(self):
         stream = self.catalog.get_stream(self.stream_name)
         schema = stream.schema.to_dict()
         try:
             write_schema(self.stream_name, schema, stream.key_properties)
@@ -57,28 +64,30 @@
             raise err
 
     def process_records(self):
         record_count = 0
         with metrics.record_counter(self.stream_name) as counter:
             for record in self.generators[0]:
                 # Process the record
-                with PerformanceMetrics(metric_name="processor"):
-                    is_processed = self.process_record(record, utils.now(),
-                                                       self.generators[0].endpoint_bookmark_field)
+                is_processed = self.process_record(record, utils.now(),
+                                                    self.generators[0].endpoint_bookmark_field)
                 if is_processed:
                     record_count += 1
                     self._process_child_records(record)
                     counter.increment()
+
         return record_count
 
     def process_streams_from_generators(self):
         self.write_schema()
 
         record_count = self.process_records()
-        self.write_bookmark()
+        if STREAMS.get(self.stream_name).get("replication_method") == "INCREMENTAL":
+            self.write_bookmark()
+
         return record_count
 
     # This function is provided for processors with child streams, must be overridden if child streams are to be used
     def _process_child_records(self, record):
         pass
 
     def _update_bookmark(self, transformed_record, bookmark_field):
@@ -96,14 +105,17 @@
         if not bookmark_field or (bookmark_field not in transformed_record):
             return True
 
         # Keep only records whose bookmark is after the last_datetime
         if str_to_localized_datetime(transformed_record[bookmark_field]) >= \
                 str_to_localized_datetime(self.last_bookmark_value):
             return True
+        else:
+            LOGGER.info(
+                f"Skipped record older than bookmark: {self.stream_name} {transformed_record.get('id')}")
         return False
 
     def process_record(self, record, time_extracted, bookmark_field):
         with Transformer() as transformer:
             transformed_record = transformer.transform(record,
                                                        self.schema,
                                                        self.stream_metadata)
```

### Comparing `tap-mambu-4.1.0/tap_mambu.egg-info/SOURCES.txt` & `tap-mambu-4.2.0/tap_mambu.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -65,17 +65,15 @@
 tap_mambu/helpers/client.py
 tap_mambu/helpers/constants.py
 tap_mambu/helpers/datetime_utils.py
 tap_mambu/helpers/discover.py
 tap_mambu/helpers/exceptions.py
 tap_mambu/helpers/generator_processor_pairs.py
 tap_mambu/helpers/hashable_dict.py
-tap_mambu/helpers/metrics_plotter.py
 tap_mambu/helpers/multithreaded_requests.py
-tap_mambu/helpers/perf_metrics.py
 tap_mambu/helpers/schema.py
 tap_mambu/helpers/transformer.py
 tap_mambu/helpers/schemas/activities.json
 tap_mambu/helpers/schemas/audit_trail.json
 tap_mambu/helpers/schemas/branches.json
 tap_mambu/helpers/schemas/cards.json
 tap_mambu/helpers/schemas/centres.json
@@ -133,14 +131,8 @@
 tap_mambu/tap_processors/child_processor.py
 tap_mambu/tap_processors/deduplication_processor.py
 tap_mambu/tap_processors/deposit_accounts_processor.py
 tap_mambu/tap_processors/deposit_cards_processor.py
 tap_mambu/tap_processors/loan_accounts_processor.py
 tap_mambu/tap_processors/loan_repayments_processor.py
 tap_mambu/tap_processors/multithreaded_parent_processor.py
-tap_mambu/tap_processors/processor.py
-tests/test_automatic_fields.py
-tests/test_bookmarks.py
-tests/test_discovery.py
-tests/test_pagination.py
-tests/test_start_date.py
-tests/test_sync_canary.py
+tap_mambu/tap_processors/processor.py
```

