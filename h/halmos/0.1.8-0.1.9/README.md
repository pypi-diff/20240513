# Comparing `tmp/halmos-0.1.8.tar.gz` & `tmp/halmos-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halmos-0.1.8.tar", last modified: Thu Oct 12 00:07:35 2023, max compression
+gzip compressed data, was "halmos-0.1.9.tar", last modified: Wed Oct 25 17:33:38 2023, max compression
```

## Comparing `halmos-0.1.8.tar` & `halmos-0.1.9.tar`

### file list

```diff
@@ -1,172 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.272094 halmos-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-10-12 00:07:20.000000 halmos-0.1.8/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.236094 halmos-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.244094 halmos-0.1.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-10-12 00:07:20.000000 halmos-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-10-12 00:07:20.000000 halmos-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.244094 halmos-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-12 00:07:20.000000 halmos-0.1.8/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-10-12 00:07:20.000000 halmos-0.1.8/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-10-12 00:07:20.000000 halmos-0.1.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-10-12 00:07:20.000000 halmos-0.1.8/.github/workflows/test-external.yml
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-10-12 00:07:20.000000 halmos-0.1.8/.github/workflows/test-ffi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-10-12 00:07:20.000000 halmos-0.1.8/.github/workflows/test-long.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-10-12 00:07:20.000000 halmos-0.1.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-10-12 00:07:20.000000 halmos-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-10-12 00:07:20.000000 halmos-0.1.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-12 00:07:20.000000 halmos-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-10-12 00:07:20.000000 halmos-0.1.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-10-12 00:07:20.000000 halmos-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2023-10-12 00:07:35.272094 halmos-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-10-12 00:07:20.000000 halmos-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.244094 halmos-0.1.8/benchmarks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      600 2023-10-12 00:07:20.000000 halmos-0.1.8/benchmarks/baolean.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.244094 halmos-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    12454 2023-10-12 00:07:20.000000 halmos-0.1.8/docs/getting-started.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.244094 halmos-0.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.244094 halmos-0.1.8/examples/simple/
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/simple/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/simple/foundry.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.244094 halmos-0.1.8/examples/simple/src/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/simple/src/IsPowerOfTwo.sol
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/simple/src/TotalPrice.sol
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/simple/src/Vault.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.248094 halmos-0.1.8/examples/simple/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/simple/test/Fork.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/simple/test/IsPowerOfTwo.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/simple/test/TotalPrice.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/simple/test/Vault.t.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.236094 halmos-0.1.8/examples/tokens/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.248094 halmos-0.1.8/examples/tokens/ERC20/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/foundry.toml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/remappings.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.248094 halmos-0.1.8/examples/tokens/ERC20/src/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/src/OpenZeppelinERC20.sol
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/src/SoladyERC20.sol
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/src/SolmateERC20.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.248094 halmos-0.1.8/examples/tokens/ERC20/test/
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/test/CurveTokenV3.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)    13832 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/test/DEIStablecoin.sol
--rw-r--r--   0 runner    (1001) docker     (127)    27846 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/test/DEIStablecoin.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/test/ERC20Test.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/test/SoladyERC20.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC20/test/SolmateERC20.t.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.248094 halmos-0.1.8/examples/tokens/ERC721/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC721/foundry.toml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC721/remappings.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.248094 halmos-0.1.8/examples/tokens/ERC721/src/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC721/src/OpenZeppelinERC721.sol
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC721/src/SoladyERC721.sol
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC721/src/SolmateERC721.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.252094 halmos-0.1.8/examples/tokens/ERC721/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC721/test/ERC721Test.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC721/test/SoladyERC721.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2023-10-12 00:07:20.000000 halmos-0.1.8/examples/tokens/ERC721/test/SolmateERC721.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-10-12 00:07:20.000000 halmos-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-12 00:07:20.000000 halmos-0.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-12 00:07:20.000000 halmos-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 00:07:35.272094 halmos-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.240094 halmos-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.252094 halmos-0.1.8/src/halmos/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42782 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/calldata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/cheatcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/pools.py
--rw-r--r--   0 runner    (1001) docker     (127)   102516 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/sevm.py
--rw-r--r--   0 runner    (1001) docker     (127)    31056 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-12 00:07:20.000000 halmos-0.1.8/src/halmos/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.256094 halmos-0.1.8/src/halmos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2023-10-12 00:07:35.000000 halmos-0.1.8/src/halmos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2023-10-12 00:07:35.000000 halmos-0.1.8/src/halmos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 00:07:35.000000 halmos-0.1.8/src/halmos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-12 00:07:35.000000 halmos-0.1.8/src/halmos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-12 00:07:35.000000 halmos-0.1.8/src/halmos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-12 00:07:35.000000 halmos-0.1.8/src/halmos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.256094 halmos-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.256094 halmos-0.1.8/tests/expected/
--rw-r--r--   0 runner    (1001) docker     (127)    56339 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/expected/all.json
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/expected/erc20.json
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/expected/erc721.json
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/expected/ffi.json
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/expected/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/expected/solver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.256094 halmos-0.1.8/tests/ffi/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/ffi/foundry.toml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/ffi/remappings.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.256094 halmos-0.1.8/tests/ffi/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/ffi/test/Ffi.t.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.260094 halmos-0.1.8/tests/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/foundry.toml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/remappings.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.260094 halmos-0.1.8/tests/regression/src/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/src/Const.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/src/Counter.sol
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/src/Create.sol
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/src/List.sol
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/src/SignExtend.sol
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/src/Storage.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.268094 halmos-0.1.8/tests/regression/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Arith.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/AssertTest.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Block.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Buffers.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Byte.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Call.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/CallAlias.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Console.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Const.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Constructor.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Context.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Counter.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Create.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Create2.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Deal.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Foundry.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Getter.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/HalmosCheatCode.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      790 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Invalid.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Library.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/LibraryLinking.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/List.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Natspec.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Opcode.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Prank.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Proxy.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Reset.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Revert.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Send.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Setup.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/SetupPlus.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/SetupSymbolic.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/SignExtend.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Signature.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/SmolWETH.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/StaticContexts.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Storage.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Storage2.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Store.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Struct.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/TestConstructor.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Token.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/UnknownCall.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/UnsupportedOpcode.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/regression/test/Warp.t.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.272094 halmos-0.1.8/tests/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/solver/foundry.toml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/solver/remappings.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 00:07:35.272094 halmos-0.1.8/tests/solver/test/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/solver/test/Math.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/solver/test/SignedDiv.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/solver/test/Solver.t.sol
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/test_halmos.py
--rw-r--r--   0 runner    (1001) docker     (127)    14064 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/test_sevm.py
--rw-r--r--   0 runner    (1001) docker     (127)    26029 2023-10-12 00:07:20.000000 halmos-0.1.8/tests/test_traces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.235533 halmos-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-10-25 17:33:29.000000 halmos-0.1.9/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.203532 halmos-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.211532 halmos-0.1.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2023-10-25 17:33:29.000000 halmos-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-10-25 17:33:29.000000 halmos-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.215532 halmos-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-25 17:33:29.000000 halmos-0.1.9/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-10-25 17:33:29.000000 halmos-0.1.9/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-10-25 17:33:29.000000 halmos-0.1.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-10-25 17:33:29.000000 halmos-0.1.9/.github/workflows/test-external.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2023-10-25 17:33:29.000000 halmos-0.1.9/.github/workflows/test-ffi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-10-25 17:33:29.000000 halmos-0.1.9/.github/workflows/test-long.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-10-25 17:33:29.000000 halmos-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2023-10-25 17:33:29.000000 halmos-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2023-10-25 17:33:29.000000 halmos-0.1.9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-25 17:33:29.000000 halmos-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-10-25 17:33:29.000000 halmos-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-10-25 17:33:29.000000 halmos-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-10-25 17:33:38.235533 halmos-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-10-25 17:33:29.000000 halmos-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.215532 halmos-0.1.9/benchmarks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      600 2023-10-25 17:33:29.000000 halmos-0.1.9/benchmarks/baolean.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.215532 halmos-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    12454 2023-10-25 17:33:29.000000 halmos-0.1.9/docs/getting-started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.215532 halmos-0.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.215532 halmos-0.1.9/examples/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/simple/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/simple/foundry.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.219532 halmos-0.1.9/examples/simple/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/simple/src/IsPowerOfTwo.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/simple/src/TotalPrice.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/simple/src/Vault.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.219532 halmos-0.1.9/examples/simple/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/simple/test/Fork.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/simple/test/IsPowerOfTwo.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/simple/test/TotalPrice.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/simple/test/Vault.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.203532 halmos-0.1.9/examples/tokens/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.219532 halmos-0.1.9/examples/tokens/ERC20/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.223532 halmos-0.1.9/examples/tokens/ERC20/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/src/OpenZeppelinERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/src/SoladyERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/src/SolmateERC20.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.223532 halmos-0.1.9/examples/tokens/ERC20/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/test/CurveTokenV3.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)    13832 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/test/DEIStablecoin.sol
+-rw-r--r--   0 runner    (1001) docker     (127)    27846 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/test/DEIStablecoin.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/test/ERC20Test.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/test/SoladyERC20.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC20/test/SolmateERC20.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.227532 halmos-0.1.9/examples/tokens/ERC721/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC721/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC721/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.227532 halmos-0.1.9/examples/tokens/ERC721/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC721/src/OpenZeppelinERC721.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC721/src/SoladyERC721.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC721/src/SolmateERC721.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.227532 halmos-0.1.9/examples/tokens/ERC721/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC721/test/ERC721Test.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC721/test/SoladyERC721.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2023-10-25 17:33:29.000000 halmos-0.1.9/examples/tokens/ERC721/test/SolmateERC721.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2023-10-25 17:33:29.000000 halmos-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-25 17:33:29.000000 halmos-0.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-25 17:33:29.000000 halmos-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 17:33:38.235533 halmos-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.207532 halmos-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.227532 halmos-0.1.9/src/halmos/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43301 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/calldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15379 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/cheatcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83943 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/sevm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37872 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-25 17:33:29.000000 halmos-0.1.9/src/halmos/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.227532 halmos-0.1.9/src/halmos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-10-25 17:33:38.000000 halmos-0.1.9/src/halmos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2023-10-25 17:33:38.000000 halmos-0.1.9/src/halmos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 17:33:38.000000 halmos-0.1.9/src/halmos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-25 17:33:38.000000 halmos-0.1.9/src/halmos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-25 17:33:38.000000 halmos-0.1.9/src/halmos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-25 17:33:38.000000 halmos-0.1.9/src/halmos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.231532 halmos-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.231532 halmos-0.1.9/tests/expected/
+-rw-r--r--   0 runner    (1001) docker     (127)    59698 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/expected/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/expected/erc20.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/expected/erc721.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/expected/ffi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/expected/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/expected/solver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.231532 halmos-0.1.9/tests/ffi/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/ffi/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/ffi/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.231532 halmos-0.1.9/tests/ffi/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/ffi/test/Ffi.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.231532 halmos-0.1.9/tests/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.231532 halmos-0.1.9/tests/regression/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/src/Const.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/src/Counter.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/src/Create.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/src/List.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/src/SignExtend.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/src/Storage.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.235533 halmos-0.1.9/tests/regression/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Arith.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/AssertTest.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Block.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Buffers.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Byte.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Call.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/CallAlias.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Console.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Const.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Constructor.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Context.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Counter.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Create.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Create2.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Deal.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Foundry.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Getter.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/HalmosCheatCode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Invalid.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Library.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/LibraryLinking.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/List.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Natspec.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Opcode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Prank.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Proxy.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Reset.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Revert.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Send.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Setup.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/SetupPlus.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/SetupSymbolic.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/SignExtend.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Signature.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/SmolWETH.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/StaticContexts.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Storage.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Storage2.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Store.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Struct.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/TestConstructor.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Token.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/UnknownCall.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/UnsupportedOpcode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/regression/test/Warp.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.235533 halmos-0.1.9/tests/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/solver/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/solver/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 17:33:38.235533 halmos-0.1.9/tests/solver/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/solver/test/Math.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/solver/test/SignedDiv.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/solver/test/Solver.t.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/test_halmos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14064 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/test_sevm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26029 2023-10-25 17:33:29.000000 halmos-0.1.9/tests/test_traces.py
```

### Comparing `halmos-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md` & `halmos-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/.github/workflows/codeql.yml` & `halmos-0.1.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/.github/workflows/test-external.yml` & `halmos-0.1.9/.github/workflows/test-external.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/.github/workflows/test-ffi.yml` & `halmos-0.1.9/.github/workflows/test-ffi.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/.github/workflows/test-long.yml` & `halmos-0.1.9/.github/workflows/test-long.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/.github/workflows/test.yml` & `halmos-0.1.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/.gitmodules` & `halmos-0.1.9/.gitmodules`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/CONTRIBUTING.md` & `halmos-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/LICENSE` & `halmos-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/PKG-INFO` & `halmos-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.1.8
-Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
+Version: 0.1.9
+Summary: A symbolic testing tool for EVM smart contracts
 Author: a16z crypto
 Maintainer: Daejun Park, karmacoma <karma@coma.lol>
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `halmos-0.1.8/README.md` & `halmos-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/benchmarks/baolean.sh` & `halmos-0.1.9/benchmarks/baolean.sh`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/docs/getting-started.md` & `halmos-0.1.9/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/README.md` & `halmos-0.1.9/examples/README.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/simple/README.md` & `halmos-0.1.9/examples/simple/README.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/simple/src/TotalPrice.sol` & `halmos-0.1.9/examples/simple/src/TotalPrice.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/simple/src/Vault.sol` & `halmos-0.1.9/examples/simple/src/Vault.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/simple/test/Fork.t.sol` & `halmos-0.1.9/examples/simple/test/Fork.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/simple/test/IsPowerOfTwo.t.sol` & `halmos-0.1.9/examples/simple/test/IsPowerOfTwo.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/simple/test/TotalPrice.t.sol` & `halmos-0.1.9/examples/simple/test/TotalPrice.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/simple/test/Vault.t.sol` & `halmos-0.1.9/examples/simple/test/Vault.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC20/src/SoladyERC20.sol` & `halmos-0.1.9/examples/tokens/ERC20/src/SoladyERC20.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC20/test/CurveTokenV3.t.sol` & `halmos-0.1.9/examples/tokens/ERC20/test/CurveTokenV3.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC20/test/DEIStablecoin.sol` & `halmos-0.1.9/examples/tokens/ERC20/test/DEIStablecoin.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC20/test/DEIStablecoin.t.sol` & `halmos-0.1.9/examples/tokens/ERC20/test/DEIStablecoin.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC20/test/ERC20Test.sol` & `halmos-0.1.9/examples/tokens/ERC20/test/ERC20Test.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol` & `halmos-0.1.9/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC20/test/SoladyERC20.t.sol` & `halmos-0.1.9/examples/tokens/ERC20/test/SoladyERC20.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC20/test/SolmateERC20.t.sol` & `halmos-0.1.9/examples/tokens/ERC20/test/SolmateERC20.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC721/src/SoladyERC721.sol` & `halmos-0.1.9/examples/tokens/ERC721/src/SoladyERC721.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC721/test/ERC721Test.sol` & `halmos-0.1.9/examples/tokens/ERC721/test/ERC721Test.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol` & `halmos-0.1.9/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC721/test/SoladyERC721.t.sol` & `halmos-0.1.9/examples/tokens/ERC721/test/SoladyERC721.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/examples/tokens/ERC721/test/SolmateERC721.t.sol` & `halmos-0.1.9/examples/tokens/ERC721/test/SolmateERC721.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/pyproject.toml` & `halmos-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2", "black"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
 [project]
 name = "halmos"
-description = "Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode"
+description = "A symbolic testing tool for EVM smart contracts"
 readme = "README.md"
 authors = [
     { name="a16z crypto" },
 ]
 maintainers = [
     { name="Daejun Park" },
     { name="karmacoma <karma@coma.lol>" },
@@ -33,8 +33,8 @@
 "Homepage" = "https://github.com/a16z/halmos"
 
 [tool.black]
 target-versions = ["py38", "py39", "py310", "py311"]
 
 [tool.pytest.ini_options]
 # TODO: re-add test_traces.py when we have a better way to support it in CI
-addopts = "--ignore=tests/lib/solady/ext/woke --ignore=tests/test_traces.py"
+addopts = "--ignore=tests/lib --ignore=tests/test_traces.py"
```

### Comparing `halmos-0.1.8/src/halmos/__main__.py` & `halmos-0.1.9/src/halmos/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 
 import os
 import sys
 import subprocess
 import uuid
 import json
 import re
+import signal
 import traceback
 
 from argparse import Namespace
 from dataclasses import dataclass, asdict
 from importlib import metadata
 
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 from .sevm import *
 from .utils import (
     create_solver,
     hexify,
+    stringify,
     indent_text,
     NamedTimer,
     yellow,
     cyan,
     green,
     red,
     error,
@@ -1062,22 +1064,22 @@
 
 def to_str_model(model: Model, print_full_model: bool) -> StrModel:
     def select(var):
         name = str(var)
         return name.startswith("p_") or name.startswith("halmos_")
 
     select_model = filter(select, model) if not print_full_model else model
-    return {str(decl): hexify(model[decl]) for decl in select_model}
+    return {str(decl): stringify(str(decl), model[decl]) for decl in select_model}
 
 
 def render_model(model: UnionType[str, StrModel]) -> str:
     if isinstance(model, str):
         return model
 
-    formatted = [f"\n    {decl} = {hexify(val)}" for decl, val in model.items()]
+    formatted = [f"\n    {decl} = {val}" for decl, val in model.items()]
     return "".join(sorted(formatted)) if formatted else "∅"
 
 
 def mk_options(args: Namespace) -> Dict:
     options = {
         "target": args.root,
         "verbose": args.verbose,
@@ -1320,23 +1322,46 @@
         print(color_warn(f"Build output parsing failed: {type(err).__name__}: {err}"))
         if args.debug:
             traceback.print_exc()
         return MainResult(1)
 
     timer.create_subtimer("tests")
 
-    #
-    # run
-    #
-
     total_passed = 0
     total_failed = 0
     total_found = 0
     test_results_map = {}
 
+    #
+    # exit and signal handlers to avoid dropping json output
+    #
+
+    def on_exit(exitcode: int) -> MainResult:
+        result = MainResult(exitcode, test_results_map)
+
+        if args.json_output:
+            with open(args.json_output, "w") as json_file:
+                json.dump(asdict(result), json_file, indent=4)
+
+        return result
+
+    def on_signal(signum, frame):
+        if args.debug:
+            debug(f"Signal {signum} received. Dumping {test_results_map}...")
+        exitcode = 128 + signum
+        on_exit(exitcode)
+        sys.exit(exitcode)
+
+    for signum in [signal.SIGINT, signal.SIGTERM]:
+        signal.signal(signum, on_signal)
+
+    #
+    # run
+    #
+
     for build_out_map, filename, contract_name in build_output_iterator(build_out):
         if args.contract and args.contract != contract_name:
             continue
 
         (contract_json, contract_type, natspec) = build_out_map[filename][contract_name]
         if contract_type != "contract":
             continue
@@ -1399,21 +1424,15 @@
         error_msg = f"Error: No tests with the prefix `{args.function}`"
         if args.contract is not None:
             error_msg += f" in {args.contract}"
         print(color_warn(error_msg))
         return MainResult(1)
 
     exitcode = 0 if total_failed == 0 else 1
-    result = MainResult(exitcode, test_results_map)
-
-    if args.json_output:
-        with open(args.json_output, "w") as json_file:
-            json.dump(asdict(result), json_file, indent=4)
-
-    return result
+    return on_exit(exitcode)
 
 
 # entrypoint for the `halmos` script
 def main() -> int:
     return _main().exitcode
```

### Comparing `halmos-0.1.8/src/halmos/calldata.py` & `halmos-0.1.9/src/halmos/calldata.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/src/halmos/exceptions.py` & `halmos-0.1.9/src/halmos/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 Exceptions thrown during EVM execution.
 
 Note: this is a modified version execution-specs' src/ethereum/<fork>/vm/exceptions.pyd
 """
 
 
+class HalmosException(Exception):
+    pass
+
+
+class NotConcreteError(HalmosException):
+    pass
+
+
 class EvmException(Exception):
     """
     Base class for all EVM exceptions.
     """
 
     pass
```

### Comparing `halmos-0.1.8/src/halmos/parser.py` & `halmos-0.1.9/src/halmos/parser.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/src/halmos/sevm.py` & `halmos-0.1.9/src/halmos/sevm.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,101 +4,45 @@
 import math
 import re
 
 from copy import deepcopy
 from collections import defaultdict
 from dataclasses import dataclass, field
 from functools import reduce
-from subprocess import Popen, PIPE
 from typing import (
     Any,
     Dict,
     Iterator,
     List,
     Optional,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union as UnionType,
 )
 from z3 import *
 
-from .cheatcodes import halmos_cheat_code, hevm_cheat_code, console, Prank
+from .cheatcodes import halmos_cheat_code, hevm_cheat_code, Prank
+from .console import console
 from .exceptions import *
-from .utils import (
-    create_solver,
-    EVM,
-    sha3_inv,
-    restore_precomputed_hashes,
-    str_opcode,
-    assert_address,
-    assert_uint256,
-    con_addr,
-    bv_value_to_bytes,
-    hexify,
-    color_info,
-)
+from .utils import *
 from .warnings import (
     warn,
-    UNSUPPORTED_OPCODE,
     LIBRARY_PLACEHOLDER,
-    UNINTERPRETED_UNKNOWN_CALLS,
     INTERNAL_ERROR,
 )
 
-Word = Any  # z3 expression (including constants)
-Byte = Any  # z3 expression (including constants)
-Bytes = Any  # z3 expression (including constants)
-Address = BitVecRef  # 160-bitvector
 
 Steps = Dict[int, Dict[str, Any]]  # execution tree
 
 EMPTY_BYTES = b""
 MAX_CALL_DEPTH = 1024
 
 
-# dynamic BitVecSort sizes
-class BitVecSortCache:
-    def __init__(self):
-        self.cache = {}
-        for size in (
-            1,
-            8,
-            16,
-            32,
-            64,
-            128,
-            160,
-            256,
-            264,
-            288,
-            512,
-            544,
-            800,
-            1024,
-            1056,
-        ):
-            self.cache[size] = BitVecSort(size)
-
-    def __getitem__(self, size: int) -> BitVecSort:
-        hit = self.cache.get(size)
-        return hit if hit is not None else BitVecSort(size)
-
-
-BitVecSorts = BitVecSortCache()
-
-# known, fixed BitVecSort sizes
-BitVecSort1 = BitVecSorts[1]
-BitVecSort8 = BitVecSorts[8]
-BitVecSort160 = BitVecSorts[160]
-BitVecSort256 = BitVecSorts[256]
-BitVecSort264 = BitVecSorts[264]
-BitVecSort512 = BitVecSorts[512]
-
 # symbolic states
 # calldataload(index)
 f_calldataload = Function("calldataload", BitVecSort256, BitVecSort256)
 # calldatasize()
 f_calldatasize = Function("calldatasize", BitVecSort256)
 # extcodesize(target address)
 f_extcodesize = Function("extcodesize", BitVecSort160, BitVecSort256)
@@ -161,61 +105,29 @@
     def __repr__(self) -> str:
         return f"Instruction({mnemonic(self.opcode)}, pc={self.pc}, operand={repr(self.operand)})"
 
     def __len__(self) -> int:
         return instruction_length(self.opcode)
 
 
-class HalmosException(Exception):
-    pass
-
-
-class NotConcreteError(HalmosException):
-    pass
-
-
 def id_str(x: Any) -> str:
     return hexify(x).replace(" ", "")
 
 
-def name_of(x: str) -> str:
-    return re.sub(r"\s+", "_", x)
-
-
 def padded_slice(lst: List, start: int, size: int, default=0) -> List:
     """
     Return a slice of lst, starting at start and with size elements. If the slice
     is out of bounds, pad with default.
     """
 
     end = start + size
     n = len(lst)
     return [lst[i] if i < n else default for i in range(start, end)]
 
 
-def unbox_int(x: Any) -> Any:
-    """Convert int-like objects to int"""
-    if isinstance(x, bytes):
-        return int.from_bytes(x, "big")
-
-    if is_bv_value(x):
-        return x.as_long()
-
-    return x
-
-
-def int_of(x: Any, err: str = "expected concrete value but got") -> int:
-    res = unbox_int(x)
-
-    if isinstance(res, int):
-        return res
-
-    raise NotConcreteError(f"{err}: {x}")
-
-
 def iter_bytes(x: Any, _byte_length: int = -1):
     """Return an iterable over the bytes of x (concrete or symbolic)"""
 
     if isinstance(x, bytes):
         return x
 
     if isinstance(x, int):
@@ -247,58 +159,14 @@
     if is_concrete(opcode):
         opcode = int_of(opcode)
         return str_opcode.get(opcode, hex(opcode))
     else:
         return str(opcode)
 
 
-def concat(args):
-    if len(args) > 1:
-        return Concat(args)
-    else:
-        return args[0]
-
-
-def uint256(x: BitVecRef) -> BitVecRef:
-    bitsize = x.size()
-    if bitsize > 256:
-        raise ValueError(x)
-    if bitsize == 256:
-        return x
-    return simplify(ZeroExt(256 - bitsize, x))
-
-
-def uint160(x: BitVecRef) -> BitVecRef:
-    bitsize = x.size()
-    if bitsize > 256:
-        raise ValueError(x)
-    if bitsize == 160:
-        return x
-    if bitsize > 160:
-        return simplify(Extract(159, 0, x))
-    else:
-        return simplify(ZeroExt(160 - bitsize, x))
-
-
-def con(n: int, size_bits=256) -> Word:
-    return BitVecVal(n, BitVecSorts[size_bits])
-
-
-def byte_length(x: Any) -> int:
-    if is_bv(x):
-        if x.size() % 8 != 0:
-            raise ValueError(x)
-        return x.size() >> 3
-
-    if isinstance(x, bytes):
-        return len(x)
-
-    raise ValueError(x)
-
-
 def instruction_length(opcode: Any) -> int:
     opcode = int_of(opcode)
     return (opcode - EVM.PUSH0 + 1) if EVM.PUSH1 <= opcode <= EVM.PUSH32 else 1
 
 
 def wextend(mem: List[UnionType[int, BitVecRef]], loc: int, size: int) -> None:
     mem.extend([0] * (loc + size - len(mem)))
@@ -385,107 +253,14 @@
     wextend(mem, loc, size)
     for i in range(size):
         if not eq(arr[i].sort(), BitVecSort8):
             raise ValueError(arr)
         mem[loc + i] = arr[i]
 
 
-def extract_bytes(data: BitVecRef, byte_offset: int, size_bytes: int) -> BitVecRef:
-    """Extract bytes from calldata. Zero-pad if out of bounds."""
-    n = data.size()
-    if n % 8 != 0:
-        raise ValueError(n)
-
-    # will extract hi - lo + 1 bits
-    hi = n - 1 - byte_offset * 8
-    lo = n - byte_offset * 8 - size_bytes * 8
-    lo = 0 if lo < 0 else lo
-
-    val = simplify(Extract(hi, lo, data))
-
-    zero_padding = size_bytes * 8 - val.size()
-    if zero_padding < 0:
-        raise ValueError(val)
-    if zero_padding > 0:
-        val = simplify(Concat(val, con(0, zero_padding)))
-
-    return val
-
-
-def extract_funsig(calldata: BitVecRef):
-    """Extracts the function signature (first 4 bytes) from calldata"""
-    return extract_bytes(calldata, 0, 4)
-
-
-def extract_string_argument(calldata: BitVecRef, arg_idx: int):
-    """Extracts idx-th argument of string from calldata"""
-    string_offset = int_of(
-        extract_bytes(calldata, 4 + arg_idx * 32, 32),
-        "symbolic offset for string argument",
-    )
-    string_length = int_of(
-        extract_bytes(calldata, 4 + string_offset, 32),
-        "symbolic size for string argument",
-    )
-    if string_length == 0:
-        return ""
-    string_value = int_of(
-        extract_bytes(calldata, 4 + string_offset + 32, string_length),
-        "symbolic string argument",
-    )
-    string_bytes = string_value.to_bytes(string_length, "big")
-    return string_bytes.decode("utf-8")
-
-
-def extract_string_array_argument(calldata: BitVecRef, arg_idx: int):
-    """Extracts idx-th argument of string array from calldata"""
-
-    array_slot = int_of(extract_bytes(calldata, 4 + 32 * arg_idx, 32))
-    num_strings = int_of(extract_bytes(calldata, 4 + array_slot, 32))
-
-    string_array = []
-
-    for i in range(num_strings):
-        string_offset = int_of(
-            extract_bytes(calldata, 4 + array_slot + 32 * (i + 1), 32)
-        )
-        string_length = int_of(
-            extract_bytes(calldata, 4 + array_slot + 32 + string_offset, 32)
-        )
-        string_value = int_of(
-            extract_bytes(
-                calldata, 4 + array_slot + 32 + string_offset + 32, string_length
-            )
-        )
-        string_bytes = string_value.to_bytes(string_length, "big")
-        string_array.append(string_bytes.decode("utf-8"))
-
-    return string_array
-
-
-def stringified_bytes_to_bytes(string_bytes: str):
-    """Converts a string of bytes to a bytes memory type"""
-
-    string_bytes_len = (len(string_bytes) + 1) // 2
-    string_bytes_len_enc = hex(string_bytes_len).replace("0x", "").rjust(64, "0")
-
-    string_bytes_len_ceil = (string_bytes_len + 31) // 32 * 32
-
-    ret_bytes = (
-        "00" * 31
-        + "20"
-        + string_bytes_len_enc
-        + string_bytes.ljust(string_bytes_len_ceil * 2, "0")
-    )
-    ret_len = len(ret_bytes) // 2
-    ret_bytes = bytes.fromhex(ret_bytes)
-
-    return BitVecVal(int.from_bytes(ret_bytes, "big"), ret_len * 8)
-
-
 @dataclass(frozen=True)
 class EventLog:
     """
     Data record produced during the execution of a transaction.
     """
 
     address: Address
@@ -910,14 +685,23 @@
 
     def current_opcode(self) -> UnionType[int, BitVecRef]:
         return unbox_int(self.pgm[self.pc])
 
     def current_instruction(self) -> Instruction:
         return self.pgm.decode_instruction(self.pc)
 
+    def set_code(
+        self, who: Address, code: UnionType[bytes, BitVecRef, Contract]
+    ) -> None:
+        """
+        Sets the code at a given address.
+        """
+        assert_address(who)
+        self.code[who] = code if isinstance(code, Contract) else Contract(code)
+
     def str_cnts(self) -> str:
         return "".join(
             [
                 f"{x[0]}: {x[1]}\n"
                 for x in sorted(self.cnts["opcode"].items(), key=lambda x: x[0])
             ]
         )
@@ -1352,39 +1136,14 @@
             res += x
         return simplify(res)
 
 
 SomeStorage = TypeVar("SomeStorage", bound=Storage)
 
 
-#             x  == b   if sort(x) = bool
-# int_to_bool(x) == b   if sort(x) = int
-def test(x: Word, b: bool) -> Word:
-    if is_bool(x):
-        if b:
-            return x
-        else:
-            return Not(x)
-    elif is_bv(x):
-        if b:
-            return x != con(0)
-        else:
-            return x == con(0)
-    else:
-        raise ValueError(x)
-
-
-def is_non_zero(x: Word) -> Word:
-    return test(x, True)
-
-
-def is_zero(x: Word) -> Word:
-    return test(x, False)
-
-
 def bitwise(op, x: Word, y: Word) -> Word:
     if is_bool(x) and is_bool(y):
         if op == EVM.AND:
             return And(x, y)
         elif op == EVM.OR:
             return Or(x, y)
         elif op == EVM.XOR:
@@ -1879,290 +1638,28 @@
                 ex.solver.add(exit_code_var != con(0))
 
             # identity
             if eq(to, con_addr(4)):
                 ex.solver.add(exit_code_var != con(0))
                 ret = arg
 
-            # TODO: factor out cheatcode semantics
             # halmos cheat code
             if eq(to, halmos_cheat_code.address):
                 ex.solver.add(exit_code_var != con(0))
-
-                funsig: int = int_of(
-                    extract_funsig(arg), "symbolic halmos cheatcode function selector"
-                )
-
-                if self.options.get("debug"):
-                    print(f"Executing halmos cheat code: {hex(funsig)}")
-
-                # createUint(uint256,string) returns (uint256)
-                if funsig == halmos_cheat_code.create_uint:
-                    bit_size = int_of(
-                        extract_bytes(arg, 4, 32),
-                        "symbolic bit size for halmos.createUint()",
-                    )
-                    name = name_of(extract_string_argument(arg, 1))
-                    if bit_size <= 256:
-                        label = f"halmos_{name}_uint{bit_size}_{ex.new_symbol_id():>02}"
-                        ret = uint256(BitVec(label, BitVecSorts[bit_size]))
-                    else:
-                        raise HalmosException(f"bitsize larger than 256: {bit_size}")
-
-                # createBytes(uint256,string) returns (bytes)
-                elif funsig == halmos_cheat_code.create_bytes:
-                    byte_size = int_of(
-                        extract_bytes(arg, 4, 32),
-                        "symbolic byte size for halmos.createBytes()",
-                    )
-                    name = name_of(extract_string_argument(arg, 1))
-                    label = f"halmos_{name}_bytes_{ex.new_symbol_id():>02}"
-                    symbolic_bytes = BitVec(label, BitVecSorts[byte_size * 8])
-                    ret = Concat(con(32), con(byte_size), symbolic_bytes)
-
-                # createUint256(string) returns (uint256)
-                elif funsig == halmos_cheat_code.create_uint256:
-                    name = name_of(extract_string_argument(arg, 0))
-                    label = f"halmos_{name}_uint256_{ex.new_symbol_id():>02}"
-                    ret = BitVec(label, BitVecSort256)
-
-                # createBytes32(string) returns (bytes32)
-                elif funsig == halmos_cheat_code.create_bytes32:
-                    name = name_of(extract_string_argument(arg, 0))
-                    label = f"halmos_{name}_bytes32_{ex.new_symbol_id():>02}"
-                    ret = BitVec(label, BitVecSort256)
-
-                # createAddress(string) returns (address)
-                elif funsig == halmos_cheat_code.create_address:
-                    name = name_of(extract_string_argument(arg, 0))
-                    label = f"halmos_{name}_address_{ex.new_symbol_id():>02}"
-                    ret = uint256(BitVec(label, BitVecSort160))
-
-                # createBool(string) returns (bool)
-                elif funsig == halmos_cheat_code.create_bool:
-                    name = name_of(extract_string_argument(arg, 0))
-                    label = f"halmos_{name}_bool_{ex.new_symbol_id():>02}"
-                    ret = uint256(BitVec(label, BitVecSort1))
-
-                else:
-                    error_msg = f"Unknown halmos cheat code: function selector = 0x{funsig:0>8x}, calldata = {hexify(arg)}"
-                    raise HalmosException(error_msg)
+                ret = halmos_cheat_code.handle(ex, arg)
 
             # vm cheat code
             if eq(to, hevm_cheat_code.address):
                 ex.solver.add(exit_code_var != con(0))
-                # vm.fail()
-                # BitVecVal(hevm_cheat_code.fail_payload, 800)
-                if arg == hevm_cheat_code.fail_payload:
-                    raise FailCheatcode()
-
-                # vm.assume(bool)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32) * 8])
-                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.assume_sig
-                ):
-                    assume_cond = simplify(is_non_zero(Extract(255, 0, arg)))
-                    ex.solver.add(assume_cond)
-                    ex.path.append(str(assume_cond))
-
-                # vm.getCode(string)
-                elif (
-                    simplify(Extract(arg_size * 8 - 1, arg_size * 8 - 32, arg))
-                    == hevm_cheat_code.get_code_sig
-                ):
-                    calldata = bytes.fromhex(hex(arg.as_long())[2:])
-                    path_len = int.from_bytes(calldata[36:68], "big")
-                    path = calldata[68 : 68 + path_len].decode("utf-8")
-
-                    if ":" in path:
-                        [filename, contract_name] = path.split(":")
-                        path = "out/" + filename + "/" + contract_name + ".json"
-
-                    target = self.options["target"].rstrip("/")
-                    path = target + "/" + path
-
-                    with open(path) as f:
-                        artifact = json.loads(f.read())
-
-                    if artifact["bytecode"]["object"]:
-                        bytecode = artifact["bytecode"]["object"].replace("0x", "")
-                    else:
-                        bytecode = artifact["bytecode"].replace("0x", "")
-
-                    ret = stringified_bytes_to_bytes(bytecode)
-                # vm.prank(address)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32) * 8])
-                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.prank_sig
-                ):
-                    result = ex.prank.prank(uint160(Extract(255, 0, arg)))
-                    if not result:
-                        raise HalmosException("You have an active prank already.")
-
-                # vm.startPrank(address)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32) * 8])
-                    and simplify(Extract(287, 256, arg))
-                    == hevm_cheat_code.start_prank_sig
-                ):
-                    result = ex.prank.startPrank(uint160(Extract(255, 0, arg)))
-                    if not result:
-                        raise HalmosException("You have an active prank already.")
-
-                # vm.stopPrank()
-                elif (
-                    eq(arg.sort(), BitVecSorts[4 * 8])
-                    and simplify(Extract(31, 0, arg)) == hevm_cheat_code.stop_prank_sig
-                ):
-                    ex.prank.stopPrank()
-                # vm.deal(address,uint256)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32 * 2) * 8])
-                    and simplify(Extract(543, 512, arg)) == hevm_cheat_code.deal_sig
-                ):
-                    who = uint160(Extract(511, 256, arg))
-                    amount = simplify(Extract(255, 0, arg))
-                    ex.balance_update(who, amount)
-                # vm.store(address,bytes32,bytes32)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32 * 3) * 8])
-                    and simplify(Extract(799, 768, arg)) == hevm_cheat_code.store_sig
-                ):
-                    store_account = uint160(Extract(767, 512, arg))
-                    store_slot = simplify(Extract(511, 256, arg))
-                    store_value = simplify(Extract(255, 0, arg))
-                    store_account_addr = self.resolve_address_alias(ex, store_account)
-                    if store_account_addr is not None:
-                        self.sstore(ex, store_account_addr, store_slot, store_value)
-                    else:
-                        raise HalmosException(f"uninitialized account: {store_account}")
-
-                # vm.load(address,bytes32)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32 * 2) * 8])
-                    and simplify(Extract(543, 512, arg)) == hevm_cheat_code.load_sig
-                ):
-                    load_account = uint160(Extract(511, 256, arg))
-                    load_slot = simplify(Extract(255, 0, arg))
-                    load_account_addr = self.resolve_address_alias(ex, load_account)
-                    if load_account_addr is not None:
-                        ret = self.sload(ex, load_account_addr, load_slot)
-                    else:
-                        raise HalmosException(f"uninitialized account: {store_account}")
-
-                # vm.fee(uint256)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32) * 8])
-                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.fee_sig
-                ):
-                    ex.block.basefee = simplify(Extract(255, 0, arg))
-                # vm.chainId(uint256)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32) * 8])
-                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.chainid_sig
-                ):
-                    ex.block.chainid = simplify(Extract(255, 0, arg))
-                # vm.coinbase(address)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32) * 8])
-                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.coinbase_sig
-                ):
-                    ex.block.coinbase = uint160(Extract(255, 0, arg))
-                # vm.difficulty(uint256)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32) * 8])
-                    and simplify(Extract(287, 256, arg))
-                    == hevm_cheat_code.difficulty_sig
-                ):
-                    ex.block.difficulty = simplify(Extract(255, 0, arg))
-                # vm.roll(uint256)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32) * 8])
-                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.roll_sig
-                ):
-                    ex.block.number = simplify(Extract(255, 0, arg))
-                # vm.warp(uint256)
-                elif (
-                    eq(arg.sort(), BitVecSorts[(4 + 32) * 8])
-                    and simplify(Extract(287, 256, arg)) == hevm_cheat_code.warp_sig
-                ):
-                    ex.block.timestamp = simplify(Extract(255, 0, arg))
-                # vm.etch(address,bytes)
-                elif extract_funsig(arg) == hevm_cheat_code.etch_sig:
-                    who = extract_bytes(arg, 4 + 12, 20)
-
-                    # who must be concrete
-                    if not is_bv_value(who):
-                        error_msg = f"vm.etch(address who, bytes code) must have concrete argument `who` but received {who}"
-                        raise HalmosException(error_msg)
-
-                    # code must be concrete
-                    try:
-                        code_offset = int_of(extract_bytes(arg, 4 + 32, 32))
-                        code_length = int_of(extract_bytes(arg, 4 + code_offset, 32))
-                        code_int = int_of(
-                            extract_bytes(arg, 4 + code_offset + 32, code_length)
-                        )
-                        code_bytes = code_int.to_bytes(code_length, "big")
-
-                        ex.code[who] = Contract(code_bytes)
-                    except Exception as e:
-                        error_msg = f"vm.etch(address who, bytes code) must have concrete argument `code` but received calldata {arg}"
-                        raise HalmosException(error_msg) from e
-                # ffi(string[]) returns (bytes)
-                elif extract_funsig(arg) == hevm_cheat_code.ffi_sig:
-                    if not self.options.get("ffi"):
-                        error_msg = "ffi cheatcode is disabled. Run again with `--ffi` if you want to enable it"
-                        raise HalmosException(error_msg)
-                    cmd = extract_string_array_argument(arg, 0)
-                    process = Popen(cmd, stdout=PIPE, stderr=PIPE)
-
-                    (stdout, stderr) = process.communicate()
-
-                    if stderr:
-                        warn(
-                            INTERNAL_ERROR,
-                            f"An exception has occurred during the usage of the ffi cheatcode:\n{stderr.decode('utf-8')}",
-                        )
-
-                    out_bytes = stdout.decode("utf-8")
-
-                    if not out_bytes.startswith("0x"):
-                        out_bytes = out_bytes.strip().encode("utf-8").hex()
-                    else:
-                        out_bytes = out_bytes.strip().replace("0x", "")
-
-                    ret = stringified_bytes_to_bytes(out_bytes)
-
-                else:
-                    # TODO: support other cheat codes
-                    msg = f"Unsupported cheat code: calldata = {hexify(arg)}"
-                    raise HalmosException(msg)
+                ret = hevm_cheat_code.handle(self, ex, arg)
 
             # console
             if eq(to, console.address):
                 ex.solver.add(exit_code_var != con(0))
-
-                funsig: int = int_of(
-                    extract_funsig(arg), "symbolic console function selector"
-                )
-
-                if funsig == console.log_uint256:
-                    print(extract_bytes(arg, 4, 32))
-
-                # elif funsig == console.log_string:
-
-                else:
-                    # TODO: support other console functions
-                    print(
-                        color_info(
-                            f"Unsupported console function: selector = 0x{funsig:0>8x}, "
-                            f"calldata = {hexify(arg)}"
-                        )
-                    )
+                console.handle(ex, arg)
 
             # store return value
             if ret_size > 0:
                 wstore(ex.st.memory, ret_loc, ret_size, ret)
 
             ex.context.trace.append(
                 CallContext(
```

### Comparing `halmos-0.1.8/src/halmos/warnings.py` & `halmos-0.1.9/src/halmos/warnings.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/src/halmos.egg-info/PKG-INFO` & `halmos-0.1.9/src/halmos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.1.8
-Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
+Version: 0.1.9
+Summary: A symbolic testing tool for EVM smart contracts
 Author: a16z crypto
 Maintainer: Daejun Park, karmacoma <karma@coma.lol>
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `halmos-0.1.8/src/halmos.egg-info/SOURCES.txt` & `halmos-0.1.9/src/halmos.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol
 examples/tokens/ERC721/test/SoladyERC721.t.sol
 examples/tokens/ERC721/test/SolmateERC721.t.sol
 src/halmos/__init__.py
 src/halmos/__main__.py
 src/halmos/calldata.py
 src/halmos/cheatcodes.py
+src/halmos/console.py
 src/halmos/exceptions.py
 src/halmos/parser.py
 src/halmos/pools.py
 src/halmos/sevm.py
 src/halmos/utils.py
 src/halmos/warnings.py
 src/halmos.egg-info/PKG-INFO
```

### Comparing `halmos-0.1.8/tests/expected/all.json` & `halmos-0.1.9/tests/expected/all.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997393731503901%*

 * *Differences: {"'test_results'": "{'test/Console.t.sol:ConsoleTest': {8: {'name': 'check_log_unsupported()'}, "*

 * *                   "insert: [(0, OrderedDict([('name', 'check_log_address()'), ('exitcode', 0), "*

 * *                   "('num_models', 0), ('models', None), ('num_paths', None), ('time', None), "*

 * *                   "('num_bounded_loops', None)])), (1, OrderedDict([('name', 'check_log_bool()'), "*

 * *                   "('exitcode', 0), ('num_models', 0), ('models', None), ('num_paths', None), "*

 * *                   "(' […]*

```diff
@@ -251,15 +251,87 @@
                 "time": null
             }
         ],
         "test/Console.t.sol:ConsoleTest": [
             {
                 "exitcode": 0,
                 "models": null,
-                "name": "check_log()",
+                "name": "check_log_address()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_log_bool()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_log_bytes()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_log_bytes32()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_log_int()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_log_string()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_log_uint()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_log_undecodable_string()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_log_unsupported()",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             }
         ],
         "test/Const.t.sol:ConstTest": [
@@ -785,14 +857,50 @@
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             },
             {
                 "exitcode": 0,
+                "models": null,
+                "name": "check_createBytes4()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_createInt()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_createInt256()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "models": null,
+                "name": "check_createString()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
                 "models": null,
                 "name": "check_createUint()",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             },
```

### Comparing `halmos-0.1.8/tests/expected/erc20.json` & `halmos-0.1.9/tests/expected/erc20.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/expected/erc721.json` & `halmos-0.1.9/tests/expected/erc721.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/expected/ffi.json` & `halmos-0.1.9/tests/expected/ffi.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/expected/simple.json` & `halmos-0.1.9/tests/expected/simple.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/expected/solver.json` & `halmos-0.1.9/tests/expected/solver.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/ffi/test/Ffi.t.sol` & `halmos-0.1.9/tests/ffi/test/Ffi.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/src/Counter.sol` & `halmos-0.1.9/tests/regression/src/Counter.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/src/Storage.sol` & `halmos-0.1.9/tests/regression/src/Storage.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Arith.t.sol` & `halmos-0.1.9/tests/regression/test/Arith.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/AssertTest.t.sol` & `halmos-0.1.9/tests/regression/test/AssertTest.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Block.t.sol` & `halmos-0.1.9/tests/regression/test/Block.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Buffers.t.sol` & `halmos-0.1.9/tests/regression/test/Buffers.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Byte.t.sol` & `halmos-0.1.9/tests/regression/test/Byte.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Call.t.sol` & `halmos-0.1.9/tests/regression/test/Call.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/CallAlias.t.sol` & `halmos-0.1.9/tests/regression/test/CallAlias.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Constructor.t.sol` & `halmos-0.1.9/tests/regression/test/Constructor.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Context.t.sol` & `halmos-0.1.9/tests/regression/test/Context.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Counter.t.sol` & `halmos-0.1.9/tests/regression/test/Counter.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Create.t.sol` & `halmos-0.1.9/tests/regression/test/Create.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Create2.t.sol` & `halmos-0.1.9/tests/regression/test/Create2.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Deal.t.sol` & `halmos-0.1.9/tests/regression/test/Deal.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Foundry.t.sol` & `halmos-0.1.9/tests/regression/test/Foundry.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/HalmosCheatCode.t.sol` & `halmos-0.1.9/tests/regression/test/HalmosCheatCode.t.sol`

 * *Files 5% similar despite different names*

```diff
@@ -9,34 +9,61 @@
         uint y = svm.createUint(160, 'y');
         uint z = svm.createUint(8, 'z');
         assert(0 <= x && x <= type(uint256).max);
         assert(0 <= y && y <= type(uint160).max);
         assert(0 <= z && z <= type(uint8).max);
     }
 
+    function check_createInt() public {
+        int x = svm.createInt(256, 'x');
+        int y = svm.createInt(160, 'y');
+        int z = svm.createInt(8, 'z');
+        assert(type(int256).min <= x && x <= type(int256).max);
+        assert(type(int160).min <= y && y <= type(int160).max);
+        assert(type(int8).min <= z && z <= type(int8).max);
+    }
+
     function check_createBytes() public {
         bytes memory data = svm.createBytes(2, 'data');
         uint x = uint(uint8(data[0]));
         uint y = uint(uint8(data[1]));
         assert(0 <= x && x <= type(uint8).max);
         assert(0 <= y && y <= type(uint8).max);
     }
 
+    function check_createString() public {
+        string memory data = svm.createString(5, 'str');
+        assert(bytes(data).length == 5);
+    }
+
     function check_createUint256() public {
         uint x = svm.createUint256('x');
         assert(0 <= x && x <= type(uint256).max);
     }
 
+    function check_createInt256() public {
+        int x = svm.createInt256('x');
+        assert(type(int256).min <= x && x <= type(int256).max);
+    }
+
     function check_createBytes32() public {
         bytes32 x = svm.createBytes32('x');
         assert(0 <= uint(x) && uint(x) <= type(uint256).max);
         uint y; assembly { y := x }
         assert(0 <= y && y <= type(uint256).max);
     }
 
+    function check_createBytes4() public {
+        bytes4 x = svm.createBytes4('x');
+        uint256 x_uint = uint256(uint32(x));
+        assert(0 <= x_uint && x_uint <= type(uint32).max);
+        uint y; assembly { y := x }
+        assert(0 <= y && y <= type(uint256).max);
+    }
+
     function check_createAddress() public {
         address x = svm.createAddress('x');
         uint y; assembly { y := x }
         assert(0 <= y && y <= type(uint160).max);
     }
 
     function check_createBool() public {
```

### Comparing `halmos-0.1.8/tests/regression/test/Invalid.t.sol` & `halmos-0.1.9/tests/regression/test/Invalid.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Library.t.sol` & `halmos-0.1.9/tests/regression/test/Library.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/List.t.sol` & `halmos-0.1.9/tests/regression/test/List.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Natspec.t.sol` & `halmos-0.1.9/tests/regression/test/Natspec.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Opcode.t.sol` & `halmos-0.1.9/tests/regression/test/Opcode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Prank.t.sol` & `halmos-0.1.9/tests/regression/test/Prank.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Proxy.t.sol` & `halmos-0.1.9/tests/regression/test/Proxy.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Reset.t.sol` & `halmos-0.1.9/tests/regression/test/Reset.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Revert.t.sol` & `halmos-0.1.9/tests/regression/test/Revert.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Send.t.sol` & `halmos-0.1.9/tests/regression/test/Send.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Setup.t.sol` & `halmos-0.1.9/tests/regression/test/Setup.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/SetupPlus.t.sol` & `halmos-0.1.9/tests/regression/test/SetupPlus.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Signature.t.sol` & `halmos-0.1.9/tests/regression/test/Signature.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/SmolWETH.t.sol` & `halmos-0.1.9/tests/regression/test/SmolWETH.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/StaticContexts.t.sol` & `halmos-0.1.9/tests/regression/test/StaticContexts.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Storage.t.sol` & `halmos-0.1.9/tests/regression/test/Storage.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Storage2.t.sol` & `halmos-0.1.9/tests/regression/test/Storage2.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Store.t.sol` & `halmos-0.1.9/tests/regression/test/Store.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Struct.t.sol` & `halmos-0.1.9/tests/regression/test/Struct.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/TestConstructor.t.sol` & `halmos-0.1.9/tests/regression/test/TestConstructor.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Token.t.sol` & `halmos-0.1.9/tests/regression/test/Token.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/UnknownCall.t.sol` & `halmos-0.1.9/tests/regression/test/UnknownCall.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/UnsupportedOpcode.t.sol` & `halmos-0.1.9/tests/regression/test/UnsupportedOpcode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/regression/test/Warp.t.sol` & `halmos-0.1.9/tests/regression/test/Warp.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/solver/test/Math.t.sol` & `halmos-0.1.9/tests/solver/test/Math.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/solver/test/SignedDiv.t.sol` & `halmos-0.1.9/tests/solver/test/SignedDiv.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/test_cli.py` & `halmos-0.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/test_fixtures.py` & `halmos-0.1.9/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/test_halmos.py` & `halmos-0.1.9/tests/test_halmos.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/test_sevm.py` & `halmos-0.1.9/tests/test_sevm.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.8/tests/test_traces.py` & `halmos-0.1.9/tests/test_traces.py`

 * *Files identical despite different names*

