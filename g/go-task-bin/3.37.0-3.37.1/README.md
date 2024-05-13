# Comparing `tmp/go_task_bin-3.37.0.tar.gz` & `tmp/go_task_bin-3.37.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_task_bin-3.37.0.tar", last modified: Thu May  9 01:41:37 2024, max compression
+gzip compressed data, was "go_task_bin-3.37.1.tar", last modified: Fri May 10 01:21:21 2024, max compression
```

## Comparing `go_task_bin-3.37.0.tar` & `go_task_bin-3.37.1.tar`

### file list

```diff
@@ -1,414 +1,414 @@
--rw-r--r--   0        0        0     1074 2024-05-09 01:39:37.449707 go_task_bin-3.37.0/LICENSE
--rw-r--r--   0        0        0     1031 2024-05-09 01:39:37.449707 go_task_bin-3.37.0/README.md
--rw-r--r--   0        0        0        0 2024-05-09 01:39:37.449707 go_task_bin-3.37.0/go_task_bin/__init__.py
--rw-r--r--   0        0        0     1384 2024-05-09 01:39:37.449707 go_task_bin-3.37.0/pdm_build.py
--rw-r--r--   0        0        0     1245 2024-05-09 01:41:37.154029 go_task_bin-3.37.0/pyproject.toml
--rw-r--r--   0        0        0      231 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.editorconfig
--rw-r--r--   0        0        0       37 2024-05-09 01:39:39.317712 go_task_bin-3.37.0/task/.git
--rw-r--r--   0        0        0       12 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.gitattributes
--rw-r--r--   0        0        0     3217 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      521 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       88 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/FUNDING.yml
--rw-r--r--   0        0        0      387 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      552 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      368 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      462 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/dependabot.yml
--rw-r--r--   0        0        0      225 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/pull_request_template.md
--rw-r--r--   0        0        0     1463 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/issue-awaiting-response.yml
--rw-r--r--   0        0        0      838 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/issue-closed.yml
--rw-r--r--   0        0        0     6565 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/issue-experiment.yml
--rw-r--r--   0        0        0      813 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/issue-needs-triage.yml
--rw-r--r--   0        0        0      865 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/lint.yml
--rw-r--r--   0        0        0      476 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/release.yml
--rw-r--r--   0        0        0      872 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/test.yml
--rw-r--r--   0        0        0      922 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/upload-source-documents.yml
--rw-r--r--   0        0        0      468 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.gitignore
--rw-r--r--   0        0        0      382 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.golangci.yml
--rw-r--r--   0        0        0     3037 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.goreleaser.yml
--rw-r--r--   0        0        0       77 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.mockery.yaml
--rw-r--r--   0        0        0        8 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.nvmrc
--rw-r--r--   0        0        0      125 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.prettierrc.yml
--rw-r--r--   0        0        0      324 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.vscode/settings-sample.json
--rw-r--r--   0        0        0    38766 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/CHANGELOG.md
--rw-r--r--   0        0        0     1080 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/LICENSE
--rw-r--r--   0        0        0      634 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/README.md
--rw-r--r--   0        0        0     2948 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/Taskfile.yml
--rw-r--r--   0        0        0      586 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/args/args.go
--rw-r--r--   0        0        0     2393 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/args/args_test.go
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/bin/.keep
--rw-r--r--   0        0        0     3288 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/cmd/release/main.go
--rw-r--r--   0        0        0     4874 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/cmd/sleepit/sleepit.go
--rw-r--r--   0        0        0     4694 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/cmd/task/task.go
--rw-r--r--   0        0        0     1329 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/completion/bash/task.bash
--rw-r--r--   0        0        0     2342 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/completion/fish/task.fish
--rw-r--r--   0        0        0     1992 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/completion/ps/task.ps1
--rwxr-xr-x   0        0        0     2466 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/completion/zsh/_task
--rw-r--r--   0        0        0      436 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/concurrency.go
--rw-r--r--   0        0        0     1612 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/errors/errors.go
--rw-r--r--   0        0        0     3645 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/errors/errors_task.go
--rw-r--r--   0        0        0     5111 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/errors/errors_taskfile.go
--rw-r--r--   0        0        0     1084 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/go.mod
--rw-r--r--   0        0        0     6204 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/go.sum
--rw-r--r--   0        0        0      445 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/hash.go
--rw-r--r--   0        0        0     5727 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/help.go
--rw-r--r--   0        0        0      770 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/init.go
--rwxr-xr-x   0        0        0     9634 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/install-task.sh
--rw-r--r--   0        0        0     5499 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/compiler/compiler.go
--rw-r--r--   0        0        0      380 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/compiler/env.go
--rw-r--r--   0        0        0     3621 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/deepcopy/deepcopy.go
--rw-r--r--   0        0        0      659 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/editors/output.go
--rw-r--r--   0        0        0      430 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/env/env.go
--rw-r--r--   0        0        0      287 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/execext/devnull.go
--rw-r--r--   0        0        0     3463 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/execext/exec.go
--rw-r--r--   0        0        0     1082 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/exp/maps.go
--rw-r--r--   0        0        0     2625 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/experiments/experiments.go
--rw-r--r--   0        0        0     1031 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/filepathext/filepathext.go
--rw-r--r--   0        0        0      518 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/checker.go
--rw-r--r--   0        0        0     1094 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/glob.go
--rw-r--r--   0        0        0      388 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources.go
--rw-r--r--   0        0        0     2791 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources_checksum.go
--rw-r--r--   0        0        0      396 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources_checksum_test.go
--rw-r--r--   0        0        0      459 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources_none.go
--rw-r--r--   0        0        0     3521 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources_timestamp.go
--rw-r--r--   0        0        0      890 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/status.go
--rw-r--r--   0        0        0     2938 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/task.go
--rw-r--r--   0        0        0     5500 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/task_test.go
--rw-r--r--   0        0        0     5815 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/flags/flags.go
--rw-r--r--   0        0        0     1191 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/goext/meta.go
--rw-r--r--   0        0        0      439 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/hash/hash.go
--rw-r--r--   0        0        0     4144 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/logger/logger.go
--rw-r--r--   0        0        0     6003 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/mocks/sources_checkable.go
--rw-r--r--   0        0        0     2592 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/mocks/status_checkable.go
--rw-r--r--   0        0        0     3805 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/omap/orderedmap.go
--rw-r--r--   0        0        0     2607 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/omap/orderedmap_test.go
--rw-r--r--   0        0        0     1058 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/group.go
--rw-r--r--   0        0        0      292 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/interleaved.go
--rw-r--r--   0        0        0     1075 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/output.go
--rw-r--r--   0        0        0     3496 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/output_test.go
--rw-r--r--   0        0        0     1359 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/prefixed.go
--rw-r--r--   0        0        0      286 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/slicesext/slicesext.go
--rw-r--r--   0        0        0     1063 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/sort/sorter.go
--rw-r--r--   0        0        0     1895 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/sort/sorter_test.go
--rw-r--r--   0        0        0     2531 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/summary/summary.go
--rw-r--r--   0        0        0     3636 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/summary/summary_test.go
--rw-r--r--   0        0        0      308 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/sysinfo/uid.go
--rw-r--r--   0        0        0      208 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/sysinfo/uid_win.go
--rw-r--r--   0        0        0     2122 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/templater/funcs.go
--rw-r--r--   0        0        0     3291 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/templater/templater.go
--rw-r--r--   0        0        0      165 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/term/term.go
--rw-r--r--   0        0        0      348 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/version/version.go
--rw-r--r--   0        0        0      924 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/package-lock.json
--rw-r--r--   0        0        0      807 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/package.json
--rw-r--r--   0        0        0      804 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/precondition.go
--rw-r--r--   0        0        0      679 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/requires.go
--rw-r--r--   0        0        0     5808 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/setup.go
--rw-r--r--   0        0        0      700 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/signals.go
--rw-r--r--   0        0        0     7605 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/signals_test.go
--rw-r--r--   0        0        0     1172 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/status.go
--rw-r--r--   0        0        0    13331 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/task.go
--rw-r--r--   0        0        0    62707 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/task_test.go
--rw-r--r--   0        0        0      185 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/call.go
--rw-r--r--   0        0        0     2490 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/cmd.go
--rw-r--r--   0        0        0      921 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/dep.go
--rw-r--r--   0        0        0     1156 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/for.go
--rw-r--r--   0        0        0      530 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/glob.go
--rw-r--r--   0        0        0     2729 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/graph.go
--rw-r--r--   0        0        0     2941 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/include.go
--rw-r--r--   0        0        0      247 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/location.go
--rw-r--r--   0        0        0     1373 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/output.go
--rw-r--r--   0        0        0     2431 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/platforms.go
--rw-r--r--   0        0        0     1522 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/platforms_test.go
--rw-r--r--   0        0        0     1150 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/precondition.go
--rw-r--r--   0        0        0      976 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/precondition_test.go
--rw-r--r--   0        0        0      318 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/requires.go
--rw-r--r--   0        0        0     5704 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/task.go
--rw-r--r--   0        0        0     2502 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/taskfile.go
--rw-r--r--   0        0        0     1887 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/taskfile_test.go
--rw-r--r--   0        0        0     4508 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/tasks.go
--rw-r--r--   0        0        0     3751 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/var.go
--rw-r--r--   0        0        0     1232 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/cache.go
--rw-r--r--   0        0        0     1011 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/dotenv.go
--rw-r--r--   0        0        0     2017 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node.go
--rw-r--r--   0        0        0      780 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node_base.go
--rw-r--r--   0        0        0     2752 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node_file.go
--rw-r--r--   0        0        0     2592 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node_http.go
--rw-r--r--   0        0        0     1444 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node_stdin.go
--rw-r--r--   0        0        0     7915 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/reader.go
--rw-r--r--   0        0        0     4843 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/taskfile.go
--rw-r--r--   0        0        0      243 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/alias/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/alias/Taskfile2.yml
--rw-r--r--   0        0        0      111 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/alias/alias-summary.txt
--rw-r--r--   0        0        0       90 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/alias/alias.txt
--rw-r--r--   0        0        0       21 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/checksum/.gitignore
--rw-r--r--   0        0        0      428 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/checksum/Taskfile.yml
--rw-r--r--   0        0        0       14 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/checksum/ignore_me.txt
--rw-r--r--   0        0        0       14 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/checksum/source.txt
--rw-r--r--   0        0        0      351 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/concurrency/Taskfile.yml
--rw-r--r--   0        0        0      104 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/cyclic/Taskfile.yml
--rw-r--r--   0        0        0      243 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/deferred/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/deps/.gitignore
--rw-r--r--   0        0        0      703 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/deps/Taskfile.yml
--rw-r--r--   0        0        0       72 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/dynamic_var/.gitignore
--rw-r--r--   0        0        0      649 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/dynamic_var/Taskfile.yml
--rw-r--r--   0        0        0      377 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/dynamic_var/subdirectory/Taskfile.yml
--rw-r--r--   0        0        0      136 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/dynamic_var_on_created_dir/Taskfile.yml
--rw-r--r--   0        0        0       90 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/explicit_doesnt_exist/Taskfile.yml
--rw-r--r--   0        0        0       88 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/explicit_exists/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/explicit_exists/exists/.keep
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/.gitignore
--rw-r--r--   0        0        0      168 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/default/Taskfile.yml
--rw-r--r--   0        0        0       31 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/env_var_in_path/.env.testing
--rw-r--r--   0        0        0      119 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/env_var_in_path/Taskfile.yml
--rw-r--r--   0        0        0      158 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/error_included_envs/Taskfile.yml
--rw-r--r--   0        0        0       23 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/include1/.env
--rw-r--r--   0        0        0       31 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/include1/Taskfile.yml
--rw-r--r--   0        0        0       23 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/include1/envs/.env
--rw-r--r--   0        0        0       31 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/local_env_in_path/.env.testing
--rw-r--r--   0        0        0      148 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/local_env_in_path/Taskfile.yml
--rw-r--r--   0        0        0       31 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/local_var_in_path/.env.testing
--rw-r--r--   0        0        0      195 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/local_var_in_path/Taskfile.yml
--rw-r--r--   0        0        0      131 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/missing_env/Taskfile.yml
--rw-r--r--   0        0        0        8 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv_task/default/.env
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv_task/default/.gitignore
--rw-r--r--   0        0        0      456 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv_task/default/Taskfile.yml
--rw-r--r--   0        0        0       63 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dry/Taskfile.yml
--rw-r--r--   0        0        0      121 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dry_checksum/Taskfile.yml
--rw-r--r--   0        0        0       13 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dry_checksum/source.txt
--rw-r--r--   0        0        0       32 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/empty_task/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/env/.gitignore
--rw-r--r--   0        0        0      499 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/env/Taskfile.yml
--rw-r--r--   0        0        0      101 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/error_code/Taskfile.yml
--rw-r--r--   0        0        0      280 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/evaluate_symlinks_in_paths/Taskfile.yaml
--rw-r--r--   0        0        0       19 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/evaluate_symlinks_in_paths/shared/b
--rw-r--r--   0        0        0       25 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/evaluate_symlinks_in_paths/shared/inner_shared/c
--rw-r--r--   0        0        0       12 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/evaluate_symlinks_in_paths/src/a
--rw-r--r--   0        0        0       89 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/exit_immediately/Taskfile.yml
--rw-r--r--   0        0        0       80 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/expand/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/.gitignore
--rw-r--r--   0        0        0       58 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/Taskfile.dist.yaml/Taskfile.dist.yaml
--rw-r--r--   0        0        0       58 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/Taskfile.dist.yml/Taskfile.dist.yml
--rw-r--r--   0        0        0       58 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/Taskfile.yaml/Taskfile.yaml
--rw-r--r--   0        0        0       58 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/Taskfile.yml/Taskfile.yml
--rw-r--r--   0        0        0     1635 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/cmds/Taskfile.yml
--rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/cmds/bar.txt
--rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/cmds/foo.txt
--rw-r--r--   0        0        0     1876 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/deps/Taskfile.yml
--rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/deps/bar.txt
--rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/deps/foo.txt
--rw-r--r--   0        0        0      295 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/force/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/generates/.gitignore
--rw-r--r--   0        0        0      986 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/generates/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/generates/sub/.keep
--rw-r--r--   0        0        0      262 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_errors/Taskfile.yml
--rw-r--r--   0        0        0       80 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/cmds/Taskfile.yml
--rw-r--r--   0        0        0      116 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/deps/Taskfile.yml
--rw-r--r--   0        0        0       94 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/includes/Taskfile.yml
--rw-r--r--   0        0        0       81 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/includes/inc.yml
--rw-r--r--   0        0        0      123 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/preconditions/Taskfile.yml
--rw-r--r--   0        0        0       66 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_signals/Taskfile.yml
--rw-r--r--   0        0        0      388 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars/Taskfile.yml
--rw-r--r--   0        0        0      229 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars/include/Taskfile.include1.yml
--rw-r--r--   0        0        0      229 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars/include/Taskfile.include2.yml
--rw-r--r--   0        0        0      229 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars/include/Taskfile.include3.yml
--rw-r--r--   0        0        0      266 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars_multi_level/Taskfile.yml
--rw-r--r--   0        0        0       97 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars_multi_level/bar/Taskfile.yml
--rw-r--r--   0        0        0       97 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars_multi_level/foo/Taskfile.yml
--rw-r--r--   0        0        0      130 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars_multi_level/lib/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/.gitignore
--rw-r--r--   0        0        0      768 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile.yml
--rw-r--r--   0        0        0       93 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile2.yml
--rw-r--r--   0        0        0       55 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile_darwin.yml
--rw-r--r--   0        0        0       55 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile_linux.yml
--rw-r--r--   0        0        0       55 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile_windows.yml
--rw-r--r--   0        0        0       95 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/included/Taskfile.yml
--rw-r--r--   0        0        0      225 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/module1/Taskfile.yml
--rw-r--r--   0        0        0      213 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/module2/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_call_root_task/.gitignore
--rw-r--r--   0        0        0      122 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_call_root_task/Taskfile.yml
--rw-r--r--   0        0        0       69 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_call_root_task/Taskfile2.yml
--rw-r--r--   0        0        0      173 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_cycle/Taskfile.yml
--rw-r--r--   0        0        0      109 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_cycle/one/Taskfile.yml
--rw-r--r--   0        0        0      109 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_cycle/one/two/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_deps/.gitignore
--rw-r--r--   0        0        0      110 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_deps/Taskfile.yml
--rw-r--r--   0        0        0      267 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_deps/Taskfile2.yml
--rw-r--r--   0        0        0        9 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_empty/.gitignore
--rw-r--r--   0        0        0       50 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_empty/Taskfile.yml
--rw-r--r--   0        0        0      125 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_empty/Taskfile2.yml
--rw-r--r--   0        0        0       51 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_incorrect/Taskfile.yml
--rw-r--r--   0        0        0       28 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_incorrect/incomplete.yml
--rw-r--r--   0        0        0      188 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_internal/Taskfile.yml
--rw-r--r--   0        0        0       70 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_internal/Taskfile2.yml
--rw-r--r--   0        0        0      101 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_interpolation/include/Taskfile.yml
--rw-r--r--   0        0        0      155 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_interpolation/include_with_dir/Taskfile.yml
--rw-r--r--   0        0        0       83 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_interpolation/include_with_env_variable/Taskfile.yml
--rw-r--r--   0        0        0       66 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_interpolation/included/Taskfile.yml
--rw-r--r--   0        0        0      161 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/Taskfile.yml
--rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/called_one.txt
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/called_three.txt
--rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/called_two.txt
--rw-r--r--   0        0        0       85 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/one/Taskfile.yml
--rw-r--r--   0        0        0      101 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/one/two/Taskfile.yml
--rw-r--r--   0        0        0       62 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/one/two/three/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_optional/.gitignore
--rw-r--r--   0        0        0      162 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_optional/Taskfile.yml
--rw-r--r--   0        0        0      149 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_optional_explicit_false/Taskfile.yml
--rw-r--r--   0        0        0      115 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_optional_implicit_false/Taskfile.yml
--rw-r--r--   0        0        0      133 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_rel_path/Taskfile.yml
--rw-r--r--   0        0        0       32 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_rel_path/common/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_rel_path/included/Taskfile.yml
--rw-r--r--   0        0        0      129 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_shadowed_default/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_shadowed_default/Taskfile2.yml
--rw-r--r--   0        0        0        9 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_shadowed_default/file.txt
--rw-r--r--   0        0        0       64 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_unshadowed_default/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_unshadowed_default/Taskfile2.yml
--rw-r--r--   0        0        0        9 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_unshadowed_default/file.txt
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_yaml/.gitignore
--rw-r--r--   0        0        0      226 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_yaml/Custom.ext
--rw-r--r--   0        0        0      115 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_yaml/included/Taskfile.yaml
--rw-r--r--   0        0        0      109 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_yaml/included/custom.yaml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/init/.gitignore
--rw-r--r--   0        0        0      167 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/internal_task/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_list/Taskfile.yml
--rw-r--r--   0        0        0       76 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_status/Taskfile.yml
--rw-r--r--   0        0        0      104 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_summary/Taskfile.yml
--rw-r--r--   0        0        0       82 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_uptodate/Taskfile.yml
--rw-r--r--   0        0        0      105 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_var/Taskfile.yml
--rw-r--r--   0        0        0       90 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/list_desc_interpolation/Taskfile.yml
--rw-r--r--   0        0        0      164 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/list_mixed_desc/Taskfile.yml
--rw-r--r--   0        0        0      199 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/output_group/Taskfile.yml
--rw-r--r--   0        0        0      255 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/output_group_error_only/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/params/.gitignore
--rw-r--r--   0        0        0     1255 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/params/Taskfile.yml
--rw-r--r--   0        0        0     1584 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/platforms/Taskfile.yml
--rw-r--r--   0        0        0      285 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/precondition/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/precondition/foo.txt
--rw-r--r--   0        0        0      226 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/prompt/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/run/.gitignore
--rw-r--r--   0        0        0      468 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/run/Taskfile.yml
--rw-r--r--   0        0        0      201 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/shopts/command_level/Taskfile.yml
--rw-r--r--   0        0        0      175 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/shopts/global_level/Taskfile.yml
--rw-r--r--   0        0        0      183 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/shopts/task_level/Taskfile.yml
--rw-r--r--   0        0        0      174 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/short_task_notation/Taskfile.yml
--rw-r--r--   0        0        0     1350 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/silent/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/single_cmd_dep/.gitignore
--rw-r--r--   0        0        0       99 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/single_cmd_dep/Taskfile.yml
--rw-r--r--   0        0        0      282 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/special_vars/Taskfile.yml
--rw-r--r--   0        0        0      214 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/special_vars/included/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/special_vars/subdir/.gitkeep
--rw-r--r--   0        0        0       92 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/split_args/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status/.gitignore
--rw-r--r--   0        0        0      331 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status/Taskfile.yml
--rw-r--r--   0        0        0       14 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status_vars/.gitignore
--rw-r--r--   0        0        0      170 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status_vars/Taskfile.yml
--rw-r--r--   0        0        0       14 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status_vars/source.txt
--rw-r--r--   0        0        0      566 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/summary/Taskfile.yml
--rw-r--r--   0        0        0      346 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/summary/task-with-summary.txt
--rw-r--r--   0        0        0       78 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/taskfile_walk/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/taskfile_walk/foo/bar/.gitkeep
--rw-r--r--   0        0        0       96 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/user_working_dir/Taskfile.yml
--rw-r--r--   0        0        0       74 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/user_working_dir_with_includes/Taskfile.yml
--rw-r--r--   0        0        0      101 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/user_working_dir_with_includes/included/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/user_working_dir_with_includes/somedir/.keep
--rw-r--r--   0        0        0       27 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/.env
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/.gitignore
--rw-r--r--   0        0        0     1008 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/Taskfile.yml
--rw-r--r--   0        0        0     2188 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/any/Taskfile.yml
--rw-r--r--   0        0        0     2791 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/any2/Taskfile.yml
--rw-r--r--   0        0        0      276 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/any2/example.json
--rw-r--r--   0        0        0      111 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/any2/example.yaml
--rw-r--r--   0        0        0       93 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/version/v1/Taskfile.yml
--rw-r--r--   0        0        0       93 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/version/v2/Taskfile.yml
--rw-r--r--   0        0        0       93 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/version/v3/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/watcher_interval/.gitignore
--rw-r--r--   0        0        0      194 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/watcher_interval/Taskfile.yaml
--rw-r--r--   0        0        0      519 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/wildcards/Taskfile.yml
--rw-r--r--   0        0        0     9281 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/variables.go
--rw-r--r--   0        0        0     4215 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/watch.go
--rw-r--r--   0        0        0     2041 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/watch_test.go
--rw-r--r--   0        0        0      238 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/.gitignore
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/.nojekyll
--rw-r--r--   0        0        0     1523 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/Taskfile.yml
--rw-r--r--   0        0        0       70 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/babel.config.ts
--rw-r--r--   0        0        0     6841 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/blog/2023-09-02-introducing-experiments.mdx
--rw-r--r--   0        0        0     4459 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/blog/2024-04-09-variables.mdx
--rw-r--r--   0        0        0      279 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/blog/authors.yml
--rw-r--r--   0        0        0      242 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/constants.ts
--rw-r--r--   0        0        0      359 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/crowdin.yml
--rw-r--r--   0        0        0    41801 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/api_reference.mdx
--rw-r--r--   0        0        0    38814 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/changelog.mdx
--rw-r--r--   0        0        0     1529 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/community.mdx
--rw-r--r--   0        0        0     7804 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/contributing.mdx
--rw-r--r--   0        0        0      711 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/deprecations/deprecations.mdx
--rw-r--r--   0        0        0      655 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/deprecations/template.mdx
--rw-r--r--   0        0        0     1245 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/deprecations/version_2_schema.mdx
--rw-r--r--   0        0        0     5677 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/experiments.mdx
--rw-r--r--   0        0        0     1540 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/gentle_force.mdx
--rw-r--r--   0        0        0     7895 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/map_variables.mdx
--rw-r--r--   0        0        0     4706 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/remote_taskfiles.mdx
--rw-r--r--   0        0        0     1128 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/template.mdx
--rw-r--r--   0        0        0     2583 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/faq.mdx
--rw-r--r--   0        0        0     6930 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/installation.mdx
--rw-r--r--   0        0        0     2911 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/integrations.mdx
--rw-r--r--   0        0        0     1993 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/intro.mdx
--rw-r--r--   0        0        0     2797 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/releasing.mdx
--rw-r--r--   0        0        0     2974 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/styleguide.mdx
--rw-r--r--   0        0        0     5473 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/taskfile_versions.mdx
--rw-r--r--   0        0        0      763 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/translate.mdx
--rw-r--r--   0        0        0    46204 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/usage.mdx
--rw-r--r--   0        0        0     5155 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docusaurus.config.ts
--rw-r--r--   0        0        0     1508 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/package.json
--rw-r--r--   0        0        0      208 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/prettier.config.js
--rw-r--r--   0        0        0      271 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/sidebars.ts
--rw-r--r--   0        0        0     1050 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/api/crowdin.js
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/components/.keep
--rw-r--r--   0        0        0     1202 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/css/carbon.css
--rw-r--r--   0        0        0     3089 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/css/custom.css
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/pages/.keep
--rw-r--r--   0        0        0     1922 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/pages/donate.md
--rw-r--r--   0        0        0     1342 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/themes/prismDark.js
--rw-r--r--   0        0        0     1679 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/themes/prismLight.js
--rw-r--r--   0        0        0        0 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/.nojekyll
--rw-r--r--   0        0        0       13 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/CNAME
--rw-r--r--   0        0        0      109 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/Taskfile.yml
--rw-r--r--   0        0        0     7281 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/appwrite.svg
--rw-r--r--   0        0        0   173915 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/favicon.ico
--rw-r--r--   0        0        0     1321 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/icon-discord.svg
--rw-r--r--   0        0        0     1227 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/icon-github.svg
--rw-r--r--   0        0        0     1717 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/icon-mastodon.svg
--rw-r--r--   0        0        0     1742 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/icon-twitter.svg
--rw-r--r--   0        0        0    13524 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/logo.png
--rw-r--r--   0        0        0      435 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/logo.svg
--rw-r--r--   0        0        0      360 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/logo_mono.svg
--rw-r--r--   0        0        0    19847 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/og-image.png
--rw-r--r--   0        0        0     1276 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/pix.png
--rwxr-xr-x   0        0        0     9634 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/install.sh
--rw-r--r--   0        0        0      784 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/js/carbon.js
--rw-r--r--   0        0        0    22415 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/static/schema.json
--rw-r--r--   0        0        0       87 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/tsconfig.json
--rw-r--r--   0        0        0    41801 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/api_reference.mdx
--rw-r--r--   0        0        0    38814 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/changelog.mdx
--rw-r--r--   0        0        0     1529 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/community.mdx
--rw-r--r--   0        0        0     7804 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/contributing.mdx
--rw-r--r--   0        0        0      711 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx
--rw-r--r--   0        0        0      655 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/template.mdx
--rw-r--r--   0        0        0     1245 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx
--rw-r--r--   0        0        0     5677 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/experiments.mdx
--rw-r--r--   0        0        0     1540 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx
--rw-r--r--   0        0        0     7895 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/map_variables.mdx
--rw-r--r--   0        0        0     4706 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx
--rw-r--r--   0        0        0     1128 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/template.mdx
--rw-r--r--   0        0        0     2583 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/faq.mdx
--rw-r--r--   0        0        0     6930 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/installation.mdx
--rw-r--r--   0        0        0     2911 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/integrations.mdx
--rw-r--r--   0        0        0     1993 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/intro.mdx
--rw-r--r--   0        0        0     2797 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/releasing.mdx
--rw-r--r--   0        0        0     2974 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/styleguide.mdx
--rw-r--r--   0        0        0     5473 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/taskfile_versions.mdx
--rw-r--r--   0        0        0      763 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/translate.mdx
--rw-r--r--   0        0        0    46204 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/usage.mdx
--rw-r--r--   0        0        0      174 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_sidebars/version-latest-sidebars.json
--rw-r--r--   0        0        0       15 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versions.json
--rw-r--r--   0        0        0   364377 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/yarn.lock
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 go_task_bin-3.37.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-10 01:19:19.558563 go_task_bin-3.37.1/LICENSE
+-rw-r--r--   0        0        0     1031 2024-05-10 01:19:19.558563 go_task_bin-3.37.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:19.558563 go_task_bin-3.37.1/go_task_bin/__init__.py
+-rw-r--r--   0        0        0     1384 2024-05-10 01:19:19.558563 go_task_bin-3.37.1/pdm_build.py
+-rw-r--r--   0        0        0     1245 2024-05-10 01:21:21.270779 go_task_bin-3.37.1/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.editorconfig
+-rw-r--r--   0        0        0       37 2024-05-10 01:19:21.442567 go_task_bin-3.37.1/task/.git
+-rw-r--r--   0        0        0       12 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.gitattributes
+-rw-r--r--   0        0        0     3217 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      521 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       88 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/FUNDING.yml
+-rw-r--r--   0        0        0      387 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      552 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      368 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      462 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/dependabot.yml
+-rw-r--r--   0        0        0      225 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1463 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/workflows/issue-awaiting-response.yml
+-rw-r--r--   0        0        0      838 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/workflows/issue-closed.yml
+-rw-r--r--   0        0        0     6565 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/workflows/issue-experiment.yml
+-rw-r--r--   0        0        0      813 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/workflows/issue-needs-triage.yml
+-rw-r--r--   0        0        0      865 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      476 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/workflows/release.yml
+-rw-r--r--   0        0        0      872 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/workflows/test.yml
+-rw-r--r--   0        0        0      922 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.github/workflows/upload-source-documents.yml
+-rw-r--r--   0        0        0      468 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.gitignore
+-rw-r--r--   0        0        0      382 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.golangci.yml
+-rw-r--r--   0        0        0     3040 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.goreleaser.yml
+-rw-r--r--   0        0        0       77 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.mockery.yaml
+-rw-r--r--   0        0        0        8 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.nvmrc
+-rw-r--r--   0        0        0      125 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.prettierrc.yml
+-rw-r--r--   0        0        0      324 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/.vscode/settings-sample.json
+-rw-r--r--   0        0        0    38940 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/CHANGELOG.md
+-rw-r--r--   0        0        0     1080 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/LICENSE
+-rw-r--r--   0        0        0      634 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/README.md
+-rw-r--r--   0        0        0     2948 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/Taskfile.yml
+-rw-r--r--   0        0        0      586 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/args/args.go
+-rw-r--r--   0        0        0     2393 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/args/args_test.go
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/bin/.keep
+-rw-r--r--   0        0        0     3288 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/cmd/release/main.go
+-rw-r--r--   0        0        0     4874 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/cmd/sleepit/sleepit.go
+-rw-r--r--   0        0        0     4694 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/cmd/task/task.go
+-rw-r--r--   0        0        0     1329 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/completion/bash/task.bash
+-rw-r--r--   0        0        0     2342 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/completion/fish/task.fish
+-rw-r--r--   0        0        0     1992 2024-05-10 01:19:21.450567 go_task_bin-3.37.1/task/completion/ps/task.ps1
+-rwxr-xr-x   0        0        0     2466 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/completion/zsh/_task
+-rw-r--r--   0        0        0      436 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/concurrency.go
+-rw-r--r--   0        0        0     1612 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/errors/errors.go
+-rw-r--r--   0        0        0     3645 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/errors/errors_task.go
+-rw-r--r--   0        0        0     5111 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/errors/errors_taskfile.go
+-rw-r--r--   0        0        0     1084 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/go.mod
+-rw-r--r--   0        0        0     6204 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/go.sum
+-rw-r--r--   0        0        0      445 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/hash.go
+-rw-r--r--   0        0        0     5727 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/help.go
+-rw-r--r--   0        0        0      770 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/init.go
+-rwxr-xr-x   0        0        0     9634 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/install-task.sh
+-rw-r--r--   0        0        0     5499 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/compiler/compiler.go
+-rw-r--r--   0        0        0      380 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/compiler/env.go
+-rw-r--r--   0        0        0     3621 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/deepcopy/deepcopy.go
+-rw-r--r--   0        0        0      659 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/editors/output.go
+-rw-r--r--   0        0        0      544 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/env/env.go
+-rw-r--r--   0        0        0      287 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/execext/devnull.go
+-rw-r--r--   0        0        0     3463 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/execext/exec.go
+-rw-r--r--   0        0        0     1082 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/exp/maps.go
+-rw-r--r--   0        0        0     2625 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/experiments/experiments.go
+-rw-r--r--   0        0        0     1031 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/filepathext/filepathext.go
+-rw-r--r--   0        0        0      518 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/checker.go
+-rw-r--r--   0        0        0     1094 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/glob.go
+-rw-r--r--   0        0        0      388 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/sources.go
+-rw-r--r--   0        0        0     2791 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/sources_checksum.go
+-rw-r--r--   0        0        0      396 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/sources_checksum_test.go
+-rw-r--r--   0        0        0      459 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/sources_none.go
+-rw-r--r--   0        0        0     3521 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/sources_timestamp.go
+-rw-r--r--   0        0        0      890 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/status.go
+-rw-r--r--   0        0        0     2938 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/task.go
+-rw-r--r--   0        0        0     5500 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/fingerprint/task_test.go
+-rw-r--r--   0        0        0     5815 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/flags/flags.go
+-rw-r--r--   0        0        0     1191 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/goext/meta.go
+-rw-r--r--   0        0        0      439 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/hash/hash.go
+-rw-r--r--   0        0        0     4144 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/logger/logger.go
+-rw-r--r--   0        0        0     6003 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/mocks/sources_checkable.go
+-rw-r--r--   0        0        0     2592 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/mocks/status_checkable.go
+-rw-r--r--   0        0        0     3805 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/omap/orderedmap.go
+-rw-r--r--   0        0        0     2607 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/omap/orderedmap_test.go
+-rw-r--r--   0        0        0     1058 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/output/group.go
+-rw-r--r--   0        0        0      292 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/output/interleaved.go
+-rw-r--r--   0        0        0     1075 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/output/output.go
+-rw-r--r--   0        0        0     3496 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/output/output_test.go
+-rw-r--r--   0        0        0     1359 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/output/prefixed.go
+-rw-r--r--   0        0        0      286 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/slicesext/slicesext.go
+-rw-r--r--   0        0        0     1063 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/sort/sorter.go
+-rw-r--r--   0        0        0     1895 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/sort/sorter_test.go
+-rw-r--r--   0        0        0     2531 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/summary/summary.go
+-rw-r--r--   0        0        0     3636 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/summary/summary_test.go
+-rw-r--r--   0        0        0      308 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/sysinfo/uid.go
+-rw-r--r--   0        0        0      208 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/sysinfo/uid_win.go
+-rw-r--r--   0        0        0     2122 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/templater/funcs.go
+-rw-r--r--   0        0        0     3291 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/templater/templater.go
+-rw-r--r--   0        0        0      165 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/term/term.go
+-rw-r--r--   0        0        0      348 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/internal/version/version.go
+-rw-r--r--   0        0        0      924 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/package-lock.json
+-rw-r--r--   0        0        0      807 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/package.json
+-rw-r--r--   0        0        0      804 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/precondition.go
+-rw-r--r--   0        0        0      679 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/requires.go
+-rw-r--r--   0        0        0     5808 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/setup.go
+-rw-r--r--   0        0        0      700 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/signals.go
+-rw-r--r--   0        0        0     7605 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/signals_test.go
+-rw-r--r--   0        0        0     1172 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/status.go
+-rw-r--r--   0        0        0    13331 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/task.go
+-rw-r--r--   0        0        0    62779 2024-05-10 01:19:21.454567 go_task_bin-3.37.1/task/task_test.go
+-rw-r--r--   0        0        0      185 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/call.go
+-rw-r--r--   0        0        0     2490 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/cmd.go
+-rw-r--r--   0        0        0      921 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/dep.go
+-rw-r--r--   0        0        0     1156 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/for.go
+-rw-r--r--   0        0        0      530 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/glob.go
+-rw-r--r--   0        0        0     2729 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/graph.go
+-rw-r--r--   0        0        0     2941 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/include.go
+-rw-r--r--   0        0        0      247 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/location.go
+-rw-r--r--   0        0        0     1373 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/output.go
+-rw-r--r--   0        0        0     2431 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/platforms.go
+-rw-r--r--   0        0        0     1522 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/platforms_test.go
+-rw-r--r--   0        0        0     1150 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/precondition.go
+-rw-r--r--   0        0        0      976 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/precondition_test.go
+-rw-r--r--   0        0        0      318 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/requires.go
+-rw-r--r--   0        0        0     5704 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/task.go
+-rw-r--r--   0        0        0     2502 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/taskfile.go
+-rw-r--r--   0        0        0     1887 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/taskfile_test.go
+-rw-r--r--   0        0        0     4508 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/tasks.go
+-rw-r--r--   0        0        0     3751 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/ast/var.go
+-rw-r--r--   0        0        0     1232 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/cache.go
+-rw-r--r--   0        0        0     1011 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/dotenv.go
+-rw-r--r--   0        0        0     2017 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/node.go
+-rw-r--r--   0        0        0      780 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/node_base.go
+-rw-r--r--   0        0        0     2752 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/node_file.go
+-rw-r--r--   0        0        0     2592 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/node_http.go
+-rw-r--r--   0        0        0     1444 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/node_stdin.go
+-rw-r--r--   0        0        0     7915 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/reader.go
+-rw-r--r--   0        0        0     4843 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/taskfile/taskfile.go
+-rw-r--r--   0        0        0      243 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/alias/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/alias/Taskfile2.yml
+-rw-r--r--   0        0        0      111 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/alias/alias-summary.txt
+-rw-r--r--   0        0        0       90 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/alias/alias.txt
+-rw-r--r--   0        0        0       21 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/checksum/.gitignore
+-rw-r--r--   0        0        0      428 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/checksum/Taskfile.yml
+-rw-r--r--   0        0        0       14 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/checksum/ignore_me.txt
+-rw-r--r--   0        0        0       14 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/checksum/source.txt
+-rw-r--r--   0        0        0      351 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/concurrency/Taskfile.yml
+-rw-r--r--   0        0        0      104 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/cyclic/Taskfile.yml
+-rw-r--r--   0        0        0      243 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/deferred/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/deps/.gitignore
+-rw-r--r--   0        0        0      703 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/deps/Taskfile.yml
+-rw-r--r--   0        0        0       72 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dir/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dir/dynamic_var/.gitignore
+-rw-r--r--   0        0        0      649 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dir/dynamic_var/Taskfile.yml
+-rw-r--r--   0        0        0      377 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dir/dynamic_var/subdirectory/Taskfile.yml
+-rw-r--r--   0        0        0      136 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dir/dynamic_var_on_created_dir/Taskfile.yml
+-rw-r--r--   0        0        0       90 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dir/explicit_doesnt_exist/Taskfile.yml
+-rw-r--r--   0        0        0       88 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dir/explicit_exists/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dir/explicit_exists/exists/.keep
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/.gitignore
+-rw-r--r--   0        0        0      168 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/default/Taskfile.yml
+-rw-r--r--   0        0        0       31 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/env_var_in_path/.env.testing
+-rw-r--r--   0        0        0      119 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/env_var_in_path/Taskfile.yml
+-rw-r--r--   0        0        0      158 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/error_included_envs/Taskfile.yml
+-rw-r--r--   0        0        0       23 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/include1/.env
+-rw-r--r--   0        0        0       31 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/include1/Taskfile.yml
+-rw-r--r--   0        0        0       23 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/include1/envs/.env
+-rw-r--r--   0        0        0       31 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/local_env_in_path/.env.testing
+-rw-r--r--   0        0        0      148 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/local_env_in_path/Taskfile.yml
+-rw-r--r--   0        0        0       31 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/local_var_in_path/.env.testing
+-rw-r--r--   0        0        0      195 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/local_var_in_path/Taskfile.yml
+-rw-r--r--   0        0        0      131 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv/missing_env/Taskfile.yml
+-rw-r--r--   0        0        0        8 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv_task/default/.env
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv_task/default/.gitignore
+-rw-r--r--   0        0        0      456 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dotenv_task/default/Taskfile.yml
+-rw-r--r--   0        0        0       63 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dry/Taskfile.yml
+-rw-r--r--   0        0        0      121 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dry_checksum/Taskfile.yml
+-rw-r--r--   0        0        0       13 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/dry_checksum/source.txt
+-rw-r--r--   0        0        0       32 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/empty_task/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/env/.gitignore
+-rw-r--r--   0        0        0      676 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/env/Taskfile.yml
+-rw-r--r--   0        0        0      101 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/error_code/Taskfile.yml
+-rw-r--r--   0        0        0      280 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/evaluate_symlinks_in_paths/Taskfile.yaml
+-rw-r--r--   0        0        0       19 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/evaluate_symlinks_in_paths/shared/b
+-rw-r--r--   0        0        0       25 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/evaluate_symlinks_in_paths/shared/inner_shared/c
+-rw-r--r--   0        0        0       12 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/evaluate_symlinks_in_paths/src/a
+-rw-r--r--   0        0        0       89 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/exit_immediately/Taskfile.yml
+-rw-r--r--   0        0        0       80 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/expand/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/file_names/.gitignore
+-rw-r--r--   0        0        0       58 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/file_names/Taskfile.dist.yaml/Taskfile.dist.yaml
+-rw-r--r--   0        0        0       58 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/file_names/Taskfile.dist.yml/Taskfile.dist.yml
+-rw-r--r--   0        0        0       58 2024-05-10 01:19:21.458567 go_task_bin-3.37.1/task/testdata/file_names/Taskfile.yaml/Taskfile.yaml
+-rw-r--r--   0        0        0       58 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/file_names/Taskfile.yml/Taskfile.yml
+-rw-r--r--   0        0        0     1635 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/for/cmds/Taskfile.yml
+-rw-r--r--   0        0        0        4 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/for/cmds/bar.txt
+-rw-r--r--   0        0        0        4 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/for/cmds/foo.txt
+-rw-r--r--   0        0        0     1876 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/for/deps/Taskfile.yml
+-rw-r--r--   0        0        0        4 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/for/deps/bar.txt
+-rw-r--r--   0        0        0        4 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/for/deps/foo.txt
+-rw-r--r--   0        0        0      295 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/force/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/generates/.gitignore
+-rw-r--r--   0        0        0      986 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/generates/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/generates/sub/.keep
+-rw-r--r--   0        0        0      262 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/ignore_errors/Taskfile.yml
+-rw-r--r--   0        0        0       80 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/ignore_nil_elements/cmds/Taskfile.yml
+-rw-r--r--   0        0        0      116 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/ignore_nil_elements/deps/Taskfile.yml
+-rw-r--r--   0        0        0       94 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/ignore_nil_elements/includes/Taskfile.yml
+-rw-r--r--   0        0        0       81 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/ignore_nil_elements/includes/inc.yml
+-rw-r--r--   0        0        0      123 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/ignore_nil_elements/preconditions/Taskfile.yml
+-rw-r--r--   0        0        0       66 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/ignore_signals/Taskfile.yml
+-rw-r--r--   0        0        0      388 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/include_with_vars/Taskfile.yml
+-rw-r--r--   0        0        0      229 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/include_with_vars/include/Taskfile.include1.yml
+-rw-r--r--   0        0        0      229 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/include_with_vars/include/Taskfile.include2.yml
+-rw-r--r--   0        0        0      229 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/include_with_vars/include/Taskfile.include3.yml
+-rw-r--r--   0        0        0      266 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/include_with_vars_multi_level/Taskfile.yml
+-rw-r--r--   0        0        0       97 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/include_with_vars_multi_level/bar/Taskfile.yml
+-rw-r--r--   0        0        0       97 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/include_with_vars_multi_level/foo/Taskfile.yml
+-rw-r--r--   0        0        0      130 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/include_with_vars_multi_level/lib/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes/.gitignore
+-rw-r--r--   0        0        0      768 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes/Taskfile.yml
+-rw-r--r--   0        0        0       93 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes/Taskfile2.yml
+-rw-r--r--   0        0        0       55 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes/Taskfile_darwin.yml
+-rw-r--r--   0        0        0       55 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes/Taskfile_linux.yml
+-rw-r--r--   0        0        0       55 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes/Taskfile_windows.yml
+-rw-r--r--   0        0        0       95 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes/included/Taskfile.yml
+-rw-r--r--   0        0        0      225 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes/module1/Taskfile.yml
+-rw-r--r--   0        0        0      213 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes/module2/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_call_root_task/.gitignore
+-rw-r--r--   0        0        0      122 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_call_root_task/Taskfile.yml
+-rw-r--r--   0        0        0       69 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_call_root_task/Taskfile2.yml
+-rw-r--r--   0        0        0      173 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_cycle/Taskfile.yml
+-rw-r--r--   0        0        0      109 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_cycle/one/Taskfile.yml
+-rw-r--r--   0        0        0      109 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_cycle/one/two/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_deps/.gitignore
+-rw-r--r--   0        0        0      110 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_deps/Taskfile.yml
+-rw-r--r--   0        0        0      267 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_deps/Taskfile2.yml
+-rw-r--r--   0        0        0        9 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_empty/.gitignore
+-rw-r--r--   0        0        0       50 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_empty/Taskfile.yml
+-rw-r--r--   0        0        0      125 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_empty/Taskfile2.yml
+-rw-r--r--   0        0        0       51 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_incorrect/Taskfile.yml
+-rw-r--r--   0        0        0       28 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_incorrect/incomplete.yml
+-rw-r--r--   0        0        0      188 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_internal/Taskfile.yml
+-rw-r--r--   0        0        0       70 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_internal/Taskfile2.yml
+-rw-r--r--   0        0        0      101 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_interpolation/include/Taskfile.yml
+-rw-r--r--   0        0        0      155 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_interpolation/include_with_dir/Taskfile.yml
+-rw-r--r--   0        0        0       83 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_interpolation/include_with_env_variable/Taskfile.yml
+-rw-r--r--   0        0        0       66 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_interpolation/included/Taskfile.yml
+-rw-r--r--   0        0        0      161 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_multi_level/Taskfile.yml
+-rw-r--r--   0        0        0        4 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_multi_level/called_one.txt
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_multi_level/called_three.txt
+-rw-r--r--   0        0        0        4 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_multi_level/called_two.txt
+-rw-r--r--   0        0        0       85 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_multi_level/one/Taskfile.yml
+-rw-r--r--   0        0        0      101 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_multi_level/one/two/Taskfile.yml
+-rw-r--r--   0        0        0       62 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_multi_level/one/two/three/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_optional/.gitignore
+-rw-r--r--   0        0        0      162 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_optional/Taskfile.yml
+-rw-r--r--   0        0        0      149 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_optional_explicit_false/Taskfile.yml
+-rw-r--r--   0        0        0      115 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_optional_implicit_false/Taskfile.yml
+-rw-r--r--   0        0        0      133 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_rel_path/Taskfile.yml
+-rw-r--r--   0        0        0       32 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_rel_path/common/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_rel_path/included/Taskfile.yml
+-rw-r--r--   0        0        0      129 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_shadowed_default/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_shadowed_default/Taskfile2.yml
+-rw-r--r--   0        0        0        9 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_shadowed_default/file.txt
+-rw-r--r--   0        0        0       64 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_unshadowed_default/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_unshadowed_default/Taskfile2.yml
+-rw-r--r--   0        0        0        9 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_unshadowed_default/file.txt
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_yaml/.gitignore
+-rw-r--r--   0        0        0      226 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_yaml/Custom.ext
+-rw-r--r--   0        0        0      115 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_yaml/included/Taskfile.yaml
+-rw-r--r--   0        0        0      109 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/includes_yaml/included/custom.yaml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/init/.gitignore
+-rw-r--r--   0        0        0      167 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/internal_task/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-10 01:19:21.462567 go_task_bin-3.37.1/task/testdata/label_list/Taskfile.yml
+-rw-r--r--   0        0        0       76 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/label_status/Taskfile.yml
+-rw-r--r--   0        0        0      104 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/label_summary/Taskfile.yml
+-rw-r--r--   0        0        0       82 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/label_uptodate/Taskfile.yml
+-rw-r--r--   0        0        0      105 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/label_var/Taskfile.yml
+-rw-r--r--   0        0        0       90 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/list_desc_interpolation/Taskfile.yml
+-rw-r--r--   0        0        0      164 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/list_mixed_desc/Taskfile.yml
+-rw-r--r--   0        0        0      199 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/output_group/Taskfile.yml
+-rw-r--r--   0        0        0      255 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/output_group_error_only/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/params/.gitignore
+-rw-r--r--   0        0        0     1255 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/params/Taskfile.yml
+-rw-r--r--   0        0        0     1584 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/platforms/Taskfile.yml
+-rw-r--r--   0        0        0      285 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/precondition/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/precondition/foo.txt
+-rw-r--r--   0        0        0      226 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/prompt/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/run/.gitignore
+-rw-r--r--   0        0        0      468 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/run/Taskfile.yml
+-rw-r--r--   0        0        0      201 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/shopts/command_level/Taskfile.yml
+-rw-r--r--   0        0        0      175 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/shopts/global_level/Taskfile.yml
+-rw-r--r--   0        0        0      183 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/shopts/task_level/Taskfile.yml
+-rw-r--r--   0        0        0      174 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/short_task_notation/Taskfile.yml
+-rw-r--r--   0        0        0     1350 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/silent/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/single_cmd_dep/.gitignore
+-rw-r--r--   0        0        0       99 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/single_cmd_dep/Taskfile.yml
+-rw-r--r--   0        0        0      282 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/special_vars/Taskfile.yml
+-rw-r--r--   0        0        0      214 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/special_vars/included/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/special_vars/subdir/.gitkeep
+-rw-r--r--   0        0        0       92 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/split_args/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/status/.gitignore
+-rw-r--r--   0        0        0      331 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/status/Taskfile.yml
+-rw-r--r--   0        0        0       14 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/status_vars/.gitignore
+-rw-r--r--   0        0        0      170 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/status_vars/Taskfile.yml
+-rw-r--r--   0        0        0       14 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/status_vars/source.txt
+-rw-r--r--   0        0        0      566 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/summary/Taskfile.yml
+-rw-r--r--   0        0        0      346 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/summary/task-with-summary.txt
+-rw-r--r--   0        0        0       78 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/taskfile_walk/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/taskfile_walk/foo/bar/.gitkeep
+-rw-r--r--   0        0        0       96 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/user_working_dir/Taskfile.yml
+-rw-r--r--   0        0        0       74 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/user_working_dir_with_includes/Taskfile.yml
+-rw-r--r--   0        0        0      101 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/user_working_dir_with_includes/included/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/user_working_dir_with_includes/somedir/.keep
+-rw-r--r--   0        0        0       27 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/vars/.env
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/vars/.gitignore
+-rw-r--r--   0        0        0     1008 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/vars/Taskfile.yml
+-rw-r--r--   0        0        0     2188 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/vars/any/Taskfile.yml
+-rw-r--r--   0        0        0     2791 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/vars/any2/Taskfile.yml
+-rw-r--r--   0        0        0      276 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/vars/any2/example.json
+-rw-r--r--   0        0        0      111 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/vars/any2/example.yaml
+-rw-r--r--   0        0        0       93 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/version/v1/Taskfile.yml
+-rw-r--r--   0        0        0       93 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/version/v2/Taskfile.yml
+-rw-r--r--   0        0        0       93 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/version/v3/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/watcher_interval/.gitignore
+-rw-r--r--   0        0        0      194 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/watcher_interval/Taskfile.yaml
+-rw-r--r--   0        0        0      519 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/testdata/wildcards/Taskfile.yml
+-rw-r--r--   0        0        0     9281 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/variables.go
+-rw-r--r--   0        0        0     4215 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/watch.go
+-rw-r--r--   0        0        0     2041 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/watch_test.go
+-rw-r--r--   0        0        0      238 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/.nojekyll
+-rw-r--r--   0        0        0     1523 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/Taskfile.yml
+-rw-r--r--   0        0        0       70 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/babel.config.ts
+-rw-r--r--   0        0        0     6841 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/blog/2023-09-02-introducing-experiments.mdx
+-rw-r--r--   0        0        0     4447 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/blog/2024-05-09-any-variables.mdx
+-rw-r--r--   0        0        0      279 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/blog/authors.yml
+-rw-r--r--   0        0        0      242 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/constants.ts
+-rw-r--r--   0        0        0      359 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/crowdin.yml
+-rw-r--r--   0        0        0    41801 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/docs/api_reference.mdx
+-rw-r--r--   0        0        0    38988 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/docs/changelog.mdx
+-rw-r--r--   0        0        0     1529 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/docs/community.mdx
+-rw-r--r--   0        0        0     7804 2024-05-10 01:19:21.466567 go_task_bin-3.37.1/task/website/docs/contributing.mdx
+-rw-r--r--   0        0        0      711 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/deprecations/deprecations.mdx
+-rw-r--r--   0        0        0      655 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/deprecations/template.mdx
+-rw-r--r--   0        0        0     1245 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/deprecations/version_2_schema.mdx
+-rw-r--r--   0        0        0     5677 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/experiments/experiments.mdx
+-rw-r--r--   0        0        0     1540 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/experiments/gentle_force.mdx
+-rw-r--r--   0        0        0     7895 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/experiments/map_variables.mdx
+-rw-r--r--   0        0        0     4706 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/experiments/remote_taskfiles.mdx
+-rw-r--r--   0        0        0     1128 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/experiments/template.mdx
+-rw-r--r--   0        0        0     2583 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/faq.mdx
+-rw-r--r--   0        0        0     6930 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/installation.mdx
+-rw-r--r--   0        0        0     2911 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/integrations.mdx
+-rw-r--r--   0        0        0     1993 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/intro.mdx
+-rw-r--r--   0        0        0     2797 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/releasing.mdx
+-rw-r--r--   0        0        0     2974 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/styleguide.mdx
+-rw-r--r--   0        0        0     5473 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/taskfile_versions.mdx
+-rw-r--r--   0        0        0      763 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/translate.mdx
+-rw-r--r--   0        0        0    46204 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docs/usage.mdx
+-rw-r--r--   0        0        0     5155 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/docusaurus.config.ts
+-rw-r--r--   0        0        0     1508 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/package.json
+-rw-r--r--   0        0        0      208 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/prettier.config.js
+-rw-r--r--   0        0        0      271 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/sidebars.ts
+-rw-r--r--   0        0        0     1050 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/src/api/crowdin.js
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/src/components/.keep
+-rw-r--r--   0        0        0     1202 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/src/css/carbon.css
+-rw-r--r--   0        0        0     3089 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/src/css/custom.css
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/src/pages/.keep
+-rw-r--r--   0        0        0     1922 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/src/pages/donate.md
+-rw-r--r--   0        0        0     1342 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/src/themes/prismDark.js
+-rw-r--r--   0        0        0     1679 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/src/themes/prismLight.js
+-rw-r--r--   0        0        0        0 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/.nojekyll
+-rw-r--r--   0        0        0       13 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/CNAME
+-rw-r--r--   0        0        0      109 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/Taskfile.yml
+-rw-r--r--   0        0        0     7281 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/appwrite.svg
+-rw-r--r--   0        0        0   173915 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/favicon.ico
+-rw-r--r--   0        0        0     1321 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/icon-discord.svg
+-rw-r--r--   0        0        0     1227 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/icon-github.svg
+-rw-r--r--   0        0        0     1717 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/icon-mastodon.svg
+-rw-r--r--   0        0        0     1742 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/icon-twitter.svg
+-rw-r--r--   0        0        0    13524 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/logo.png
+-rw-r--r--   0        0        0      435 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/logo.svg
+-rw-r--r--   0        0        0      360 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/logo_mono.svg
+-rw-r--r--   0        0        0    19847 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/og-image.png
+-rw-r--r--   0        0        0     1276 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/img/pix.png
+-rwxr-xr-x   0        0        0     9634 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/install.sh
+-rw-r--r--   0        0        0      784 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/js/carbon.js
+-rw-r--r--   0        0        0    22417 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/static/schema.json
+-rw-r--r--   0        0        0       87 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/tsconfig.json
+-rw-r--r--   0        0        0    41801 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/api_reference.mdx
+-rw-r--r--   0        0        0    38988 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/changelog.mdx
+-rw-r--r--   0        0        0     1529 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/community.mdx
+-rw-r--r--   0        0        0     7804 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/contributing.mdx
+-rw-r--r--   0        0        0      711 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx
+-rw-r--r--   0        0        0      655 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/deprecations/template.mdx
+-rw-r--r--   0        0        0     1245 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx
+-rw-r--r--   0        0        0     5677 2024-05-10 01:19:21.470567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/experiments.mdx
+-rw-r--r--   0        0        0     1540 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx
+-rw-r--r--   0        0        0     7895 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/map_variables.mdx
+-rw-r--r--   0        0        0     4706 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx
+-rw-r--r--   0        0        0     1128 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/template.mdx
+-rw-r--r--   0        0        0     2583 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/faq.mdx
+-rw-r--r--   0        0        0     6930 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/installation.mdx
+-rw-r--r--   0        0        0     2911 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/integrations.mdx
+-rw-r--r--   0        0        0     1993 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/intro.mdx
+-rw-r--r--   0        0        0     2797 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/releasing.mdx
+-rw-r--r--   0        0        0     2974 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/styleguide.mdx
+-rw-r--r--   0        0        0     5473 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/taskfile_versions.mdx
+-rw-r--r--   0        0        0      763 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/translate.mdx
+-rw-r--r--   0        0        0    46204 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_docs/version-latest/usage.mdx
+-rw-r--r--   0        0        0      174 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versioned_sidebars/version-latest-sidebars.json
+-rw-r--r--   0        0        0       15 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/versions.json
+-rw-r--r--   0        0        0   364377 2024-05-10 01:19:21.474567 go_task_bin-3.37.1/task/website/yarn.lock
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 go_task_bin-3.37.1/PKG-INFO
```

### Comparing `go_task_bin-3.37.0/LICENSE` & `go_task_bin-3.37.1/LICENSE`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/README.md` & `go_task_bin-3.37.1/README.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/pdm_build.py` & `go_task_bin-3.37.1/pdm_build.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from wheel.cli.tags import tags
 
 if TYPE_CHECKING:
     from pdm.backend.hooks import Context
 
 NAME = "task"
-VERSION = "3.37.0"
+VERSION = "3.37.1"
 
 
 def is_windows():
     if "GOOS" in os.environ:
         return os.environ["GOOS"] == "windows"
     return sys.platform == "win32"
```

### Comparing `go_task_bin-3.37.0/pyproject.toml` & `go_task_bin-3.37.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "go-task-bin"
 description = "task - A task runner / simpler Make alternative written in Go"
-version = "3.37.0"
+version = "3.37.1"
 authors = [
     { name = "dowon", email = "ks2515@naver.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
```

### Comparing `go_task_bin-3.37.0/task/.github/CODE_OF_CONDUCT.md` & `go_task_bin-3.37.1/task/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.github/CONTRIBUTING.md` & `go_task_bin-3.37.1/task/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.github/ISSUE_TEMPLATE/config.yml` & `go_task_bin-3.37.1/task/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.github/workflows/issue-awaiting-response.yml` & `go_task_bin-3.37.1/task/.github/workflows/issue-awaiting-response.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.github/workflows/issue-closed.yml` & `go_task_bin-3.37.1/task/.github/workflows/issue-closed.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.github/workflows/issue-experiment.yml` & `go_task_bin-3.37.1/task/.github/workflows/issue-experiment.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.github/workflows/issue-needs-triage.yml` & `go_task_bin-3.37.1/task/.github/workflows/issue-needs-triage.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.github/workflows/lint.yml` & `go_task_bin-3.37.1/task/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.github/workflows/test.yml` & `go_task_bin-3.37.1/task/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.github/workflows/upload-source-documents.yml` & `go_task_bin-3.37.1/task/.github/workflows/upload-source-documents.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/.goreleaser.yml` & `go_task_bin-3.37.1/task/.goreleaser.yml`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         dst: /usr/local/share/zsh/site-functions/_task
 
 brews:
   - name: go-task
     description: Task runner / simpler Make alternative written in Go
     license: MIT
     homepage: https://taskfile.dev
-    folder: Formula
+    directory: Formula
     repository:
       owner: go-task
       name: homebrew-tap
     test:
       system "#{bin}/task", "--help"
     install: |-
       bin.install "task"
```

### Comparing `go_task_bin-3.37.0/task/CHANGELOG.md` & `go_task_bin-3.37.1/task/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## v3.37.1 - 2024-05-09
+
+- Fix bug where non-string values (numbers, bools) added to `env:` weren't been
+  correctly exported (#1640, #1641 by @vmaerten and @andreynering).
+
 ## v3.37.0 - 2024-05-08
 
 - Released the
   [Any Variables experiment](https://taskfile.dev/blog/any-variables), but
   [_without support for maps_](https://github.com/go-task/task/issues/1415#issuecomment-2044756925)
   (#1415, #1547 by @pd93).
 - Refactored how Task reads, parses and merges Taskfiles using a DAG (#1563,
```

### Comparing `go_task_bin-3.37.0/task/LICENSE` & `go_task_bin-3.37.1/task/LICENSE`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/README.md` & `go_task_bin-3.37.1/task/README.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/Taskfile.yml` & `go_task_bin-3.37.1/task/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/args/args.go` & `go_task_bin-3.37.1/task/args/args.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/args/args_test.go` & `go_task_bin-3.37.1/task/args/args_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/cmd/release/main.go` & `go_task_bin-3.37.1/task/cmd/release/main.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/cmd/sleepit/sleepit.go` & `go_task_bin-3.37.1/task/cmd/sleepit/sleepit.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/cmd/task/task.go` & `go_task_bin-3.37.1/task/cmd/task/task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/completion/bash/task.bash` & `go_task_bin-3.37.1/task/completion/bash/task.bash`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/completion/fish/task.fish` & `go_task_bin-3.37.1/task/completion/fish/task.fish`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/completion/ps/task.ps1` & `go_task_bin-3.37.1/task/completion/ps/task.ps1`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/completion/zsh/_task` & `go_task_bin-3.37.1/task/completion/zsh/_task`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/errors/errors.go` & `go_task_bin-3.37.1/task/errors/errors.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/errors/errors_task.go` & `go_task_bin-3.37.1/task/errors/errors_task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/errors/errors_taskfile.go` & `go_task_bin-3.37.1/task/errors/errors_taskfile.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/go.mod` & `go_task_bin-3.37.1/task/go.mod`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/go.sum` & `go_task_bin-3.37.1/task/go.sum`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/help.go` & `go_task_bin-3.37.1/task/help.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/init.go` & `go_task_bin-3.37.1/task/init.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/install-task.sh` & `go_task_bin-3.37.1/task/install-task.sh`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/compiler/compiler.go` & `go_task_bin-3.37.1/task/internal/compiler/compiler.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/deepcopy/deepcopy.go` & `go_task_bin-3.37.1/task/internal/deepcopy/deepcopy.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/editors/output.go` & `go_task_bin-3.37.1/task/internal/editors/output.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/execext/exec.go` & `go_task_bin-3.37.1/task/internal/execext/exec.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/exp/maps.go` & `go_task_bin-3.37.1/task/internal/exp/maps.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/experiments/experiments.go` & `go_task_bin-3.37.1/task/internal/experiments/experiments.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/filepathext/filepathext.go` & `go_task_bin-3.37.1/task/internal/filepathext/filepathext.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/fingerprint/checker.go` & `go_task_bin-3.37.1/task/internal/fingerprint/checker.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/fingerprint/glob.go` & `go_task_bin-3.37.1/task/internal/fingerprint/glob.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/fingerprint/sources_checksum.go` & `go_task_bin-3.37.1/task/internal/fingerprint/sources_checksum.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/fingerprint/sources_timestamp.go` & `go_task_bin-3.37.1/task/internal/fingerprint/sources_timestamp.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/fingerprint/status.go` & `go_task_bin-3.37.1/task/internal/fingerprint/status.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/fingerprint/task.go` & `go_task_bin-3.37.1/task/internal/fingerprint/task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/fingerprint/task_test.go` & `go_task_bin-3.37.1/task/internal/fingerprint/task_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/flags/flags.go` & `go_task_bin-3.37.1/task/internal/flags/flags.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/goext/meta.go` & `go_task_bin-3.37.1/task/internal/goext/meta.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/logger/logger.go` & `go_task_bin-3.37.1/task/internal/logger/logger.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/mocks/sources_checkable.go` & `go_task_bin-3.37.1/task/internal/mocks/sources_checkable.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/mocks/status_checkable.go` & `go_task_bin-3.37.1/task/internal/mocks/status_checkable.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/omap/orderedmap.go` & `go_task_bin-3.37.1/task/internal/omap/orderedmap.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/omap/orderedmap_test.go` & `go_task_bin-3.37.1/task/internal/omap/orderedmap_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/output/group.go` & `go_task_bin-3.37.1/task/internal/output/group.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/output/output.go` & `go_task_bin-3.37.1/task/internal/output/output.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/output/output_test.go` & `go_task_bin-3.37.1/task/internal/output/output_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/output/prefixed.go` & `go_task_bin-3.37.1/task/internal/output/prefixed.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/sort/sorter.go` & `go_task_bin-3.37.1/task/internal/sort/sorter.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/sort/sorter_test.go` & `go_task_bin-3.37.1/task/internal/sort/sorter_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/summary/summary.go` & `go_task_bin-3.37.1/task/internal/summary/summary.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/summary/summary_test.go` & `go_task_bin-3.37.1/task/internal/summary/summary_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/templater/funcs.go` & `go_task_bin-3.37.1/task/internal/templater/funcs.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/internal/templater/templater.go` & `go_task_bin-3.37.1/task/internal/templater/templater.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/package-lock.json` & `go_task_bin-3.37.1/task/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'version'": "'3.37.1'"}*

```diff
@@ -24,9 +24,9 @@
             },
             "integrity": "sha512-vQbdtBvesHm8EUFHX8QKg4rbBodmu9VsAXH1ozpbiN5jdTMOYHTCMM31EurAYmY+rNNtxJQ4JGy6t383RPlqbw==",
             "resolved": "https://registry.npmjs.org/@go-task/go-npm/-/go-npm-0.2.0.tgz",
             "version": "0.2.0"
         }
     },
     "requires": true,
-    "version": "3.37.0"
+    "version": "3.37.1"
 }
```

### Comparing `go_task_bin-3.37.0/task/package.json` & `go_task_bin-3.37.1/task/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'3.37.1'"}*

```diff
@@ -26,9 +26,9 @@
         "type": "git",
         "url": "https://github.com/go-task/task.git"
     },
     "scripts": {
         "postinstall": "go-npm install",
         "preuninstall": "go-npm uninstall"
     },
-    "version": "3.37.0"
+    "version": "3.37.1"
 }
```

### Comparing `go_task_bin-3.37.0/task/precondition.go` & `go_task_bin-3.37.1/task/precondition.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/requires.go` & `go_task_bin-3.37.1/task/requires.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/setup.go` & `go_task_bin-3.37.1/task/setup.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/signals.go` & `go_task_bin-3.37.1/task/signals.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/signals_test.go` & `go_task_bin-3.37.1/task/signals_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/status.go` & `go_task_bin-3.37.1/task/status.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/task.go` & `go_task_bin-3.37.1/task/task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/task_test.go` & `go_task_bin-3.37.1/task/task_test.go`

 * *Files 0% similar despite different names*

```diff
@@ -97,16 +97,17 @@
 
 func TestEnv(t *testing.T) {
 	tt := fileContentTest{
 		Dir:       "testdata/env",
 		Target:    "default",
 		TrimSpace: false,
 		Files: map[string]string{
-			"local.txt":  "GOOS='linux' GOARCH='amd64' CGO_ENABLED='0'\n",
-			"global.txt": "FOO='foo' BAR='overriden' BAZ='baz'\n",
+			"local.txt":         "GOOS='linux' GOARCH='amd64' CGO_ENABLED='0'\n",
+			"global.txt":        "FOO='foo' BAR='overriden' BAZ='baz'\n",
+			"multiple_type.txt": "FOO='1' BAR='true' BAZ='1.1'\n",
 		},
 	}
 	tt.Run(t)
 }
 
 func TestVars(t *testing.T) {
 	tt := fileContentTest{
```

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/cmd.go` & `go_task_bin-3.37.1/task/taskfile/ast/cmd.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/dep.go` & `go_task_bin-3.37.1/task/taskfile/ast/dep.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/for.go` & `go_task_bin-3.37.1/task/taskfile/ast/for.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/glob.go` & `go_task_bin-3.37.1/task/taskfile/ast/glob.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/graph.go` & `go_task_bin-3.37.1/task/taskfile/ast/graph.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/include.go` & `go_task_bin-3.37.1/task/taskfile/ast/include.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/output.go` & `go_task_bin-3.37.1/task/taskfile/ast/output.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/platforms.go` & `go_task_bin-3.37.1/task/taskfile/ast/platforms.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/platforms_test.go` & `go_task_bin-3.37.1/task/taskfile/ast/platforms_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/precondition.go` & `go_task_bin-3.37.1/task/taskfile/ast/precondition.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/precondition_test.go` & `go_task_bin-3.37.1/task/taskfile/ast/precondition_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/task.go` & `go_task_bin-3.37.1/task/taskfile/ast/task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/taskfile.go` & `go_task_bin-3.37.1/task/taskfile/ast/taskfile.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/taskfile_test.go` & `go_task_bin-3.37.1/task/taskfile/ast/taskfile_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/tasks.go` & `go_task_bin-3.37.1/task/taskfile/ast/tasks.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/ast/var.go` & `go_task_bin-3.37.1/task/taskfile/ast/var.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/cache.go` & `go_task_bin-3.37.1/task/taskfile/cache.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/dotenv.go` & `go_task_bin-3.37.1/task/taskfile/dotenv.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/node.go` & `go_task_bin-3.37.1/task/taskfile/node.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/node_base.go` & `go_task_bin-3.37.1/task/taskfile/node_base.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/node_file.go` & `go_task_bin-3.37.1/task/taskfile/node_file.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/node_http.go` & `go_task_bin-3.37.1/task/taskfile/node_http.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/node_stdin.go` & `go_task_bin-3.37.1/task/taskfile/node_stdin.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/reader.go` & `go_task_bin-3.37.1/task/taskfile/reader.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/taskfile/taskfile.go` & `go_task_bin-3.37.1/task/taskfile/taskfile.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/deps/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/deps/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/dir/dynamic_var/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/dir/dynamic_var/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/for/cmds/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/for/cmds/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/for/deps/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/for/deps/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/generates/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/generates/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/includes/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/includes/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/params/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/params/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/platforms/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/platforms/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/silent/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/silent/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/summary/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/summary/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/vars/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/vars/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/vars/any/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/vars/any/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/vars/any2/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/vars/any2/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/testdata/wildcards/Taskfile.yml` & `go_task_bin-3.37.1/task/testdata/wildcards/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/variables.go` & `go_task_bin-3.37.1/task/variables.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/watch.go` & `go_task_bin-3.37.1/task/watch.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/watch_test.go` & `go_task_bin-3.37.1/task/watch_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/Taskfile.yml` & `go_task_bin-3.37.1/task/website/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/blog/2023-09-02-introducing-experiments.mdx` & `go_task_bin-3.37.1/task/website/blog/2023-09-02-introducing-experiments.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/blog/2024-04-09-variables.mdx` & `go_task_bin-3.37.1/task/website/blog/2024-05-09-any-variables.mdx`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 title: Any Variables
 description: Task variables are no longer limited to strings!
 slug: any-variables
 authors: [pd93]
 tags: [experiments, variables]
 image: https://i.imgur.com/mErPwqL.png
 hide_table_of_contents: false
-draft: true
 ---
 
 import Tabs from '@theme/Tabs';
 import TabItem from '@theme/TabItem';
 
 Task has always had variables, but even though you were able to define them
 using different YAML types, they would always be converted to strings by Task.
 This limited users to string manipulation and encouraged messy workarounds for
-simple problems. Starting from [v3.36.0][v3.36.0], this is no longer the case!
+simple problems. Starting from [v3.37.0][v3.37.0], this is no longer the case!
 Task now supports most variable types, including **booleans**, **integers**,
 **floats** and **arrays**!
 
 {/* truncate */}
 
 ## What's the big deal?
 
@@ -171,12 +170,12 @@
 
 :::
 
 We're looking for feedback on a couple of different proposals, so please give
 them a go and let us know what you think. :pray:
 
 {/* prettier-ignore-start */}
-[v3.36.0]: https://github.com/go-task/task/releases/tag/v3.36.0
+[v3.37.0]: https://github.com/go-task/task/releases/tag/v3.37.0
 [slim-sprig-math]: https://go-task.github.io/slim-sprig/math.html
 [slim-sprig-list]: https://go-task.github.io/slim-sprig/lists.html
 [map-variables]: /experiments/map-variables
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.37.0/task/website/docs/api_reference.mdx` & `go_task_bin-3.37.1/task/website/docs/api_reference.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/changelog.mdx` & `go_task_bin-3.37.1/task/website/docs/changelog.mdx`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 ---
 slug: /changelog/
 sidebar_position: 14
 ---
 
 # Changelog
 
+## v3.37.1 - 2024-05-09
+
+- Fix bug where non-string values (numbers, bools) added to `env:` weren't been
+  correctly exported (#1640, #1641 by @vmaerten and @andreynering).
+
 ## v3.37.0 - 2024-05-08
 
 - Released the
   [Any Variables experiment](https://taskfile.dev/blog/any-variables), but
   [_without support for maps_](https://github.com/go-task/task/issues/1415#issuecomment-2044756925)
   (#1415, #1547 by @pd93).
 - Refactored how Task reads, parses and merges Taskfiles using a DAG (#1563,
```

### Comparing `go_task_bin-3.37.0/task/website/docs/community.mdx` & `go_task_bin-3.37.1/task/website/docs/community.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/contributing.mdx` & `go_task_bin-3.37.1/task/website/docs/contributing.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/deprecations/deprecations.mdx` & `go_task_bin-3.37.1/task/website/docs/deprecations/deprecations.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/deprecations/template.mdx` & `go_task_bin-3.37.1/task/website/docs/deprecations/template.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/deprecations/version_2_schema.mdx` & `go_task_bin-3.37.1/task/website/docs/deprecations/version_2_schema.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/experiments/experiments.mdx` & `go_task_bin-3.37.1/task/website/docs/experiments/experiments.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/experiments/gentle_force.mdx` & `go_task_bin-3.37.1/task/website/docs/experiments/gentle_force.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/experiments/map_variables.mdx` & `go_task_bin-3.37.1/task/website/docs/experiments/map_variables.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/experiments/remote_taskfiles.mdx` & `go_task_bin-3.37.1/task/website/docs/experiments/remote_taskfiles.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/experiments/template.mdx` & `go_task_bin-3.37.1/task/website/docs/experiments/template.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/faq.mdx` & `go_task_bin-3.37.1/task/website/docs/faq.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/installation.mdx` & `go_task_bin-3.37.1/task/website/docs/installation.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/integrations.mdx` & `go_task_bin-3.37.1/task/website/docs/integrations.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/intro.mdx` & `go_task_bin-3.37.1/task/website/docs/intro.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/releasing.mdx` & `go_task_bin-3.37.1/task/website/docs/releasing.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/styleguide.mdx` & `go_task_bin-3.37.1/task/website/docs/styleguide.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/taskfile_versions.mdx` & `go_task_bin-3.37.1/task/website/docs/taskfile_versions.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/translate.mdx` & `go_task_bin-3.37.1/task/website/docs/translate.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docs/usage.mdx` & `go_task_bin-3.37.1/task/website/docs/usage.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/docusaurus.config.ts` & `go_task_bin-3.37.1/task/website/docusaurus.config.ts`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/package.json` & `go_task_bin-3.37.1/task/website/package.json`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/src/api/crowdin.js` & `go_task_bin-3.37.1/task/website/src/api/crowdin.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/src/css/carbon.css` & `go_task_bin-3.37.1/task/website/src/css/carbon.css`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/src/css/custom.css` & `go_task_bin-3.37.1/task/website/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/src/pages/donate.md` & `go_task_bin-3.37.1/task/website/src/pages/donate.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/src/themes/prismDark.js` & `go_task_bin-3.37.1/task/website/src/themes/prismDark.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/src/themes/prismLight.js` & `go_task_bin-3.37.1/task/website/src/themes/prismLight.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/img/appwrite.svg` & `go_task_bin-3.37.1/task/website/static/img/appwrite.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/img/favicon.ico` & `go_task_bin-3.37.1/task/website/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/img/icon-discord.svg` & `go_task_bin-3.37.1/task/website/static/img/icon-discord.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/img/icon-github.svg` & `go_task_bin-3.37.1/task/website/static/img/icon-github.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/img/icon-mastodon.svg` & `go_task_bin-3.37.1/task/website/static/img/icon-mastodon.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/img/icon-twitter.svg` & `go_task_bin-3.37.1/task/website/static/img/icon-twitter.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/img/logo.png` & `go_task_bin-3.37.1/task/website/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/img/og-image.png` & `go_task_bin-3.37.1/task/website/static/img/og-image.png`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/img/pix.png` & `go_task_bin-3.37.1/task/website/static/img/pix.png`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/install.sh` & `go_task_bin-3.37.1/task/website/static/install.sh`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/js/carbon.js` & `go_task_bin-3.37.1/task/website/static/js/carbon.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/static/schema.json` & `go_task_bin-3.37.1/task/website/static/schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998459757834757%*

 * *Differences: {"'allOf'": '{0: {\'properties\': {\'silent\': {\'description\': "Default \'silent\' options for '*

 * *            'this Taskfile. If `false`, can be overridden with `true` in a task by task '*

 * *            'basis."}}}}',*

 * * "'definitions'": "{'glob_obj': {'properties': {'exclude': {'description': 'File or glob pattern "*

 * *                  "to exclude from the list'}}}}"}*

```diff
@@ -119,15 +119,15 @@
                     "description": "Enables Bash shell options for all commands in the Taskfile. See https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html",
                     "items": {
                         "$ref": "#/definitions/shopt"
                     },
                     "type": "array"
                 },
                 "silent": {
-                    "description": "Default 'silent' options for this Taskfile. If `false`, can be overidden with `true` in a task by task basis.",
+                    "description": "Default 'silent' options for this Taskfile. If `false`, can be overridden with `true` in a task by task basis.",
                     "type": "boolean"
                 },
                 "tasks": {
                     "$ref": "#/definitions/tasks",
                     "description": "A set of task definitions."
                 },
                 "vars": {
@@ -405,15 +405,15 @@
                     "$ref": "#/definitions/glob_obj"
                 }
             ]
         },
         "glob_obj": {
             "properties": {
                 "exclude": {
-                    "description": "File or glob patter to exclude from the list",
+                    "description": "File or glob pattern to exclude from the list",
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "outputObject": {
             "properties": {
```

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/api_reference.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/api_reference.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/changelog.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/changelog.mdx`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 ---
 slug: /changelog/
 sidebar_position: 14
 ---
 
 # Changelog
 
+## v3.37.1 - 2024-05-09
+
+- Fix bug where non-string values (numbers, bools) added to `env:` weren't been
+  correctly exported (#1640, #1641 by @vmaerten and @andreynering).
+
 ## v3.37.0 - 2024-05-08
 
 - Released the
   [Any Variables experiment](https://taskfile.dev/blog/any-variables), but
   [_without support for maps_](https://github.com/go-task/task/issues/1415#issuecomment-2044756925)
   (#1415, #1547 by @pd93).
 - Refactored how Task reads, parses and merges Taskfiles using a DAG (#1563,
```

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/community.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/community.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/contributing.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/contributing.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/template.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/deprecations/template.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/experiments.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/experiments.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/map_variables.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/map_variables.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/template.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/experiments/template.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/faq.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/faq.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/installation.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/installation.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/integrations.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/integrations.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/intro.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/intro.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/releasing.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/releasing.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/styleguide.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/styleguide.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/taskfile_versions.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/taskfile_versions.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/translate.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/translate.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/usage.mdx` & `go_task_bin-3.37.1/task/website/versioned_docs/version-latest/usage.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/task/website/yarn.lock` & `go_task_bin-3.37.1/task/website/yarn.lock`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.37.0/PKG-INFO` & `go_task_bin-3.37.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: go-task-bin
-Version: 3.37.0
+Version: 3.37.1
 Summary: task - A task runner / simpler Make alternative written in Go
 Keywords: build,build-tool,devops,go,make,makefile,runner,task,task-runner,taskfile,tool
 Author-Email: dowon <ks2515@naver.com>
 License: MIT
 Classifier: Programming Language :: Other
 Classifier: Topic :: Software Development :: Build Tools
 Project-URL: Repository, https://github.com/Bing-su/pip-binary-factory
```

