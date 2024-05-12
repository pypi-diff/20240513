# Comparing `tmp/smartExecutorx-4.0.0.tar.gz` & `tmp/smartExecutorx-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartExecutorx-4.0.0.tar", last modified: Wed May  1 17:35:25 2024, max compression
+gzip compressed data, was "smartExecutorx-4.1.tar", last modified: Sun May 12 23:15:25 2024, max compression
```

## Comparing `smartExecutorx-4.0.0.tar` & `smartExecutorx-4.1.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.119751 smartExecutorx-4.0.0/
--rw-rw-rw-   0        0        0     1112 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/LICENSE
--rw-rw-rw-   0        0        0      112 2023-10-09 05:58:34.000000 smartExecutorx-4.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5878 2024-05-01 17:35:25.119751 smartExecutorx-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5091 2024-05-01 11:40:16.000000 smartExecutorx-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.912821 smartExecutorx-4.0.0/fdg/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/fdg/__init__.py
--rw-rw-rw-   0        0        0       21 2024-05-01 04:56:29.000000 smartExecutorx-4.0.0/fdg/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.928331 smartExecutorx-4.0.0/fdg/control/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/fdg/control/__init__.py
--rw-rw-rw-   0        0        0    13717 2024-04-30 03:03:58.000000 smartExecutorx-4.0.0/fdg/control/ftn_search_strategy.py
--rw-rw-rw-   0        0        0    12289 2023-11-07 20:50:26.000000 smartExecutorx-4.0.0/fdg/control/function_assignment.py
--rw-rw-rw-   0        0        0     9908 2024-04-30 03:03:58.000000 smartExecutorx-4.0.0/fdg/control/guider.py
--rw-rw-rw-   0        0        0    23756 2024-04-30 11:17:07.000000 smartExecutorx-4.0.0/fdg/control/mine.py
--rw-rw-rw-   0        0        0     2219 2023-10-30 22:15:11.000000 smartExecutorx-4.0.0/fdg/control/weight_computation.py
--rw-rw-rw-   0        0        0     6308 2024-04-30 11:09:14.000000 smartExecutorx-4.0.0/fdg/expression_slot.py
--rw-rw-rw-   0        0        0    14495 2024-05-01 04:56:29.000000 smartExecutorx-4.0.0/fdg/fdg_pruner.py
--rw-rw-rw-   0        0        0     5658 2024-04-30 03:03:58.000000 smartExecutorx-4.0.0/fdg/function_coverage.py
--rw-rw-rw-   0        0        0    13147 2024-05-01 04:27:00.000000 smartExecutorx-4.0.0/fdg/fwrg_manager.py
--rw-rw-rw-   0        0        0     3263 2024-04-30 03:03:58.000000 smartExecutorx-4.0.0/fdg/global_config.py
--rw-rw-rw-   0        0        0    16303 2024-04-17 02:45:47.000000 smartExecutorx-4.0.0/fdg/instruction_modification.py
--rw-rw-rw-   0        0        0     9534 2023-11-05 22:48:36.000000 smartExecutorx-4.0.0/fdg/output_data.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.940341 smartExecutorx-4.0.0/fdg/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/fdg/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2028 2023-10-16 02:38:03.000000 smartExecutorx-4.0.0/fdg/preprocessing/address_collection.py
--rw-rw-rw-   0        0        0     4959 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/fdg/preprocessing/instruction_coverage.py
--rw-rw-rw-   0        0        0     4583 2024-04-17 02:45:47.000000 smartExecutorx-4.0.0/fdg/preprocessing/preprocess.py
--rw-rw-rw-   0        0        0     3149 2024-04-17 02:45:47.000000 smartExecutorx-4.0.0/fdg/preprocessing/read_in_conditions.py
--rw-rw-rw-   0        0        0     7945 2024-04-17 02:45:47.000000 smartExecutorx-4.0.0/fdg/preprocessing/slot_location.py
--rw-rw-rw-   0        0        0     4215 2023-11-01 01:55:38.000000 smartExecutorx-4.0.0/fdg/preprocessing/write_read_info.py
--rw-rw-rw-   0        0        0     4182 2024-05-01 04:56:29.000000 smartExecutorx-4.0.0/fdg/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.942366 smartExecutorx-4.0.0/mythril/
--rw-rw-rw-   0        0        0      371 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/__init__.py
--rw-rw-rw-   0        0        0      145 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/__main__.py
--rw-rw-rw-   0        0        0      265 2024-05-01 03:09:12.000000 smartExecutorx-4.0.0/mythril/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.952382 smartExecutorx-4.0.0/mythril/analysis/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/analysis_args.py
--rw-rw-rw-   0        0        0     1847 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/call_helpers.py
--rw-rw-rw-   0        0        0     7045 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/callgraph.py
--rw-rw-rw-   0        0        0     1067 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/issue_annotation.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.961005 smartExecutorx-4.0.0/mythril/analysis/module/
--rw-rw-rw-   0        0        0      236 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/__init__.py
--rw-rw-rw-   0        0        0     4358 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/base.py
--rw-rw-rw-   0        0        0     4187 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/loader.py
--rw-rw-rw-   0        0        0      407 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/module_helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.976093 smartExecutorx-4.0.0/mythril/analysis/module/modules/
--rw-rw-rw-   0        0        0        2 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/__init__.py
--rw-rw-rw-   0        0        0     3738 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/arbitrary_jump.py
--rw-rw-rw-   0        0        0     2594 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/arbitrary_write.py
--rw-rw-rw-   0        0        0     3761 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/delegatecall.py
--rw-rw-rw-   0        0        0     4068 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/dependence_on_origin.py
--rw-rw-rw-   0        0        0     7652 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/dependence_on_predictable_vars.py
--rw-rw-rw-   0        0        0     3601 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/ether_thief.py
--rw-rw-rw-   0        0        0     5319 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/exceptions.py
--rw-rw-rw-   0        0        0     4033 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/external_calls.py
--rw-rw-rw-   0        0        0    11819 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/integer.py
--rw-rw-rw-   0        0        0     4353 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/multiple_sends.py
--rw-rw-rw-   0        0        0     7843 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/state_change_external_calls.py
--rw-rw-rw-   0        0        0     4793 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/suicide.py
--rw-rw-rw-   0        0        0     5791 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/unchecked_retval.py
--rw-rw-rw-   0        0        0     4303 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/modules/user_assertions.py
--rw-rw-rw-   0        0        0     2006 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/module/util.py
--rw-rw-rw-   0        0        0     1915 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/ops.py
--rw-rw-rw-   0        0        0     4506 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/potential_issues.py
--rw-rw-rw-   0        0        0    12882 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/report.py
--rw-rw-rw-   0        0        0     1535 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/security.py
--rw-rw-rw-   0        0        0     9558 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/solver.py
--rw-rw-rw-   0        0        0     2452 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/swc_data.py
--rw-rw-rw-   0        0        0    12997 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/symbolic.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.980540 smartExecutorx-4.0.0/mythril/analysis/templates/
--rw-rw-rw-   0        0        0     2262 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/templates/callgraph.html
--rw-rw-rw-   0        0        0     2075 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/templates/report_as_markdown.jinja2
--rw-rw-rw-   0        0        0     1954 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/templates/report_as_text.jinja2
--rw-rw-rw-   0        0        0     4902 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/analysis/traceexplore.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.980540 smartExecutorx-4.0.0/mythril/concolic/
--rw-rw-rw-   0        0        0      128 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/concolic/__init__.py
--rw-rw-rw-   0        0        0     2959 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/concolic/concolic_execution.py
--rw-rw-rw-   0        0        0      645 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/concolic/concrete_data.py
--rw-rw-rw-   0        0        0     3469 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/concolic/find_trace.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.980540 smartExecutorx-4.0.0/mythril/disassembler/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/disassembler/__init__.py
--rw-rw-rw-   0        0        0     4523 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/disassembler/asm.py
--rw-rw-rw-   0        0        0     4770 2023-12-01 18:42:42.000000 smartExecutorx-4.0.0/mythril/disassembler/disassembly.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.992049 smartExecutorx-4.0.0/mythril/ethereum/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/ethereum/__init__.py
--rw-rw-rw-   0        0        0     3282 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/ethereum/evmcontract.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.992049 smartExecutorx-4.0.0/mythril/ethereum/interface/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/ethereum/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.992049 smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/__init__.py
--rw-rw-rw-   0        0        0     2896 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/base_client.py
--rw-rw-rw-   0        0        0     2500 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/client.py
--rw-rw-rw-   0        0        0      248 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/constants.py
--rw-rw-rw-   0        0        0      765 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/exceptions.py
--rw-rw-rw-   0        0        0      991 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/utils.py
--rw-rw-rw-   0        0        0     6534 2023-11-01 14:54:19.000000 smartExecutorx-4.0.0/mythril/ethereum/util.py
--rw-rw-rw-   0        0        0     1175 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.003056 smartExecutorx-4.0.0/mythril/interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/interfaces/__init__.py
--rw-rw-rw-   0        0        0    34731 2024-05-01 03:08:10.000000 smartExecutorx-4.0.0/mythril/interfaces/cli.py
--rw-rw-rw-   0        0        0     7462 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/interfaces/epic.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.003056 smartExecutorx-4.0.0/mythril/laser/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.008082 smartExecutorx-4.0.0/mythril/laser/ethereum/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/__init__.py
--rw-rw-rw-   0        0        0     8985 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/call.py
--rw-rw-rw-   0        0        0     2825 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/cfg.py
--rw-rw-rw-   0        0        0     1924 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/cheat_code.py
--rw-rw-rw-   0        0        0      936 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/evm_exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.008082 smartExecutorx-4.0.0/mythril/laser/ethereum/function_managers/
--rw-rw-rw-   0        0        0      151 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/function_managers/__init__.py
--rw-rw-rw-   0        0        0     2291 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/function_managers/exponent_function_manager.py
--rw-rw-rw-   0        0        0     7644 2023-10-30 20:54:42.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/function_managers/keccak_function_manager.py
--rw-rw-rw-   0        0        0     1447 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/instruction_data.py
--rw-rw-rw-   0        0        0    87355 2023-10-30 20:54:42.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/instructions.py
--rw-rw-rw-   0        0        0     8063 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/natives.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.008082 smartExecutorx-4.0.0/mythril/laser/ethereum/state/
--rw-rw-rw-   0        0        0       10 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/__init__.py
--rw-rw-rw-   0        0        0     7426 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/account.py
--rw-rw-rw-   0        0        0     2200 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/annotation.py
--rw-rw-rw-   0        0        0    10018 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/calldata.py
--rw-rw-rw-   0        0        0     4489 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/constraints.py
--rw-rw-rw-   0        0        0     2152 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/environment.py
--rw-rw-rw-   0        0        0     5814 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/global_state.py
--rw-rw-rw-   0        0        0     8218 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/machine_state.py
--rw-rw-rw-   0        0        0     8877 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/memory.py
--rw-rw-rw-   0        0        0      742 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/return_data.py
--rw-rw-rw-   0        0        0     9119 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/state/world_state.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.023708 smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/
--rw-rw-rw-   0        0        0     1583 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/__init__.py
--rw-rw-rw-   0        0        0     3639 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/basic.py
--rw-rw-rw-   0        0        0     1266 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/beam.py
--rw-rw-rw-   0        0        0     5023 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/concolic.py
--rw-rw-rw-   0        0        0     1799 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/constraint_strategy.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.023708 smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/extensions/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/extensions/__init__.py
--rw-rw-rw-   0        0        0     4546 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/extensions/bounded_loops.py
--rw-rw-rw-   0        0        0    40658 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/svm.py
--rw-rw-rw-   0        0        0      521 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/time_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.023708 smartExecutorx-4.0.0/mythril/laser/ethereum/transaction/
--rw-rw-rw-   0        0        0      190 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/transaction/__init__.py
--rw-rw-rw-   0        0        0     5546 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/transaction/concolic.py
--rw-rw-rw-   0        0        0    10799 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/transaction/symbolic.py
--rw-rw-rw-   0        0        0    10038 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/transaction/transaction_models.py
--rw-rw-rw-   0        0        0     5023 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/ethereum/util.py
--rw-rw-rw-   0        0        0      284 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/execution_info.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.033217 smartExecutorx-4.0.0/mythril/laser/plugin/
--rw-rw-rw-   0        0        0      754 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/__init__.py
--rw-rw-rw-   0        0        0      454 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/builder.py
--rw-rw-rw-   0        0        0      939 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/interface.py
--rw-rw-rw-   0        0        0     3826 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.040239 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/
--rw-rw-rw-   0        0        0      623 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/__init__.py
--rw-rw-rw-   0        0        0     2867 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/benchmark.py
--rw-rw-rw-   0        0        0     1036 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/call_depth_limiter.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.041258 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/coverage/
--rw-rw-rw-   0        0        0      104 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/coverage/__init__.py
--rw-rw-rw-   0        0        0     4401 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/coverage/coverage_plugin.py
--rw-rw-rw-   0        0        0     1869 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/coverage/coverage_strategy.py
--rw-rw-rw-   0        0        0    12968 2024-02-04 06:04:24.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/dependency_pruner.py
--rw-rw-rw-   0        0        0     3745 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/instruction_profiler.py
--rw-rw-rw-   0        0        0     3574 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/mutation_pruner.py
--rw-rw-rw-   0        0        0     4960 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/plugin_annotations.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.041258 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/summary_backup/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/plugins/summary_backup/__init__.py
--rw-rw-rw-   0        0        0      677 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/plugin/signals.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.041258 smartExecutorx-4.0.0/mythril/laser/smt/
--rw-rw-rw-   0        0        0     5236 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/array.py
--rw-rw-rw-   0        0        0     8808 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/bitvec.py
--rw-rw-rw-   0        0        0     6161 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/bitvec_helper.py
--rw-rw-rw-   0        0        0     4130 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/bool.py
--rw-rw-rw-   0        0        0     2386 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/expression.py
--rw-rw-rw-   0        0        0     1133 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/function.py
--rw-rw-rw-   0        0        0     2213 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/model.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.041258 smartExecutorx-4.0.0/mythril/laser/smt/solver/
--rw-rw-rw-   0        0        0      356 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/solver/__init__.py
--rw-rw-rw-   0        0        0     5157 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/solver/independence_solver.py
--rw-rw-rw-   0        0        0     3626 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/solver/solver.py
--rw-rw-rw-   0        0        0     1041 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/laser/smt/solver/solver_statistics.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.052275 smartExecutorx-4.0.0/mythril/mythril/
--rw-rw-rw-   0        0        0      145 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/mythril/__init__.py
--rw-rw-rw-   0        0        0     8065 2024-05-01 04:56:29.000000 smartExecutorx-4.0.0/mythril/mythril/mythril_analyzer.py
--rw-rw-rw-   0        0        0     8198 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/mythril/mythril_config.py
--rw-rw-rw-   0        0        0    15253 2023-10-14 18:03:08.000000 smartExecutorx-4.0.0/mythril/mythril/mythril_disassembler.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.055796 smartExecutorx-4.0.0/mythril/plugin/
--rw-rw-rw-   0        0        0      125 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/plugin/__init__.py
--rw-rw-rw-   0        0        0     2235 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/plugin/discovery.py
--rw-rw-rw-   0        0        0     1441 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/plugin/interface.py
--rw-rw-rw-   0        0        0     2849 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/plugin/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.055796 smartExecutorx-4.0.0/mythril/solidity/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/solidity/__init__.py
--rw-rw-rw-   0        0        0    12703 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/solidity/soliditycontract.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.065819 smartExecutorx-4.0.0/mythril/support/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.065819 smartExecutorx-4.0.0/mythril/support/assets/
--rw-rw-rw-   0        0        0 12406784 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/assets/signatures.db
--rw-rw-rw-   0        0        0     3069 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/loader.py
--rw-rw-rw-   0        0        0     2094 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/lock.py
--rw-rw-rw-   0        0        0     3923 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/model.py
--rw-rw-rw-   0        0        0     7543 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/opcodes.py
--rw-rw-rw-   0        0        0     9223 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/signatures.py
--rw-rw-rw-   0        0        0     2613 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/source_support.py
--rw-rw-rw-   0        0        0      260 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/start_time.py
--rw-rw-rw-   0        0        0      734 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/support_args.py
--rw-rw-rw-   0        0        0     3255 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/mythril/support/support_utils.py
--rw-rw-rw-   0        0        0      695 2024-05-01 16:57:09.000000 smartExecutorx-4.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 17:35:25.124258 smartExecutorx-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4269 2024-05-01 17:35:15.000000 smartExecutorx-4.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.074394 smartExecutorx-4.0.0/smartExecutorx.egg-info/
--rw-rw-rw-   0        0        0     5878 2024-05-01 17:35:24.000000 smartExecutorx-4.0.0/smartExecutorx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7691 2024-05-01 17:35:24.000000 smartExecutorx-4.0.0/smartExecutorx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 17:35:24.000000 smartExecutorx-4.0.0/smartExecutorx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-01 17:35:24.000000 smartExecutorx-4.0.0/smartExecutorx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      695 2024-05-01 17:35:24.000000 smartExecutorx-4.0.0/smartExecutorx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-01 17:35:24.000000 smartExecutorx-4.0.0/smartExecutorx.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:24.908189 smartExecutorx-4.0.0/tests/
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.087969 smartExecutorx-4.0.0/tests/disassembler/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/disassembler/__init__.py
--rw-rw-rw-   0        0        0     3152 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/disassembler/asm.py
--rw-rw-rw-   0        0        0     1728 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/disassembler/disassembly.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.093690 smartExecutorx-4.0.0/tests/instructions/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/__init__.py
--rw-rw-rw-   0        0        0     2747 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/berlin_fork_opcodes_test.py
--rw-rw-rw-   0        0        0     1319 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/codecopy_test.py
--rw-rw-rw-   0        0        0     2579 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/create2_test.py
--rw-rw-rw-   0        0        0     1947 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/create_test.py
--rw-rw-rw-   0        0        0     2295 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/extcodecopy_test.py
--rw-rw-rw-   0        0        0     2015 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/extcodehash_test.py
--rw-rw-rw-   0        0        0     5835 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/sar_test.py
--rw-rw-rw-   0        0        0     4698 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/shl_test.py
--rw-rw-rw-   0        0        0     4763 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/shr_test.py
--rw-rw-rw-   0        0        0     4067 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/static_call_test.py
--rw-rw-rw-   0        0        0     1393 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/instructions/test_basefee.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.106730 smartExecutorx-4.0.0/tests/laser/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0.0/tests/laser/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/keccak_tests.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.107743 smartExecutorx-4.0.0/tests/laser/smt/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/smt/__init__.py
--rw-rw-rw-   0        0        0     3570 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/smt/independece_solver_test.py
--rw-rw-rw-   0        0        0     1189 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/smt/model_test.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.107743 smartExecutorx-4.0.0/tests/laser/state/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/state/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/state/calldata_test.py
--rw-rw-rw-   0        0        0     1327 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/state/mstack_test.py
--rw-rw-rw-   0        0        0     3673 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/state/mstate_test.py
--rw-rw-rw-   0        0        0     1584 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/state/storage_test.py
--rw-rw-rw-   0        0        0     1909 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/state/world_state_account_exist_load_test.py
--rw-rw-rw-   0        0        0     2546 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/test_transaction.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.119751 smartExecutorx-4.0.0/tests/laser/transaction/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/transaction/__init__.py
--rw-rw-rw-   0        0        0     1732 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/transaction/create_transaction_test.py
--rw-rw-rw-   0        0        0     2143 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/laser/transaction/symbolic_test.py
-drwxrwxrwx   0        0        0        0 2024-05-01 17:35:25.119751 smartExecutorx-4.0.0/tests/testdata/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/testdata/__init__.py
--rw-rw-rw-   0        0        0      446 2023-10-09 01:29:56.000000 smartExecutorx-4.0.0/tests/testdata/compile.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.630316 smartExecutorx-4.1/
+-rw-rw-rw-   0        0        0     1112 2023-10-09 01:29:55.000000 smartExecutorx-4.1/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-10-09 05:58:34.000000 smartExecutorx-4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6413 2024-05-12 23:15:25.628306 smartExecutorx-4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5620 2024-05-09 20:51:22.000000 smartExecutorx-4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.428347 smartExecutorx-4.1/fdg/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/fdg/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-05-12 23:14:38.000000 smartExecutorx-4.1/fdg/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.428347 smartExecutorx-4.1/fdg/control/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/fdg/control/__init__.py
+-rw-rw-rw-   0        0        0    12777 2024-05-12 06:56:59.000000 smartExecutorx-4.1/fdg/control/ftn_search_strategy.py
+-rw-rw-rw-   0        0        0    12374 2024-05-12 05:20:26.000000 smartExecutorx-4.1/fdg/control/function_assignment.py
+-rw-rw-rw-   0        0        0     9848 2024-05-12 06:48:26.000000 smartExecutorx-4.1/fdg/control/guider.py
+-rw-rw-rw-   0        0        0    24291 2024-05-09 19:47:05.000000 smartExecutorx-4.1/fdg/control/mine.py
+-rw-rw-rw-   0        0        0     2219 2023-10-30 22:15:11.000000 smartExecutorx-4.1/fdg/control/weight_computation.py
+-rw-rw-rw-   0        0        0     6491 2024-05-05 05:38:36.000000 smartExecutorx-4.1/fdg/expression_slot.py
+-rw-rw-rw-   0        0        0    16463 2024-05-12 06:25:16.000000 smartExecutorx-4.1/fdg/fdg_pruner.py
+-rw-rw-rw-   0        0        0     5658 2024-05-05 05:38:36.000000 smartExecutorx-4.1/fdg/function_coverage.py
+-rw-rw-rw-   0        0        0    13519 2024-05-05 05:38:36.000000 smartExecutorx-4.1/fdg/fwrg_manager.py
+-rw-rw-rw-   0        0        0     3136 2024-05-12 06:19:51.000000 smartExecutorx-4.1/fdg/global_config.py
+-rw-rw-rw-   0        0        0    16303 2024-04-17 02:45:47.000000 smartExecutorx-4.1/fdg/instruction_modification.py
+-rw-rw-rw-   0        0        0     9534 2024-05-05 05:33:47.000000 smartExecutorx-4.1/fdg/output_data.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.445322 smartExecutorx-4.1/fdg/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/fdg/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2028 2023-10-16 02:38:03.000000 smartExecutorx-4.1/fdg/preprocessing/address_collection.py
+-rw-rw-rw-   0        0        0     4959 2023-10-09 01:29:55.000000 smartExecutorx-4.1/fdg/preprocessing/instruction_coverage.py
+-rw-rw-rw-   0        0        0     4583 2024-05-09 19:47:05.000000 smartExecutorx-4.1/fdg/preprocessing/preprocess.py
+-rw-rw-rw-   0        0        0     3149 2024-04-17 02:45:47.000000 smartExecutorx-4.1/fdg/preprocessing/read_in_conditions.py
+-rw-rw-rw-   0        0        0     7945 2024-04-17 02:45:47.000000 smartExecutorx-4.1/fdg/preprocessing/slot_location.py
+-rw-rw-rw-   0        0        0     4215 2023-11-01 01:55:38.000000 smartExecutorx-4.1/fdg/preprocessing/write_read_info.py
+-rw-rw-rw-   0        0        0     4337 2024-05-05 05:38:36.000000 smartExecutorx-4.1/fdg/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.448328 smartExecutorx-4.1/mythril/
+-rw-rw-rw-   0        0        0      371 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/__init__.py
+-rw-rw-rw-   0        0        0      145 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/__main__.py
+-rw-rw-rw-   0        0        0      265 2024-05-12 23:15:08.000000 smartExecutorx-4.1/mythril/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.448328 smartExecutorx-4.1/mythril/analysis/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/analysis_args.py
+-rw-rw-rw-   0        0        0     1847 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/call_helpers.py
+-rw-rw-rw-   0        0        0     7045 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/callgraph.py
+-rw-rw-rw-   0        0        0     1067 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/issue_annotation.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.466356 smartExecutorx-4.1/mythril/analysis/module/
+-rw-rw-rw-   0        0        0      236 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/__init__.py
+-rw-rw-rw-   0        0        0     4358 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/base.py
+-rw-rw-rw-   0        0        0     4187 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/loader.py
+-rw-rw-rw-   0        0        0      407 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/module_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.478594 smartExecutorx-4.1/mythril/analysis/module/modules/
+-rw-rw-rw-   0        0        0        2 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/__init__.py
+-rw-rw-rw-   0        0        0     3738 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/arbitrary_jump.py
+-rw-rw-rw-   0        0        0     2594 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/arbitrary_write.py
+-rw-rw-rw-   0        0        0     3761 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/delegatecall.py
+-rw-rw-rw-   0        0        0     4068 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/dependence_on_origin.py
+-rw-rw-rw-   0        0        0     7652 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/dependence_on_predictable_vars.py
+-rw-rw-rw-   0        0        0     3601 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/ether_thief.py
+-rw-rw-rw-   0        0        0     5319 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/exceptions.py
+-rw-rw-rw-   0        0        0     4033 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/external_calls.py
+-rw-rw-rw-   0        0        0    11819 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/integer.py
+-rw-rw-rw-   0        0        0     4353 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/multiple_sends.py
+-rw-rw-rw-   0        0        0     7843 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/state_change_external_calls.py
+-rw-rw-rw-   0        0        0     4793 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/suicide.py
+-rw-rw-rw-   0        0        0     5791 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/unchecked_retval.py
+-rw-rw-rw-   0        0        0     4303 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/modules/user_assertions.py
+-rw-rw-rw-   0        0        0     2006 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/module/util.py
+-rw-rw-rw-   0        0        0     1915 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/ops.py
+-rw-rw-rw-   0        0        0     4506 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/potential_issues.py
+-rw-rw-rw-   0        0        0    12882 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/report.py
+-rw-rw-rw-   0        0        0     1535 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/security.py
+-rw-rw-rw-   0        0        0     9558 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/solver.py
+-rw-rw-rw-   0        0        0     2452 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/swc_data.py
+-rw-rw-rw-   0        0        0    12997 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/symbolic.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.478594 smartExecutorx-4.1/mythril/analysis/templates/
+-rw-rw-rw-   0        0        0     2262 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/templates/callgraph.html
+-rw-rw-rw-   0        0        0     2075 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/templates/report_as_markdown.jinja2
+-rw-rw-rw-   0        0        0     1954 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/templates/report_as_text.jinja2
+-rw-rw-rw-   0        0        0     4902 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/analysis/traceexplore.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.478594 smartExecutorx-4.1/mythril/concolic/
+-rw-rw-rw-   0        0        0      128 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/concolic/__init__.py
+-rw-rw-rw-   0        0        0     2959 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/concolic/concolic_execution.py
+-rw-rw-rw-   0        0        0      645 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/concolic/concrete_data.py
+-rw-rw-rw-   0        0        0     3469 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/concolic/find_trace.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.478594 smartExecutorx-4.1/mythril/disassembler/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/disassembler/__init__.py
+-rw-rw-rw-   0        0        0     4523 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/disassembler/asm.py
+-rw-rw-rw-   0        0        0     4770 2023-12-01 18:42:42.000000 smartExecutorx-4.1/mythril/disassembler/disassembly.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.497377 smartExecutorx-4.1/mythril/ethereum/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/ethereum/__init__.py
+-rw-rw-rw-   0        0        0     3282 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/ethereum/evmcontract.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.498896 smartExecutorx-4.1/mythril/ethereum/interface/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/ethereum/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.501938 smartExecutorx-4.1/mythril/ethereum/interface/rpc/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/ethereum/interface/rpc/__init__.py
+-rw-rw-rw-   0        0        0     2896 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/ethereum/interface/rpc/base_client.py
+-rw-rw-rw-   0        0        0     2500 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/ethereum/interface/rpc/client.py
+-rw-rw-rw-   0        0        0      248 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/ethereum/interface/rpc/constants.py
+-rw-rw-rw-   0        0        0      765 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/ethereum/interface/rpc/exceptions.py
+-rw-rw-rw-   0        0        0      991 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/ethereum/interface/rpc/utils.py
+-rw-rw-rw-   0        0        0     6534 2023-11-01 14:54:19.000000 smartExecutorx-4.1/mythril/ethereum/util.py
+-rw-rw-rw-   0        0        0     1175 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.501938 smartExecutorx-4.1/mythril/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/interfaces/__init__.py
+-rw-rw-rw-   0        0        0    35354 2024-05-12 06:19:51.000000 smartExecutorx-4.1/mythril/interfaces/cli.py
+-rw-rw-rw-   0        0        0     7462 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/interfaces/epic.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.501938 smartExecutorx-4.1/mythril/laser/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.511630 smartExecutorx-4.1/mythril/laser/ethereum/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/__init__.py
+-rw-rw-rw-   0        0        0     8985 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/call.py
+-rw-rw-rw-   0        0        0     2825 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/cfg.py
+-rw-rw-rw-   0        0        0     1924 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/cheat_code.py
+-rw-rw-rw-   0        0        0      936 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/evm_exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.511630 smartExecutorx-4.1/mythril/laser/ethereum/function_managers/
+-rw-rw-rw-   0        0        0      151 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/function_managers/__init__.py
+-rw-rw-rw-   0        0        0     2291 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/function_managers/exponent_function_manager.py
+-rw-rw-rw-   0        0        0     7644 2023-10-30 20:54:42.000000 smartExecutorx-4.1/mythril/laser/ethereum/function_managers/keccak_function_manager.py
+-rw-rw-rw-   0        0        0     1447 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/instruction_data.py
+-rw-rw-rw-   0        0        0    89995 2024-05-09 19:47:05.000000 smartExecutorx-4.1/mythril/laser/ethereum/instructions.py
+-rw-rw-rw-   0        0        0     8063 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/natives.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.526184 smartExecutorx-4.1/mythril/laser/ethereum/state/
+-rw-rw-rw-   0        0        0       10 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/__init__.py
+-rw-rw-rw-   0        0        0     7426 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/account.py
+-rw-rw-rw-   0        0        0     2200 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/annotation.py
+-rw-rw-rw-   0        0        0    10018 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/calldata.py
+-rw-rw-rw-   0        0        0     4489 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/constraints.py
+-rw-rw-rw-   0        0        0     2152 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/environment.py
+-rw-rw-rw-   0        0        0     5814 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/global_state.py
+-rw-rw-rw-   0        0        0     8218 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/machine_state.py
+-rw-rw-rw-   0        0        0     8877 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/memory.py
+-rw-rw-rw-   0        0        0      742 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/return_data.py
+-rw-rw-rw-   0        0        0     9119 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/state/world_state.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.529947 smartExecutorx-4.1/mythril/laser/ethereum/strategy/
+-rw-rw-rw-   0        0        0     1583 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/strategy/__init__.py
+-rw-rw-rw-   0        0        0     3639 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/strategy/basic.py
+-rw-rw-rw-   0        0        0     1266 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/strategy/beam.py
+-rw-rw-rw-   0        0        0     5023 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/strategy/concolic.py
+-rw-rw-rw-   0        0        0     1799 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/strategy/constraint_strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.529947 smartExecutorx-4.1/mythril/laser/ethereum/strategy/extensions/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/strategy/extensions/__init__.py
+-rw-rw-rw-   0        0        0     4546 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/strategy/extensions/bounded_loops.py
+-rw-rw-rw-   0        0        0    39661 2024-05-12 06:22:23.000000 smartExecutorx-4.1/mythril/laser/ethereum/svm.py
+-rw-rw-rw-   0        0        0      521 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/time_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.539469 smartExecutorx-4.1/mythril/laser/ethereum/transaction/
+-rw-rw-rw-   0        0        0      190 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/transaction/__init__.py
+-rw-rw-rw-   0        0        0     5546 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/transaction/concolic.py
+-rw-rw-rw-   0        0        0    10799 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/transaction/symbolic.py
+-rw-rw-rw-   0        0        0    10038 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/transaction/transaction_models.py
+-rw-rw-rw-   0        0        0     5023 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/ethereum/util.py
+-rw-rw-rw-   0        0        0      284 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/execution_info.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.543475 smartExecutorx-4.1/mythril/laser/plugin/
+-rw-rw-rw-   0        0        0      754 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/__init__.py
+-rw-rw-rw-   0        0        0      454 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/builder.py
+-rw-rw-rw-   0        0        0      939 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/interface.py
+-rw-rw-rw-   0        0        0     3826 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.544885 smartExecutorx-4.1/mythril/laser/plugin/plugins/
+-rw-rw-rw-   0        0        0      623 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/__init__.py
+-rw-rw-rw-   0        0        0     2867 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/benchmark.py
+-rw-rw-rw-   0        0        0     1036 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/call_depth_limiter.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.544885 smartExecutorx-4.1/mythril/laser/plugin/plugins/coverage/
+-rw-rw-rw-   0        0        0      104 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/coverage/__init__.py
+-rw-rw-rw-   0        0        0     4401 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/coverage/coverage_plugin.py
+-rw-rw-rw-   0        0        0     1869 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/coverage/coverage_strategy.py
+-rw-rw-rw-   0        0        0    12968 2024-02-04 06:04:24.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/dependency_pruner.py
+-rw-rw-rw-   0        0        0     3745 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/instruction_profiler.py
+-rw-rw-rw-   0        0        0     3574 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/mutation_pruner.py
+-rw-rw-rw-   0        0        0     4960 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/plugin_annotations.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.544885 smartExecutorx-4.1/mythril/laser/plugin/plugins/summary_backup/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/plugins/summary_backup/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/plugin/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.560707 smartExecutorx-4.1/mythril/laser/smt/
+-rw-rw-rw-   0        0        0     5236 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/array.py
+-rw-rw-rw-   0        0        0     8808 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/bitvec.py
+-rw-rw-rw-   0        0        0     6161 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/bitvec_helper.py
+-rw-rw-rw-   0        0        0     4130 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/bool.py
+-rw-rw-rw-   0        0        0     2386 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/expression.py
+-rw-rw-rw-   0        0        0     1133 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/function.py
+-rw-rw-rw-   0        0        0     2213 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/model.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.562252 smartExecutorx-4.1/mythril/laser/smt/solver/
+-rw-rw-rw-   0        0        0      356 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/solver/__init__.py
+-rw-rw-rw-   0        0        0     5157 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/solver/independence_solver.py
+-rw-rw-rw-   0        0        0     3626 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/solver/solver.py
+-rw-rw-rw-   0        0        0     1041 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/laser/smt/solver/solver_statistics.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.562252 smartExecutorx-4.1/mythril/mythril/
+-rw-rw-rw-   0        0        0      145 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/mythril/__init__.py
+-rw-rw-rw-   0        0        0     8269 2024-05-05 05:38:36.000000 smartExecutorx-4.1/mythril/mythril/mythril_analyzer.py
+-rw-rw-rw-   0        0        0     8198 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/mythril/mythril_config.py
+-rw-rw-rw-   0        0        0    15253 2023-10-14 18:03:08.000000 smartExecutorx-4.1/mythril/mythril/mythril_disassembler.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.569759 smartExecutorx-4.1/mythril/plugin/
+-rw-rw-rw-   0        0        0      125 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/plugin/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/plugin/discovery.py
+-rw-rw-rw-   0        0        0     1441 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/plugin/interface.py
+-rw-rw-rw-   0        0        0     2849 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/plugin/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.569759 smartExecutorx-4.1/mythril/solidity/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/solidity/__init__.py
+-rw-rw-rw-   0        0        0    12703 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/solidity/soliditycontract.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.578129 smartExecutorx-4.1/mythril/support/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.578129 smartExecutorx-4.1/mythril/support/assets/
+-rw-rw-rw-   0        0        0 12406784 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/assets/signatures.db
+-rw-rw-rw-   0        0        0     3069 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/loader.py
+-rw-rw-rw-   0        0        0     2094 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/lock.py
+-rw-rw-rw-   0        0        0     3923 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/model.py
+-rw-rw-rw-   0        0        0     7543 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/opcodes.py
+-rw-rw-rw-   0        0        0     9223 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/signatures.py
+-rw-rw-rw-   0        0        0     2613 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/source_support.py
+-rw-rw-rw-   0        0        0      260 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/start_time.py
+-rw-rw-rw-   0        0        0      734 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/support_args.py
+-rw-rw-rw-   0        0        0     3255 2023-10-09 01:29:55.000000 smartExecutorx-4.1/mythril/support/support_utils.py
+-rw-rw-rw-   0        0        0      736 2024-05-05 05:38:36.000000 smartExecutorx-4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 23:15:25.630316 smartExecutorx-4.1/setup.cfg
+-rw-rw-rw-   0        0        0     4267 2024-05-12 23:15:08.000000 smartExecutorx-4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.602326 smartExecutorx-4.1/smartExecutorx.egg-info/
+-rw-rw-rw-   0        0        0     6413 2024-05-12 23:15:25.000000 smartExecutorx-4.1/smartExecutorx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7691 2024-05-12 23:15:25.000000 smartExecutorx-4.1/smartExecutorx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 23:15:25.000000 smartExecutorx-4.1/smartExecutorx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-12 23:15:25.000000 smartExecutorx-4.1/smartExecutorx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      695 2024-05-12 23:15:25.000000 smartExecutorx-4.1/smartExecutorx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-12 23:15:25.000000 smartExecutorx-4.1/smartExecutorx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.418127 smartExecutorx-4.1/tests/
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.602326 smartExecutorx-4.1/tests/disassembler/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/disassembler/__init__.py
+-rw-rw-rw-   0        0        0     3152 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/disassembler/asm.py
+-rw-rw-rw-   0        0        0     1728 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/disassembler/disassembly.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.612259 smartExecutorx-4.1/tests/instructions/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/__init__.py
+-rw-rw-rw-   0        0        0     2747 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/berlin_fork_opcodes_test.py
+-rw-rw-rw-   0        0        0     1319 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/codecopy_test.py
+-rw-rw-rw-   0        0        0     2579 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/create2_test.py
+-rw-rw-rw-   0        0        0     1947 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/create_test.py
+-rw-rw-rw-   0        0        0     2295 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/extcodecopy_test.py
+-rw-rw-rw-   0        0        0     2015 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/extcodehash_test.py
+-rw-rw-rw-   0        0        0     5835 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/sar_test.py
+-rw-rw-rw-   0        0        0     4698 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/shl_test.py
+-rw-rw-rw-   0        0        0     4763 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/shr_test.py
+-rw-rw-rw-   0        0        0     4067 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/static_call_test.py
+-rw-rw-rw-   0        0        0     1393 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/instructions/test_basefee.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.612259 smartExecutorx-4.1/tests/laser/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.1/tests/laser/__init__.py
+-rw-rw-rw-   0        0        0     4300 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/keccak_tests.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.612259 smartExecutorx-4.1/tests/laser/smt/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/smt/__init__.py
+-rw-rw-rw-   0        0        0     3570 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/smt/independece_solver_test.py
+-rw-rw-rw-   0        0        0     1189 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/smt/model_test.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.622337 smartExecutorx-4.1/tests/laser/state/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/state/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/state/calldata_test.py
+-rw-rw-rw-   0        0        0     1327 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/state/mstack_test.py
+-rw-rw-rw-   0        0        0     3673 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/state/mstate_test.py
+-rw-rw-rw-   0        0        0     1584 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/state/storage_test.py
+-rw-rw-rw-   0        0        0     1909 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/state/world_state_account_exist_load_test.py
+-rw-rw-rw-   0        0        0     2546 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/test_transaction.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.625527 smartExecutorx-4.1/tests/laser/transaction/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/transaction/__init__.py
+-rw-rw-rw-   0        0        0     1732 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/transaction/create_transaction_test.py
+-rw-rw-rw-   0        0        0     2143 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/laser/transaction/symbolic_test.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:15:25.627796 smartExecutorx-4.1/tests/testdata/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/testdata/__init__.py
+-rw-rw-rw-   0        0        0      446 2023-10-09 01:29:56.000000 smartExecutorx-4.1/tests/testdata/compile.py
```

### Comparing `smartExecutorx-4.0.0/LICENSE` & `smartExecutorx-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/PKG-INFO` & `smartExecutorx-4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartExecutorx
-Version: 4.0.0
+Version: 4.1
 Summary: Security analysis tool for Ethereum smart contracts
 Home-page: https://github.com/contractAnalysis/smartExecutor
 Author: contractAnalysis
 License: MIT
 Keywords: hacking disassembler security ethereum
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -21,41 +21,41 @@
 ##  SmartExecutor ##
 
 SmartExecutor is a guided symbolic execution tool for security analysis on EVM bytecode. It is designed to reduce the sequence explosion of symbolic execution to provide a scalable solution to symbolic execution while trying to maximize code coverage.  It has a dual-phase process. In Phase 1, it symbolically executes all possible function sequences within the given depth limit.
 
 Phase 2 then targets the not-fully-covered functions based on instruction coverage. This is the phase where the guidance takes place. SmartExecutor can direct the execution flow by prioritizing the states more significant to the target functions and selecting the functions at states to be executed that are more likely to cover the targets. The state significance value calculation and the function selection are based on static data dependency analysis and runtime execution data like function coverage and target functions.
 
 
-This is the [link](https://ieeexplore.ieee.org/document/10316942) to our conference paper: SmartExecutor: Coverage-Driven Symbolic Execution Guided by a Function Dependency Graph. 
+This is the [link](https://ieeexplore.ieee.org/document/10316942) to our conference paper: SmartExecutor: Coverage-Driven Symbolic Execution Guided by a Function Dependency Graph. The [documentation](https://page.d1xp6o5ammny8t.amplifyapp.com/) is available.
 
 
 
 ###  Run SmartExecutor through Docker: 
 
 1, Pull the Docker image of SmartExecutor:
 ```bash
 $ sudo docker pull 23278942/smartexecutor
 ```
 
 2, Run SmartExecutor with a single Docker command. Replace a_host_directory with the path to your host directory containing the Solidity file, for example, Crowdsale.sol.
 ```bash
-$ sudo docker run -it --rm -v a_host_directory:/home/smartExecutor/ image_id analyze ./Crowdsale.sol:Crowdsale
+$ sudo docker run -it --rm -v a_host_directory:/home/smartExecutor/ --entrypoint semyth 3278942/smartexecutor:latest analyze ./Crowdsale.sol:Crowdsale
 ```
 This command mounts the host directory to a directory inside the container and analyzes the contract Crowdsale defined in the Solidity file Crowdsale.sol.
 
 To analyze the sample Solidity file provided with the Docker image, you can use the following command:
 ```bash
-$ sudo docker run -it --rm image_id analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
+$ sudo docker run -it --rm --entrypoint semyth 3278942/smartexecutor:latest analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
 ```
 
 3, Additional Options
 
 To see more intermediate data, add the -v option followed by a value (3 or larger):
 ```bash
-$ sudo docker run -it --rm image_id -v 3 analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
+$ sudo docker run -it --rm --entrypoint semyth 3278942/smartexecutor:latest -v 3 analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
 ```
 
 Click [here](./example_output/Crowdsale.sol_terminal_output.txt) to see the terminal output.
 
 Click [here](./example_output/Crowdsale.sol_terminal_output_verbose.txt) to see the verbose intermediate results printed out in the terminal.
 
 <!--
@@ -70,14 +70,22 @@
 # set option '-v' to 3 to show the verbose intermediate results
 semyth -v 3 analyze ./Crowdsale.sol:Crowdsale 
 
 ```
 -->
 
 
+### Install solc-select and all versions of solc
+```
+pip install solc-select  # solc-select is a package to switch among different versions of solc (Solidity compiler)
+solc-select install all  # install all possible versions of solc 
+solc-select use 0.4.25   # example of using solc-select: set the version of solc to 0.4.25
+```
+
+
 ### Run SmartExecutor in Pycharm IDE:
 
 1, Create a project through Pycharm IDE by cloning https://github.com/contractAnalysis/smartExecutor.git.
 
 2, Create a virtual environment and install dependencies.
 
 3, Find semyth.py in the root directory and add the parameters. Take the example of Crowdsale.sol:
@@ -108,15 +116,15 @@
 For this reason, here show some useful documents of Mythril:
 
 - [Instructions for using Mythril](https://mythril-classic.readthedocs.io/en/master/)
 - [Mythril's documentation](https://mythril-classic.readthedocs.io/en/develop/)
 - [Vulnerability Remediation](https://swcregistry.io/)
 -->
 If you find this tool helpful, we would appreciate it if you could cite it. Here is the BibTex:
-```json
+```text
 @INPROCEEDINGS{10316942,
   author={Wei, Qiping and Sikder, Fadul and Feng, Huadong and Lei, Yu and Kacker, Raghu and Kuhn, Richard},
   booktitle={2023 5th Conference on Blockchain Research & Applications for Innovative Networks and Services (BRAINS)}, 
   title={SmartExecutor: Coverage-Driven Symbolic Execution Guided by a Function Dependency Graph}, 
   year={2023},
   volume={},
   number={},
```

### Comparing `smartExecutorx-4.0.0/README.md` & `smartExecutorx-4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 ##  SmartExecutor ##
 
 SmartExecutor is a guided symbolic execution tool for security analysis on EVM bytecode. It is designed to reduce the sequence explosion of symbolic execution to provide a scalable solution to symbolic execution while trying to maximize code coverage.  It has a dual-phase process. In Phase 1, it symbolically executes all possible function sequences within the given depth limit.
 
 Phase 2 then targets the not-fully-covered functions based on instruction coverage. This is the phase where the guidance takes place. SmartExecutor can direct the execution flow by prioritizing the states more significant to the target functions and selecting the functions at states to be executed that are more likely to cover the targets. The state significance value calculation and the function selection are based on static data dependency analysis and runtime execution data like function coverage and target functions.
 
 
-This is the [link](https://ieeexplore.ieee.org/document/10316942) to our conference paper: SmartExecutor: Coverage-Driven Symbolic Execution Guided by a Function Dependency Graph. 
+This is the [link](https://ieeexplore.ieee.org/document/10316942) to our conference paper: SmartExecutor: Coverage-Driven Symbolic Execution Guided by a Function Dependency Graph. The [documentation](https://page.d1xp6o5ammny8t.amplifyapp.com/) is available.
 
 
 
 ###  Run SmartExecutor through Docker: 
 
 1, Pull the Docker image of SmartExecutor:
 ```bash
 $ sudo docker pull 23278942/smartexecutor
 ```
 
 2, Run SmartExecutor with a single Docker command. Replace a_host_directory with the path to your host directory containing the Solidity file, for example, Crowdsale.sol.
 ```bash
-$ sudo docker run -it --rm -v a_host_directory:/home/smartExecutor/ image_id analyze ./Crowdsale.sol:Crowdsale
+$ sudo docker run -it --rm -v a_host_directory:/home/smartExecutor/ --entrypoint semyth 3278942/smartexecutor:latest analyze ./Crowdsale.sol:Crowdsale
 ```
 This command mounts the host directory to a directory inside the container and analyzes the contract Crowdsale defined in the Solidity file Crowdsale.sol.
 
 To analyze the sample Solidity file provided with the Docker image, you can use the following command:
 ```bash
-$ sudo docker run -it --rm image_id analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
+$ sudo docker run -it --rm --entrypoint semyth 3278942/smartexecutor:latest analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
 ```
 
 3, Additional Options
 
 To see more intermediate data, add the -v option followed by a value (3 or larger):
 ```bash
-$ sudo docker run -it --rm image_id -v 3 analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
+$ sudo docker run -it --rm --entrypoint semyth 3278942/smartexecutor:latest -v 3 analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
 ```
 
 Click [here](./example_output/Crowdsale.sol_terminal_output.txt) to see the terminal output.
 
 Click [here](./example_output/Crowdsale.sol_terminal_output_verbose.txt) to see the verbose intermediate results printed out in the terminal.
 
 <!--
@@ -51,14 +51,22 @@
 # set option '-v' to 3 to show the verbose intermediate results
 semyth -v 3 analyze ./Crowdsale.sol:Crowdsale 
 
 ```
 -->
 
 
+### Install solc-select and all versions of solc
+```
+pip install solc-select  # solc-select is a package to switch among different versions of solc (Solidity compiler)
+solc-select install all  # install all possible versions of solc 
+solc-select use 0.4.25   # example of using solc-select: set the version of solc to 0.4.25
+```
+
+
 ### Run SmartExecutor in Pycharm IDE:
 
 1, Create a project through Pycharm IDE by cloning https://github.com/contractAnalysis/smartExecutor.git.
 
 2, Create a virtual environment and install dependencies.
 
 3, Find semyth.py in the root directory and add the parameters. Take the example of Crowdsale.sol:
@@ -89,15 +97,15 @@
 For this reason, here show some useful documents of Mythril:
 
 - [Instructions for using Mythril](https://mythril-classic.readthedocs.io/en/master/)
 - [Mythril's documentation](https://mythril-classic.readthedocs.io/en/develop/)
 - [Vulnerability Remediation](https://swcregistry.io/)
 -->
 If you find this tool helpful, we would appreciate it if you could cite it. Here is the BibTex:
-```json
+```text
 @INPROCEEDINGS{10316942,
   author={Wei, Qiping and Sikder, Fadul and Feng, Huadong and Lei, Yu and Kacker, Raghu and Kuhn, Richard},
   booktitle={2023 5th Conference on Blockchain Research & Applications for Innovative Networks and Services (BRAINS)}, 
   title={SmartExecutor: Coverage-Driven Symbolic Execution Guided by a Function Dependency Graph}, 
   year={2023},
   volume={},
   number={},
```

### Comparing `smartExecutorx-4.0.0/fdg/control/ftn_search_strategy.py` & `smartExecutorx-4.1/fdg/control/ftn_search_strategy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,368 +1,353 @@
-import ast
-
-from copy import deepcopy
-
-
-import fdg.global_config
-from fdg.control.function_assignment import FunctionAssignment
-
-from fdg.fwrg_manager import FWRG_manager
-from fdg.output_data import print_data_for_bfs_strategy, print_data_for_dfs_strategy
-
-from fdg.utils import get_ftn_seq_from_key_1
-
-
-
-
-class FunctionSearchStrategy():
-    def __init__(self,strategy_name:str):
-        self.name=strategy_name
-        self.world_states={}
-        self.search_history={}
-        self.current_state_key=''
-        # print(f'search strategy: {self.name}')
-
-    def save_states(self,key:str,states:list):
-        if key in self.world_states.keys():
-            self.world_states[key]+=states
-        else:
-            self.world_states[key]=states
-    def get_states(self,key:str):
-        if key in self.world_states.keys():
-            return self.world_states[key]
-        else:
-            return []
-    def delete_state(self,key:str):
-        if key in self.world_states.keys():
-            self.world_states.pop(key)
-
-    def assign_states(self, deep_functions: list=None, current_state_key: str = None, fdfg: FWRG_manager = None,
-                      states_dict: dict = {},iteration:int=0) -> list:
-        pass
-
-
-
-    def termination(self,states_num:int=0,current_seq_length:int=0,sequence_depth_limit:int=0,iteration:int=0)->bool:
-        ...
-
-
-
-class Seq(FunctionSearchStrategy):
-    def __init__(self):
-        self.queue = []
-
-        # # 0x00c0443f42932d9efe27e64409b21d2e48928d66.sol	0.5.8	JarvisExchange
-        # self.sequences = [
-        #     ['setController(address)', 'withdrawToken(address,uint256,uint256)']
-        # ]
-
-        # 0x9afb9d7ed0f6c054ec76ea61d5cabc384d4dcb25.sol	0.4.26	ConverterFactory
-        self.sequences = [
-            ['transferOwnership(address)', 'acceptOwnership()']
-        ]
-        #0x2caf5a42ec2d6747ec696714bf913b174d94fdf0.sol	0.5.17	LexLocker
-        # contain GT, and function signature with 3 bytes
-        self.sequences = [
-            ['updateJudgmentReward(uint256)']
-        ]
-
-        if len(fdg.global_config.sequences)>0:
-            # assume that the sequenes are presented as string
-            self.sequences=ast.literal_eval(fdg.global_config.sequences)
-        else:self.sequences=[]
-
-        super().__init__('seq')
-
-    def initialize(self, main_path_sf: dict, main_path_df: dict, fdfg_manager: FWRG_manager):
-        ...
-
-
-
-
-
-    def termination(self, states_num: int = 0, current_seq_length: int = 0, sequence_depth_limit: int = 0,
-                    iteration: int = 0) -> bool:
-        # need to test
-        if states_num == 0: return True
-        if iteration>2:
-            if len(self.queue) == 0:
-                return True
-        return False
-
-    def assign_states(self, deep_functions: list = None, current_state_key: str = None, fdfg: FWRG_manager = None,
-                      states_dict: dict = {},iteration:int=0) -> list:
-        """
-
-        :param deep_functions:
-        :param current_state_key:
-        :param fdfg:
-        :param states_dict:
-        :return:
-        """
-        if len(states_dict)>0:
-            for key, states in states_dict.items():
-
-                if key not in self.world_states.keys():
-                    self.world_states[key]=deepcopy(states)
-                else:
-                    self.world_states[key]+=deepcopy(states)
-                self.queue.append(key)
-
-        while True:
-            if len(self.queue)==0: return {},False
-            state_key=self.queue.pop(0)
-            if state_key=='constructor':
-                if len(self.sequences)==0:
-                    return {},True
-                return {'constructor':[seq[0] for seq in self.sequences]},True
-
-            seq=get_ftn_seq_from_key_1(state_key)
-            functions=[]
-            for seq_ in self.sequences:
-                if len(seq)==len(seq_):continue
-                if len(seq)<len(seq_):
-                    for i in range(len(seq)):
-                        if seq[i]!=seq_[i]:break
-                    functions.append(seq_[len(seq)])
-            if len(functions)>0:
-                return {state_key:functions},True
-
-
-class DFS(FunctionSearchStrategy):
-    def __init__(self):
-        self.stack=[]
-        self.preprocess_timeout = False
-        self.preprocess_coverage = 0
-        self.flag_one_start_function=False
-        super().__init__('dfs')
-
-    def initialize(self, flag_one_start_function:bool, preprocess_timeout:bool, preprocess_coverage:float, all_functions:list, fwrg_manager:FWRG_manager):
-        self.flag_one_start_function=flag_one_start_function
-        self.preprocess_timeout = preprocess_timeout
-        self.preprocess_coverage = preprocess_coverage
-        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
-
-
-    def termination(self,states_num:int=0, current_seq_length: int = 0, sequence_depth_limit: int = 0,iteration:int=0)->bool:
-        if iteration<=2:
-            if states_num==0:return True
-        return False
-
-
-
-
-
-    def assign_states(self, deep_functions: list=None, states_dict: dict = {},iteration:int=0) -> list:
-
-        """
-            save states, push state keys to the stack
-            select a state by poping an item from the stack
-            assign functions to be executed on the selected state
-        :param deep_functions:
-        :param current_state_key:
-        :param fdfg:
-        :param states_dict:
-        :return:
-        """
-        if len(states_dict)>0:
-            for key, states in states_dict.items():
-                ftn_seq=get_ftn_seq_from_key_1(key)
-                if len(ftn_seq)>=fdg.global_config.seq_len_limit:
-                    continue # do not save these states as they will not be explored
-                # save states
-                self.world_states[key]=deepcopy(states)
-                self.stack.append(key)
-
-        print_data_for_dfs_strategy(self.stack)
-
-        if self.flag_one_start_function:
-            self.flag_one_start_function=False
-            state_key = self.stack.pop()
-            assign_functions = self.functionAssignment.assign_all_functions()
-
-            return {state_key : assign_functions},True
-
-        while True:
-            if len(self.stack)==0:
-                return {},None
-
-            state_key=self.stack.pop()
-
-            if self.preprocess_timeout or fdg.global_config.preprocessing_exception:
-                if self.preprocess_coverage<50:
-                    assigned_functions=self.functionAssignment.assign_functions_timeout(state_key,deep_functions, 7)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-                elif self.preprocess_coverage < 80:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,deep_functions, 5)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-                else:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,deep_functions, 3)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-            assigned_functions = self.functionAssignment.assign_functions(state_key,deep_functions)
-            if len(assigned_functions) > 0:
-                return {state_key: assigned_functions},True
-
-
-
-class BFS(FunctionSearchStrategy):
-    """
-    no need to save states
-    """
-    def __init__(self):
-        self.flag_one_start_function=False
-        self.preprocess_timeout = False
-        self.preprocess_coverage = 0
-        self.queue=[]
-        super().__init__('bfs')
-        pass
-
-    def initialize(self, flag_one_start_function:bool, preprocess_timeout:bool, preprocess_coverage:float, all_functions:list, fwrg_manager:FWRG_manager):
-        self.flag_one_start_function=flag_one_start_function
-        self.preprocess_timeout = preprocess_timeout
-        self.preprocess_coverage = preprocess_coverage
-        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
-
-    def termination(self,states_num:int=0, current_seq_length: int = 0, sequence_depth_limit: int = 0,iteration:int=0)->bool:
-        if iteration <= fdg.global_config.p1_dl+1:
-            if states_num == 0: return True
-        return False
-
-
-    def assign_states(self, dk_functions: list=None, current_state_key: str = None, fwrg: FWRG_manager = None,
-                      states_dict: dict = {},iteration:int=0) -> list:
-        """
-        assign functions for multiple states at the same time.
-        :param deep_functions:
-        :param current_state_key:
-        :param fwrg:
-        :param states_dict:
-        :return:
-        """
-
-        if len(states_dict) > 0:
-            for key, states in states_dict.items():
-                ftn_seq = get_ftn_seq_from_key_1(key)
-                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
-                    continue  # do not save these states as they will not be explored
-                # save states
-                self.world_states[key] = deepcopy(states)
-                self.queue.append(key)
-
-            # # put key containing fallback at the end of the queue
-            # if len(ftn_seq)==1:
-            #     temp=[]
-            #     for item in self.queue:
-            #         if 'fallback' in item:
-            #             temp.append(item)
-            #         else:
-            #             temp=[item]+temp
-            #     self.queue=temp
-
-
-        print_data_for_bfs_strategy(self.queue)
-
-        if self.flag_one_start_function:
-            self.flag_one_start_function = False
-            state_key = self.queue.pop(0)
-            assign_functions = self.functionAssignment.assign_all_functions()
-
-            return {state_key: assign_functions},True
-
-
-        while True:
-            if len(self.queue) == 0:
-                return {},None
-
-            state_key = self.queue.pop(0)
-            if self.preprocess_timeout or  fdg.global_config.preprocessing_exception:
-                if self.preprocess_coverage < 50:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 7)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-                elif self.preprocess_coverage < 80:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 5)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-                else:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 3)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-            assigned_functions = self.functionAssignment.assign_functions(state_key, dk_functions)
-            if len(assigned_functions) > 0:
-                return {state_key: assigned_functions},True
-
-
-
-class RandomBaseline(FunctionSearchStrategy):
-    """
-    no need to save states
-    """
-    def __init__(self,percent_of_functions:int,functions:list):
-        self.functionAssignment=FunctionAssignment(functions,None,select_percent=percent_of_functions)
-        self.flag_one_start_function=False
-        self.queue=[]
-        super().__init__('baseline')
-
-    def initialize(self, flag_one_start_function: bool):
-        self.flag_one_start_function = flag_one_start_function
-
-    def assign_states(self, dk_functions: list=None, states_dict: dict = {}) -> list:
-        """
-        apply BFS
-        :param dk_functions:
-        :param current_state_key:
-        :param fwrg:
-        :param states_dict:
-        :return:
-        """
-        if len(states_dict) > 0:
-            for key, states in states_dict.items():
-                ftn_seq = get_ftn_seq_from_key_1(key)
-                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
-                    continue  # do not save these states as they will not be explored
-                # save states
-                self.world_states[key] = deepcopy(states)
-                self.queue.append(key)
-
-        print_data_for_bfs_strategy(self.queue)
-
-        if self.flag_one_start_function:
-            self.flag_one_start_function = False
-            state_key = self.queue.pop(0)
-            assign_functions = self.functionAssignment.assign_all_functions()
-
-            return {state_key: assign_functions}, True
-
-        while True:
-            if len(self.queue) == 0:
-                return {}, None
-
-            state_key = self.queue.pop(0)
-
-            assigned_functions =self.functionAssignment.assign_functions_for_baseline()
-            if len(assigned_functions) > 0:
-                return {state_key: assigned_functions}, True
-
-
-
-
-    def termination(self, states_num: int = None, current_seq_length: int = 0,
-                    sequence_depth_limit: int = 0,iteration:int=0) -> bool:
-
-        if iteration <= 1:
-            if states_num == 0: return True
-
-        return False
-
-
-
-
+import ast
+
+from copy import deepcopy
+
+
+import fdg.global_config
+from fdg.control.function_assignment import FunctionAssignment
+
+from fdg.fwrg_manager import FWRG_manager
+from fdg.output_data import print_data_for_bfs_strategy, print_data_for_dfs_strategy
+
+from fdg.utils import get_ftn_seq_from_key_1
+
+
+
+
+class FunctionSearchStrategy():
+    def __init__(self,strategy_name:str):
+        self.name=strategy_name
+        self.world_states={}
+        self.search_history={}
+        self.current_state_key=''
+        # print(f'search strategy: {self.name}')
+
+    def save_states(self,key:str,states:list):
+        if key in self.world_states.keys():
+            self.world_states[key]+=states
+        else:
+            self.world_states[key]=states
+    def get_states(self,key:str):
+        if key in self.world_states.keys():
+            return self.world_states[key]
+        else:
+            return []
+    def delete_state(self,key:str):
+        if key in self.world_states.keys():
+            self.world_states.pop(key)
+
+    def assign_states(self, dk_functions: list=None, current_state_key: str = None, fdfg: FWRG_manager = None,
+                      states_dict: dict = {}, iteration:int=0) -> list:
+        pass
+
+
+
+    def termination(self,states_num:int=0,current_seq_length:int=0,sequence_depth_limit:int=0,iteration:int=0)->bool:
+        ...
+
+
+
+class Seq(FunctionSearchStrategy):
+    def __init__(self):
+        self.queue = []
+        if len(fdg.global_config.sequences)>0:
+            # assume that the sequenes are presented as string
+            self.sequences=fdg.global_config.sequences
+        else:self.sequences=[]
+
+        super().__init__('seq')
+
+    def initialize(self):
+        ...
+
+
+    def termination(self, states_num: int = 0, current_seq_length: int = 0, sequence_depth_limit: int = 0,
+                    iteration: int = 0) -> bool:
+        # need to test
+        if states_num == 0: return True
+        return False
+
+    def assign_states(self, dk_functions: list = None, current_state_key: str = None, fdfg: FWRG_manager = None,
+                      states_dict: dict = {}, iteration:int=0) -> list:
+        """
+
+        :param dk_functions:
+        :param current_state_key:
+        :param fdfg:
+        :param states_dict:
+        :return:
+        """
+        if len(states_dict)>0:
+            for key, states in states_dict.items():
+
+                if key not in self.world_states.keys():
+                    self.world_states[key]=deepcopy(states)
+                else:
+                    self.world_states[key]+=deepcopy(states)
+                self.queue.append(key)
+
+        while True:
+            if len(self.queue)==0: return {},False
+            state_key=self.queue.pop(0)
+            if state_key=='constructor':
+                if len(self.sequences)==0:
+                    return {},True
+                return {'constructor':[seq[0] for seq in self.sequences]},True
+
+            seq=get_ftn_seq_from_key_1(state_key)
+            functions=[]
+            for seq_ in self.sequences:
+                if len(seq)==len(seq_):continue
+                if len(seq)<len(seq_):
+                    flag_add=True
+                    for i in range(len(seq)):
+                        if seq[i]!=seq_[i]:
+                            flag_add=False
+                            break
+                    if flag_add:
+                        functions.append(seq_[len(seq)])
+            if len(functions)>0:
+                return {state_key:functions},True
+
+
+class DFS(FunctionSearchStrategy):
+    def __init__(self):
+        self.stack=[]
+        self.preprocess_timeout = False
+        self.preprocess_coverage = 0
+        self.flag_one_start_function=False
+        super().__init__('dfs')
+
+    def initialize(self, flag_one_start_function:bool, preprocess_timeout:bool, preprocess_coverage:float, all_functions:list, fwrg_manager:FWRG_manager):
+        self.flag_one_start_function=flag_one_start_function
+        self.preprocess_timeout = preprocess_timeout
+        self.preprocess_coverage = preprocess_coverage
+        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
+
+
+    def termination(self,states_num:int=0, current_seq_length: int = 0, sequence_depth_limit: int = 0,iteration:int=0)->bool:
+        if iteration<=2:
+            if states_num==0:return True
+        return False
+
+
+
+
+
+    def assign_states(self, dk_functions: list=None, states_dict: dict = {}, iteration:int=0) -> list:
+
+        """
+            save states, push state keys to the stack
+            select a state by poping an item from the stack
+            assign functions to be executed on the selected state
+        :param dk_functions:
+        :param current_state_key:
+        :param fdfg:
+        :param states_dict:
+        :return:
+        """
+        if len(states_dict)>0:
+            for key, states in states_dict.items():
+                ftn_seq=get_ftn_seq_from_key_1(key)
+                if len(ftn_seq)>=fdg.global_config.seq_len_limit:
+                    continue # do not save these states as they will not be explored
+                # save states
+                self.world_states[key]=deepcopy(states)
+                self.stack.append(key)
+
+        print_data_for_dfs_strategy(self.stack)
+
+        if self.flag_one_start_function:
+            self.flag_one_start_function=False
+            state_key = self.stack.pop()
+            assign_functions = self.functionAssignment.assign_all_functions()
+
+            return {state_key : assign_functions},True
+
+        while True:
+            if len(self.stack)==0:
+                return {},None
+
+            state_key=self.stack.pop()
+
+            if self.preprocess_timeout or fdg.global_config.preprocessing_exception:
+                if self.preprocess_coverage<50:
+                    assigned_functions=self.functionAssignment.assign_functions_timeout(state_key, dk_functions, 7)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+                elif self.preprocess_coverage < 80:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key, dk_functions, 5)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+                else:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key, dk_functions, 3)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+            assigned_functions = self.functionAssignment.assign_functions(state_key, dk_functions)
+            if len(assigned_functions) > 0:
+                return {state_key: assigned_functions},True
+
+
+
+class BFS(FunctionSearchStrategy):
+    """
+    no need to save states
+    """
+    def __init__(self):
+        self.flag_one_start_function=False
+        self.preprocess_timeout = False
+        self.preprocess_coverage = 0
+        self.queue=[]
+        super().__init__('bfs')
+        pass
+
+    def initialize(self, flag_one_start_function:bool, preprocess_timeout:bool, preprocess_coverage:float, all_functions:list, fwrg_manager:FWRG_manager):
+        self.flag_one_start_function=flag_one_start_function
+        self.preprocess_timeout = preprocess_timeout
+        self.preprocess_coverage = preprocess_coverage
+        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
+
+    def termination(self,states_num:int=0, current_seq_length: int = 0, sequence_depth_limit: int = 0,iteration:int=0)->bool:
+        if iteration <= fdg.global_config.p1_dl+1:
+            if states_num == 0: return True
+        return False
+
+
+    def assign_states(self, dk_functions: list=None, current_state_key: str = None, fwrg: FWRG_manager = None,
+                      states_dict: dict = {},iteration:int=0) -> list:
+        """
+        assign functions for multiple states at the same time.
+        :param deep_functions:
+        :param current_state_key:
+        :param fwrg:
+        :param states_dict:
+        :return:
+        """
+
+        if len(states_dict) > 0:
+            for key, states in states_dict.items():
+                ftn_seq = get_ftn_seq_from_key_1(key)
+                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
+                    continue  # do not save these states as they will not be explored
+                # save states
+                self.world_states[key] = deepcopy(states)
+                self.queue.append(key)
+
+            # # put key containing fallback at the end of the queue
+            # if len(ftn_seq)==1:
+            #     temp=[]
+            #     for item in self.queue:
+            #         if 'fallback' in item:
+            #             temp.append(item)
+            #         else:
+            #             temp=[item]+temp
+            #     self.queue=temp
+
+
+        print_data_for_bfs_strategy(self.queue)
+
+        if self.flag_one_start_function:
+            self.flag_one_start_function = False
+            state_key = self.queue.pop(0)
+            assign_functions = self.functionAssignment.assign_all_functions()
+
+            return {state_key: assign_functions},True
+
+
+        while True:
+            if len(self.queue) == 0:
+                return {},None
+
+            state_key = self.queue.pop(0)
+            if self.preprocess_timeout or  fdg.global_config.preprocessing_exception:
+                if self.preprocess_coverage < 50:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 7)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+                elif self.preprocess_coverage < 80:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 5)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+                else:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 3)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+            assigned_functions = self.functionAssignment.assign_functions(state_key, dk_functions)
+            if len(assigned_functions) > 0:
+                return {state_key: assigned_functions},True
+
+
+
+class RandomBaseline(FunctionSearchStrategy):
+    """
+    no need to save states
+    """
+    def __init__(self,percent_of_functions:int,functions:list):
+        self.functionAssignment=FunctionAssignment(functions,None,select_percent=percent_of_functions)
+        self.flag_one_start_function=False
+        self.queue=[]
+        super().__init__('baseline')
+
+    def initialize(self, flag_one_start_function: bool):
+        self.flag_one_start_function = flag_one_start_function
+
+    def assign_states(self, dk_functions: list=None, states_dict: dict = {}) -> list:
+        """
+        apply BFS
+        :param dk_functions:
+        :param current_state_key:
+        :param fwrg:
+        :param states_dict:
+        :return:
+        """
+        if len(states_dict) > 0:
+            for key, states in states_dict.items():
+                ftn_seq = get_ftn_seq_from_key_1(key)
+                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
+                    continue  # do not save these states as they will not be explored
+                # save states
+                self.world_states[key] = deepcopy(states)
+                self.queue.append(key)
+
+        print_data_for_bfs_strategy(self.queue)
+
+        if self.flag_one_start_function:
+            self.flag_one_start_function = False
+            state_key = self.queue.pop(0)
+            assign_functions = self.functionAssignment.assign_all_functions()
+
+            return {state_key: assign_functions}, True
+
+        while True:
+            if len(self.queue) == 0:
+                return {}, None
+
+            state_key = self.queue.pop(0)
+
+            assigned_functions =self.functionAssignment.assign_functions_for_baseline()
+            if len(assigned_functions) > 0:
+                return {state_key: assigned_functions}, True
+
+
+
+
+    def termination(self, states_num: int = None, current_seq_length: int = 0,
+                    sequence_depth_limit: int = 0,iteration:int=0) -> bool:
+
+        if iteration <= 1:
+            if states_num == 0: return True
+        else:
+            if len(self.queue)==0:
+                return True
+
+        return False
+
+
+
+
```

### Comparing `smartExecutorx-4.0.0/fdg/control/function_assignment.py` & `smartExecutorx-4.1/fdg/control/function_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,17 @@
             functions=list(set(all_children))
         return targets_be_reached
 
 
     def assign_functions_for_baseline(self)->list:
 
         to_consider_functions=self.all_functions
+        if self.random_select_percent>10:
+            self.random_select_percent=10
+
         select_num=math.ceil((self.random_select_percent/10)*len(to_consider_functions))
 
         select_indices=random_indices(0,len(to_consider_functions)-1,select_num)
         selected_functions=[ftn for idx,ftn in enumerate(to_consider_functions) if idx in select_indices]
 
         # self.record_assignment(selected_functions)
         return selected_functions
```

### Comparing `smartExecutorx-4.0.0/fdg/control/guider.py` & `smartExecutorx-4.1/fdg/control/guider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,215 +1,220 @@
-from copy import deepcopy
-
-import fdg.global_config
-from fdg.control.ftn_search_strategy import FunctionSearchStrategy
-from fdg.fwrg_manager import FWRG_manager
-from fdg.output_data import print_list, print_assigned_functions
-from fdg.instruction_modification import InstructionModification
-from fdg.preprocessing.preprocess import Preprocessing
-from fdg.utils import get_key_1, get_ftn_seq_from_key_1
-from mythril.laser.ethereum.state.world_state import WorldState
-from mythril.laser.ethereum.svm import LaserEVM
-from mythril.laser.plugin.plugins.dependency_pruner import get_ftn_seq_annotation_from_ws
-
-
-
-class Guider():
-    def __init__(self, ftn_search_strategy:FunctionSearchStrategy,functions:list):
-        self.ftn_search_strategy=ftn_search_strategy
-        self.instructionModification = InstructionModification(fdg.global_config.method_identifiers)
-        self.all_functions=functions
-
-        self.termination=False
-
-        self.genesis_states=[]
-        self.state_index=0 # used to form state keys
-
-
-    def init(self, start_functions:list, depth_k_functions:list, preprocess:Preprocessing):
-        fwrg_manager=FWRG_manager(start_functions, depth_k_functions, preprocess)
-        if self.ftn_search_strategy.name in ['seq']:
-            self.ftn_search_strategy.initialize(fwrg_manager.acyclicPaths.main_paths_sf, fwrg_manager.updateFWRG.main_paths_df, fwrg_manager)
-        elif self.ftn_search_strategy.name in ['mine','bfs','dfs']:
-            flag_one_start_function=True if len(start_functions)==1 else False  #to-do: how to update flag_one_state_dpeht1
-            if preprocess.coverage is None:
-                preprocess.coverage=0
-            self.ftn_search_strategy.initialize(flag_one_start_function,preprocess.timeout,preprocess.coverage,preprocess.write_read_info.all_functions,fwrg_manager)
-
-
-
-    def organize_states(self, states:[WorldState]):
-        all_states = {}
-        for state in states:
-            ftn_seq = get_ftn_seq_annotation_from_ws(state)
-
-            if ftn_seq is None or len(ftn_seq) == 0:
-                key = get_key_1(['constructor'], self.state_index)
-            else:
-                # do not save states that are generated at maximum depth
-                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
-                    continue
-                key = get_key_1(ftn_seq, self.state_index)
-
-            # save state
-            all_states[key] = [state]
-            self.state_index += 1
-        return all_states
-
-    def start_iteration(self,laserEVM:LaserEVM=None,deep_functions:list=None,iteration:int=0):
-        """
-            prepare for states and functions to be executed on the states
-        :param laserEVM:
-        :param deep_function:
-        :param iteration:
-        :return:
-        """
-        #============================================
-        if self.ftn_search_strategy.name in ['seq']:
-            if iteration == 2:
-                self.ftn_search_strategy.initialize(None,None,None)
-
-                organize_states_dict={'constructor':laserEVM.open_states}
-                states_functions,flag_world_state_del = self.ftn_search_strategy.assign_states(deep_functions=None, fdfg=None,states_dict=organize_states_dict)
-                self._prepare_states(laserEVM, organize_states_dict, states_functions,flag_world_state_del)
-
-            else:
-                organize_states_dict = self.organize_states(laserEVM.open_states)
-                states_functions,flag_world_state_del = self.ftn_search_strategy.assign_states(deep_functions=None, fdfg=None,
-                                                                          states_dict=organize_states_dict)
-                organize_states_dict = {}
-                for key, function in states_functions.items():
-                    if len(function) > 0:
-                        organize_states_dict[key] = deepcopy(self.ftn_search_strategy.world_states[key])
-
-                self._prepare_states(laserEVM, organize_states_dict, states_functions,flag_world_state_del)
-            return
-
-
-        # ============================================
-        if self.ftn_search_strategy.name in ['baseline']:
-            if iteration==1:
-                laserEVM.open_states = self.genesis_states
-                sequences= [[ftn] for ftn in self.all_functions]
-                print_list(sequences, f'current all sequence(s):')
-
-            else:
-                organize_states_dict = self.organize_states(laserEVM.open_states)
-
-
-                states_functions,flag_world_state_del = self.ftn_search_strategy.assign_states(deep_functions=None, states_dict=organize_states_dict)
-                print_assigned_functions(states_functions)
-                if self.ftn_search_strategy.name in ['baseline']:
-                    organize_states_dict = {}
-                    for key, function in states_functions.items():
-                        if len(function) > 0:
-                            organize_states_dict[key] = deepcopy(self.ftn_search_strategy.world_states[key])
-
-                self._prepare_states(laserEVM, organize_states_dict, states_functions,False)
-            return
-
-        # =============== bfs,dfs,mine=============================
-        # prepare for depth 1 execution for deep function collection
-        if iteration==2 :
-            laserEVM.open_states=self.genesis_states
-            sequences=[[ftn] for ftn in self.all_functions]
-            print_list(sequences, f'current all sequence(s):')
-        else:
-            # when iteration >2
-            organize_states_dict=self.organize_states(laserEVM.open_states)
-            states_functions,flag_world_state_del=self.ftn_search_strategy.assign_states(dk_functions=deep_functions, states_dict=organize_states_dict,iteration=iteration)
-
-            if len(states_functions)==0:
-                # no functions will be executed
-                self.termination=True
-
-            # get the states for the state keys in data states_functions returned from assign_states
-            if self.ftn_search_strategy.name in ['dfs','mine','bfs','mine1']:
-                organize_states_dict = {}
-                for key,function in states_functions.items():
-                    if len(function)>0:
-                        organize_states_dict[key]=self.ftn_search_strategy.world_states[key]
-
-
-            print_assigned_functions(states_functions)
-            self._prepare_states(laserEVM, organize_states_dict, states_functions,flag_world_state_del)
-
-
-    def _prepare_states(self, laserEVM:LaserEVM, states_dict:dict, states_functions:dict,flag_wd_del:bool):
-        cur_iteration_all_sequences = []
-        # specify the functions to be executed on each open states(world states)
-        modified_states = []
-        for key, states in states_dict.items():
-            ftn_seq = get_ftn_seq_from_key_1(key)
-            next_functions = states_functions[key]
-
-            if len(next_functions) > 0:
-                # # save sequences to be executed
-                # for child in next_functions:
-                #     cur_iteration_all_sequences.append(ftn_seq + [child])
-
-                # modify function dispatcher so that only specified functions are executed
-                to_modify_states = deepcopy(states)
-                self.instructionModification.modity_on_multiple_states(to_modify_states, next_functions)
-                modified_states += to_modify_states
-
-
-        # update the open states so that the states having no children nodes are removed
-        laserEVM.open_states = modified_states
-
-        if flag_wd_del:
-            # delete states
-            # print(f'\nbefore state delete:{self.ftn_search_strategy.world_states.keys()}')
-            for key in states_dict.keys():
-                self.ftn_search_strategy.delete_state(key)
-            # print(f'\n after state delete:{self.ftn_search_strategy.world_states.keys()}')
-
-        # print_list(cur_iteration_all_sequences, f'current all sequence(s):')
-
-
-
-    def end_iteration(self,laserEVM:LaserEVM,iteration:int):
-        state_changing_seq = []
-        len_seq=0
-        for state in laserEVM.open_states:
-            seq = get_ftn_seq_annotation_from_ws(state)
-            if seq is None:continue
-            len_seq=len(seq)
-            if len_seq==0:continue
-            if seq not in state_changing_seq:
-                state_changing_seq.append(seq)
-        print_list(state_changing_seq, f'current state changing sequence(s):')
-
-
-
-        self.termination=self.ftn_search_strategy.termination(
-            states_num=len(laserEVM.open_states),
-            current_seq_length=len_seq,
-            sequence_depth_limit=fdg.global_config.seq_len_limit,
-            iteration=iteration)
-
-    def get_start_sequence(self,laserEVM:LaserEVM):
-        """
-        get the sequences used to annotate the states (world states) at the end of Phase 1
-        """
-        state_chaning_seq = []
-        for state in laserEVM.open_states:
-            seq = get_ftn_seq_annotation_from_ws(state)
-            if seq not in state_chaning_seq:
-                state_chaning_seq.append(seq)
-        return state_chaning_seq
-
-
-    def should_terminate(self):
-        return self.termination
-
-    # def save_genesis_states(self,states:list):
-    #     self.genesis_states=deepcopy(states)
-    #     if self.ftn_search_strategy.name in ['mine']:
-    #         states_dict=self.organize_states(states)
-    #         # if len(states_dict)>=2:
-    #         #     print('Check when two or more genesis states are generated (guider.py)')
-    #         self.ftn_search_strategy.update_states(states_dict)
-    #         self.ftn_search_strategy.state_key_assigned_at_last =list(states_dict.keys())[0]
-
-
-
+from copy import deepcopy
+
+import fdg.global_config
+from fdg.control.ftn_search_strategy import FunctionSearchStrategy
+from fdg.fwrg_manager import FWRG_manager
+from fdg.output_data import print_list, print_assigned_functions
+from fdg.instruction_modification import InstructionModification
+from fdg.preprocessing.preprocess import Preprocessing
+from fdg.utils import get_key_1, get_ftn_seq_from_key_1
+from mythril.laser.ethereum.state.world_state import WorldState
+from mythril.laser.ethereum.svm import LaserEVM
+from mythril.laser.plugin.plugins.dependency_pruner import get_ftn_seq_annotation_from_ws
+
+
+
+class Guider():
+    def __init__(self, ftn_search_strategy:FunctionSearchStrategy,functions:list):
+        self.ftn_search_strategy=ftn_search_strategy
+        self.instructionModification = InstructionModification(fdg.global_config.method_identifiers)
+        self.all_functions=functions
+
+        self.termination=False
+
+        self.genesis_states=[]
+        self.state_index=0 # used to form state keys
+
+
+    def init(self, start_functions:list, depth_k_functions:list, preprocess:Preprocessing):
+        fwrg_manager=FWRG_manager(start_functions, depth_k_functions, preprocess)
+        if self.ftn_search_strategy.name in ['seq']:
+            self.ftn_search_strategy.initialize(fwrg_manager.acyclicPaths.main_paths_sf, fwrg_manager.updateFWRG.main_paths_df, fwrg_manager)
+        elif self.ftn_search_strategy.name in ['mine','bfs','dfs']:
+            flag_one_start_function=True if len(start_functions)==1 else False  #to-do: how to update flag_one_state_dpeht1
+            if preprocess.coverage is None:
+                preprocess.coverage=0
+            self.ftn_search_strategy.initialize(flag_one_start_function,preprocess.timeout,preprocess.coverage,preprocess.write_read_info.all_functions,fwrg_manager)
+
+
+
+    def organize_states(self, states:[WorldState]):
+        all_states = {}
+        for state in states:
+            ftn_seq = get_ftn_seq_annotation_from_ws(state)
+
+            if ftn_seq is None or len(ftn_seq) == 0:
+                key = get_key_1(['constructor'], self.state_index)
+            else:
+                # do not save states that are generated at maximum depth
+                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
+                    continue
+                key = get_key_1(ftn_seq, self.state_index)
+
+            # save state
+            all_states[key] = [state]
+            self.state_index += 1
+        return all_states
+
+    def start_iteration(self, laserEVM:LaserEVM=None, dk_functions:list=None, iteration:int=0):
+        """
+            prepare for states and functions to be executed on the states
+        :param laserEVM:
+        :param deep_function:
+        :param iteration:
+        :return:
+        """
+        #============================================
+        if self.ftn_search_strategy.name in ['seq']:
+            if iteration == 1:
+                self.ftn_search_strategy.initialize()
+
+                organize_states_dict={'constructor':laserEVM.open_states}
+                states_functions,flag_world_state_del = self.ftn_search_strategy.assign_states(
+                    dk_functions=None, fdfg=None, states_dict=organize_states_dict)
+                print_assigned_functions(states_functions)
+                self._prepare_states(laserEVM, organize_states_dict, states_functions,flag_world_state_del)
+
+            else:
+                organize_states_dict = self.organize_states(laserEVM.open_states)
+                states_functions,flag_world_state_del = self.ftn_search_strategy.assign_states(
+                    dk_functions=None, fdfg=None,
+                    states_dict=organize_states_dict)
+                organize_states_dict = {}
+                if len(states_functions)>0:
+                    for key, function in states_functions.items():
+                        if len(function) > 0:
+                            organize_states_dict[key] = deepcopy(self.ftn_search_strategy.world_states[key])
+                    print_assigned_functions(states_functions)
+                    self._prepare_states(laserEVM, organize_states_dict, states_functions,flag_world_state_del)
+            return
+
+
+        # ============================================
+        if self.ftn_search_strategy.name in ['baseline']:
+            if iteration==1:
+                laserEVM.open_states = self.genesis_states
+                sequences= [[ftn] for ftn in self.all_functions]
+                print_list(sequences, f'current all sequence(s):')
+
+            else:
+                organize_states_dict = self.organize_states(laserEVM.open_states)
+
+
+                states_functions,flag_world_state_del = self.ftn_search_strategy.assign_states(
+                    dk_functions=None, states_dict=organize_states_dict)
+                print_assigned_functions(states_functions)
+                if self.ftn_search_strategy.name in ['baseline']:
+                    organize_states_dict = {}
+                    for key, function in states_functions.items():
+                        if len(function) > 0:
+                            organize_states_dict[key] = deepcopy(self.ftn_search_strategy.world_states[key])
+
+                self._prepare_states(laserEVM, organize_states_dict, states_functions,False)
+            return
+
+        # =============== bfs,dfs,mine=============================
+        # prepare for depth 1 execution for deep function collection
+        if iteration==2 :
+            laserEVM.open_states=self.genesis_states
+            sequences=[[ftn] for ftn in self.all_functions]
+            print_list(sequences, f'current all sequence(s):')
+        else:
+            # when iteration >2
+            organize_states_dict=self.organize_states(laserEVM.open_states)
+            states_functions,flag_world_state_del=self.ftn_search_strategy.assign_states(dk_functions=dk_functions, states_dict=organize_states_dict, iteration=iteration)
+
+            if len(states_functions)==0:
+                # no functions will be executed
+                self.termination=True
+
+            # get the states for the state keys in data states_functions returned from assign_states
+            if self.ftn_search_strategy.name in ['dfs','mine','bfs','mine1']:
+                organize_states_dict = {}
+                for key,function in states_functions.items():
+                    if len(function)>0:
+                        organize_states_dict[key]=self.ftn_search_strategy.world_states[key]
+
+
+            print_assigned_functions(states_functions)
+            self._prepare_states(laserEVM, organize_states_dict, states_functions,flag_world_state_del)
+
+
+    def _prepare_states(self, laserEVM:LaserEVM, states_dict:dict, states_functions:dict,flag_wd_del:bool):
+        cur_iteration_all_sequences = []
+        # specify the functions to be executed on each open states(world states)
+        modified_states = []
+        for key, states in states_dict.items():
+            ftn_seq = get_ftn_seq_from_key_1(key)
+            next_functions = states_functions[key]
+
+            if len(next_functions) > 0:
+                # # save sequences to be executed
+                # for child in next_functions:
+                #     cur_iteration_all_sequences.append(ftn_seq + [child])
+
+                # modify function dispatcher so that only specified functions are executed
+                to_modify_states = deepcopy(states)
+                self.instructionModification.modity_on_multiple_states(to_modify_states, next_functions)
+                modified_states += to_modify_states
+
+
+        # update the open states so that the states having no children nodes are removed
+        laserEVM.open_states = modified_states
+
+        if flag_wd_del:
+            # delete states
+            # print(f'\nbefore state delete:{self.ftn_search_strategy.world_states.keys()}')
+            for key in states_dict.keys():
+                self.ftn_search_strategy.delete_state(key)
+            # print(f'\n after state delete:{self.ftn_search_strategy.world_states.keys()}')
+
+        # print_list(cur_iteration_all_sequences, f'current all sequence(s):')
+
+
+
+    def end_iteration(self,laserEVM:LaserEVM,iteration:int):
+        state_changing_seq = []
+        len_seq=0
+        for state in laserEVM.open_states:
+            seq = get_ftn_seq_annotation_from_ws(state)
+            if seq is None:continue
+            len_seq=len(seq)
+            if len_seq==0:continue
+            if seq not in state_changing_seq:
+                state_changing_seq.append(seq)
+        print_list(state_changing_seq, f'current state changing sequence(s):')
+
+
+
+        self.termination=self.ftn_search_strategy.termination(
+            states_num=len(laserEVM.open_states),
+            current_seq_length=len_seq,
+            sequence_depth_limit=fdg.global_config.seq_len_limit,
+            iteration=iteration)
+
+    def get_start_sequence(self,laserEVM:LaserEVM):
+        """
+        get the sequences used to annotate the states (world states) at the end of Phase 1
+        """
+        state_chaning_seq = []
+        for state in laserEVM.open_states:
+            seq = get_ftn_seq_annotation_from_ws(state)
+            if seq not in state_chaning_seq:
+                state_chaning_seq.append(seq)
+        return state_chaning_seq
+
+
+    def should_terminate(self):
+        return self.termination
+
+    def save_genesis_states(self,states:list):
+        self.genesis_states=deepcopy(states)
+        if self.ftn_search_strategy.name in ['mine']:
+            states_dict=self.organize_states(states)
+            # if len(states_dict)>=2:
+            #     print('Check when two or more genesis states are generated (guider.py)')
+            self.ftn_search_strategy.update_states(states_dict)
+            self.ftn_search_strategy.state_key_assigned_at_last =list(states_dict.keys())[0]
+
+
+
```

### Comparing `smartExecutorx-4.0.0/fdg/control/mine.py` & `smartExecutorx-4.1/fdg/control/mine.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,535 +1,535 @@
-from copy import deepcopy
-
-import fdg
-from fdg.control.ftn_search_strategy import FunctionSearchStrategy
-from fdg.control.function_assignment import FunctionAssignment
-from fdg.control.weight_computation import compute, \
-    turn_write_features_to_a_value
-from fdg.expression_slot import is_slot_in_a_list, \
-    identify_slot_from_symbolic_slot_expression, common_elements
-
-from fdg.fwrg_manager import FWRG_manager
-from fdg.output_data import print_data_for_mine_strategy_1, \
-    print_data_for_mine_strategy, my_print
-from fdg.utils import get_ftn_seq_from_key_1, get_key_1_prefix, \
-    random_select_from_list
-from mythril.laser.plugin.plugins.dependency_pruner import \
-    get_writes_annotation_from_ws
-
-
-
-class Mine(FunctionSearchStrategy):
-    def __init__(self):
-        self.preprocess_timeout=False
-        self.preprocess_coverage=0
-
-        self.state_storage={}
-        self.written_slots_in_depth_str={} # the writes from all depths in str version
-
-        self.queue=[]
-        self.state_key_assigned_at_last=""
-        # self.parent_state_keys = {}
-        self.flag_one_start_function=False
-        super().__init__('mine')
-
-
-    def initialize(self, flag_one_start_function:bool, preprocess_timeout:bool, preprocess_coverage:float, all_functions:list, fwrg_manager:FWRG_manager):
-        self.flag_one_start_function=flag_one_start_function
-        self.preprocess_timeout=preprocess_timeout
-        self.preprocess_coverage=preprocess_coverage
-
-        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
-        self.fwrg_manager=fwrg_manager
-
-
-    def assign_states(self, dk_functions: list = None, states_dict: dict = {}, iteration:int=0) -> list:
-        """
-
-        :param dk_functions:
-        :param fwrg:
-        :param states_dict:
-        :return:
-        """
-        if self.preprocess_timeout or fdg.global_config.preprocessing_exception:
-            if self.preprocess_coverage<50:
-                # execute 70% of functions+ functions assigned based on the partial graph
-                return self.assign_states_timeout(dk_functions, states_dict, 7)
-            elif self.preprocess_coverage<80:
-                # execute 50% of functions+ functions assigned based on the partial graph
-                return self.assign_states_timeout(dk_functions, states_dict, 5)
-            elif self.preprocess_coverage<90:
-                # execute 50% of functions+ functions assigned based on the partial graph
-                return self.assign_states_timeout(dk_functions, states_dict, 3)
-            else:
-                # execute 10% of functions + functions assigned based on the partial graph
-                return self.assign_states_timeout(dk_functions, states_dict, 1)
-        return self.assign_states_normal(dk_functions, states_dict)
-
-    def assign_states_normal(self, dk_functions: list = None, states_dict: dict = {}) -> list:
-        """
-
-        :param dk_functions:
-        :param fwrg:
-        :param states_dict:
-        :return: a state and the functions to be executed on it
-        a flag indicating whether this state can be deleted or not.
-        """
-        if len(dk_functions)==0:return {}, None
-        if len(states_dict) > 0:
-
-            # save the new states
-            self.update_states(states_dict)
-            self.filter_states()
-
-        # ---------------
-        print_data_for_mine_strategy(self.queue)
-
-        # --------------
-        # case 1
-        # assign the only state
-        if self.flag_one_start_function:
-            self.flag_one_start_function=False # only consider once
-            state_key=self.queue.pop(0)
-            assign_functions= self.functionAssignment.assign_all_functions()
-            self.state_key_assigned_at_last=state_key
-            return {state_key: assign_functions},True
-
-        # --------------
-        # case 2
-        # assign a state and the functions to be executed on it
-        while True:
-            if len(self.queue) == 0:
-                return {}, None
-
-            to_execute_children = []
-            not_to_execute = []
-            flag_can_be_deleted=True
-
-            # pick up a state from the queue
-            targets=[dk for dk,_ in dk_functions]
-            state_key = self.pickup_a_state(targets)  # order the states in self.queue and pick up the one has the highest weight
-
-            # assign functions
-            assigned_children=self.functionAssignment.assign_functions(state_key,dk_functions,to_execute_children,not_to_execute)
-            if len(assigned_children)>0:
-                self.state_key_assigned_at_last = state_key
-                return {state_key: assigned_children},flag_can_be_deleted
-
-    def assign_states_timeout(self, dk_functions: list = None, states_dict: dict = {}, percent_of_functions:int=1) -> list:
-        """
-
-        :param dk_functions:
-        :param fwrg:
-        :param states_dict:
-        :return:
-        """
-        if len(states_dict) > 0:
-            # save the new states
-            self.update_states(states_dict)
-            self.filter_states()
-
-
-        # ---------------
-        print_data_for_mine_strategy(self.queue)
-
-        # --------------
-        # case 1
-        # assign the only state
-        if self.flag_one_start_function:
-            self.flag_one_start_function=False # only consider once
-            state_key=self.queue.pop(0)
-            assign_functions= self.functionAssignment.assign_all_functions()
-            self.state_key_assigned_at_last = state_key
-            return {state_key: assign_functions},True
-
-        # --------------
-        # case 2
-        # assign a state and the functions to be executed on it
-        while True:
-            if len(self.queue) == 0:
-                return {}, None
-
-            # pick up a state from the queue
-            targets=[dk for dk,_ in dk_functions]
-            random_selected_functions=self.functionAssignment.select_functions_randomly(percent_of_functions)
-            # for func in random_selected_functions:
-            #     if func not in targets:
-            #         targets.append(func)
-            print(f'randomly selected functions: {random_selected_functions}')
-
-            state_key = self.pickup_a_state(targets)  # order the states in self.queue and pick up the one has the highest weight
-
-            # assign functions
-            assigned_functions=self.functionAssignment.assign_functions_timeout_mine(state_key, dk_functions,random_selected_functions)
-            if len(assigned_functions)>0:
-                self.state_key_assigned_at_last = state_key
-                return {state_key: assigned_functions},True
-
-    def termination(self, states_num: int = 0, current_seq_length: int = 0, sequence_depth_limit: int = 0,
-                    iteration: int = 0) -> bool:
-        # print(f'{states_num}:{len(self.d1)}:{len(self.d2)}:{len(self.d3)}:{len(self.cur_queue)}:{iteration}')
-        if iteration <= 2:
-            if states_num == 0: return True
-
-        return False
-
-    def update_states(self, states_dict:dict)->list:
-        """
-        save states
-        """
-        address = fdg.global_config.contract_address.value
-
-        for key,states in states_dict.items():
-            for state in states:
-                ftn_seq=get_ftn_seq_from_key_1(key)
-                if 'constructor' not in ftn_seq:
-                    self.world_states[key]=[deepcopy(state)]
-                    self.queue.append(key)
-                    self.state_storage[key] = state.accounts[
-                        address].storage.printable_storage
-
-                    # # save the parent state key for a state
-                    # if len(self.state_key_assigned_at_last) > 0:
-                    #     if key not in self.parent_state_keys.keys():
-                    #         self.parent_state_keys[key] = self.state_key_assigned_at_last
-                    #     else:
-                    #         my_print(f'Why a state has two or more parent state keys')
-                    #         self.parent_state_keys[key] = self.state_key_assigned_at_last
-
-                    # get written slots for this state
-                    # get written slots from its parent, the key of which is saved in self.state_key_assigned_at_last
-                    written_slots_all_steps = deepcopy(self.get_written_slots_in_depth_str(self.state_key_assigned_at_last))
-
-                    # get the current writes from the dependency pruner
-                    written_slots=get_writes_annotation_from_ws(state)
-                    # self.state_write_slots[key]= written_slots
-
-                    writes_str=[]
-                    if len(ftn_seq) in written_slots.keys():
-                        writes=written_slots[len(ftn_seq)]
-                        writes_str=[identify_slot_from_symbolic_slot_expression(s) for s in writes]
-                        writes_str=list(set(writes_str))
-
-                    if len(ftn_seq) not in written_slots_all_steps.keys():
-                        written_slots_all_steps[len(ftn_seq)]=writes_str
-                        self.written_slots_in_depth_str[key]=written_slots_all_steps
-                    else:
-                        written_slots_all_steps[len(ftn_seq)] = writes_str
-                        self.written_slots_in_depth_str[
-                            key] = written_slots_all_steps
-
-
-                else:
-                    slots=state.accounts[address].storage.printable_storage.keys()
-
-                    # save the slots in str version
-                    slots_str=[identify_slot_from_symbolic_slot_expression(s) for s in slots]
-                    if key not in self.written_slots_in_depth_str.keys():
-                        self.written_slots_in_depth_str[key]={0:slots_str}
-
-
-                    self.state_storage[key] = state.accounts[address].storage.printable_storage
-
-    def filter_states(self):
-        """
-        for states generated from the same function sequence, only one is considered if two or more write the same state variables in the last step
-        """
-        def two_list_equal(lst1:list,lst2:list)->bool:
-            if len([e for e in lst1 if e not in lst2])>0:
-                return False
-            elif len([e for e in lst2 if e not in lst1])>0:
-                return False
-            else:
-                return True
-
-        # for key in state_keys:
-        #     self.queue.append(key)
-        # count based on the key prefix
-        count = {}
-        for key in self.queue:
-            key_prefix = get_key_1_prefix(key)
-            if '#' in key_prefix: # a state at depth 2 or deeper
-                if key_prefix.startswith('fallback') and key_prefix.endswith('fallback'):
-                    continue
-                else:
-                    if key_prefix.endswith('fallback#fallback'):
-                        continue
-
-            if key_prefix not in count.keys():
-                count[key_prefix] = [key]
-            else:
-                count[key_prefix] += [key]
-
-        self.queue=[]
-        # compute priority values
-        for key_prefix, keys in count.items():
-            if len(keys) == 1:
-                self.queue.append(keys[0])
-            else:
-                # get state keys with different priority values that share the same function sequence (key prefix)
-                key_recent_writes_pairs = []
-                for key in keys:
-                    seq_len=len(get_ftn_seq_from_key_1(key))
-                    if seq_len in self.written_slots_in_depth_str[key].keys():
-                        recent_writes = self.written_slots_in_depth_str[key][seq_len]
-                    else:
-                        recent_writes=[]
-
-                    key_recent_writes_pairs.append((key, recent_writes))
-
-                # sort the based on weights in descending order
-                key_recent_writes_pairs.sort(key=lambda x: len(x[1]), reverse=True)
-
-                # only keep states that have different writes
-                cur_writes = []
-                for idx,(key, recent_writes) in enumerate(key_recent_writes_pairs):
-                    if idx<=2:
-                        self.queue.append(key)
-                        cur_writes = recent_writes  # update cur_writes
-                    else:
-                        # only keep keys that have weights different than -1
-                        if not two_list_equal(cur_writes,recent_writes):
-                            self.queue.append(key)
-                            cur_writes = recent_writes   # update cur_writes
-
-    def get_written_slots_in_depth_str(self, state_key:str):
-        if state_key not in self.written_slots_in_depth_str.keys():
-            return {}
-        else:
-            return self.written_slots_in_depth_str[state_key]
-
-    def pickup_a_state(self,targets:list):
-        """
-        order states in self.queue
-        return the first state in self.queue
-        """
-
-        def evaluate_state(state_key: str, reads_in_conditions_of_targets: dict):
-            written_slot_by_state=get_storage_written_slots_str(state_key)
-            data = []
-            for dk, reads in reads_in_conditions_of_targets.items():
-                if len(reads) > 0:
-                    my_print(f'\tfor function {dk}:')
-                    reads_str = [identify_slot_from_symbolic_slot_expression(s)
-                                 for s in
-                                 reads]
-                    my_print(f'\t\tread slots:{reads_str}')
-                    count_common = common_elements(reads_str,written_slot_by_state)
-                    data.append(len(count_common) / len(reads))
-
-            my_print(f'evaluation raw data:{data}')
-            v = 0
-            for ele in data:
-                v += ele
-            my_print(f'evaluation value:{v}')
-            return v
-
-        def get_storage_written_slots_str(state_key:str)->[str]:
-            my_print(f'-- {state_key} --')
-
-            # ------------------------
-            # consider all the writes without repeated elements
-            written_slots_str= [identify_slot_from_symbolic_slot_expression(s) for s in
-                     self.state_storage[state_key].keys()]
-            my_print(f'\twrite slots:{written_slots_str}')
-
-            written_slots_str_all=self.get_written_slots_in_depth_str(state_key)
-            my_print(f'\twrite slots:{written_slots_str_all} (writes at each depth)')
-
-            return written_slots_str
-
-        if len(self.queue)==1:
-            return self.queue.pop(0)
-
-        reads_in_conditions_of_targets = {
-            dk: self.fwrg_manager.fwrg.get_reads_in_conditions(dk) for
-            dk in targets}
-
-        my_print(f'\n==== Reads in conditions for targets====')
-        for key,value in reads_in_conditions_of_targets.items():
-            my_print(f'\t{key}:{value}')
-
-        my_print(f'\n==== evaluation on the storage writes ====')
-        state_key_value_pairs=[(key,evaluate_state(key,reads_in_conditions_of_targets)) for key in self.queue]
-        state_key_value_pairs.sort(key=lambda x: x[1], reverse=True)
-        self.queue = [key for key, _ in state_key_value_pairs]
-        # print data
-        my_print(f'-- summary --')
-        for key,value in state_key_value_pairs:
-            my_print(f'\t{key}: {value}')
-
-        high_v=state_key_value_pairs[0][1]
-        state_key_value_pairs_candi=[(idx,key) for idx, (key,value) in enumerate(state_key_value_pairs) if value==high_v]
-
-        if len(state_key_value_pairs_candi)==1:
-            my_print(f'select {state_key_value_pairs_candi[0][1]} based on the evaluation of the writes in state storage')
-            return self.queue.pop(0)
-
-        # begin tie break
-        win_idx=self.break_a_tie(state_key_value_pairs_candi,targets)
-        return self.queue.pop(win_idx)
-
-    def break_a_tie(self,index_key_pairs:list,targets:list)->int:
-        def most_recent_new_writes(state_key:str):
-            written_slots_str=self.get_written_slots_in_depth_str(state_key)
-            func_seq=get_ftn_seq_from_key_1(state_key)
-
-            recent_writes=written_slots_str[len(func_seq)] if len(func_seq) in written_slots_str.keys() else []
-            previous_writes=[]
-            for depth, writes in written_slots_str.items():
-                if depth==len(func_seq):continue
-                for w in writes:
-                    if w not in previous_writes:
-                        previous_writes.append(w)
-
-            new_recent_writes=[w for w in recent_writes if w not in previous_writes]
-            return new_recent_writes
-
-        def most_recent_writes(state_key:str):
-            my_print(f'-- {state_key} --')
-            written_slots_str = self.get_written_slots_in_depth_str(state_key)
-            my_print(f'\trecent writes:{written_slots_str}')
-            func_seq=get_ftn_seq_from_key_1(state_key)
-            if len(func_seq) in written_slots_str.keys():
-                return written_slots_str[len(func_seq)]
-            else:
-                return []
-
-
-        def evaluate_recent_writes(state_key: str, reads_in_conditions_of_targets: dict):
-            recent_writes=most_recent_writes(state_key)
-
-            data = []
-            for dk, reads in reads_in_conditions_of_targets.items():
-                if len(reads) > 0:
-                    my_print(f'\tfor function {dk}:')
-                    reads_str = [identify_slot_from_symbolic_slot_expression(s)
-                                 for s in
-                                 reads]
-                    my_print(f'\t\tread slots:{reads_str}')
-                    count_common = common_elements(reads_str, recent_writes)
-                    data.append(len(count_common) / len(reads))
-
-            my_print(f'evaluation raw data:{data}')
-            v = 0
-            for ele in data:
-                v += ele
-            my_print(f'evaluation value:{v}')
-            return v
-
-        # begin tie break
-
-        def break_by_new_recent_writes(idx_key_pairs:list):
-            # check based on the new recent writes
-            idx_key_new_recent_writes = [(idx, key, most_recent_new_writes(key))
-                                         for
-                                         idx, key in idx_key_pairs]
-            idx_key_new_recent_writes.sort(key=lambda x: len(x[2]),
-                                           reverse=True)
-
-            my_print(f'\n==== new recent writes ====')
-            for idx, key, new_recent_writes in idx_key_new_recent_writes:
-                my_print(f'\t{key}: {new_recent_writes}')
-
-            max_new_writes = len(idx_key_new_recent_writes[0][2])
-            idx_key_new_recent_writes_candi = [(idx, key) for
-                                               idx, key, new_writes in
-                                               idx_key_new_recent_writes if
-                                               len(new_writes) == max_new_writes]
-            if len(idx_key_new_recent_writes_candi) == 1:
-                my_print(f'select {idx_key_new_recent_writes_candi[0][1]} based on new recent writes')
-                return idx_key_new_recent_writes_candi[0][0],idx_key_new_recent_writes_candi
-            elif len(idx_key_new_recent_writes_candi) == 0:
-                idx_key_new_recent_writes_candi = [(idx, key) for idx, key, _ in
-                                                   idx_key_new_recent_writes]
-            return None,idx_key_new_recent_writes_candi
-
-        def break_by_recent_writes(idx_key_pairs:list, targets):
-            # evaluate the recent writes to targets (a way to consider repeated writes)
-            reads_in_conditions_of_targets = {
-                dk: self.fwrg_manager.fwrg.get_reads_in_conditions(dk) for
-                dk in targets}
-
-            my_print(f'\n==== evaluation on the recent writes ====')
-            idx_key_recent_writes = [(idx, key, evaluate_recent_writes(key,
-                                                                       reads_in_conditions_of_targets))
-                                     for idx, key in idx_key_pairs]
-            idx_key_recent_writes.sort(key=lambda x: x[2], reverse=True)
-            # print
-            my_print(f'-- summary --')
-            for idx, key, value in idx_key_recent_writes:
-                my_print(f'\t{key}: {value}')
-
-            max_value = idx_key_recent_writes[0][2]
-            idx_key_recent_writes_candi = [(idx, key) for idx, key, value in
-                                           idx_key_recent_writes if
-                                           value == max_value]
-            if len(idx_key_recent_writes_candi) == 1:
-                my_print(f'select {idx_key_recent_writes_candi[0][1]} based on the evaluation of the recent writes')
-                return idx_key_recent_writes_candi[0][0],idx_key_recent_writes_candi
-            else:
-                return None,idx_key_recent_writes_candi
-
-        def break_by_depth(idx_key_pairs:list):
-            def state_depth(state_key:str)->int:
-                return len(get_ftn_seq_from_key_1(state_key))
-
-            idx_key_depth = [(idx, key, state_depth(key)) for idx,key in idx_key_pairs]
-            idx_key_depth.sort(key=lambda x:x[2],reverse=False)
-            small_depth=idx_key_depth[0][2]
-            idx_key_depth_candi=[(idx,key) for idx,key,depth in idx_key_depth if depth==small_depth]
-            if len(idx_key_depth_candi)==1:
-                my_print(f'select {idx_key_depth_candi[0][1]} based on depth')
-                return idx_key_depth_candi[0][0],idx_key_depth_candi
-            else:
-                return None,idx_key_depth_candi
-
-        def break_num_reached_dk_functions(idx_key_pairs:list,targets:list):
-            def num_reached_dk_functions(state_key:str,targets:list)->int:
-                return len(self.functionAssignment.get_targets_be_reached(get_ftn_seq_from_key_1(state_key)[-1], targets, 1))
-
-
-            idx_key_num_dk = [(idx, key, num_reached_dk_functions(key,targets)) for idx,key in idx_key_pairs]
-            idx_key_num_dk.sort(key=lambda x:x[2],reverse=True)
-            max_num=idx_key_num_dk[0][2]
-            if max_num==0:
-                return None,[(idx,key) for idx,key,num in idx_key_num_dk]
-
-            idx_key_num_dk_candi=[(idx,key) for idx,key,num in idx_key_num_dk if num==max_num]
-            if len(idx_key_num_dk_candi)==1:
-                my_print(f'select {idx_key_num_dk_candi[0][1]} based on the number of dk functions that can be reached directly')
-                return idx_key_num_dk_candi[0][0],idx_key_num_dk_candi
-            else:
-                return None,idx_key_num_dk_candi
-
-        def select_randomly(idx_key_pairs: list) -> int:
-            # randomly select one
-            selected = random_select_from_list(
-                [idx for idx, _ in idx_key_pairs], 1)
-            # print
-            for idx, key in idx_key_pairs:
-                if idx == selected[0]:
-                    my_print(f'select {key} based on random policy')
-            return selected[0]
-
-        # ------------- new recent writes -----------------
-        win_idx,new_recent_writes_candi=break_by_new_recent_writes(index_key_pairs)
-        if win_idx is not None: return win_idx
-
-        # ------------- recent writes -----------------
-        win_idx, recent_writes_candi = break_by_recent_writes(
-            new_recent_writes_candi, targets)
-        if win_idx is not None: return win_idx
-
-        # ------------- depth -----------------
-        win_idx, depth_candi = break_by_depth(recent_writes_candi)
-        if win_idx is not None: return win_idx
-
-        win_idx, num_dk_candi=break_num_reached_dk_functions(depth_candi,targets)
-        if win_idx is not None: return win_idx
-
-        # -------------- random policy ----------------
-        return select_randomly(num_dk_candi)
-
-
-
+from copy import deepcopy
+
+import fdg
+from fdg.control.ftn_search_strategy import FunctionSearchStrategy
+from fdg.control.function_assignment import FunctionAssignment
+from fdg.control.weight_computation import compute, \
+    turn_write_features_to_a_value
+from fdg.expression_slot import is_slot_in_a_list, \
+    identify_slot_from_symbolic_slot_expression, common_elements
+
+from fdg.fwrg_manager import FWRG_manager
+from fdg.output_data import print_data_for_mine_strategy_1, \
+    print_data_for_mine_strategy, my_print
+from fdg.utils import get_ftn_seq_from_key_1, get_key_1_prefix, \
+    random_select_from_list
+from mythril.laser.plugin.plugins.dependency_pruner import \
+    get_writes_annotation_from_ws
+
+
+
+class Mine(FunctionSearchStrategy):
+    def __init__(self):
+        self.preprocess_timeout=False
+        self.preprocess_coverage=0
+
+        self.state_storage={}
+        self.written_slots_in_depth_str={} # the writes from all depths in str version
+
+        self.queue=[]
+        self.state_key_assigned_at_last=""
+        # self.parent_state_keys = {}
+        self.flag_one_start_function=False
+        super().__init__('mine')
+
+
+    def initialize(self, flag_one_start_function:bool, preprocess_timeout:bool, preprocess_coverage:float, all_functions:list, fwrg_manager:FWRG_manager):
+        self.flag_one_start_function=flag_one_start_function
+        self.preprocess_timeout=preprocess_timeout
+        self.preprocess_coverage=preprocess_coverage
+
+        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
+        self.fwrg_manager=fwrg_manager
+
+
+    def assign_states(self, dk_functions: list = None, states_dict: dict = {}, iteration:int=0) -> list:
+        """
+
+        :param dk_functions:
+        :param fwrg:
+        :param states_dict:
+        :return:
+        """
+        if self.preprocess_timeout or fdg.global_config.preprocessing_exception:
+            if self.preprocess_coverage<50:
+                # execute 70% of functions+ functions assigned based on the partial graph
+                return self.assign_states_timeout(dk_functions, states_dict, 7)
+            elif self.preprocess_coverage<80:
+                # execute 50% of functions+ functions assigned based on the partial graph
+                return self.assign_states_timeout(dk_functions, states_dict, 5)
+            elif self.preprocess_coverage<90:
+                # execute 50% of functions+ functions assigned based on the partial graph
+                return self.assign_states_timeout(dk_functions, states_dict, 3)
+            else:
+                # execute 10% of functions + functions assigned based on the partial graph
+                return self.assign_states_timeout(dk_functions, states_dict, 1)
+        return self.assign_states_normal(dk_functions, states_dict)
+
+    def assign_states_normal(self, dk_functions: list = None, states_dict: dict = {}) -> list:
+        """
+
+        :param dk_functions:
+        :param fwrg:
+        :param states_dict:
+        :return: a state and the functions to be executed on it
+        a flag indicating whether this state can be deleted or not.
+        """
+        if len(dk_functions)==0:return {}, None
+        if len(states_dict) > 0:
+
+            # save the new states
+            self.update_states(states_dict)
+            self.filter_states()
+
+        # ---------------
+        print_data_for_mine_strategy(self.queue)
+
+        # --------------
+        # case 1
+        # assign the only state
+        if self.flag_one_start_function:
+            self.flag_one_start_function=False # only consider once
+            state_key=self.queue.pop(0)
+            assign_functions= self.functionAssignment.assign_all_functions()
+            self.state_key_assigned_at_last=state_key
+            return {state_key: assign_functions},True
+
+        # --------------
+        # case 2
+        # assign a state and the functions to be executed on it
+        while True:
+            if len(self.queue) == 0:
+                return {}, None
+
+            to_execute_children = []
+            not_to_execute = []
+            flag_can_be_deleted=True
+
+            # pick up a state from the queue
+            targets=[dk for dk,_ in dk_functions]
+            state_key = self.pickup_a_state(targets)  # order the states in self.queue and pick up the one has the highest weight
+
+            # assign functions
+            assigned_children=self.functionAssignment.assign_functions(state_key,dk_functions,to_execute_children,not_to_execute)
+            if len(assigned_children)>0:
+                self.state_key_assigned_at_last = state_key
+                return {state_key: assigned_children},flag_can_be_deleted
+
+    def assign_states_timeout(self, dk_functions: list = None, states_dict: dict = {}, percent_of_functions:int=1) -> list:
+        """
+
+        :param dk_functions:
+        :param fwrg:
+        :param states_dict:
+        :return:
+        """
+        if len(states_dict) > 0:
+            # save the new states
+            self.update_states(states_dict)
+            self.filter_states()
+
+
+        # ---------------
+        print_data_for_mine_strategy(self.queue)
+
+        # --------------
+        # case 1
+        # assign the only state
+        if self.flag_one_start_function:
+            self.flag_one_start_function=False # only consider once
+            state_key=self.queue.pop(0)
+            assign_functions= self.functionAssignment.assign_all_functions()
+            self.state_key_assigned_at_last = state_key
+            return {state_key: assign_functions},True
+
+        # --------------
+        # case 2
+        # assign a state and the functions to be executed on it
+        while True:
+            if len(self.queue) == 0:
+                return {}, None
+
+            # pick up a state from the queue
+            targets=[dk for dk,_ in dk_functions]
+            random_selected_functions=self.functionAssignment.select_functions_randomly(percent_of_functions)
+            # for func in random_selected_functions:
+            #     if func not in targets:
+            #         targets.append(func)
+            print(f'randomly selected functions: {random_selected_functions}')
+
+            state_key = self.pickup_a_state(targets)  # order the states in self.queue and pick up the one has the highest weight
+
+            # assign functions
+            assigned_functions=self.functionAssignment.assign_functions_timeout_mine(state_key, dk_functions,random_selected_functions)
+            if len(assigned_functions)>0:
+                self.state_key_assigned_at_last = state_key
+                return {state_key: assigned_functions},True
+
+    def termination(self, states_num: int = 0, current_seq_length: int = 0, sequence_depth_limit: int = 0,
+                    iteration: int = 0) -> bool:
+        # print(f'{states_num}:{len(self.d1)}:{len(self.d2)}:{len(self.d3)}:{len(self.cur_queue)}:{iteration}')
+        if iteration <= 2:
+            if states_num == 0: return True
+
+        return False
+
+    def update_states(self, states_dict:dict)->list:
+        """
+        save states
+        """
+        address = fdg.global_config.contract_address.value
+
+        for key,states in states_dict.items():
+            for state in states:
+                ftn_seq=get_ftn_seq_from_key_1(key)
+                if 'constructor' not in ftn_seq:
+                    self.world_states[key]=[deepcopy(state)]
+                    self.queue.append(key)
+                    self.state_storage[key] = state.accounts[
+                        address].storage.printable_storage
+
+                    # # save the parent state key for a state
+                    # if len(self.state_key_assigned_at_last) > 0:
+                    #     if key not in self.parent_state_keys.keys():
+                    #         self.parent_state_keys[key] = self.state_key_assigned_at_last
+                    #     else:
+                    #         my_print(f'Why a state has two or more parent state keys')
+                    #         self.parent_state_keys[key] = self.state_key_assigned_at_last
+
+                    # get written slots for this state
+                    # get written slots from its parent, the key of which is saved in self.state_key_assigned_at_last
+                    written_slots_all_steps = deepcopy(self.get_written_slots_in_depth_str(self.state_key_assigned_at_last))
+
+                    # get the current writes from the dependency pruner
+                    written_slots=get_writes_annotation_from_ws(state)
+                    # self.state_write_slots[key]= written_slots
+
+                    writes_str=[]
+                    if len(ftn_seq) in written_slots.keys():
+                        writes=written_slots[len(ftn_seq)]
+                        writes_str=[identify_slot_from_symbolic_slot_expression(s) for s in writes]
+                        writes_str=list(set(writes_str))
+
+                    if len(ftn_seq) not in written_slots_all_steps.keys():
+                        written_slots_all_steps[len(ftn_seq)]=writes_str
+                        self.written_slots_in_depth_str[key]=written_slots_all_steps
+                    else:
+                        written_slots_all_steps[len(ftn_seq)] = writes_str
+                        self.written_slots_in_depth_str[
+                            key] = written_slots_all_steps
+
+
+                else:
+                    slots=state.accounts[address].storage.printable_storage.keys()
+
+                    # save the slots in str version
+                    slots_str=[identify_slot_from_symbolic_slot_expression(s) for s in slots]
+                    if key not in self.written_slots_in_depth_str.keys():
+                        self.written_slots_in_depth_str[key]={0:slots_str}
+
+
+                    self.state_storage[key] = state.accounts[address].storage.printable_storage
+
+    def filter_states(self):
+        """
+        for states generated from the same function sequence, only one is considered if two or more write the same state variables in the last step
+        """
+        def two_list_equal(lst1:list,lst2:list)->bool:
+            if len([e for e in lst1 if e not in lst2])>0:
+                return False
+            elif len([e for e in lst2 if e not in lst1])>0:
+                return False
+            else:
+                return True
+
+        # for key in state_keys:
+        #     self.queue.append(key)
+        # count based on the key prefix
+        count = {}
+        for key in self.queue:
+            key_prefix = get_key_1_prefix(key)
+            if '#' in key_prefix: # a state at depth 2 or deeper
+                if key_prefix.startswith('fallback') and key_prefix.endswith('fallback'):
+                    continue
+                else:
+                    if key_prefix.endswith('fallback#fallback'):
+                        continue
+
+            if key_prefix not in count.keys():
+                count[key_prefix] = [key]
+            else:
+                count[key_prefix] += [key]
+
+        self.queue=[]
+        # compute priority values
+        for key_prefix, keys in count.items():
+            if len(keys) == 1:
+                self.queue.append(keys[0])
+            else:
+                # get state keys with different priority values that share the same function sequence (key prefix)
+                key_recent_writes_pairs = []
+                for key in keys:
+                    seq_len=len(get_ftn_seq_from_key_1(key))
+                    if seq_len in self.written_slots_in_depth_str[key].keys():
+                        recent_writes = self.written_slots_in_depth_str[key][seq_len]
+                    else:
+                        recent_writes=[]
+
+                    key_recent_writes_pairs.append((key, recent_writes))
+
+                # sort the based on weights in descending order
+                key_recent_writes_pairs.sort(key=lambda x: len(x[1]), reverse=True)
+
+                # only keep states that have different writes
+                cur_writes = []
+                for idx,(key, recent_writes) in enumerate(key_recent_writes_pairs):
+                    if idx<=2:
+                        self.queue.append(key)
+                        cur_writes = recent_writes  # update cur_writes
+                    else:
+                        # only keep keys that have weights different than -1
+                        if not two_list_equal(cur_writes,recent_writes):
+                            self.queue.append(key)
+                            cur_writes = recent_writes   # update cur_writes
+
+    def get_written_slots_in_depth_str(self, state_key:str):
+        if state_key not in self.written_slots_in_depth_str.keys():
+            return {}
+        else:
+            return self.written_slots_in_depth_str[state_key]
+
+    def pickup_a_state(self,targets:list):
+        """
+        order states in self.queue
+        return the first state in self.queue
+        """
+
+        def evaluate_state(state_key: str, reads_in_conditions_of_targets: dict):
+            written_slot_by_state=get_storage_written_slots_str(state_key)
+            data = []
+            for dk, reads in reads_in_conditions_of_targets.items():
+                if len(reads) > 0:
+                    my_print(f'\tfor function {dk}:')
+                    reads_str = [identify_slot_from_symbolic_slot_expression(s)
+                                 for s in
+                                 reads]
+                    my_print(f'\t\tread slots:{reads_str}')
+                    count_common = common_elements(reads_str,written_slot_by_state)
+                    data.append(len(count_common) / len(reads))
+
+            my_print(f'evaluation raw data:{data}')
+            v = 0
+            for ele in data:
+                v += ele
+            my_print(f'evaluation value:{v}')
+            return v
+
+        def get_storage_written_slots_str(state_key:str)->[str]:
+            my_print(f'-- {state_key} --')
+
+            # ------------------------
+            # consider all the writes without repeated elements
+            written_slots_str= [identify_slot_from_symbolic_slot_expression(s) for s in
+                     self.state_storage[state_key].keys()]
+            my_print(f'\twrite slots:{written_slots_str}')
+
+            written_slots_str_all=self.get_written_slots_in_depth_str(state_key)
+            my_print(f'\twrite slots:{written_slots_str_all} (writes at each depth)')
+
+            return written_slots_str
+
+        if len(self.queue)==1:
+            return self.queue.pop(0)
+
+        reads_in_conditions_of_targets = {
+            dk: self.fwrg_manager.fwrg.get_reads_in_conditions(dk) for
+            dk in targets}
+
+        my_print(f'\n==== Reads in conditions for targets====')
+        for key,value in reads_in_conditions_of_targets.items():
+            my_print(f'\t{key}:{value}')
+
+        my_print(f'\n==== evaluation on the storage writes ====')
+        state_key_value_pairs=[(key,evaluate_state(key,reads_in_conditions_of_targets)) for key in self.queue]
+        state_key_value_pairs.sort(key=lambda x: x[1], reverse=True)
+        self.queue = [key for key, _ in state_key_value_pairs]
+        # print data
+        my_print(f'-- summary --')
+        for key,value in state_key_value_pairs:
+            my_print(f'\t{key}: {value}')
+
+        high_v=state_key_value_pairs[0][1]
+        state_key_value_pairs_candi=[(idx,key) for idx, (key,value) in enumerate(state_key_value_pairs) if value==high_v]
+
+        if len(state_key_value_pairs_candi)==1:
+            my_print(f'select {state_key_value_pairs_candi[0][1]} based on the evaluation of the writes in state storage')
+            return self.queue.pop(0)
+
+        # begin tie break
+        win_idx=self.break_a_tie(state_key_value_pairs_candi,targets)
+        return self.queue.pop(win_idx)
+
+    def break_a_tie(self,index_key_pairs:list,targets:list)->int:
+        def most_recent_new_writes(state_key:str):
+            written_slots_str=self.get_written_slots_in_depth_str(state_key)
+            func_seq=get_ftn_seq_from_key_1(state_key)
+
+            recent_writes=written_slots_str[len(func_seq)] if len(func_seq) in written_slots_str.keys() else []
+            previous_writes=[]
+            for depth, writes in written_slots_str.items():
+                if depth==len(func_seq):continue
+                for w in writes:
+                    if w not in previous_writes:
+                        previous_writes.append(w)
+
+            new_recent_writes=[w for w in recent_writes if w not in previous_writes]
+            return new_recent_writes
+
+        def most_recent_writes(state_key:str):
+            my_print(f'-- {state_key} --')
+            written_slots_str = self.get_written_slots_in_depth_str(state_key)
+            my_print(f'\trecent writes:{written_slots_str}')
+            func_seq=get_ftn_seq_from_key_1(state_key)
+            if len(func_seq) in written_slots_str.keys():
+                return written_slots_str[len(func_seq)]
+            else:
+                return []
+
+
+        def evaluate_recent_writes(state_key: str, reads_in_conditions_of_targets: dict):
+            recent_writes=most_recent_writes(state_key)
+
+            data = []
+            for dk, reads in reads_in_conditions_of_targets.items():
+                if len(reads) > 0:
+                    my_print(f'\tfor function {dk}:')
+                    reads_str = [identify_slot_from_symbolic_slot_expression(s)
+                                 for s in
+                                 reads]
+                    my_print(f'\t\tread slots:{reads_str}')
+                    count_common = common_elements(reads_str, recent_writes)
+                    data.append(len(count_common) / len(reads))
+
+            my_print(f'evaluation raw data:{data}')
+            v = 0
+            for ele in data:
+                v += ele
+            my_print(f'evaluation value:{v}')
+            return v
+
+        # begin tie break
+
+        def break_by_new_recent_writes(idx_key_pairs:list):
+            # check based on the new recent writes
+            idx_key_new_recent_writes = [(idx, key, most_recent_new_writes(key))
+                                         for
+                                         idx, key in idx_key_pairs]
+            idx_key_new_recent_writes.sort(key=lambda x: len(x[2]),
+                                           reverse=True)
+
+            my_print(f'\n==== new recent writes ====')
+            for idx, key, new_recent_writes in idx_key_new_recent_writes:
+                my_print(f'\t{key}: {new_recent_writes}')
+
+            max_new_writes = len(idx_key_new_recent_writes[0][2])
+            idx_key_new_recent_writes_candi = [(idx, key) for
+                                               idx, key, new_writes in
+                                               idx_key_new_recent_writes if
+                                               len(new_writes) == max_new_writes]
+            if len(idx_key_new_recent_writes_candi) == 1:
+                my_print(f'select {idx_key_new_recent_writes_candi[0][1]} based on new recent writes')
+                return idx_key_new_recent_writes_candi[0][0],idx_key_new_recent_writes_candi
+            elif len(idx_key_new_recent_writes_candi) == 0:
+                idx_key_new_recent_writes_candi = [(idx, key) for idx, key, _ in
+                                                   idx_key_new_recent_writes]
+            return None,idx_key_new_recent_writes_candi
+
+        def break_by_recent_writes(idx_key_pairs:list, targets):
+            # evaluate the recent writes to targets (a way to consider repeated writes)
+            reads_in_conditions_of_targets = {
+                dk: self.fwrg_manager.fwrg.get_reads_in_conditions(dk) for
+                dk in targets}
+
+            my_print(f'\n==== evaluation on the recent writes ====')
+            idx_key_recent_writes = [(idx, key, evaluate_recent_writes(key,
+                                                                       reads_in_conditions_of_targets))
+                                     for idx, key in idx_key_pairs]
+            idx_key_recent_writes.sort(key=lambda x: x[2], reverse=True)
+            # print
+            my_print(f'-- summary --')
+            for idx, key, value in idx_key_recent_writes:
+                my_print(f'\t{key}: {value}')
+
+            max_value = idx_key_recent_writes[0][2]
+            idx_key_recent_writes_candi = [(idx, key) for idx, key, value in
+                                           idx_key_recent_writes if
+                                           value == max_value]
+            if len(idx_key_recent_writes_candi) == 1:
+                my_print(f'select {idx_key_recent_writes_candi[0][1]} based on the evaluation of the recent writes')
+                return idx_key_recent_writes_candi[0][0],idx_key_recent_writes_candi
+            else:
+                return None,idx_key_recent_writes_candi
+
+        def break_by_depth(idx_key_pairs:list):
+            def state_depth(state_key:str)->int:
+                return len(get_ftn_seq_from_key_1(state_key))
+
+            idx_key_depth = [(idx, key, state_depth(key)) for idx,key in idx_key_pairs]
+            idx_key_depth.sort(key=lambda x:x[2],reverse=False)
+            small_depth=idx_key_depth[0][2]
+            idx_key_depth_candi=[(idx,key) for idx,key,depth in idx_key_depth if depth==small_depth]
+            if len(idx_key_depth_candi)==1:
+                my_print(f'select {idx_key_depth_candi[0][1]} based on depth')
+                return idx_key_depth_candi[0][0],idx_key_depth_candi
+            else:
+                return None,idx_key_depth_candi
+
+        def break_num_reached_dk_functions(idx_key_pairs:list,targets:list):
+            def num_reached_dk_functions(state_key:str,targets:list)->int:
+                return len(self.functionAssignment.get_targets_be_reached(get_ftn_seq_from_key_1(state_key)[-1], targets, 1))
+
+
+            idx_key_num_dk = [(idx, key, num_reached_dk_functions(key,targets)) for idx,key in idx_key_pairs]
+            idx_key_num_dk.sort(key=lambda x:x[2],reverse=True)
+            max_num=idx_key_num_dk[0][2]
+            if max_num==0:
+                return None,[(idx,key) for idx,key,num in idx_key_num_dk]
+
+            idx_key_num_dk_candi=[(idx,key) for idx,key,num in idx_key_num_dk if num==max_num]
+            if len(idx_key_num_dk_candi)==1:
+                my_print(f'select {idx_key_num_dk_candi[0][1]} based on the number of dk functions that can be reached directly')
+                return idx_key_num_dk_candi[0][0],idx_key_num_dk_candi
+            else:
+                return None,idx_key_num_dk_candi
+
+        def select_randomly(idx_key_pairs: list) -> int:
+            # randomly select one
+            selected = random_select_from_list(
+                [idx for idx, _ in idx_key_pairs], 1)
+            # print
+            for idx, key in idx_key_pairs:
+                if idx == selected[0]:
+                    my_print(f'select {key} based on random policy')
+            return selected[0]
+
+        # ------------- new recent writes -----------------
+        win_idx,new_recent_writes_candi=break_by_new_recent_writes(index_key_pairs)
+        if win_idx is not None: return win_idx
+
+        # ------------- recent writes -----------------
+        win_idx, recent_writes_candi = break_by_recent_writes(
+            new_recent_writes_candi, targets)
+        if win_idx is not None: return win_idx
+
+        # ------------- depth -----------------
+        win_idx, depth_candi = break_by_depth(recent_writes_candi)
+        if win_idx is not None: return win_idx
+
+        win_idx, num_dk_candi=break_num_reached_dk_functions(depth_candi,targets)
+        if win_idx is not None: return win_idx
+
+        # -------------- random policy ----------------
+        return select_randomly(num_dk_candi)
+
+
+
```

### Comparing `smartExecutorx-4.0.0/fdg/control/weight_computation.py` & `smartExecutorx-4.1/fdg/control/weight_computation.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/expression_slot.py` & `smartExecutorx-4.1/fdg/expression_slot.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-import re
-
-from fdg.output_data import my_print
-from fdg.utils import str_without_space_line
-from mythril.laser.smt import BitVec
-from z3 import  Z3Exception
-
-"""
-extract the storage locations from Concat() expressions, condition expressions, and (not know yet)
-
-observation: the expression can be extracted multiple times, so, saving the extracted results
-On HoloToken.sol: before saving the results: 28 times
-after saving the results: 6
-
-
-"""
-
-
-max_length=10000
-expression_str_to_slot_normal={} # used in the normal execution process
-
-def map_concrete_hash_key_to_slot_normal(expression:BitVec, data:BitVec):
-    """
-    pplied in create_keccak(self, data: BitVec) n keccak_function_manager.py module
-    """
-    if not expression.symbolic:
-        expr_str = str_without_space_line(expression)
-        data_str=str_without_space_line(data)
-        if expr_str not in expression_str_to_slot_normal.keys():
-            if data_str in expression_str_to_slot_normal.keys():
-                final_data_str=expression_str_to_slot_normal[data_str]
-                expression_str_to_slot_normal[expr_str] = final_data_str
-                # print(f'map: {expr_str}')
-                # print(f'to: {final_data_str}')
-            else:
-                expression_str_to_slot_normal[expr_str] = data_str
-                # print(f'map: {expr_str}')
-                # print(f'to: {data_str}')
-
-
-def identify_slot_from_symbolic_slot_expression(concat_expr: BitVec) -> str:
-    """
-    get the locations of storage from expressions:
-        Concat(0,x,location)
-        keccak256_512(Concat(0,x,location))
-        need to think about the case of array
-
-    also consider the case of concrete hash, the location info is collected in a place where it is created.
-    """
-
-    def map_expr_str_to_slot(expr_str:str)->str:
-        matched_expr = find_matched_expr(expr_str,
-                                         expression_str_to_slot_normal.keys())
-        if matched_expr is not None:
-            temp = expression_str_to_slot_normal[matched_expr]
-            if temp in expression_str_to_slot_normal.keys():
-                return expression_str_to_slot_normal[temp]
-            else:
-                return temp
-
-        slot = expr_str
-        # save the result
-        if expr_str not in expression_str_to_slot_normal.keys():
-            expression_str_to_slot_normal[expr_str] = slot
-        return slot
-
-    def find_matched_expr(expr:str, expr_list:list)->str:
-        if len(expr)>=10:
-            expr_prefix=expr[0:len(expr)-2]
-            for e in expr_list:
-                if str(e[0:len(e)-2]).__eq__(expr_prefix):
-                    return e
-            return None
-        else:
-            if expr in expr_list:
-                return expr
-            else:
-                return None
-
-    if isinstance(concat_expr,BitVec):
-        if not concat_expr.symbolic:
-            expr_str = str_without_space_line(concat_expr)
-            # check if it is already considered once
-            return map_expr_str_to_slot(expr_str)
-
-    if isinstance(concat_expr, str):
-        if concat_expr.isdigit():
-            return map_expr_str_to_slot(concat_expr)
-
-    str_data = str_without_space_line(concat_expr)
-    if len(str_data)>=max_length:
-        # print(f'reach max length')
-        return ""
-
-    # handle the case: 62514009886607029107290561805838585334079798074568712924583230797734656856475 +
-    # Concat(If(1_calldatasize <= 4, 0, 1_calldata[4]),
-    if str_data.count('+')==1:
-        items=str_data.split('+')
-        if items[0].isdigit() and len(items[0])>=10:
-            return map_expr_str_to_slot(items[0])
-        else:
-            str_data=items[1]
-
-
-    last_parameter = ""
-    try:
-
-        # handle the case below:
-        # 1+keccak256_512(Concat(If(1_calldatasize<=4...)
-        # 2+keccak256_512(Concat(If(1_calldatasize<=4...)
-        pattern = r"^(\d+\+)\w+"
-        results = re.search(pattern, str_data)
-        if results:
-            # get the str that
-            str_data = str_data.split(results.group(1))[-1]
-
-        # check if it is already considered once
-        if str_data in expression_str_to_slot_normal.keys():
-            last_parameter = expression_str_to_slot_normal[str_data]
-        else:
-            if str_data.startswith('keccak256_512'):
-                # Use regular expressions to find the last parameter within the keccak256_512 function
-                last_parameter = re.search(r'keccak256_512\(.*?,(\d+)\)',
-                                           str_data)
-            else:
-                # Use regular expressions to find the last parameter within the Concat function
-                last_parameter = re.search(r'Concat\(.*?,(\d+)\)', str_data)
-
-            if last_parameter is not None:
-                last_parameter = last_parameter.group(1)
-                # print(f'(new) exp:{str_data}')
-                # print(f'(new) slot:{last_parameter}')
-                # save the result
-                expression_str_to_slot_normal[str_data] = str(last_parameter)
-            else:
-                # print(f'Failed to identify a slot from {concat_expr}')
-                last_parameter=""
-
-    except Z3Exception as ze:
-        print(f'Have Z3Exception: {concat_expr}')
-    finally:
-        return last_parameter
-
-
-
-def is_slot_in_a_list(slot, slot_list: list) -> bool:
-    """
-    pay special attention to slot that is symbolic. need to find the original slot, i.e., where the dynamic state variable is declared
-    """
-    if slot.symbolic:
-        slot_str = identify_slot_from_symbolic_slot_expression(slot)
-
-        if len(slot_str) == 0:
-            my_print(f'slot_str:{slot_str}')
-            my_print(
-                f'Check why original slot can not be identified for {slot}.')
-            return False
-    else:
-        slot_str = str(slot)
-
-    slot_str_list = [identify_slot_from_symbolic_slot_expression(s) for s in slot_list]
-
-    my_print(f'is slot {slot_str} in slots {slot_str_list}?')
-    if slot_str in slot_str_list:
-        my_print(f'\t yes')
-        return True
-    else:
-        my_print(f'\t no')
-        return False
-
-
-def common_elements(lst_1_str:list,lst_2_str:list)->list:
-
-    common_ele=[]
-    for ele in lst_1_str:
-        if ele in lst_2_str:
-            common_ele.append(ele)
-    return common_ele
-
-
-
-
-
+import re
+
+from fdg.output_data import my_print
+from fdg.utils import str_without_space_line
+from mythril.laser.smt import BitVec
+from z3 import  Z3Exception
+
+"""
+extract the storage locations from Concat() expressions, condition expressions, and (not know yet)
+
+observation: the expression can be extracted multiple times, so, saving the extracted results
+On HoloToken.sol: before saving the results: 28 times
+after saving the results: 6
+
+
+"""
+
+
+max_length=10000
+expression_str_to_slot_normal={} # used in the normal execution process
+
+def map_concrete_hash_key_to_slot_normal(expression:BitVec, data:BitVec):
+    """
+    pplied in create_keccak(self, data: BitVec) n keccak_function_manager.py module
+    """
+    if not expression.symbolic:
+        expr_str = str_without_space_line(expression)
+        data_str=str_without_space_line(data)
+        if expr_str not in expression_str_to_slot_normal.keys():
+            if data_str in expression_str_to_slot_normal.keys():
+                final_data_str=expression_str_to_slot_normal[data_str]
+                expression_str_to_slot_normal[expr_str] = final_data_str
+                # print(f'map: {expr_str}')
+                # print(f'to: {final_data_str}')
+            else:
+                expression_str_to_slot_normal[expr_str] = data_str
+                # print(f'map: {expr_str}')
+                # print(f'to: {data_str}')
+
+
+def identify_slot_from_symbolic_slot_expression(concat_expr: BitVec) -> str:
+    """
+    get the locations of storage from expressions:
+        Concat(0,x,location)
+        keccak256_512(Concat(0,x,location))
+        need to think about the case of array
+
+    also consider the case of concrete hash, the location info is collected in a place where it is created.
+    """
+
+    def map_expr_str_to_slot(expr_str:str)->str:
+        matched_expr = find_matched_expr(expr_str,
+                                         expression_str_to_slot_normal.keys())
+        if matched_expr is not None:
+            temp = expression_str_to_slot_normal[matched_expr]
+            if temp in expression_str_to_slot_normal.keys():
+                return expression_str_to_slot_normal[temp]
+            else:
+                return temp
+
+        slot = expr_str
+        # save the result
+        if expr_str not in expression_str_to_slot_normal.keys():
+            expression_str_to_slot_normal[expr_str] = slot
+        return slot
+
+    def find_matched_expr(expr:str, expr_list:list)->str:
+        if len(expr)>=10:
+            expr_prefix=expr[0:len(expr)-2]
+            for e in expr_list:
+                if str(e[0:len(e)-2]).__eq__(expr_prefix):
+                    return e
+            return None
+        else:
+            if expr in expr_list:
+                return expr
+            else:
+                return None
+
+    if isinstance(concat_expr,BitVec):
+        if not concat_expr.symbolic:
+            expr_str = str_without_space_line(concat_expr)
+            # check if it is already considered once
+            return map_expr_str_to_slot(expr_str)
+
+    if isinstance(concat_expr, str):
+        if concat_expr.isdigit():
+            return map_expr_str_to_slot(concat_expr)
+
+    str_data = str_without_space_line(concat_expr)
+    if len(str_data)>=max_length:
+        # print(f'reach max length')
+        return ""
+
+    # handle the case: 62514009886607029107290561805838585334079798074568712924583230797734656856475 +
+    # Concat(If(1_calldatasize <= 4, 0, 1_calldata[4]),
+    if str_data.count('+')==1:
+        items=str_data.split('+')
+        if items[0].isdigit() and len(items[0])>=10:
+            return map_expr_str_to_slot(items[0])
+        else:
+            str_data=items[1]
+
+
+    last_parameter = ""
+    try:
+
+        # handle the case below:
+        # 1+keccak256_512(Concat(If(1_calldatasize<=4...)
+        # 2+keccak256_512(Concat(If(1_calldatasize<=4...)
+        pattern = r"^(\d+\+)\w+"
+        results = re.search(pattern, str_data)
+        if results:
+            # get the str that
+            str_data = str_data.split(results.group(1))[-1]
+
+        # check if it is already considered once
+        if str_data in expression_str_to_slot_normal.keys():
+            last_parameter = expression_str_to_slot_normal[str_data]
+        else:
+            if str_data.startswith('keccak256_512'):
+                # Use regular expressions to find the last parameter within the keccak256_512 function
+                last_parameter = re.search(r'keccak256_512\(.*?,(\d+)\)',
+                                           str_data)
+            else:
+                # Use regular expressions to find the last parameter within the Concat function
+                last_parameter = re.search(r'Concat\(.*?,(\d+)\)', str_data)
+
+            if last_parameter is not None:
+                last_parameter = last_parameter.group(1)
+                # print(f'(new) exp:{str_data}')
+                # print(f'(new) slot:{last_parameter}')
+                # save the result
+                expression_str_to_slot_normal[str_data] = str(last_parameter)
+            else:
+                # print(f'Failed to identify a slot from {concat_expr}')
+                last_parameter=""
+
+    except Z3Exception as ze:
+        print(f'Have Z3Exception: {concat_expr}')
+    finally:
+        return last_parameter
+
+
+
+def is_slot_in_a_list(slot, slot_list: list) -> bool:
+    """
+    pay special attention to slot that is symbolic. need to find the original slot, i.e., where the dynamic state variable is declared
+    """
+    if slot.symbolic:
+        slot_str = identify_slot_from_symbolic_slot_expression(slot)
+
+        if len(slot_str) == 0:
+            my_print(f'slot_str:{slot_str}')
+            my_print(
+                f'Check why original slot can not be identified for {slot}.')
+            return False
+    else:
+        slot_str = str(slot)
+
+    slot_str_list = [identify_slot_from_symbolic_slot_expression(s) for s in slot_list]
+
+    my_print(f'is slot {slot_str} in slots {slot_str_list}?')
+    if slot_str in slot_str_list:
+        my_print(f'\t yes')
+        return True
+    else:
+        my_print(f'\t no')
+        return False
+
+
+def common_elements(lst_1_str:list,lst_2_str:list)->list:
+
+    common_ele=[]
+    for ele in lst_1_str:
+        if ele in lst_2_str:
+            common_ele.append(ele)
+    return common_ele
+
+
+
+
+
```

### Comparing `smartExecutorx-4.0.0/fdg/fdg_pruner.py` & `smartExecutorx-4.1/fdg/fdg_pruner.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         elif fdg.global_config.function_search_strategy=='dfs':
             self.search_stragety=DFS()
         elif fdg.global_config.function_search_strategy=='mine':
             self.search_stragety=Mine()
         elif fdg.global_config.function_search_strategy=='seq':
             self.search_stragety=Seq()
         else:
-            self.search_stragety = Mine()
+            self.search_stragety = BFS()
 
         self.guider=Guider(self.search_stragety,list(fdg.global_config.method_identifiers.keys()))
 
         self.depth_k=[]
         self.flag_code_cov=True
         self.flag_num_condition=False
 
@@ -84,30 +84,14 @@
             # self.state_hash_check=state_constraints_hash_check()
             pass
 
 
         @symbolic_vm.laser_hook("stop_sym_exec")
         def stop_sym_exec_hook():
             if fdg.global_config.random_baseline>0:return
-            # if not fdg.global_config.flag_preprocess_timeout:
-            #     if not fdg.global_config.preprocessing_exception:
-            #         if self.preprocess is not None and self.functionCoverage is not None:
-            #             if self.preprocess.coverage == self.functionCoverage.coverage:
-            #                 print(f'Reach the maximum coverage.')
-            #
-            # if fdg.global_config.print_function_coverage==1:
-            #    deep_functions_1st_time=self.functionCoverage.get_deep_functions_1st_time()
-            #    if len(deep_functions_1st_time) > 0:
-            #         self.get_depth_k_functions()
-            #         deep_function_in_the_end =self.depth_k
-            #         print(
-            #             f'depth-k functions: {len(deep_functions_1st_time) - len(deep_function_in_the_end)} out of {len(deep_functions_1st_time)} reaches the threshold {fdg.global_config.function_coverage_threshold}%')
-            #
-            #         print(f'all depth-k function(s): {deep_functions_1st_time}')
-            #         print(f'left depth-k function(s): {deep_function_in_the_end}')
 
 
 
         @symbolic_vm.laser_hook("start_sym_trans_laserEVM")
         def start_sym_trans_hook_laserEVM(laserEVM: LaserEVM):
             """
             ...
@@ -134,18 +118,28 @@
 
                 # it means no contract is deployed as no valid contracts are given
                 if isinstance(fdg.global_config.contract_address,str): return
 
                 self.guider.instructionModification.feed_instructions(
                     laserEVM.open_states[0], fdg.global_config.contract_address)
 
-                # self.guider.save_genesis_states(laserEVM.open_states) # to-do: think about removing it
+                self.guider.save_genesis_states(laserEVM.open_states) # to-do: think about removing it
                 self.get_runtime_bytecode(laserEVM.open_states[0],fdg.global_config.contract_address)
 
+            if fdg.global_config.random_baseline > 0:
+                self.guider.start_iteration(
+                    laserEVM=laserEVM, dk_functions=None,
+                    iteration=self._iteration_)
+                return
 
+            if self.search_stragety.name in ['seq']:
+                self.guider.start_iteration(
+                    laserEVM=laserEVM, dk_functions=None,
+                    iteration=self._iteration_)
+                return
 
             if self._iteration_==1:
                 # create a Preprocessing instance
                 self.preprocess = Preprocessing(fdg.global_config.method_identifiers,
                                                 laserEVM.open_states[0],
                                                 fdg.global_config.contract_address)
 
@@ -174,14 +168,69 @@
             - some saved states are used as initial states in sequence execution
 
             :param laserEVM:
             :return:
             """
             log.info(f'\n----------------------------------------')
             log.info(f'end: self._iteration_={self._iteration_}')
+            # ++++++++++++++++++++++++++++++++++++++++++++++++++
+            if fdg.global_config.random_baseline > 0:
+                # prune unfeasible states
+                old_states_count = len(laserEVM.open_states)
+                laserEVM.open_states = [
+                    state for state in laserEVM.open_states if
+                    state.constraints.is_possible
+                ]
+                prune_count = old_states_count - len(laserEVM.open_states)
+                if prune_count: log.info(
+                    "Pruned {} unreachable states".format(prune_count))
+
+                # compute coverage
+                self.functionCoverage.compute_contract_coverage(
+                    fdg.global_config.target_runtime_bytecode)
+                # self.functionCoverage.print_coverage()
+
+                # check at the end of iteration
+                self.guider.end_iteration(laserEVM, self._iteration_)
+                flag_terminate = self.guider.should_terminate()
+                if flag_terminate:
+                    fdg.global_config.transaction_count = self._iteration_
+
+                if self._iteration_ == 1 and len(laserEVM.open_states) == 1:
+                    # in case that there are one state
+                    self.search_stragety.initialize(True)
+
+                # termination based on the coverage of the contract
+                if self.functionCoverage.coverage >= fdg.global_config.function_coverage_threshold:
+                    if not self.search_stragety.flag_one_start_function:
+                        fdg.global_config.transaction_count = self._iteration_
+
+                return
+
+            if self.search_stragety.name in ['seq']:
+                # prune unfeasible states
+                old_states_count = len(laserEVM.open_states)
+                laserEVM.open_states = [
+                    state for state in laserEVM.open_states if
+                    state.constraints.is_possible
+                ]
+                prune_count = old_states_count - len(laserEVM.open_states)
+                if prune_count: log.info(
+                    "Pruned {} unreachable states".format(prune_count))
+
+                # compute coverage
+                self.functionCoverage.compute_contract_coverage(
+                    fdg.global_config.target_runtime_bytecode)
+                # self.functionCoverage.print_coverage()
+
+                # check at the end of iteration
+                self.guider.end_iteration(laserEVM, self._iteration_)
+                flag_terminate = self.guider.should_terminate()
+                if flag_terminate:
+                    fdg.global_config.transaction_count = self._iteration_
 
             #++++++++++++++++++++++++++++++++++++++++++++++++++
             if self.preprocess is None: return
 
             # collect results at the end of preprocessing
             if self._iteration_==1:
                 self.preprocess.main_preprocessing_end(self._iteration_)
```

### Comparing `smartExecutorx-4.0.0/fdg/function_coverage.py` & `smartExecutorx-4.1/fdg/function_coverage.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/fwrg_manager.py` & `smartExecutorx-4.1/fdg/fwrg_manager.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,372 +1,372 @@
-from copy import copy, deepcopy
-
-import fdg.global_config
-
-from fdg.output_data import output_fwrg_data
-from fdg.preprocessing.preprocess import Preprocessing
-
-class FWRG():
-    def __init__(self,ftn_reads_in_condition:dict,ftn_writes:dict):
-        self.ftn_reads_in_condition = ftn_reads_in_condition
-        self.ftn_writes = ftn_writes
-        self.fwrg_dict={}
-        self.frwg_dict={}
-
-        self._generate_fwrg()
-        self._generate_frwg()
-
-    def _generate_fwrg(self):
-        for ftn,writes in self.ftn_writes.items():
-            if len(writes)==0:
-                self.fwrg_dict[ftn]={}
-                continue
-
-            children={}
-            for ftn_read,reads in self.ftn_reads_in_condition.items():
-                for write in writes:
-                    if write in reads:
-                        if ftn_read not in children.keys():
-                            children[ftn_read]=[write]
-                        else:
-                            children[ftn_read]+=[write]
-            self.fwrg_dict[ftn]=children
-
-    def _generate_frwg(self):
-        for ftn, reads in self.ftn_reads_in_condition.items():
-            if len(reads)==0:
-                self.frwg_dict[ftn]={}
-                continue
-            for ftn_write,writes in self.ftn_writes.items():
-                for read in reads:
-                    if read in writes:
-                        if ftn not in self.frwg_dict.keys():
-                            self.frwg_dict[ftn]=[ftn_write]
-                        else:
-                            if ftn_write not in self.frwg_dict[ftn]:
-                                self.frwg_dict[ftn]+=[ftn_write]
-                        break
-
-    def get_reads_in_conditions(self,ftn_name:str):
-        if ftn_name in self.ftn_reads_in_condition.keys():
-            return self.ftn_reads_in_condition[ftn_name]
-        else:return []
-
-class AcyclicPath():
-    def __init__(self, start_functions:list, dk_functions:list, fwrg:FWRG):
-        self.path_len_limit = fdg.global_config.seq_len_limit
-        self.fwrg=fwrg
-        self.start_functions=start_functions
-        self.dk_functions=[ftn for ftn,_ in dk_functions]
-
-        self.paths = {}
-        self._get_path()
-        self.paths_df={}
-        self.organize_paths()
-
-    def _get_path(self):
-        """
-        get all acyclic paths from starting functions (bounded by sequence length)
-        :return:
-        """
-        def get_children(ftn:str):
-            if ftn in self.fwrg.fwrg_dict.keys():
-                children=self.fwrg.fwrg_dict[ftn]
-                if len(children)>0:
-                    return list(children.keys())
-            return []
-        def derive_paths(start_ftn:str):
-            all_paths=[]
-            paths=[[start_ftn]]
-            for i in range(self.path_len_limit-1):
-                derived_paths=[]
-                for path in paths:
-                    children=get_children(path[-1])
-                    if len(children)==0:
-                        if path not in all_paths:
-                            all_paths.append(path)
-                    else:
-                        for child in children:
-                            if child in path:
-                                # think of the case [A(),A()](self dependency)
-                                if child==path[0] and len(path)==1:
-                                    path.append(child)
-                                if path not in all_paths:
-                                    all_paths.append(path)
-                            else:
-                                derived_paths.append(path+[child])
-                paths=derived_paths
-
-            all_paths+=paths
-            return all_paths
-
-
-        for sf in self.start_functions:
-            sf_path=derive_paths(sf)
-            self.paths[sf]=sf_path
-
-    def organize_paths(self):
-        for paths in self.paths.values():
-            for path in paths:
-                for idx,ftn in enumerate(path):
-                    if ftn in self.dk_functions and idx>0:# deep function can not be the frist function in a sequence
-                        t_path=path[0:idx+1]
-                        # add t_path
-                        if ftn not in self.paths_df.keys():
-                            self.paths_df[ftn]={}
-                        if len(t_path)-1 not in self.paths_df[ftn].keys():
-                            self.paths_df[ftn][len(t_path)-1]=[t_path]
-                        else:
-                            if t_path not in self.paths_df[ftn][len(t_path)-1]:
-                                self.paths_df[ftn][len(t_path)-1] += [t_path]
-
-class UpdateFWRG():
-    def __init__(self, fdg:FWRG, paths:AcyclicPath):
-        self.fwrg=fdg
-        self.acyclicPaths=paths
-
-        self.fwrg_targets={}
-
-        self.construct_fwrg_targets()
-
-        self.print_graphs(self.fwrg_targets,'fwrg_targets_data.txt')
-
-        self.fwrg_targets_augmented=deepcopy(self.fwrg_targets)
-        self.add_edges_1()
-        self.print_graphs(self.fwrg_targets_augmented,'fwrg_targets_augmented_data_update.txt')
-
-        self.dk_not_reachable=[]
-        self.identity_dk_function_not_reachable()
-
-    def print_graphs(self,data:dict,file_name:str):
-        output_fwrg_data(data, file_name, 'funtion write-read graph data')
-
-
-    def add_edge_to_graph(self,from_:str,to_:str):
-        if from_ in self.fwrg_targets_augmented.keys():
-            if to_ not in self.fwrg_targets_augmented[from_]:
-                self.fwrg_targets_augmented[from_].append(to_)
-        else:
-            self.fwrg_targets_augmented[from_]=[to_]
-
-
-    def construct_fwrg_targets(self):
-        # reconstruct edges from given acyclic paths
-        for value in self.acyclicPaths.paths_df.values():
-            if not isinstance(value,dict):continue
-            for paths in value.values():
-                for path in paths:
-                    # add edges
-                    for i in range(len(path) - 1):
-                        if path[i] not in self.fwrg_targets.keys():
-                            self.fwrg_targets[path[i]] = [path[i + 1]]
-                        else:
-                            if path[i+1] not in self.fwrg_targets[path[i]]:
-                                self.fwrg_targets[path[i]] += [path[i + 1]]
-
-
-
-    def add_edges_1(self):
-        """
-        for each deep function, add edges to connect some of its paths
-
-        for each deep function, try to find a combined path
-        :return:
-        """
-        def belong_relation(seq1:list,seq2:list):
-            s1=seq1
-            s2=seq2
-            if len(seq1)>len(seq2):
-                s1=seq2
-                s2=seq1
-            if [True for e in s1 if e not in s2].count(True)>0:
-                return False
-            else:
-                return True
-
-        def common_elements(seq1: list, seq2: list):
-            common=[]
-            s1 = seq1
-            s2 = seq2
-            if len(seq1) > len(seq2):
-                s1 = seq2
-                s2 = seq1
-            for e in s1:
-                if e in s2:
-                    common.append(e)
-            return common
-
-        def find_edges(seq1: list, seq2: list, common: list):
-            edges = []
-            s1 = seq1
-            s2 = seq2
-            if len(seq1) > len(seq2):
-                s1 = seq2
-                s2 = seq1
-
-            f1 = -1
-            t1 = -1
-            f2 = -1
-            t2 = -1
-            idx2 = 0
-            for idx, e in enumerate(s1):
-                if e not in common:
-                    if t1 == -1:
-                        t1 = idx
-                    f1 = idx
-                else:
-
-                    # check s2 if there are elements before e
-                    for i in range(idx2, len(s2)):
-                        if not s2[i] == e:
-                            if t2 == -1:
-                                t2 = i
-                            f2 = i
-                        else:
-
-                            break
-
-                    if f2 >= 0 and t2 >= 0 and t1 >= 0 and f1 >= 0:
-                        edges.append((s2[f2], s1[t1]))
-                        edges.append((s1[f1], s2[t2]))
-
-                    idx2 = i + 1
-                    f1 = f2 = t1 = t2 = -1
-                    continue
-
-            if t1 >= 0 and f1 >= 0:
-                if idx2 > len(s2) - 1:
-                    return edges
-                for i in range(idx2, len(s2)):
-                    if not s2[i] == e:
-                        if t2 == -1:
-                            t2 = i
-                        f2 = i
-                    else:
-                        break
-                if f2 >= 0 and t2 >= 0:
-                    edges.append((s2[f2], s1[t1]))
-                    edges.append((s1[f1], s2[t2]))
-
-            return edges
-        for df,value in self.acyclicPaths.paths_df.items():
-
-            if isinstance(value,dict):
-                sequences=[]
-                for seq_list in value.values():
-                    for seq in seq_list:
-                        sequences.append(seq[0:-1])
-
-                all_pairs=[(a,b) for idx,a in enumerate(sequences) for b in sequences[idx+1:]]
-
-                for seq1,seq2 in all_pairs:
-                    if belong_relation(seq1, seq2):
-                        # do not add edges
-                        continue
-                    common = common_elements(seq1, seq2)
-                    if len(common) == 0:
-                        # add edges
-                        self.add_edge_to_graph(seq1[-1], seq2[0])
-                        self.add_edge_to_graph(seq2[-1], seq1[0])
-
-                    else:
-                        edges=find_edges(seq1, seq2, common)
-                        for f,t in edges:
-                            self.add_edge_to_graph(f, t)
-
-    def identity_dk_function_not_reachable(self):
-        for dk in self.acyclicPaths.dk_functions:
-            if dk not in self.acyclicPaths.paths_df.keys():
-                self.dk_not_reachable.append(dk)
-                # print(f'{dk} is not reachable')
-            else:
-                if len(self.acyclicPaths.paths_df[dk])==0:
-                    self.dk_not_reachable.append(dk)
-                    # print(f'{dk} is not reachable')
-
-class FWRG_manager():
-    def __init__(self, start_functions:list, dk_functions:list, preprocess:Preprocessing):
-        self.fwrg=FWRG(preprocess.read_in_conditions.read_slots_in_conditions,
-                       preprocess.write_read_info.write_slots)
-        self.fwrg_all_reads={}
-        self.generate_graph_all_reads(preprocess.write_read_info.write_slots,preprocess.write_read_info.read_slots)
-
-        self.acyclicPaths=AcyclicPath(start_functions, dk_functions, self.fwrg)
-        self.updateFWRG=UpdateFWRG(self.fwrg, self.acyclicPaths)
-
-    def generate_graph_all_reads(self,writes:dict,all_reads:dict):
-        for ftn,writes in writes.items():
-            if len(writes)==0:
-                self.fwrg_all_reads[ftn]={}
-                continue
-            children={}
-            for ftn_read,reads in all_reads.items():
-                for write in writes:
-                     if write in reads:
-                         if ftn_read not in children.keys():
-                             children[ftn_read]=[write]
-                         else:
-                             children[ftn_read]+=[write]
-            self.fwrg_all_reads[ftn]=children
-                
-    def get_children_all_reads(self,ftn:str):
-        if ftn in self.fwrg_all_reads.keys():
-            return list(self.fwrg_all_reads[ftn].keys())
-        else:
-            return []
-    def get_children_fwrg(self,ftn:str):
-        if ftn in self.fwrg.fwrg_dict.keys():
-            return list(self.fwrg.fwrg_dict[ftn])
-        else:
-            return []
-
-    def get_children_fwrg_T_A(self, ftn:str)->list:
-        if ftn in self.updateFWRG.fwrg_targets_augmented.keys():
-            return self.updateFWRG.fwrg_targets_augmented[ftn]
-        else: return []
-
-    def get_parents_frwg(self, ftn:str)->list:
-        if ftn in self.fwrg.frwg_dict.keys():
-            return self.fwrg.frwg_dict[ftn]
-        else:
-            return []
-
-    def get_children_bf_update(self, ftn:str)->list:
-        if ftn in self.updateFWRG.fwrg_targets.keys():
-            return self.updateFWRG.fwrg_targets[ftn]
-        else: return []
-
-
-
-
-
-
-
-
-def test_1():
-    ftn_r_in_condi = {'f2': ['a'], 'f3': ['b'], 'f4': ['c'], 'f5': ['c']}
-    ftn_w = {'f2': ['b'], 'f3': ['a', 'c'], 'f4': [], 'f5': []}
-    fdg = FWRG(ftn_r_in_condi, ftn_w)
-
-    starts = ['f1', 'f2', 'f3']
-    df = ['f4', 'f5']
-    paths = AcyclicPath(starts, df, fdg)
-    print(f'{paths.paths}')
-
-def test_2():
-    ftn_r_in_condi = {'f1': ['a'], 'f2': [], 'f3': ['b'], 'f4': ['c','a']}
-    ftn_w = {'f1': ['a'], 'f2': ['b'], 'f3': ['c'], 'f4': []}
-    fdg = FWRG(ftn_r_in_condi, ftn_w)
-
-    starts = ['f1', 'f2' ]
-    df = ['f3', 'f4']
-    paths = AcyclicPath(starts, df, fdg)
-    print(f'{paths.paths}')
-    print(f'{paths.paths_df}')
-
-    updateFDG=UpdateFWRG(fdg, paths)
-    updateFDG.construct_fwrg_targets()
-    updateFDG.add_edges()
-    print(f'{updateFDG.fwrg_targets}')
-if __name__=='__main__':
-    test_2()
-
+from copy import copy, deepcopy
+
+import fdg.global_config
+
+from fdg.output_data import output_fwrg_data
+from fdg.preprocessing.preprocess import Preprocessing
+
+class FWRG():
+    def __init__(self,ftn_reads_in_condition:dict,ftn_writes:dict):
+        self.ftn_reads_in_condition = ftn_reads_in_condition
+        self.ftn_writes = ftn_writes
+        self.fwrg_dict={}
+        self.frwg_dict={}
+
+        self._generate_fwrg()
+        self._generate_frwg()
+
+    def _generate_fwrg(self):
+        for ftn,writes in self.ftn_writes.items():
+            if len(writes)==0:
+                self.fwrg_dict[ftn]={}
+                continue
+
+            children={}
+            for ftn_read,reads in self.ftn_reads_in_condition.items():
+                for write in writes:
+                    if write in reads:
+                        if ftn_read not in children.keys():
+                            children[ftn_read]=[write]
+                        else:
+                            children[ftn_read]+=[write]
+            self.fwrg_dict[ftn]=children
+
+    def _generate_frwg(self):
+        for ftn, reads in self.ftn_reads_in_condition.items():
+            if len(reads)==0:
+                self.frwg_dict[ftn]={}
+                continue
+            for ftn_write,writes in self.ftn_writes.items():
+                for read in reads:
+                    if read in writes:
+                        if ftn not in self.frwg_dict.keys():
+                            self.frwg_dict[ftn]=[ftn_write]
+                        else:
+                            if ftn_write not in self.frwg_dict[ftn]:
+                                self.frwg_dict[ftn]+=[ftn_write]
+                        break
+
+    def get_reads_in_conditions(self,ftn_name:str):
+        if ftn_name in self.ftn_reads_in_condition.keys():
+            return self.ftn_reads_in_condition[ftn_name]
+        else:return []
+
+class AcyclicPath():
+    def __init__(self, start_functions:list, dk_functions:list, fwrg:FWRG):
+        self.path_len_limit = fdg.global_config.seq_len_limit
+        self.fwrg=fwrg
+        self.start_functions=start_functions
+        self.dk_functions=[ftn for ftn,_ in dk_functions]
+
+        self.paths = {}
+        self._get_path()
+        self.paths_df={}
+        self.organize_paths()
+
+    def _get_path(self):
+        """
+        get all acyclic paths from starting functions (bounded by sequence length)
+        :return:
+        """
+        def get_children(ftn:str):
+            if ftn in self.fwrg.fwrg_dict.keys():
+                children=self.fwrg.fwrg_dict[ftn]
+                if len(children)>0:
+                    return list(children.keys())
+            return []
+        def derive_paths(start_ftn:str):
+            all_paths=[]
+            paths=[[start_ftn]]
+            for i in range(self.path_len_limit-1):
+                derived_paths=[]
+                for path in paths:
+                    children=get_children(path[-1])
+                    if len(children)==0:
+                        if path not in all_paths:
+                            all_paths.append(path)
+                    else:
+                        for child in children:
+                            if child in path:
+                                # think of the case [A(),A()](self dependency)
+                                if child==path[0] and len(path)==1:
+                                    path.append(child)
+                                if path not in all_paths:
+                                    all_paths.append(path)
+                            else:
+                                derived_paths.append(path+[child])
+                paths=derived_paths
+
+            all_paths+=paths
+            return all_paths
+
+
+        for sf in self.start_functions:
+            sf_path=derive_paths(sf)
+            self.paths[sf]=sf_path
+
+    def organize_paths(self):
+        for paths in self.paths.values():
+            for path in paths:
+                for idx,ftn in enumerate(path):
+                    if ftn in self.dk_functions and idx>0:# deep function can not be the frist function in a sequence
+                        t_path=path[0:idx+1]
+                        # add t_path
+                        if ftn not in self.paths_df.keys():
+                            self.paths_df[ftn]={}
+                        if len(t_path)-1 not in self.paths_df[ftn].keys():
+                            self.paths_df[ftn][len(t_path)-1]=[t_path]
+                        else:
+                            if t_path not in self.paths_df[ftn][len(t_path)-1]:
+                                self.paths_df[ftn][len(t_path)-1] += [t_path]
+
+class UpdateFWRG():
+    def __init__(self, fdg:FWRG, paths:AcyclicPath):
+        self.fwrg=fdg
+        self.acyclicPaths=paths
+
+        self.fwrg_targets={}
+
+        self.construct_fwrg_targets()
+
+        self.print_graphs(self.fwrg_targets,'fwrg_targets_data.txt')
+
+        self.fwrg_targets_augmented=deepcopy(self.fwrg_targets)
+        self.add_edges_1()
+        self.print_graphs(self.fwrg_targets_augmented,'fwrg_targets_augmented_data_update.txt')
+
+        self.dk_not_reachable=[]
+        self.identity_dk_function_not_reachable()
+
+    def print_graphs(self,data:dict,file_name:str):
+        output_fwrg_data(data, file_name, 'funtion write-read graph data')
+
+
+    def add_edge_to_graph(self,from_:str,to_:str):
+        if from_ in self.fwrg_targets_augmented.keys():
+            if to_ not in self.fwrg_targets_augmented[from_]:
+                self.fwrg_targets_augmented[from_].append(to_)
+        else:
+            self.fwrg_targets_augmented[from_]=[to_]
+
+
+    def construct_fwrg_targets(self):
+        # reconstruct edges from given acyclic paths
+        for value in self.acyclicPaths.paths_df.values():
+            if not isinstance(value,dict):continue
+            for paths in value.values():
+                for path in paths:
+                    # add edges
+                    for i in range(len(path) - 1):
+                        if path[i] not in self.fwrg_targets.keys():
+                            self.fwrg_targets[path[i]] = [path[i + 1]]
+                        else:
+                            if path[i+1] not in self.fwrg_targets[path[i]]:
+                                self.fwrg_targets[path[i]] += [path[i + 1]]
+
+
+
+    def add_edges_1(self):
+        """
+        for each deep function, add edges to connect some of its paths
+
+        for each deep function, try to find a combined path
+        :return:
+        """
+        def belong_relation(seq1:list,seq2:list):
+            s1=seq1
+            s2=seq2
+            if len(seq1)>len(seq2):
+                s1=seq2
+                s2=seq1
+            if [True for e in s1 if e not in s2].count(True)>0:
+                return False
+            else:
+                return True
+
+        def common_elements(seq1: list, seq2: list):
+            common=[]
+            s1 = seq1
+            s2 = seq2
+            if len(seq1) > len(seq2):
+                s1 = seq2
+                s2 = seq1
+            for e in s1:
+                if e in s2:
+                    common.append(e)
+            return common
+
+        def find_edges(seq1: list, seq2: list, common: list):
+            edges = []
+            s1 = seq1
+            s2 = seq2
+            if len(seq1) > len(seq2):
+                s1 = seq2
+                s2 = seq1
+
+            f1 = -1
+            t1 = -1
+            f2 = -1
+            t2 = -1
+            idx2 = 0
+            for idx, e in enumerate(s1):
+                if e not in common:
+                    if t1 == -1:
+                        t1 = idx
+                    f1 = idx
+                else:
+
+                    # check s2 if there are elements before e
+                    for i in range(idx2, len(s2)):
+                        if not s2[i] == e:
+                            if t2 == -1:
+                                t2 = i
+                            f2 = i
+                        else:
+
+                            break
+
+                    if f2 >= 0 and t2 >= 0 and t1 >= 0 and f1 >= 0:
+                        edges.append((s2[f2], s1[t1]))
+                        edges.append((s1[f1], s2[t2]))
+
+                    idx2 = i + 1
+                    f1 = f2 = t1 = t2 = -1
+                    continue
+
+            if t1 >= 0 and f1 >= 0:
+                if idx2 > len(s2) - 1:
+                    return edges
+                for i in range(idx2, len(s2)):
+                    if not s2[i] == e:
+                        if t2 == -1:
+                            t2 = i
+                        f2 = i
+                    else:
+                        break
+                if f2 >= 0 and t2 >= 0:
+                    edges.append((s2[f2], s1[t1]))
+                    edges.append((s1[f1], s2[t2]))
+
+            return edges
+        for df,value in self.acyclicPaths.paths_df.items():
+
+            if isinstance(value,dict):
+                sequences=[]
+                for seq_list in value.values():
+                    for seq in seq_list:
+                        sequences.append(seq[0:-1])
+
+                all_pairs=[(a,b) for idx,a in enumerate(sequences) for b in sequences[idx+1:]]
+
+                for seq1,seq2 in all_pairs:
+                    if belong_relation(seq1, seq2):
+                        # do not add edges
+                        continue
+                    common = common_elements(seq1, seq2)
+                    if len(common) == 0:
+                        # add edges
+                        self.add_edge_to_graph(seq1[-1], seq2[0])
+                        self.add_edge_to_graph(seq2[-1], seq1[0])
+
+                    else:
+                        edges=find_edges(seq1, seq2, common)
+                        for f,t in edges:
+                            self.add_edge_to_graph(f, t)
+
+    def identity_dk_function_not_reachable(self):
+        for dk in self.acyclicPaths.dk_functions:
+            if dk not in self.acyclicPaths.paths_df.keys():
+                self.dk_not_reachable.append(dk)
+                # print(f'{dk} is not reachable')
+            else:
+                if len(self.acyclicPaths.paths_df[dk])==0:
+                    self.dk_not_reachable.append(dk)
+                    # print(f'{dk} is not reachable')
+
+class FWRG_manager():
+    def __init__(self, start_functions:list, dk_functions:list, preprocess:Preprocessing):
+        self.fwrg=FWRG(preprocess.read_in_conditions.read_slots_in_conditions,
+                       preprocess.write_read_info.write_slots)
+        self.fwrg_all_reads={}
+        self.generate_graph_all_reads(preprocess.write_read_info.write_slots,preprocess.write_read_info.read_slots)
+
+        self.acyclicPaths=AcyclicPath(start_functions, dk_functions, self.fwrg)
+        self.updateFWRG=UpdateFWRG(self.fwrg, self.acyclicPaths)
+
+    def generate_graph_all_reads(self,writes:dict,all_reads:dict):
+        for ftn,writes in writes.items():
+            if len(writes)==0:
+                self.fwrg_all_reads[ftn]={}
+                continue
+            children={}
+            for ftn_read,reads in all_reads.items():
+                for write in writes:
+                     if write in reads:
+                         if ftn_read not in children.keys():
+                             children[ftn_read]=[write]
+                         else:
+                             children[ftn_read]+=[write]
+            self.fwrg_all_reads[ftn]=children
+                
+    def get_children_all_reads(self,ftn:str):
+        if ftn in self.fwrg_all_reads.keys():
+            return list(self.fwrg_all_reads[ftn].keys())
+        else:
+            return []
+    def get_children_fwrg(self,ftn:str):
+        if ftn in self.fwrg.fwrg_dict.keys():
+            return list(self.fwrg.fwrg_dict[ftn])
+        else:
+            return []
+
+    def get_children_fwrg_T_A(self, ftn:str)->list:
+        if ftn in self.updateFWRG.fwrg_targets_augmented.keys():
+            return self.updateFWRG.fwrg_targets_augmented[ftn]
+        else: return []
+
+    def get_parents_frwg(self, ftn:str)->list:
+        if ftn in self.fwrg.frwg_dict.keys():
+            return self.fwrg.frwg_dict[ftn]
+        else:
+            return []
+
+    def get_children_bf_update(self, ftn:str)->list:
+        if ftn in self.updateFWRG.fwrg_targets.keys():
+            return self.updateFWRG.fwrg_targets[ftn]
+        else: return []
+
+
+
+
+
+
+
+
+def test_1():
+    ftn_r_in_condi = {'f2': ['a'], 'f3': ['b'], 'f4': ['c'], 'f5': ['c']}
+    ftn_w = {'f2': ['b'], 'f3': ['a', 'c'], 'f4': [], 'f5': []}
+    fdg = FWRG(ftn_r_in_condi, ftn_w)
+
+    starts = ['f1', 'f2', 'f3']
+    df = ['f4', 'f5']
+    paths = AcyclicPath(starts, df, fdg)
+    print(f'{paths.paths}')
+
+def test_2():
+    ftn_r_in_condi = {'f1': ['a'], 'f2': [], 'f3': ['b'], 'f4': ['c','a']}
+    ftn_w = {'f1': ['a'], 'f2': ['b'], 'f3': ['c'], 'f4': []}
+    fdg = FWRG(ftn_r_in_condi, ftn_w)
+
+    starts = ['f1', 'f2' ]
+    df = ['f3', 'f4']
+    paths = AcyclicPath(starts, df, fdg)
+    print(f'{paths.paths}')
+    print(f'{paths.paths_df}')
+
+    updateFDG=UpdateFWRG(fdg, paths)
+    updateFDG.construct_fwrg_targets()
+    updateFDG.add_edges()
+    print(f'{updateFDG.fwrg_targets}')
+if __name__=='__main__':
+    test_2()
+
```

### Comparing `smartExecutorx-4.0.0/fdg/global_config.py` & `smartExecutorx-4.1/fdg/global_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-
-"""
-Important parameters 
-"""
-#===============================================
-# parameters that can be set by users
-#--------------------------------------------
-
-# indicate if a graph strategy is used to direct the symbolic execution
-global flag_fwrg
-fdg_fwrg=False
-
-
-# set the search strategy when guiding the symolic execution using a graph structure
-global function_search_strategy
-function_search_strategy='bfs'
-
-
-# having value larger than 0 means brandom baseline is active
-# the value indicates the percentage of functions to be selected
-# 1: 10%, 5:50%,...
-global random_baseline
-random_baseline=0
-
-
-# indicate the code coverage that a function should reach
-global function_coverage_threshold
-function_coverage_threshold=98
-
-
-# set the timeout for the preprocessing
-global preprocess_timeout
-preprocess_timeout=300
-
-
-# indicate if functions' coverage will be printed.1:yes, 0:no
-global print_function_coverage
-print_function_coverage=1
-
-# set to 1 if optimization is considered or not
-# optimizations:
-#    collect concrete addresses and treat them as the possible address msg.sender can take
-#    add initial ether for the contract
-global optimization
-optimization=1
-
-
-# indicate if all the state variables read in functions should be considered.
-# by default, only the state varibles read in conditions are considered.
-global flag_consider_all_reads
-flag_consider_all_read=1
-
-
-# set the limit on the times a function can be executed
-global execution_times_limit
-execution_times_limit=5
-
-
-# provide the sequences to  be executed
-global sequences
-sequences=[]
-
-#===============================================
-# currently, does not support to change them through command line
-#----------------------------------------------
-global output_path
-output_path='C:\\Users\\18178\\Desktop\\temp\\'
-
-# set maximum number of iterations of the symbolic execution engine
-global transaction_count
-transaction_count=100
-
-# the max length of a sequence
-global seq_len_limit
-seq_len_limit=4
-
-
-#===============================================
-# their values are set based on the execution
-#----------------------------------------------
-# save the contract address
-global contract_address
-contract_address=''
-
-# save the function signatures from the disassembler
-global method_identifiers
-method_identifiers={}
-
-# set True if there is an exception in the preprocessing
-global preprocessing_exception
-preprocessing_exception=False
-
-# indicate if the execution is in the preprocessing
-global flag_preprocessing
-flag_preprocessing=False
-
-# set True if there is timeout in the preprocessing
-global flag_preprocess_timeout
-flag_preprocess_timeout=False
-
-# save the runtime bytecode of the target function
-global target_runtime_bytecode
-target_runtime_bytecode= ''
-
-# there are used by the modules (no need to set their values)
-global flag_query_solver
-flag_query_solver=[]
-
-# indicate the length of the transaction sequence
-global tx_len
-tx_len=0
-
-global flag_fallback
-flag_fallback=False
-
-global p1_dl
-p1_dl=1
-
-#===============================================
-
-global temp_count
-temp_count=0
-
-global time_temp
-time_temp=0
-
-global count
-count=0
+
+"""
+Important parameters 
+"""
+#===============================================
+# parameters that can be set by users
+#--------------------------------------------
+
+# indicate if a graph strategy is used to direct the symbolic execution
+global flag_fwrg
+fdg_fwrg=False
+
+
+# set the search strategy when guiding the symolic execution using a graph structure
+global function_search_strategy
+function_search_strategy='mine'
+
+
+# having value larger than 0 means brandom baseline is active
+# the value indicates the percentage of functions to be selected
+# 1: 10%, 5:50%,...
+global random_baseline
+random_baseline=0
+
+
+# indicate the code coverage that a function should reach
+global function_coverage_threshold
+function_coverage_threshold=98
+
+
+# set the timeout for the preprocessing
+global preprocess_timeout
+preprocess_timeout=300
+
+
+# indicate if functions' coverage will be printed.1:yes, 0:no
+global print_function_coverage
+print_function_coverage=1
+
+# set to 1 if optimization is considered or not
+# optimizations:
+#    collect concrete addresses and treat them as the possible address msg.sender can take
+#    add initial ether for the contract
+global optimization
+optimization=1
+
+
+# indicate if all the state variables read in functions should be considered.
+# by default, only the state varibles read in conditions are considered.
+global flag_consider_all_reads
+flag_consider_all_read=1
+
+
+# set the limit on the times a function can be executed
+global execution_times_limit
+execution_times_limit=5
+
+
+# provide the sequences to  be executed
+global sequences
+sequences=[]
+
+#===============================================
+# currently, does not support to change them through command line
+#----------------------------------------------
+global output_path
+output_path='C:\\Users\\18178\\Desktop\\temp\\'
+
+# set maximum number of iterations of the symbolic execution engine
+global transaction_count
+transaction_count=100
+
+# the max length of a sequence
+global seq_len_limit
+seq_len_limit=4
+
+
+#===============================================
+# their values are set based on the execution
+#----------------------------------------------
+# save the contract address
+global contract_address
+contract_address=''
+
+# save the function signatures from the disassembler
+global method_identifiers
+method_identifiers={}
+
+# set True if there is an exception in the preprocessing
+global preprocessing_exception
+preprocessing_exception=False
+
+# indicate if the execution is in the preprocessing
+global flag_preprocessing
+flag_preprocessing=False
+
+# set True if there is timeout in the preprocessing
+global flag_preprocess_timeout
+flag_preprocess_timeout=False
+
+# save the runtime bytecode of the target function
+global target_runtime_bytecode
+target_runtime_bytecode= ''
+
+# there are used by the modules (no need to set their values)
+global flag_query_solver
+flag_query_solver=[]
+
+# indicate the length of the transaction sequence
+global tx_len
+tx_len=0
+
+global flag_fallback
+flag_fallback=False
+
+global p1_dl
+p1_dl=1
+
+#===============================================
+
+global temp_count
+temp_count=0
+
+global time_temp
+time_temp=0
+
+global count
+count=0
```

### Comparing `smartExecutorx-4.0.0/fdg/instruction_modification.py` & `smartExecutorx-4.1/fdg/instruction_modification.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/output_data.py` & `smartExecutorx-4.1/fdg/output_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/preprocessing/address_collection.py` & `smartExecutorx-4.1/fdg/preprocessing/address_collection.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/preprocessing/instruction_coverage.py` & `smartExecutorx-4.1/fdg/preprocessing/instruction_coverage.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/preprocessing/preprocess.py` & `smartExecutorx-4.1/fdg/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/preprocessing/read_in_conditions.py` & `smartExecutorx-4.1/fdg/preprocessing/read_in_conditions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/preprocessing/slot_location.py` & `smartExecutorx-4.1/fdg/preprocessing/slot_location.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/preprocessing/write_read_info.py` & `smartExecutorx-4.1/fdg/preprocessing/write_read_info.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/fdg/utils.py` & `smartExecutorx-4.1/fdg/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-
-import itertools as it
-import string
-import time
-import numpy as np
-# from ethereum import utils
-
-# solve case 6: msg.sender must be a particular value
-# type 1: msg.sender==a particular value
-from z3 import BitVecNumRef
-
-import fdg.global_config
-from mythril.laser.smt import BitVec
-
-
-def str_without_space_line(data:str)->str:
-    if isinstance(data,BitVec):
-        data=str(data.raw)
-    else:
-        data=str(data)
-
-    return data.translate({ord(term): None for term in string.whitespace})
-
-def random_indices(start:int,end:int,size_select:int)->list:
-    select=np.random.choice(range(start,end+1,1),size=size_select,replace=False)
-    return select
-
-def random_select_from_list(given_data:list,size_select:int)->list:
-    select=np.random.choice(range(len(given_data)),size=size_select,replace=False)
-    return [given_data[idx] for idx in select]
-
-def random_select(sequences: list, num_selected: int):
-    if len(sequences)>num_selected:
-        select = np.random.choice(range(len(sequences)), size=num_selected, replace=False)
-        return [sequences[idx] for idx in select]
-    else: return sequences
-
-
-def get_combination(list_for_comb,comb_length:int):
-    """
-    :param list_for_comb: [[1,4], [2,6],[5]]
-    :param comb_length: 2 (two elements in a combination)
-    :return: [(1, 2), (1, 6), (4, 2), (4, 6), (1, 5), (4, 5), (2, 5), (6, 5)]
-    """
-    com_re = []
-    # do combination with length
-    num_groups = len(list_for_comb)
-    if num_groups<comb_length:return []
-
-    # get group combinations
-    com_groups = it.combinations(list_for_comb, comb_length)
-
-    for groups in com_groups:
-        com_re +=it.product(*list(groups))
-
-    return com_re
-
-def get_combination_for_a_list(list_for_comb,comb_length:int):
-    re=[]
-    if comb_length==1:
-        re=[[item] for item in list_for_comb]
-        return re
-    for item in it.combinations(list_for_comb, comb_length):
-        re.append(list(item))
-    return re
-
-
-def get_binary(length:int,number:int):
-    bin_list=[]
-    bin_str=bin(number)
-
-    bin_list=[int(bin_str[i]) for i in range(2,len(bin_str))]
-    if length>len(bin_list):
-        extra=[0 for i in range(length -len(bin_list))]
-        bin_list=extra+bin_list
-    return bin_list
-
-
-
-def hash_for_list(constraints:list) -> str:
-    """
-    Return function names corresponding signature hash
-    :param func: function name
-    :return: Its hash signature
-    """
-
-    # start=time.time()
-    # combined=''
-    # for item in constraints:
-    #     if str(item) not in ['True','False']:
-    #         # print(f'constraint item is considered: {str(item)}')
-    #         combined+=str(item)
-    #     else:
-    #         # print(f'constriant item not considered:{str(item)}')
-    #         ...
-    # end=time.time()
-    # fdg.global_config.time_temp+=end-start
-    # #return combined
-    # return utils.sha3(combined).hex()
-    ...
-
-def hash_for_constraint_list(constraints:list) -> list:
-    # start=time.time()
-    # hash_results=[utils.sha3(str(con)) for con in constraints if str(con) not in ['True','False']]
-    # end=time.time()
-    # fdg.global_config.time_temp+=end-start
-    # return hash_results
-    ...
-
-def print_sequences(sequences,description:str=''):
-    print(f'\n{description}')
-    if len(sequences)==0:
-        print(f'\t[]')
-    else:
-        for seq in sequences:
-            print(f'\t{seq}')
-def get_key(ftn_seq:list)->str:
-    if len(ftn_seq)==1:
-        return ftn_seq[0]
-    if len(ftn_seq)==0:
-        return ''
-    key=ftn_seq[0]
-    for i in range(1,len(ftn_seq)):
-        key+="#"+ftn_seq[i]
-    return key
-def get_ftn_seq_from_key(key:str)->list:
-    if '#' in key:
-        return key.split('#')
-    else:
-        return [key]
-
-def get_key_1(ftn_seq:list,index:int)->str:
-    if len(ftn_seq)==1:
-        return ftn_seq[0]+"#"+str(index)
-    if len(ftn_seq)==0:
-        return ''
-    key=ftn_seq[0]
-    for i in range(1,len(ftn_seq)):
-        key+="#"+ftn_seq[i]
-    return key+"#"+str(index)
-
-def get_key_1_prefix(key:str)->str:
-    idx=key.rindex("#")
-    return key[0:idx]
-
-
-def get_ftn_seq_from_key_1(key:str)->list:
-    if '#' in key:
-        return key.split('#')[0:-1]
-    else:
-        return [key]
-
-
-
-
+
+import itertools as it
+import string
+import time
+import numpy as np
+# from ethereum import utils
+
+# solve case 6: msg.sender must be a particular value
+# type 1: msg.sender==a particular value
+from z3 import BitVecNumRef
+
+import fdg.global_config
+from mythril.laser.smt import BitVec
+
+
+def str_without_space_line(data:str)->str:
+    if isinstance(data,BitVec):
+        data=str(data.raw)
+    else:
+        data=str(data)
+
+    return data.translate({ord(term): None for term in string.whitespace})
+
+def random_indices(start:int,end:int,size_select:int)->list:
+    select=np.random.choice(range(start,end+1,1),size=size_select,replace=False)
+    return select
+
+def random_select_from_list(given_data:list,size_select:int)->list:
+    select=np.random.choice(range(len(given_data)),size=size_select,replace=False)
+    return [given_data[idx] for idx in select]
+
+def random_select(sequences: list, num_selected: int):
+    if len(sequences)>num_selected:
+        select = np.random.choice(range(len(sequences)), size=num_selected, replace=False)
+        return [sequences[idx] for idx in select]
+    else: return sequences
+
+
+def get_combination(list_for_comb,comb_length:int):
+    """
+    :param list_for_comb: [[1,4], [2,6],[5]]
+    :param comb_length: 2 (two elements in a combination)
+    :return: [(1, 2), (1, 6), (4, 2), (4, 6), (1, 5), (4, 5), (2, 5), (6, 5)]
+    """
+    com_re = []
+    # do combination with length
+    num_groups = len(list_for_comb)
+    if num_groups<comb_length:return []
+
+    # get group combinations
+    com_groups = it.combinations(list_for_comb, comb_length)
+
+    for groups in com_groups:
+        com_re +=it.product(*list(groups))
+
+    return com_re
+
+def get_combination_for_a_list(list_for_comb,comb_length:int):
+    re=[]
+    if comb_length==1:
+        re=[[item] for item in list_for_comb]
+        return re
+    for item in it.combinations(list_for_comb, comb_length):
+        re.append(list(item))
+    return re
+
+
+def get_binary(length:int,number:int):
+    bin_list=[]
+    bin_str=bin(number)
+
+    bin_list=[int(bin_str[i]) for i in range(2,len(bin_str))]
+    if length>len(bin_list):
+        extra=[0 for i in range(length -len(bin_list))]
+        bin_list=extra+bin_list
+    return bin_list
+
+
+
+def hash_for_list(constraints:list) -> str:
+    """
+    Return function names corresponding signature hash
+    :param func: function name
+    :return: Its hash signature
+    """
+
+    # start=time.time()
+    # combined=''
+    # for item in constraints:
+    #     if str(item) not in ['True','False']:
+    #         # print(f'constraint item is considered: {str(item)}')
+    #         combined+=str(item)
+    #     else:
+    #         # print(f'constriant item not considered:{str(item)}')
+    #         ...
+    # end=time.time()
+    # fdg.global_config.time_temp+=end-start
+    # #return combined
+    # return utils.sha3(combined).hex()
+    ...
+
+def hash_for_constraint_list(constraints:list) -> list:
+    # start=time.time()
+    # hash_results=[utils.sha3(str(con)) for con in constraints if str(con) not in ['True','False']]
+    # end=time.time()
+    # fdg.global_config.time_temp+=end-start
+    # return hash_results
+    ...
+
+def print_sequences(sequences,description:str=''):
+    print(f'\n{description}')
+    if len(sequences)==0:
+        print(f'\t[]')
+    else:
+        for seq in sequences:
+            print(f'\t{seq}')
+def get_key(ftn_seq:list)->str:
+    if len(ftn_seq)==1:
+        return ftn_seq[0]
+    if len(ftn_seq)==0:
+        return ''
+    key=ftn_seq[0]
+    for i in range(1,len(ftn_seq)):
+        key+="#"+ftn_seq[i]
+    return key
+def get_ftn_seq_from_key(key:str)->list:
+    if '#' in key:
+        return key.split('#')
+    else:
+        return [key]
+
+def get_key_1(ftn_seq:list,index:int)->str:
+    if len(ftn_seq)==1:
+        return ftn_seq[0]+"#"+str(index)
+    if len(ftn_seq)==0:
+        return ''
+    key=ftn_seq[0]
+    for i in range(1,len(ftn_seq)):
+        key+="#"+ftn_seq[i]
+    return key+"#"+str(index)
+
+def get_key_1_prefix(key:str)->str:
+    idx=key.rindex("#")
+    return key[0:idx]
+
+
+def get_ftn_seq_from_key_1(key:str)->list:
+    if '#' in key:
+        return key.split('#')[0:-1]
+    else:
+        return [key]
+
+
+
+
```

### Comparing `smartExecutorx-4.0.0/mythril/analysis/call_helpers.py` & `smartExecutorx-4.1/mythril/analysis/call_helpers.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/callgraph.py` & `smartExecutorx-4.1/mythril/analysis/callgraph.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/issue_annotation.py` & `smartExecutorx-4.1/mythril/analysis/issue_annotation.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/base.py` & `smartExecutorx-4.1/mythril/analysis/module/base.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/loader.py` & `smartExecutorx-4.1/mythril/analysis/module/loader.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/arbitrary_jump.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/arbitrary_jump.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/arbitrary_write.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/arbitrary_write.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/delegatecall.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/delegatecall.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/dependence_on_origin.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/dependence_on_origin.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/dependence_on_predictable_vars.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/dependence_on_predictable_vars.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/ether_thief.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/ether_thief.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/exceptions.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/external_calls.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/external_calls.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/integer.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/integer.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/multiple_sends.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/multiple_sends.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/state_change_external_calls.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/state_change_external_calls.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/suicide.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/suicide.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/unchecked_retval.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/unchecked_retval.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/modules/user_assertions.py` & `smartExecutorx-4.1/mythril/analysis/module/modules/user_assertions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/module/util.py` & `smartExecutorx-4.1/mythril/analysis/module/util.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/ops.py` & `smartExecutorx-4.1/mythril/analysis/ops.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/potential_issues.py` & `smartExecutorx-4.1/mythril/analysis/potential_issues.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/report.py` & `smartExecutorx-4.1/mythril/analysis/report.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/security.py` & `smartExecutorx-4.1/mythril/analysis/security.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/solver.py` & `smartExecutorx-4.1/mythril/analysis/solver.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/swc_data.py` & `smartExecutorx-4.1/mythril/analysis/swc_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/symbolic.py` & `smartExecutorx-4.1/mythril/analysis/symbolic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/templates/callgraph.html` & `smartExecutorx-4.1/mythril/analysis/templates/callgraph.html`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/templates/report_as_markdown.jinja2` & `smartExecutorx-4.1/mythril/analysis/templates/report_as_markdown.jinja2`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/templates/report_as_text.jinja2` & `smartExecutorx-4.1/mythril/analysis/templates/report_as_text.jinja2`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/analysis/traceexplore.py` & `smartExecutorx-4.1/mythril/analysis/traceexplore.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/concolic/concolic_execution.py` & `smartExecutorx-4.1/mythril/concolic/concolic_execution.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/concolic/concrete_data.py` & `smartExecutorx-4.1/mythril/concolic/concrete_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/concolic/find_trace.py` & `smartExecutorx-4.1/mythril/concolic/find_trace.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/disassembler/asm.py` & `smartExecutorx-4.1/mythril/disassembler/asm.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/disassembler/disassembly.py` & `smartExecutorx-4.1/mythril/disassembler/disassembly.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/ethereum/evmcontract.py` & `smartExecutorx-4.1/mythril/ethereum/evmcontract.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/base_client.py` & `smartExecutorx-4.1/mythril/ethereum/interface/rpc/base_client.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/client.py` & `smartExecutorx-4.1/mythril/ethereum/interface/rpc/client.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/exceptions.py` & `smartExecutorx-4.1/mythril/ethereum/interface/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/ethereum/interface/rpc/utils.py` & `smartExecutorx-4.1/mythril/ethereum/interface/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/ethereum/util.py` & `smartExecutorx-4.1/mythril/ethereum/util.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/exceptions.py` & `smartExecutorx-4.1/mythril/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/interfaces/cli.py` & `smartExecutorx-4.1/mythril/interfaces/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 """mythril.py: Bug hunting on the Ethereum blockchain
 
    http://www.github.com/ConsenSys/mythril
 """
 
 import argparse
+import ast
 import json
 import logging
 import os
 import sys
 
 import coloredlogs
 import traceback
@@ -435,14 +436,15 @@
         "usage: file1.sol:OptionalContractName file2.sol file3.sol:OptionalContractName",
     )
 
     options = parser.add_argument_group("options")
     add_analysis_args(options)
     add_fwrg_analysis_args(options) #@wei
 
+
 def add_fwrg_analysis_args(options):
     # @wei
     options.add_argument(
         "--optimization",
         type=int,
         default=1,
         help="optimization, current support: 1(yes),0(no)",
@@ -473,15 +475,15 @@
         help="Function data flow graph search strategy",
     )
 
     # @wei
     options.add_argument(
         "-seq",
         "--sequences",
-        type=str,
+        type=parse_list_of_lists,
         help="sequences that will be executed directly",
 
     )
 
     options.add_argument(
         "-p",
         "--print-function-coverage",
@@ -507,21 +509,42 @@
 
     options.add_argument(
         "--execution-times-limit",
         type=int,
         default=5,
         help="limit the times a function can be executed",
     )
+    options.add_argument(
+        "--seq-len-limit",
+        type=int,
+        default=4,
+        help="set the maximum sequence length to be executed",
+    )
 
     options.add_argument(
         "--random-baseline",
         type=int,
         default=0,  # 0 means the baseline is inactive
         help=" with values from  0 to 10. indicate the percent of functions to be considered",
     )
+    options.add_argument(
+
+        "--no-guidance",
+        default=False,
+        action="store_true",
+        help="use guided exploration",
+    )
+
+
+def parse_list_of_lists(value):
+    try:
+        # Parse the string representation of the list of lists into an actual list of lists
+        return ast.literal_eval(value)
+    except (ValueError, SyntaxError) as e:
+        raise argparse.ArgumentTypeError(f"Invalid value for list of lists: {value}")
 
 def add_fwrg_arguments(args: Namespace):
     """
     collect the values for the global parameters defined in fdg.global_config.py.
     """
     fdg.global_config.function_coverage_threshold = args.function_coverage_threshold
     fdg.global_config.function_search_strategy = args.function_search_strategy
@@ -530,14 +553,16 @@
 
     fdg.global_config.print_function_coverage = args.print_function_coverage
     fdg.global_config.p1_dl=args.phase1_depth_limit
     fdg.global_config.preprocess_timeout = args.preprocess_timeout
     fdg.global_config.optimization = args.optimization
     fdg.global_config.flag_consider_all_reads = args.consider_all_reads
     fdg.global_config.execution_times_limit = args.execution_times_limit
+    fdg.global_config.seq_len_limit=args.seq_len_limit
+    fdg.global_config.function_search_strategy=args.function_search_strategy
     if args.no_guidance:
         fdg.global_config.flag_fwrg=False
     else:
         fdg.global_config.flag_fwrg=True
     # fdg.global_config.flag_fwrg=args.function_wr_graph
     if args.v>=3:
         fdg.output_data.flag_basic=True
@@ -551,21 +576,15 @@
     options.add_argument(
         "-fdg",
         "--function-wr-graph",
         default=True,
         action="store_true", #
         help="use guided exploration",
     )
-    options.add_argument(
 
-        "--no-guidance",
-        default=False,
-        action="store_true",
-        help="use guided exploration",
-    )
 
     options.add_argument(
         "-m",
         "--modules",
         help="Comma-separated list of security analysis modules",
         metavar="MODULES",
     )
```

### Comparing `smartExecutorx-4.0.0/mythril/interfaces/epic.py` & `smartExecutorx-4.1/mythril/interfaces/epic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/call.py` & `smartExecutorx-4.1/mythril/laser/ethereum/call.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/cfg.py` & `smartExecutorx-4.1/mythril/laser/ethereum/cfg.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/cheat_code.py` & `smartExecutorx-4.1/mythril/laser/ethereum/cheat_code.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/evm_exceptions.py` & `smartExecutorx-4.1/mythril/laser/ethereum/evm_exceptions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/function_managers/exponent_function_manager.py` & `smartExecutorx-4.1/mythril/laser/ethereum/function_managers/exponent_function_manager.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/function_managers/keccak_function_manager.py` & `smartExecutorx-4.1/mythril/laser/ethereum/function_managers/keccak_function_manager.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/instruction_data.py` & `smartExecutorx-4.1/mythril/laser/ethereum/instruction_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/instructions.py` & `smartExecutorx-4.1/mythril/laser/ethereum/instructions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,2640 +1,2640 @@
-"""This module contains a representation class for EVM instructions and
-transitions between them."""
-import logging
-import time
-
-from copy import copy, deepcopy
-from typing import cast, Callable, List, Union, Tuple
-
-from fdg.expression_slot import map_concrete_hash_key_to_slot_normal
-from mythril.exceptions import UnsatError
-from mythril.laser.smt import (
-    Extract,
-    Expression,
-    UDiv,
-    simplify,
-    Concat,
-    ULT,
-    UGT,
-    BitVec,
-    is_false,
-    URem,
-    SRem,
-    If,
-    Bool,
-    Not,
-    LShR,
-    UGE,
-)
-from mythril.laser.smt import symbol_factory
-
-from mythril.disassembler.disassembly import Disassembly
-
-from mythril.laser.ethereum.state.calldata import ConcreteCalldata, SymbolicCalldata
-
-import mythril.laser.ethereum.util as helper
-from mythril.laser.ethereum import util
-from mythril.laser.ethereum.function_managers import (
-    keccak_function_manager,
-    exponent_function_manager,
-)
-
-from mythril.laser.ethereum.call import (
-    get_call_parameters,
-    native_call,
-    get_call_data,
-    SYMBOLIC_CALLDATA_SIZE,
-)
-from mythril.laser.ethereum.evm_exceptions import (
-    VmException,
-    StackUnderflowException,
-    InvalidJumpDestination,
-    InvalidInstruction,
-    OutOfGasException,
-    WriteProtection,
-)
-from mythril.laser.ethereum.instruction_data import get_opcode_gas, calculate_sha3_gas
-from mythril.laser.ethereum.state.global_state import GlobalState
-from mythril.laser.ethereum.state.return_data import ReturnData
-
-from mythril.laser.ethereum.transaction import (
-    MessageCallTransaction,
-    TransactionStartSignal,
-    ContractCreationTransaction,
-    tx_id_manager,
-)
-from mythril.support.model import get_model
-from mythril.support.support_utils import get_code_hash
-
-from mythril.support.loader import DynLoader
-import fdg
-from mythril.laser.smt.expression import simplify_yes
-
-log = logging.getLogger(__name__)
-
-TT256 = symbol_factory.BitVecVal(0, 256)
-TT256M1 = symbol_factory.BitVecVal(2**256 - 1, 256)
-
-
-def transfer_ether(
-    global_state: GlobalState,
-    sender: BitVec,
-    receiver: BitVec,
-    value: Union[int, BitVec],
-):
-    """
-    Perform an Ether transfer between two accounts
-
-    :param global_state: The global state in which the Ether transfer occurs
-    :param sender: The sender of the Ether
-    :param receiver: The recipient of the Ether
-    :param value: The amount of Ether to send
-    :return:
-    """
-    value = value if isinstance(value, BitVec) else symbol_factory.BitVecVal(value, 256)
-
-    global_state.world_state.constraints.append(
-        UGE(global_state.world_state.balances[sender], value)
-    )
-    global_state.world_state.balances[receiver] += value
-    global_state.world_state.balances[sender] -= value
-
-
-class StateTransition(object):
-    """Decorator that handles global state copy and original return.
-
-    This decorator calls the decorated instruction mutator function on a
-    copy of the state that is passed to it. After the call, the
-    resulting new states' program counter is automatically incremented
-    if `increment_pc=True`.
-    """
-
-    def __init__(
-        self, increment_pc=True, enable_gas=True, is_state_mutation_instruction=False
-    ):
-        """
-
-        :param increment_pc:
-        :param enable_gas:
-        :param is_state_mutation_instruction: The function mutates state
-        """
-        self.increment_pc = increment_pc
-        self.enable_gas = enable_gas
-        self.is_state_mutation_instruction = is_state_mutation_instruction
-
-    @staticmethod
-    def call_on_state_copy(func: Callable, func_obj: "Instruction", state: GlobalState):
-        """
-
-        :param func:
-        :param func_obj:
-        :param state:
-        :return:
-        """
-        global_state_copy = copy(state)
-        return func(func_obj, global_state_copy)
-
-    def increment_states_pc(self, states: List[GlobalState]) -> List[GlobalState]:
-        """
-
-        :param states:
-        :return:
-        """
-        if self.increment_pc:
-            for state in states:
-                state.mstate.pc += 1
-        return states
-
-    @staticmethod
-    def check_gas_usage_limit(global_state: GlobalState):
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.check_gas()
-        if isinstance(global_state.current_transaction.gas_limit, BitVec):
-            value = global_state.current_transaction.gas_limit.value
-            if value is None:
-                return
-            global_state.current_transaction.gas_limit = value
-        if (
-            global_state.mstate.min_gas_used
-            >= global_state.current_transaction.gas_limit
-        ):
-            raise OutOfGasException()
-
-    def accumulate_gas(self, global_state: GlobalState):
-        """
-
-        :param global_state:
-        :return:
-        """
-        if not self.enable_gas:
-            return global_state
-        opcode = global_state.instruction["opcode"]
-        min_gas, max_gas = get_opcode_gas(opcode)
-        global_state.mstate.min_gas_used += min_gas
-        global_state.mstate.max_gas_used += max_gas
-        self.check_gas_usage_limit(global_state)
-
-        return global_state
-
-    def __call__(self, func: Callable) -> Callable:
-        def wrapper(
-            func_obj: "Instruction", global_state: GlobalState
-        ) -> List[GlobalState]:
-            """
-
-            :param func_obj:
-            :param global_state:
-            :return:
-            """
-            if self.is_state_mutation_instruction and global_state.environment.static:
-                raise WriteProtection(
-                    "The function {} cannot be executed in a static call".format(
-                        func.__name__[:-1]
-                    )
-                )
-
-            new_global_states = self.call_on_state_copy(func, func_obj, global_state)
-            new_global_states = [
-                self.accumulate_gas(state) for state in new_global_states
-            ]
-
-            return self.increment_states_pc(new_global_states)
-
-        return wrapper
-
-
-class Instruction:
-    """Instruction class is used to mutate a state according to the current
-    instruction."""
-
-    def __init__(
-        self,
-        op_code: str,
-        dynamic_loader: DynLoader,
-        pre_hooks: List[Callable] = None,
-        post_hooks: List[Callable] = None,
-    ) -> None:
-        """
-
-        :param op_code:
-        :param dynamic_loader:
-        :param iprof:
-        """
-        self.dynamic_loader = dynamic_loader
-        self.op_code = op_code.upper()
-        self.pre_hook = pre_hooks if pre_hooks else []
-        self.post_hook = post_hooks if post_hooks else []
-
-    def _execute_pre_hooks(self, global_state: GlobalState):
-        for hook in self.pre_hook:
-            hook(global_state)
-
-    def _execute_post_hooks(self, global_state: GlobalState):
-        for hook in self.post_hook:
-            hook(global_state)
-
-    def evaluate(self, global_state: GlobalState, post=False) -> List[GlobalState]:
-        """Performs the mutation for this instruction.
-
-        :param global_state:
-        :param post:
-        :return:
-        """
-        # Generalize some ops
-        log.debug("Evaluating %s at %i", self.op_code, global_state.mstate.pc)
-
-        op = self.op_code.lower()
-        if self.op_code.startswith("PUSH"):
-            op = "push"
-        elif self.op_code.startswith("DUP"):
-            op = "dup"
-        elif self.op_code.startswith("SWAP"):
-            op = "swap"
-        elif self.op_code.startswith("LOG"):
-            op = "log"
-        elif self.op_code.startswith("EMPTY"):#@wei: to handle opcode "-"
-            op = "empty"
-        instruction_mutator = (
-            getattr(self, op + "_", None)
-            if not post
-            else getattr(self, op + "_" + "post", None)
-        )
-        if instruction_mutator is None:
-            raise NotImplementedError
-
-        self._execute_pre_hooks(global_state)
-        result = instruction_mutator(global_state)
-        self._execute_post_hooks(global_state)
-
-        return result
-
-    @StateTransition()
-    def jumpdest_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        return [global_state]
-
-    @StateTransition()
-    def push_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        push_instruction = global_state.get_current_instruction()
-        push_value = push_instruction["argument"]
-        try:
-            length_of_value = 2 * int(push_instruction["opcode"][4:])
-        except ValueError:
-            raise VmException("Invalid Push instruction")
-
-        if type(push_value) == tuple:
-            if type(push_value[0]) == int:
-                new_value = symbol_factory.BitVecVal(push_value[0], 8)
-            else:
-                new_value = push_value[0]
-            if len(push_value) > 1:
-                for val in push_value[1:]:
-                    if type(val) == int:
-                        new_value = Concat(new_value, symbol_factory.BitVecVal(val, 8))
-                    else:
-                        new_value = Concat(new_value, val)
-
-            pad_length = length_of_value // 2 - len(push_value)
-
-            if pad_length > 0:
-                new_value = Concat(new_value, symbol_factory.BitVecVal(0, pad_length))
-            if new_value.size() < 256:
-                new_value = Concat(
-                    symbol_factory.BitVecVal(0, 256 - new_value.size()), new_value
-                )
-            # global_state.mstate.stack.append(new_value)
-            global_state.mstate.stack.append(simplify_yes(new_value))
-
-        else:
-            push_value += "0" * max(length_of_value - (len(push_value) - 2), 0)
-            # global_state.mstate.stack.append(
-            #     symbol_factory.BitVecVal(int(push_value, 16), 256)
-            # )
-
-            global_state.mstate.stack.append(
-                simplify_yes(symbol_factory.BitVecVal(int(push_value, 16), 256))
-            )
-
-        return [global_state]
-
-    @StateTransition()
-    def dup_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        value = int(global_state.get_current_instruction()["opcode"][3:], 10)
-        global_state.mstate.stack.append(global_state.mstate.stack[-value])
-        return [global_state]
-
-    @StateTransition()
-    def empty_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        return [global_state]
-
-    @StateTransition()
-    def swap_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        depth = int(self.op_code[4:])
-        stack = global_state.mstate.stack
-        stack[-depth - 1], stack[-1] = stack[-1], stack[-depth - 1]
-        return [global_state]
-
-    @StateTransition()
-    def pop_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.pop()
-        return [global_state]
-
-    @StateTransition()
-    def and_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        stack = global_state.mstate.stack
-        op1, op2 = stack.pop(), stack.pop()
-        if isinstance(op1, Bool):
-            op1 = If(
-                op1, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
-            )
-        if isinstance(op2, Bool):
-            op2 = If(
-                op2, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
-            )
-        if not isinstance(op1, Expression):
-            op1 = symbol_factory.BitVecVal(op1, 256)
-        if not isinstance(op2, Expression):
-            op2 = symbol_factory.BitVecVal(op2, 256)
-        stack.append(op1 & op2)
-
-        return [global_state]
-
-    @StateTransition()
-    def or_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        stack = global_state.mstate.stack
-        op1, op2 = stack.pop(), stack.pop()
-
-        if isinstance(op1, Bool):
-            op1 = If(
-                op1, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
-            )
-
-        if isinstance(op2, Bool):
-            op2 = If(
-                op2, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
-            )
-
-        stack.append(op1 | op2)
-
-        return [global_state]
-
-    @StateTransition()
-    def xor_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        mstate = global_state.mstate
-        mstate.stack.append(mstate.stack.pop() ^ mstate.stack.pop())
-        return [global_state]
-
-    @StateTransition()
-    def not_(self, global_state: GlobalState):
-        """
-
-        :param global_state:
-        :return:
-        """
-        mstate = global_state.mstate
-        mstate.stack.append(TT256M1 - mstate.stack.pop())
-        return [global_state]
-
-    @StateTransition()
-    def byte_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        mstate = global_state.mstate
-        op0, op1 = mstate.stack.pop(), mstate.stack.pop()
-        if not isinstance(op1, Expression):
-            op1 = symbol_factory.BitVecVal(op1, 256)
-        try:
-            index = util.get_concrete_int(op0)
-            offset = (31 - index) * 8
-            if offset >= 0:
-                result = simplify(
-                    Concat(
-                        symbol_factory.BitVecVal(0, 248),
-                        Extract(offset + 7, offset, op1),
-                    )
-                )  # type: Union[int, Expression]
-            else:
-                result = 0
-        except TypeError:
-            log.debug("BYTE: Unsupported symbolic byte offset")
-            result = global_state.new_bitvec(
-                str(simplify(op1)) + "[" + str(simplify(op0)) + "]", 256
-            )
-
-        mstate.stack.append(result)
-        return [global_state]
-
-    # Arithmetic
-    @StateTransition()
-    def add_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(
-            (
-                helper.pop_bitvec(global_state.mstate)
-                + helper.pop_bitvec(global_state.mstate)
-            )
-        )
-
-        return [global_state]
-
-    @StateTransition()
-    def sub_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(
-            (
-                helper.pop_bitvec(global_state.mstate)
-                - helper.pop_bitvec(global_state.mstate)
-            )
-        )
-        return [global_state]
-
-    @StateTransition()
-    def mul_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(
-            (
-                helper.pop_bitvec(global_state.mstate)
-                * helper.pop_bitvec(global_state.mstate)
-            )
-        )
-
-        return [global_state]
-
-    @StateTransition()
-    def div_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        op0, op1 = (
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-        )
-        if op1 == 0:
-            global_state.mstate.stack.append(symbol_factory.BitVecVal(0, 256))
-        else:
-            global_state.mstate.stack.append(UDiv(op0, op1))
-        return [global_state]
-
-    @StateTransition()
-    def sdiv_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        s0, s1 = (
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-        )
-        if s1 == 0:
-            global_state.mstate.stack.append(symbol_factory.BitVecVal(0, 256))
-        else:
-            global_state.mstate.stack.append(s0 / s1)
-        return [global_state]
-
-    @StateTransition()
-    def mod_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        s0, s1 = (
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-        )
-        global_state.mstate.stack.append(0 if s1 == 0 else URem(s0, s1))
-        return [global_state]
-
-    @StateTransition()
-    def shl_(self, global_state: GlobalState) -> List[GlobalState]:
-        shift, value = (
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-        )
-        global_state.mstate.stack.append(value << shift)
-        return [global_state]
-
-    @StateTransition()
-    def shr_(self, global_state: GlobalState) -> List[GlobalState]:
-        shift, value = (
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-        )
-        global_state.mstate.stack.append(LShR(value, shift))
-        return [global_state]
-
-    @StateTransition()
-    def sar_(self, global_state: GlobalState) -> List[GlobalState]:
-        shift, value = (
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-        )
-        global_state.mstate.stack.append(value >> shift)
-        return [global_state]
-
-    @StateTransition()
-    def smod_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        s0, s1 = (
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-        )
-        global_state.mstate.stack.append(0 if s1 == 0 else SRem(s0, s1))
-        return [global_state]
-
-    @StateTransition()
-    def addmod_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        s0, s1, s2 = (
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-        )
-        global_state.mstate.stack.append(URem(URem(s0, s2) + URem(s1, s2), s2))
-        return [global_state]
-
-    @StateTransition()
-    def mulmod_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        s0, s1, s2 = (
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-            util.pop_bitvec(global_state.mstate),
-        )
-        global_state.mstate.stack.append(URem(URem(s0, s2) * URem(s1, s2), s2))
-        return [global_state]
-
-    @StateTransition()
-    def exp_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        base, exponent = util.pop_bitvec(state), util.pop_bitvec(state)
-        exponentiation, constraint = exponent_function_manager.create_condition(
-            base, exponent
-        )
-        state.stack.append(exponentiation)
-        global_state.world_state.constraints.append(constraint)
-        return [global_state]
-
-    @StateTransition()
-    def signextend_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        mstate = global_state.mstate
-        s0, s1 = mstate.stack.pop(), mstate.stack.pop()
-
-        testbit = s0 * symbol_factory.BitVecVal(8, 256) + symbol_factory.BitVecVal(
-            7, 256
-        )
-        set_testbit = symbol_factory.BitVecVal(1, 256) << testbit
-        sign_bit_set = simplify(Not(s1 & set_testbit == 0))
-
-        mstate.stack.append(
-            simplify(
-                If(
-                    s0 <= 31,
-                    If(
-                        sign_bit_set, s1 | (TT256 - set_testbit), s1 & (set_testbit - 1)
-                    ),
-                    s1,
-                )
-            )
-        )
-
-        return [global_state]
-
-    # Comparisons
-    @StateTransition()
-    def lt_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        exp = ULT(util.pop_bitvec(state), util.pop_bitvec(state))
-        state.stack.append(exp)
-        return [global_state]
-
-    @StateTransition()
-    def gt_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        op1, op2 = util.pop_bitvec(state), util.pop_bitvec(state)
-        exp = UGT(op1, op2)
-        state.stack.append(exp)
-        return [global_state]
-
-    @StateTransition()
-    def slt_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        exp = util.pop_bitvec(state) < util.pop_bitvec(state)
-        state.stack.append(exp)
-        return [global_state]
-
-    @StateTransition()
-    def sgt_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-
-        exp = util.pop_bitvec(state) > util.pop_bitvec(state)
-        state.stack.append(exp)
-        return [global_state]
-
-    @StateTransition()
-    def eq_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-
-        state = global_state.mstate
-
-        op1 = state.stack.pop()
-        op2 = state.stack.pop()
-        if isinstance(op1, Bool):
-            op1 = If(
-                op1, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
-            )
-
-        if isinstance(op2, Bool):
-            op2 = If(
-                op2, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
-            )
-
-        exp = op1 == op2
-
-        state.stack.append(exp)
-        return [global_state]
-
-    @StateTransition()
-    def iszero_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        val = state.stack.pop()
-        exp = Not(val) if isinstance(val, Bool) else val == 0
-
-        exp = If(
-            exp, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
-        )
-        state.stack.append(simplify(exp))
-
-        return [global_state]
-
-    # Call data
-    @StateTransition()
-    def callvalue_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        environment = global_state.environment
-        state.stack.append(environment.callvalue)
-
-        return [global_state]
-
-    @StateTransition()
-    def calldataload_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        environment = global_state.environment
-        op0 = state.stack.pop()
-
-        value = environment.calldata.get_word_at(op0)
-
-        state.stack.append(value)
-
-        return [global_state]
-
-    @StateTransition()
-    def calldatasize_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(global_state.environment.calldata.calldatasize)
-        return [global_state]
-
-    @staticmethod
-    def _calldata_copy_helper(global_state, mstate, mstart, dstart, size):
-        environment = global_state.environment
-
-        try:
-            mstart = util.get_concrete_int(mstart)
-        except TypeError:
-            log.debug("Unsupported symbolic memory offset in CALLDATACOPY")
-            return [global_state]
-
-        try:
-            dstart = util.get_concrete_int(dstart)  # type: Union[int, BitVec]
-        except TypeError:
-            log.debug("Unsupported symbolic calldata offset in CALLDATACOPY")
-            dstart = simplify(dstart)
-
-        try:
-            size = util.get_concrete_int(size)  # type: Union[int, BitVec]
-        except TypeError:
-            log.debug("Unsupported symbolic size in CALLDATACOPY")
-            size = SYMBOLIC_CALLDATA_SIZE  # The excess size will get overwritten
-
-        size = cast(int, size)
-        if size > 0:
-            try:
-                mstate.mem_extend(mstart, size)
-            except TypeError as e:
-                log.debug("Memory allocation error: {}".format(e))
-                mstate.mem_extend(mstart, 1)
-                mstate.memory[mstart] = global_state.new_bitvec(
-                    "calldata_"
-                    + str(environment.active_account.contract_name)
-                    + "["
-                    + str(dstart)
-                    + ": + "
-                    + str(size)
-                    + "]",
-                    8,
-                )
-                return [global_state]
-
-            try:
-                i_data = dstart
-                new_memory = []
-                for i in range(size):
-                    value = environment.calldata[i_data]
-                    new_memory.append(value)
-
-                    i_data = (
-                        i_data + 1
-                        if isinstance(i_data, int)
-                        else simplify(cast(BitVec, i_data) + 1)
-                    )
-                for i in range(len(new_memory)):
-                    mstate.memory[i + mstart] = new_memory[i]
-
-            except IndexError:
-                log.debug("Exception copying calldata to memory")
-
-                mstate.memory[mstart] = global_state.new_bitvec(
-                    "calldata_"
-                    + str(environment.active_account.contract_name)
-                    + "["
-                    + str(dstart)
-                    + ": + "
-                    + str(size)
-                    + "]",
-                    8,
-                )
-        return [global_state]
-
-    @StateTransition()
-    def calldatacopy_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        op0, op1, op2 = state.stack.pop(), state.stack.pop(), state.stack.pop()
-
-        if isinstance(global_state.current_transaction, ContractCreationTransaction):
-            log.debug("Attempt to use CALLDATACOPY in creation transaction")
-            return [global_state]
-
-        return self._calldata_copy_helper(global_state, state, op0, op1, op2)
-
-    # Environment
-    @StateTransition()
-    def address_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        environment = global_state.environment
-        state.stack.append(environment.address)
-        return [global_state]
-
-    @StateTransition()
-    def balance_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        address = state.stack.pop()
-        onchain_access = True
-        if address.symbolic is False:
-            try:
-                balance = global_state.world_state.accounts_exist_or_load(
-                    address.value, self.dynamic_loader
-                ).balance()
-            except ValueError:
-                onchain_access = False
-        else:
-            onchain_access = False
-
-        if onchain_access is False:
-            balance = symbol_factory.BitVecVal(0, 256)
-            for account in global_state.world_state.accounts.values():
-                balance = If(address == account.address, account.balance(), balance)
-        state.stack.append(balance)
-        return [global_state]
-
-    @StateTransition()
-    def origin_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        environment = global_state.environment
-        state.stack.append(environment.origin)
-        return [global_state]
-
-    @StateTransition()
-    def caller_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        environment = global_state.environment
-        state.stack.append(environment.sender)
-        return [global_state]
-
-    @StateTransition()
-    def chainid_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(global_state.environment.chainid)
-        return [global_state]
-
-    @StateTransition()
-    def selfbalance_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        balance = global_state.environment.active_account.balance()
-        global_state.mstate.stack.append(balance)
-        return [global_state]
-
-    @StateTransition()
-    def codesize_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        environment = global_state.environment
-        disassembly = environment.code
-        calldata = global_state.environment.calldata
-        if isinstance(global_state.current_transaction, ContractCreationTransaction):
-            # Hacky way to ensure constructor arguments work - Pick some reasonably large size.
-            no_of_bytes = len(disassembly.bytecode) // 2
-            if isinstance(calldata, ConcreteCalldata):
-                no_of_bytes += calldata.size
-            else:
-                no_of_bytes += 0x200  # space for 16 32-byte arguments
-                global_state.world_state.constraints.append(
-                    global_state.environment.calldata.size == no_of_bytes
-                )
-
-        else:
-            no_of_bytes = len(disassembly.bytecode) // 2
-        state.stack.append(no_of_bytes)
-        return [global_state]
-
-    @staticmethod
-    def _sha3_gas_helper(global_state, length):
-        min_gas, max_gas = calculate_sha3_gas(length)
-        global_state.mstate.min_gas_used += min_gas
-        global_state.mstate.max_gas_used += max_gas
-        StateTransition.check_gas_usage_limit(global_state)
-        return global_state
-
-    @StateTransition(enable_gas=False)
-    def sha3_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-
-        state = global_state.mstate
-        index, op1 = state.stack.pop(), state.stack.pop()
-
-        try:
-            length = util.get_concrete_int(op1)
-        except TypeError:
-            # Can't access symbolic memory offsets
-            length = 64
-            global_state.world_state.constraints.append(op1 == length)
-        Instruction._sha3_gas_helper(global_state, length)
-
-        state.mem_extend(index, length)
-        data_list = [
-            b if isinstance(b, BitVec) else symbol_factory.BitVecVal(b, 8)
-            for b in state.memory[index : index + length]
-        ]
-
-        if len(data_list) > 1:
-            data = simplify(Concat(data_list))
-            # still need to collect the data when data is a concrete value.
-            # @wei
-            if fdg.global_config.flag_preprocessing or fdg.global_config.tx_len == 0:
-                fdg.preprocessing.slot_location.map_concrete_hash_key_to_slot(
-                    data,data_list[-1])
-
-            # @wei
-            if not fdg.global_config.flag_preprocessing:
-                # collect the map from data to concrete hash in the normal execution
-                map_concrete_hash_key_to_slot_normal(data, data_list[-1])
-
-            # # # @wei
-            # # print(f'_=_=_')
-            # # print(f'in sha3_() of instructions.py: ')
-            # # print(f'slot index: {data_list[-1]} ')
-            # # print(f'simplified data: {data}\n')
-            #
-            # seconds_start = time.time()
-            #
-            # if fdg.global_config.flag_preprocessing or fdg.global_config.tx_len == 0:
-            #     fdg.preprocessing.slot_location.map_key_to_slot(Concat(data_list), data_list)
-            # seconds_end = time.time()
-            # print(f'#@time sha3')
-            # print(f'time used(s):{seconds_end - seconds_start}')
-
-        elif len(data_list) == 1:
-            data = data_list[0]
-            # # # @wei
-            # # print(f'_=_=_')
-            # # print(f'in sha3_() of instructions.py: ')
-            # # print(f'slot index: {data_list[-1]} ')
-            # # print(f'simplified data: {data}')
-            #
-            # if fdg.global_config.flag_preprocessing or fdg.global_config.tx_len == 0:
-            #     try:
-            #         # sim_data = simplify_yes(data_list[0])
-            #         fdg.preprocessing.slot_location.map_key_to_slot(data_list[0], data_list)
-            #         print(f'instructions.py: sim_data: {data_list[0]}')
-            #     except:
-            #         print(f'instructions.py: has a problem to collect data')
-
-        else:
-            # @wei
-            print(f'in sha3_() of instructions.py: get empty keccak hash')
-
-            # TODO: handle finding x where func(x)==func("")
-            result = keccak_function_manager.get_empty_keccak_hash()
-            state.stack.append(result)
-            return [global_state]
-
-
-        result = keccak_function_manager.create_keccak(data)
-        # if fdg.global_config.flag_preprocessing or fdg.global_config.tx_len == 0:
-        #     fdg.preprocessing.slot_location.map_key_to_slot(result, data_list)
-
-        state.stack.append(result)
-
-        return [global_state]
-
-    @StateTransition()
-    def gasprice_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(global_state.environment.gasprice)
-        return [global_state]
-
-    @StateTransition()
-    def basefee_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(global_state.environment.basefee)
-        return [global_state]
-
-    @StateTransition()
-    def codecopy_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        memory_offset, code_offset, size = (
-            global_state.mstate.stack.pop(),
-            global_state.mstate.stack.pop(),
-            global_state.mstate.stack.pop(),
-        )
-        code = global_state.environment.code.bytecode
-        if code[0:2] == "0x":
-            code = code[2:]
-        code_size = len(code) // 2
-        if isinstance(global_state.current_transaction, ContractCreationTransaction):
-            # Treat creation code after the expected disassembly as calldata.
-            # This is a slightly hacky way to ensure that symbolic constructor
-            # arguments work correctly.
-            mstate = global_state.mstate
-            offset = code_offset - code_size
-            log.debug("Copying from code offset: {} with size: {}".format(offset, size))
-
-            if isinstance(global_state.environment.calldata, SymbolicCalldata):
-                if code_offset >= code_size:
-                    return self._calldata_copy_helper(
-                        global_state, mstate, memory_offset, offset, size
-                    )
-            else:
-                # Copy from both code and calldata appropriately.
-                concrete_code_offset = helper.get_concrete_int(code_offset)
-                concrete_size = helper.get_concrete_int(size)
-
-                code_copy_offset = concrete_code_offset
-                code_copy_size = (
-                    concrete_size
-                    if concrete_code_offset + concrete_size <= code_size
-                    else code_size - concrete_code_offset
-                )
-                code_copy_size = code_copy_size if code_copy_size >= 0 else 0
-
-                calldata_copy_offset = (
-                    concrete_code_offset - code_size
-                    if concrete_code_offset - code_size > 0
-                    else 0
-                )
-                calldata_copy_size = concrete_code_offset + concrete_size - code_size
-                calldata_copy_size = (
-                    calldata_copy_size if calldata_copy_size >= 0 else 0
-                )
-
-                [global_state] = self._code_copy_helper(
-                    code=global_state.environment.code.bytecode,
-                    memory_offset=memory_offset,
-                    code_offset=code_copy_offset,
-                    size=code_copy_size,
-                    op="CODECOPY",
-                    global_state=global_state,
-                )
-                return self._calldata_copy_helper(
-                    global_state=global_state,
-                    mstate=mstate,
-                    mstart=memory_offset + code_copy_size,
-                    dstart=calldata_copy_offset,
-                    size=calldata_copy_size,
-                )
-
-        return self._code_copy_helper(
-            code=global_state.environment.code.bytecode,
-            memory_offset=memory_offset,
-            code_offset=code_offset,
-            size=size,
-            op="CODECOPY",
-            global_state=global_state,
-        )
-
-    @StateTransition()
-    def extcodesize_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        addr = state.stack.pop()
-        try:
-            addr = hex(helper.get_concrete_int(addr))
-        except TypeError:
-            log.debug("unsupported symbolic address for EXTCODESIZE")
-            state.stack.append(global_state.new_bitvec("extcodesize_" + str(addr), 256))
-            return [global_state]
-        try:
-            code = global_state.world_state.accounts_exist_or_load(
-                addr, self.dynamic_loader
-            ).code.bytecode
-        except (ValueError, AttributeError) as e:
-            log.debug("error accessing contract storage due to: " + str(e))
-            state.stack.append(global_state.new_bitvec("extcodesize_" + str(addr), 256))
-            return [global_state]
-
-        state.stack.append(len(code) // 2)
-
-        return [global_state]
-
-    @staticmethod
-    def _code_copy_helper(
-        code: Union[str, Tuple],
-        memory_offset: Union[int, BitVec],
-        code_offset: Union[int, BitVec],
-        size: Union[int, BitVec],
-        op: str,
-        global_state: GlobalState,
-    ) -> List[GlobalState]:
-        try:
-            concrete_memory_offset = helper.get_concrete_int(memory_offset)
-        except TypeError:
-            log.debug("Unsupported symbolic memory offset in {}".format(op))
-            return [global_state]
-
-        try:
-            concrete_size = helper.get_concrete_int(size)
-            global_state.mstate.mem_extend(concrete_memory_offset, concrete_size)
-
-        except TypeError:
-            # except both attribute error and Exception
-            global_state.mstate.mem_extend(concrete_memory_offset, 1)
-            global_state.mstate.memory[
-                concrete_memory_offset
-            ] = global_state.new_bitvec(
-                "code({})".format(
-                    global_state.environment.active_account.contract_name
-                ),
-                8,
-            )
-            return [global_state]
-
-        try:
-            concrete_code_offset = helper.get_concrete_int(code_offset)
-        except TypeError:
-            log.debug("Unsupported symbolic code offset in {}".format(op))
-            global_state.mstate.mem_extend(concrete_memory_offset, concrete_size)
-            for i in range(concrete_size):
-                global_state.mstate.memory[
-                    concrete_memory_offset + i
-                ] = global_state.new_bitvec(
-                    "code({})".format(
-                        global_state.environment.active_account.contract_name
-                    ),
-                    8,
-                )
-            return [global_state]
-
-        if code[0:2] == "0x":
-            code = code[2:]
-
-        for i in range(concrete_size):
-            if isinstance(code, str):
-                if 2 * (concrete_code_offset + i + 1) > len(code):
-                    break
-
-                global_state.mstate.memory[concrete_memory_offset + i] = int(
-                    code[
-                        2
-                        * (concrete_code_offset + i) : 2
-                        * (concrete_code_offset + i + 1)
-                    ],
-                    16,
-                )
-            else:
-                if (concrete_code_offset + i + 1) > len(code):
-                    break
-
-                global_state.mstate.memory[concrete_memory_offset + i] = code[
-                    concrete_code_offset + i
-                ]
-
-        return [global_state]
-
-    @StateTransition()
-    def extcodecopy_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        addr, memory_offset, code_offset, size = (
-            state.stack.pop(),
-            state.stack.pop(),
-            state.stack.pop(),
-            state.stack.pop(),
-        )
-        try:
-            addr = hex(helper.get_concrete_int(addr))
-        except TypeError:
-            log.debug("unsupported symbolic address for EXTCODECOPY")
-            return [global_state]
-
-        try:
-            code = global_state.world_state.accounts_exist_or_load(
-                addr, self.dynamic_loader
-            ).code.bytecode
-        except (ValueError, AttributeError) as e:
-            log.debug("error accessing contract storage due to: " + str(e))
-            return [global_state]
-
-        return self._code_copy_helper(
-            code=code,
-            memory_offset=memory_offset,
-            code_offset=code_offset,
-            size=size,
-            op="EXTCODECOPY",
-            global_state=global_state,
-        )
-
-    @StateTransition()
-    def extcodehash_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return: List of global states possible, list of size 1 in this case
-        """
-        world_state = global_state.world_state
-        stack = global_state.mstate.stack
-        address = Extract(159, 0, stack.pop())
-
-        if address.symbolic:
-            code_hash = symbol_factory.BitVecVal(int(get_code_hash(""), 16), 256)
-        elif address.value not in world_state.accounts:
-            code_hash = symbol_factory.BitVecVal(0, 256)
-        else:
-            addr = "0" * (40 - len(hex(address.value)[2:])) + hex(address.value)[2:]
-            code = world_state.accounts_exist_or_load(
-                addr, self.dynamic_loader
-            ).code.bytecode
-            code_hash = symbol_factory.BitVecVal(int(get_code_hash(code), 16), 256)
-        stack.append(code_hash)
-        return [global_state]
-
-    @StateTransition()
-    def returndatacopy_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        memory_offset, return_offset, size = (
-            state.stack.pop(),
-            state.stack.pop(),
-            state.stack.pop(),
-        )
-
-        try:
-            concrete_memory_offset = helper.get_concrete_int(memory_offset)
-        except TypeError:
-            log.debug("Unsupported symbolic memory offset in RETURNDATACOPY")
-            return [global_state]
-
-        try:
-            concrete_return_offset = helper.get_concrete_int(return_offset)
-        except TypeError:
-            log.debug("Unsupported symbolic return offset in RETURNDATACOPY")
-            return [global_state]
-
-        try:
-            concrete_size = helper.get_concrete_int(size)
-        except TypeError:
-            log.debug("Unsupported symbolic max_length offset in RETURNDATACOPY")
-            return [global_state]
-
-        if global_state.last_return_data is None:
-            return [global_state]
-
-        global_state.mstate.mem_extend(concrete_memory_offset, concrete_size)
-        for i in range(concrete_size):
-            global_state.mstate.memory[concrete_memory_offset + i] = (
-                global_state.last_return_data[concrete_return_offset + i]
-                if concrete_return_offset + i < global_state.last_return_data.size
-                else 0
-            )
-
-        return [global_state]
-
-    @StateTransition()
-    def returndatasize_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        if global_state.last_return_data:
-            global_state.mstate.stack.append(global_state.last_return_data.size)
-        else:
-            global_state.mstate.stack.append(0)
-        return [global_state]
-
-    @StateTransition()
-    def blockhash_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        blocknumber = state.stack.pop()
-        state.stack.append(
-            global_state.new_bitvec("blockhash_block_" + str(blocknumber), 256)
-        )
-        return [global_state]
-
-    @StateTransition()
-    def coinbase_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(global_state.new_bitvec("coinbase", 256))
-        return [global_state]
-
-    @StateTransition()
-    def timestamp_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(global_state.new_bitvec("timestamp", 256))
-        return [global_state]
-
-    @StateTransition()
-    def number_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(global_state.environment.block_number)
-        return [global_state]
-
-    @StateTransition()
-    def difficulty_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(
-            global_state.new_bitvec("block_difficulty", 256)
-        )
-        return [global_state]
-
-    @StateTransition()
-    def gaslimit_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(global_state.mstate.gas_limit)
-        return [global_state]
-
-    # Memory operations
-    @StateTransition()
-    def mload_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        offset = state.stack.pop()
-
-        state.mem_extend(offset, 32)
-        data = state.memory.get_word_at(offset)
-        state.stack.append(data)
-        return [global_state]
-
-    @StateTransition()
-    def mstore_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        mstart, value = state.stack.pop(), state.stack.pop()
-
-        try:
-            state.mem_extend(mstart, 32)
-        except Exception:
-            log.debug("Error extending memory")
-
-        state.memory.write_word_at(mstart, value)
-
-        return [global_state]
-
-    @StateTransition()
-    def mstore8_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        offset, value = state.stack.pop(), state.stack.pop()
-
-        state.mem_extend(offset, 1)
-
-        try:
-            value_to_write = (
-                util.get_concrete_int(value) % 256
-            )  # type: Union[int, BitVec]
-        except TypeError:  # BitVec
-            value_to_write = Extract(7, 0, value)
-
-        state.memory[offset] = value_to_write
-
-        return [global_state]
-
-    @StateTransition()
-    def sload_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-
-        state = global_state.mstate
-        index = state.stack.pop()
-        state.stack.append(global_state.environment.active_account.storage[index])
-        return [global_state]
-
-    @StateTransition(is_state_mutation_instruction=True)
-    def sstore_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        index, value = state.stack.pop(), state.stack.pop()
-        global_state.environment.active_account.storage[index] = value
-        return [global_state]
-
-    @StateTransition(increment_pc=False, enable_gas=False)
-    def jump_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        state = global_state.mstate
-        disassembly = global_state.environment.code
-        try:
-            jump_addr = util.get_concrete_int(state.stack.pop())
-        except TypeError:
-            raise InvalidJumpDestination("Invalid jump argument (symbolic address)")
-        except IndexError:
-            raise StackUnderflowException()
-
-        index = util.get_instruction_index(disassembly.instruction_list, jump_addr)
-        if index is None:
-            raise InvalidJumpDestination("JUMP to invalid address")
-
-        op_code = disassembly.instruction_list[index]["opcode"]
-
-        if op_code != "JUMPDEST":
-            raise InvalidJumpDestination(
-                "Skipping JUMP to invalid destination (not JUMPDEST): " + str(jump_addr)
-            )
-
-        new_state = copy(global_state)
-        # add JUMP gas cost
-        min_gas, max_gas = get_opcode_gas("JUMP")
-        new_state.mstate.min_gas_used += min_gas
-        new_state.mstate.max_gas_used += max_gas
-
-        # manually set PC to destination
-        new_state.mstate.pc = index
-
-        return [new_state]
-
-
-    @StateTransition(increment_pc=False, enable_gas=False)
-    def jumpi_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-
-        state = global_state.mstate
-        disassembly = global_state.environment.code
-        min_gas, max_gas = get_opcode_gas("JUMPI")
-        states = []
-
-        op0, condition = state.stack.pop(), state.stack.pop()
-
-        try:
-            jump_addr = util.get_concrete_int(op0)
-
-        except TypeError:
-            log.debug("Skipping JUMPI to invalid destination.")
-            global_state.mstate.pc += 1
-            global_state.mstate.min_gas_used += min_gas
-            global_state.mstate.max_gas_used += max_gas
-            return [global_state]
-
-
-        if fdg.global_config.flag_preprocessing:
-            negated = True
-            condi = True
-            negated_cond=True
-            positive_cond=True
-        else:
-            # False case
-            negated = (
-                simplify(Not(condition)) if isinstance(condition, Bool) else condition == 0
-            )
-
-            negated.simplify()  # it is simplified
-
-            # True case
-            condi = simplify(condition) if isinstance(condition, Bool) else condition != 0
-
-            condi.simplify()
-
-            negated_cond = (type(negated) == bool and negated) or (
-                isinstance(negated, Bool) and not is_false(negated)
-            )
-            positive_cond = (type(condi) == bool and condi) or (
-                isinstance(condi, Bool) and not is_false(condi)
-            )
-
-
-        if  negated_cond:
-            # States have to be deep copied during a fork as summaries assume independence across states.
-            new_state = deepcopy(global_state)
-            # add JUMPI gas cost
-            new_state.mstate.min_gas_used += min_gas
-            new_state.mstate.max_gas_used += max_gas
-
-            # manually increment PC
-            new_state.mstate.depth += 1
-            new_state.mstate.pc += 1
-            new_state.world_state.constraints.append(negated)
-            states.append(new_state)
-        else:
-            log.debug("Pruned unreachable states.")
-
-        # Get jump destination
-        index = util.get_instruction_index(disassembly.instruction_list, jump_addr)
-
-        if index is None:
-            log.debug("Invalid jump destination: " + str(jump_addr))
-            return states
-
-        instr = disassembly.instruction_list[index]
-
-        if instr["opcode"] == "JUMPDEST":
-            if  positive_cond:
-                new_state = deepcopy(global_state)
-                # add JUMPI gas cost
-                new_state.mstate.min_gas_used += min_gas
-                new_state.mstate.max_gas_used += max_gas
-
-                # manually set PC to destination
-                new_state.mstate.pc = index
-                new_state.mstate.depth += 1
-                new_state.world_state.constraints.append(condi)
-                states.append(new_state)
-            else:
-                log.debug("Pruned unreachable states.")
-        return states
-
-    @StateTransition()
-    def beginsub_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-        This opcode depicts the start of the subroutine
-        """
-        raise OutOfGasException("Encountered BEGINSUB")
-
-    @StateTransition()
-    def jumpsub_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-        Jump to the subroutine
-        """
-        disassembly = global_state.environment.code
-        try:
-            location = util.get_concrete_int(global_state.mstate.stack.pop())
-        except TypeError:
-            raise VmException("Encountered symbolic JUMPSUB location")
-        index = util.get_instruction_index(disassembly.instruction_list, location)
-        instr = disassembly.instruction_list[index]
-
-        if instr["opcode"] != "BEGINSUB":
-            raise VmException(
-                "Encountered invalid JUMPSUB location :{}".format(instr["address"])
-            )
-        global_state.mstate.subroutine_stack.append(global_state.mstate.pc + 1)
-        global_state.mstate.pc = location
-        return [global_state]
-
-    @StateTransition(increment_pc=False)
-    def returnsub_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-        Returns control to the caller of the subroutine
-        """
-        global_state.mstate.pc = global_state.mstate.subroutine_stack.pop()
-        return [global_state]
-
-    @StateTransition()
-    def pc_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        index = global_state.mstate.pc
-        program_counter = global_state.environment.code.instruction_list[index][
-            "address"
-        ]
-        global_state.mstate.stack.append(symbol_factory.BitVecVal(program_counter, 256))
-
-        return [global_state]
-
-    @StateTransition()
-    def msize_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        global_state.mstate.stack.append(global_state.mstate.memory_size)
-        return [global_state]
-
-    @StateTransition()
-    def gas_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        # TODO: Push a Constrained variable which lies between min gas and max gas
-        global_state.mstate.stack.append(global_state.new_bitvec("gas", 256))
-        return [global_state]
-
-    @StateTransition(is_state_mutation_instruction=True)
-    def log_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        # TODO: implement me
-        state = global_state.mstate
-        depth = int(self.op_code[3:])
-        state.stack.pop(), state.stack.pop()
-        _ = [state.stack.pop() for _ in range(depth)]
-        # Not supported
-        return [global_state]
-
-    def _create_transaction_helper(
-        self, global_state, call_value, mem_offset, mem_size, create2_salt=None
-    ) -> List[GlobalState]:
-        mstate = global_state.mstate
-        environment = global_state.environment
-        world_state = global_state.world_state
-
-        call_data = get_call_data(global_state, mem_offset, mem_offset + mem_size)
-        code_raw = []
-        code_end = call_data.size
-        size = call_data.size
-
-        if isinstance(size, BitVec):
-            # Other size restriction checks handle this
-            if size.symbolic:
-                size = 10**4
-            else:
-                size = size.value
-        code_raw = []
-        constraints = global_state.world_state.constraints
-        try:
-            model = get_model(constraints)
-        except UnsatError:
-            model = None
-        except TypeError:
-            # # fix the error:
-            # # TypeError: unhashable        type: 'list'
-            model = None
-
-        if isinstance(call_data, ConcreteCalldata):
-            for element in call_data.concrete(model):
-                if isinstance(element, BitVec) and element.symbolic:
-                    break
-                if isinstance(element, BitVec):
-                    code_raw.append(element.value)
-                else:
-                    code_raw.append(element)
-
-        if len(code_raw) < 1:
-            global_state.mstate.stack.append(1)
-            log.debug("No code found for trying to execute a create type instruction.")
-            return [global_state]
-
-        code_str = bytes.hex(bytes(code_raw))
-
-        next_transaction_id = tx_id_manager.get_next_tx_id()
-        constructor_arguments = ConcreteCalldata(
-            next_transaction_id, call_data[code_end:]
-        )
-        code = Disassembly(code_str)
-
-        caller = environment.active_account.address
-        gas_price = environment.gasprice
-        origin = environment.origin
-
-        contract_address = None  # type: Union[BitVec, int]
-        Instruction._sha3_gas_helper(global_state, len(code_str[2:]) // 2)
-
-        if create2_salt:
-            if create2_salt.symbolic:
-                if create2_salt.size() != 256:
-                    pad = symbol_factory.BitVecVal(0, 256 - create2_salt.size())
-                    create2_salt = Concat(pad, create2_salt)
-                address = keccak_function_manager.create_keccak(
-                    Concat(
-                        symbol_factory.BitVecVal(255, 8),
-                        caller,
-                        create2_salt,
-                        symbol_factory.BitVecVal(int(get_code_hash(code_str), 16), 256),
-                    )
-                )
-                contract_address = Extract(255, 96, address)
-
-            else:
-                salt = hex(create2_salt.value)[2:]
-                salt = "0" * (64 - len(salt)) + salt
-
-                addr = hex(caller.value)[2:]
-                addr = "0" * (40 - len(addr)) + addr
-
-                contract_address = int(
-                    get_code_hash("0xff" + addr + salt + get_code_hash(code_str)[2:])[
-                        26:
-                    ],
-                    16,
-                )
-        transaction = ContractCreationTransaction(
-            world_state=world_state,
-            caller=caller,
-            code=code,
-            call_data=constructor_arguments,
-            gas_price=gas_price,
-            gas_limit=mstate.gas_limit,
-            origin=origin,
-            call_value=call_value,
-            contract_address=contract_address,
-        )
-        log.info("Raise transaction start signal")
-        raise TransactionStartSignal(transaction, self.op_code, global_state)
-
-    @StateTransition(is_state_mutation_instruction=True)
-    def create_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        call_value, mem_offset, mem_size = global_state.mstate.pop(3)
-        return self._create_transaction_helper(
-            global_state, call_value, mem_offset, mem_size
-        )
-
-    @StateTransition()
-    def create_post(self, global_state: GlobalState) -> List[GlobalState]:
-        return self._handle_create_type_post(global_state)
-
-    @StateTransition(is_state_mutation_instruction=True)
-    def create2_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        call_value, mem_offset, mem_size, salt = global_state.mstate.pop(4)
-
-        return self._create_transaction_helper(
-            global_state, call_value, mem_offset, mem_size, salt
-        )
-
-    @StateTransition()
-    def create2_post(self, global_state: GlobalState) -> List[GlobalState]:
-        return self._handle_create_type_post(global_state, opcode="create2")
-
-    @staticmethod
-    def _handle_create_type_post(global_state, opcode="create"):
-        if opcode == "create2":
-            global_state.mstate.pop(4)
-        else:
-            global_state.mstate.pop(3)
-        if global_state.last_return_data:
-            return_val = symbol_factory.BitVecVal(
-                int(global_state.last_return_data.return_data, 16), 256
-            )
-        else:
-            return_val = symbol_factory.BitVecVal(0, 256)
-        global_state.mstate.stack.append(return_val)
-        return [global_state]
-
-    @StateTransition()
-    def return_(self, global_state: GlobalState):
-        """
-
-        :param global_state:
-        """
-        state = global_state.mstate
-        offset, length = state.stack.pop(), state.stack.pop()
-        if length.symbolic:
-            return_data = [global_state.new_bitvec("return_data", 8)]
-            log.debug("Return with symbolic length or offset. Not supported")
-        else:
-            state.mem_extend(offset, length)
-            StateTransition.check_gas_usage_limit(global_state)
-            return_data = state.memory[offset : offset + length]
-        global_state.current_transaction.end(
-            global_state, ReturnData(return_data, length)
-        )
-
-    @StateTransition(is_state_mutation_instruction=True)
-    def selfdestruct_(self, global_state: GlobalState):
-        """
-
-        :param global_state:
-        """
-        target = global_state.mstate.stack.pop()
-        transfer_amount = global_state.environment.active_account.balance()
-        # Often the target of the selfdestruct instruction will be symbolic
-        # If it isn't then we'll transfer the balance to the indicated contract
-        global_state.world_state.balances[target] += transfer_amount
-
-        global_state.environment.active_account = deepcopy(
-            global_state.environment.active_account
-        )
-        global_state.accounts[
-            global_state.environment.active_account.address.value
-        ] = global_state.environment.active_account
-
-        global_state.environment.active_account.set_balance(0)
-        global_state.environment.active_account.deleted = True
-        global_state.current_transaction.end(global_state)
-
-    @StateTransition()
-    def revert_(self, global_state: GlobalState) -> None:
-        """
-
-        :param global_state:
-        """
-        state = global_state.mstate
-        offset, length = state.stack.pop(), state.stack.pop()
-        if length.symbolic is False:
-            return_data = [
-                global_state.new_bitvec(
-                    f"{global_state.current_transaction.id}_return_data_{i}", 8
-                )
-                for i in range(length.value)
-            ]
-        else:
-            return_data = [
-                If(
-                    i < length,
-                    global_state.new_bitvec(
-                        f"{global_state.current_transaction.id}_return_data_{i}", 8
-                    ),
-                    0,
-                )
-                for i in range(300)
-            ]
-
-        try:
-            return_data = state.memory[
-                util.get_concrete_int(offset) : util.get_concrete_int(offset + length)
-            ]
-        except TypeError:
-            log.debug("Return with symbolic length or offset. Not supported")
-        global_state.current_transaction.end(
-            global_state, return_data=ReturnData(return_data, length), revert=True
-        )
-
-    @StateTransition()
-    def assert_fail_(self, global_state: GlobalState):
-        """
-
-        :param global_state:
-        """
-        # 0xfe: designated invalid opcode
-        raise InvalidInstruction
-
-    @StateTransition()
-    def invalid_(self, global_state: GlobalState):
-        """
-
-        :param global_state:
-        """
-        raise InvalidInstruction
-
-    @StateTransition()
-    def stop_(self, global_state: GlobalState):
-        """
-
-        :param global_state:
-        """
-        global_state.current_transaction.end(global_state)
-
-    @staticmethod
-    def _write_symbolic_returndata(
-        global_state: GlobalState, memory_out_offset: BitVec, memory_out_size: BitVec
-    ):
-        """
-        Writes symbolic return-data into memory, The memory offset and size should be concrete
-        :param global_state:
-        :param memory_out_offset:
-        :param memory_out_size:
-        :return:
-        """
-        if memory_out_offset.symbolic is True or memory_out_size.symbolic is True:
-            return
-        return_data = []
-        return_data_size = global_state.new_bitvec("returndatasize", 256)
-
-        for i in range(memory_out_size.value):
-            data = global_state.new_bitvec(
-                "call_output_var({})_{}".format(
-                    simplify(memory_out_offset + i), global_state.mstate.pc
-                ),
-                8,
-            )
-            return_data.append(data)
-
-        global_state.mstate.mem_extend(memory_out_offset, memory_out_size)
-        for i in range(memory_out_size.value):
-            global_state.mstate.memory[memory_out_offset + i] = If(
-                i <= return_data_size,
-                return_data[i],
-                global_state.mstate.memory[memory_out_offset + i],
-            )
-
-        global_state.last_return_data = ReturnData(
-            return_data=return_data, return_data_size=return_data_size
-        )
-
-    @StateTransition()
-    def call_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        instr = global_state.get_current_instruction()
-        environment = global_state.environment
-
-        memory_out_size, memory_out_offset = global_state.mstate.stack[-7:-5]
-        try:
-            (
-                callee_address,
-                callee_account,
-                call_data,
-                value,
-                gas,
-                memory_out_offset,
-                memory_out_size,
-            ) = get_call_parameters(global_state, self.dynamic_loader, True)
-
-            if callee_account is not None and callee_account.code.bytecode == "":
-                log.debug("The call is related to ether transfer between accounts")
-                sender = environment.active_account.address
-                receiver = callee_account.address
-
-                transfer_ether(global_state, sender, receiver, value)
-                self._write_symbolic_returndata(
-                    global_state, memory_out_offset, memory_out_size
-                )
-
-                global_state.mstate.stack.append(
-                    global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-                )
-                return [global_state]
-
-        except ValueError as e:
-            log.debug(
-                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
-                    e
-                )
-            )
-            self._write_symbolic_returndata(
-                global_state, memory_out_offset, memory_out_size
-            )
-            # TODO: decide what to do in this case
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-            return [global_state]
-
-        if environment.static:
-            if isinstance(value, int) and value > 0:
-                raise WriteProtection(
-                    "Cannot call with non zero value in a static call"
-                )
-            if isinstance(value, BitVec):
-                if value.symbolic:
-                    global_state.world_state.constraints.append(
-                        value == symbol_factory.BitVecVal(0, 256)
-                    )
-                elif value.value > 0:
-                    raise WriteProtection(
-                        "Cannot call with non zero value in a static call"
-                    )
-
-        native_result = native_call(
-            global_state, callee_address, call_data, memory_out_offset, memory_out_size
-        )
-        if native_result:
-            return native_result
-        transaction = MessageCallTransaction(
-            world_state=global_state.world_state,
-            gas_price=environment.gasprice,
-            gas_limit=gas,
-            origin=environment.origin,
-            caller=environment.active_account.address,
-            callee_account=callee_account,
-            call_data=call_data,
-            call_value=value,
-            static=environment.static,
-        )
-        raise TransactionStartSignal(transaction, self.op_code, global_state)
-
-    @StateTransition()
-    def call_post(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-
-        return self.post_handler(global_state, function_name="call")
-
-    @StateTransition()
-    def callcode_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        instr = global_state.get_current_instruction()
-        environment = global_state.environment
-        memory_out_size, memory_out_offset = global_state.mstate.stack[-7:-5]
-        try:
-            (
-                callee_address,
-                callee_account,
-                call_data,
-                value,
-                gas,
-                _,
-                _,
-            ) = get_call_parameters(global_state, self.dynamic_loader, True)
-
-            if callee_account is not None and callee_account.code.bytecode == "":
-                log.debug("The call is related to ether transfer between accounts")
-                sender = global_state.environment.active_account.address
-                receiver = callee_account.address
-                transfer_ether(global_state, sender, receiver, value)
-                self._write_symbolic_returndata(
-                    global_state, memory_out_offset, memory_out_size
-                )
-
-                global_state.mstate.stack.append(
-                    global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-                )
-                return [global_state]
-
-        except ValueError as e:
-            log.debug(
-                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
-                    e
-                )
-            )
-            self._write_symbolic_returndata(
-                global_state, memory_out_offset, memory_out_size
-            )
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-            return [global_state]
-
-        native_result = native_call(
-            global_state, callee_address, call_data, memory_out_offset, memory_out_size
-        )
-        if native_result:
-            return native_result
-
-        transaction = MessageCallTransaction(
-            world_state=global_state.world_state,
-            gas_price=environment.gasprice,
-            gas_limit=gas,
-            origin=environment.origin,
-            code=callee_account.code,
-            caller=environment.address,
-            callee_account=environment.active_account,
-            call_data=call_data,
-            call_value=value,
-            static=environment.static,
-        )
-        raise TransactionStartSignal(transaction, self.op_code, global_state)
-
-    @StateTransition()
-    def callcode_post(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        instr = global_state.get_current_instruction()
-        memory_out_size, memory_out_offset = global_state.mstate.stack[-7:-5]
-        try:
-            (
-                _,
-                _,
-                _,
-                _,
-                _,
-                memory_out_offset,
-                memory_out_size,
-            ) = get_call_parameters(global_state, self.dynamic_loader, True)
-        except ValueError as e:
-            log.debug(
-                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
-                    e
-                )
-            )
-            self._write_symbolic_returndata(
-                global_state, memory_out_offset, memory_out_size
-            )
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-            return [global_state]
-
-        if global_state.last_return_data is None:
-            # Put return value on stack
-            return_value = global_state.new_bitvec(
-                "retval_" + str(instr["address"]), 256
-            )
-            global_state.mstate.stack.append(return_value)
-            self._write_symbolic_returndata(
-                global_state, memory_out_offset, memory_out_size
-            )
-            global_state.world_state.constraints.append(return_value == 0)
-            return [global_state]
-
-        try:
-            memory_out_offset = (
-                util.get_concrete_int(memory_out_offset)
-                if isinstance(memory_out_offset, Expression)
-                else memory_out_offset
-            )
-            memory_out_size = (
-                util.get_concrete_int(memory_out_size)
-                if isinstance(memory_out_size, Expression)
-                else memory_out_size
-            )
-        except TypeError:
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-            return [global_state]
-
-        # Copy memory
-        global_state.mstate.mem_extend(
-            memory_out_offset, min(memory_out_size, global_state.last_return_data.size)
-        )
-        if global_state.last_return_data.size.symbolic:
-            ret_size = 500
-        else:
-            ret_size = global_state.last_return_data.size.value
-        for i in range(min(memory_out_size, ret_size)):
-            global_state.mstate.memory[
-                i + memory_out_offset
-            ] = global_state.last_return_data[i]
-
-        # Put return value on stack
-        return_value = global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-        global_state.mstate.stack.append(return_value)
-        global_state.world_state.constraints.append(return_value == 1)
-        return [global_state]
-
-    @StateTransition()
-    def delegatecall_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        instr = global_state.get_current_instruction()
-        environment = global_state.environment
-        memory_out_size, memory_out_offset = global_state.mstate.stack[-6:-4]
-
-        try:
-            (
-                callee_address,
-                callee_account,
-                call_data,
-                value,
-                gas,
-                _,
-                _,
-            ) = get_call_parameters(global_state, self.dynamic_loader)
-
-            if callee_account is not None and callee_account.code.bytecode == "":
-                log.debug("The call is related to ether transfer between accounts")
-                sender = global_state.environment.active_account.address
-                receiver = callee_account.address
-
-                transfer_ether(global_state, sender, receiver, value)
-                self._write_symbolic_returndata(
-                    global_state, memory_out_offset, memory_out_size
-                )
-                global_state.mstate.stack.append(
-                    global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-                )
-                return [global_state]
-        except ValueError as e:
-            log.debug(
-                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
-                    e
-                )
-            )
-            self._write_symbolic_returndata(
-                global_state, memory_out_offset, memory_out_size
-            )
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-            return [global_state]
-
-        native_result = native_call(
-            global_state, callee_address, call_data, memory_out_offset, memory_out_size
-        )
-        if native_result:
-            return native_result
-
-        transaction = MessageCallTransaction(
-            world_state=global_state.world_state,
-            gas_price=environment.gasprice,
-            gas_limit=gas,
-            origin=environment.origin,
-            code=callee_account.code,
-            caller=environment.sender,
-            callee_account=environment.active_account,
-            call_data=call_data,
-            call_value=environment.callvalue,
-            static=environment.static,
-        )
-        raise TransactionStartSignal(transaction, self.op_code, global_state)
-
-    @StateTransition()
-    def delegatecall_post(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        instr = global_state.get_current_instruction()
-        memory_out_size, memory_out_offset = global_state.mstate.stack[-6:-4]
-
-        try:
-            (
-                _,
-                _,
-                _,
-                _,
-                _,
-                memory_out_offset,
-                memory_out_size,
-            ) = get_call_parameters(global_state, self.dynamic_loader)
-        except ValueError as e:
-            log.debug(
-                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
-                    e
-                )
-            )
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-            self._write_symbolic_returndata(
-                global_state, memory_out_offset, memory_out_size
-            )
-            return [global_state]
-
-        if global_state.last_return_data is None:
-            # Put return value on stack
-            return_value = global_state.new_bitvec(
-                "retval_" + str(instr["address"]), 256
-            )
-            global_state.mstate.stack.append(return_value)
-            global_state.world_state.constraints.append(return_value == 0)
-            return [global_state]
-
-        try:
-            memory_out_offset = (
-                util.get_concrete_int(memory_out_offset)
-                if isinstance(memory_out_offset, Expression)
-                else memory_out_offset
-            )
-            memory_out_size = (
-                util.get_concrete_int(memory_out_size)
-                if isinstance(memory_out_size, Expression)
-                else memory_out_size
-            )
-        except TypeError:
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-            return [global_state]
-
-            # Copy memory
-        global_state.mstate.mem_extend(
-            memory_out_offset, min(memory_out_size, global_state.last_return_data.size)
-        )
-        if global_state.last_return_data.size.symbolic:
-            ret_size = 500
-        else:
-            ret_size = global_state.last_return_data.size.value
-        for i in range(min(memory_out_size, ret_size)):
-            global_state.mstate.memory[
-                i + memory_out_offset
-            ] = global_state.last_return_data[i]
-
-        # Put return value on stack
-        return_value = global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-        global_state.mstate.stack.append(return_value)
-        global_state.world_state.constraints.append(return_value == 1)
-        return [global_state]
-
-    @StateTransition()
-    def staticcall_(self, global_state: GlobalState) -> List[GlobalState]:
-        """
-
-        :param global_state:
-        :return:
-        """
-        instr = global_state.get_current_instruction()
-        environment = global_state.environment
-        memory_out_size, memory_out_offset = global_state.mstate.stack[-6:-4]
-        try:
-            (
-                callee_address,
-                callee_account,
-                call_data,
-                value,
-                gas,
-                memory_out_offset,
-                memory_out_size,
-            ) = get_call_parameters(global_state, self.dynamic_loader)
-
-            if callee_account is not None and callee_account.code.bytecode == "":
-                log.debug("The call is related to ether transfer between accounts")
-                sender = environment.active_account.address
-                receiver = callee_account.address
-                transfer_ether(global_state, sender, receiver, value)
-                self._write_symbolic_returndata(
-                    global_state, memory_out_offset, memory_out_size
-                )
-                global_state.mstate.stack.append(
-                    global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-                )
-
-                return [global_state]
-
-        except ValueError as e:
-            log.debug(
-                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
-                    e
-                )
-            )
-            self._write_symbolic_returndata(
-                global_state, memory_out_offset, memory_out_size
-            )
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-
-            return [global_state]
-
-        native_result = native_call(
-            global_state, callee_address, call_data, memory_out_offset, memory_out_size
-        )
-
-        if native_result:
-            return native_result
-
-        transaction = MessageCallTransaction(
-            world_state=global_state.world_state,
-            gas_price=environment.gasprice,
-            gas_limit=gas,
-            origin=environment.origin,
-            code=callee_account.code,
-            caller=environment.address,
-            callee_account=callee_account,
-            call_data=call_data,
-            call_value=value,
-            static=True,
-        )
-        raise TransactionStartSignal(transaction, self.op_code, global_state)
-
-    @StateTransition()
-    def staticcall_post(self, global_state: GlobalState) -> List[GlobalState]:
-        return self.post_handler(global_state, function_name="staticcall")
-
-    def post_handler(self, global_state, function_name: str):
-        instr = global_state.get_current_instruction()
-        if function_name in ("staticcall", "delegatecall"):
-            memory_out_size, memory_out_offset = global_state.mstate.stack[-6:-4]
-        else:
-            memory_out_size, memory_out_offset = global_state.mstate.stack[-7:-5]
-
-        try:
-            with_value = function_name != "staticcall"
-            (
-                _,
-                _,
-                _,
-                _,
-                _,
-                memory_out_offset,
-                memory_out_size,
-            ) = get_call_parameters(global_state, self.dynamic_loader, with_value)
-        except ValueError as e:
-            log.debug(
-                "Could not determine required parameters for {}, putting fresh symbol on the stack. \n{}".format(
-                    function_name, e
-                )
-            )
-            self._write_symbolic_returndata(
-                global_state, memory_out_offset, memory_out_size
-            )
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-            return [global_state]
-
-        if global_state.last_return_data is None:
-            # Put return value on stack
-            return_value = global_state.new_bitvec(
-                "retval_" + str(instr["address"]), 256
-            )
-            global_state.mstate.stack.append(return_value)
-            return [global_state]
-
-        try:
-            memory_out_offset = (
-                util.get_concrete_int(memory_out_offset)
-                if isinstance(memory_out_offset, Expression)
-                else memory_out_offset
-            )
-            memory_out_size = (
-                util.get_concrete_int(memory_out_size)
-                if isinstance(memory_out_size, Expression)
-                else memory_out_size
-            )
-        except TypeError:
-            global_state.mstate.stack.append(
-                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
-            )
-            return [global_state]
-
-        global_state.mstate.mem_extend(
-            memory_out_offset, min(memory_out_size, global_state.last_return_data.size)
-        )
-        if global_state.last_return_data.size.symbolic:
-            ret_size = 500
-        else:
-            ret_size = global_state.last_return_data.size.value
-
-        for i in range(min(memory_out_size, ret_size)):
-            global_state.mstate.memory[
-                i + memory_out_offset
-            ] = global_state.last_return_data[i]
-
-        # Put return value on stack
-        return_value = global_state.new_bitvec(
-            "retval_" + str(global_state.get_current_instruction()["address"]), 256
-        )
-        global_state.mstate.stack.append(return_value)
-        global_state.world_state.constraints.append(return_value == 1)
-
-        return [global_state]
+"""This module contains a representation class for EVM instructions and
+transitions between them."""
+import logging
+import time
+
+from copy import copy, deepcopy
+from typing import cast, Callable, List, Union, Tuple
+
+from fdg.expression_slot import map_concrete_hash_key_to_slot_normal
+from mythril.exceptions import UnsatError
+from mythril.laser.smt import (
+    Extract,
+    Expression,
+    UDiv,
+    simplify,
+    Concat,
+    ULT,
+    UGT,
+    BitVec,
+    is_false,
+    URem,
+    SRem,
+    If,
+    Bool,
+    Not,
+    LShR,
+    UGE,
+)
+from mythril.laser.smt import symbol_factory
+
+from mythril.disassembler.disassembly import Disassembly
+
+from mythril.laser.ethereum.state.calldata import ConcreteCalldata, SymbolicCalldata
+
+import mythril.laser.ethereum.util as helper
+from mythril.laser.ethereum import util
+from mythril.laser.ethereum.function_managers import (
+    keccak_function_manager,
+    exponent_function_manager,
+)
+
+from mythril.laser.ethereum.call import (
+    get_call_parameters,
+    native_call,
+    get_call_data,
+    SYMBOLIC_CALLDATA_SIZE,
+)
+from mythril.laser.ethereum.evm_exceptions import (
+    VmException,
+    StackUnderflowException,
+    InvalidJumpDestination,
+    InvalidInstruction,
+    OutOfGasException,
+    WriteProtection,
+)
+from mythril.laser.ethereum.instruction_data import get_opcode_gas, calculate_sha3_gas
+from mythril.laser.ethereum.state.global_state import GlobalState
+from mythril.laser.ethereum.state.return_data import ReturnData
+
+from mythril.laser.ethereum.transaction import (
+    MessageCallTransaction,
+    TransactionStartSignal,
+    ContractCreationTransaction,
+    tx_id_manager,
+)
+from mythril.support.model import get_model
+from mythril.support.support_utils import get_code_hash
+
+from mythril.support.loader import DynLoader
+import fdg
+from mythril.laser.smt.expression import simplify_yes
+
+log = logging.getLogger(__name__)
+
+TT256 = symbol_factory.BitVecVal(0, 256)
+TT256M1 = symbol_factory.BitVecVal(2**256 - 1, 256)
+
+
+def transfer_ether(
+    global_state: GlobalState,
+    sender: BitVec,
+    receiver: BitVec,
+    value: Union[int, BitVec],
+):
+    """
+    Perform an Ether transfer between two accounts
+
+    :param global_state: The global state in which the Ether transfer occurs
+    :param sender: The sender of the Ether
+    :param receiver: The recipient of the Ether
+    :param value: The amount of Ether to send
+    :return:
+    """
+    value = value if isinstance(value, BitVec) else symbol_factory.BitVecVal(value, 256)
+
+    global_state.world_state.constraints.append(
+        UGE(global_state.world_state.balances[sender], value)
+    )
+    global_state.world_state.balances[receiver] += value
+    global_state.world_state.balances[sender] -= value
+
+
+class StateTransition(object):
+    """Decorator that handles global state copy and original return.
+
+    This decorator calls the decorated instruction mutator function on a
+    copy of the state that is passed to it. After the call, the
+    resulting new states' program counter is automatically incremented
+    if `increment_pc=True`.
+    """
+
+    def __init__(
+        self, increment_pc=True, enable_gas=True, is_state_mutation_instruction=False
+    ):
+        """
+
+        :param increment_pc:
+        :param enable_gas:
+        :param is_state_mutation_instruction: The function mutates state
+        """
+        self.increment_pc = increment_pc
+        self.enable_gas = enable_gas
+        self.is_state_mutation_instruction = is_state_mutation_instruction
+
+    @staticmethod
+    def call_on_state_copy(func: Callable, func_obj: "Instruction", state: GlobalState):
+        """
+
+        :param func:
+        :param func_obj:
+        :param state:
+        :return:
+        """
+        global_state_copy = copy(state)
+        return func(func_obj, global_state_copy)
+
+    def increment_states_pc(self, states: List[GlobalState]) -> List[GlobalState]:
+        """
+
+        :param states:
+        :return:
+        """
+        if self.increment_pc:
+            for state in states:
+                state.mstate.pc += 1
+        return states
+
+    @staticmethod
+    def check_gas_usage_limit(global_state: GlobalState):
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.check_gas()
+        if isinstance(global_state.current_transaction.gas_limit, BitVec):
+            value = global_state.current_transaction.gas_limit.value
+            if value is None:
+                return
+            global_state.current_transaction.gas_limit = value
+        if (
+            global_state.mstate.min_gas_used
+            >= global_state.current_transaction.gas_limit
+        ):
+            raise OutOfGasException()
+
+    def accumulate_gas(self, global_state: GlobalState):
+        """
+
+        :param global_state:
+        :return:
+        """
+        if not self.enable_gas:
+            return global_state
+        opcode = global_state.instruction["opcode"]
+        min_gas, max_gas = get_opcode_gas(opcode)
+        global_state.mstate.min_gas_used += min_gas
+        global_state.mstate.max_gas_used += max_gas
+        self.check_gas_usage_limit(global_state)
+
+        return global_state
+
+    def __call__(self, func: Callable) -> Callable:
+        def wrapper(
+            func_obj: "Instruction", global_state: GlobalState
+        ) -> List[GlobalState]:
+            """
+
+            :param func_obj:
+            :param global_state:
+            :return:
+            """
+            if self.is_state_mutation_instruction and global_state.environment.static:
+                raise WriteProtection(
+                    "The function {} cannot be executed in a static call".format(
+                        func.__name__[:-1]
+                    )
+                )
+
+            new_global_states = self.call_on_state_copy(func, func_obj, global_state)
+            new_global_states = [
+                self.accumulate_gas(state) for state in new_global_states
+            ]
+
+            return self.increment_states_pc(new_global_states)
+
+        return wrapper
+
+
+class Instruction:
+    """Instruction class is used to mutate a state according to the current
+    instruction."""
+
+    def __init__(
+        self,
+        op_code: str,
+        dynamic_loader: DynLoader,
+        pre_hooks: List[Callable] = None,
+        post_hooks: List[Callable] = None,
+    ) -> None:
+        """
+
+        :param op_code:
+        :param dynamic_loader:
+        :param iprof:
+        """
+        self.dynamic_loader = dynamic_loader
+        self.op_code = op_code.upper()
+        self.pre_hook = pre_hooks if pre_hooks else []
+        self.post_hook = post_hooks if post_hooks else []
+
+    def _execute_pre_hooks(self, global_state: GlobalState):
+        for hook in self.pre_hook:
+            hook(global_state)
+
+    def _execute_post_hooks(self, global_state: GlobalState):
+        for hook in self.post_hook:
+            hook(global_state)
+
+    def evaluate(self, global_state: GlobalState, post=False) -> List[GlobalState]:
+        """Performs the mutation for this instruction.
+
+        :param global_state:
+        :param post:
+        :return:
+        """
+        # Generalize some ops
+        log.debug("Evaluating %s at %i", self.op_code, global_state.mstate.pc)
+
+        op = self.op_code.lower()
+        if self.op_code.startswith("PUSH"):
+            op = "push"
+        elif self.op_code.startswith("DUP"):
+            op = "dup"
+        elif self.op_code.startswith("SWAP"):
+            op = "swap"
+        elif self.op_code.startswith("LOG"):
+            op = "log"
+        elif self.op_code.startswith("EMPTY"):#@wei: to handle opcode "-"
+            op = "empty"
+        instruction_mutator = (
+            getattr(self, op + "_", None)
+            if not post
+            else getattr(self, op + "_" + "post", None)
+        )
+        if instruction_mutator is None:
+            raise NotImplementedError
+
+        self._execute_pre_hooks(global_state)
+        result = instruction_mutator(global_state)
+        self._execute_post_hooks(global_state)
+
+        return result
+
+    @StateTransition()
+    def jumpdest_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        return [global_state]
+
+    @StateTransition()
+    def push_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        push_instruction = global_state.get_current_instruction()
+        push_value = push_instruction["argument"]
+        try:
+            length_of_value = 2 * int(push_instruction["opcode"][4:])
+        except ValueError:
+            raise VmException("Invalid Push instruction")
+
+        if type(push_value) == tuple:
+            if type(push_value[0]) == int:
+                new_value = symbol_factory.BitVecVal(push_value[0], 8)
+            else:
+                new_value = push_value[0]
+            if len(push_value) > 1:
+                for val in push_value[1:]:
+                    if type(val) == int:
+                        new_value = Concat(new_value, symbol_factory.BitVecVal(val, 8))
+                    else:
+                        new_value = Concat(new_value, val)
+
+            pad_length = length_of_value // 2 - len(push_value)
+
+            if pad_length > 0:
+                new_value = Concat(new_value, symbol_factory.BitVecVal(0, pad_length))
+            if new_value.size() < 256:
+                new_value = Concat(
+                    symbol_factory.BitVecVal(0, 256 - new_value.size()), new_value
+                )
+            # global_state.mstate.stack.append(new_value)
+            global_state.mstate.stack.append(simplify_yes(new_value))
+
+        else:
+            push_value += "0" * max(length_of_value - (len(push_value) - 2), 0)
+            # global_state.mstate.stack.append(
+            #     symbol_factory.BitVecVal(int(push_value, 16), 256)
+            # )
+
+            global_state.mstate.stack.append(
+                simplify_yes(symbol_factory.BitVecVal(int(push_value, 16), 256))
+            )
+
+        return [global_state]
+
+    @StateTransition()
+    def dup_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        value = int(global_state.get_current_instruction()["opcode"][3:], 10)
+        global_state.mstate.stack.append(global_state.mstate.stack[-value])
+        return [global_state]
+
+    @StateTransition()
+    def empty_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        return [global_state]
+
+    @StateTransition()
+    def swap_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        depth = int(self.op_code[4:])
+        stack = global_state.mstate.stack
+        stack[-depth - 1], stack[-1] = stack[-1], stack[-depth - 1]
+        return [global_state]
+
+    @StateTransition()
+    def pop_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.pop()
+        return [global_state]
+
+    @StateTransition()
+    def and_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        stack = global_state.mstate.stack
+        op1, op2 = stack.pop(), stack.pop()
+        if isinstance(op1, Bool):
+            op1 = If(
+                op1, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
+            )
+        if isinstance(op2, Bool):
+            op2 = If(
+                op2, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
+            )
+        if not isinstance(op1, Expression):
+            op1 = symbol_factory.BitVecVal(op1, 256)
+        if not isinstance(op2, Expression):
+            op2 = symbol_factory.BitVecVal(op2, 256)
+        stack.append(op1 & op2)
+
+        return [global_state]
+
+    @StateTransition()
+    def or_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        stack = global_state.mstate.stack
+        op1, op2 = stack.pop(), stack.pop()
+
+        if isinstance(op1, Bool):
+            op1 = If(
+                op1, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
+            )
+
+        if isinstance(op2, Bool):
+            op2 = If(
+                op2, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
+            )
+
+        stack.append(op1 | op2)
+
+        return [global_state]
+
+    @StateTransition()
+    def xor_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        mstate = global_state.mstate
+        mstate.stack.append(mstate.stack.pop() ^ mstate.stack.pop())
+        return [global_state]
+
+    @StateTransition()
+    def not_(self, global_state: GlobalState):
+        """
+
+        :param global_state:
+        :return:
+        """
+        mstate = global_state.mstate
+        mstate.stack.append(TT256M1 - mstate.stack.pop())
+        return [global_state]
+
+    @StateTransition()
+    def byte_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        mstate = global_state.mstate
+        op0, op1 = mstate.stack.pop(), mstate.stack.pop()
+        if not isinstance(op1, Expression):
+            op1 = symbol_factory.BitVecVal(op1, 256)
+        try:
+            index = util.get_concrete_int(op0)
+            offset = (31 - index) * 8
+            if offset >= 0:
+                result = simplify(
+                    Concat(
+                        symbol_factory.BitVecVal(0, 248),
+                        Extract(offset + 7, offset, op1),
+                    )
+                )  # type: Union[int, Expression]
+            else:
+                result = 0
+        except TypeError:
+            log.debug("BYTE: Unsupported symbolic byte offset")
+            result = global_state.new_bitvec(
+                str(simplify(op1)) + "[" + str(simplify(op0)) + "]", 256
+            )
+
+        mstate.stack.append(result)
+        return [global_state]
+
+    # Arithmetic
+    @StateTransition()
+    def add_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(
+            (
+                helper.pop_bitvec(global_state.mstate)
+                + helper.pop_bitvec(global_state.mstate)
+            )
+        )
+
+        return [global_state]
+
+    @StateTransition()
+    def sub_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(
+            (
+                helper.pop_bitvec(global_state.mstate)
+                - helper.pop_bitvec(global_state.mstate)
+            )
+        )
+        return [global_state]
+
+    @StateTransition()
+    def mul_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(
+            (
+                helper.pop_bitvec(global_state.mstate)
+                * helper.pop_bitvec(global_state.mstate)
+            )
+        )
+
+        return [global_state]
+
+    @StateTransition()
+    def div_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        op0, op1 = (
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+        )
+        if op1 == 0:
+            global_state.mstate.stack.append(symbol_factory.BitVecVal(0, 256))
+        else:
+            global_state.mstate.stack.append(UDiv(op0, op1))
+        return [global_state]
+
+    @StateTransition()
+    def sdiv_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        s0, s1 = (
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+        )
+        if s1 == 0:
+            global_state.mstate.stack.append(symbol_factory.BitVecVal(0, 256))
+        else:
+            global_state.mstate.stack.append(s0 / s1)
+        return [global_state]
+
+    @StateTransition()
+    def mod_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        s0, s1 = (
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+        )
+        global_state.mstate.stack.append(0 if s1 == 0 else URem(s0, s1))
+        return [global_state]
+
+    @StateTransition()
+    def shl_(self, global_state: GlobalState) -> List[GlobalState]:
+        shift, value = (
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+        )
+        global_state.mstate.stack.append(value << shift)
+        return [global_state]
+
+    @StateTransition()
+    def shr_(self, global_state: GlobalState) -> List[GlobalState]:
+        shift, value = (
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+        )
+        global_state.mstate.stack.append(LShR(value, shift))
+        return [global_state]
+
+    @StateTransition()
+    def sar_(self, global_state: GlobalState) -> List[GlobalState]:
+        shift, value = (
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+        )
+        global_state.mstate.stack.append(value >> shift)
+        return [global_state]
+
+    @StateTransition()
+    def smod_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        s0, s1 = (
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+        )
+        global_state.mstate.stack.append(0 if s1 == 0 else SRem(s0, s1))
+        return [global_state]
+
+    @StateTransition()
+    def addmod_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        s0, s1, s2 = (
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+        )
+        global_state.mstate.stack.append(URem(URem(s0, s2) + URem(s1, s2), s2))
+        return [global_state]
+
+    @StateTransition()
+    def mulmod_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        s0, s1, s2 = (
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+            util.pop_bitvec(global_state.mstate),
+        )
+        global_state.mstate.stack.append(URem(URem(s0, s2) * URem(s1, s2), s2))
+        return [global_state]
+
+    @StateTransition()
+    def exp_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        base, exponent = util.pop_bitvec(state), util.pop_bitvec(state)
+        exponentiation, constraint = exponent_function_manager.create_condition(
+            base, exponent
+        )
+        state.stack.append(exponentiation)
+        global_state.world_state.constraints.append(constraint)
+        return [global_state]
+
+    @StateTransition()
+    def signextend_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        mstate = global_state.mstate
+        s0, s1 = mstate.stack.pop(), mstate.stack.pop()
+
+        testbit = s0 * symbol_factory.BitVecVal(8, 256) + symbol_factory.BitVecVal(
+            7, 256
+        )
+        set_testbit = symbol_factory.BitVecVal(1, 256) << testbit
+        sign_bit_set = simplify(Not(s1 & set_testbit == 0))
+
+        mstate.stack.append(
+            simplify(
+                If(
+                    s0 <= 31,
+                    If(
+                        sign_bit_set, s1 | (TT256 - set_testbit), s1 & (set_testbit - 1)
+                    ),
+                    s1,
+                )
+            )
+        )
+
+        return [global_state]
+
+    # Comparisons
+    @StateTransition()
+    def lt_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        exp = ULT(util.pop_bitvec(state), util.pop_bitvec(state))
+        state.stack.append(exp)
+        return [global_state]
+
+    @StateTransition()
+    def gt_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        op1, op2 = util.pop_bitvec(state), util.pop_bitvec(state)
+        exp = UGT(op1, op2)
+        state.stack.append(exp)
+        return [global_state]
+
+    @StateTransition()
+    def slt_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        exp = util.pop_bitvec(state) < util.pop_bitvec(state)
+        state.stack.append(exp)
+        return [global_state]
+
+    @StateTransition()
+    def sgt_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+
+        exp = util.pop_bitvec(state) > util.pop_bitvec(state)
+        state.stack.append(exp)
+        return [global_state]
+
+    @StateTransition()
+    def eq_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+
+        state = global_state.mstate
+
+        op1 = state.stack.pop()
+        op2 = state.stack.pop()
+        if isinstance(op1, Bool):
+            op1 = If(
+                op1, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
+            )
+
+        if isinstance(op2, Bool):
+            op2 = If(
+                op2, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
+            )
+
+        exp = op1 == op2
+
+        state.stack.append(exp)
+        return [global_state]
+
+    @StateTransition()
+    def iszero_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        val = state.stack.pop()
+        exp = Not(val) if isinstance(val, Bool) else val == 0
+
+        exp = If(
+            exp, symbol_factory.BitVecVal(1, 256), symbol_factory.BitVecVal(0, 256)
+        )
+        state.stack.append(simplify(exp))
+
+        return [global_state]
+
+    # Call data
+    @StateTransition()
+    def callvalue_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        environment = global_state.environment
+        state.stack.append(environment.callvalue)
+
+        return [global_state]
+
+    @StateTransition()
+    def calldataload_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        environment = global_state.environment
+        op0 = state.stack.pop()
+
+        value = environment.calldata.get_word_at(op0)
+
+        state.stack.append(value)
+
+        return [global_state]
+
+    @StateTransition()
+    def calldatasize_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(global_state.environment.calldata.calldatasize)
+        return [global_state]
+
+    @staticmethod
+    def _calldata_copy_helper(global_state, mstate, mstart, dstart, size):
+        environment = global_state.environment
+
+        try:
+            mstart = util.get_concrete_int(mstart)
+        except TypeError:
+            log.debug("Unsupported symbolic memory offset in CALLDATACOPY")
+            return [global_state]
+
+        try:
+            dstart = util.get_concrete_int(dstart)  # type: Union[int, BitVec]
+        except TypeError:
+            log.debug("Unsupported symbolic calldata offset in CALLDATACOPY")
+            dstart = simplify(dstart)
+
+        try:
+            size = util.get_concrete_int(size)  # type: Union[int, BitVec]
+        except TypeError:
+            log.debug("Unsupported symbolic size in CALLDATACOPY")
+            size = SYMBOLIC_CALLDATA_SIZE  # The excess size will get overwritten
+
+        size = cast(int, size)
+        if size > 0:
+            try:
+                mstate.mem_extend(mstart, size)
+            except TypeError as e:
+                log.debug("Memory allocation error: {}".format(e))
+                mstate.mem_extend(mstart, 1)
+                mstate.memory[mstart] = global_state.new_bitvec(
+                    "calldata_"
+                    + str(environment.active_account.contract_name)
+                    + "["
+                    + str(dstart)
+                    + ": + "
+                    + str(size)
+                    + "]",
+                    8,
+                )
+                return [global_state]
+
+            try:
+                i_data = dstart
+                new_memory = []
+                for i in range(size):
+                    value = environment.calldata[i_data]
+                    new_memory.append(value)
+
+                    i_data = (
+                        i_data + 1
+                        if isinstance(i_data, int)
+                        else simplify(cast(BitVec, i_data) + 1)
+                    )
+                for i in range(len(new_memory)):
+                    mstate.memory[i + mstart] = new_memory[i]
+
+            except IndexError:
+                log.debug("Exception copying calldata to memory")
+
+                mstate.memory[mstart] = global_state.new_bitvec(
+                    "calldata_"
+                    + str(environment.active_account.contract_name)
+                    + "["
+                    + str(dstart)
+                    + ": + "
+                    + str(size)
+                    + "]",
+                    8,
+                )
+        return [global_state]
+
+    @StateTransition()
+    def calldatacopy_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        op0, op1, op2 = state.stack.pop(), state.stack.pop(), state.stack.pop()
+
+        if isinstance(global_state.current_transaction, ContractCreationTransaction):
+            log.debug("Attempt to use CALLDATACOPY in creation transaction")
+            return [global_state]
+
+        return self._calldata_copy_helper(global_state, state, op0, op1, op2)
+
+    # Environment
+    @StateTransition()
+    def address_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        environment = global_state.environment
+        state.stack.append(environment.address)
+        return [global_state]
+
+    @StateTransition()
+    def balance_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        address = state.stack.pop()
+        onchain_access = True
+        if address.symbolic is False:
+            try:
+                balance = global_state.world_state.accounts_exist_or_load(
+                    address.value, self.dynamic_loader
+                ).balance()
+            except ValueError:
+                onchain_access = False
+        else:
+            onchain_access = False
+
+        if onchain_access is False:
+            balance = symbol_factory.BitVecVal(0, 256)
+            for account in global_state.world_state.accounts.values():
+                balance = If(address == account.address, account.balance(), balance)
+        state.stack.append(balance)
+        return [global_state]
+
+    @StateTransition()
+    def origin_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        environment = global_state.environment
+        state.stack.append(environment.origin)
+        return [global_state]
+
+    @StateTransition()
+    def caller_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        environment = global_state.environment
+        state.stack.append(environment.sender)
+        return [global_state]
+
+    @StateTransition()
+    def chainid_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(global_state.environment.chainid)
+        return [global_state]
+
+    @StateTransition()
+    def selfbalance_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        balance = global_state.environment.active_account.balance()
+        global_state.mstate.stack.append(balance)
+        return [global_state]
+
+    @StateTransition()
+    def codesize_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        environment = global_state.environment
+        disassembly = environment.code
+        calldata = global_state.environment.calldata
+        if isinstance(global_state.current_transaction, ContractCreationTransaction):
+            # Hacky way to ensure constructor arguments work - Pick some reasonably large size.
+            no_of_bytes = len(disassembly.bytecode) // 2
+            if isinstance(calldata, ConcreteCalldata):
+                no_of_bytes += calldata.size
+            else:
+                no_of_bytes += 0x200  # space for 16 32-byte arguments
+                global_state.world_state.constraints.append(
+                    global_state.environment.calldata.size == no_of_bytes
+                )
+
+        else:
+            no_of_bytes = len(disassembly.bytecode) // 2
+        state.stack.append(no_of_bytes)
+        return [global_state]
+
+    @staticmethod
+    def _sha3_gas_helper(global_state, length):
+        min_gas, max_gas = calculate_sha3_gas(length)
+        global_state.mstate.min_gas_used += min_gas
+        global_state.mstate.max_gas_used += max_gas
+        StateTransition.check_gas_usage_limit(global_state)
+        return global_state
+
+    @StateTransition(enable_gas=False)
+    def sha3_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+
+        state = global_state.mstate
+        index, op1 = state.stack.pop(), state.stack.pop()
+
+        try:
+            length = util.get_concrete_int(op1)
+        except TypeError:
+            # Can't access symbolic memory offsets
+            length = 64
+            global_state.world_state.constraints.append(op1 == length)
+        Instruction._sha3_gas_helper(global_state, length)
+
+        state.mem_extend(index, length)
+        data_list = [
+            b if isinstance(b, BitVec) else symbol_factory.BitVecVal(b, 8)
+            for b in state.memory[index : index + length]
+        ]
+
+        if len(data_list) > 1:
+            data = simplify(Concat(data_list))
+            # still need to collect the data when data is a concrete value.
+            # @wei
+            if fdg.global_config.flag_preprocessing or fdg.global_config.tx_len == 0:
+                fdg.preprocessing.slot_location.map_concrete_hash_key_to_slot(
+                    data,data_list[-1])
+
+            # @wei
+            if not fdg.global_config.flag_preprocessing:
+                # collect the map from data to concrete hash in the normal execution
+                map_concrete_hash_key_to_slot_normal(data, data_list[-1])
+
+            # # # @wei
+            # # print(f'_=_=_')
+            # # print(f'in sha3_() of instructions.py: ')
+            # # print(f'slot index: {data_list[-1]} ')
+            # # print(f'simplified data: {data}\n')
+            #
+            # seconds_start = time.time()
+            #
+            # if fdg.global_config.flag_preprocessing or fdg.global_config.tx_len == 0:
+            #     fdg.preprocessing.slot_location.map_key_to_slot(Concat(data_list), data_list)
+            # seconds_end = time.time()
+            # print(f'#@time sha3')
+            # print(f'time used(s):{seconds_end - seconds_start}')
+
+        elif len(data_list) == 1:
+            data = data_list[0]
+            # # # @wei
+            # # print(f'_=_=_')
+            # # print(f'in sha3_() of instructions.py: ')
+            # # print(f'slot index: {data_list[-1]} ')
+            # # print(f'simplified data: {data}')
+            #
+            # if fdg.global_config.flag_preprocessing or fdg.global_config.tx_len == 0:
+            #     try:
+            #         # sim_data = simplify_yes(data_list[0])
+            #         fdg.preprocessing.slot_location.map_key_to_slot(data_list[0], data_list)
+            #         print(f'instructions.py: sim_data: {data_list[0]}')
+            #     except:
+            #         print(f'instructions.py: has a problem to collect data')
+
+        else:
+            # @wei
+            print(f'in sha3_() of instructions.py: get empty keccak hash')
+
+            # TODO: handle finding x where func(x)==func("")
+            result = keccak_function_manager.get_empty_keccak_hash()
+            state.stack.append(result)
+            return [global_state]
+
+
+        result = keccak_function_manager.create_keccak(data)
+        # if fdg.global_config.flag_preprocessing or fdg.global_config.tx_len == 0:
+        #     fdg.preprocessing.slot_location.map_key_to_slot(result, data_list)
+
+        state.stack.append(result)
+
+        return [global_state]
+
+    @StateTransition()
+    def gasprice_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(global_state.environment.gasprice)
+        return [global_state]
+
+    @StateTransition()
+    def basefee_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(global_state.environment.basefee)
+        return [global_state]
+
+    @StateTransition()
+    def codecopy_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        memory_offset, code_offset, size = (
+            global_state.mstate.stack.pop(),
+            global_state.mstate.stack.pop(),
+            global_state.mstate.stack.pop(),
+        )
+        code = global_state.environment.code.bytecode
+        if code[0:2] == "0x":
+            code = code[2:]
+        code_size = len(code) // 2
+        if isinstance(global_state.current_transaction, ContractCreationTransaction):
+            # Treat creation code after the expected disassembly as calldata.
+            # This is a slightly hacky way to ensure that symbolic constructor
+            # arguments work correctly.
+            mstate = global_state.mstate
+            offset = code_offset - code_size
+            log.debug("Copying from code offset: {} with size: {}".format(offset, size))
+
+            if isinstance(global_state.environment.calldata, SymbolicCalldata):
+                if code_offset >= code_size:
+                    return self._calldata_copy_helper(
+                        global_state, mstate, memory_offset, offset, size
+                    )
+            else:
+                # Copy from both code and calldata appropriately.
+                concrete_code_offset = helper.get_concrete_int(code_offset)
+                concrete_size = helper.get_concrete_int(size)
+
+                code_copy_offset = concrete_code_offset
+                code_copy_size = (
+                    concrete_size
+                    if concrete_code_offset + concrete_size <= code_size
+                    else code_size - concrete_code_offset
+                )
+                code_copy_size = code_copy_size if code_copy_size >= 0 else 0
+
+                calldata_copy_offset = (
+                    concrete_code_offset - code_size
+                    if concrete_code_offset - code_size > 0
+                    else 0
+                )
+                calldata_copy_size = concrete_code_offset + concrete_size - code_size
+                calldata_copy_size = (
+                    calldata_copy_size if calldata_copy_size >= 0 else 0
+                )
+
+                [global_state] = self._code_copy_helper(
+                    code=global_state.environment.code.bytecode,
+                    memory_offset=memory_offset,
+                    code_offset=code_copy_offset,
+                    size=code_copy_size,
+                    op="CODECOPY",
+                    global_state=global_state,
+                )
+                return self._calldata_copy_helper(
+                    global_state=global_state,
+                    mstate=mstate,
+                    mstart=memory_offset + code_copy_size,
+                    dstart=calldata_copy_offset,
+                    size=calldata_copy_size,
+                )
+
+        return self._code_copy_helper(
+            code=global_state.environment.code.bytecode,
+            memory_offset=memory_offset,
+            code_offset=code_offset,
+            size=size,
+            op="CODECOPY",
+            global_state=global_state,
+        )
+
+    @StateTransition()
+    def extcodesize_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        addr = state.stack.pop()
+        try:
+            addr = hex(helper.get_concrete_int(addr))
+        except TypeError:
+            log.debug("unsupported symbolic address for EXTCODESIZE")
+            state.stack.append(global_state.new_bitvec("extcodesize_" + str(addr), 256))
+            return [global_state]
+        try:
+            code = global_state.world_state.accounts_exist_or_load(
+                addr, self.dynamic_loader
+            ).code.bytecode
+        except (ValueError, AttributeError) as e:
+            log.debug("error accessing contract storage due to: " + str(e))
+            state.stack.append(global_state.new_bitvec("extcodesize_" + str(addr), 256))
+            return [global_state]
+
+        state.stack.append(len(code) // 2)
+
+        return [global_state]
+
+    @staticmethod
+    def _code_copy_helper(
+        code: Union[str, Tuple],
+        memory_offset: Union[int, BitVec],
+        code_offset: Union[int, BitVec],
+        size: Union[int, BitVec],
+        op: str,
+        global_state: GlobalState,
+    ) -> List[GlobalState]:
+        try:
+            concrete_memory_offset = helper.get_concrete_int(memory_offset)
+        except TypeError:
+            log.debug("Unsupported symbolic memory offset in {}".format(op))
+            return [global_state]
+
+        try:
+            concrete_size = helper.get_concrete_int(size)
+            global_state.mstate.mem_extend(concrete_memory_offset, concrete_size)
+
+        except TypeError:
+            # except both attribute error and Exception
+            global_state.mstate.mem_extend(concrete_memory_offset, 1)
+            global_state.mstate.memory[
+                concrete_memory_offset
+            ] = global_state.new_bitvec(
+                "code({})".format(
+                    global_state.environment.active_account.contract_name
+                ),
+                8,
+            )
+            return [global_state]
+
+        try:
+            concrete_code_offset = helper.get_concrete_int(code_offset)
+        except TypeError:
+            log.debug("Unsupported symbolic code offset in {}".format(op))
+            global_state.mstate.mem_extend(concrete_memory_offset, concrete_size)
+            for i in range(concrete_size):
+                global_state.mstate.memory[
+                    concrete_memory_offset + i
+                ] = global_state.new_bitvec(
+                    "code({})".format(
+                        global_state.environment.active_account.contract_name
+                    ),
+                    8,
+                )
+            return [global_state]
+
+        if code[0:2] == "0x":
+            code = code[2:]
+
+        for i in range(concrete_size):
+            if isinstance(code, str):
+                if 2 * (concrete_code_offset + i + 1) > len(code):
+                    break
+
+                global_state.mstate.memory[concrete_memory_offset + i] = int(
+                    code[
+                        2
+                        * (concrete_code_offset + i) : 2
+                        * (concrete_code_offset + i + 1)
+                    ],
+                    16,
+                )
+            else:
+                if (concrete_code_offset + i + 1) > len(code):
+                    break
+
+                global_state.mstate.memory[concrete_memory_offset + i] = code[
+                    concrete_code_offset + i
+                ]
+
+        return [global_state]
+
+    @StateTransition()
+    def extcodecopy_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        addr, memory_offset, code_offset, size = (
+            state.stack.pop(),
+            state.stack.pop(),
+            state.stack.pop(),
+            state.stack.pop(),
+        )
+        try:
+            addr = hex(helper.get_concrete_int(addr))
+        except TypeError:
+            log.debug("unsupported symbolic address for EXTCODECOPY")
+            return [global_state]
+
+        try:
+            code = global_state.world_state.accounts_exist_or_load(
+                addr, self.dynamic_loader
+            ).code.bytecode
+        except (ValueError, AttributeError) as e:
+            log.debug("error accessing contract storage due to: " + str(e))
+            return [global_state]
+
+        return self._code_copy_helper(
+            code=code,
+            memory_offset=memory_offset,
+            code_offset=code_offset,
+            size=size,
+            op="EXTCODECOPY",
+            global_state=global_state,
+        )
+
+    @StateTransition()
+    def extcodehash_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return: List of global states possible, list of size 1 in this case
+        """
+        world_state = global_state.world_state
+        stack = global_state.mstate.stack
+        address = Extract(159, 0, stack.pop())
+
+        if address.symbolic:
+            code_hash = symbol_factory.BitVecVal(int(get_code_hash(""), 16), 256)
+        elif address.value not in world_state.accounts:
+            code_hash = symbol_factory.BitVecVal(0, 256)
+        else:
+            addr = "0" * (40 - len(hex(address.value)[2:])) + hex(address.value)[2:]
+            code = world_state.accounts_exist_or_load(
+                addr, self.dynamic_loader
+            ).code.bytecode
+            code_hash = symbol_factory.BitVecVal(int(get_code_hash(code), 16), 256)
+        stack.append(code_hash)
+        return [global_state]
+
+    @StateTransition()
+    def returndatacopy_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        memory_offset, return_offset, size = (
+            state.stack.pop(),
+            state.stack.pop(),
+            state.stack.pop(),
+        )
+
+        try:
+            concrete_memory_offset = helper.get_concrete_int(memory_offset)
+        except TypeError:
+            log.debug("Unsupported symbolic memory offset in RETURNDATACOPY")
+            return [global_state]
+
+        try:
+            concrete_return_offset = helper.get_concrete_int(return_offset)
+        except TypeError:
+            log.debug("Unsupported symbolic return offset in RETURNDATACOPY")
+            return [global_state]
+
+        try:
+            concrete_size = helper.get_concrete_int(size)
+        except TypeError:
+            log.debug("Unsupported symbolic max_length offset in RETURNDATACOPY")
+            return [global_state]
+
+        if global_state.last_return_data is None:
+            return [global_state]
+
+        global_state.mstate.mem_extend(concrete_memory_offset, concrete_size)
+        for i in range(concrete_size):
+            global_state.mstate.memory[concrete_memory_offset + i] = (
+                global_state.last_return_data[concrete_return_offset + i]
+                if concrete_return_offset + i < global_state.last_return_data.size
+                else 0
+            )
+
+        return [global_state]
+
+    @StateTransition()
+    def returndatasize_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        if global_state.last_return_data:
+            global_state.mstate.stack.append(global_state.last_return_data.size)
+        else:
+            global_state.mstate.stack.append(0)
+        return [global_state]
+
+    @StateTransition()
+    def blockhash_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        blocknumber = state.stack.pop()
+        state.stack.append(
+            global_state.new_bitvec("blockhash_block_" + str(blocknumber), 256)
+        )
+        return [global_state]
+
+    @StateTransition()
+    def coinbase_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(global_state.new_bitvec("coinbase", 256))
+        return [global_state]
+
+    @StateTransition()
+    def timestamp_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(global_state.new_bitvec("timestamp", 256))
+        return [global_state]
+
+    @StateTransition()
+    def number_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(global_state.environment.block_number)
+        return [global_state]
+
+    @StateTransition()
+    def difficulty_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(
+            global_state.new_bitvec("block_difficulty", 256)
+        )
+        return [global_state]
+
+    @StateTransition()
+    def gaslimit_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(global_state.mstate.gas_limit)
+        return [global_state]
+
+    # Memory operations
+    @StateTransition()
+    def mload_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        offset = state.stack.pop()
+
+        state.mem_extend(offset, 32)
+        data = state.memory.get_word_at(offset)
+        state.stack.append(data)
+        return [global_state]
+
+    @StateTransition()
+    def mstore_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        mstart, value = state.stack.pop(), state.stack.pop()
+
+        try:
+            state.mem_extend(mstart, 32)
+        except Exception:
+            log.debug("Error extending memory")
+
+        state.memory.write_word_at(mstart, value)
+
+        return [global_state]
+
+    @StateTransition()
+    def mstore8_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        offset, value = state.stack.pop(), state.stack.pop()
+
+        state.mem_extend(offset, 1)
+
+        try:
+            value_to_write = (
+                util.get_concrete_int(value) % 256
+            )  # type: Union[int, BitVec]
+        except TypeError:  # BitVec
+            value_to_write = Extract(7, 0, value)
+
+        state.memory[offset] = value_to_write
+
+        return [global_state]
+
+    @StateTransition()
+    def sload_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+
+        state = global_state.mstate
+        index = state.stack.pop()
+        state.stack.append(global_state.environment.active_account.storage[index])
+        return [global_state]
+
+    @StateTransition(is_state_mutation_instruction=True)
+    def sstore_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        index, value = state.stack.pop(), state.stack.pop()
+        global_state.environment.active_account.storage[index] = value
+        return [global_state]
+
+    @StateTransition(increment_pc=False, enable_gas=False)
+    def jump_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        state = global_state.mstate
+        disassembly = global_state.environment.code
+        try:
+            jump_addr = util.get_concrete_int(state.stack.pop())
+        except TypeError:
+            raise InvalidJumpDestination("Invalid jump argument (symbolic address)")
+        except IndexError:
+            raise StackUnderflowException()
+
+        index = util.get_instruction_index(disassembly.instruction_list, jump_addr)
+        if index is None:
+            raise InvalidJumpDestination("JUMP to invalid address")
+
+        op_code = disassembly.instruction_list[index]["opcode"]
+
+        if op_code != "JUMPDEST":
+            raise InvalidJumpDestination(
+                "Skipping JUMP to invalid destination (not JUMPDEST): " + str(jump_addr)
+            )
+
+        new_state = copy(global_state)
+        # add JUMP gas cost
+        min_gas, max_gas = get_opcode_gas("JUMP")
+        new_state.mstate.min_gas_used += min_gas
+        new_state.mstate.max_gas_used += max_gas
+
+        # manually set PC to destination
+        new_state.mstate.pc = index
+
+        return [new_state]
+
+
+    @StateTransition(increment_pc=False, enable_gas=False)
+    def jumpi_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+
+        state = global_state.mstate
+        disassembly = global_state.environment.code
+        min_gas, max_gas = get_opcode_gas("JUMPI")
+        states = []
+
+        op0, condition = state.stack.pop(), state.stack.pop()
+
+        try:
+            jump_addr = util.get_concrete_int(op0)
+
+        except TypeError:
+            log.debug("Skipping JUMPI to invalid destination.")
+            global_state.mstate.pc += 1
+            global_state.mstate.min_gas_used += min_gas
+            global_state.mstate.max_gas_used += max_gas
+            return [global_state]
+
+
+        if fdg.global_config.flag_preprocessing:
+            negated = True
+            condi = True
+            negated_cond=True
+            positive_cond=True
+        else:
+            # False case
+            negated = (
+                simplify(Not(condition)) if isinstance(condition, Bool) else condition == 0
+            )
+
+            negated.simplify()  # it is simplified
+
+            # True case
+            condi = simplify(condition) if isinstance(condition, Bool) else condition != 0
+
+            condi.simplify()
+
+            negated_cond = (type(negated) == bool and negated) or (
+                isinstance(negated, Bool) and not is_false(negated)
+            )
+            positive_cond = (type(condi) == bool and condi) or (
+                isinstance(condi, Bool) and not is_false(condi)
+            )
+
+
+        if  negated_cond:
+            # States have to be deep copied during a fork as summaries assume independence across states.
+            new_state = deepcopy(global_state)
+            # add JUMPI gas cost
+            new_state.mstate.min_gas_used += min_gas
+            new_state.mstate.max_gas_used += max_gas
+
+            # manually increment PC
+            new_state.mstate.depth += 1
+            new_state.mstate.pc += 1
+            new_state.world_state.constraints.append(negated)
+            states.append(new_state)
+        else:
+            log.debug("Pruned unreachable states.")
+
+        # Get jump destination
+        index = util.get_instruction_index(disassembly.instruction_list, jump_addr)
+
+        if index is None:
+            log.debug("Invalid jump destination: " + str(jump_addr))
+            return states
+
+        instr = disassembly.instruction_list[index]
+
+        if instr["opcode"] == "JUMPDEST":
+            if  positive_cond:
+                new_state = deepcopy(global_state)
+                # add JUMPI gas cost
+                new_state.mstate.min_gas_used += min_gas
+                new_state.mstate.max_gas_used += max_gas
+
+                # manually set PC to destination
+                new_state.mstate.pc = index
+                new_state.mstate.depth += 1
+                new_state.world_state.constraints.append(condi)
+                states.append(new_state)
+            else:
+                log.debug("Pruned unreachable states.")
+        return states
+
+    @StateTransition()
+    def beginsub_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+        This opcode depicts the start of the subroutine
+        """
+        raise OutOfGasException("Encountered BEGINSUB")
+
+    @StateTransition()
+    def jumpsub_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+        Jump to the subroutine
+        """
+        disassembly = global_state.environment.code
+        try:
+            location = util.get_concrete_int(global_state.mstate.stack.pop())
+        except TypeError:
+            raise VmException("Encountered symbolic JUMPSUB location")
+        index = util.get_instruction_index(disassembly.instruction_list, location)
+        instr = disassembly.instruction_list[index]
+
+        if instr["opcode"] != "BEGINSUB":
+            raise VmException(
+                "Encountered invalid JUMPSUB location :{}".format(instr["address"])
+            )
+        global_state.mstate.subroutine_stack.append(global_state.mstate.pc + 1)
+        global_state.mstate.pc = location
+        return [global_state]
+
+    @StateTransition(increment_pc=False)
+    def returnsub_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+        Returns control to the caller of the subroutine
+        """
+        global_state.mstate.pc = global_state.mstate.subroutine_stack.pop()
+        return [global_state]
+
+    @StateTransition()
+    def pc_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        index = global_state.mstate.pc
+        program_counter = global_state.environment.code.instruction_list[index][
+            "address"
+        ]
+        global_state.mstate.stack.append(symbol_factory.BitVecVal(program_counter, 256))
+
+        return [global_state]
+
+    @StateTransition()
+    def msize_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        global_state.mstate.stack.append(global_state.mstate.memory_size)
+        return [global_state]
+
+    @StateTransition()
+    def gas_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        # TODO: Push a Constrained variable which lies between min gas and max gas
+        global_state.mstate.stack.append(global_state.new_bitvec("gas", 256))
+        return [global_state]
+
+    @StateTransition(is_state_mutation_instruction=True)
+    def log_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        # TODO: implement me
+        state = global_state.mstate
+        depth = int(self.op_code[3:])
+        state.stack.pop(), state.stack.pop()
+        _ = [state.stack.pop() for _ in range(depth)]
+        # Not supported
+        return [global_state]
+
+    def _create_transaction_helper(
+        self, global_state, call_value, mem_offset, mem_size, create2_salt=None
+    ) -> List[GlobalState]:
+        mstate = global_state.mstate
+        environment = global_state.environment
+        world_state = global_state.world_state
+
+        call_data = get_call_data(global_state, mem_offset, mem_offset + mem_size)
+        code_raw = []
+        code_end = call_data.size
+        size = call_data.size
+
+        if isinstance(size, BitVec):
+            # Other size restriction checks handle this
+            if size.symbolic:
+                size = 10**4
+            else:
+                size = size.value
+        code_raw = []
+        constraints = global_state.world_state.constraints
+        try:
+            model = get_model(constraints)
+        except UnsatError:
+            model = None
+        except TypeError:
+            # # fix the error:
+            # # TypeError: unhashable        type: 'list'
+            model = None
+
+        if isinstance(call_data, ConcreteCalldata):
+            for element in call_data.concrete(model):
+                if isinstance(element, BitVec) and element.symbolic:
+                    break
+                if isinstance(element, BitVec):
+                    code_raw.append(element.value)
+                else:
+                    code_raw.append(element)
+
+        if len(code_raw) < 1:
+            global_state.mstate.stack.append(1)
+            log.debug("No code found for trying to execute a create type instruction.")
+            return [global_state]
+
+        code_str = bytes.hex(bytes(code_raw))
+
+        next_transaction_id = tx_id_manager.get_next_tx_id()
+        constructor_arguments = ConcreteCalldata(
+            next_transaction_id, call_data[code_end:]
+        )
+        code = Disassembly(code_str)
+
+        caller = environment.active_account.address
+        gas_price = environment.gasprice
+        origin = environment.origin
+
+        contract_address = None  # type: Union[BitVec, int]
+        Instruction._sha3_gas_helper(global_state, len(code_str[2:]) // 2)
+
+        if create2_salt:
+            if create2_salt.symbolic:
+                if create2_salt.size() != 256:
+                    pad = symbol_factory.BitVecVal(0, 256 - create2_salt.size())
+                    create2_salt = Concat(pad, create2_salt)
+                address = keccak_function_manager.create_keccak(
+                    Concat(
+                        symbol_factory.BitVecVal(255, 8),
+                        caller,
+                        create2_salt,
+                        symbol_factory.BitVecVal(int(get_code_hash(code_str), 16), 256),
+                    )
+                )
+                contract_address = Extract(255, 96, address)
+
+            else:
+                salt = hex(create2_salt.value)[2:]
+                salt = "0" * (64 - len(salt)) + salt
+
+                addr = hex(caller.value)[2:]
+                addr = "0" * (40 - len(addr)) + addr
+
+                contract_address = int(
+                    get_code_hash("0xff" + addr + salt + get_code_hash(code_str)[2:])[
+                        26:
+                    ],
+                    16,
+                )
+        transaction = ContractCreationTransaction(
+            world_state=world_state,
+            caller=caller,
+            code=code,
+            call_data=constructor_arguments,
+            gas_price=gas_price,
+            gas_limit=mstate.gas_limit,
+            origin=origin,
+            call_value=call_value,
+            contract_address=contract_address,
+        )
+        log.info("Raise transaction start signal")
+        raise TransactionStartSignal(transaction, self.op_code, global_state)
+
+    @StateTransition(is_state_mutation_instruction=True)
+    def create_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        call_value, mem_offset, mem_size = global_state.mstate.pop(3)
+        return self._create_transaction_helper(
+            global_state, call_value, mem_offset, mem_size
+        )
+
+    @StateTransition()
+    def create_post(self, global_state: GlobalState) -> List[GlobalState]:
+        return self._handle_create_type_post(global_state)
+
+    @StateTransition(is_state_mutation_instruction=True)
+    def create2_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        call_value, mem_offset, mem_size, salt = global_state.mstate.pop(4)
+
+        return self._create_transaction_helper(
+            global_state, call_value, mem_offset, mem_size, salt
+        )
+
+    @StateTransition()
+    def create2_post(self, global_state: GlobalState) -> List[GlobalState]:
+        return self._handle_create_type_post(global_state, opcode="create2")
+
+    @staticmethod
+    def _handle_create_type_post(global_state, opcode="create"):
+        if opcode == "create2":
+            global_state.mstate.pop(4)
+        else:
+            global_state.mstate.pop(3)
+        if global_state.last_return_data:
+            return_val = symbol_factory.BitVecVal(
+                int(global_state.last_return_data.return_data, 16), 256
+            )
+        else:
+            return_val = symbol_factory.BitVecVal(0, 256)
+        global_state.mstate.stack.append(return_val)
+        return [global_state]
+
+    @StateTransition()
+    def return_(self, global_state: GlobalState):
+        """
+
+        :param global_state:
+        """
+        state = global_state.mstate
+        offset, length = state.stack.pop(), state.stack.pop()
+        if length.symbolic:
+            return_data = [global_state.new_bitvec("return_data", 8)]
+            log.debug("Return with symbolic length or offset. Not supported")
+        else:
+            state.mem_extend(offset, length)
+            StateTransition.check_gas_usage_limit(global_state)
+            return_data = state.memory[offset : offset + length]
+        global_state.current_transaction.end(
+            global_state, ReturnData(return_data, length)
+        )
+
+    @StateTransition(is_state_mutation_instruction=True)
+    def selfdestruct_(self, global_state: GlobalState):
+        """
+
+        :param global_state:
+        """
+        target = global_state.mstate.stack.pop()
+        transfer_amount = global_state.environment.active_account.balance()
+        # Often the target of the selfdestruct instruction will be symbolic
+        # If it isn't then we'll transfer the balance to the indicated contract
+        global_state.world_state.balances[target] += transfer_amount
+
+        global_state.environment.active_account = deepcopy(
+            global_state.environment.active_account
+        )
+        global_state.accounts[
+            global_state.environment.active_account.address.value
+        ] = global_state.environment.active_account
+
+        global_state.environment.active_account.set_balance(0)
+        global_state.environment.active_account.deleted = True
+        global_state.current_transaction.end(global_state)
+
+    @StateTransition()
+    def revert_(self, global_state: GlobalState) -> None:
+        """
+
+        :param global_state:
+        """
+        state = global_state.mstate
+        offset, length = state.stack.pop(), state.stack.pop()
+        if length.symbolic is False:
+            return_data = [
+                global_state.new_bitvec(
+                    f"{global_state.current_transaction.id}_return_data_{i}", 8
+                )
+                for i in range(length.value)
+            ]
+        else:
+            return_data = [
+                If(
+                    i < length,
+                    global_state.new_bitvec(
+                        f"{global_state.current_transaction.id}_return_data_{i}", 8
+                    ),
+                    0,
+                )
+                for i in range(300)
+            ]
+
+        try:
+            return_data = state.memory[
+                util.get_concrete_int(offset) : util.get_concrete_int(offset + length)
+            ]
+        except TypeError:
+            log.debug("Return with symbolic length or offset. Not supported")
+        global_state.current_transaction.end(
+            global_state, return_data=ReturnData(return_data, length), revert=True
+        )
+
+    @StateTransition()
+    def assert_fail_(self, global_state: GlobalState):
+        """
+
+        :param global_state:
+        """
+        # 0xfe: designated invalid opcode
+        raise InvalidInstruction
+
+    @StateTransition()
+    def invalid_(self, global_state: GlobalState):
+        """
+
+        :param global_state:
+        """
+        raise InvalidInstruction
+
+    @StateTransition()
+    def stop_(self, global_state: GlobalState):
+        """
+
+        :param global_state:
+        """
+        global_state.current_transaction.end(global_state)
+
+    @staticmethod
+    def _write_symbolic_returndata(
+        global_state: GlobalState, memory_out_offset: BitVec, memory_out_size: BitVec
+    ):
+        """
+        Writes symbolic return-data into memory, The memory offset and size should be concrete
+        :param global_state:
+        :param memory_out_offset:
+        :param memory_out_size:
+        :return:
+        """
+        if memory_out_offset.symbolic is True or memory_out_size.symbolic is True:
+            return
+        return_data = []
+        return_data_size = global_state.new_bitvec("returndatasize", 256)
+
+        for i in range(memory_out_size.value):
+            data = global_state.new_bitvec(
+                "call_output_var({})_{}".format(
+                    simplify(memory_out_offset + i), global_state.mstate.pc
+                ),
+                8,
+            )
+            return_data.append(data)
+
+        global_state.mstate.mem_extend(memory_out_offset, memory_out_size)
+        for i in range(memory_out_size.value):
+            global_state.mstate.memory[memory_out_offset + i] = If(
+                i <= return_data_size,
+                return_data[i],
+                global_state.mstate.memory[memory_out_offset + i],
+            )
+
+        global_state.last_return_data = ReturnData(
+            return_data=return_data, return_data_size=return_data_size
+        )
+
+    @StateTransition()
+    def call_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        instr = global_state.get_current_instruction()
+        environment = global_state.environment
+
+        memory_out_size, memory_out_offset = global_state.mstate.stack[-7:-5]
+        try:
+            (
+                callee_address,
+                callee_account,
+                call_data,
+                value,
+                gas,
+                memory_out_offset,
+                memory_out_size,
+            ) = get_call_parameters(global_state, self.dynamic_loader, True)
+
+            if callee_account is not None and callee_account.code.bytecode == "":
+                log.debug("The call is related to ether transfer between accounts")
+                sender = environment.active_account.address
+                receiver = callee_account.address
+
+                transfer_ether(global_state, sender, receiver, value)
+                self._write_symbolic_returndata(
+                    global_state, memory_out_offset, memory_out_size
+                )
+
+                global_state.mstate.stack.append(
+                    global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+                )
+                return [global_state]
+
+        except ValueError as e:
+            log.debug(
+                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
+                    e
+                )
+            )
+            self._write_symbolic_returndata(
+                global_state, memory_out_offset, memory_out_size
+            )
+            # TODO: decide what to do in this case
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+            return [global_state]
+
+        if environment.static:
+            if isinstance(value, int) and value > 0:
+                raise WriteProtection(
+                    "Cannot call with non zero value in a static call"
+                )
+            if isinstance(value, BitVec):
+                if value.symbolic:
+                    global_state.world_state.constraints.append(
+                        value == symbol_factory.BitVecVal(0, 256)
+                    )
+                elif value.value > 0:
+                    raise WriteProtection(
+                        "Cannot call with non zero value in a static call"
+                    )
+
+        native_result = native_call(
+            global_state, callee_address, call_data, memory_out_offset, memory_out_size
+        )
+        if native_result:
+            return native_result
+        transaction = MessageCallTransaction(
+            world_state=global_state.world_state,
+            gas_price=environment.gasprice,
+            gas_limit=gas,
+            origin=environment.origin,
+            caller=environment.active_account.address,
+            callee_account=callee_account,
+            call_data=call_data,
+            call_value=value,
+            static=environment.static,
+        )
+        raise TransactionStartSignal(transaction, self.op_code, global_state)
+
+    @StateTransition()
+    def call_post(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+
+        return self.post_handler(global_state, function_name="call")
+
+    @StateTransition()
+    def callcode_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        instr = global_state.get_current_instruction()
+        environment = global_state.environment
+        memory_out_size, memory_out_offset = global_state.mstate.stack[-7:-5]
+        try:
+            (
+                callee_address,
+                callee_account,
+                call_data,
+                value,
+                gas,
+                _,
+                _,
+            ) = get_call_parameters(global_state, self.dynamic_loader, True)
+
+            if callee_account is not None and callee_account.code.bytecode == "":
+                log.debug("The call is related to ether transfer between accounts")
+                sender = global_state.environment.active_account.address
+                receiver = callee_account.address
+                transfer_ether(global_state, sender, receiver, value)
+                self._write_symbolic_returndata(
+                    global_state, memory_out_offset, memory_out_size
+                )
+
+                global_state.mstate.stack.append(
+                    global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+                )
+                return [global_state]
+
+        except ValueError as e:
+            log.debug(
+                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
+                    e
+                )
+            )
+            self._write_symbolic_returndata(
+                global_state, memory_out_offset, memory_out_size
+            )
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+            return [global_state]
+
+        native_result = native_call(
+            global_state, callee_address, call_data, memory_out_offset, memory_out_size
+        )
+        if native_result:
+            return native_result
+
+        transaction = MessageCallTransaction(
+            world_state=global_state.world_state,
+            gas_price=environment.gasprice,
+            gas_limit=gas,
+            origin=environment.origin,
+            code=callee_account.code,
+            caller=environment.address,
+            callee_account=environment.active_account,
+            call_data=call_data,
+            call_value=value,
+            static=environment.static,
+        )
+        raise TransactionStartSignal(transaction, self.op_code, global_state)
+
+    @StateTransition()
+    def callcode_post(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        instr = global_state.get_current_instruction()
+        memory_out_size, memory_out_offset = global_state.mstate.stack[-7:-5]
+        try:
+            (
+                _,
+                _,
+                _,
+                _,
+                _,
+                memory_out_offset,
+                memory_out_size,
+            ) = get_call_parameters(global_state, self.dynamic_loader, True)
+        except ValueError as e:
+            log.debug(
+                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
+                    e
+                )
+            )
+            self._write_symbolic_returndata(
+                global_state, memory_out_offset, memory_out_size
+            )
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+            return [global_state]
+
+        if global_state.last_return_data is None:
+            # Put return value on stack
+            return_value = global_state.new_bitvec(
+                "retval_" + str(instr["address"]), 256
+            )
+            global_state.mstate.stack.append(return_value)
+            self._write_symbolic_returndata(
+                global_state, memory_out_offset, memory_out_size
+            )
+            global_state.world_state.constraints.append(return_value == 0)
+            return [global_state]
+
+        try:
+            memory_out_offset = (
+                util.get_concrete_int(memory_out_offset)
+                if isinstance(memory_out_offset, Expression)
+                else memory_out_offset
+            )
+            memory_out_size = (
+                util.get_concrete_int(memory_out_size)
+                if isinstance(memory_out_size, Expression)
+                else memory_out_size
+            )
+        except TypeError:
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+            return [global_state]
+
+        # Copy memory
+        global_state.mstate.mem_extend(
+            memory_out_offset, min(memory_out_size, global_state.last_return_data.size)
+        )
+        if global_state.last_return_data.size.symbolic:
+            ret_size = 500
+        else:
+            ret_size = global_state.last_return_data.size.value
+        for i in range(min(memory_out_size, ret_size)):
+            global_state.mstate.memory[
+                i + memory_out_offset
+            ] = global_state.last_return_data[i]
+
+        # Put return value on stack
+        return_value = global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+        global_state.mstate.stack.append(return_value)
+        global_state.world_state.constraints.append(return_value == 1)
+        return [global_state]
+
+    @StateTransition()
+    def delegatecall_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        instr = global_state.get_current_instruction()
+        environment = global_state.environment
+        memory_out_size, memory_out_offset = global_state.mstate.stack[-6:-4]
+
+        try:
+            (
+                callee_address,
+                callee_account,
+                call_data,
+                value,
+                gas,
+                _,
+                _,
+            ) = get_call_parameters(global_state, self.dynamic_loader)
+
+            if callee_account is not None and callee_account.code.bytecode == "":
+                log.debug("The call is related to ether transfer between accounts")
+                sender = global_state.environment.active_account.address
+                receiver = callee_account.address
+
+                transfer_ether(global_state, sender, receiver, value)
+                self._write_symbolic_returndata(
+                    global_state, memory_out_offset, memory_out_size
+                )
+                global_state.mstate.stack.append(
+                    global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+                )
+                return [global_state]
+        except ValueError as e:
+            log.debug(
+                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
+                    e
+                )
+            )
+            self._write_symbolic_returndata(
+                global_state, memory_out_offset, memory_out_size
+            )
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+            return [global_state]
+
+        native_result = native_call(
+            global_state, callee_address, call_data, memory_out_offset, memory_out_size
+        )
+        if native_result:
+            return native_result
+
+        transaction = MessageCallTransaction(
+            world_state=global_state.world_state,
+            gas_price=environment.gasprice,
+            gas_limit=gas,
+            origin=environment.origin,
+            code=callee_account.code,
+            caller=environment.sender,
+            callee_account=environment.active_account,
+            call_data=call_data,
+            call_value=environment.callvalue,
+            static=environment.static,
+        )
+        raise TransactionStartSignal(transaction, self.op_code, global_state)
+
+    @StateTransition()
+    def delegatecall_post(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        instr = global_state.get_current_instruction()
+        memory_out_size, memory_out_offset = global_state.mstate.stack[-6:-4]
+
+        try:
+            (
+                _,
+                _,
+                _,
+                _,
+                _,
+                memory_out_offset,
+                memory_out_size,
+            ) = get_call_parameters(global_state, self.dynamic_loader)
+        except ValueError as e:
+            log.debug(
+                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
+                    e
+                )
+            )
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+            self._write_symbolic_returndata(
+                global_state, memory_out_offset, memory_out_size
+            )
+            return [global_state]
+
+        if global_state.last_return_data is None:
+            # Put return value on stack
+            return_value = global_state.new_bitvec(
+                "retval_" + str(instr["address"]), 256
+            )
+            global_state.mstate.stack.append(return_value)
+            global_state.world_state.constraints.append(return_value == 0)
+            return [global_state]
+
+        try:
+            memory_out_offset = (
+                util.get_concrete_int(memory_out_offset)
+                if isinstance(memory_out_offset, Expression)
+                else memory_out_offset
+            )
+            memory_out_size = (
+                util.get_concrete_int(memory_out_size)
+                if isinstance(memory_out_size, Expression)
+                else memory_out_size
+            )
+        except TypeError:
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+            return [global_state]
+
+            # Copy memory
+        global_state.mstate.mem_extend(
+            memory_out_offset, min(memory_out_size, global_state.last_return_data.size)
+        )
+        if global_state.last_return_data.size.symbolic:
+            ret_size = 500
+        else:
+            ret_size = global_state.last_return_data.size.value
+        for i in range(min(memory_out_size, ret_size)):
+            global_state.mstate.memory[
+                i + memory_out_offset
+            ] = global_state.last_return_data[i]
+
+        # Put return value on stack
+        return_value = global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+        global_state.mstate.stack.append(return_value)
+        global_state.world_state.constraints.append(return_value == 1)
+        return [global_state]
+
+    @StateTransition()
+    def staticcall_(self, global_state: GlobalState) -> List[GlobalState]:
+        """
+
+        :param global_state:
+        :return:
+        """
+        instr = global_state.get_current_instruction()
+        environment = global_state.environment
+        memory_out_size, memory_out_offset = global_state.mstate.stack[-6:-4]
+        try:
+            (
+                callee_address,
+                callee_account,
+                call_data,
+                value,
+                gas,
+                memory_out_offset,
+                memory_out_size,
+            ) = get_call_parameters(global_state, self.dynamic_loader)
+
+            if callee_account is not None and callee_account.code.bytecode == "":
+                log.debug("The call is related to ether transfer between accounts")
+                sender = environment.active_account.address
+                receiver = callee_account.address
+                transfer_ether(global_state, sender, receiver, value)
+                self._write_symbolic_returndata(
+                    global_state, memory_out_offset, memory_out_size
+                )
+                global_state.mstate.stack.append(
+                    global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+                )
+
+                return [global_state]
+
+        except ValueError as e:
+            log.debug(
+                "Could not determine required parameters for call, putting fresh symbol on the stack. \n{}".format(
+                    e
+                )
+            )
+            self._write_symbolic_returndata(
+                global_state, memory_out_offset, memory_out_size
+            )
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+
+            return [global_state]
+
+        native_result = native_call(
+            global_state, callee_address, call_data, memory_out_offset, memory_out_size
+        )
+
+        if native_result:
+            return native_result
+
+        transaction = MessageCallTransaction(
+            world_state=global_state.world_state,
+            gas_price=environment.gasprice,
+            gas_limit=gas,
+            origin=environment.origin,
+            code=callee_account.code,
+            caller=environment.address,
+            callee_account=callee_account,
+            call_data=call_data,
+            call_value=value,
+            static=True,
+        )
+        raise TransactionStartSignal(transaction, self.op_code, global_state)
+
+    @StateTransition()
+    def staticcall_post(self, global_state: GlobalState) -> List[GlobalState]:
+        return self.post_handler(global_state, function_name="staticcall")
+
+    def post_handler(self, global_state, function_name: str):
+        instr = global_state.get_current_instruction()
+        if function_name in ("staticcall", "delegatecall"):
+            memory_out_size, memory_out_offset = global_state.mstate.stack[-6:-4]
+        else:
+            memory_out_size, memory_out_offset = global_state.mstate.stack[-7:-5]
+
+        try:
+            with_value = function_name != "staticcall"
+            (
+                _,
+                _,
+                _,
+                _,
+                _,
+                memory_out_offset,
+                memory_out_size,
+            ) = get_call_parameters(global_state, self.dynamic_loader, with_value)
+        except ValueError as e:
+            log.debug(
+                "Could not determine required parameters for {}, putting fresh symbol on the stack. \n{}".format(
+                    function_name, e
+                )
+            )
+            self._write_symbolic_returndata(
+                global_state, memory_out_offset, memory_out_size
+            )
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+            return [global_state]
+
+        if global_state.last_return_data is None:
+            # Put return value on stack
+            return_value = global_state.new_bitvec(
+                "retval_" + str(instr["address"]), 256
+            )
+            global_state.mstate.stack.append(return_value)
+            return [global_state]
+
+        try:
+            memory_out_offset = (
+                util.get_concrete_int(memory_out_offset)
+                if isinstance(memory_out_offset, Expression)
+                else memory_out_offset
+            )
+            memory_out_size = (
+                util.get_concrete_int(memory_out_size)
+                if isinstance(memory_out_size, Expression)
+                else memory_out_size
+            )
+        except TypeError:
+            global_state.mstate.stack.append(
+                global_state.new_bitvec("retval_" + str(instr["address"]), 256)
+            )
+            return [global_state]
+
+        global_state.mstate.mem_extend(
+            memory_out_offset, min(memory_out_size, global_state.last_return_data.size)
+        )
+        if global_state.last_return_data.size.symbolic:
+            ret_size = 500
+        else:
+            ret_size = global_state.last_return_data.size.value
+
+        for i in range(min(memory_out_size, ret_size)):
+            global_state.mstate.memory[
+                i + memory_out_offset
+            ] = global_state.last_return_data[i]
+
+        # Put return value on stack
+        return_value = global_state.new_bitvec(
+            "retval_" + str(global_state.get_current_instruction()["address"]), 256
+        )
+        global_state.mstate.stack.append(return_value)
+        global_state.world_state.constraints.append(return_value == 1)
+
+        return [global_state]
```

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/natives.py` & `smartExecutorx-4.1/mythril/laser/ethereum/natives.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/account.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/account.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/annotation.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/annotation.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/calldata.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/calldata.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/constraints.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/constraints.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/environment.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/environment.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/global_state.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/global_state.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/machine_state.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/machine_state.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/memory.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/memory.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/return_data.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/return_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/state/world_state.py` & `smartExecutorx-4.1/mythril/laser/ethereum/state/world_state.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/__init__.py` & `smartExecutorx-4.1/mythril/laser/ethereum/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/basic.py` & `smartExecutorx-4.1/mythril/laser/ethereum/strategy/basic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/beam.py` & `smartExecutorx-4.1/mythril/laser/ethereum/strategy/beam.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/concolic.py` & `smartExecutorx-4.1/mythril/laser/ethereum/strategy/concolic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/constraint_strategy.py` & `smartExecutorx-4.1/mythril/laser/ethereum/strategy/constraint_strategy.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/strategy/extensions/bounded_loops.py` & `smartExecutorx-4.1/mythril/laser/ethereum/strategy/extensions/bounded_loops.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/svm.py` & `smartExecutorx-4.1/mythril/laser/ethereum/svm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1072 +1,1073 @@
-"""This module implements the main symbolic execution engine."""
-import logging
-from collections import defaultdict
-from copy import copy, deepcopy
-from datetime import datetime, timedelta
-import random
-from typing import Callable, Dict, DefaultDict, List, Tuple, Optional
-
-from mythril.support.opcodes import OPCODES
-from mythril.analysis.potential_issues import check_potential_issues
-from mythril.laser.execution_info import ExecutionInfo
-from mythril.laser.ethereum.cfg import NodeFlags, Node, Edge, JumpType
-from mythril.laser.ethereum.evm_exceptions import StackUnderflowException, VmException
-from mythril.laser.ethereum.instructions import Instruction
-from mythril.laser.ethereum.instruction_data import get_required_stack_elements
-from mythril.laser.plugin.signals import PluginSkipWorldState, PluginSkipState
-from mythril.laser.ethereum.state.global_state import GlobalState
-from mythril.laser.ethereum.state.world_state import WorldState
-from mythril.laser.ethereum.strategy.basic import DepthFirstSearchStrategy
-from mythril.laser.ethereum.strategy.constraint_strategy import DelayConstraintStrategy
-from abc import ABCMeta
-from mythril.laser.ethereum.time_handler import time_handler
-
-from mythril.laser.ethereum.transaction import (
-    ContractCreationTransaction,
-    TransactionEndSignal,
-    TransactionStartSignal,
-    execute_contract_creation,
-    execute_message_call,
-)
-from mythril.laser.smt import symbol_factory
-from mythril.support.support_args import args
-import fdg
-
-from fdg.preprocessing.preprocess import execute_preprocessing
-log = logging.getLogger(__name__)
-
-
-class SVMError(Exception):
-    """An exception denoting an unexpected state in symbolic execution."""
-
-    pass
-
-
-class LaserEVM:
-    """The LASER EVM.
-
-    Just as Mithril had to be mined at great efforts to provide the
-    Dwarves with their exceptional armour, LASER stands at the heart of
-    Mythril, digging deep in the depths of call graphs, unearthing the
-    most precious symbolic call data, that is then hand-forged into
-    beautiful and strong security issues by the experienced smiths we
-    call detection modules. It is truly a magnificent symbiosis.
-    """
-
-    def __init__(
-        self,
-        dynamic_loader=None,
-        max_depth=float("inf"),
-        execution_timeout=60,
-        create_timeout=10,
-        strategy=DepthFirstSearchStrategy,
-        transaction_count=2,
-        requires_statespace=True,
-        iprof=None,
-        use_reachability_check=True,
-        beam_width=None,
-    ) -> None:
-        """
-        Initializes the laser evm object
-
-        :param dynamic_loader: Loads data from chain
-        :param max_depth: Maximum execution depth this vm should execute
-        :param execution_timeout: Time to take for execution
-        :param create_timeout: Time to take for contract creation
-        :param strategy: Execution search strategy
-        :param transaction_count: The amount of transactions to execute
-        :param requires_statespace: Variable indicating whether the statespace should be recorded
-        :param iprof: Instruction Profiler
-        """
-        self.execution_info: List[ExecutionInfo] = []
-
-        self.open_states: List[WorldState] = []
-        self.total_states = 0
-        self.dynamic_loader = dynamic_loader
-        self.use_reachability_check = use_reachability_check
-
-        self.work_list: List[GlobalState] = []
-        self.strategy = strategy(self.work_list, max_depth, beam_width=beam_width)
-        self.max_depth = max_depth
-        self.transaction_count = transaction_count
-
-        self.execution_timeout = execution_timeout or 0
-        self.create_timeout = create_timeout or 0
-
-        self.requires_statespace = requires_statespace
-        if self.requires_statespace:
-            self.nodes: Dict[int, Node] = {}
-            self.edges: List[Edge] = []
-
-        self.time: datetime = None
-        self.executed_transactions: bool = False
-
-        self.pre_hooks: DefaultDict[str, List[Callable]] = defaultdict(list)
-        self.post_hooks: DefaultDict[str, List[Callable]] = defaultdict(list)
-
-        self._add_world_state_hooks: List[Callable] = []
-        self._execute_state_hooks: List[Callable] = []
-
-        self._start_exec_trans_hooks: List[Callable] = []
-        self._stop_exec_trans_hooks: List[Callable] = []
-
-        self._start_sym_trans_hooks: List[Callable] = []
-        self._stop_sym_trans_hooks: List[Callable] = []
-
-        self._start_sym_exec_hooks: List[Callable] = []
-        self._stop_sym_exec_hooks: List[Callable] = []
-
-        self._start_exec_hooks: List[Callable] = []
-        self._stop_exec_hooks: List[Callable] = []
-
-        self._transaction_end_hooks: List[Callable] = []
-
-        self.iprof = iprof
-        self.instr_pre_hook: Dict[str, List[Callable]] = {}
-        self.instr_post_hook: Dict[str, List[Callable]] = {}
-
-        self._start_sym_trans_hooks_laserEVM=[] #@wei
-        self._stop_sym_trans_hooks_laserEVM = []  # @wei
-        self._branch_check_hooks = []  # @wei
-        self.preprocessing_pre_hooks = defaultdict(list)  # @wei
-        self._pre_execute_state_hooks = []  # type:List[Callable]#@wei
-        self._post_execute_state_hooks = []  # type:List[Callable] #@wei
-        self._preprocessing_execute_state_hooks = []
-        for op in OPCODES:
-            self.instr_pre_hook[op] = []
-            self.instr_post_hook[op] = []
-        self.hook_type_map = {
-            "start_execute_transactions": self._start_exec_trans_hooks,
-            "stop_execute_transactions": self._stop_exec_trans_hooks,
-            "add_world_state": self._add_world_state_hooks,
-            "execute_state": self._execute_state_hooks,
-            "start_sym_exec": self._start_sym_exec_hooks,
-            "stop_sym_exec": self._stop_sym_exec_hooks,
-            "start_sym_trans": self._start_sym_trans_hooks,
-            "stop_sym_trans": self._stop_sym_trans_hooks,
-            "start_exec": self._start_exec_hooks,
-            "stop_exec": self._stop_exec_hooks,
-            "transaction_end": self._transaction_end_hooks,
-            'pre_execute_state':self._pre_execute_state_hooks,#@wei
-            'post_execute_state':self._post_execute_state_hooks,#@wei
-            'branch_check':self._branch_check_hooks,#@wei
-            'preprocessing_execute_state':self._preprocessing_execute_state_hooks,#@wei
-            'start_sym_trans_laserEVM':self._start_sym_trans_hooks_laserEVM,#@wei
-            'stop_sym_trans_laserEVM':self._stop_sym_trans_hooks_laserEVM,#@wei
-        }
-        log.info("LASER EVM initialized with dynamic loader: " + str(dynamic_loader))
-
-
-    def extend_strategy(self, extension: ABCMeta, **kwargs) -> None:
-        self.strategy = extension(self.strategy, **kwargs)
-
-    def sym_exec(
-        self,
-        world_state: WorldState = None,
-        target_address: int = None,
-        creation_code: str = None,
-        contract_name: str = None,
-    ) -> None:
-        """Starts symbolic execution
-        There are two modes of execution.
-        Either we analyze a preconfigured configuration, in which case the world_state and target_address variables
-        must be supplied.
-        Or we execute the creation code of a contract, in which case the creation code and desired name of that
-        contract should be provided.
-
-        :param world_state The world state configuration from which to perform analysis
-        :param target_address The address of the contract account in the world state which analysis should target
-        :param creation_code The creation code to create the target contract in the symbolic environment
-        :param contract_name The name that the created account should be associated with
-        """
-        pre_configuration_mode = target_address is not None
-        scratch_mode = creation_code is not None and contract_name is not None
-        if pre_configuration_mode == scratch_mode:
-            raise ValueError("Symbolic execution started with invalid parameters")
-
-        log.debug("Starting LASER execution")
-        for hook in self._start_sym_exec_hooks:
-            hook()
-
-        time_handler.start_execution(self.execution_timeout)
-        self.time = datetime.now()
-
-        if pre_configuration_mode:
-            self.open_states = [world_state]
-            log.info("Starting message call transaction to {}".format(target_address))
-            self.execute_transactions(symbol_factory.BitVecVal(target_address, 256))
-
-        elif scratch_mode:
-            log.info("Starting contract creation transaction")
-
-            created_account = execute_contract_creation(
-                self, creation_code, contract_name, world_state=world_state
-            )
-            fdg.global_config.contract_address = created_account.address
-
-            log.info(
-                "Finished contract creation, found {} open states".format(
-                    len(self.open_states)
-                )
-            )
-
-            if len(self.open_states) == 0:
-                log.warning(
-                    "No contract was created during the execution of contract creation "
-                    "Increase the resources for creation execution (--max-depth or --create-timeout) "
-                    "Check whether the bytecode is indeed the creation code, otherwise use the --bin-runtime flag"
-                )
-
-            # if fdg.global_config.flag_fwrg:
-            #     self._execute_transactions_fdg(created_account.address)
-            # else:
-            #     self._execute_transactions(created_account.address)
-            self.execute_transactions(created_account.address)
-        log.info("Finished symbolic execution")
-        if self.requires_statespace:
-            log.info(
-                "%d nodes, %d edges, %d total states",
-                len(self.nodes),
-                len(self.edges),
-                self.total_states,
-            )
-            print(f'#@statespace')
-            print("{} nodes, {} edges, {} total states".format(len(self.nodes), len(self.edges), self.total_states))
-        for hook in self._stop_sym_exec_hooks:
-            hook()
-
-    def execute_transactions(self, address) -> None:
-        """This function helps runs plugins that can order transactions.
-        Such plugins should set self.executed_transactions as True after its execution
-
-        :param address: Address of the contract
-        :return: None
-        """
-        for hook in self._start_exec_trans_hooks:
-            hook()
-
-        if self.executed_transactions is False:
-            if fdg.global_config.flag_fwrg:
-                self._execute_transactions_fdg(address)
-            else:
-                self._execute_transactions(address)
-            # self._execute_transactions(address)
-
-        for hook in self._stop_exec_trans_hooks:
-            hook()
-
-    def _execute_transactions(self, address):
-        """This function executes multiple transactions on the address
-
-        :param address: Address of the contract
-        :return:
-        """
-        self.time = datetime.now()
-
-        for i in range(self.transaction_count):
-            if len(self.open_states) == 0:
-                break
-            old_states_count = len(self.open_states)
-
-            if self.use_reachability_check:
-                log.info("do reachability check")
-                self.open_states = [
-                    state
-                    for state in self.open_states
-                    if state.constraints.is_possible()
-                ]
-                prune_count = old_states_count - len(self.open_states)
-                if prune_count:
-                    log.info("Pruned {} unreachable states".format(prune_count))
-            log.info(
-                "Starting message call transaction, iteration: {}, {} initial states".format(
-                    i, len(self.open_states)
-                )
-            )
-            func_hashes = (
-                args.transaction_sequences[i] if args.transaction_sequences else None
-            )
-
-            if func_hashes:
-                for itr, func_hash in enumerate(func_hashes):
-                    if func_hash in (-1, -2):
-                        func_hashes[itr] = func_hash
-                    else:
-                        func_hashes[itr] = bytes.fromhex(hex(func_hash)[2:].zfill(8))
-
-            for hook in self._start_sym_trans_hooks:
-                hook()
-
-            execute_message_call(self, address, func_hashes=func_hashes)
-
-            for hook in self._stop_sym_trans_hooks:
-                hook()
-
-        self.executed_transactions = True
-
-    def _execute_transactions_fdg(self, address):
-        """This function executes multiple transactions on the address
-
-        :param address: Address of the contract
-        :return:
-        """
-        self.time = datetime.now()
-        i = 0
-        while i < fdg.global_config.transaction_count:  # @wei rewrite loop
-            if fdg.global_config.random_baseline == 0:
-                if i == 0:
-                    copy_laserEVM = deepcopy(self)
-                    copy_laserEVM.requires_statespace=False
-                    copy_laserEVM.post_hooks={}
-                    copy_laserEVM.pre_hooks={}
-                    execute_preprocessing(address, copy_laserEVM)
-                    i += 1
-                    continue
-
-            log.info(
-                "Starting message call transaction, iteration: {}, {} initial states".format(
-                    i, len(self.open_states)
-                )
-            )
-            for hook in self._start_sym_trans_hooks:
-                hook()
-            for hook in self._start_sym_trans_hooks_laserEVM:
-                hook(self)
-
-            execute_message_call(self, address)
-
-            for hook in self._stop_sym_trans_hooks:
-                hook()
-
-            for hook in self._stop_sym_trans_hooks_laserEVM:
-                hook(self)
-            i += 1
-
-    def _check_create_termination(self) -> bool:
-        if len(self.open_states) != 0:
-            return (
-                self.create_timeout > 0
-                and self.time + timedelta(seconds=self.create_timeout) <= datetime.now()
-            )
-        return self._check_execution_termination()
-
-    def _check_execution_termination(self) -> bool:
-        return (
-            self.execution_timeout > 0
-            and self.time + timedelta(seconds=self.execution_timeout) <= datetime.now()
-        )
-
-        # @wei
-
-    def _check_preprocessing_termination(self) -> bool:
-
-        return self.time + timedelta(seconds=fdg.global_config.preprocess_timeout) <= datetime.now()
-
-        # @wei
-
-    def _check_preprocessing_error(self) -> bool:
-        return fdg.global_config.preprocessing_exception
-
-
-    # @wei adopt from exec()
-    def exec_preprocessing(self):
-        """
-                :param create:
-                :param track_gas:
-                :return:
-        """
-        for global_state in self.strategy:
-            # @wei througth timeout
-            if self._check_preprocessing_termination():
-                log.debug("hit the exec_preprocessing excution time, return.")
-                print("hit the exec_preprocessing excution time, return.")
-                fdg.global_config.flag_preprocess_timeout = True
-                return None
-            # @wei check errors in preprocessing
-            if self._check_preprocessing_error():
-                log.debug("have exceptions in preprocessing.")
-                print("have exceptions in preprocessing.")
-                return None
-
-            try:
-                new_states, op_code = self.execute_state_preprocessing(global_state)
-
-            except NotImplementedError:
-                log.debug("Encountered unimplemented instruction")
-                continue
-
-            # should be kept otherwise, active function information can not be obtained.
-            self.manage_cfg(op_code, new_states)  # TODO: What about op_code is None?
-            if new_states:
-                self.work_list += new_states
-
-        return None
-
-    # @wei
-    def _execute_preprocessing_pre_hook(self, op_code: str, global_state):
-        if op_code not in self.preprocessing_pre_hooks.keys():
-            return
-        for hook in self.preprocessing_pre_hooks[op_code]:
-            hook(global_state)
-
-    # @wei
-    def execute_state_preprocessing(
-        self, global_state: GlobalState
-    ) -> Tuple[List[GlobalState], Optional[str]]:
-        """Execute a single instruction in global_state.
-
-        :param global_state:
-        :return: A list of successor states.
-        """
-
-        instructions = global_state.environment.code.instruction_list
-
-        try:
-            op_code = instructions[global_state.mstate.pc]["opcode"]
-            # Execute hooks
-            for hook in self._preprocessing_execute_state_hooks:
-                hook(global_state, op_code)
-
-            # if global_state.environment.active_function_name in ['getBalance(address,address)']:
-            #     print(f'{global_state.environment.active_function_name}:{instructions[global_state.mstate.pc]}')
-
-        except IndexError:
-            # self._add_world_state(global_state)
-            return [], None
-
-        if len(global_state.mstate.stack) < get_required_stack_elements(op_code):
-            error_msg = (
-                "Stack Underflow Exception due to insufficient "
-                "stack elements for the address {}".format(
-                    instructions[global_state.mstate.pc]["address"]
-                )
-            )
-            new_global_states = self.handle_vm_exception(
-                global_state, op_code, error_msg
-            )
-            # self._execute_post_hook(op_code, new_global_states)
-            return new_global_states, op_code
-
-        try:
-            self._execute_preprocessing_pre_hook(op_code, global_state)
-        except PluginSkipState:
-            return [], None
-
-        try:
-            new_global_states = Instruction(
-                op_code,
-                self.dynamic_loader,
-                pre_hooks=[],
-                post_hooks=[],
-            ).evaluate(global_state)
-
-        except VmException as e:
-            # for hook in self._transaction_end_hooks:
-            #     hook(
-            #         global_state,
-            #         global_state.current_transaction,
-            #         None,
-            #         False,
-            #     )
-            new_global_states = self.handle_vm_exception(global_state, op_code, str(e))
-
-        except TransactionStartSignal as start_signal:
-            # Setup new global state
-            new_global_state = start_signal.transaction.initial_global_state()
-
-            new_global_state.transaction_stack = copy(
-                global_state.transaction_stack
-            ) + [(start_signal.transaction, global_state)]
-            new_global_state.node = global_state.node
-            new_global_state.world_state.constraints = (
-                start_signal.global_state.world_state.constraints
-            )
-
-            log.debug("Starting new transaction %s", start_signal.transaction)
-
-            return [new_global_state], op_code
-
-        except TransactionEndSignal as end_signal:
-            (
-                transaction,
-                return_global_state,
-            ) = end_signal.global_state.transaction_stack[-1]
-
-            log.debug("Ending transaction %s.", transaction)
-
-            # for hook in self._transaction_end_hooks:
-            #     hook(
-            #         end_signal.global_state,
-            #         transaction,
-            #         return_global_state,
-            #         end_signal.revert,
-            #     )
-
-            if return_global_state is None:
-                # if (
-                #     not isinstance(transaction, ContractCreationTransaction)
-                #     or transaction.return_data
-                # ) and not end_signal.revert:
-                #     check_potential_issues(global_state)
-                #     end_signal.global_state.world_state.node = global_state.node
-                #     self._add_world_state(end_signal.global_state)
-
-                new_global_states = []
-            else:
-
-                # # First execute the post hook for the transaction ending instruction
-                # self._execute_post_hook(op_code, [end_signal.global_state])
-
-                # Propagate annotations
-                new_annotations = [
-                    annotation
-                    for annotation in global_state.annotations
-                    if annotation.persist_over_calls
-                ]
-                return_global_state.add_annotations(new_annotations)
-
-                new_global_states = self._end_message_call(
-                    copy(return_global_state),
-                    global_state,
-                    revert_changes=False or end_signal.revert,
-                    return_data=transaction.return_data,
-                )
-
-        # self._execute_post_hook(op_code, new_global_states)
-
-        return new_global_states, op_code
-
-
-
-    def exec(self, create=False, track_gas=False) -> Optional[List[GlobalState]]:
-        """
-
-        :param create:
-        :param track_gas:
-        :return:
-        """
-        final_states = []  # type: List[GlobalState]
-        for hook in self._start_exec_hooks:
-            hook()
-
-        for global_state in self.strategy:
-
-            if create and self._check_create_termination():
-                log.debug("Hit create timeout, returning.")
-                return final_states + [global_state] if track_gas else None
-
-            if not create and self._check_execution_termination():
-                log.debug("Hit execution timeout, returning.")
-                return final_states + [global_state] if track_gas else None
-            try:
-
-                new_states, op_code = self.execute_state(global_state)
-
-            except NotImplementedError:
-                log.debug("Encountered unimplemented instruction")
-                continue
-
-            if self.strategy.run_check() and (
-                len(new_states) > 1 and random.uniform(0, 1) < args.pruning_factor
-            ): # need to be careful: previous version:if args.sparse_pruning is False:
-
-                new_states = [
-                    state
-                    for state in new_states
-                    if state.world_state.constraints.is_possible()
-                ]
-
-
-
-            self.manage_cfg(op_code, new_states)  # TODO: What about op_code is None?
-            if new_states:
-                self.work_list += new_states
-            elif track_gas:
-                final_states.append(global_state)
-            self.total_states += len(new_states)
-
-        # need to be careful as this does not appear in previous version
-        for hook in self._stop_exec_hooks:
-            hook()
-
-        return final_states if track_gas else None
-
-    def _add_world_state(self, global_state: GlobalState):
-        """Stores the world_state of the passed global state in the open states"""
-
-        for hook in self._add_world_state_hooks:
-            try:
-                hook(global_state)
-            except PluginSkipWorldState:
-                return
-
-        self.open_states.append(global_state.world_state)
-
-    def handle_vm_exception(
-        self, global_state: GlobalState, op_code: str, error_msg: str
-    ) -> List[GlobalState]:
-        _, return_global_state = global_state.transaction_stack.pop()
-
-        if return_global_state is None:
-            # In this case we don't put an unmodified world state in the open_states list Since in the case of an
-            #  exceptional halt all changes should be discarded, and this world state would not provide us with a
-            #  previously unseen world state
-            log.debug("Encountered a VmException, ending path: `{}`".format(error_msg))
-            new_global_states = []  # type: List[GlobalState]
-        else:
-            # First execute the post hook for the transaction ending instruction
-            self._execute_post_hook(op_code, [global_state])
-            new_global_states = self._end_message_call(
-                return_global_state, global_state, revert_changes=True, return_data=None
-            )
-        return new_global_states
-
-    def execute_state(
-        self, global_state: GlobalState
-    ) -> Tuple[List[GlobalState], Optional[str]]:
-        """Execute a single instruction in global_state.
-
-        :param global_state:
-        :return: A list of successor states.
-        """
-        # Execute hooks
-        try:
-            for hook in self._execute_state_hooks:
-                hook(global_state)
-        except PluginSkipState:
-            return [], None
-
-        instructions = global_state.environment.code.instruction_list
-
-        try:
-            op_code = instructions[global_state.mstate.pc]["opcode"]
-            # if global_state.environment.active_function_name in ['getBalance(address,address)']:
-            #     print(f'{global_state.environment.active_function_name}:{instructions[global_state.mstate.pc]}')
-
-        except IndexError:
-            self._add_world_state(global_state)
-            return [], None
-
-        if len(global_state.mstate.stack) < get_required_stack_elements(op_code):
-            error_msg = (
-                "Stack Underflow Exception due to insufficient "
-                "stack elements for the address {}".format(
-                    instructions[global_state.mstate.pc]["address"]
-                )
-            )
-            new_global_states = self.handle_vm_exception(
-                global_state, op_code, error_msg
-            )
-            self._execute_post_hook(op_code, new_global_states)
-            return new_global_states, op_code
-
-        try:
-            self._execute_pre_hook(op_code, global_state)
-        except PluginSkipState:
-            return [], None
-
-        try:
-            new_global_states = Instruction(
-                op_code,
-                self.dynamic_loader,
-                pre_hooks=self.instr_pre_hook[op_code],
-                post_hooks=self.instr_post_hook[op_code],
-            ).evaluate(global_state)
-
-        except VmException as e:
-            for hook in self._transaction_end_hooks:
-                hook(
-                    global_state,
-                    global_state.current_transaction,
-                    None,
-                    False,
-                )
-            new_global_states = self.handle_vm_exception(global_state, op_code, str(e))
-
-        except TransactionStartSignal as start_signal:
-            # Setup new global state
-            new_global_state = start_signal.transaction.initial_global_state()
-
-            new_global_state.transaction_stack = copy(
-                global_state.transaction_stack
-            ) + [(start_signal.transaction, global_state)]
-            new_global_state.node = global_state.node
-            new_global_state.world_state.constraints = (
-                start_signal.global_state.world_state.constraints
-            )
-
-            log.debug("Starting new transaction %s", start_signal.transaction)
-
-            return [new_global_state], op_code
-
-        except TransactionEndSignal as end_signal:
-            (
-                transaction,
-                return_global_state,
-            ) = end_signal.global_state.transaction_stack[-1]
-
-            log.debug("Ending transaction %s.", transaction)
-
-            for hook in self._transaction_end_hooks:
-                hook(
-                    end_signal.global_state,
-                    transaction,
-                    return_global_state,
-                    end_signal.revert,
-                )
-
-            if return_global_state is None:
-                if (
-                    not isinstance(transaction, ContractCreationTransaction)
-                    or transaction.return_data
-                ) and not end_signal.revert:
-                    check_potential_issues(global_state)
-                    end_signal.global_state.world_state.node = global_state.node
-                    self._add_world_state(end_signal.global_state)
-
-                new_global_states = []
-            else:
-
-                # First execute the post hook for the transaction ending instruction
-                self._execute_post_hook(op_code, [end_signal.global_state])
-
-                # Propagate annotations
-                new_annotations = [
-                    annotation
-                    for annotation in global_state.annotations
-                    if annotation.persist_over_calls
-                ]
-                return_global_state.add_annotations(new_annotations)
-
-                new_global_states = self._end_message_call(
-                    copy(return_global_state),
-                    global_state,
-                    revert_changes=False or end_signal.revert,
-                    return_data=transaction.return_data,
-                )
-
-        self._execute_post_hook(op_code, new_global_states)
-
-        return new_global_states, op_code
-
-    def _end_message_call(
-        self,
-        return_global_state: GlobalState,
-        global_state: GlobalState,
-        revert_changes=False,
-        return_data=None,
-    ) -> List[GlobalState]:
-        """
-
-        :param return_global_state:
-        :param global_state:
-        :param revert_changes:
-        :param return_data:
-        :return:
-        """
-
-        return_global_state.world_state.constraints += (
-            global_state.world_state.constraints
-        )
-        # Resume execution of the transaction initializing instruction
-        op_code = return_global_state.environment.code.instruction_list[
-            return_global_state.mstate.pc
-        ]["opcode"]
-
-        # Set execution result in the return_state
-        return_global_state.last_return_data = return_data
-        if not revert_changes:
-            return_global_state.world_state = copy(global_state.world_state)
-            return_global_state.environment.active_account = global_state.accounts[
-                return_global_state.environment.active_account.address.value
-            ]
-            if isinstance(
-                global_state.current_transaction, ContractCreationTransaction
-            ):
-                return_global_state.mstate.min_gas_used += (
-                    global_state.mstate.min_gas_used
-                )
-                return_global_state.mstate.max_gas_used += (
-                    global_state.mstate.max_gas_used
-                )
-        try:
-            # Execute the post instruction handler
-            new_global_states = Instruction(
-                op_code,
-                self.dynamic_loader,
-                pre_hooks=self.instr_pre_hook[op_code],
-                post_hooks=self.instr_post_hook[op_code],
-            ).evaluate(return_global_state, True)
-        except VmException:
-            new_global_states = []
-        # In order to get a nice call graph we need to set the nodes here
-        for state in new_global_states:
-            state.node = global_state.node
-
-        return new_global_states
-
-    def manage_cfg(self, opcode: str, new_states: List[GlobalState]) -> None:
-        """
-
-        :param opcode:
-        :param new_states:
-        """
-        if opcode == "JUMP":
-            assert len(new_states) <= 1
-            for state in new_states:
-                self._new_node_state(state)
-        elif opcode == "JUMPI":
-            assert len(new_states) <= 2
-            for state in new_states:
-                self._new_node_state(
-                    state, JumpType.CONDITIONAL, state.world_state.constraints[-1]
-                )
-        elif opcode in ("SLOAD", "SSTORE") and len(new_states) > 1:
-            for state in new_states:
-                self._new_node_state(
-                    state, JumpType.CONDITIONAL, state.world_state.constraints[-1]
-                )
-        elif opcode == "RETURN":
-            for state in new_states:
-                self._new_node_state(state, JumpType.RETURN)
-
-        for state in new_states:
-            # state.node.states.append(state)
-            # @wei
-            if state.mstate.pc >= len(state.environment.code.instruction_list):
-                print(
-                    f'self.mstate.pc:{state.mstate.pc}; len(instructions):{len(state.environment.code.instruction_list)}')
-            else:
-                state.node.states.append(state)
-    def _new_node_state(
-        self, state: GlobalState, edge_type=JumpType.UNCONDITIONAL, condition=None
-    ) -> None:
-        """
-
-        :param state:
-        :param edge_type:
-        :param condition:
-        """
-        try:
-            address = state.environment.code.instruction_list[state.mstate.pc][
-                "address"
-            ]
-        except IndexError:
-            return
-        new_node = Node(state.environment.active_account.contract_name)
-        old_node = state.node
-        state.node = new_node
-        new_node.constraints = state.world_state.constraints
-        if self.requires_statespace:
-            self.nodes[new_node.uid] = new_node
-            self.edges.append(
-                Edge(
-                    old_node.uid, new_node.uid, edge_type=edge_type, condition=condition
-                )
-            )
-
-        if edge_type == JumpType.RETURN:
-            new_node.flags |= NodeFlags.CALL_RETURN
-        elif edge_type == JumpType.CALL:
-            try:
-                if "retval" in str(state.mstate.stack[-1]):
-                    new_node.flags |= NodeFlags.CALL_RETURN
-                else:
-                    new_node.flags |= NodeFlags.FUNC_ENTRY
-            except StackUnderflowException:
-                new_node.flags |= NodeFlags.FUNC_ENTRY
-
-        environment = state.environment
-        disassembly = environment.code
-        if isinstance(
-            state.world_state.transaction_sequence[-1], ContractCreationTransaction
-        ):
-            environment.active_function_name = "constructor"
-        elif address in disassembly.address_to_function_name:
-            # Enter a new function
-            environment.active_function_name = disassembly.address_to_function_name[
-                address
-            ]
-            new_node.flags |= NodeFlags.FUNC_ENTRY
-
-            log.debug(
-                "- Entering function "
-                + environment.active_account.contract_name
-                + ":"
-                + new_node.function_name
-            )
-        elif address == 0:
-            environment.active_function_name = "fallback"
-
-        new_node.function_name = environment.active_function_name
-
-    def register_hooks(self, hook_type: str, hook_dict: Dict[str, List[Callable]]):
-        """
-
-        :param hook_type:
-        :param hook_dict:
-        """
-        if hook_type == "pre":
-            entrypoint = self.pre_hooks
-        elif hook_type == "post":
-            entrypoint = self.post_hooks
-        elif hook_type=='preprocessing_pre': #@wei
-            entrypoint=self.preprocessing_pre_hooks
-        else:
-            raise ValueError(
-                "Invalid hook type %s. Must be one of {pre, post}", hook_type
-            )
-
-        for op_code, funcs in hook_dict.items():
-            entrypoint[op_code].extend(funcs)
-
-    def register_laser_hooks(self, hook_type: str, hook: Callable):
-        """registers the hook with this Laser VM"""
-
-        if hook_type in self.hook_type_map:
-            self.hook_type_map[hook_type].append(hook)
-        else:
-            raise ValueError(f"Invalid hook type {hook_type}")
-
-    def register_instr_hooks(self, hook_type: str, opcode: str, hook: Callable):
-        """Registers instructions hooks from plugins"""
-        if hook_type == "pre":
-            if opcode is None:
-                for op in OPCODES:
-                    self.instr_pre_hook[op].append(hook(op))
-            else:
-                self.instr_pre_hook[opcode].append(hook)
-        elif hook_type == 'preprocessing_pre':  # @wei
-            if opcode is None:
-                for op, _, _, _ in OPCODES.values():
-                    self.instr_post_hook[op].append(hook(op))
-            else:
-                self.instr_post_hook[opcode].append(hook)
-        else:
-            if opcode is None:
-                for op in OPCODES:
-                    self.instr_post_hook[op].append(hook(op))
-            else:
-                self.instr_post_hook[opcode].append(hook)
-
-    def instr_hook(self, hook_type, opcode) -> Callable:
-        """Registers the annoted function with register_instr_hooks
-
-        :param hook_type: Type of hook pre/post
-        :param opcode: The opcode related to the function
-        """
-
-        def hook_decorator(func: Callable):
-            """Hook decorator generated by laser_hook
-
-            :param func: Decorated function
-            """
-            self.register_instr_hooks(hook_type, opcode, func)
-
-        return hook_decorator
-
-    def laser_hook(self, hook_type: str) -> Callable:
-        """Registers the annotated function with register_laser_hooks
-
-        :param hook_type:
-        :return: hook decorator
-        """
-
-        def hook_decorator(func: Callable):
-            """Hook decorator generated by laser_hook
-
-            :param func: Decorated function
-            """
-            self.register_laser_hooks(hook_type, func)
-            return func
-
-        return hook_decorator
-
-    def _execute_pre_hook(self, op_code: str, global_state: GlobalState) -> None:
-        """
-
-        :param op_code:
-        :param global_state:
-        :return:
-        """
-        if op_code not in self.pre_hooks.keys():
-            return
-        for hook in self.pre_hooks[op_code]:
-            hook(global_state)
-
-    def _execute_post_hook(
-        self, op_code: str, global_states: List[GlobalState]
-    ) -> None:
-        """
-
-        :param op_code:
-        :param global_states:
-        :return:
-        """
-        if op_code not in self.post_hooks.keys():
-            return
-
-        for hook in self.post_hooks[op_code]:
-            for global_state in global_states:
-                try:
-                    hook(global_state)
-                except PluginSkipState:
-                    global_states.remove(global_state)
-
-    def pre_hook(self, op_code: str) -> Callable:
-        """
-
-        :param op_code:
-        :return:
-        """
-
-        def hook_decorator(func: Callable):
-            """
-
-            :param func:
-            :return:
-            """
-            if op_code not in self.pre_hooks.keys():
-                self.pre_hooks[op_code] = []
-            self.pre_hooks[op_code].append(func)
-            return func
-
-        return hook_decorator
-
-    def post_hook(self, op_code: str) -> Callable:
-        """
-
-        :param op_code:
-        :return:
-        """
-
-        def hook_decorator(func: Callable):
-            """
-
-            :param func:
-            :return:
-            """
-            if op_code not in self.post_hooks.keys():
-                self.post_hooks[op_code] = []
-            self.post_hooks[op_code].append(func)
-            return func
-
-        return hook_decorator
-
-    #@wei  preprocessing_pre_hook
-    def preprocessing_pre_hook(self, op_code: str) -> Callable:
-        """
-        :param op_code:
-        :return:
-        """
-        def hook_decorator(func: Callable):
-            """
-            :param func:
-            :return:
-            """
-            if op_code not in self.preprocessing_pre_hooks.keys():
-                self.preprocessing_pre_hooks[op_code] = []
-            self.preprocessing_pre_hooks[op_code].append(func)
-            return func
-
-        return hook_decorator
+"""This module implements the main symbolic execution engine."""
+import logging
+from collections import defaultdict
+from copy import copy, deepcopy
+from datetime import datetime, timedelta
+import random
+from typing import Callable, Dict, DefaultDict, List, Tuple, Optional
+
+from mythril.support.opcodes import OPCODES
+from mythril.analysis.potential_issues import check_potential_issues
+from mythril.laser.execution_info import ExecutionInfo
+from mythril.laser.ethereum.cfg import NodeFlags, Node, Edge, JumpType
+from mythril.laser.ethereum.evm_exceptions import StackUnderflowException, VmException
+from mythril.laser.ethereum.instructions import Instruction
+from mythril.laser.ethereum.instruction_data import get_required_stack_elements
+from mythril.laser.plugin.signals import PluginSkipWorldState, PluginSkipState
+from mythril.laser.ethereum.state.global_state import GlobalState
+from mythril.laser.ethereum.state.world_state import WorldState
+from mythril.laser.ethereum.strategy.basic import DepthFirstSearchStrategy
+from mythril.laser.ethereum.strategy.constraint_strategy import DelayConstraintStrategy
+from abc import ABCMeta
+from mythril.laser.ethereum.time_handler import time_handler
+
+from mythril.laser.ethereum.transaction import (
+    ContractCreationTransaction,
+    TransactionEndSignal,
+    TransactionStartSignal,
+    execute_contract_creation,
+    execute_message_call,
+)
+from mythril.laser.smt import symbol_factory
+from mythril.support.support_args import args
+import fdg
+
+from fdg.preprocessing.preprocess import execute_preprocessing
+log = logging.getLogger(__name__)
+
+
+class SVMError(Exception):
+    """An exception denoting an unexpected state in symbolic execution."""
+
+    pass
+
+
+class LaserEVM:
+    """The LASER EVM.
+
+    Just as Mithril had to be mined at great efforts to provide the
+    Dwarves with their exceptional armour, LASER stands at the heart of
+    Mythril, digging deep in the depths of call graphs, unearthing the
+    most precious symbolic call data, that is then hand-forged into
+    beautiful and strong security issues by the experienced smiths we
+    call detection modules. It is truly a magnificent symbiosis.
+    """
+
+    def __init__(
+        self,
+        dynamic_loader=None,
+        max_depth=float("inf"),
+        execution_timeout=60,
+        create_timeout=10,
+        strategy=DepthFirstSearchStrategy,
+        transaction_count=2,
+        requires_statespace=True,
+        iprof=None,
+        use_reachability_check=True,
+        beam_width=None,
+    ) -> None:
+        """
+        Initializes the laser evm object
+
+        :param dynamic_loader: Loads data from chain
+        :param max_depth: Maximum execution depth this vm should execute
+        :param execution_timeout: Time to take for execution
+        :param create_timeout: Time to take for contract creation
+        :param strategy: Execution search strategy
+        :param transaction_count: The amount of transactions to execute
+        :param requires_statespace: Variable indicating whether the statespace should be recorded
+        :param iprof: Instruction Profiler
+        """
+        self.execution_info: List[ExecutionInfo] = []
+
+        self.open_states: List[WorldState] = []
+        self.total_states = 0
+        self.dynamic_loader = dynamic_loader
+        self.use_reachability_check = use_reachability_check
+
+        self.work_list: List[GlobalState] = []
+        self.strategy = strategy(self.work_list, max_depth, beam_width=beam_width)
+        self.max_depth = max_depth
+        self.transaction_count = transaction_count
+
+        self.execution_timeout = execution_timeout or 0
+        self.create_timeout = create_timeout or 0
+
+        self.requires_statespace = requires_statespace
+        if self.requires_statespace:
+            self.nodes: Dict[int, Node] = {}
+            self.edges: List[Edge] = []
+
+        self.time: datetime = None
+        self.executed_transactions: bool = False
+
+        self.pre_hooks: DefaultDict[str, List[Callable]] = defaultdict(list)
+        self.post_hooks: DefaultDict[str, List[Callable]] = defaultdict(list)
+
+        self._add_world_state_hooks: List[Callable] = []
+        self._execute_state_hooks: List[Callable] = []
+
+        self._start_exec_trans_hooks: List[Callable] = []
+        self._stop_exec_trans_hooks: List[Callable] = []
+
+        self._start_sym_trans_hooks: List[Callable] = []
+        self._stop_sym_trans_hooks: List[Callable] = []
+
+        self._start_sym_exec_hooks: List[Callable] = []
+        self._stop_sym_exec_hooks: List[Callable] = []
+
+        self._start_exec_hooks: List[Callable] = []
+        self._stop_exec_hooks: List[Callable] = []
+
+        self._transaction_end_hooks: List[Callable] = []
+
+        self.iprof = iprof
+        self.instr_pre_hook: Dict[str, List[Callable]] = {}
+        self.instr_post_hook: Dict[str, List[Callable]] = {}
+
+        self._start_sym_trans_hooks_laserEVM=[] #@wei
+        self._stop_sym_trans_hooks_laserEVM = []  # @wei
+        self._branch_check_hooks = []  # @wei
+        self.preprocessing_pre_hooks = defaultdict(list)  # @wei
+        self._pre_execute_state_hooks = []  # type:List[Callable]#@wei
+        self._post_execute_state_hooks = []  # type:List[Callable] #@wei
+        self._preprocessing_execute_state_hooks = []
+        for op in OPCODES:
+            self.instr_pre_hook[op] = []
+            self.instr_post_hook[op] = []
+        self.hook_type_map = {
+            "start_execute_transactions": self._start_exec_trans_hooks,
+            "stop_execute_transactions": self._stop_exec_trans_hooks,
+            "add_world_state": self._add_world_state_hooks,
+            "execute_state": self._execute_state_hooks,
+            "start_sym_exec": self._start_sym_exec_hooks,
+            "stop_sym_exec": self._stop_sym_exec_hooks,
+            "start_sym_trans": self._start_sym_trans_hooks,
+            "stop_sym_trans": self._stop_sym_trans_hooks,
+            "start_exec": self._start_exec_hooks,
+            "stop_exec": self._stop_exec_hooks,
+            "transaction_end": self._transaction_end_hooks,
+            'pre_execute_state':self._pre_execute_state_hooks,#@wei
+            'post_execute_state':self._post_execute_state_hooks,#@wei
+            'branch_check':self._branch_check_hooks,#@wei
+            'preprocessing_execute_state':self._preprocessing_execute_state_hooks,#@wei
+            'start_sym_trans_laserEVM':self._start_sym_trans_hooks_laserEVM,#@wei
+            'stop_sym_trans_laserEVM':self._stop_sym_trans_hooks_laserEVM,#@wei
+        }
+        log.info("LASER EVM initialized with dynamic loader: " + str(dynamic_loader))
+
+
+    def extend_strategy(self, extension: ABCMeta, **kwargs) -> None:
+        self.strategy = extension(self.strategy, **kwargs)
+
+    def sym_exec(
+        self,
+        world_state: WorldState = None,
+        target_address: int = None,
+        creation_code: str = None,
+        contract_name: str = None,
+    ) -> None:
+        """Starts symbolic execution
+        There are two modes of execution.
+        Either we analyze a preconfigured configuration, in which case the world_state and target_address variables
+        must be supplied.
+        Or we execute the creation code of a contract, in which case the creation code and desired name of that
+        contract should be provided.
+
+        :param world_state The world state configuration from which to perform analysis
+        :param target_address The address of the contract account in the world state which analysis should target
+        :param creation_code The creation code to create the target contract in the symbolic environment
+        :param contract_name The name that the created account should be associated with
+        """
+        pre_configuration_mode = target_address is not None
+        scratch_mode = creation_code is not None and contract_name is not None
+        if pre_configuration_mode == scratch_mode:
+            raise ValueError("Symbolic execution started with invalid parameters")
+
+        log.debug("Starting LASER execution")
+        for hook in self._start_sym_exec_hooks:
+            hook()
+
+        time_handler.start_execution(self.execution_timeout)
+        self.time = datetime.now()
+
+        if pre_configuration_mode:
+            self.open_states = [world_state]
+            log.info("Starting message call transaction to {}".format(target_address))
+            self.execute_transactions(symbol_factory.BitVecVal(target_address, 256))
+
+        elif scratch_mode:
+            log.info("Starting contract creation transaction")
+
+            created_account = execute_contract_creation(
+                self, creation_code, contract_name, world_state=world_state
+            )
+            fdg.global_config.contract_address = created_account.address
+
+            log.info(
+                "Finished contract creation, found {} open states".format(
+                    len(self.open_states)
+                )
+            )
+
+            if len(self.open_states) == 0:
+                log.warning(
+                    "No contract was created during the execution of contract creation "
+                    "Increase the resources for creation execution (--max-depth or --create-timeout) "
+                    "Check whether the bytecode is indeed the creation code, otherwise use the --bin-runtime flag"
+                )
+
+            # if fdg.global_config.flag_fwrg:
+            #     self._execute_transactions_fdg(created_account.address)
+            # else:
+            #     self._execute_transactions(created_account.address)
+            self.execute_transactions(created_account.address)
+        log.info("Finished symbolic execution")
+        if self.requires_statespace:
+            log.info(
+                "%d nodes, %d edges, %d total states",
+                len(self.nodes),
+                len(self.edges),
+                self.total_states,
+            )
+            print(f'#@statespace')
+            print("{} nodes, {} edges, {} total states".format(len(self.nodes), len(self.edges), self.total_states))
+        for hook in self._stop_sym_exec_hooks:
+            hook()
+
+    def execute_transactions(self, address) -> None:
+        """This function helps runs plugins that can order transactions.
+        Such plugins should set self.executed_transactions as True after its execution
+
+        :param address: Address of the contract
+        :return: None
+        """
+        for hook in self._start_exec_trans_hooks:
+            hook()
+
+        if self.executed_transactions is False:
+            if fdg.global_config.flag_fwrg:
+                self._execute_transactions_fdg(address)
+            else:
+                self._execute_transactions(address)
+            # self._execute_transactions(address)
+
+        for hook in self._stop_exec_trans_hooks:
+            hook()
+
+    def _execute_transactions(self, address):
+        """This function executes multiple transactions on the address
+
+        :param address: Address of the contract
+        :return:
+        """
+        self.time = datetime.now()
+
+        for i in range(self.transaction_count):
+            if len(self.open_states) == 0:
+                break
+            old_states_count = len(self.open_states)
+
+            if self.use_reachability_check:
+                log.info("do reachability check")
+                self.open_states = [
+                    state
+                    for state in self.open_states
+                    if state.constraints.is_possible()
+                ]
+                prune_count = old_states_count - len(self.open_states)
+                if prune_count:
+                    log.info("Pruned {} unreachable states".format(prune_count))
+            log.info(
+                "Starting message call transaction, iteration: {}, {} initial states".format(
+                    i, len(self.open_states)
+                )
+            )
+            func_hashes = (
+                args.transaction_sequences[i] if args.transaction_sequences else None
+            )
+
+            if func_hashes:
+                for itr, func_hash in enumerate(func_hashes):
+                    if func_hash in (-1, -2):
+                        func_hashes[itr] = func_hash
+                    else:
+                        func_hashes[itr] = bytes.fromhex(hex(func_hash)[2:].zfill(8))
+
+            for hook in self._start_sym_trans_hooks:
+                hook()
+
+            execute_message_call(self, address, func_hashes=func_hashes)
+
+            for hook in self._stop_sym_trans_hooks:
+                hook()
+
+        self.executed_transactions = True
+
+    def _execute_transactions_fdg(self, address):
+        """This function executes multiple transactions on the address
+
+        :param address: Address of the contract
+        :return:
+        """
+        self.time = datetime.now()
+        i = 0
+        while i < fdg.global_config.transaction_count:  # @wei rewrite loop
+            if fdg.global_config.function_search_strategy in ['mine','bfs','dfs']:
+                # need the special transaction
+                if i == 0:
+                    copy_laserEVM = deepcopy(self)
+                    copy_laserEVM.requires_statespace=False
+                    copy_laserEVM.post_hooks={}
+                    copy_laserEVM.pre_hooks={}
+                    execute_preprocessing(address, copy_laserEVM)
+                    i += 1
+                    continue
+
+            log.info(
+                "Starting message call transaction, iteration: {}, {} initial states".format(
+                    i, len(self.open_states)
+                )
+            )
+            for hook in self._start_sym_trans_hooks:
+                hook()
+            for hook in self._start_sym_trans_hooks_laserEVM:
+                hook(self)
+
+            execute_message_call(self, address)
+
+            for hook in self._stop_sym_trans_hooks:
+                hook()
+
+            for hook in self._stop_sym_trans_hooks_laserEVM:
+                hook(self)
+            i += 1
+
+    def _check_create_termination(self) -> bool:
+        if len(self.open_states) != 0:
+            return (
+                self.create_timeout > 0
+                and self.time + timedelta(seconds=self.create_timeout) <= datetime.now()
+            )
+        return self._check_execution_termination()
+
+    def _check_execution_termination(self) -> bool:
+        return (
+            self.execution_timeout > 0
+            and self.time + timedelta(seconds=self.execution_timeout) <= datetime.now()
+        )
+
+        # @wei
+
+    def _check_preprocessing_termination(self) -> bool:
+
+        return self.time + timedelta(seconds=fdg.global_config.preprocess_timeout) <= datetime.now()
+
+        # @wei
+
+    def _check_preprocessing_error(self) -> bool:
+        return fdg.global_config.preprocessing_exception
+
+
+    # @wei adopt from exec()
+    def exec_preprocessing(self):
+        """
+                :param create:
+                :param track_gas:
+                :return:
+        """
+        for global_state in self.strategy:
+            # @wei througth timeout
+            if self._check_preprocessing_termination():
+                log.debug("hit the exec_preprocessing excution time, return.")
+                print("hit the exec_preprocessing excution time, return.")
+                fdg.global_config.flag_preprocess_timeout = True
+                return None
+            # @wei check errors in preprocessing
+            if self._check_preprocessing_error():
+                log.debug("have exceptions in preprocessing.")
+                print("have exceptions in preprocessing.")
+                return None
+
+            try:
+                new_states, op_code = self.execute_state_preprocessing(global_state)
+
+            except NotImplementedError:
+                log.debug("Encountered unimplemented instruction")
+                continue
+
+            # should be kept otherwise, active function information can not be obtained.
+            self.manage_cfg(op_code, new_states)  # TODO: What about op_code is None?
+            if new_states:
+                self.work_list += new_states
+
+        return None
+
+    # @wei
+    def _execute_preprocessing_pre_hook(self, op_code: str, global_state):
+        if op_code not in self.preprocessing_pre_hooks.keys():
+            return
+        for hook in self.preprocessing_pre_hooks[op_code]:
+            hook(global_state)
+
+    # @wei
+    def execute_state_preprocessing(
+        self, global_state: GlobalState
+    ) -> Tuple[List[GlobalState], Optional[str]]:
+        """Execute a single instruction in global_state.
+
+        :param global_state:
+        :return: A list of successor states.
+        """
+
+        instructions = global_state.environment.code.instruction_list
+
+        try:
+            op_code = instructions[global_state.mstate.pc]["opcode"]
+            # Execute hooks
+            for hook in self._preprocessing_execute_state_hooks:
+                hook(global_state, op_code)
+
+            # if global_state.environment.active_function_name in ['getBalance(address,address)']:
+            #     print(f'{global_state.environment.active_function_name}:{instructions[global_state.mstate.pc]}')
+
+        except IndexError:
+            # self._add_world_state(global_state)
+            return [], None
+
+        if len(global_state.mstate.stack) < get_required_stack_elements(op_code):
+            error_msg = (
+                "Stack Underflow Exception due to insufficient "
+                "stack elements for the address {}".format(
+                    instructions[global_state.mstate.pc]["address"]
+                )
+            )
+            new_global_states = self.handle_vm_exception(
+                global_state, op_code, error_msg
+            )
+            # self._execute_post_hook(op_code, new_global_states)
+            return new_global_states, op_code
+
+        try:
+            self._execute_preprocessing_pre_hook(op_code, global_state)
+        except PluginSkipState:
+            return [], None
+
+        try:
+            new_global_states = Instruction(
+                op_code,
+                self.dynamic_loader,
+                pre_hooks=[],
+                post_hooks=[],
+            ).evaluate(global_state)
+
+        except VmException as e:
+            # for hook in self._transaction_end_hooks:
+            #     hook(
+            #         global_state,
+            #         global_state.current_transaction,
+            #         None,
+            #         False,
+            #     )
+            new_global_states = self.handle_vm_exception(global_state, op_code, str(e))
+
+        except TransactionStartSignal as start_signal:
+            # Setup new global state
+            new_global_state = start_signal.transaction.initial_global_state()
+
+            new_global_state.transaction_stack = copy(
+                global_state.transaction_stack
+            ) + [(start_signal.transaction, global_state)]
+            new_global_state.node = global_state.node
+            new_global_state.world_state.constraints = (
+                start_signal.global_state.world_state.constraints
+            )
+
+            log.debug("Starting new transaction %s", start_signal.transaction)
+
+            return [new_global_state], op_code
+
+        except TransactionEndSignal as end_signal:
+            (
+                transaction,
+                return_global_state,
+            ) = end_signal.global_state.transaction_stack[-1]
+
+            log.debug("Ending transaction %s.", transaction)
+
+            # for hook in self._transaction_end_hooks:
+            #     hook(
+            #         end_signal.global_state,
+            #         transaction,
+            #         return_global_state,
+            #         end_signal.revert,
+            #     )
+
+            if return_global_state is None:
+                # if (
+                #     not isinstance(transaction, ContractCreationTransaction)
+                #     or transaction.return_data
+                # ) and not end_signal.revert:
+                #     check_potential_issues(global_state)
+                #     end_signal.global_state.world_state.node = global_state.node
+                #     self._add_world_state(end_signal.global_state)
+
+                new_global_states = []
+            else:
+
+                # # First execute the post hook for the transaction ending instruction
+                # self._execute_post_hook(op_code, [end_signal.global_state])
+
+                # Propagate annotations
+                new_annotations = [
+                    annotation
+                    for annotation in global_state.annotations
+                    if annotation.persist_over_calls
+                ]
+                return_global_state.add_annotations(new_annotations)
+
+                new_global_states = self._end_message_call(
+                    copy(return_global_state),
+                    global_state,
+                    revert_changes=False or end_signal.revert,
+                    return_data=transaction.return_data,
+                )
+
+        # self._execute_post_hook(op_code, new_global_states)
+
+        return new_global_states, op_code
+
+
+
+    def exec(self, create=False, track_gas=False) -> Optional[List[GlobalState]]:
+        """
+
+        :param create:
+        :param track_gas:
+        :return:
+        """
+        final_states = []  # type: List[GlobalState]
+        for hook in self._start_exec_hooks:
+            hook()
+
+        for global_state in self.strategy:
+
+            if create and self._check_create_termination():
+                log.debug("Hit create timeout, returning.")
+                return final_states + [global_state] if track_gas else None
+
+            if not create and self._check_execution_termination():
+                log.debug("Hit execution timeout, returning.")
+                return final_states + [global_state] if track_gas else None
+            try:
+
+                new_states, op_code = self.execute_state(global_state)
+
+            except NotImplementedError:
+                log.debug("Encountered unimplemented instruction")
+                continue
+
+            if self.strategy.run_check() and (
+                len(new_states) > 1 and random.uniform(0, 1) < args.pruning_factor
+            ): # need to be careful: previous version:if args.sparse_pruning is False:
+
+                new_states = [
+                    state
+                    for state in new_states
+                    if state.world_state.constraints.is_possible()
+                ]
+
+
+
+            self.manage_cfg(op_code, new_states)  # TODO: What about op_code is None?
+            if new_states:
+                self.work_list += new_states
+            elif track_gas:
+                final_states.append(global_state)
+            self.total_states += len(new_states)
+
+        # need to be careful as this does not appear in previous version
+        for hook in self._stop_exec_hooks:
+            hook()
+
+        return final_states if track_gas else None
+
+    def _add_world_state(self, global_state: GlobalState):
+        """Stores the world_state of the passed global state in the open states"""
+
+        for hook in self._add_world_state_hooks:
+            try:
+                hook(global_state)
+            except PluginSkipWorldState:
+                return
+
+        self.open_states.append(global_state.world_state)
+
+    def handle_vm_exception(
+        self, global_state: GlobalState, op_code: str, error_msg: str
+    ) -> List[GlobalState]:
+        _, return_global_state = global_state.transaction_stack.pop()
+
+        if return_global_state is None:
+            # In this case we don't put an unmodified world state in the open_states list Since in the case of an
+            #  exceptional halt all changes should be discarded, and this world state would not provide us with a
+            #  previously unseen world state
+            log.debug("Encountered a VmException, ending path: `{}`".format(error_msg))
+            new_global_states = []  # type: List[GlobalState]
+        else:
+            # First execute the post hook for the transaction ending instruction
+            self._execute_post_hook(op_code, [global_state])
+            new_global_states = self._end_message_call(
+                return_global_state, global_state, revert_changes=True, return_data=None
+            )
+        return new_global_states
+
+    def execute_state(
+        self, global_state: GlobalState
+    ) -> Tuple[List[GlobalState], Optional[str]]:
+        """Execute a single instruction in global_state.
+
+        :param global_state:
+        :return: A list of successor states.
+        """
+        # Execute hooks
+        try:
+            for hook in self._execute_state_hooks:
+                hook(global_state)
+        except PluginSkipState:
+            return [], None
+
+        instructions = global_state.environment.code.instruction_list
+
+        try:
+            op_code = instructions[global_state.mstate.pc]["opcode"]
+            # if global_state.environment.active_function_name in ['getBalance(address,address)']:
+            #     print(f'{global_state.environment.active_function_name}:{instructions[global_state.mstate.pc]}')
+
+        except IndexError:
+            self._add_world_state(global_state)
+            return [], None
+
+        if len(global_state.mstate.stack) < get_required_stack_elements(op_code):
+            error_msg = (
+                "Stack Underflow Exception due to insufficient "
+                "stack elements for the address {}".format(
+                    instructions[global_state.mstate.pc]["address"]
+                )
+            )
+            new_global_states = self.handle_vm_exception(
+                global_state, op_code, error_msg
+            )
+            self._execute_post_hook(op_code, new_global_states)
+            return new_global_states, op_code
+
+        try:
+            self._execute_pre_hook(op_code, global_state)
+        except PluginSkipState:
+            return [], None
+
+        try:
+            new_global_states = Instruction(
+                op_code,
+                self.dynamic_loader,
+                pre_hooks=self.instr_pre_hook[op_code],
+                post_hooks=self.instr_post_hook[op_code],
+            ).evaluate(global_state)
+
+        except VmException as e:
+            for hook in self._transaction_end_hooks:
+                hook(
+                    global_state,
+                    global_state.current_transaction,
+                    None,
+                    False,
+                )
+            new_global_states = self.handle_vm_exception(global_state, op_code, str(e))
+
+        except TransactionStartSignal as start_signal:
+            # Setup new global state
+            new_global_state = start_signal.transaction.initial_global_state()
+
+            new_global_state.transaction_stack = copy(
+                global_state.transaction_stack
+            ) + [(start_signal.transaction, global_state)]
+            new_global_state.node = global_state.node
+            new_global_state.world_state.constraints = (
+                start_signal.global_state.world_state.constraints
+            )
+
+            log.debug("Starting new transaction %s", start_signal.transaction)
+
+            return [new_global_state], op_code
+
+        except TransactionEndSignal as end_signal:
+            (
+                transaction,
+                return_global_state,
+            ) = end_signal.global_state.transaction_stack[-1]
+
+            log.debug("Ending transaction %s.", transaction)
+
+            for hook in self._transaction_end_hooks:
+                hook(
+                    end_signal.global_state,
+                    transaction,
+                    return_global_state,
+                    end_signal.revert,
+                )
+
+            if return_global_state is None:
+                if (
+                    not isinstance(transaction, ContractCreationTransaction)
+                    or transaction.return_data
+                ) and not end_signal.revert:
+                    check_potential_issues(global_state)
+                    end_signal.global_state.world_state.node = global_state.node
+                    self._add_world_state(end_signal.global_state)
+
+                new_global_states = []
+            else:
+
+                # First execute the post hook for the transaction ending instruction
+                self._execute_post_hook(op_code, [end_signal.global_state])
+
+                # Propagate annotations
+                new_annotations = [
+                    annotation
+                    for annotation in global_state.annotations
+                    if annotation.persist_over_calls
+                ]
+                return_global_state.add_annotations(new_annotations)
+
+                new_global_states = self._end_message_call(
+                    copy(return_global_state),
+                    global_state,
+                    revert_changes=False or end_signal.revert,
+                    return_data=transaction.return_data,
+                )
+
+        self._execute_post_hook(op_code, new_global_states)
+
+        return new_global_states, op_code
+
+    def _end_message_call(
+        self,
+        return_global_state: GlobalState,
+        global_state: GlobalState,
+        revert_changes=False,
+        return_data=None,
+    ) -> List[GlobalState]:
+        """
+
+        :param return_global_state:
+        :param global_state:
+        :param revert_changes:
+        :param return_data:
+        :return:
+        """
+
+        return_global_state.world_state.constraints += (
+            global_state.world_state.constraints
+        )
+        # Resume execution of the transaction initializing instruction
+        op_code = return_global_state.environment.code.instruction_list[
+            return_global_state.mstate.pc
+        ]["opcode"]
+
+        # Set execution result in the return_state
+        return_global_state.last_return_data = return_data
+        if not revert_changes:
+            return_global_state.world_state = copy(global_state.world_state)
+            return_global_state.environment.active_account = global_state.accounts[
+                return_global_state.environment.active_account.address.value
+            ]
+            if isinstance(
+                global_state.current_transaction, ContractCreationTransaction
+            ):
+                return_global_state.mstate.min_gas_used += (
+                    global_state.mstate.min_gas_used
+                )
+                return_global_state.mstate.max_gas_used += (
+                    global_state.mstate.max_gas_used
+                )
+        try:
+            # Execute the post instruction handler
+            new_global_states = Instruction(
+                op_code,
+                self.dynamic_loader,
+                pre_hooks=self.instr_pre_hook[op_code],
+                post_hooks=self.instr_post_hook[op_code],
+            ).evaluate(return_global_state, True)
+        except VmException:
+            new_global_states = []
+        # In order to get a nice call graph we need to set the nodes here
+        for state in new_global_states:
+            state.node = global_state.node
+
+        return new_global_states
+
+    def manage_cfg(self, opcode: str, new_states: List[GlobalState]) -> None:
+        """
+
+        :param opcode:
+        :param new_states:
+        """
+        if opcode == "JUMP":
+            assert len(new_states) <= 1
+            for state in new_states:
+                self._new_node_state(state)
+        elif opcode == "JUMPI":
+            assert len(new_states) <= 2
+            for state in new_states:
+                self._new_node_state(
+                    state, JumpType.CONDITIONAL, state.world_state.constraints[-1]
+                )
+        elif opcode in ("SLOAD", "SSTORE") and len(new_states) > 1:
+            for state in new_states:
+                self._new_node_state(
+                    state, JumpType.CONDITIONAL, state.world_state.constraints[-1]
+                )
+        elif opcode == "RETURN":
+            for state in new_states:
+                self._new_node_state(state, JumpType.RETURN)
+
+        for state in new_states:
+            # state.node.states.append(state)
+            # @wei
+            if state.mstate.pc >= len(state.environment.code.instruction_list):
+                print(
+                    f'self.mstate.pc:{state.mstate.pc}; len(instructions):{len(state.environment.code.instruction_list)}')
+            else:
+                state.node.states.append(state)
+    def _new_node_state(
+        self, state: GlobalState, edge_type=JumpType.UNCONDITIONAL, condition=None
+    ) -> None:
+        """
+
+        :param state:
+        :param edge_type:
+        :param condition:
+        """
+        try:
+            address = state.environment.code.instruction_list[state.mstate.pc][
+                "address"
+            ]
+        except IndexError:
+            return
+        new_node = Node(state.environment.active_account.contract_name)
+        old_node = state.node
+        state.node = new_node
+        new_node.constraints = state.world_state.constraints
+        if self.requires_statespace:
+            self.nodes[new_node.uid] = new_node
+            self.edges.append(
+                Edge(
+                    old_node.uid, new_node.uid, edge_type=edge_type, condition=condition
+                )
+            )
+
+        if edge_type == JumpType.RETURN:
+            new_node.flags |= NodeFlags.CALL_RETURN
+        elif edge_type == JumpType.CALL:
+            try:
+                if "retval" in str(state.mstate.stack[-1]):
+                    new_node.flags |= NodeFlags.CALL_RETURN
+                else:
+                    new_node.flags |= NodeFlags.FUNC_ENTRY
+            except StackUnderflowException:
+                new_node.flags |= NodeFlags.FUNC_ENTRY
+
+        environment = state.environment
+        disassembly = environment.code
+        if isinstance(
+            state.world_state.transaction_sequence[-1], ContractCreationTransaction
+        ):
+            environment.active_function_name = "constructor"
+        elif address in disassembly.address_to_function_name:
+            # Enter a new function
+            environment.active_function_name = disassembly.address_to_function_name[
+                address
+            ]
+            new_node.flags |= NodeFlags.FUNC_ENTRY
+
+            log.debug(
+                "- Entering function "
+                + environment.active_account.contract_name
+                + ":"
+                + new_node.function_name
+            )
+        elif address == 0:
+            environment.active_function_name = "fallback"
+
+        new_node.function_name = environment.active_function_name
+
+    def register_hooks(self, hook_type: str, hook_dict: Dict[str, List[Callable]]):
+        """
+
+        :param hook_type:
+        :param hook_dict:
+        """
+        if hook_type == "pre":
+            entrypoint = self.pre_hooks
+        elif hook_type == "post":
+            entrypoint = self.post_hooks
+        elif hook_type=='preprocessing_pre': #@wei
+            entrypoint=self.preprocessing_pre_hooks
+        else:
+            raise ValueError(
+                "Invalid hook type %s. Must be one of {pre, post}", hook_type
+            )
+
+        for op_code, funcs in hook_dict.items():
+            entrypoint[op_code].extend(funcs)
+
+    def register_laser_hooks(self, hook_type: str, hook: Callable):
+        """registers the hook with this Laser VM"""
+
+        if hook_type in self.hook_type_map:
+            self.hook_type_map[hook_type].append(hook)
+        else:
+            raise ValueError(f"Invalid hook type {hook_type}")
+
+    def register_instr_hooks(self, hook_type: str, opcode: str, hook: Callable):
+        """Registers instructions hooks from plugins"""
+        if hook_type == "pre":
+            if opcode is None:
+                for op in OPCODES:
+                    self.instr_pre_hook[op].append(hook(op))
+            else:
+                self.instr_pre_hook[opcode].append(hook)
+        elif hook_type == 'preprocessing_pre':  # @wei
+            if opcode is None:
+                for op, _, _, _ in OPCODES.values():
+                    self.instr_post_hook[op].append(hook(op))
+            else:
+                self.instr_post_hook[opcode].append(hook)
+        else:
+            if opcode is None:
+                for op in OPCODES:
+                    self.instr_post_hook[op].append(hook(op))
+            else:
+                self.instr_post_hook[opcode].append(hook)
+
+    def instr_hook(self, hook_type, opcode) -> Callable:
+        """Registers the annoted function with register_instr_hooks
+
+        :param hook_type: Type of hook pre/post
+        :param opcode: The opcode related to the function
+        """
+
+        def hook_decorator(func: Callable):
+            """Hook decorator generated by laser_hook
+
+            :param func: Decorated function
+            """
+            self.register_instr_hooks(hook_type, opcode, func)
+
+        return hook_decorator
+
+    def laser_hook(self, hook_type: str) -> Callable:
+        """Registers the annotated function with register_laser_hooks
+
+        :param hook_type:
+        :return: hook decorator
+        """
+
+        def hook_decorator(func: Callable):
+            """Hook decorator generated by laser_hook
+
+            :param func: Decorated function
+            """
+            self.register_laser_hooks(hook_type, func)
+            return func
+
+        return hook_decorator
+
+    def _execute_pre_hook(self, op_code: str, global_state: GlobalState) -> None:
+        """
+
+        :param op_code:
+        :param global_state:
+        :return:
+        """
+        if op_code not in self.pre_hooks.keys():
+            return
+        for hook in self.pre_hooks[op_code]:
+            hook(global_state)
+
+    def _execute_post_hook(
+        self, op_code: str, global_states: List[GlobalState]
+    ) -> None:
+        """
+
+        :param op_code:
+        :param global_states:
+        :return:
+        """
+        if op_code not in self.post_hooks.keys():
+            return
+
+        for hook in self.post_hooks[op_code]:
+            for global_state in global_states:
+                try:
+                    hook(global_state)
+                except PluginSkipState:
+                    global_states.remove(global_state)
+
+    def pre_hook(self, op_code: str) -> Callable:
+        """
+
+        :param op_code:
+        :return:
+        """
+
+        def hook_decorator(func: Callable):
+            """
+
+            :param func:
+            :return:
+            """
+            if op_code not in self.pre_hooks.keys():
+                self.pre_hooks[op_code] = []
+            self.pre_hooks[op_code].append(func)
+            return func
+
+        return hook_decorator
+
+    def post_hook(self, op_code: str) -> Callable:
+        """
+
+        :param op_code:
+        :return:
+        """
+
+        def hook_decorator(func: Callable):
+            """
+
+            :param func:
+            :return:
+            """
+            if op_code not in self.post_hooks.keys():
+                self.post_hooks[op_code] = []
+            self.post_hooks[op_code].append(func)
+            return func
+
+        return hook_decorator
+
+    #@wei  preprocessing_pre_hook
+    def preprocessing_pre_hook(self, op_code: str) -> Callable:
+        """
+        :param op_code:
+        :return:
+        """
+        def hook_decorator(func: Callable):
+            """
+            :param func:
+            :return:
+            """
+            if op_code not in self.preprocessing_pre_hooks.keys():
+                self.preprocessing_pre_hooks[op_code] = []
+            self.preprocessing_pre_hooks[op_code].append(func)
+            return func
+
+        return hook_decorator
```

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/time_handler.py` & `smartExecutorx-4.1/mythril/laser/ethereum/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/transaction/concolic.py` & `smartExecutorx-4.1/mythril/laser/ethereum/transaction/concolic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/transaction/symbolic.py` & `smartExecutorx-4.1/mythril/laser/ethereum/transaction/symbolic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/transaction/transaction_models.py` & `smartExecutorx-4.1/mythril/laser/ethereum/transaction/transaction_models.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/ethereum/util.py` & `smartExecutorx-4.1/mythril/laser/ethereum/util.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/__init__.py` & `smartExecutorx-4.1/mythril/laser/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/interface.py` & `smartExecutorx-4.1/mythril/laser/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/loader.py` & `smartExecutorx-4.1/mythril/laser/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/plugins/__init__.py` & `smartExecutorx-4.1/mythril/laser/plugin/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/plugins/benchmark.py` & `smartExecutorx-4.1/mythril/laser/plugin/plugins/benchmark.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/plugins/call_depth_limiter.py` & `smartExecutorx-4.1/mythril/laser/plugin/plugins/call_depth_limiter.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/plugins/coverage/coverage_plugin.py` & `smartExecutorx-4.1/mythril/laser/plugin/plugins/coverage/coverage_plugin.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/plugins/coverage/coverage_strategy.py` & `smartExecutorx-4.1/mythril/laser/plugin/plugins/coverage/coverage_strategy.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/plugins/dependency_pruner.py` & `smartExecutorx-4.1/mythril/laser/plugin/plugins/dependency_pruner.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/plugins/instruction_profiler.py` & `smartExecutorx-4.1/mythril/laser/plugin/plugins/instruction_profiler.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/plugins/mutation_pruner.py` & `smartExecutorx-4.1/mythril/laser/plugin/plugins/mutation_pruner.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/plugins/plugin_annotations.py` & `smartExecutorx-4.1/mythril/laser/plugin/plugins/plugin_annotations.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/plugin/signals.py` & `smartExecutorx-4.1/mythril/laser/plugin/signals.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/__init__.py` & `smartExecutorx-4.1/mythril/laser/smt/__init__.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/array.py` & `smartExecutorx-4.1/mythril/laser/smt/array.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/bitvec.py` & `smartExecutorx-4.1/mythril/laser/smt/bitvec.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/bitvec_helper.py` & `smartExecutorx-4.1/mythril/laser/smt/bitvec_helper.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/bool.py` & `smartExecutorx-4.1/mythril/laser/smt/bool.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/expression.py` & `smartExecutorx-4.1/mythril/laser/smt/expression.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/function.py` & `smartExecutorx-4.1/mythril/laser/smt/function.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/model.py` & `smartExecutorx-4.1/mythril/laser/smt/model.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/solver/independence_solver.py` & `smartExecutorx-4.1/mythril/laser/smt/solver/independence_solver.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/solver/solver.py` & `smartExecutorx-4.1/mythril/laser/smt/solver/solver.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/laser/smt/solver/solver_statistics.py` & `smartExecutorx-4.1/mythril/laser/smt/solver/solver_statistics.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/mythril/mythril_analyzer.py` & `smartExecutorx-4.1/mythril/mythril/mythril_analyzer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-import logging
-import traceback
-from typing import Optional, List
-from argparse import Namespace
-
-
-from . import MythrilDisassembler
-from mythril.support.source_support import Source
-from mythril.support.loader import DynLoader
-from mythril.support.support_args import args
-from mythril.analysis.symbolic import SymExecWrapper
-from mythril.analysis.callgraph import generate_graph
-from mythril.analysis.traceexplore import get_serializable_statespace
-from mythril.analysis.security import fire_lasers, retrieve_callback_issues
-from mythril.analysis.report import Report, Issue
-from mythril.ethereum.evmcontract import EVMContract
-from mythril.laser.smt import SolverStatistics
-from mythril.support.start_time import StartTime
-from mythril.exceptions import DetectorNotFoundError
-from mythril.laser.execution_info import ExecutionInfo
-
-log = logging.getLogger(__name__)
-
-LARGE_TIME = 300
-
-
-class MythrilAnalyzer:
-    """
-    The Mythril Analyzer class
-    Responsible for the analysis of the smart contracts
-    """
-
-    def __init__(
-        self,
-        disassembler: MythrilDisassembler,
-        cmd_args: Namespace,
-        strategy: str = "dfs",
-        address: Optional[str] = None,
-    ):
-        """
-
-        :param disassembler: The MythrilDisassembler class
-        :param cmd_args: The command line args Namespace
-        :param strategy: Search strategy
-        :param address: Address of the contract
-        """
-        self.eth = disassembler.eth
-        self.contracts = disassembler.contracts or []  # type: List[EVMContract]
-        self.enable_online_lookup = disassembler.enable_online_lookup
-        self.use_onchain_data = not cmd_args.no_onchain_data
-        self.strategy = strategy
-        self.address = address
-        self.max_depth = cmd_args.max_depth
-        self.execution_timeout = cmd_args.execution_timeout
-        self.loop_bound = cmd_args.loop_bound
-        self.create_timeout = cmd_args.create_timeout
-        self.disable_dependency_pruning = cmd_args.disable_dependency_pruning
-        self.custom_modules_directory = (
-            cmd_args.custom_modules_directory
-            if cmd_args.custom_modules_directory
-            else ""
-        )
-        args.pruning_factor = cmd_args.pruning_factor
-        args.solver_timeout = cmd_args.solver_timeout
-        args.parallel_solving = cmd_args.parallel_solving
-        args.unconstrained_storage = cmd_args.unconstrained_storage
-        args.call_depth_limit = cmd_args.call_depth_limit
-        args.iprof = cmd_args.enable_iprof
-        args.solver_log = cmd_args.solver_log
-        args.transaction_sequences = cmd_args.transaction_sequences
-
-        if args.pruning_factor is None:
-            if self.execution_timeout > LARGE_TIME:
-                args.pruning_factor = 1
-            else:
-                args.pruning_factor = 0
-
-    def dump_statespace(self, contract: EVMContract = None) -> str:
-        """
-        Returns serializable statespace of the contract
-        :param contract: The Contract on which the analysis should be done
-        :return: The serialized state space
-        """
-        sym = SymExecWrapper(
-            contract or self.contracts[0],
-            self.address,
-            self.strategy,
-            dynloader=DynLoader(self.eth, active=self.use_onchain_data),
-            max_depth=self.max_depth,
-            execution_timeout=self.execution_timeout,
-            create_timeout=self.create_timeout,
-            disable_dependency_pruning=self.disable_dependency_pruning,
-            run_analysis_modules=False,
-            custom_modules_directory=self.custom_modules_directory,
-        )
-
-        return get_serializable_statespace(sym)
-
-    def graph_html(
-        self,
-        contract: EVMContract = None,
-        enable_physics: bool = False,
-        phrackify: bool = False,
-        transaction_count: Optional[int] = None,
-    ) -> str:
-        """
-
-        :param contract: The Contract on which the analysis should be done
-        :param enable_physics: If true then enables the graph physics simulation
-        :param phrackify: If true generates Phrack-style call graph
-        :param transaction_count: The amount of transactions to be executed
-        :return: The generated graph in html format
-        """
-
-        sym = SymExecWrapper(
-            contract or self.contracts[0],
-            self.address,
-            self.strategy,
-            dynloader=DynLoader(self.eth, active=self.use_onchain_data),
-            max_depth=self.max_depth,
-            execution_timeout=self.execution_timeout,
-            transaction_count=transaction_count,
-            create_timeout=self.create_timeout,
-            disable_dependency_pruning=self.disable_dependency_pruning,
-            run_analysis_modules=False,
-            custom_modules_directory=self.custom_modules_directory,
-        )
-        return generate_graph(sym, physics=enable_physics, phrackify=phrackify)
-
-    def fire_lasers(
-        self,
-        modules: Optional[List[str]] = None,
-        transaction_count: Optional[int] = None,
-    ) -> Report:
-        """
-        :param modules: The analysis modules which should be executed
-        :param transaction_count: The amount of transactions to be executed
-        :return: The Report class which contains the all the issues/vulnerabilities
-        """
-        all_issues = []  # type: List[Issue]
-        SolverStatistics().enabled = True
-
-        exceptions = []
-        execution_info = None  # type: Optional[List[ExecutionInfo]]
-        for contract in self.contracts:
-            StartTime()  # Reinitialize start time for new contracts
-            try:
-                sym = SymExecWrapper(
-                    contract,
-                    self.address,
-                    self.strategy,
-                    dynloader=DynLoader(self.eth, active=self.use_onchain_data),
-                    max_depth=self.max_depth,
-                    execution_timeout=self.execution_timeout,
-                    loop_bound=self.loop_bound,
-                    create_timeout=self.create_timeout,
-                    transaction_count=transaction_count,
-                    modules=modules,
-                    compulsory_statespace=True,  # @wei
-                    # compulsory_statespace=False,
-                    disable_dependency_pruning=self.disable_dependency_pruning,
-                    custom_modules_directory=self.custom_modules_directory,
-                )
-                issues = fire_lasers(sym, modules)
-                execution_info = sym.execution_info
-            except DetectorNotFoundError as e:
-                # Bubble up
-                raise e
-            except KeyboardInterrupt:
-                log.critical("Keyboard Interrupt")
-                issues = retrieve_callback_issues(modules)
-            except Exception:
-                log.critical(
-                    "Exception occurred, aborting analysis. Please report this issue to the Mythril GitHub page.\n"
-                    + traceback.format_exc()
-                )
-                issues = retrieve_callback_issues(modules)
-                exceptions.append(traceback.format_exc())
-            for issue in issues:
-                issue.add_code_info(contract)
-
-            all_issues += issues
-            # log.info("Solver statistics: \n{}".format(str(SolverStatistics())))
-            # print("Solver statistics:{}".format(str(SolverStatistics())))
-            # # @wei
-            # log.info(f'state constraint checking statistics:\n{str(StateConstraintCheckIndicator())}')
-            # print(f'state constraint checking statistics:{str(StateConstraintCheckIndicator())}')
-
-        source_data = Source()
-        source_data.get_source_from_contracts_list(self.contracts)
-
-        # Finally, output the results
-        report = Report(
-            contracts=self.contracts,
-            exceptions=exceptions,
-            execution_info=execution_info,
-        )
-        for issue in all_issues:
-            report.append_issue(issue)
-
-        return report
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import logging
+import traceback
+from typing import Optional, List
+from argparse import Namespace
+
+
+from . import MythrilDisassembler
+from mythril.support.source_support import Source
+from mythril.support.loader import DynLoader
+from mythril.support.support_args import args
+from mythril.analysis.symbolic import SymExecWrapper
+from mythril.analysis.callgraph import generate_graph
+from mythril.analysis.traceexplore import get_serializable_statespace
+from mythril.analysis.security import fire_lasers, retrieve_callback_issues
+from mythril.analysis.report import Report, Issue
+from mythril.ethereum.evmcontract import EVMContract
+from mythril.laser.smt import SolverStatistics
+from mythril.support.start_time import StartTime
+from mythril.exceptions import DetectorNotFoundError
+from mythril.laser.execution_info import ExecutionInfo
+
+log = logging.getLogger(__name__)
+
+LARGE_TIME = 300
+
+
+class MythrilAnalyzer:
+    """
+    The Mythril Analyzer class
+    Responsible for the analysis of the smart contracts
+    """
+
+    def __init__(
+        self,
+        disassembler: MythrilDisassembler,
+        cmd_args: Namespace,
+        strategy: str = "dfs",
+        address: Optional[str] = None,
+    ):
+        """
+
+        :param disassembler: The MythrilDisassembler class
+        :param cmd_args: The command line args Namespace
+        :param strategy: Search strategy
+        :param address: Address of the contract
+        """
+        self.eth = disassembler.eth
+        self.contracts = disassembler.contracts or []  # type: List[EVMContract]
+        self.enable_online_lookup = disassembler.enable_online_lookup
+        self.use_onchain_data = not cmd_args.no_onchain_data
+        self.strategy = strategy
+        self.address = address
+        self.max_depth = cmd_args.max_depth
+        self.execution_timeout = cmd_args.execution_timeout
+        self.loop_bound = cmd_args.loop_bound
+        self.create_timeout = cmd_args.create_timeout
+        self.disable_dependency_pruning = cmd_args.disable_dependency_pruning
+        self.custom_modules_directory = (
+            cmd_args.custom_modules_directory
+            if cmd_args.custom_modules_directory
+            else ""
+        )
+        args.pruning_factor = cmd_args.pruning_factor
+        args.solver_timeout = cmd_args.solver_timeout
+        args.parallel_solving = cmd_args.parallel_solving
+        args.unconstrained_storage = cmd_args.unconstrained_storage
+        args.call_depth_limit = cmd_args.call_depth_limit
+        args.iprof = cmd_args.enable_iprof
+        args.solver_log = cmd_args.solver_log
+        args.transaction_sequences = cmd_args.transaction_sequences
+
+        if args.pruning_factor is None:
+            if self.execution_timeout > LARGE_TIME:
+                args.pruning_factor = 1
+            else:
+                args.pruning_factor = 0
+
+    def dump_statespace(self, contract: EVMContract = None) -> str:
+        """
+        Returns serializable statespace of the contract
+        :param contract: The Contract on which the analysis should be done
+        :return: The serialized state space
+        """
+        sym = SymExecWrapper(
+            contract or self.contracts[0],
+            self.address,
+            self.strategy,
+            dynloader=DynLoader(self.eth, active=self.use_onchain_data),
+            max_depth=self.max_depth,
+            execution_timeout=self.execution_timeout,
+            create_timeout=self.create_timeout,
+            disable_dependency_pruning=self.disable_dependency_pruning,
+            run_analysis_modules=False,
+            custom_modules_directory=self.custom_modules_directory,
+        )
+
+        return get_serializable_statespace(sym)
+
+    def graph_html(
+        self,
+        contract: EVMContract = None,
+        enable_physics: bool = False,
+        phrackify: bool = False,
+        transaction_count: Optional[int] = None,
+    ) -> str:
+        """
+
+        :param contract: The Contract on which the analysis should be done
+        :param enable_physics: If true then enables the graph physics simulation
+        :param phrackify: If true generates Phrack-style call graph
+        :param transaction_count: The amount of transactions to be executed
+        :return: The generated graph in html format
+        """
+
+        sym = SymExecWrapper(
+            contract or self.contracts[0],
+            self.address,
+            self.strategy,
+            dynloader=DynLoader(self.eth, active=self.use_onchain_data),
+            max_depth=self.max_depth,
+            execution_timeout=self.execution_timeout,
+            transaction_count=transaction_count,
+            create_timeout=self.create_timeout,
+            disable_dependency_pruning=self.disable_dependency_pruning,
+            run_analysis_modules=False,
+            custom_modules_directory=self.custom_modules_directory,
+        )
+        return generate_graph(sym, physics=enable_physics, phrackify=phrackify)
+
+    def fire_lasers(
+        self,
+        modules: Optional[List[str]] = None,
+        transaction_count: Optional[int] = None,
+    ) -> Report:
+        """
+        :param modules: The analysis modules which should be executed
+        :param transaction_count: The amount of transactions to be executed
+        :return: The Report class which contains the all the issues/vulnerabilities
+        """
+        all_issues = []  # type: List[Issue]
+        SolverStatistics().enabled = True
+
+        exceptions = []
+        execution_info = None  # type: Optional[List[ExecutionInfo]]
+        for contract in self.contracts:
+            StartTime()  # Reinitialize start time for new contracts
+            try:
+                sym = SymExecWrapper(
+                    contract,
+                    self.address,
+                    self.strategy,
+                    dynloader=DynLoader(self.eth, active=self.use_onchain_data),
+                    max_depth=self.max_depth,
+                    execution_timeout=self.execution_timeout,
+                    loop_bound=self.loop_bound,
+                    create_timeout=self.create_timeout,
+                    transaction_count=transaction_count,
+                    modules=modules,
+                    compulsory_statespace=True,  # @wei
+                    # compulsory_statespace=False,
+                    disable_dependency_pruning=self.disable_dependency_pruning,
+                    custom_modules_directory=self.custom_modules_directory,
+                )
+                issues = fire_lasers(sym, modules)
+                execution_info = sym.execution_info
+            except DetectorNotFoundError as e:
+                # Bubble up
+                raise e
+            except KeyboardInterrupt:
+                log.critical("Keyboard Interrupt")
+                issues = retrieve_callback_issues(modules)
+            except Exception:
+                log.critical(
+                    "Exception occurred, aborting analysis. Please report this issue to the Mythril GitHub page.\n"
+                    + traceback.format_exc()
+                )
+                issues = retrieve_callback_issues(modules)
+                exceptions.append(traceback.format_exc())
+            for issue in issues:
+                issue.add_code_info(contract)
+
+            all_issues += issues
+            # log.info("Solver statistics: \n{}".format(str(SolverStatistics())))
+            # print("Solver statistics:{}".format(str(SolverStatistics())))
+            # # @wei
+            # log.info(f'state constraint checking statistics:\n{str(StateConstraintCheckIndicator())}')
+            # print(f'state constraint checking statistics:{str(StateConstraintCheckIndicator())}')
+
+        source_data = Source()
+        source_data.get_source_from_contracts_list(self.contracts)
+
+        # Finally, output the results
+        report = Report(
+            contracts=self.contracts,
+            exceptions=exceptions,
+            execution_info=execution_info,
+        )
+        for issue in all_issues:
+            report.append_issue(issue)
+
+        return report
```

### Comparing `smartExecutorx-4.0.0/mythril/mythril/mythril_config.py` & `smartExecutorx-4.1/mythril/mythril/mythril_config.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/mythril/mythril_disassembler.py` & `smartExecutorx-4.1/mythril/mythril/mythril_disassembler.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/plugin/discovery.py` & `smartExecutorx-4.1/mythril/plugin/discovery.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/plugin/interface.py` & `smartExecutorx-4.1/mythril/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/plugin/loader.py` & `smartExecutorx-4.1/mythril/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/solidity/soliditycontract.py` & `smartExecutorx-4.1/mythril/solidity/soliditycontract.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/support/assets/signatures.db` & `smartExecutorx-4.1/mythril/support/assets/signatures.db`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/support/loader.py` & `smartExecutorx-4.1/mythril/support/loader.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/support/lock.py` & `smartExecutorx-4.1/mythril/support/lock.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/support/model.py` & `smartExecutorx-4.1/mythril/support/model.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/support/opcodes.py` & `smartExecutorx-4.1/mythril/support/opcodes.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/support/signatures.py` & `smartExecutorx-4.1/mythril/support/signatures.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/support/source_support.py` & `smartExecutorx-4.1/mythril/support/source_support.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/support/support_args.py` & `smartExecutorx-4.1/mythril/support/support_args.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/mythril/support/support_utils.py` & `smartExecutorx-4.1/mythril/support/support_utils.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/requirements.txt` & `smartExecutorx-4.1/smartExecutorx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/setup.py` & `smartExecutorx-4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 TESTS_REQUIRE = ["mypy==0.782", "pytest>=3.6.0", "pytest_mock", "pytest-cov"]
 
 # What packages are optional?
 EXTRAS = {}
 
 # If version is set to None then it will be fetched from __version__.py
-VERSION = "v4.0.0"
+VERSION = "v4.1"
 
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
     with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
```

### Comparing `smartExecutorx-4.0.0/smartExecutorx.egg-info/PKG-INFO` & `smartExecutorx-4.1/smartExecutorx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartExecutorx
-Version: 4.0.0
+Version: 4.1
 Summary: Security analysis tool for Ethereum smart contracts
 Home-page: https://github.com/contractAnalysis/smartExecutor
 Author: contractAnalysis
 License: MIT
 Keywords: hacking disassembler security ethereum
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -21,41 +21,41 @@
 ##  SmartExecutor ##
 
 SmartExecutor is a guided symbolic execution tool for security analysis on EVM bytecode. It is designed to reduce the sequence explosion of symbolic execution to provide a scalable solution to symbolic execution while trying to maximize code coverage.  It has a dual-phase process. In Phase 1, it symbolically executes all possible function sequences within the given depth limit.
 
 Phase 2 then targets the not-fully-covered functions based on instruction coverage. This is the phase where the guidance takes place. SmartExecutor can direct the execution flow by prioritizing the states more significant to the target functions and selecting the functions at states to be executed that are more likely to cover the targets. The state significance value calculation and the function selection are based on static data dependency analysis and runtime execution data like function coverage and target functions.
 
 
-This is the [link](https://ieeexplore.ieee.org/document/10316942) to our conference paper: SmartExecutor: Coverage-Driven Symbolic Execution Guided by a Function Dependency Graph. 
+This is the [link](https://ieeexplore.ieee.org/document/10316942) to our conference paper: SmartExecutor: Coverage-Driven Symbolic Execution Guided by a Function Dependency Graph. The [documentation](https://page.d1xp6o5ammny8t.amplifyapp.com/) is available.
 
 
 
 ###  Run SmartExecutor through Docker: 
 
 1, Pull the Docker image of SmartExecutor:
 ```bash
 $ sudo docker pull 23278942/smartexecutor
 ```
 
 2, Run SmartExecutor with a single Docker command. Replace a_host_directory with the path to your host directory containing the Solidity file, for example, Crowdsale.sol.
 ```bash
-$ sudo docker run -it --rm -v a_host_directory:/home/smartExecutor/ image_id analyze ./Crowdsale.sol:Crowdsale
+$ sudo docker run -it --rm -v a_host_directory:/home/smartExecutor/ --entrypoint semyth 3278942/smartexecutor:latest analyze ./Crowdsale.sol:Crowdsale
 ```
 This command mounts the host directory to a directory inside the container and analyzes the contract Crowdsale defined in the Solidity file Crowdsale.sol.
 
 To analyze the sample Solidity file provided with the Docker image, you can use the following command:
 ```bash
-$ sudo docker run -it --rm image_id analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
+$ sudo docker run -it --rm --entrypoint semyth 3278942/smartexecutor:latest analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
 ```
 
 3, Additional Options
 
 To see more intermediate data, add the -v option followed by a value (3 or larger):
 ```bash
-$ sudo docker run -it --rm image_id -v 3 analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
+$ sudo docker run -it --rm --entrypoint semyth 3278942/smartexecutor:latest -v 3 analyze /opt/smartExecutor/tests/testdata/solidity_files/Crowdsale.sol:Crowdsale 
 ```
 
 Click [here](./example_output/Crowdsale.sol_terminal_output.txt) to see the terminal output.
 
 Click [here](./example_output/Crowdsale.sol_terminal_output_verbose.txt) to see the verbose intermediate results printed out in the terminal.
 
 <!--
@@ -70,14 +70,22 @@
 # set option '-v' to 3 to show the verbose intermediate results
 semyth -v 3 analyze ./Crowdsale.sol:Crowdsale 
 
 ```
 -->
 
 
+### Install solc-select and all versions of solc
+```
+pip install solc-select  # solc-select is a package to switch among different versions of solc (Solidity compiler)
+solc-select install all  # install all possible versions of solc 
+solc-select use 0.4.25   # example of using solc-select: set the version of solc to 0.4.25
+```
+
+
 ### Run SmartExecutor in Pycharm IDE:
 
 1, Create a project through Pycharm IDE by cloning https://github.com/contractAnalysis/smartExecutor.git.
 
 2, Create a virtual environment and install dependencies.
 
 3, Find semyth.py in the root directory and add the parameters. Take the example of Crowdsale.sol:
@@ -108,15 +116,15 @@
 For this reason, here show some useful documents of Mythril:
 
 - [Instructions for using Mythril](https://mythril-classic.readthedocs.io/en/master/)
 - [Mythril's documentation](https://mythril-classic.readthedocs.io/en/develop/)
 - [Vulnerability Remediation](https://swcregistry.io/)
 -->
 If you find this tool helpful, we would appreciate it if you could cite it. Here is the BibTex:
-```json
+```text
 @INPROCEEDINGS{10316942,
   author={Wei, Qiping and Sikder, Fadul and Feng, Huadong and Lei, Yu and Kacker, Raghu and Kuhn, Richard},
   booktitle={2023 5th Conference on Blockchain Research & Applications for Innovative Networks and Services (BRAINS)}, 
   title={SmartExecutor: Coverage-Driven Symbolic Execution Guided by a Function Dependency Graph}, 
   year={2023},
   volume={},
   number={},
```

### Comparing `smartExecutorx-4.0.0/smartExecutorx.egg-info/SOURCES.txt` & `smartExecutorx-4.1/smartExecutorx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/disassembler/asm.py` & `smartExecutorx-4.1/tests/disassembler/asm.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/disassembler/disassembly.py` & `smartExecutorx-4.1/tests/disassembler/disassembly.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/berlin_fork_opcodes_test.py` & `smartExecutorx-4.1/tests/instructions/berlin_fork_opcodes_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/codecopy_test.py` & `smartExecutorx-4.1/tests/instructions/codecopy_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/create2_test.py` & `smartExecutorx-4.1/tests/instructions/create2_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/create_test.py` & `smartExecutorx-4.1/tests/instructions/create_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/extcodecopy_test.py` & `smartExecutorx-4.1/tests/instructions/extcodecopy_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/extcodehash_test.py` & `smartExecutorx-4.1/tests/instructions/extcodehash_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/sar_test.py` & `smartExecutorx-4.1/tests/instructions/sar_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/shl_test.py` & `smartExecutorx-4.1/tests/instructions/shl_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/shr_test.py` & `smartExecutorx-4.1/tests/instructions/shr_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/static_call_test.py` & `smartExecutorx-4.1/tests/instructions/static_call_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/instructions/test_basefee.py` & `smartExecutorx-4.1/tests/instructions/test_basefee.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/keccak_tests.py` & `smartExecutorx-4.1/tests/laser/keccak_tests.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/smt/independece_solver_test.py` & `smartExecutorx-4.1/tests/laser/smt/independece_solver_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/smt/model_test.py` & `smartExecutorx-4.1/tests/laser/smt/model_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/state/calldata_test.py` & `smartExecutorx-4.1/tests/laser/state/calldata_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/state/mstack_test.py` & `smartExecutorx-4.1/tests/laser/state/mstack_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/state/mstate_test.py` & `smartExecutorx-4.1/tests/laser/state/mstate_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/state/storage_test.py` & `smartExecutorx-4.1/tests/laser/state/storage_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/state/world_state_account_exist_load_test.py` & `smartExecutorx-4.1/tests/laser/state/world_state_account_exist_load_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/test_transaction.py` & `smartExecutorx-4.1/tests/laser/test_transaction.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/transaction/create_transaction_test.py` & `smartExecutorx-4.1/tests/laser/transaction/create_transaction_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-4.0.0/tests/laser/transaction/symbolic_test.py` & `smartExecutorx-4.1/tests/laser/transaction/symbolic_test.py`

 * *Files identical despite different names*

