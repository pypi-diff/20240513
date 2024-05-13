# Comparing `tmp/cycode-1.9.5.dev2.tar.gz` & `tmp/cycode-1.9.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-1.9.5.dev2.tar", max compression
+gzip compressed data, was "cycode-1.9.5.dev3.tar", max compression
```

## Comparing `cycode-1.9.5.dev2.tar` & `cycode-1.9.5.dev3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0    42683 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/README.md
--rw-r--r--   0        0        0      114 2024-05-10 14:09:50.274375 cycode-1.9.5.dev2/cycode/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/auth/__init__.py
--rw-r--r--   0        0        0     2897 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/auth/auth_command.py
--rw-r--r--   0        0        0     4722 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/auth/auth_manager.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/configure/__init__.py
--rw-r--r--   0        0        0     5423 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/configure/configure_command.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/ignore/__init__.py
--rw-r--r--   0        0        0     3873 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/ignore/ignore_command.py
--rw-r--r--   0        0        0     2497 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/main_cli.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/__init__.py
--rw-r--r--   0        0        0      563 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/report_command.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/__init__.py
--rw-r--r--   0        0        0     3429 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/common.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/path/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/path/path_command.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/repository_url/__init__.py
--rw-r--r--   0        0        0     2143 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
--rw-r--r--   0        0        0     2358 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/sbom_command.py
--rw-r--r--   0        0        0     1533 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/sbom_report_file.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.822269 cycode-1.9.5.dev2/cycode/cli/commands/scan/__init__.py
--rw-r--r--   0        0        0    38706 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/code_scanner.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/commit_history/__init__.py
--rw-r--r--   0        0        0      975 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/commit_history/commit_history_command.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/path/__init__.py
--rw-r--r--   0        0        0      590 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/path/path_command.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/pre_commit/__init__.py
--rw-r--r--   0        0        0     1605 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/pre_receive/__init__.py
--rw-r--r--   0        0        0     2699 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/repository/__init__.py
--rw-r--r--   0        0        0     2710 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/repository/repository_command.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/scan_ci/__init__.py
--rw-r--r--   0        0        0     1588 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/scan_ci/ci_integrations.py
--rw-r--r--   0        0        0      552 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
--rw-r--r--   0        0        0     5082 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/scan/scan_command.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/version/__init__.py
--rw-r--r--   0        0        0      509 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/commands/version/version_command.py
--rw-r--r--   0        0        0      466 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/config.py
--rw-r--r--   0        0        0      463 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/config.yaml
--rw-r--r--   0        0        0     6194 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     2109 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0     1620 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/exceptions/handle_report_sbom_errors.py
--rw-r--r--   0        0        0     2785 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/exceptions/handle_scan_errors.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/__init__.py
--rw-r--r--   0        0        0     5468 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/excluder.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/iac/__init__.py
--rw-r--r--   0        0        0     2457 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/iac/tf_content_generator.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/models/__init__.py
--rw-r--r--   0        0        0     1247 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/models/in_memory_zip.py
--rw-r--r--   0        0        0     4393 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/path_documents.py
--rw-r--r--   0        0        0     4940 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/repository_documents.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/sca/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/sca/maven/__init__.py
--rw-r--r--   0        0        0     2417 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0     1136 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     3119 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     6398 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/sca/sca_code_scanner.py
--rw-r--r--   0        0        0     1836 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/files_collector/zip_documents.py
--rw-r--r--   0        0        0      387 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/main.py
--rw-r--r--   0        0        0     2051 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0     2395 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     2290 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     1613 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/printer_base.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/tables/__init__.py
--rw-r--r--   0        0        0     7660 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/tables/sca_table_printer.py
--rw-r--r--   0        0        0     2281 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/tables/table.py
--rw-r--r--   0        0        0      480 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/tables/table_models.py
--rw-r--r--   0        0        0     5216 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/tables/table_printer.py
--rw-r--r--   0        0        0     2400 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/tables/table_printer_base.py
--rw-r--r--   0        0        0    10484 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      630 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4939 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     7591 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     2987 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0      745 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/user_settings/jwt_creator.py
--rw-r--r--   0        0        0        0 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0      211 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/enum_utils.py
--rw-r--r--   0        0        0     1584 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/get_api_client.py
--rw-r--r--   0        0        0     1953 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0     9716 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/progress_bar.py
--rw-r--r--   0        0        0     2794 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/scan_batch.py
--rw-r--r--   0        0        0      334 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      978 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     2034 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2748 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      934 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0       71 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1777 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     1072 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cyclient/client_creator.py
--rw-r--r--   0        0        0     2937 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      120 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      257 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3570 2024-05-10 14:09:43.826269 cycode-1.9.5.dev2/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      670 2024-05-10 14:09:43.830269 cycode-1.9.5.dev2/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     3600 2024-05-10 14:09:43.830269 cycode-1.9.5.dev2/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     1318 2024-05-10 14:09:43.830269 cycode-1.9.5.dev2/cycode/cyclient/headers.py
--rw-r--r--   0        0        0    13148 2024-05-10 14:09:43.830269 cycode-1.9.5.dev2/cycode/cyclient/models.py
--rw-r--r--   0        0        0     3971 2024-05-10 14:09:43.830269 cycode-1.9.5.dev2/cycode/cyclient/report_client.py
--rw-r--r--   0        0        0    13449 2024-05-10 14:09:43.830269 cycode-1.9.5.dev2/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0     1658 2024-05-10 14:09:43.830269 cycode-1.9.5.dev2/cycode/cyclient/scan_config_base.py
--rw-r--r--   0        0        0     3458 2024-05-10 14:09:50.274375 cycode-1.9.5.dev2/pyproject.toml
--rw-r--r--   0        0        0    44261 1970-01-01 00:00:00.000000 cycode-1.9.5.dev2/PKG-INFO
+-rw-r--r--   0        0        0    42683 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/README.md
+-rw-r--r--   0        0        0      114 2024-05-13 12:29:12.296821 cycode-1.9.5.dev3/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/auth/__init__.py
+-rw-r--r--   0        0        0     2897 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/auth/auth_command.py
+-rw-r--r--   0        0        0     4722 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/auth/auth_manager.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/configure/__init__.py
+-rw-r--r--   0        0        0     5423 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/configure/configure_command.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/ignore/__init__.py
+-rw-r--r--   0        0        0     3873 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/ignore/ignore_command.py
+-rw-r--r--   0        0        0     2497 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/main_cli.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/__init__.py
+-rw-r--r--   0        0        0      563 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/report_command.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/__init__.py
+-rw-r--r--   0        0        0     3429 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/common.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/path/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/repository_url/__init__.py
+-rw-r--r--   0        0        0     2143 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
+-rw-r--r--   0        0        0     2358 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/sbom_command.py
+-rw-r--r--   0        0        0     1533 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/sbom_report_file.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/__init__.py
+-rw-r--r--   0        0        0    38491 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/code_scanner.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/commit_history/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/commit_history/commit_history_command.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/path/__init__.py
+-rw-r--r--   0        0        0      590 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/pre_commit/__init__.py
+-rw-r--r--   0        0        0     1605 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/pre_receive/__init__.py
+-rw-r--r--   0        0        0     2699 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/repository/__init__.py
+-rw-r--r--   0        0        0     2710 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/repository/repository_command.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/scan_ci/__init__.py
+-rw-r--r--   0        0        0     1588 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/scan_ci/ci_integrations.py
+-rw-r--r--   0        0        0      552 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
+-rw-r--r--   0        0        0     5082 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/scan/scan_command.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/version/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/commands/version/version_command.py
+-rw-r--r--   0        0        0      466 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/config.py
+-rw-r--r--   0        0        0      463 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     6194 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     2109 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/exceptions/handle_report_sbom_errors.py
+-rw-r--r--   0        0        0     2785 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/exceptions/handle_scan_errors.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/__init__.py
+-rw-r--r--   0        0        0     5468 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/excluder.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/iac/__init__.py
+-rw-r--r--   0        0        0     2457 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/iac/tf_content_generator.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/models/__init__.py
+-rw-r--r--   0        0        0     1247 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/models/in_memory_zip.py
+-rw-r--r--   0        0        0     4393 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/path_documents.py
+-rw-r--r--   0        0        0     4940 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/repository_documents.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/sca/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/sca/maven/__init__.py
+-rw-r--r--   0        0        0     2417 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0     1136 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     3119 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     6398 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/sca/sca_code_scanner.py
+-rw-r--r--   0        0        0     1836 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/files_collector/zip_documents.py
+-rw-r--r--   0        0        0      387 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/main.py
+-rw-r--r--   0        0        0     2051 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0     2395 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     2290 2024-05-13 12:29:02.440676 cycode-1.9.5.dev3/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     1613 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/printers/printer_base.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/printers/tables/__init__.py
+-rw-r--r--   0        0        0     7660 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/printers/tables/sca_table_printer.py
+-rw-r--r--   0        0        0     2281 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/printers/tables/table.py
+-rw-r--r--   0        0        0      480 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/printers/tables/table_models.py
+-rw-r--r--   0        0        0     5216 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/printers/tables/table_printer.py
+-rw-r--r--   0        0        0     2400 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/printers/tables/table_printer_base.py
+-rw-r--r--   0        0        0    10484 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4939 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     7591 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     2987 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0      745 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/user_settings/jwt_creator.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     1584 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/get_api_client.py
+-rw-r--r--   0        0        0     1953 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     9716 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2794 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      978 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     2034 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2748 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      934 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0       71 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1777 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     1072 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/client_creator.py
+-rw-r--r--   0        0        0     2937 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      120 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      257 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3570 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      670 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     3600 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     1318 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/headers.py
+-rw-r--r--   0        0        0    13050 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     3971 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/report_client.py
+-rw-r--r--   0        0        0    12573 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0     1658 2024-05-13 12:29:02.444676 cycode-1.9.5.dev3/cycode/cyclient/scan_config_base.py
+-rw-r--r--   0        0        0     3458 2024-05-13 12:29:12.292821 cycode-1.9.5.dev3/pyproject.toml
+-rw-r--r--   0        0        0    44261 1970-01-01 00:00:00.000000 cycode-1.9.5.dev3/PKG-INFO
```

### Comparing `cycode-1.9.5.dev2/README.md` & `cycode-1.9.5.dev3/README.md`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/auth/auth_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/auth/auth_manager.py` & `cycode-1.9.5.dev3/cycode/cli/commands/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/configure/configure_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/configure/configure_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/ignore/ignore_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/ignore/ignore_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/main_cli.py` & `cycode-1.9.5.dev3/cycode/cli/commands/main_cli.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/report/report_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/report/report_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/common.py` & `cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/common.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/path/path_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/sbom_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/sbom_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/report/sbom/sbom_report_file.py` & `cycode-1.9.5.dev3/cycode/cli/commands/report/sbom/sbom_report_file.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/scan/code_scanner.py` & `cycode-1.9.5.dev3/cycode/cli/commands/scan/code_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,39 +112,34 @@
     if scan_parameters.get('report') is True:
         raise ValueError('You can not use sync flow with report option. Either remove "report" or "sync" option.')
 
     return True
 
 
 def _enrich_scan_result_with_data_from_detection_rules(
-    cycode_client: 'ScanClient', scan_type: str, scan_result: ZippedFileScanResult
+    cycode_client: 'ScanClient', scan_result: ZippedFileScanResult
 ) -> None:
-    # TODO(MarshalX): remove scan_type arg after migration to new backend filter
-    if scan_type not in {consts.SECRET_SCAN_TYPE, consts.INFRA_CONFIGURATION_SCAN_TYPE}:
-        # not yet
-        return
-
     detection_rule_ids = set()
     for detections_per_file in scan_result.detections_per_file:
         for detection in detections_per_file.detections:
             detection_rule_ids.add(detection.detection_rule_id)
 
-    detection_rules = cycode_client.get_detection_rules(scan_type, detection_rule_ids)
+    detection_rules = cycode_client.get_detection_rules(detection_rule_ids)
     detection_rules_by_id = {detection_rule.detection_rule_id: detection_rule for detection_rule in detection_rules}
 
     for detections_per_file in scan_result.detections_per_file:
         for detection in detections_per_file.detections:
             detection_rule = detection_rules_by_id.get(detection.detection_rule_id)
             if not detection_rule:
                 # we want to make sure that BE returned it. better to not map data instead of failed scan
                 continue
 
-            if detection_rule.classification_data:
+            if not detection.severity and detection_rule.classification_data:
                 # it's fine to take the first one, because:
-                # - for "secrets" and "iac" there is only one classification rule per detection rule
+                # - for "secrets" and "iac" there is only one classification rule per-detection rule
                 # - for "sca" and "sast" we get severity from detection service
                 detection.severity = detection_rule.classification_data[0].severity
 
             # detection_details never was typed properly. so not a problem for now
             detection.detection_details['custom_remediation_guidelines'] = detection_rule.custom_remediation_guidelines
             detection.detection_details['remediation_guidelines'] = detection_rule.remediation_guidelines
             detection.detection_details['description'] = detection_rule.description
@@ -183,15 +178,15 @@
                 is_git_diff,
                 is_commit_range,
                 scan_parameters,
                 should_use_scan_service,
                 should_use_sync_flow,
             )
 
-            _enrich_scan_result_with_data_from_detection_rules(cycode_client, scan_type, scan_result)
+            _enrich_scan_result_with_data_from_detection_rules(cycode_client, scan_result)
 
             local_scan_result = create_local_scan_result(
                 scan_result, batch, command_scan_type, scan_type, severity_threshold
             )
 
             scan_completed = True
         except Exception as e:
```

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/scan/commit_history/commit_history_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/scan/commit_history/commit_history_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/scan/path/path_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/scan/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/scan/pre_commit/pre_commit_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/scan/pre_commit/pre_commit_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/scan/pre_receive/pre_receive_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/scan/pre_receive/pre_receive_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/scan/repository/repository_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/scan/repository/repository_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/scan/scan_ci/ci_integrations.py` & `cycode-1.9.5.dev3/cycode/cli/commands/scan/scan_ci/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/scan/scan_ci/scan_ci_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/scan/scan_ci/scan_ci_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/commands/scan/scan_command.py` & `cycode-1.9.5.dev3/cycode/cli/commands/scan/scan_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/consts.py` & `cycode-1.9.5.dev3/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/exceptions/custom_exceptions.py` & `cycode-1.9.5.dev3/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/exceptions/handle_report_sbom_errors.py` & `cycode-1.9.5.dev3/cycode/cli/exceptions/handle_report_sbom_errors.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/exceptions/handle_scan_errors.py` & `cycode-1.9.5.dev3/cycode/cli/exceptions/handle_scan_errors.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/excluder.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/excluder.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/iac/tf_content_generator.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/iac/tf_content_generator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/models/in_memory_zip.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/models/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/path_documents.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/path_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/repository_documents.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/repository_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/sca/sca_code_scanner.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/sca/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/files_collector/zip_documents.py` & `cycode-1.9.5.dev3/cycode/cli/files_collector/zip_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/models.py` & `cycode-1.9.5.dev3/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/printers/console_printer.py` & `cycode-1.9.5.dev3/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/printers/json_printer.py` & `cycode-1.9.5.dev3/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/printers/printer_base.py` & `cycode-1.9.5.dev3/cycode/cli/printers/printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/printers/tables/sca_table_printer.py` & `cycode-1.9.5.dev3/cycode/cli/printers/tables/sca_table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/printers/tables/table.py` & `cycode-1.9.5.dev3/cycode/cli/printers/tables/table.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/printers/tables/table_printer.py` & `cycode-1.9.5.dev3/cycode/cli/printers/tables/table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/printers/tables/table_printer_base.py` & `cycode-1.9.5.dev3/cycode/cli/printers/tables/table_printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/printers/text_printer.py` & `cycode-1.9.5.dev3/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/user_settings/base_file_manager.py` & `cycode-1.9.5.dev3/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/user_settings/config_file_manager.py` & `cycode-1.9.5.dev3/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/user_settings/configuration_manager.py` & `cycode-1.9.5.dev3/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/user_settings/credentials_manager.py` & `cycode-1.9.5.dev3/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/user_settings/jwt_creator.py` & `cycode-1.9.5.dev3/cycode/cli/user_settings/jwt_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/utils/get_api_client.py` & `cycode-1.9.5.dev3/cycode/cli/utils/get_api_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/utils/path_utils.py` & `cycode-1.9.5.dev3/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/utils/progress_bar.py` & `cycode-1.9.5.dev3/cycode/cli/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/utils/scan_batch.py` & `cycode-1.9.5.dev3/cycode/cli/utils/scan_batch.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/utils/shell_executor.py` & `cycode-1.9.5.dev3/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/utils/string_utils.py` & `cycode-1.9.5.dev3/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/utils/task_timer.py` & `cycode-1.9.5.dev3/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cli/utils/yaml_utils.py` & `cycode-1.9.5.dev3/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/auth_client.py` & `cycode-1.9.5.dev3/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/client_creator.py` & `cycode-1.9.5.dev3/cycode/cyclient/client_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/config.py` & `cycode-1.9.5.dev3/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/cycode_client_base.py` & `cycode-1.9.5.dev3/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/cycode_dev_based_client.py` & `cycode-1.9.5.dev3/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/cycode_token_based_client.py` & `cycode-1.9.5.dev3/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/headers.py` & `cycode-1.9.5.dev3/cycode/cyclient/headers.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/models.py` & `cycode-1.9.5.dev3/cycode/cyclient/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 
 class DetectionSchema(Schema):
     class Meta:
         unknown = EXCLUDE
 
     message = fields.String()
     type = fields.String()
-    severity = fields.String(missing='High')
-    # TODO(MarshalX): Remove "missing" arg when IaC and Secrets scans will have classifications
+    severity = fields.String(missing=None)
     detection_type_id = fields.String()
     detection_details = fields.Dict()
     detection_rule_id = fields.String()
 
     @post_load
     def build_dto(self, data: Dict[str, Any], **_) -> Detection:
         return Detection(**data)
```

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/report_client.py` & `cycode-1.9.5.dev3/cycode/cyclient/report_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/scan_client.py` & `cycode-1.9.5.dev3/cycode/cyclient/scan_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         response = self.scan_cycode_client.get(url_path=path)
         return models.ScanDetailsResponseSchema().load(response.json())
 
     def get_detection_rules_path(self) -> str:
         return (
             f'{self.scan_config.get_detections_prefix()}/'
             f'{self.POLICIES_SERVICE_CONTROLLER_PATH_V3}/'
-            f'detection_rules'
+            f'detection_rules/byIds'
         )
 
     @staticmethod
     def _get_policy_type_by_scan_type(scan_type: str) -> str:
         scan_type_to_policy_type = {
             consts.INFRA_CONFIGURATION_SCAN_TYPE: 'IaC',
             consts.SCA_SCAN_TYPE: 'SCA',
@@ -178,43 +178,25 @@
 
         if scan_type not in scan_type_to_policy_type:
             raise CycodeError('Invalid scan type')
 
         return scan_type_to_policy_type[scan_type]
 
     @staticmethod
-    def _filter_detection_rules_by_ids(
-        detection_rules: List[models.DetectionRule], detection_rules_ids: Union[Set[str], List[str]]
-    ) -> List[models.DetectionRule]:
-        ids = set(detection_rules_ids)  # cast to set to perform faster search
-        return [rule for rule in detection_rules if rule.detection_rule_id in ids]
-
-    @staticmethod
     def parse_detection_rules_response(response: Response) -> List[models.DetectionRule]:
         return models.DetectionRuleSchema().load(response.json(), many=True)
 
-    def get_detection_rules(
-        self, scan_type: str, detection_rules_ids: Union[Set[str], List[str]]
-    ) -> List[models.DetectionRule]:
-        # TODO(MarshalX): use filter by list of IDs instead of policy_type when BE will be ready
-        params = {
-            'include_hidden': False,
-            'include_only_enabled_detection_rules': True,
-            'page_number': 0,
-            'page_size': 5000,
-            'policy_types_v2': self._get_policy_type_by_scan_type(scan_type),
-        }
+    def get_detection_rules(self, detection_rules_ids: Union[Set[str], List[str]]) -> List[models.DetectionRule]:
         response = self.scan_cycode_client.get(
             url_path=self.get_detection_rules_path(),
-            params=params,
+            params={'ids': detection_rules_ids},
             hide_response_content_log=self._hide_response_log,
         )
 
-        # we are filtering rules by ids in-place for smooth migration when backend will be ready
-        return self._filter_detection_rules_by_ids(self.parse_detection_rules_response(response), detection_rules_ids)
+        return self.parse_detection_rules_response(response)
 
     def get_scan_detections_path(self, scan_type: str) -> str:
         return f'{self.scan_config.get_detections_prefix()}/{self.get_detections_service_controller_path(scan_type)}'
 
     @staticmethod
     def get_scan_detections_list_path_suffix(scan_type: str) -> str:
         # we don't use async flow for IaC scan yet
```

### Comparing `cycode-1.9.5.dev2/cycode/cyclient/scan_config_base.py` & `cycode-1.9.5.dev3/cycode/cyclient/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.5.dev2/pyproject.toml` & `cycode-1.9.5.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "1.9.5.dev2" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "1.9.5.dev3" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning."
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-1.9.5.dev2/PKG-INFO` & `cycode-1.9.5.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 1.9.5.dev2
+Version: 1.9.5.dev3
 Summary: Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning.
 Home-page: https://github.com/cycodehq/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.13
```

