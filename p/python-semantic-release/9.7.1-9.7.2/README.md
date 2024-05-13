# Comparing `tmp/python_semantic_release-9.7.1.tar.gz` & `tmp/python_semantic_release-9.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_semantic_release-9.7.1.tar", last modified: Tue May  7 03:29:03 2024, max compression
+gzip compressed data, was "python_semantic_release-9.7.2.tar", last modified: Mon May 13 03:23:03 2024, max compression
```

## Comparing `python_semantic_release-9.7.1.tar` & `python_semantic_release-9.7.2.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.137456 python_semantic_release-9.7.1/
--rw-r--r--   0 root         (0) root         (0)      230 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      225 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5282 2024-05-07 03:29:03.137456 python_semantic_release-9.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2673 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.105455 python_semantic_release-9.7.1/docs/
--rw-r--r--   0 root         (0) root         (0)     6984 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     9656 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/algorithm.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.109455 python_semantic_release-9.7.1/docs/automatic-releases/
--rw-r--r--   0 root         (0) root         (0)     1284 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/automatic-releases/cronjobs.rst
--rw-r--r--   0 root         (0) root         (0)     4046 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/automatic-releases/github-actions.rst
--rw-r--r--   0 root         (0) root         (0)      738 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/automatic-releases/index.rst
--rw-r--r--   0 root         (0) root         (0)     2268 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/automatic-releases/travis.rst
--rw-r--r--   0 root         (0) root         (0)    17609 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/changelog_templates.rst
--rw-r--r--   0 root         (0) root         (0)    16256 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/commands.rst
--rw-r--r--   0 root         (0) root         (0)    15380 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/commit-parsing.rst
--rw-r--r--   0 root         (0) root         (0)     2288 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    29841 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/contributors.rst
--rw-r--r--   0 root         (0) root         (0)     3644 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/github-action.rst
--rw-r--r--   0 root         (0) root         (0)     6814 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     6735 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    21218 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/migrating_from_v7.rst
--rw-r--r--   0 root         (0) root         (0)     8869 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/multibranch_releases.rst
--rw-r--r--   0 root         (0) root         (0)     2403 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/strict_mode.rst
--rw-r--r--   0 root         (0) root         (0)     1452 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/troubleshooting.rst
--rw-r--r--   0 root         (0) root         (0)     9237 2024-05-07 03:28:56.000000 python_semantic_release-9.7.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.133455 python_semantic_release-9.7.1/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5282 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5600 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      614 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.109455 python_semantic_release-9.7.1/semantic_release/
--rw-r--r--   0 root         (0) root         (0)      870 2024-05-07 03:28:56.000000 python_semantic_release-9.7.1/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.109455 python_semantic_release-9.7.1/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1051 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6675 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4640 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.113455 python_semantic_release-9.7.1/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      419 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.113455 python_semantic_release-9.7.1/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     3443 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/cli_context.py
--rw-r--r--   0 root         (0) root         (0)     1699 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     2900 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    25912 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)     1439 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    20389 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.117455 python_semantic_release-9.7.1/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      615 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3004 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4579 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3452 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5879 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3353 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1505 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.097455 python_semantic_release-9.7.1/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.117455 python_semantic_release-9.7.1/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     5581 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.117455 python_semantic_release-9.7.1/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2607 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     9216 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    11152 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    18287 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     6249 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)     6055 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/remote_hvcs_base.py
--rw-r--r--   0 root         (0) root         (0)      663 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2886 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.121455 python_semantic_release-9.7.1/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16854 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7357 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14175 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 03:29:03.137456 python_semantic_release-9.7.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.121455 python_semantic_release-9.7.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.121455 python_semantic_release-9.7.1/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2983 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)    11360 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1759 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)     6566 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     5255 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    31841 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_version.py
--rw-r--r--   0 root         (0) root         (0)     2880 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     7826 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      197 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1178 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)    12976 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    13342 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/git_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/repos/
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/
--rw-r--r--   0 root         (0) root         (0)      140 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21042 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
--rw-r--r--   0 root         (0) root         (0)    21711 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/repos/github_flow/
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/github_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15712 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/github_flow/repo_w_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/
--rw-r--r--   0 root         (0) root         (0)      199 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10463 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
--rw-r--r--   0 root         (0) root         (0)    13604 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
--rw-r--r--   0 root         (0) root         (0)    10698 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
--rw-r--r--   0 root         (0) root         (0)    14083 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127286 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12845 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     5074 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.129455 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10042 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     6358 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     3560 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.129455 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8907 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     2129 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     6361 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     4344 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_util.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.129455 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6374 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2567 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      778 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_parsed_commit.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2203 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.133455 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1761 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    10290 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    27795 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    36478 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    15576 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_util.py
--rw-r--r--   0 root         (0) root         (0)     4507 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.133455 python_semantic_release-9.7.1/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9605 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3874 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2951 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9714 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_version.py
--rw-r--r--   0 root         (0) root         (0)     6271 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.582741 python_semantic_release-9.7.2/
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      225 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5348 2024-05-13 03:23:03.582741 python_semantic_release-9.7.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.554741 python_semantic_release-9.7.2/docs/
+-rw-r--r--   0 root         (0) root         (0)     6984 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9656 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/algorithm.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.554741 python_semantic_release-9.7.2/docs/automatic-releases/
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/automatic-releases/cronjobs.rst
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/automatic-releases/github-actions.rst
+-rw-r--r--   0 root         (0) root         (0)      738 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/automatic-releases/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/automatic-releases/travis.rst
+-rw-r--r--   0 root         (0) root         (0)    17609 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/changelog_templates.rst
+-rw-r--r--   0 root         (0) root         (0)    16256 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/commands.rst
+-rw-r--r--   0 root         (0) root         (0)    15380 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/commit-parsing.rst
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)    33028 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/contributors.rst
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/github-action.rst
+-rw-r--r--   0 root         (0) root         (0)     6814 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6735 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    21218 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/migrating_from_v7.rst
+-rw-r--r--   0 root         (0) root         (0)     8869 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/multibranch_releases.rst
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/strict_mode.rst
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/troubleshooting.rst
+-rw-r--r--   0 root         (0) root         (0)     9264 2024-05-13 03:22:52.000000 python_semantic_release-9.7.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.578741 python_semantic_release-9.7.2/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5348 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5600 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      634 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.558741 python_semantic_release-9.7.2/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)      870 2024-05-13 03:22:52.000000 python_semantic_release-9.7.2/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.558741 python_semantic_release-9.7.2/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.558741 python_semantic_release-9.7.2/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.562741 python_semantic_release-9.7.2/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/cli_context.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    26160 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    21769 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.562741 python_semantic_release-9.7.2/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      615 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5879 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.546742 python_semantic_release-9.7.2/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.562741 python_semantic_release-9.7.2/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.566742 python_semantic_release-9.7.2/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    11152 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    18287 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/remote_hvcs_base.py
+-rw-r--r--   0 root         (0) root         (0)      663 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.566742 python_semantic_release-9.7.2/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16854 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14175 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 03:23:03.582741 python_semantic_release-9.7.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.566742 python_semantic_release-9.7.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    35485 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)    12976 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    13342 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/git_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/repos/
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/
+-rw-r--r--   0 root         (0) root         (0)      140 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/repos/github_flow/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/github_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15712 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/github_flow/repo_w_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
+-rw-r--r--   0 root         (0) root         (0)    10698 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
+-rw-r--r--   0 root         (0) root         (0)    14083 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127286 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12845 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     5074 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     6361 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.578741 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6374 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      778 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_parsed_commit.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.578741 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    10290 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    27795 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    36478 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    15576 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.578741 python_semantic_release-9.7.2/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9605 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     6271 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/util.py
```

### Comparing `python_semantic_release-9.7.1/LICENSE` & `python_semantic_release-9.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/PKG-INFO` & `python_semantic_release-9.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.7.1
+Version: 9.7.2
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -28,14 +28,16 @@
 Requires-Dist: python-gitlab~=4.0
 Requires-Dist: tomlkit~=0.11
 Requires-Dist: dotty-dict~=1.3
 Requires-Dist: importlib-resources~=6.0
 Requires-Dist: pydantic~=2.0
 Requires-Dist: rich~=13.0
 Requires-Dist: shellingham~=1.5
+Provides-Extra: build
+Requires-Dist: build~=1.2; extra == "build"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=6.0; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc==0.5.0; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
 Requires-Dist: furo~=2024.1; extra == "docs"
 Provides-Extra: test
 Requires-Dist: coverage[toml]~=7.0; extra == "test"
```

### Comparing `python_semantic_release-9.7.1/README.rst` & `python_semantic_release-9.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/docs/Makefile` & `python_semantic_release-9.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/docs/algorithm.rst` & `python_semantic_release-9.7.2/docs/algorithm.rst`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   this branch's history.
 * If we can identify a commit as a ``merge-base`` between our HEAD commit and one
   or more tags, then that merge-base should be unique.
 * We know ahead of time what ``prerelease_token`` to use for prereleases - e.g.
   ``rc``.
 * We know ahead of time whether ``major`` changes introduced by commits
   should cause the new version to remain on ``0.y.z`` if the project is already
-  on a ``0.`` version - see :ref:`major_on_zero <config-major-on-zero>`.
+  on a ``0.`` version - see :ref:`major_on_zero <config-major_on_zero>`.
 
 .. _algorithm-implementation:
 
 Implementation
 ~~~~~~~~~~~~~~
 
 1. Parse all the Git tags of the repository into semantic versions, and **sort**
```

### Comparing `python_semantic_release-9.7.1/docs/automatic-releases/cronjobs.rst` & `python_semantic_release-9.7.2/docs/automatic-releases/cronjobs.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/docs/automatic-releases/github-actions.rst` & `python_semantic_release-9.7.2/docs/automatic-releases/github-actions.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/docs/automatic-releases/index.rst` & `python_semantic_release-9.7.2/docs/automatic-releases/index.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/docs/automatic-releases/travis.rst` & `python_semantic_release-9.7.2/docs/automatic-releases/travis.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This guide expects you to have activated the repository on Travis CI.
 If this is not the case, please refer to `Travis documentation`_ on how to do that.
 
 1. Add python-semantic-release settings
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 See :doc:`../configuration` for details on how to configure Python Semantic Release.
-Make sure that at least you have set :ref:`config-version-variables` before continuing.
+Make sure that at least you have set :ref:`config-version_variables` before continuing.
 
 2. Add environment variables
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 You will need to set up an environment variable in Travis. An easy way to do that
 is to go to the settings page for your package and add it there. Make sure that the
 secret toggle is set correctly.
```

### Comparing `python_semantic_release-9.7.1/docs/changelog_templates.rst` & `python_semantic_release-9.7.2/docs/changelog_templates.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 .. _changelog-templates:
 
 Changelog Templates
 ===================
 
 .. warning::
     If you have an existing changelog in the location you have configured with
-    the :ref:`changelog_file <config-changelog-changelog-file>` setting,
-    or if you have a template inside your :ref:`template directory <config-changelog-template-dir>`
+    the :ref:`changelog_file <config-changelog-changelog_file>` setting,
+    or if you have a template inside your :ref:`template directory <config-changelog-template_dir>`
     which will render to the location of an existing file, Python Semantic Release will
     overwrite the contents of this file.
 
     Please make sure to refer to :ref:`changelog-templates-migrating-existing-changelog`.
 
 Python Semantic Release can write a changelog for your project. By default, it uses an
 in-built template; once rendered this will be written to the location you configure with the
-:ref:`changelog_file <config-changelog-changelog-file>` setting.
+:ref:`changelog_file <config-changelog-changelog_file>` setting.
 
 However, Python Semantic Release is also capable of rendering an entire directory tree
 of templates during the changelog generation process. This directory is specified
-using the :ref:`template directory <config-changelog-template-dir>` setting.
+using the :ref:`template directory <config-changelog-template_dir>` setting.
 
 Python Semantic Release uses `Jinja`_ as its template engine, so you should refer to the
 `Template Designer Documentation`_ for guidance on how to customize the appearance of
 the files which are rendered during the release process. If you would like to customize
 the template environment itself, then certain options are available to you via
 :ref:`changelog environment configuration <config-changelog-environment>`.
 
@@ -44,15 +44,15 @@
 
 Directory Structure:
 ^^^^^^^^^^^^^^^^^^^^
 
 If you don't want to set up your own custom changelog template, you can have Python
 Semantic Release use its in-built template. If you would like to customize the
 appearance of the changelog, or to render additional files, then you will need to
-create a directory within your repository and set the :ref:`template_dir <config-changelog-template-dir>`
+create a directory within your repository and set the :ref:`template_dir <config-changelog-template_dir>`
 setting to the name of this directory. The default name is ``"templates"``.
 
 .. note::
    It is *strongly* recommended that you use a dedicated top-level folder for the
    template directory.
 
 When the templates are rendered, files within the tree are output to the location
@@ -74,15 +74,15 @@
 a ``"."``.
 
 .. _changelog-templates-template-rendering-directory-structure-example:
 
 Directory Structure (Example)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Suppose a project sets :ref:`template_dir <config-changelog-template-dir>` to
+Suppose a project sets :ref:`template_dir <config-changelog-template_dir>` to
 ``"templates"`` and has the following structure:
 
 .. code-block::
 
     example-project
     ├── src
     │   └── example_project
@@ -285,15 +285,15 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The same :ref:`template rendering <changelog-templates-template-rendering>` mechanism
 generates the release notes when :ref:`creating VCS releases <index-creating-vcs-releases>`:
 
 * the `in-built template`_ is used by default
 * create a file named ``.release_notes.md.j2`` inside the project's
-  :ref:`template_dir <config-changelog-template-dir>` to customize the release notes
+  :ref:`template_dir <config-changelog-template_dir>` to customize the release notes
 
 .. _changelog-templates-customizing-vcs-release-notes-release-notes-context:
 
 Release Notes Context
 """""""""""""""""""""
 
 All of the changelog's
```

### Comparing `python_semantic_release-9.7.1/docs/commands.rst` & `python_semantic_release-9.7.2/docs/commands.rst`

 * *Files 1% similar despite different names*

```diff
@@ -97,33 +97,33 @@
 Detect the semantically correct next version that should be applied to your
 project.
 
 By default:
 
   * Write this new version to the project metadata locations
     specified in the configuration file
-  * Build the project using :ref:`config-build-command`, if specified
+  * Build the project using :ref:`config-build_command`, if specified
   * Create a new commit with these locations and any other assets configured
     to be included in a release
   * Tag this commit according the configured format, with a tag that uniquely
     identifies the version being released
   * Push the new tag and commit to the remote for the repository
   * Create a release (if supported) in the remote VCS for this tag
 
 Changelog generation is done identically to the way it is done in :ref:`cmd-changelog`,
 but this command additionally ensures the updated changelog is included in the release
 commit that is made.
 
 .. seealso::
     - :ref:`cmd-changelog`
     - :ref:`changelog-templates`
-    - :ref:`config-tag-format`
+    - :ref:`config-tag_format`
     - :ref:`config-assets`
-    - :ref:`config-version-toml`
-    - :ref:`config-version-variables`
+    - :ref:`config-version_toml`
+    - :ref:`config-version_variables`
 
 .. _cmd-version-options:
 
 Options:
 --------
 
 .. _cmd-version-option-print:
@@ -312,15 +312,15 @@
 command invocation, and to run ``git tag`` on this new commit with a tag corresponding to the new version.
 
 If ``--no-commit`` is supplied, it may disable other options derivatively; please see below.
 
 **Default:** ``--commit``
 
 .. seealso::
-   - :ref:`tag_format <config-tag-format>`
+   - :ref:`tag_format <config-tag_format>`
 
 .. _cmd-version-option-tag:
 
 ``--tag/--no-tag``
 ************************
 
 Whether or not to perform a ``git tag`` to apply a tag of the corresponding to the new version during this
@@ -366,26 +366,26 @@
 
 **Default:** ``--no-vcs-release`` if ``--no-push`` is supplied (including where this is
 implied by supplying only ``--no-commit``), otherwise ``--vcs-release``
 
 ``--skip-build``
 ****************
 
-If passed, skip building the current project using :ref:`build_command <config-build-command>`.
+If passed, skip building the current project using :ref:`build_command <config-build_command>`.
 
 .. _cmd-publish:
 
 ``semantic-release publish``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Publish a distribution to a VCS release. Uploads using :ref:`config-publish`
 
 .. seealso::
     - :ref:`config-publish`
-    - :ref:`config-build-command`
+    - :ref:`config-build_command`
 
 .. _cmd-publish-options:
 
 Options:
 --------
 
 .. _cmd-publish-option-tag:
```

### Comparing `python_semantic_release-9.7.1/docs/commit-parsing.rst` & `python_semantic_release-9.7.2/docs/commit-parsing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
   However, other tools may not do this, so if you plan to use any similar
   programs then you should try to stick to the official format.
 
 More information about the style can be found in the `angular commit guidelines`_.
 
 .. seealso::
-  - :ref:`commit_parser <config-commit-parser>`
-  - :ref:`commit_parser_options <config-commit-parser-options>`
+  - :ref:`commit_parser <config-commit_parser>`
+  - :ref:`commit_parser_options <config-commit_parser_options>`
 
 .. _commit-parser-builtin:
 
 Built-in Commit Parsers
 -----------------------
 
 The following parsers are built in to Python Semantic Release:
@@ -177,15 +177,15 @@
 Writing your own parser
 -----------------------
 
 If you would prefer to use an alternative commit style, for example to adjust the
 different ``type`` values that are associated with a particular commit, this is
 possible.
 
-The :ref:`commit_parser <config-commit-parser>` option, if set to a string which
+The :ref:`commit_parser <config-commit_parser>` option, if set to a string which
 does not match one of Python Semantic Release's inbuilt commit parsers, will be
 used to attempt to dynamically import a custom commit parser class. As such you will
 need to ensure that your custom commit parser is import-able from the environment in
 which you are running Python Semantic Release. The string should be structured in the
 standard ``module:attr`` format; for example, to import the class ``MyCommitParser``
 from the file ``custom_parser.py`` at the root of your repository, you should specify
 ``"commit_parser=custom_parser:MyCommitParser"`` in your configuration, and run the
@@ -292,16 +292,16 @@
 """"""""""""""
 
 To provide options to the commit parser which is configured in the :ref:`configuration file
 <configuration>`, Python Semantic Release includes a :py:class:`semantic_release.ParserOptions`
 class. Each parser built into Python Semantic Release has a corresponding "options" class, which
 subclasses :py:class:`semantic_release.ParserOptions`.
 
-The configuration in :ref:`commit_parser_options <config-commit-parser-options>` is passed to the
-"options" class which is specified by the configured :ref:`commit_parser <config-commit-parser>` -
+The configuration in :ref:`commit_parser_options <config-commit_parser_options>` is passed to the
+"options" class which is specified by the configured :ref:`commit_parser <config-commit_parser>` -
 more information on how this is specified is below.
 
 The "options" class is used to validate the options which are configured in the repository,
 and to provide default values for these options where appropriate.
 
 If you are writing your own parser, you should accompany it with an "options" class
 which accepts the appropriate keyword arguments. This class' ``__init__`` method should
```

### Comparing `python_semantic_release-9.7.1/docs/conf.py` & `python_semantic_release-9.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/docs/configuration.rst` & `python_semantic_release-9.7.2/docs/configuration.rst`

 * *Files 9% similar despite different names*

```diff
@@ -63,60 +63,94 @@
 including long after its deleted if a token is in your git history. Instead, define the name
 of the environment variable which contains your :ref:`remote.token <config-remote-token>`,
 such as ``GH_TOKEN``, in your configuration file, and Python Semantic Release will do the
 rest, as seen below.
 
 .. code-block:: toml
 
-    [tool.semantic_release.remote.token]
+    [semantic_release.remote.token]
     env = "GH_TOKEN"
 
 Given basic TOML syntax compatibility, this is equivalent to:
 
 .. code-block:: toml
 
-    [tool.semantic_release.remote]
+    [semantic_release.remote]
     token = { env = "GH_TOKEN" }
 
 The general format for specifying that some configuration should be sourced from an
 environment variable is:
 
 .. code-block:: toml
 
-    [tool.semantic_release.<setting>]
+    [semantic_release.variable]
     env = "ENV_VAR"
     default_env = "FALLBACK_ENV_VAR"
     default = "default value"
 
 In this structure:
   * ``env`` represents the environment variable that Python Semantic Release will search for
   * ``default_env`` is a fallback environment variable to read in case the variable specified
     by ``env`` is not set. This is optional - if not specified then no fallback will be used.
   * ``default`` is a default value to use in case the environment variable specified by ``env``
     is not set. This is optional - if ``default`` is not specified then the environment variable
     specified by ``env`` is considered required.
 
-.. _config-settings:
+.. _config-root:
+
+``semantic_release`` settings
+-----------------------------
+
+The following sections outline all the definitions and descriptions of each supported
+configuration setting. If there are type mis-matches, PSR will throw validation errors upon load.
+If a setting is not provided, than PSR will fill in the value with the default value.
+
+Python Semantic Release expects a root level key to start the configuration definition. Make
+sure to use the correct root key dependending on the configuration format you are using.
+
+.. note:: If you are using ``pyproject.toml``, this heading should include the `tool`` prefix
+          as specified within PEP 517, resulting in ``[tool.semantic_release]``.
 
-Settings
---------
+.. note:: If you are using a ``releaserc.toml``, use ``[semantic_release]`` as the root key
+
+.. note:: If you are using a ``releaserc.json``, ``semantic_release`` must be the root key in the
+          top level dictionary.
 
 ----
 
-.. _config-root:
+.. _config-allow_zero_version:
 
-``[tool.semantic_release]``
-***************************
+``allow_zero_version``
+""""""""""""""""""""""
+
+**Type:** ``bool``
+
+This flag controls whether or not Python Semantic Release will use version
+numbers aligning with the ``0.x.x`` pattern.
+
+If set to ``true`` and starting at ``0.0.0``, a minor bump would set the
+next version as ``0.1.0`` whereas a patch bump would set the next version as
+``0.0.1``. A breaking change (ie. major bump) would set the next version as
+``1.0.0`` unless the :ref:`config-major_on_zero` is set to ``false``.
+
+If set to ``false``, Python Semantic Release will consider the first possible
+version to be ``1.0.0``, regardless of patch, minor, or major change level.
+Additionally, when ``allow_zero_version`` is set to ``false``,
+the :ref:`config-major_on_zero` setting is ignored.
+
+**Default:** ``true``
 
 ----
 
 .. _config-assets:
 
-``assets (List[str])``
-""""""""""""""""""""""
+``assets``
+""""""""""
+
+**Type:** ``list[str]``
 
 One or more paths to additional assets that should committed to the remote repository
 in addition to any files modified by writing the new version.
 
 **Default:** ``[]``
 
 ----
@@ -128,22 +162,22 @@
 
 This setting is discussed in more detail at :ref:`multibranch-releases`
 
 **Default:**
 
 .. code-block:: toml
 
-    [tool.semantic_release.branches.main]
+    [semantic_release.branches.main]
     match = "(main|master)"
     prerelease_token = "rc"
     prerelease = false
 
 ----
 
-.. _config-build-command:
+.. _config-build_command:
 
 ``build_command``
 """""""""""""""""
 
 **Type:** ``Optional[str]``
 
 Command to use to build the current project during :ref:`cmd-version`.
@@ -151,14 +185,17 @@
 Python Semantic Release will execute the build command in the OS default
 shell with a subset of environment variables. PSR provides the variable
 ``NEW_VERSION`` in the environment with the value of the next determined
 version. The following table summarizes all the environment variables that
 are passed on to the ``build_command`` runtime if they exist in the parent
 process.
 
+If you would like to pass additional environment variables to your build
+command, see :ref:`config-build_command_env`.
+
 ========================  ======================================================================
 Variable Name             Description
 ========================  ======================================================================
 CI                        Pass-through ``true`` if exists in process env, unset otherwise
 BITBUCKET_CI              ``true`` if Bitbucket CI variables exist in env, unset otherwise
 GITHUB_ACTIONS            Pass-through ``true`` if exists in process env, unset otherwise
 GITEA_ACTIONS             Pass-through ``true`` if exists in process env, unset otherwise
@@ -170,526 +207,572 @@
 VIRTUAL_ENV               Pass-through ``VIRTUAL_ENV`` if exists in process env, unset otherwise
 ========================  ======================================================================
 
 **Default:** ``None`` (not specified)
 
 ----
 
-.. _config-commit_author:
+.. _config-build_command_env:
 
-``commit_author (str)``
-"""""""""""""""""""""""
-Author used in commits in the format ``name <email>``.
+``build_command_env``
+"""""""""""""""""""""
+
+**Type:** ``Optional[list[str]]``
+
+List of environment variables to include or pass-through on to the build command that executes
+during :ref:`cmd-version`.
+
+This configuration option allows the user to extend the list of environment variables
+from the table above in :ref:`config-build_command`. The input is a list of strings
+where each individual string handles a single variable definition. There are two formats
+accepted and are detailed in the following table:
+
+==================  ===================================================================
+FORMAT              Description
+==================  ===================================================================
+``VAR_NAME``        Detects value from the PSR process environment, and passes value to
+                    ``build_command`` process
+
+``VAR_NAME=value``  Sets variable name to value inside of ``build_command`` process
+==================  ===================================================================
+
+.. note:: Although variable name capitalization is not required, it is recommended as
+          to be in-line with the POSIX-compliant recommendation for shell variable names.
+
+**Default:** ``None`` (not specified)
+
+----
+
+.. _config-changelog:
+
+``changelog``
+"""""""""""""
+
+This section outlines the configuration options available that modify changelog generation.
 
 .. note::
-  If you are using the built-in GitHub Action, the default value is set to
-  ``github-actions <actions@github.com>``. You can modify this with the
-  ``git_committer_name`` and ``git_committer_name`` inputs.
+    **pyproject.toml:** ``[tool.semantic_release.changelog]``
 
-.. seealso::
-   - :ref:`github-actions`
+    **releaserc.toml:** ``[semantic_release.changelog]``
 
-**Default:** ``semantic-release <semantic-release>``
+    **releaserc.json:** ``{ "semantic_release": { "changelog": {} } }``
 
 ----
 
-.. _config-commit-message:
+.. _config-changelog-changelog_file:
 
-``commit_message (str)``
-""""""""""""""""""""""""
+``changelog_file``
+******************
 
-Commit message to use when making release commits. The message can use ``{version}``
-as a format key, in which case the version being released will be formatted into
-the message.
+**Type:** ``str``
 
-If at some point in your project's lifetime you change this, you may wish to consider,
-adding the old message pattern(s) to :ref:`exclude_commit_patterns <config-changelog-exclude-commit-patterns>`.
+Specify the name of the changelog file (after template rendering has taken place).
 
-**Default:** ``"{version}\n\nAutomatically generated by python-semantic-release"``
+**Default:** ``"CHANGELOG.md"``
 
 ----
 
-.. _config-commit-parser:
+.. _config-changelog-environment:
 
-``commit_parser (str)``
-"""""""""""""""""""""""
+``environment``
+***************
 
-Specify which commit parser Python Semantic Release should use to parse the commits
-within the Git repository.
+.. note::
+   This section of the configuration contains options which customize the template
+   environment used to render templates such as the changelog. Most options are
+   passed directly to the `jinja2.Environment`_ constructor, and further
+   documentation one these parameters can be found there.
 
-Built-in parsers:
-    * ``angular`` - :ref:`AngularCommitParser <commit-parser-angular>`
-    * ``emoji`` - :ref:`EmojiCommitParser <commit-parser-emoji>`
-    * ``scipy`` - :ref:`ScipyCommitParser <commit-parser-scipy>`
-    * ``tag`` - :ref:`TagCommitParser <commit-parser-tag>`
+.. _`jinja2.Environment`: https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment
 
-You can set any of the built-in parsers by their keyword but you can also specify
-your own commit parser in ``module:attr`` form.
+.. note::
+    **pyproject.toml:** ``[tool.semantic_release.changelog.environment]``
 
-For more information see :ref:`commit-parsing`.
+    **releaserc.toml:** ``[semantic_release.changelog.environment]``
 
-**Default:** ``"angular"``
+    **releaserc.json:** ``{ "semantic_release": { "changelog": { "environment": {} } } }``
 
 ----
 
-.. _config-commit-parser-options:
+.. _config-changelog-environment-autoescape:
 
-``commit_parser_options (Dict[str, Any])``
-""""""""""""""""""""""""""""""""""""""""""
+``autoescape``
+''''''''''''''
 
-These options are passed directly to the ``parser_options`` method of
-:ref:`the commit parser <config-commit-parser>`, without validation
-or transformation.
+**Type:** ``Union[str, bool]``
 
-For more information, see :ref:`commit-parsing-parser-options`.
+If this setting is a string, it should be given in ``module:attr`` form; Python
+Semantic Release will attempt to dynamically import this string, which should
+represent a path to a suitable callable that satisfies the following:
 
-The default value for this setting depends on what you specify as
-:ref:`commit_parser <config-commit-parser>`. The table below outlines
-the expections from ``commit_parser`` value to default options value.
+    As of Jinja 2.4 this can also be a callable that is passed the template name
+    and has to return ``True`` or ``False`` depending on autoescape should be
+    enabled by default.
 
-==================  ==   =================================
-``commit_parser``        Default ``commit_parser_options``
-==================  ==   =================================
-``"angular"``       ->   .. code-block:: toml
+The result of this dynamic import is passed directly to the `jinja2.Environment`_
+constructor.
 
-                             [tool.semantic_release.commit_parser_options]
-                             allowed_types = [
-                                 "build", "chore", "ci", "docs", "feat", "fix",
-                                 "perf", "style", "refactor", "test"
-                             ]
-                             minor_types = ["feat"]
-                             patch_types = ["fix", "perf"]
+If this setting is a boolean, it is passed directly to the `jinja2.Environment`_
+constructor.
 
-``"emoji"``         ->   .. code-block:: toml
+**Default:** ``true``
 
-                             [tool.semantic_release.commit_parser_options]
-                             major_tags = [":boom:"]
-                             minor_tags = [
-                                 ":sparkles:", ":children_crossing:", ":lipstick:",
-                                 ":iphone:", ":egg:", ":chart_with_upwards_trend:"
-                             ]
-                             patch_tags = [
-                                 ":ambulance:", ":lock:", ":bug:", ":zap:", ":goal_net:",
-                                 ":alien:", ":wheelchair:", ":speech_balloon:", ":mag:",
-                                 ":apple:", ":penguin:", ":checkered_flag:", ":robot:",
-                                 ":green_apple:"
-                             ]
+----
 
-``"scipy"``         ->   .. code-block:: toml
+.. _config-changelog-environment-block_start_string:
 
-                             [tool.semantic_release.commit_parser_options]
-                             allowed_tags = [
-                                "API", "DEP", "ENH", "REV", "BUG", "MAINT", "BENCH",
-                                "BLD", "DEV", "DOC", "STY", "TST", "REL", "FEAT", "TEST",
-                             ]
-                             major_tags = ["API",]
-                             minor_tags = ["DEP", "DEV", "ENH", "REV", "FEAT"]
-                             patch_tags = ["BLD", "BUG", "MAINT"]
+``block_start_string``
+''''''''''''''''''''''
 
-``"tag"``           ->   .. code-block:: toml
+**Type:** ``str``
 
-                             [tool.semantic_release.commit_parser_options]
-                             minor_tag = ":sparkles:"
-                             patch_tag = ":nut_and_bolt:"
+This setting is passed directly to the `jinja2.Environment`_ constructor.
 
-``"module:class"``  ->   ``**module:class.parser_options()``
-==================  ==   =================================
+**Default:** ``"{%"``
 
-**Default:** ``ParserOptions { ... }``, where ``...`` depends on
-:ref:`commit_parser <config-commit-parser>` as indicated above.
+----
+
+.. _config-changelog-environment-block_end_string:
+
+``block_end_string``
+''''''''''''''''''''
 
+**Type:** ``str``
+
+This setting is passed directly to the `jinja2.Environment`_ constructor.
+
+**Default:** ``"%}"``
 
 ----
 
-.. _config-logging-use-named-masks:
+.. _config-changelog-environment-comment_start_string:
 
-``logging_use_named_masks (bool)``
-""""""""""""""""""""""""""""""""""
+``comment_start_string``
+''''''''''''''''''''''''
 
-Whether or not to replace secrets identified in logging messages with named masks
-identifying which secrets were replaced, or use a generic string to mask them.
+**Type:** ``str``
 
-**Default:** ``false``
+This setting is passed directly to the `jinja2.Environment`_ constructor.
 
-----
+**Default:** ``{#``
 
-.. _config-allow-zero-version:
+----
 
-``allow_zero_version (bool)``
-"""""""""""""""""""""""""""""
+.. _config-changelog-environment-comment_end_string:
 
-This flag controls whether or not Python Semantic Release will use version
-numbers aligning with the ``0.x.x`` pattern.
+``comment_end_string``
+''''''''''''''''''''''
 
-If set to ``true`` and starting at ``0.0.0``, a minor bump would set the
-next version as ``0.1.0`` whereas a patch bump would set the next version as
-``0.0.1``. A breaking change (ie. major bump) would set the next version as
-``1.0.0`` unless the :ref:`major_on_zero` is set to ``false``.
+**Type:** ``str``
 
-If set to ``false``, Python Semantic Release will consider the first possible
-version to be ``1.0.0``, regardless of patch, minor, or major change level.
-Additionally, when ``allow_zero_version`` is set to ``false``,
-the :ref:`major_on_zero` setting is ignored.
+This setting is passed directly to the `jinja2.Environment`_ constructor.
 
-**Default:** ``true``
+**Default:** ``"#}"``
 
 ----
 
-.. _config-major-on-zero:
+.. _config-changelog-environment-extensions:
 
-``major_on_zero (bool)``
-""""""""""""""""""""""""
+``extensions``
+''''''''''''''
 
-This flag controls whether or not Python Semantic Release will increment the major
-version upon a breaking change when the version matches ``0.y.z``. This value is
-set to ``true`` by default, where breaking changes will increment the ``0`` major
-version to ``1.0.0`` like normally expected.
+**Type:** ``list[str]``
 
-If set to ``false``, major (breaking) releases will increment the minor digit of the
-version while the major version is ``0``, instead of the major digit. This allows for
-continued breaking changes to be made while the major version remains ``0``.
+This setting is passed directly to the `jinja2.Environment`_ constructor.
 
-From the `Semantic Versioning Specification`_:
+**Default:** ``[]``
 
-   Major version zero (0.y.z) is for initial development. Anything MAY change at
-   any time. The public API SHOULD NOT be considered stable.
+----
 
-.. _Semantic Versioning Specification: https://semver.org/spec/v2.0.0.html#spec-item-4
+.. _config-changelog-environment-keep_trailing_newline:
 
-When you are ready to release a stable version, set ``major_on_zero`` to ``true`` and
-run Python Semantic Release again. This will increment the major version to ``1.0.0``.
+``keep_trailing_newline``
+'''''''''''''''''''''''''
 
-When :ref:`allow_zero_version` is set to ``false``, this setting is ignored.
+**Type:** ``bool``
 
-**Default:** ``true``
+This setting is passed directly to the `jinja2.Environment`_ constructor.
+
+**Default:** ``false``
 
 ----
 
-.. _config-tag-format:
+.. _config-changelog-environment-line_comment_prefix:
 
-``tag_format (str)``
-""""""""""""""""""""
+``line_comment_prefix``
+'''''''''''''''''''''''
 
-Specify the format to be used for the Git tag that will be added to the repo during
-a release invoked via :ref:`cmd-version`. The format string is a regular expression,
-which also must include the format keys below, otherwise an exception will be thrown.
-It *may* include any of the optional format keys, in which case the contents
-described will be formatted into the specified location in the Git tag that is created.
+**Type:** ``Optional[str]``
 
-For example, ``"(dev|stg|prod)-v{version}"`` is a valid ``tag_format`` matching tags such
-as:
+This setting is passed directly to the `jinja2.Environment`_ constructor.
 
-- ``dev-v1.2.3``
-- ``stg-v0.1.0-rc.1``
-- ``prod-v2.0.0+20230701``
+**Default:** ``None`` (not specified)
 
-This format will also be used for parsing tags already present in the repository into
-semantic versions; therefore if the tag format changes at some point in the
-repository's history, historic versions that no longer match this pattern will not be
-considered as versions.
+----
 
-================ =========  ========
-Format Key       Mandatory  Contents
-================ =========  ========
-``{version}``    Yes        The new semantic version number, for example ``1.2.3``, or
-                            ``2.1.0-alpha.1+build.1234``
-================ =========  ========
+.. _config-changelog-environment-line_statement_prefix:
 
-Tags which do not match this format will not be considered as versions of your project.
+``line_statement_prefix``
+'''''''''''''''''''''''''
 
-**Default:** ``"v{version}"``
+**Type:** ``Optional[str]``
 
-----
+This setting is passed directly to the `jinja2.Environment`_ constructor.
+
+**Default:** ``None`` (not specified)
 
-.. _config-version-variables:
+----
 
-``version_variables (List[str])``
-"""""""""""""""""""""""""""""""""
+.. _config-changelog-environment-lstrip_blocks:
 
-Each entry represents a location where the version is stored in the source code,
-specified in ``file:variable`` format. For example:
+``lstrip_blocks``
+'''''''''''''''''
 
-.. code-block:: toml
+**Type:** ``bool``
 
-    [tool.semantic_release]
-    version_variables = [
-        "semantic_release/__init__.py:__version__",
-        "docs/conf.py:version",
-    ]
+This setting is passed directly to the `jinja2.Environment`_ constructor.
 
-**Default:** ``[]``
+**Default:** ``false``
 
 ----
 
-.. _config-version-toml:
+.. _config-changelog-environment-newline_sequence:
 
-``version_toml (List[str])``
-""""""""""""""""""""""""""""
-Similar to :ref:`config-version-variables`, but allows the version number to be
-identified safely in a toml file like ``pyproject.toml``, with each entry using
-dotted notation to indicate the key for which the value represents the version:
+``newline_sequence``
+''''''''''''''''''''
 
-.. code-block:: toml
+**Type:** ``Literal["\n", "\r", "\r\n"]``
 
-    [tool.semantic_release]
-    version_toml = [
-        "pyproject.toml:tool.poetry.version",
-    ]
+This setting is passed directly to the `jinja2.Environment`_ constructor.
 
-**Default:** ``[]``
+**Default:** ``"\n"``
 
 ----
 
-.. _config-changelog:
+.. _config-changelog-environment-trim_blocks:
 
-``[tool.semantic_release.changelog]``
-*************************************
+``trim_blocks``
+'''''''''''''''
+
+**Type:** ``bool``
+
+This setting is passed directly to the `jinja2.Environment`_ constructor.
+
+**Default:** ``false``
 
 ----
 
-.. _config-changelog-template-dir:
+.. _config-changelog-environment-variable_start_string:
 
-``template_dir (str)``
-""""""""""""""""""""""
+``variable_start_string``
+'''''''''''''''''''''''''
 
-If given, specifies a directory of templates that will be rendered during creation
-of the changelog. If not given, the default changelog template will be used.
+**Type:** ``str``
 
-This option is discussed in more detail at :ref:`changelog-templates`
+This setting is passed directly to the `jinja2.Environment`_ constructor.
 
-**Default:** ``"templates"``
+**Default:** ``"{{"``
 
 ----
 
-.. _config-changelog-changelog-file:
+.. _config-changelog-environment-variable_end_string:
 
-``changelog_file (str)``
-""""""""""""""""""""""""
+``variable_end_string``
+'''''''''''''''''''''''
 
-Specify the name of the changelog file (after template rendering has taken place).
+**Type:** ``str``
 
-**Default:** ``"CHANGELOG.md"``
+This setting is passed directly to the `jinja2.Environment`_ constructor.
+
+**Default:** ``"}}"``
 
 ----
 
-.. _config-changelog-exclude-commit-patterns:
+.. _config-changelog-exclude_commit_patterns:
+
+``exclude_commit_patterns``
+***************************
 
-``exclude_commit_patterns (List[str])``
-"""""""""""""""""""""""""""""""""""""""
+**Type:** ``list[str]``
 
 Any patterns specified here will be excluded from the commits which are available
 to your changelog. This allows, for example, automated commits to be removed if desired.
 Python Semantic Release also removes its own commits from the Changelog via this mechanism;
 therefore if you change the automated commit message that Python Semantic Release uses when
 making commits, you may wish to add the *old* commit message pattern here.
 
 The patterns in this list are treated as regular expressions.
 
 **Default:** ``[]``
 
 ----
 
-.. _config-changelog-environment:
+.. _config-changelog-template_dir:
 
-``[tool.semantic_release.changelog.environment]``
-*************************************************
+``template_dir``
+****************
 
-.. note::
-   This section of the configuration contains options which customize the template
-   environment used to render templates such as the changelog. Most options are
-   passed directly to the `jinja2.Environment`_ constructor, and further
-   documentation one these parameters can be found there.
+**Type:** ``str``
 
-.. _`jinja2.Environment`: https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment
+If given, specifies a directory of templates that will be rendered during creation
+of the changelog. If not given, the default changelog template will be used.
 
-----
+This option is discussed in more detail at :ref:`changelog-templates`
 
-.. _config-changelog-environment-block-start-string:
+**Default:** ``"templates"``
 
-``block_start_string (str)``
-""""""""""""""""""""""""""""
+----
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+.. _config-commit_author:
 
-**Default:** ``"{%"``
+``commit_author``
+"""""""""""""""""
 
-----
+**Type:** ``str``
 
-.. _config-changelog-environment-block-end-string:
+Author used in commits in the format ``name <email>``.
 
-``block_end_string (str)``
-""""""""""""""""""""""""""
+.. note::
+  If you are using the built-in GitHub Action, the default value is set to
+  ``github-actions <actions@github.com>``. You can modify this with the
+  ``git_committer_name`` and ``git_committer_name`` inputs.
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+.. seealso::
+   - :ref:`github-actions`
 
-**Default:** ``"%}"``
+**Default:** ``semantic-release <semantic-release>``
 
 ----
 
-.. _config-changelog-environment-variable-start-string:
+.. _config-commit_message:
 
-``variable_start_string (str)``
-"""""""""""""""""""""""""""""""
+``commit_message``
+""""""""""""""""""
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+**Type:** ``str``
 
-**Default:** ``"{{"``
+Commit message to use when making release commits. The message can use ``{version}``
+as a format key, in which case the version being released will be formatted into
+the message.
 
-----
+If at some point in your project's lifetime you change this, you may wish to consider,
+adding the old message pattern(s) to :ref:`exclude_commit_patterns <config-changelog-exclude_commit_patterns>`.
 
-.. _config-changelog-environment-variable-end-string:
+**Default:** ``"{version}\n\nAutomatically generated by python-semantic-release"``
 
-``variable_end_string (str)``
-"""""""""""""""""""""""""""""
+----
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+.. _config-commit_parser:
 
-**Default:** ``"}}"``
+``commit_parser``
+"""""""""""""""""
 
-----
+**Type:** ``str``
 
-.. _config-changelog-environment-comment-start-string:
+Specify which commit parser Python Semantic Release should use to parse the commits
+within the Git repository.
 
-``comment_start_string (str)``
-""""""""""""""""""""""""""""""
+Built-in parsers:
+    * ``angular`` - :ref:`AngularCommitParser <commit-parser-angular>`
+    * ``emoji`` - :ref:`EmojiCommitParser <commit-parser-emoji>`
+    * ``scipy`` - :ref:`ScipyCommitParser <commit-parser-scipy>`
+    * ``tag`` - :ref:`TagCommitParser <commit-parser-tag>`
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+You can set any of the built-in parsers by their keyword but you can also specify
+your own commit parser in ``module:attr`` form.
 
-**Default:** ``{#``
+For more information see :ref:`commit-parsing`.
+
+**Default:** ``"angular"``
 
 ----
 
-.. _config-changelog-environment-comment-end-string:
+.. _config-commit_parser_options:
+
+``commit_parser_options``
+"""""""""""""""""""""""""
 
-``comment_end_string (str)``
-""""""""""""""""""""""""""""
+**Type:** ``dict[str, Any]``
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+These options are passed directly to the ``parser_options`` method of
+:ref:`the commit parser <config-commit_parser>`, without validation
+or transformation.
 
-**Default:** ``"#}"``
+For more information, see :ref:`commit-parsing-parser-options`.
 
-----
+The default value for this setting depends on what you specify as
+:ref:`commit_parser <config-commit_parser>`. The table below outlines
+the expections from ``commit_parser`` value to default options value.
 
-.. _config-changelog-environment-line-statement-prefix:
+==================  ==   =================================
+``commit_parser``        Default ``commit_parser_options``
+==================  ==   =================================
+``"angular"``       ->   .. code-block:: toml
 
-``line_statement_prefix (Optional[str])``
-"""""""""""""""""""""""""""""""""""""""""
+                             [semantic_release.commit_parser_options]
+                             allowed_types = [
+                                 "build", "chore", "ci", "docs", "feat", "fix",
+                                 "perf", "style", "refactor", "test"
+                             ]
+                             minor_types = ["feat"]
+                             patch_types = ["fix", "perf"]
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+``"emoji"``         ->   .. code-block:: toml
 
-**Default:** ``None`` (not specified)
+                             [semantic_release.commit_parser_options]
+                             major_tags = [":boom:"]
+                             minor_tags = [
+                                 ":sparkles:", ":children_crossing:", ":lipstick:",
+                                 ":iphone:", ":egg:", ":chart_with_upwards_trend:"
+                             ]
+                             patch_tags = [
+                                 ":ambulance:", ":lock:", ":bug:", ":zap:", ":goal_net:",
+                                 ":alien:", ":wheelchair:", ":speech_balloon:", ":mag:",
+                                 ":apple:", ":penguin:", ":checkered_flag:", ":robot:",
+                                 ":green_apple:"
+                             ]
 
-----
+``"scipy"``         ->   .. code-block:: toml
 
-.. _config-changelog-environment-line-comment-prefix:
+                             [semantic_release.commit_parser_options]
+                             allowed_tags = [
+                                "API", "DEP", "ENH", "REV", "BUG", "MAINT", "BENCH",
+                                "BLD", "DEV", "DOC", "STY", "TST", "REL", "FEAT", "TEST",
+                             ]
+                             major_tags = ["API",]
+                             minor_tags = ["DEP", "DEV", "ENH", "REV", "FEAT"]
+                             patch_tags = ["BLD", "BUG", "MAINT"]
 
-``line_comment_prefix (Optional[str])``
-"""""""""""""""""""""""""""""""""""""""
+``"tag"``           ->   .. code-block:: toml
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+                             [semantic_release.commit_parser_options]
+                             minor_tag = ":sparkles:"
+                             patch_tag = ":nut_and_bolt:"
 
-**Default:** ``None`` (not specified)
+``"module:class"``  ->   ``**module:class.parser_options()``
+==================  ==   =================================
+
+**Default:** ``ParserOptions { ... }``, where ``...`` depends on
+:ref:`config-commit_parser` as indicated above.
 
 ----
 
-.. _config-changelog-environment-trim-blocks:
+.. _config-logging_use_named_masks:
 
-``trim_blocks (bool)``
-""""""""""""""""""""""
+``logging_use_named_masks``
+"""""""""""""""""""""""""""
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+**Type:** ``bool``
+
+Whether or not to replace secrets identified in logging messages with named masks
+identifying which secrets were replaced, or use a generic string to mask them.
 
 **Default:** ``false``
 
 ----
 
-.. _config-changelog-environment-lstrip-blocks:
+.. _config-major_on_zero:
 
-``lstrip_blocks (bool)``
-""""""""""""""""""""""""
+``major_on_zero``
+"""""""""""""""""
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+**Type:** ``bool``
 
-**Default:** ``false``
+This flag controls whether or not Python Semantic Release will increment the major
+version upon a breaking change when the version matches ``0.y.z``. This value is
+set to ``true`` by default, where breaking changes will increment the ``0`` major
+version to ``1.0.0`` like normally expected.
 
-----
+If set to ``false``, major (breaking) releases will increment the minor digit of the
+version while the major version is ``0``, instead of the major digit. This allows for
+continued breaking changes to be made while the major version remains ``0``.
+
+From the `Semantic Versioning Specification`_:
 
-.. _config-changelog-environment-newline-sequence:
+   Major version zero (0.y.z) is for initial development. Anything MAY change at
+   any time. The public API SHOULD NOT be considered stable.
 
-``newline_sequence (Literal["\n", "\r", "\r\n"])``
-""""""""""""""""""""""""""""""""""""""""""""""""""
+.. _Semantic Versioning Specification: https://semver.org/spec/v2.0.0.html#spec-item-4
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+When you are ready to release a stable version, set ``major_on_zero`` to ``true`` and
+run Python Semantic Release again. This will increment the major version to ``1.0.0``.
 
-**Default:** ``"\n"``
+When :ref:`config-allow_zero_version` is set to ``false``, this setting is ignored.
+
+**Default:** ``true``
 
 ----
 
-.. _config-changelog-environment-keep-trailing-newline:
+.. _config-publish:
 
-``keep_trailing_newline (bool)``
-""""""""""""""""""""""""""""""""
+``publish``
+"""""""""""
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+This section defines configuration options that modify :ref:`cmd-publish`.
 
-**Default:** ``false``
+.. note::
+    **pyproject.toml:** ``[tool.semantic_release.publish]``
 
-----
+    **releaserc.toml:** ``[semantic_release.publish]``
 
-.. _config-changelog-environment-extensions:
+    **releaserc.json:** ``{ "semantic_release": { "publish": {} } }``
 
-``extensions (List[str])``
-""""""""""""""""""""""""""
+----
 
-This setting is passed directly to the `jinja2.Environment`_ constructor.
+.. _config-publish-dist_glob_patterns:
 
-**Default:** ``[]``
+``dist_glob_patterns``
+**********************
 
-----
+**Type:** ``list[str]``
 
-.. _config-changelog-environment-autoescape:
+Upload any files matching any of these globs to your VCS release. Each item in this
+list should be a string containing a Unix-style glob pattern.
 
-``autoescape (Union[str, bool])``
-""""""""""""""""""""""""""""""""""
+**Default:** ``["dist/*"]``
 
-If this setting is a string, it should be given in ``module:attr`` form; Python
-Semantic Release will attempt to dynamically import this string, which should
-represent a path to a suitable callable that satisfies the following:
+----
 
-    As of Jinja 2.4 this can also be a callable that is passed the template name
-    and has to return ``True`` or ``False`` depending on autoescape should be
-    enabled by default.
+.. _config-publish-upload_to_vcs_release:
 
-The result of this dynamic import is passed directly to the `jinja2.Environment`_
-constructor.
+``upload_to_vcs_release``
+*************************
 
-If this setting is a boolean, it is passed directly to the `jinja2.Environment`_
-constructor.
+**Type:** ``bool``
+
+If set to ``true``, upload any artifacts matched by the
+:ref:`dist_glob_patterns <config-publish-dist_glob_patterns>` to the release created
+in the remote VCS corresponding to the latest tag. Artifacts are only uploaded if
+release artifact uploads are supported by the :ref:`VCS type <config-remote-type>`.
 
 **Default:** ``true``
 
 ----
 
 .. _config-remote:
 
 ``remote``
-**********
+""""""""""
 
-.. note::
-    The remote configuration is a group of settings that configure PSR's integration
-    with remote version control systems.
+The remote configuration is a group of settings that configure PSR's integration
+with remote version control systems.
 
+.. note::
     **pyproject.toml:** ``[tool.semantic_release.remote]``
 
+    **releaserc.toml:** ``[semantic_release.remote]``
+
+    **releaserc.json:** ``{ "semantic_release": { "remote": {} } }``
+
 ----
 
 .. _config-remote-api_domain:
 
 ``api_domain``
-""""""""""""""
+**************
 
 **Type:** ``Optional[str | Dict['env', str]]``
 
 The hosting domain for the API of your remote HVCS if different than the ``domain``.
 Generally, this will be used to specify a separate subdomain that is used for API
 calls rather than the primary domain (ex. ``api.github.com``).
 
@@ -717,15 +800,15 @@
 **Default:** ``None``
 
 ----
 
 .. _config-remote-domain:
 
 ``domain``
-""""""""""
+**********
 
 **Type:** ``Optional[str | Dict['env', str]]``
 
 The host domain for your HVCS server. This setting is used to support on-premise
 installations of HVCS providers with custom domain hosts.
 
 If you are using the official domain of the associated
@@ -745,37 +828,37 @@
 be checked so this value is not required in default environments.  For example, when
 ``remote.type="gitlab"`` is specified, PSR will look to the ``CI_SERVER_URL`` environment
 variable when ``remote.domain`` is not specified.
 
 **Default:** ``None``
 
 .. seealso::
-   - :ref:`remote.api_domain <config-remote-api-domain>`
+   - :ref:`remote.api_domain <config-remote-api_domain>`
 
 ----
 
-.. _config-remote-ignore-token-for-push:
+.. _config-remote-ignore_token_for_push:
 
 ``ignore_token_for_push``
-"""""""""""""""""""""""""
+*************************
 
 **Type:** ``bool``
 
 If set to ``True``, ignore the authentication token when pushing changes to the remote.
 This is ideal, for example, if you already have SSH keys set up which can be used for
 pushing.
 
 **Default:** ``False``
 
 ----
 
 .. _config-remote-insecure:
 
 ``insecure``
-""""""""""""
+************
 
 **Type:** ``bool``
 
 Insecure is used to allow non-secure ``HTTP`` connections to your HVCS server. If set to
 ``True``, any domain value passed will assume ``http://`` if it is not specified and allow
 it. When set to ``False`` (implicitly or explicitly), it will force ``https://`` communications.
 
@@ -792,63 +875,28 @@
 **Default:** ``False``
 
 ----
 
 .. _config-remote-name:
 
 ``name``
-""""""""
+********
 
 **Type:** ``str``
 
 Name of the remote to push to using ``git push -u $name <branch_name>``
 
 **Default:** ``"origin"``
 
 ----
 
-.. _config-remote-url:
-
-``url``
-"""""""
-
-**Type:** ``Optional[str | Dict['env', str]]``
-
-An override setting used to specify the remote upstream location of ``git push``.
-
-**Not commonly used!** This is used to override the derived upstream location when
-the desired push location is different than the location the repository was cloned
-from.
-
-This setting will override the upstream location url that would normally be derived
-from the :ref:`remote.name <config-remote-name>` location of your git repository.
-
-**Default:** ``None``
-
-----
-
-.. _config-remote-type:
-
-``type``
-""""""""
-
-**Type:** ``Literal["bitbucket", "gitea", "github", "gitlab"]``
-
-The type of the remote VCS. Currently, Python Semantic Release supports ``"github"``,
-``"gitlab"``, ``"gitea"`` and ``"bitbucket"``. Not all functionality is available with all
-remote types, but we welcome pull requests to help improve this!
-
-**Default:** ``"github"``
-
-----
-
 .. _config-remote-token:
 
 ``token``
-"""""""""
+*********
 
 **Type:** ``Optional[str | Dict['env', str]]``
 
 :ref:`Environment Variable <config-environment-variables>` from which to source the
 authentication token for the remote VCS. Common examples include ``"GH_TOKEN"``,
 ``"GITLAB_TOKEN"`` or ``"GITEA_TOKEN"``, however, you may choose to use a custom
 environment variable if you wish.
@@ -881,37 +929,121 @@
 ================  ==  ===============================
 
 **Default:** ``{ env = "<envvar name>" }``, where ``<envvar name>`` depends on
 :ref:`remote.type <config-remote-type>` as indicated above.
 
 ----
 
-.. _config-publish:
+.. _config-remote-type:
 
-``[tool.semantic_release.publish]``
-***********************************
+``type``
+********
+
+**Type:** ``Literal["bitbucket", "gitea", "github", "gitlab"]``
+
+The type of the remote VCS. Currently, Python Semantic Release supports ``"github"``,
+``"gitlab"``, ``"gitea"`` and ``"bitbucket"``. Not all functionality is available with all
+remote types, but we welcome pull requests to help improve this!
+
+**Default:** ``"github"``
 
 ----
 
-.. _config-publish-dist-glob-patterns:
+.. _config-remote-url:
 
-``dist_glob_patterns (List[str])``
-""""""""""""""""""""""""""""""""""
+``url``
+*******
 
-Upload any files matching any of these globs to your VCS release. Each item in this
-list should be a string containing a Unix-style glob pattern.
+**Type:** ``Optional[str | Dict['env', str]]``
 
-**Default:** ``["dist/*"]``
+An override setting used to specify the remote upstream location of ``git push``.
+
+**Not commonly used!** This is used to override the derived upstream location when
+the desired push location is different than the location the repository was cloned
+from.
+
+This setting will override the upstream location url that would normally be derived
+from the :ref:`remote.name <config-remote-name>` location of your git repository.
+
+**Default:** ``None``
 
 ----
 
-.. _config-publish-upload-to-vcs-release:
+.. _config-tag_format:
 
-``upload_to_vcs_release (bool)``
-""""""""""""""""""""""""""""""""
+``tag_format``
+""""""""""""""
 
-If set to ``true``, upload any artifacts matched by the
-:ref:`dist_glob_patterns <config-publish-dist-glob-patterns>` to the release created
-in the remote VCS corresponding to the latest tag. Artifacts are only uploaded if
-release artifact uploads are supported by the :ref:`VCS type <config-remote-type>`.
+**Type:** ``str``
 
-**Default:** ``true``
+Specify the format to be used for the Git tag that will be added to the repo during
+a release invoked via :ref:`cmd-version`. The format string is a regular expression,
+which also must include the format keys below, otherwise an exception will be thrown.
+It *may* include any of the optional format keys, in which case the contents
+described will be formatted into the specified location in the Git tag that is created.
+
+For example, ``"(dev|stg|prod)-v{version}"`` is a valid ``tag_format`` matching tags such
+as:
+
+- ``dev-v1.2.3``
+- ``stg-v0.1.0-rc.1``
+- ``prod-v2.0.0+20230701``
+
+This format will also be used for parsing tags already present in the repository into
+semantic versions; therefore if the tag format changes at some point in the
+repository's history, historic versions that no longer match this pattern will not be
+considered as versions.
+
+================ =========  ==========================================================
+Format Key       Mandatory  Contents
+================ =========  ==========================================================
+``{version}``    Yes        The new semantic version number, for example ``1.2.3``, or
+                            ``2.1.0-alpha.1+build.1234``
+================ =========  ==========================================================
+
+Tags which do not match this format will not be considered as versions of your project.
+
+**Default:** ``"v{version}"``
+
+----
+
+.. _config-version_toml:
+
+``version_toml``
+""""""""""""""""
+
+**Type:** ``list[str]``
+
+Similar to :ref:`config-version_variables`, but allows the version number to be
+identified safely in a toml file like ``pyproject.toml``, with each entry using
+dotted notation to indicate the key for which the value represents the version:
+
+.. code-block:: toml
+
+    [semantic_release]
+    version_toml = [
+        "pyproject.toml:tool.poetry.version",
+    ]
+
+**Default:** ``[]``
+
+----
+
+.. _config-version_variables:
+
+``version_variables``
+"""""""""""""""""""""
+
+**Type:** ``list[str]``
+
+Each entry represents a location where the version is stored in the source code,
+specified in ``file:variable`` format. For example:
+
+.. code-block:: toml
+
+    [semantic_release]
+    version_variables = [
+        "semantic_release/__init__.py:__version__",
+        "docs/conf.py:version",
+    ]
+
+**Default:** ``[]``
```

### Comparing `python_semantic_release-9.7.1/docs/github-action.rst` & `python_semantic_release-9.7.2/docs/github-action.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/docs/index.rst` & `python_semantic_release-9.7.2/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
       # And so on...
    )
 
 Python Semantic Release can be configured using a TOML or JSON file; the default configuration file is
 ``pyproject.toml``, if you wish to use another file you will need to use the ``-c/--config`` option to
 specify the file.
 
-Set :ref:`version_variables <config-version-variables>` to a list, the only element of which should be the location of your
+Set :ref:`version_variables <config-version_variables>` to a list, the only element of which should be the location of your
 version variable inside any Python file, specified in standard ``module:attribute`` syntax:
 
 ``pyproject.toml``::
 
    [tool.semantic_release]
    version_variables = ["setup.py:__version__"]
 
@@ -92,15 +92,15 @@
 We rely on commit messages to detect when a version bump is needed.
 By default, Python Semantic Release uses the
 `Angular style <https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#commits>`_.
 You can find out more about this in :ref:`commit-parsing`.
 
 .. seealso::
    - :ref:`config-branches` - Adding configuration for releases from multiple branches.
-   - :ref:`commit_parser <config-commit-parser>` - use a different parser for commit messages.
+   - :ref:`commit_parser <config-commit_parser>` - use a different parser for commit messages.
      For example, Python Semantic Release also ships with emoji and scipy-style parsers.
    - :ref:`remote.type <config-remote-type>` - specify the type of your remote VCS.
 
 Setting up the changelog
 ------------------------
 
 .. seealso::
@@ -155,15 +155,15 @@
 .. _App Secret: https://support.atlassian.com/bitbucket-cloud/docs/push-back-to-your-repository/#App-secret
 .. _Access Token: https://support.atlassian.com/bitbucket-cloud/docs/repository-access-tokens
 
 .. seealso::
    - :ref:`Changelog <config-changelog>` - customize your project's changelog.
    - :ref:`Customizing VCS Release Notes <changelog-templates-customizing-vcs-release-notes>` - customize
      the VCS release notes.
-   - :ref:`upload_to_vcs_release <config-publish-upload-to-vcs-release>` -
+   - :ref:`upload_to_vcs_release <config-publish-upload_to_vcs_release>` -
      enable/disable uploading artefacts to VCS releases
    - :ref:`version --vcs-release/--no-vcs-release <cmd-version-option-vcs-release>` - enable/disable VCS release
      creation.
    - `upload-to-gh-release`_, a GitHub Action for running ``semantic-release publish``
 
 .. _upload-to-gh-release: https://github.com/python-semantic-release/upload-to-gh-release
```

### Comparing `python_semantic_release-9.7.1/docs/make.bat` & `python_semantic_release-9.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/docs/migrating_from_v7.rst` & `python_semantic_release-9.7.2/docs/migrating_from_v7.rst`

 * *Files 0% similar despite different names*

```diff
@@ -538,25 +538,25 @@
 """""""""""""""""""""
 
 Options such as ``major_emoji``, ``parser_angular_patch_types`` or
 ``parser_angular_default_level_bump`` have been removed. Instead, these have been
 replaced with a single set of recognised commit parser options, ``allowed_tags``,
 ``major_tags``, ``minor_tags``, and ``patch_tags``, though the interpretation of
 these is up to the specific parsers in use. You can read more detail about using
-commit parser options in :ref:`commit_parser_options <config-commit-parser-options>`,
+commit parser options in :ref:`commit_parser_options <config-commit_parser_options>`,
 and if you need to parse multiple commit styles for a single project it's recommended
 that you create a parser following :ref:`commit-parser-writing-your-own-parser` that
 is tailored to the specific needs of your project.
 
 .. _breaking-version-variable-rename:
 
 ``version_variable``
 """"""""""""""""""""
 
-This option has been renamed to :ref:`version_variables <config-version-variables>`
+This option has been renamed to :ref:`version_variables <config-version_variables>`
 as it refers to a list of variables which can be updated.
 
 .. _breaking-version-pattern-removed:
 
 ``version_pattern``
 """""""""""""""""""
 
@@ -599,15 +599,15 @@
 
 .. _breaking-upload-to-release-rename:
 
 ``upload_to_release``
 """""""""""""""""""""
 
 This option has been renamed to
-:ref:`upload_to_vcs_release <config-publish-upload-to-vcs-release>`.
+:ref:`upload_to_vcs_release <config-publish-upload_to_vcs_release>`.
 
 .. _breaking-custom-commit-parsers:
 
 Custom Commit Parsers
 ---------------------
 
 Previously, a custom commit parser had to satisfy the following criteria:
```

### Comparing `python_semantic_release-9.7.1/docs/multibranch_releases.rst` & `python_semantic_release-9.7.2/docs/multibranch_releases.rst`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 but when merged to the branch configured to produce full releases (``main``), if
 released separately the changes from each branch would be released in two versions
 that would be considered different according to the semver specification.
 
 .. note::
 
    If you have tags in your Git repository that are not valid semantic versions
-   (which have then been formatted into your :ref:`tag_format <config-tag-format>`),
+   (which have then been formatted into your :ref:`tag_format <config-tag_format>`),
    these tags will be ignored for the purposes of calculating the next version.
 
 .. _prereleases: https://semver.org/#spec-item-9
 .. _build metadata MUST be ignored: https://semver.org/#spec-item-10
 
 .. _multibranch-releases-configuring:
```

### Comparing `python_semantic_release-9.7.1/docs/strict_mode.rst` & `python_semantic_release-9.7.2/docs/strict_mode.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/docs/troubleshooting.rst` & `python_semantic_release-9.7.2/docs/troubleshooting.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _troubleshooting:
 
 Troubleshooting
 ===============
 
 - Check your configuration file for :ref:`configuration`
-- Check your Git tags match your :ref:`tag_format <config-tag-format>`; tags using
+- Check your Git tags match your :ref:`tag_format <config-tag_format>`; tags using
   other formats are ignored during calculation of the next version.
 
 .. _troubleshooting-verbosity:
 
 Increasing Verbosity
 ====================
 If you are having trouble with Python Semantic Release or would like to see additional
```

### Comparing `python_semantic_release-9.7.1/pyproject.toml` & `python_semantic_release-9.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools ~= 69.0", "wheel ~= 0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "9.7.1"
+version = "9.7.2"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
@@ -44,14 +44,17 @@
 changelog = "https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md"
 documentation = "https://python-semantic-release.readthedocs.io"
 homepage = "https://python-semantic-release.readthedocs.io"
 issues = "https://github.com/python-semantic-release/python-semantic-release/issues"
 repository = "http://github.com/python-semantic-release/python-semantic-release.git"
 
 [project.optional-dependencies]
+build = [
+  "build ~= 1.2"
+]
 docs = [
   "Sphinx ~= 6.0",
   "sphinxcontrib-apidoc == 0.5.0",
   "sphinx-autobuild == 2024.2.4",
   "furo ~= 2024.1",
 ]
 test = [
@@ -364,15 +367,15 @@
 [tool.vulture]
 ignore_names = ["change_to_ex_proj_dir", "init_example_project"]
 
 [tool.semantic_release]
 logging_use_named_masks = true
 commit_parser = "angular"
 build_command = """
-    python -m pip install build~=0.10.0
+    python -m pip install -e .[build]
     python -m build .
 """
 major_on_zero = true
 version_variables = ["semantic_release/__init__.py:__version__"]
 version_toml = ["pyproject.toml:project.version"]
 
 [tool.semantic_release.changelog]
```

### Comparing `python_semantic_release-9.7.1/python_semantic_release.egg-info/PKG-INFO` & `python_semantic_release-9.7.2/python_semantic_release.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.7.1
+Version: 9.7.2
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -28,14 +28,16 @@
 Requires-Dist: python-gitlab~=4.0
 Requires-Dist: tomlkit~=0.11
 Requires-Dist: dotty-dict~=1.3
 Requires-Dist: importlib-resources~=6.0
 Requires-Dist: pydantic~=2.0
 Requires-Dist: rich~=13.0
 Requires-Dist: shellingham~=1.5
+Provides-Extra: build
+Requires-Dist: build~=1.2; extra == "build"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=6.0; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc==0.5.0; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
 Requires-Dist: furo~=2024.1; extra == "docs"
 Provides-Extra: test
 Requires-Dist: coverage[toml]~=7.0; extra == "test"
```

### Comparing `python_semantic_release-9.7.1/python_semantic_release.egg-info/SOURCES.txt` & `python_semantic_release-9.7.2/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/python_semantic_release.egg-info/requires.txt` & `python_semantic_release-9.7.2/python_semantic_release.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 tomlkit~=0.11
 dotty-dict~=1.3
 importlib-resources~=6.0
 pydantic~=2.0
 rich~=13.0
 shellingham~=1.5
 
+[build]
+build~=1.2
+
 [dev]
 pre-commit~=3.5
 tox~=4.11
 ruff==0.4.3
 
 [docs]
 Sphinx~=6.0
```

### Comparing `python_semantic_release-9.7.1/semantic_release/__init__.py` & `python_semantic_release-9.7.2/semantic_release/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from semantic_release.version import (
     Version,
     VersionTranslator,
     next_version,
     tags_and_versions,
 )
 
-__version__ = "9.7.1"
+__version__ = "9.7.2"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python_semantic_release-9.7.1/semantic_release/changelog/context.py` & `python_semantic_release-9.7.2/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/changelog/release_history.py` & `python_semantic_release-9.7.2/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/changelog/template.py` & `python_semantic_release-9.7.2/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/commands/changelog.py` & `python_semantic_release-9.7.2/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/commands/cli_context.py` & `python_semantic_release-9.7.2/semantic_release/cli/commands/cli_context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/commands/generate_config.py` & `python_semantic_release-9.7.2/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/commands/main.py` & `python_semantic_release-9.7.2/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/commands/publish.py` & `python_semantic_release-9.7.2/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/commands/version.py` & `python_semantic_release-9.7.2/semantic_release/cli/commands/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
             shell(
                 build_command,
                 check=True,
                 env=dict(
                     filter(
                         lambda k_v: k_v[1] is not None,  # type: ignore
                         {
-                            "NEW_VERSION": str(new_version),
+                            # Common values
                             "PATH": os.getenv("PATH", ""),
                             "HOME": os.getenv("HOME", None),
                             "VIRTUAL_ENV": os.getenv("VIRTUAL_ENV", None),
                             # affects build decisions
                             "CI": os.getenv("CI", None),
                             # Identifies which CI environment
                             "GITHUB_ACTIONS": os.getenv("GITHUB_ACTIONS", None),
@@ -531,14 +531,18 @@
                                 str(True).lower()
                                 if os.getenv("BITBUCKET_REPO_FULL_NAME", None)
                                 else None
                             ),
                             "PSR_DOCKER_GITHUB_ACTION": os.getenv(
                                 "PSR_DOCKER_GITHUB_ACTION", None
                             ),
+                            # User defined overrides of environment (from config)
+                            **runtime.build_command_env,
+                            # PSR injected environment variables
+                            "NEW_VERSION": str(new_version),
                         }.items(),
                     )
                 ),
             )
         except subprocess.CalledProcessError as exc:
             ctx.fail(str(exc))
```

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/common.py` & `python_semantic_release-9.7.2/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/config.py` & `python_semantic_release-9.7.2/semantic_release/cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,14 +208,15 @@
     upload_to_vcs_release: bool = True
 
 
 class RawConfig(BaseModel):
     assets: List[str] = []
     branches: Dict[str, BranchConfig] = {"main": BranchConfig()}
     build_command: Optional[str] = None
+    build_command_env: List[str] = []
     changelog: ChangelogConfig = ChangelogConfig()
     commit_author: MaybeFromEnv = EnvConfigVar(
         env="GIT_COMMIT_AUTHOR", default=DEFAULT_COMMIT_AUTHOR
     )
     commit_message: str = COMMIT_MESSAGE
     commit_parser: NonEmptyString = "angular"
     # It's up to the parser_options() method to validate these
@@ -225,14 +226,19 @@
     allow_zero_version: bool = True
     remote: RemoteConfig = RemoteConfig()
     tag_format: str = "v{version}"
     publish: PublishConfig = PublishConfig()
     version_toml: Optional[Tuple[str, ...]] = None
     version_variables: Optional[Tuple[str, ...]] = None
 
+    @field_validator("build_command_env", mode="after")
+    @classmethod
+    def remove_whitespace(cls, val: list[str]) -> list[str]:
+        return [entry.strip() for entry in val]
+
     @model_validator(mode="after")
     def set_default_opts(self) -> Self:
         # Set the default parser options for the given commit parser when no user input is given
         if not self.commit_parser_options and self.commit_parser:
             parser_opts_type = None
             # If the commit parser is a known one, pull the default options object from it
             if self.commit_parser in _known_commit_parsers:
@@ -348,14 +354,15 @@
     version_declarations: Tuple[VersionDeclarationABC, ...]
     hvcs_client: hvcs.HvcsBase
     changelog_file: Path
     ignore_token_for_push: bool
     template_environment: Environment
     template_dir: Path
     build_command: Optional[str]
+    build_command_env: dict[str, str]
     dist_glob_patterns: Tuple[str, ...]
     upload_to_vcs_release: bool
     global_cli_options: GlobalCommandLineOptions
     # This way the filter can be passed around if needed, so that another function
     # can accept the filter as an argument and call
     masker: MaskingFilter
 
@@ -537,21 +544,47 @@
         )
 
         # version_translator
         version_translator = VersionTranslator(
             tag_format=raw.tag_format, prerelease_token=branch_config.prerelease_token
         )
 
+        build_cmd_env = {}
+
+        for i, env_var_def in enumerate(raw.build_command_env):
+            # creative hack to handle, missing =, but also = that then can be unpacked
+            # as the resulting parts array can be either 2 or 3 in length. it becomes 3
+            # with our forced empty value at the end which can be dropped
+            parts = [*env_var_def.split("=", 1), ""]
+            # removes any odd spacing around =, and extracts name=value
+            name, env_val = [part.strip() for part in parts[:2]]
+
+            if not name:
+                # Skip when invalid format (ex. starting with = and no name)
+                logging.warning(
+                    "Skipping invalid build_command_env[%s] definition",
+                    i,
+                )
+                continue
+
+            if not env_val and env_var_def[-1] != "=":
+                # avoid the edge case that user wants to define a value as empty
+                # and don't autoresolve it
+                env_val = os.getenv(name, "")
+
+            build_cmd_env[name] = env_val
+
         self = cls(
             repo=repo,
             commit_parser=commit_parser,
             version_translator=version_translator,
             major_on_zero=raw.major_on_zero,
             allow_zero_version=raw.allow_zero_version,
             build_command=raw.build_command,
+            build_command_env=build_cmd_env,
             version_declarations=tuple(version_declarations),
             hvcs_client=hvcs_client,
             changelog_file=changelog_file,
             assets=raw.assets,
             commit_author=commit_author,
             commit_message=raw.commit_message,
             changelog_excluded_commit_patterns=changelog_excluded_commit_patterns,
```

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/github_actions_output.py` & `python_semantic_release-9.7.2/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/masking_filter.py` & `python_semantic_release-9.7.2/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/cli/util.py` & `python_semantic_release-9.7.2/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/commit_parser/__init__.py` & `python_semantic_release-9.7.2/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/commit_parser/_base.py` & `python_semantic_release-9.7.2/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/commit_parser/angular.py` & `python_semantic_release-9.7.2/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/commit_parser/emoji.py` & `python_semantic_release-9.7.2/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/commit_parser/scipy.py` & `python_semantic_release-9.7.2/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/commit_parser/tag.py` & `python_semantic_release-9.7.2/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/commit_parser/token.py` & `python_semantic_release-9.7.2/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/commit_parser/util.py` & `python_semantic_release-9.7.2/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/const.py` & `python_semantic_release-9.7.2/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/data/templates/CHANGELOG.md.j2` & `python_semantic_release-9.7.2/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/enums.py` & `python_semantic_release-9.7.2/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/errors.py` & `python_semantic_release-9.7.2/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/helpers.py` & `python_semantic_release-9.7.2/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/hvcs/_base.py` & `python_semantic_release-9.7.2/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/hvcs/bitbucket.py` & `python_semantic_release-9.7.2/semantic_release/hvcs/bitbucket.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/hvcs/gitea.py` & `python_semantic_release-9.7.2/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/hvcs/github.py` & `python_semantic_release-9.7.2/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/hvcs/gitlab.py` & `python_semantic_release-9.7.2/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/hvcs/remote_hvcs_base.py` & `python_semantic_release-9.7.2/semantic_release/hvcs/remote_hvcs_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/hvcs/token_auth.py` & `python_semantic_release-9.7.2/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/hvcs/util.py` & `python_semantic_release-9.7.2/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/version/algorithm.py` & `python_semantic_release-9.7.2/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/version/declaration.py` & `python_semantic_release-9.7.2/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/version/translator.py` & `python_semantic_release-9.7.2/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/semantic_release/version/version.py` & `python_semantic_release-9.7.2/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/command_line/conftest.py` & `python_semantic_release-9.7.2/tests/command_line/conftest.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/command_line/test_changelog.py` & `python_semantic_release-9.7.2/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/command_line/test_generate_config.py` & `python_semantic_release-9.7.2/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/command_line/test_help.py` & `python_semantic_release-9.7.2/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/command_line/test_main.py` & `python_semantic_release-9.7.2/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/command_line/test_publish.py` & `python_semantic_release-9.7.2/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/command_line/test_version.py` & `python_semantic_release-9.7.2/tests/command_line/test_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -547,15 +547,14 @@
     assert result.stdout == "1.2.0-alpha.2\n"
 
 
 @pytest.mark.parametrize("shell", ("/usr/bin/bash", "/usr/bin/zsh", "powershell"))
 def test_version_runs_build_command(
     repo_with_git_flow_angular_commits: Repo,
     cli_runner: CliRunner,
-    example_pyproject_toml: Path,
     update_pyproject_toml: UpdatePyprojectTomlFn,
     shell: str,
 ):
     # Setup
     build_command = "bash -c \"echo 'hello world'\""
     update_pyproject_toml("tool.semantic_release.build_command", build_command)
     exe = shell.split("/")[-1]
@@ -600,14 +599,100 @@
                 "PSR_DOCKER_GITHUB_ACTION": patched_os_environment[
                     "PSR_DOCKER_GITHUB_ACTION"
                 ],
             },
         )
 
 
+def test_version_runs_build_command_w_user_env(
+    repo_with_git_flow_angular_commits: Repo,
+    cli_runner: CliRunner,
+    update_pyproject_toml: UpdatePyprojectTomlFn,
+):
+    # Setup
+    patched_os_environment = {
+        "CI": "true",
+        "PATH": os.getenv("PATH"),
+        "HOME": os.getenv("HOME"),
+        "VIRTUAL_ENV": os.getenv("VIRTUAL_ENV", "./.venv"),
+        # Simulate that all CI's are set
+        "GITHUB_ACTIONS": "true",
+        "GITLAB_CI": "true",
+        "GITEA_ACTIONS": "true",
+        "BITBUCKET_REPO_FULL_NAME": "python-semantic-release/python-semantic-release.git",
+        "PSR_DOCKER_GITHUB_ACTION": "true",
+        # User environment variables (varying passthrough results)
+        "MY_CUSTOM_VARIABLE": "custom",
+        "IGNORED_VARIABLE": "ignore_me",
+        "OVERWRITTEN_VAR": "initial",
+        "SET_AS_EMPTY_VAR": "not_empty",
+    }
+    build_command = "bash -c \"echo 'hello world'\""
+    update_pyproject_toml("tool.semantic_release.build_command", build_command)
+    update_pyproject_toml(
+        "tool.semantic_release.build_command_env",
+        [
+            # Includes arbitrary whitespace which will be removed
+            " MY_CUSTOM_VARIABLE ",  # detect and pass from environment
+            " OVERWRITTEN_VAR = overrided",  # pass hardcoded value which overrides environment
+            " SET_AS_EMPTY_VAR = ",  # keep variable initialized but as empty string
+            " HARDCODED_VAR=hardcoded ",  # pass hardcoded value that doesn't override anything
+            "VAR_W_EQUALS = a-var===condition",  # only splits on 1st equals sign
+            "=ignored-invalid-named-var",  # TODO: validation error instead, but currently just ignore
+        ],
+    )
+
+    # Mock out subprocess.run
+    with mock.patch(
+        "subprocess.run", return_value=CompletedProcess(args=(), returncode=0)
+    ) as patched_subprocess_run, mock.patch(
+        "shellingham.detect_shell", return_value=("bash", "/usr/bin/bash")
+    ), mock.patch.dict("os.environ", patched_os_environment, clear=True):
+        # ACT: run & force a new version that will trigger the build command
+        result = cli_runner.invoke(
+            main,
+            [
+                version_subcmd,
+                "--patch",
+                "--no-commit",
+                "--no-tag",
+                "--no-changelog",
+                "--no-push",
+            ],
+        )
+
+        patched_subprocess_run.assert_called_once_with(
+            ["bash", "-c", build_command],
+            check=True,
+            env={
+                "NEW_VERSION": "1.2.1",  # injected into environment
+                "CI": patched_os_environment["CI"],
+                "BITBUCKET_CI": "true",  # Converted
+                "GITHUB_ACTIONS": patched_os_environment["GITHUB_ACTIONS"],
+                "GITEA_ACTIONS": patched_os_environment["GITEA_ACTIONS"],
+                "GITLAB_CI": patched_os_environment["GITLAB_CI"],
+                "HOME": patched_os_environment["HOME"],
+                "PATH": patched_os_environment["PATH"],
+                "VIRTUAL_ENV": patched_os_environment["VIRTUAL_ENV"],
+                "PSR_DOCKER_GITHUB_ACTION": patched_os_environment[
+                    "PSR_DOCKER_GITHUB_ACTION"
+                ],
+                "MY_CUSTOM_VARIABLE": patched_os_environment["MY_CUSTOM_VARIABLE"],
+                "OVERWRITTEN_VAR": "overrided",
+                "SET_AS_EMPTY_VAR": "",
+                "HARDCODED_VAR": "hardcoded",
+                # Note that IGNORED_VARIABLE is not here.
+                "VAR_W_EQUALS": "a-var===condition",
+            },
+        )
+
+        # Make sure it did not error internally
+        assert result.exit_code == 0
+
+
 def test_version_skips_build_command_with_skip_build(
     repo_with_git_flow_angular_commits, cli_runner
 ):
     with mock.patch(
         "subprocess.run", return_value=CompletedProcess(args=(), returncode=0)
     ) as patched_subprocess_run:
         result = cli_runner.invoke(
```

### Comparing `python_semantic_release-9.7.1/tests/conftest.py` & `python_semantic_release-9.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/const.py` & `python_semantic_release-9.7.2/tests/const.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/commit_parsers.py` & `python_semantic_release-9.7.2/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/example_project.py` & `python_semantic_release-9.7.2/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/git_repo.py` & `python_semantic_release-9.7.2/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py` & `python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py` & `python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/repos/github_flow/repo_w_release_channels.py` & `python_semantic_release-9.7.2/tests/fixtures/repos/github_flow/repo_w_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py` & `python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py` & `python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py` & `python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/fixtures/scipy.py` & `python_semantic_release-9.7.2/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/scenario/test_next_version.py` & `python_semantic_release-9.7.2/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/scenario/test_release_history.py` & `python_semantic_release-9.7.2/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/scenario/test_template_render.py` & `python_semantic_release-9.7.2/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_release_notes.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_template.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_config.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_masking_filter.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_util.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_version.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_angular.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_parsed_commit.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_parsed_commit.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_scipy.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_tag.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_util.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test__base.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_bitbucket.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_gitea.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_github.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/test_helpers.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_algorithm.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_declaration.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_translator.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_version.py` & `python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.1/tests/util.py` & `python_semantic_release-9.7.2/tests/util.py`

 * *Files identical despite different names*

