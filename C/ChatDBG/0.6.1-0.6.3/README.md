# Comparing `tmp/chatdbg-0.6.1.tar.gz` & `tmp/chatdbg-0.6.3.tar.gz`

## Comparing `chatdbg-0.6.1.tar` & `chatdbg-0.6.3.tar`

### file list

```diff
@@ -1,197 +1,199 @@
--rw-r--r--   0        0        0   431302 2020-02-02 00:00:00.000000 chatdbg-0.6.1/ChatDBG-arxiv-2403.16354.pdf
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 chatdbg-0.6.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 chatdbg-0.6.1/.github/workflows/sanity.yml
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 chatdbg-0.6.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0    12771 2020-02-02 00:00:00.000000 chatdbg-0.6.1/media/gdb.svg
--rw-r--r--   0        0        0    17963 2020-02-02 00:00:00.000000 chatdbg-0.6.1/media/lldb.svg
--rw-r--r--   0        0        0    11033 2020-02-02 00:00:00.000000 chatdbg-0.6.1/media/pdb.svg
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 chatdbg-0.6.1/rust-support/Cargo.toml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chatdbg-0.6.1/rust-support/chatdbg/Cargo.toml
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 chatdbg-0.6.1/rust-support/chatdbg/src/lib.rs
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 chatdbg-0.6.1/rust-support/chatdbg_macros/Cargo.toml
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chatdbg-0.6.1/rust-support/chatdbg_macros/src/lib.rs
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-deep-recursion.cpp
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-definition-likely.cpp
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-failed-assert.cpp
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-failed-assert.why.txt
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-input-file.cpp
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-input-file.txt
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-overflow.cpp
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-overflow.why.txt
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-pointers-loop.cpp
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-pointers.cpp
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-stack-overflow.cpp
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-stack-overflow.why.txt
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-use-after-free.cpp
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-use-after-free.why.txt
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-user-input.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/cpp/test-user-input.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/README.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/bootstrap.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/bootstrap2.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/ds101.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/marble-sample.csv
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/marbles.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/mean.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/nb.ipynb
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/requirements.txt
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/sample.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/python/testme.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/rust/.gitignore
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/rust/Cargo.toml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.6.1/samples/rust/test-failed-assert.rs
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/__init__.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/__main__.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/chatdbg_gdb.py
--rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/chatdbg_lldb.py
--rw-r--r--   0        0        0    23352 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/chatdbg_pdb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/assistant/__init__.py
--rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/assistant/assistant.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/assistant/listeners.py
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/native_util/clangd_lsp_integration.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/native_util/code.py
--rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/native_util/dbg_dialog.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/native_util/stacks.py
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/old_stuff/chatdbg_utils.py
--rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/old_stuff/gdb_print_test.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/old_stuff/lldb_why.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/old_stuff/prompts.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/pdb/prompts.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/pdb/text.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/pdb_util/capture.py
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/pdb_util/locals.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/pdb_util/paths.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/config.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/history.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/instructions.txt
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/jupyter.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/log.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/markdown.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/plog.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/printer.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/prompts.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/stream.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/text.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/trim.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/util/wrap.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/CMakeLists.txt
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/build-chatdbg.bat
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/chatdbg.cpp
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/vcpkg-configuration.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/vcpkg.json
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/include/appendlines.hpp
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/include/getmodel.hpp
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/include/joinstrings.hpp
--rw-r--r--   0        0        0    25429 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/include/openai.hpp
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/include/wordwrap.hpp
--rw-r--r--   0        0        0   915040 2020-02-02 00:00:00.000000 chatdbg-0.6.1/src/chatdbg/windbg/nlohmann/json.hpp
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/requirements.txt
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_1.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_10.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_100.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_101.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_102.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_103.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_104.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_105.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_11.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_12.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_13.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_14.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_15.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_16.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_17.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_18.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_19.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_2.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_20.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_21.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_22.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_23.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_24.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_25.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_26.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_27.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_28.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_29.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_3.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_30.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_31.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_32.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_33.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_34.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_35.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_36.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_37.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_38.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_39.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_4.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_40.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_41.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_42.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_43.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_44.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_45.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_46.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_47.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_48.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_49.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_5.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_50.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_51.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_52.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_53.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_54.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_55.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_56.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_57.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_58.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_59.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_6.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_60.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_61.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_62.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_63.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_64.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_65.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_66.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_67.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_68.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_69.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_7.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_70.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_71.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_72.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_73.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_74.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_75.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_76.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_77.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_78.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_79.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_8.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_80.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_81.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_82.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_83.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_84.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_85.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_86.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_87.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_88.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_89.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_9.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_90.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_91.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_92.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_93.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_94.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_95.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_96.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_97.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 chatdbg-0.6.1/test/test_coverup_99.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 chatdbg-0.6.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 chatdbg-0.6.1/LICENSE
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 chatdbg-0.6.1/README.md
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 chatdbg-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    12763 2020-02-02 00:00:00.000000 chatdbg-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0   431302 2020-02-02 00:00:00.000000 chatdbg-0.6.3/ChatDBG-arxiv-2403.16354.pdf
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chatdbg-0.6.3/check-version-bump.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 chatdbg-0.6.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 chatdbg-0.6.3/.github/workflows/sanity.yml
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 chatdbg-0.6.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    12771 2020-02-02 00:00:00.000000 chatdbg-0.6.3/media/gdb.svg
+-rw-r--r--   0        0        0    17963 2020-02-02 00:00:00.000000 chatdbg-0.6.3/media/lldb.svg
+-rw-r--r--   0        0        0    11033 2020-02-02 00:00:00.000000 chatdbg-0.6.3/media/pdb.svg
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 chatdbg-0.6.3/rust-support/Cargo.toml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 chatdbg-0.6.3/rust-support/fill-crate-version.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chatdbg-0.6.3/rust-support/chatdbg/Cargo.toml
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 chatdbg-0.6.3/rust-support/chatdbg/src/lib.rs
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 chatdbg-0.6.3/rust-support/chatdbg_macros/Cargo.toml
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chatdbg-0.6.3/rust-support/chatdbg_macros/src/lib.rs
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-deep-recursion.cpp
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-definition-likely.cpp
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-failed-assert.cpp
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-failed-assert.why.txt
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-input-file.cpp
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-input-file.txt
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-overflow.cpp
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-overflow.why.txt
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-pointers-loop.cpp
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-pointers.cpp
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-stack-overflow.cpp
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-stack-overflow.why.txt
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-use-after-free.cpp
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-use-after-free.why.txt
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-user-input.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/cpp/test-user-input.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/README.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/bootstrap.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/bootstrap2.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/ds101.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/marble-sample.csv
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/marbles.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/mean.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/nb.ipynb
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/requirements.txt
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/sample.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/python/testme.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/rust/.gitignore
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/rust/Cargo.toml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.6.3/samples/rust/test-failed-assert.rs
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/__main__.py
+-rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/chatdbg_gdb.py
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/chatdbg_lldb.py
+-rw-r--r--   0        0        0    23352 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/chatdbg_pdb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/assistant/__init__.py
+-rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/assistant/assistant.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/assistant/listeners.py
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/native_util/clangd_lsp_integration.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/native_util/code.py
+-rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/native_util/dbg_dialog.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/native_util/stacks.py
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/old_stuff/chatdbg_utils.py
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/old_stuff/gdb_print_test.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/old_stuff/lldb_why.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/old_stuff/prompts.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/pdb/prompts.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/pdb/text.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/pdb_util/capture.py
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/pdb_util/locals.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/pdb_util/paths.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/config.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/history.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/instructions.txt
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/jupyter.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/log.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/markdown.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/plog.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/printer.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/prompts.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/stream.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/text.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/trim.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/util/wrap.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/CMakeLists.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/build-chatdbg.bat
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/chatdbg.cpp
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/vcpkg-configuration.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/vcpkg.json
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/include/appendlines.hpp
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/include/getmodel.hpp
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/include/joinstrings.hpp
+-rw-r--r--   0        0        0    25429 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/include/openai.hpp
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/include/wordwrap.hpp
+-rw-r--r--   0        0        0   915040 2020-02-02 00:00:00.000000 chatdbg-0.6.3/src/chatdbg/windbg/nlohmann/json.hpp
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/requirements.txt
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_1.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_10.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_100.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_101.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_102.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_103.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_104.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_105.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_11.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_12.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_13.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_14.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_15.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_16.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_17.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_18.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_19.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_2.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_20.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_21.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_22.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_23.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_24.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_25.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_26.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_27.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_28.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_29.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_3.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_30.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_31.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_32.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_33.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_34.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_35.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_36.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_37.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_38.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_39.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_4.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_40.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_41.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_42.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_43.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_44.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_45.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_46.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_47.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_48.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_49.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_5.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_50.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_51.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_52.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_53.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_54.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_55.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_56.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_57.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_58.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_59.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_6.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_60.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_61.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_62.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_63.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_64.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_65.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_66.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_67.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_68.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_69.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_7.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_70.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_71.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_72.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_73.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_74.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_75.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_76.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_77.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_78.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_79.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_8.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_80.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_81.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_82.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_83.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_84.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_85.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_86.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_87.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_88.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_89.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_9.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_90.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_91.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_92.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_93.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_94.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_95.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_96.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_97.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 chatdbg-0.6.3/test/test_coverup_99.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 chatdbg-0.6.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 chatdbg-0.6.3/LICENSE
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 chatdbg-0.6.3/README.md
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 chatdbg-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    12763 2020-02-02 00:00:00.000000 chatdbg-0.6.3/PKG-INFO
```

### Comparing `chatdbg-0.6.1/ChatDBG-arxiv-2403.16354.pdf` & `chatdbg-0.6.3/ChatDBG-arxiv-2403.16354.pdf`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/.github/workflows/release.yml` & `chatdbg-0.6.3/.github/workflows/release.yml`

 * *Files 23% similar despite different names*

```diff
@@ -13,22 +13,36 @@
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
-        python-version: '3.x'
+        python-version: '>=3.11'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install build
+        pip install build packaging requests
+
+    - name: Check version bump
+      run: python3 check-version-bump.py
+
+    - name: Sync pyproject.toml/Cargo.toml versions
+      run: python3 rust-support/fill-crate-version.py
 
     - name: Build package
       run: python -m build
 
-    - name: Publish package
+    - name: Publish to crates.io
+      run: |
+        cargo publish -p chatdbg_macros --allow-dirty
+        cargo publish -p chatdbg --allow-dirty
+      env:
+        CARGO_REGISTRY_TOKEN: ${{ secrets.CARGO_REGISTRY_TOKEN }}
+      working-directory: rust-support
+
+    - name: Publish to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `chatdbg-0.6.1/.github/workflows/sanity.yml` & `chatdbg-0.6.3/.github/workflows/sanity.yml`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/.github/workflows/tests.yml` & `chatdbg-0.6.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/media/gdb.svg` & `chatdbg-0.6.3/media/gdb.svg`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/media/lldb.svg` & `chatdbg-0.6.3/media/lldb.svg`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/media/pdb.svg` & `chatdbg-0.6.3/media/pdb.svg`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/rust-support/chatdbg/src/lib.rs` & `chatdbg-0.6.3/rust-support/chatdbg/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/rust-support/chatdbg_macros/src/lib.rs` & `chatdbg-0.6.3/rust-support/chatdbg_macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/cpp/test-deep-recursion.cpp` & `chatdbg-0.6.3/samples/cpp/test-deep-recursion.cpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/cpp/test-failed-assert.why.txt` & `chatdbg-0.6.3/samples/cpp/test-failed-assert.why.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/cpp/test-input-file.cpp` & `chatdbg-0.6.3/samples/cpp/test-input-file.cpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/cpp/test-overflow.why.txt` & `chatdbg-0.6.3/samples/cpp/test-overflow.why.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/cpp/test-use-after-free.why.txt` & `chatdbg-0.6.3/samples/cpp/test-use-after-free.why.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/cpp/test-user-input.cpp` & `chatdbg-0.6.3/samples/cpp/test-user-input.cpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/python/bootstrap.py` & `chatdbg-0.6.3/samples/python/bootstrap.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/python/bootstrap2.py` & `chatdbg-0.6.3/samples/python/bootstrap2.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/python/ds101.py` & `chatdbg-0.6.3/samples/python/ds101.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/python/mean.py` & `chatdbg-0.6.3/samples/python/mean.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/samples/python/nb.ipynb` & `chatdbg-0.6.3/samples/python/nb.ipynb`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/__main__.py` & `chatdbg-0.6.3/src/chatdbg/__main__.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/chatdbg_gdb.py` & `chatdbg-0.6.3/src/chatdbg/chatdbg_gdb.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/chatdbg_lldb.py` & `chatdbg-0.6.3/src/chatdbg/chatdbg_lldb.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/chatdbg_pdb.py` & `chatdbg-0.6.3/src/chatdbg/chatdbg_pdb.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/assistant/assistant.py` & `chatdbg-0.6.3/src/chatdbg/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/assistant/listeners.py` & `chatdbg-0.6.3/src/chatdbg/assistant/listeners.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/native_util/clangd_lsp_integration.py` & `chatdbg-0.6.3/src/chatdbg/native_util/clangd_lsp_integration.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/native_util/dbg_dialog.py` & `chatdbg-0.6.3/src/chatdbg/native_util/dbg_dialog.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/native_util/stacks.py` & `chatdbg-0.6.3/src/chatdbg/native_util/stacks.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/old_stuff/chatdbg_utils.py` & `chatdbg-0.6.3/src/chatdbg/old_stuff/chatdbg_utils.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/old_stuff/gdb_print_test.py` & `chatdbg-0.6.3/src/chatdbg/old_stuff/gdb_print_test.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/old_stuff/lldb_why.py` & `chatdbg-0.6.3/src/chatdbg/old_stuff/lldb_why.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/old_stuff/prompts.py` & `chatdbg-0.6.3/src/chatdbg/old_stuff/prompts.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/pdb/prompts.py` & `chatdbg-0.6.3/src/chatdbg/pdb/prompts.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/pdb/text.py` & `chatdbg-0.6.3/src/chatdbg/pdb/text.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/pdb_util/capture.py` & `chatdbg-0.6.3/src/chatdbg/pdb_util/capture.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/pdb_util/locals.py` & `chatdbg-0.6.3/src/chatdbg/pdb_util/locals.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/pdb_util/paths.py` & `chatdbg-0.6.3/src/chatdbg/pdb_util/paths.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/config.py` & `chatdbg-0.6.3/src/chatdbg/util/config.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/history.py` & `chatdbg-0.6.3/src/chatdbg/util/history.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/instructions.txt` & `chatdbg-0.6.3/src/chatdbg/util/instructions.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/jupyter.py` & `chatdbg-0.6.3/src/chatdbg/util/jupyter.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/log.py` & `chatdbg-0.6.3/src/chatdbg/util/log.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/markdown.py` & `chatdbg-0.6.3/src/chatdbg/util/markdown.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/plog.py` & `chatdbg-0.6.3/src/chatdbg/util/plog.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/printer.py` & `chatdbg-0.6.3/src/chatdbg/util/printer.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/prompts.py` & `chatdbg-0.6.3/src/chatdbg/util/prompts.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/stream.py` & `chatdbg-0.6.3/src/chatdbg/util/stream.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/text.py` & `chatdbg-0.6.3/src/chatdbg/util/text.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/trim.py` & `chatdbg-0.6.3/src/chatdbg/util/trim.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/util/wrap.py` & `chatdbg-0.6.3/src/chatdbg/util/wrap.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/windbg/CMakeLists.txt` & `chatdbg-0.6.3/src/chatdbg/windbg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/windbg/chatdbg.cpp` & `chatdbg-0.6.3/src/chatdbg/windbg/chatdbg.cpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/windbg/include/appendlines.hpp` & `chatdbg-0.6.3/src/chatdbg/windbg/include/appendlines.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/windbg/include/openai.hpp` & `chatdbg-0.6.3/src/chatdbg/windbg/include/openai.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/windbg/include/wordwrap.hpp` & `chatdbg-0.6.3/src/chatdbg/windbg/include/wordwrap.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/src/chatdbg/windbg/nlohmann/json.hpp` & `chatdbg-0.6.3/src/chatdbg/windbg/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_1.py` & `chatdbg-0.6.3/test/test_coverup_1.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_10.py` & `chatdbg-0.6.3/test/test_coverup_10.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_100.py` & `chatdbg-0.6.3/test/test_coverup_100.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_101.py` & `chatdbg-0.6.3/test/test_coverup_101.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_102.py` & `chatdbg-0.6.3/test/test_coverup_102.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_103.py` & `chatdbg-0.6.3/test/test_coverup_103.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_104.py` & `chatdbg-0.6.3/test/test_coverup_104.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_105.py` & `chatdbg-0.6.3/test/test_coverup_105.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_11.py` & `chatdbg-0.6.3/test/test_coverup_11.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_12.py` & `chatdbg-0.6.3/test/test_coverup_12.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_13.py` & `chatdbg-0.6.3/test/test_coverup_13.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_14.py` & `chatdbg-0.6.3/test/test_coverup_14.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_15.py` & `chatdbg-0.6.3/test/test_coverup_15.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_16.py` & `chatdbg-0.6.3/test/test_coverup_16.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_17.py` & `chatdbg-0.6.3/test/test_coverup_17.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_18.py` & `chatdbg-0.6.3/test/test_coverup_18.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_19.py` & `chatdbg-0.6.3/test/test_coverup_19.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_2.py` & `chatdbg-0.6.3/test/test_coverup_2.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_20.py` & `chatdbg-0.6.3/test/test_coverup_20.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_21.py` & `chatdbg-0.6.3/test/test_coverup_21.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_22.py` & `chatdbg-0.6.3/test/test_coverup_22.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_23.py` & `chatdbg-0.6.3/test/test_coverup_23.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_24.py` & `chatdbg-0.6.3/test/test_coverup_24.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_26.py` & `chatdbg-0.6.3/test/test_coverup_26.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_27.py` & `chatdbg-0.6.3/test/test_coverup_27.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_28.py` & `chatdbg-0.6.3/test/test_coverup_28.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_29.py` & `chatdbg-0.6.3/test/test_coverup_29.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_3.py` & `chatdbg-0.6.3/test/test_coverup_3.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_30.py` & `chatdbg-0.6.3/test/test_coverup_30.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_31.py` & `chatdbg-0.6.3/test/test_coverup_31.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_32.py` & `chatdbg-0.6.3/test/test_coverup_32.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_33.py` & `chatdbg-0.6.3/test/test_coverup_33.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_34.py` & `chatdbg-0.6.3/test/test_coverup_34.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_35.py` & `chatdbg-0.6.3/test/test_coverup_35.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_36.py` & `chatdbg-0.6.3/test/test_coverup_36.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_37.py` & `chatdbg-0.6.3/test/test_coverup_37.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_38.py` & `chatdbg-0.6.3/test/test_coverup_38.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_39.py` & `chatdbg-0.6.3/test/test_coverup_39.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_4.py` & `chatdbg-0.6.3/test/test_coverup_4.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_40.py` & `chatdbg-0.6.3/test/test_coverup_40.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_41.py` & `chatdbg-0.6.3/test/test_coverup_41.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_42.py` & `chatdbg-0.6.3/test/test_coverup_42.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_43.py` & `chatdbg-0.6.3/test/test_coverup_43.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_44.py` & `chatdbg-0.6.3/test/test_coverup_44.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_45.py` & `chatdbg-0.6.3/test/test_coverup_45.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_46.py` & `chatdbg-0.6.3/test/test_coverup_46.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_47.py` & `chatdbg-0.6.3/test/test_coverup_47.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_48.py` & `chatdbg-0.6.3/test/test_coverup_48.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_49.py` & `chatdbg-0.6.3/test/test_coverup_49.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_5.py` & `chatdbg-0.6.3/test/test_coverup_5.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_50.py` & `chatdbg-0.6.3/test/test_coverup_50.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_51.py` & `chatdbg-0.6.3/test/test_coverup_51.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_52.py` & `chatdbg-0.6.3/test/test_coverup_52.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_53.py` & `chatdbg-0.6.3/test/test_coverup_53.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_54.py` & `chatdbg-0.6.3/test/test_coverup_54.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_55.py` & `chatdbg-0.6.3/test/test_coverup_55.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_56.py` & `chatdbg-0.6.3/test/test_coverup_56.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_57.py` & `chatdbg-0.6.3/test/test_coverup_57.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_58.py` & `chatdbg-0.6.3/test/test_coverup_58.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_59.py` & `chatdbg-0.6.3/test/test_coverup_59.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_6.py` & `chatdbg-0.6.3/test/test_coverup_6.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_60.py` & `chatdbg-0.6.3/test/test_coverup_60.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_61.py` & `chatdbg-0.6.3/test/test_coverup_61.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_62.py` & `chatdbg-0.6.3/test/test_coverup_62.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_63.py` & `chatdbg-0.6.3/test/test_coverup_63.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_64.py` & `chatdbg-0.6.3/test/test_coverup_64.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_65.py` & `chatdbg-0.6.3/test/test_coverup_65.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_66.py` & `chatdbg-0.6.3/test/test_coverup_66.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_67.py` & `chatdbg-0.6.3/test/test_coverup_67.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_7.py` & `chatdbg-0.6.3/test/test_coverup_7.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_70.py` & `chatdbg-0.6.3/test/test_coverup_70.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_71.py` & `chatdbg-0.6.3/test/test_coverup_71.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_72.py` & `chatdbg-0.6.3/test/test_coverup_72.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_73.py` & `chatdbg-0.6.3/test/test_coverup_73.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_74.py` & `chatdbg-0.6.3/test/test_coverup_74.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_75.py` & `chatdbg-0.6.3/test/test_coverup_75.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_76.py` & `chatdbg-0.6.3/test/test_coverup_76.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_77.py` & `chatdbg-0.6.3/test/test_coverup_77.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_78.py` & `chatdbg-0.6.3/test/test_coverup_78.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_79.py` & `chatdbg-0.6.3/test/test_coverup_79.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_8.py` & `chatdbg-0.6.3/test/test_coverup_8.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_80.py` & `chatdbg-0.6.3/test/test_coverup_80.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_81.py` & `chatdbg-0.6.3/test/test_coverup_81.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_82.py` & `chatdbg-0.6.3/test/test_coverup_82.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_83.py` & `chatdbg-0.6.3/test/test_coverup_83.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_84.py` & `chatdbg-0.6.3/test/test_coverup_84.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_85.py` & `chatdbg-0.6.3/test/test_coverup_85.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_86.py` & `chatdbg-0.6.3/test/test_coverup_86.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_87.py` & `chatdbg-0.6.3/test/test_coverup_87.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_88.py` & `chatdbg-0.6.3/test/test_coverup_88.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_89.py` & `chatdbg-0.6.3/test/test_coverup_89.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_9.py` & `chatdbg-0.6.3/test/test_coverup_9.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_91.py` & `chatdbg-0.6.3/test/test_coverup_91.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_94.py` & `chatdbg-0.6.3/test/test_coverup_94.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_95.py` & `chatdbg-0.6.3/test/test_coverup_95.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_96.py` & `chatdbg-0.6.3/test/test_coverup_96.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_97.py` & `chatdbg-0.6.3/test/test_coverup_97.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/test/test_coverup_99.py` & `chatdbg-0.6.3/test/test_coverup_99.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/.gitignore` & `chatdbg-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/LICENSE` & `chatdbg-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatdbg-0.6.1/README.md` & `chatdbg-0.6.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 To use ChatDBG with Rust, you need to do two steps: modify your
 `Cargo.toml` file and add one line to your source program.
 
 1. Add this to your `Cargo.toml` file:
 
 ```toml
 [dependencies]
-chatdbg = "0.1.3"
+chatdbg = "0.6.2"
 
 [profile.dev]
 panic = "abort"
 
 [profile.release]
 panic = "abort"
 ```
```

#### html2text {}

```diff
@@ -93,15 +93,15 @@
 debuggers work slightly differently than Pdb. After the debugger responds to
 your question, you will enter into ChatDBG's command loop, as indicated by the
 `(ChatDBG chatting)` prompt. You may continue issuing debugging commands and
 you may send additional messages to the LLM by starting those messages with
 "chat". When you are done, type `quit` to return to the debugger's main command
 loop. DDeebbuuggggiinngg RRuusstt pprrooggrraammss To use ChatDBG with Rust, you need to do two
 steps: modify your `Cargo.toml` file and add one line to your source program.
-1. Add this to your `Cargo.toml` file: ```toml [dependencies] chatdbg = "0.1.3"
+1. Add this to your `Cargo.toml` file: ```toml [dependencies] chatdbg = "0.6.2"
 [profile.dev] panic = "abort" [profile.release] panic = "abort" ``` 2. In your
 program, apply the `#[chatdbg::main]` attribute to your `main` function:
 ```rust #[chatdbg::main] fn main() { ``` Now you can debug your Rust code with
 `gdb` or `lldb`. ### Examples CChhaattDDBBGG eexxaammppllee iinn llllddbb ```gdb (ChatDBG lldb) run
 Process 85494 launched: '/Users/emery/git/ChatDBG/test/a.out' (arm64) TEST 1
 TEST -422761288 TEST 0 TEST 0 TEST 0 TEST 0 TEST 0 TEST 0 Process 85494 stopped
 * thread #1, queue = 'com.apple.main-thread', stop reason = EXC_BAD_ACCESS
```

### Comparing `chatdbg-0.6.1/pyproject.toml` & `chatdbg-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ChatDBG"
-version = "0.6.1"
+version = "0.6.3"
 authors = [
   { name="Emery Berger", email="emery.berger@gmail.com" },
   { name="Stephen Freund", email="sfreund@williams.edu" },
   { name="Kyla Levin", email="khlevin@umass.edu" },
   { name="Nicolas van Kempen", email="nvankemp@gmail.com" },
 ]
 dependencies = [
```

### Comparing `chatdbg-0.6.1/PKG-INFO` & `chatdbg-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ChatDBG
-Version: 0.6.1
+Version: 0.6.3
 Summary: AI-assisted debugging. Uses AI to answer 'why'.
 Project-URL: Homepage, https://github.com/plasma-umass/ChatDBG
 Project-URL: Bug Tracker, https://github.com/plasma-umass/ChatDBG/issues
 Author-email: Emery Berger <emery.berger@gmail.com>, Stephen Freund <sfreund@williams.edu>, Kyla Levin <khlevin@umass.edu>, Nicolas van Kempen <nvankemp@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -200,15 +200,15 @@
 To use ChatDBG with Rust, you need to do two steps: modify your
 `Cargo.toml` file and add one line to your source program.
 
 1. Add this to your `Cargo.toml` file:
 
 ```toml
 [dependencies]
-chatdbg = "0.1.3"
+chatdbg = "0.6.2"
 
 [profile.dev]
 panic = "abort"
 
 [profile.release]
 panic = "abort"
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: ChatDBG Version: 0.6.1 Summary: AI-assisted
+Metadata-Version: 2.3 Name: ChatDBG Version: 0.6.3 Summary: AI-assisted
 debugging. Uses AI to answer 'why'. Project-URL: Homepage, https://github.com/
 plasma-umass/ChatDBG Project-URL: Bug Tracker, https://github.com/plasma-umass/
 ChatDBG/issues Author-email: Emery Berger
 gmail.com>, Stephen Freund
 williams.edu>, Kyla Levin
 umass.edu>, Nicolas van Kempen
 gmail.com> License-File: LICENSE Classifier: License :: OSI Approved :: Apache
@@ -108,15 +108,15 @@
 debuggers work slightly differently than Pdb. After the debugger responds to
 your question, you will enter into ChatDBG's command loop, as indicated by the
 `(ChatDBG chatting)` prompt. You may continue issuing debugging commands and
 you may send additional messages to the LLM by starting those messages with
 "chat". When you are done, type `quit` to return to the debugger's main command
 loop. DDeebbuuggggiinngg RRuusstt pprrooggrraammss To use ChatDBG with Rust, you need to do two
 steps: modify your `Cargo.toml` file and add one line to your source program.
-1. Add this to your `Cargo.toml` file: ```toml [dependencies] chatdbg = "0.1.3"
+1. Add this to your `Cargo.toml` file: ```toml [dependencies] chatdbg = "0.6.2"
 [profile.dev] panic = "abort" [profile.release] panic = "abort" ``` 2. In your
 program, apply the `#[chatdbg::main]` attribute to your `main` function:
 ```rust #[chatdbg::main] fn main() { ``` Now you can debug your Rust code with
 `gdb` or `lldb`. ### Examples CChhaattDDBBGG eexxaammppllee iinn llllddbb ```gdb (ChatDBG lldb) run
 Process 85494 launched: '/Users/emery/git/ChatDBG/test/a.out' (arm64) TEST 1
 TEST -422761288 TEST 0 TEST 0 TEST 0 TEST 0 TEST 0 TEST 0 Process 85494 stopped
 * thread #1, queue = 'com.apple.main-thread', stop reason = EXC_BAD_ACCESS
```

