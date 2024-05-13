# Comparing `tmp/ms-ait-7.0.0b430.zip` & `tmp/ms-ait-7.0.0rc2.zip`

## zipinfo {}

```diff
@@ -1,548 +1,529 @@
-Zip file size: 691450 bytes, number of entries: 546
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/ms_ait.egg-info/
--rwxrwxrwx  2.0 unx      228 b- defN 24-May-13 12:35 ms-ait-7.0.0b430/PKG-INFO
--rwxrwxrwx  2.0 unx     4802 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/README.md
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/requirements.txt
--rwxrwxrwx  2.0 unx       38 b- defN 24-May-13 12:35 ms-ait-7.0.0b430/setup.cfg
--rwxrwxrwx  2.0 unx     1855 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/setup.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/profile/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/tensor_view/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/tests/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/utils/
--rwxrwxrwx  2.0 unx      600 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/__init__.py
--rwxrwxrwx  2.0 unx     1744 b- defN 24-May-08 11:39 ms-ait-7.0.0b430/components/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/
--rwxrwxrwx  2.0 unx     5220 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/README.md
--rwxrwxrwx  2.0 unx       65 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/requirements.txt
--rwxrwxrwx  2.0 unx     2227 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/analyze/setup.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/analyze/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/data/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/__init__.py
--rwxrwxrwx  2.0 unx      695 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/analyze/model_evaluation/__install__.py
--rwxrwxrwx  2.0 unx     5943 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/__main__.py
--rwxrwxrwx  2.0 unx      843 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/config.py
--rwxrwxrwx  2.0 unx      936 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/op_info.py
--rwxrwxrwx  2.0 unx      712 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/
--rwxrwxrwx  2.0 unx      882 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/const.py
--rwxrwxrwx  2.0 unx     1078 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/log.py
--rwxrwxrwx  2.0 unx     1917 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/utils.py
--rwxrwxrwx  2.0 unx       95 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/__init__.py
--rwxrwxrwx  2.0 unx     1072 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/atc_err.py
--rwxrwxrwx  2.0 unx      730 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/engine.py
--rwxrwxrwx  2.0 unx      712 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/framework.py
--rwxrwxrwx  2.0 unx      852 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
--rwxrwxrwx  2.0 unx      692 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/soc_type.py
--rwxrwxrwx  2.0 unx      305 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/
--rwxrwxrwx  2.0 unx     7722 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/analysis.py
--rwxrwxrwx  2.0 unx     4707 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/result.py
--rwxrwxrwx  2.0 unx     1236 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/rule.py
--rwxrwxrwx  2.0 unx       51 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/__init__.py
--rwxrwxrwx  2.0 unx     2495 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/onnx.py
--rwxrwxrwx  2.0 unx       59 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/__init__.py
--rwxrwxrwx  2.0 unx     4428 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/data/opp.py
--rwxrwxrwx  2.0 unx     2212 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/data/op_map.py
--rwxrwxrwx  2.0 unx      683 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/data/__init__.py
--rwxrwxrwx  2.0 unx     2210 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/onnx.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/__init__.py
--rwxrwxrwx  2.0 unx     4426 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/atc.py
--rwxrwxrwx  2.0 unx     5374 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/model.py
--rwxrwxrwx  2.0 unx     5339 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/om.py
--rwxrwxrwx  2.0 unx      750 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/backend/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/infer_analyser/
--rwxrwxrwx  2.0 unx      762 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_infer.py
--rwxrwxrwx  2.0 unx     1835 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/install.sh
--rwxrwxrwx  2.0 unx    51061 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/README.md
--rwxrwxrwx  2.0 unx       26 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/requirements.txt
--rwxrwxrwx  2.0 unx     1769 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/benchmark/setup.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/benchmark/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/
--rwxrwxrwx  2.0 unx     2426 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/benchmark/ais_bench/install.sh
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/__init__.py
--rwxrwxrwx  2.0 unx     1763 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/benchmark/ais_bench/__install__.py
--rwxrwxrwx  2.0 unx      752 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/
--rwxrwxrwx  2.0 unx     2685 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/interface.py
--rwxrwxrwx  2.0 unx      759 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/log.py
--rwxrwxrwx  2.0 unx     1591 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/README.md
--rwxrwxrwx  2.0 unx     2433 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/recorder.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/__init__.py
--rwxrwxrwx  2.0 unx     3142 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
--rwxrwxrwx  2.0 unx     4606 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
--rwxrwxrwx  2.0 unx     1375 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
--rwxrwxrwx  2.0 unx     2196 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/download.sh
--rwxrwxrwx  2.0 unx     3978 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
--rwxrwxrwx  2.0 unx     4244 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/__init__.py
--rwxrwxrwx  2.0 unx     2999 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement.py
--rwxrwxrwx  2.0 unx     1260 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/
--rwxrwxrwx  2.0 unx     4614 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_adapter.py
--rwxrwxrwx  2.0 unx     7151 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_check.py
--rwxrwxrwx  2.0 unx    31048 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/benchmark_process.py
--rwxrwxrwx  2.0 unx    37710 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/interface.py
--rwxrwxrwx  2.0 unx    14389 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/io_oprations.py
--rwxrwxrwx  2.0 unx    10701 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/main_cli.py
--rwxrwxrwx  2.0 unx    10444 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/miscellaneous.py
--rwxrwxrwx  2.0 unx    12012 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/path_security_check.py
--rwxrwxrwx  2.0 unx     3260 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/registry.py
--rwxrwxrwx  2.0 unx     9472 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/summary.py
--rwxrwxrwx  2.0 unx    10122 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__init__.py
--rwxrwxrwx  2.0 unx     8700 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__main__.py
--rwxrwxrwx  2.0 unx     3025 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend.py
--rwxrwxrwx  2.0 unx     5400 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
--rwxrwxrwx  2.0 unx      960 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/__init__.py
--rwxrwxrwx  2.0 unx     1623 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/benchmark/backend/install.sh
--rwxrwxrwx  2.0 unx     6911 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/backend/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/backend/__init__.py
--rwxrwxrwx  2.0 unx     2843 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/infer_analyser/analyser.py
--rwxrwxrwx  2.0 unx     8588 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/infer_analyser/infer_analyser.sh
--rwxrwxrwx  2.0 unx     1680 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/infer_analyser/info_convert_json.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/benchmark/infer_analyser/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/
--rwxrwxrwx  2.0 unx     1520 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/build.sh
--rwxrwxrwx  2.0 unx     3162 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/README.md
--rwxrwxrwx  2.0 unx       43 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/convert/requirements.txt
--rwxrwxrwx  2.0 unx     2167 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/setup.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/aie/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/aoe/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/atc/
--rwxrwxrwx  2.0 unx     3463 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/cmd_utils.py
--rwxrwxrwx  2.0 unx     1520 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/model_convert/install.sh
--rwxrwxrwx  2.0 unx      590 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/__init__.py
--rwxrwxrwx  2.0 unx     1382 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/model_convert/__install__.py
--rwxrwxrwx  2.0 unx     3982 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/convert/model_convert/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/convert/model_convert/aie/core/
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/__init__.py
--rwxrwxrwx  2.0 unx      775 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/config.py
--rwxrwxrwx  2.0 unx      646 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/__init__.py
--rwxrwxrwx  2.0 unx     2221 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/core/convert.py
--rwxrwxrwx  2.0 unx      591 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aie/core/__init__.py
--rwxrwxrwx  2.0 unx     9218 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aoe/aoe_args_map.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/aoe/__init__.py
--rwxrwxrwx  2.0 unx    12775 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/atc/atc_args_map.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/convert/model_convert/atc/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/
--rwxrwxrwx  2.0 unx      787 b- defN 24-May-08 11:39 ms-ait-7.0.0b430/components/debug/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/
--rwxrwxrwx  2.0 unx     5324 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/main.py
--rwxrwxrwx  2.0 unx    11876 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/README.md
--rwxrwxrwx  2.0 unx      160 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/requirements.txt
--rwxrwxrwx  2.0 unx     2317 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/
--rwxrwxrwx  2.0 unx    24580 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/cmp_process.py
--rwxrwxrwx  2.0 unx     2181 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/install.sh
--rwxrwxrwx  2.0 unx     5359 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
--rwxrwxrwx  2.0 unx     5175 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf_debug_runner.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__init__.py
--rwxrwxrwx  2.0 unx     1716 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__install__.py
--rwxrwxrwx  2.0 unx     7990 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__main__.py
--rwxrwxrwx  2.0 unx     5723 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
--rwxrwxrwx  2.0 unx     2293 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/__init__.py
--rwxrwxrwx  2.0 unx     3526 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/atc_utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/__init__.py
--rwxrwxrwx  2.0 unx     5651 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/__init__.py
--rwxrwxrwx  2.0 unx     8737 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/args_check.py
--rwxrwxrwx  2.0 unx     3621 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/convert.py
--rwxrwxrwx  2.0 unx     4757 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dump_data.py
--rwxrwxrwx  2.0 unx     1309 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
--rwxrwxrwx  2.0 unx     6098 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/tf_common.py
--rwxrwxrwx  2.0 unx    23475 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/__init__.py
--rwxrwxrwx  2.0 unx    11004 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/analyser.py
--rwxrwxrwx  2.0 unx    15491 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/net_compare.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/__init__.py
--rwxrwxrwx  2.0 unx    26647 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/npu_dump_data.py
--rwxrwxrwx  2.0 unx    17174 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/om_parser.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/__init__.py
--rwxrwxrwx  2.0 unx     9202 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/custom_op.py
--rwxrwxrwx  2.0 unx    15327 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/__init__.py
--rwxrwxrwx  2.0 unx      619 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/__init__.py
--rwxrwxrwx  2.0 unx     7707 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/single_op.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/__init__.py
--rwxrwxrwx  2.0 unx    13711 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/tf_dump_data.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/
--rwxrwxrwx  2.0 unx    11087 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/README.md
--rwxrwxrwx  2.0 unx      140 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/requirements.txt
--rwxrwxrwx  2.0 unx     2811 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/surgeon/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/
--rwxrwxrwx  2.0 unx    15282 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/ait_main.py
--rwxrwxrwx  2.0 unx     5587 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/options.py
--rwxrwxrwx  2.0 unx      878 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__init__.py
--rwxrwxrwx  2.0 unx     1160 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__install__.py
--rwxrwxrwx  2.0 unx     6305 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__main__.py
--rwxrwxrwx  2.0 unx     6012 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/args_check.py
--rwxrwxrwx  2.0 unx     8574 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/click_utils.py
--rwxrwxrwx  2.0 unx     2307 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/config.py
--rwxrwxrwx  2.0 unx     1633 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/log.py
--rwxrwxrwx  2.0 unx     2265 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/register.py
--rwxrwxrwx  2.0 unx      880 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/singleton.py
--rwxrwxrwx  2.0 unx     5111 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/utils.py
--rwxrwxrwx  2.0 unx     1032 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/__init__.py
--rwxrwxrwx  2.0 unx    11302 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
--rwxrwxrwx  2.0 unx       85 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
--rwxrwxrwx  2.0 unx     2102 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
--rwxrwxrwx  2.0 unx      784 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
--rwxrwxrwx  2.0 unx    28389 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
--rwxrwxrwx  2.0 unx     8101 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
--rwxrwxrwx  2.0 unx      755 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
--rwxrwxrwx  2.0 unx    28573 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
--rwxrwxrwx  2.0 unx     4880 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
--rwxrwxrwx  2.0 unx      747 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
--rwxrwxrwx  2.0 unx     4582 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
--rwxrwxrwx  2.0 unx     5214 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/README.md
--rwxrwxrwx  2.0 unx     1024 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
--rwxrwxrwx  2.0 unx      736 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
--rwxrwxrwx  2.0 unx     1694 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
--rwxrwxrwx  2.0 unx     2074 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
--rwxrwxrwx  2.0 unx     1390 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
--rwxrwxrwx  2.0 unx     4242 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
--rwxrwxrwx  2.0 unx     1556 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
--rwxrwxrwx  2.0 unx     2736 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
--rwxrwxrwx  2.0 unx      719 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
--rwxrwxrwx  2.0 unx     2234 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
--rwxrwxrwx  2.0 unx      679 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
--rwxrwxrwx  2.0 unx     1342 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
--rwxrwxrwx  2.0 unx     1404 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
--rwxrwxrwx  2.0 unx     1387 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
--rwxrwxrwx  2.0 unx     5279 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/
--rwxrwxrwx  2.0 unx     1565 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
--rwxrwxrwx  2.0 unx    15557 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/matcher.py
--rwxrwxrwx  2.0 unx     7709 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/pattern.py
--rwxrwxrwx  2.0 unx     6596 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/utils.py
--rwxrwxrwx  2.0 unx     2028 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
--rwxrwxrwx  2.0 unx     5589 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
--rwxrwxrwx  2.0 unx     7914 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
--rwxrwxrwx  2.0 unx     6563 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
--rwxrwxrwx  2.0 unx     6124 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
--rwxrwxrwx  2.0 unx    12418 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
--rwxrwxrwx  2.0 unx     5534 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
--rwxrwxrwx  2.0 unx    11185 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
--rwxrwxrwx  2.0 unx    10165 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
--rwxrwxrwx  2.0 unx     6285 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
--rwxrwxrwx  2.0 unx     7235 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
--rwxrwxrwx  2.0 unx     6958 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
--rwxrwxrwx  2.0 unx     3107 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
--rwxrwxrwx  2.0 unx    10959 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
--rwxrwxrwx  2.0 unx    19159 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
--rwxrwxrwx  2.0 unx     5350 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
--rwxrwxrwx  2.0 unx     8097 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
--rwxrwxrwx  2.0 unx    25805 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
--rwxrwxrwx  2.0 unx     1665 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
--rwxrwxrwx  2.0 unx    16842 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
--rwxrwxrwx  2.0 unx     5031 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
--rwxrwxrwx  2.0 unx    13241 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
--rwxrwxrwx  2.0 unx     8003 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
--rwxrwxrwx  2.0 unx     6050 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/inference.py
--rwxrwxrwx  2.0 unx     1559 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/log.py
--rwxrwxrwx  2.0 unx      505 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/README.md
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/
--rwxrwxrwx  2.0 unx    10044 b- defN 24-May-08 11:27 ms-ait-7.0.0b430/components/llm/README.md
--rwxrwxrwx  2.0 unx      108 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/requirements.txt
--rwxrwxrwx  2.0 unx     2370 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/llm/setup.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/llm/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/compare/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/dump/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/metrics/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/transform/
--rwxrwxrwx  2.0 unx      903 b- defN 24-May-09 18:08 ms-ait-7.0.0b430/components/llm/ait_llm/install.sh
--rwxrwxrwx  2.0 unx      920 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/__init__.py
--rwxrwxrwx  2.0 unx     1792 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/llm/ait_llm/__install__.py
--rwxrwxrwx  2.0 unx    14898 b- defN 24-May-09 19:39 ms-ait-7.0.0b430/components/llm/ait_llm/__main__.py
--rwxrwxrwx  2.0 unx     2609 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/constant.py
--rwxrwxrwx  2.0 unx     4826 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/json_fitter.py
--rwxrwxrwx  2.0 unx     1581 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/log.py
--rwxrwxrwx  2.0 unx     3267 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/tool.py
--rwxrwxrwx  2.0 unx     4657 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/utils.py
--rwxrwxrwx  2.0 unx     8522 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/common/validate.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/common/__init__.py
--rwxrwxrwx  2.0 unx    22815 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/compare/atb_acc_cmp.py
--rwxrwxrwx  2.0 unx     5949 b- defN 24-May-09 19:39 ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_algorithm.py
--rwxrwxrwx  2.0 unx     8511 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_utils.py
--rwxrwxrwx  2.0 unx      957 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/compare/op_mapping.py
--rwxrwxrwx  2.0 unx    19113 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/compare/torchair_acc_cmp.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/compare/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/
--rwxrwxrwx  2.0 unx     8268 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/initial.py
--rwxrwxrwx  2.0 unx     2576 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/manual_dump.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/__init__.py
--rwxrwxrwx  2.0 unx     2445 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
--rwxrwxrwx  2.0 unx       91 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/__init__.py
--rwxrwxrwx  2.0 unx     3413 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_config.py
--rwxrwxrwx  2.0 unx     7648 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_hook.py
--rwxrwxrwx  2.0 unx     1647 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook.py
--rwxrwxrwx  2.0 unx     3067 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook_ops.py
--rwxrwxrwx  2.0 unx     7174 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/topo.py
--rwxrwxrwx  2.0 unx      722 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/__init__.py
--rwxrwxrwx  2.0 unx     4755 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/process.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/__init__.py
--rwxrwxrwx  2.0 unx     5241 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/metrics/case_filter.py
--rwxrwxrwx  2.0 unx    10300 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/metrics/metrics.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/metrics/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/
--rwxrwxrwx  2.0 unx     1645 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/case_manager.py
--rwxrwxrwx  2.0 unx    15421 b- defN 24-May-09 19:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/opchecker.py
--rwxrwxrwx  2.0 unx    11806 b- defN 24-May-09 19:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/operation_test.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/__init__.py
--rwxrwxrwx  2.0 unx     3879 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/build.sh
--rwxrwxrwx  2.0 unx      938 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/CMakeLists.txt
--rwxrwxrwx  2.0 unx    29744 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
--rwxrwxrwx  2.0 unx     1354 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/__init__.py
--rwxrwxrwx  2.0 unx     4577 b- defN 24-May-13 12:29 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/activation.py
--rwxrwxrwx  2.0 unx      925 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_gather.py
--rwxrwxrwx  2.0 unx     3251 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_reduce.py
--rwxrwxrwx  2.0 unx     1469 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/as_strided.py
--rwxrwxrwx  2.0 unx     1286 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/broadcast.py
--rwxrwxrwx  2.0 unx     1319 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/concat.py
--rwxrwxrwx  2.0 unx     1197 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/cumsum.py
--rwxrwxrwx  2.0 unx     5721 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/elewise.py
--rwxrwxrwx  2.0 unx     1783 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
--rwxrwxrwx  2.0 unx     1975 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
--rwxrwxrwx  2.0 unx     1592 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fill.py
--rwxrwxrwx  2.0 unx     2707 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/gather.py
--rwxrwxrwx  2.0 unx     1453 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
--rwxrwxrwx  2.0 unx     1274 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/kv_cache.py
--rwxrwxrwx  2.0 unx     4084 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/layer_norm.py
--rwxrwxrwx  2.0 unx     2687 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear.py
--rwxrwxrwx  2.0 unx     1165 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
--rwxrwxrwx  2.0 unx     2838 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
--rwxrwxrwx  2.0 unx     2631 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/matmul.py
--rwxrwxrwx  2.0 unx     1903 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/multinomial.py
--rwxrwxrwx  2.0 unx     1307 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/pad.py
--rwxrwxrwx  2.0 unx     1247 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/paged_attention.py
--rwxrwxrwx  2.0 unx     1372 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reduce.py
--rwxrwxrwx  2.0 unx     1210 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/repeat.py
--rwxrwxrwx  2.0 unx     1283 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
--rwxrwxrwx  2.0 unx     3504 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rms_norm.py
--rwxrwxrwx  2.0 unx     6893 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope.py
--rwxrwxrwx  2.0 unx     1942 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope_grad.py
--rwxrwxrwx  2.0 unx     9533 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/self_attention.py
--rwxrwxrwx  2.0 unx     1434 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/set_value.py
--rwxrwxrwx  2.0 unx     2261 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/slice.py
--rwxrwxrwx  2.0 unx     1222 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/softmax.py
--rwxrwxrwx  2.0 unx     1233 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/sort.py
--rwxrwxrwx  2.0 unx     1368 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/split.py
--rwxrwxrwx  2.0 unx     3198 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
--rwxrwxrwx  2.0 unx     2677 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
--rwxrwxrwx  2.0 unx     4783 b- defN 24-May-13 12:29 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transdata.py
--rwxrwxrwx  2.0 unx     1196 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transpose.py
--rwxrwxrwx  2.0 unx     2143 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/unpad.py
--rwxrwxrwx  2.0 unx      935 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/where.py
--rwxrwxrwx  2.0 unx     5680 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/__init__.py
--rwxrwxrwx  2.0 unx    12784 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant.py
--rwxrwxrwx  2.0 unx    22320 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
--rwxrwxrwx  2.0 unx     2542 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/transform/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/llm/ait_llm/transform/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/profile/msprof/
--rwxrwxrwx  2.0 unx      602 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/profile/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:34 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/
--rwxrwxrwx  2.0 unx     1835 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/install.sh
--rwxrwxrwx  2.0 unx     5011 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/README.md
--rwxrwxrwx  2.0 unx       10 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/requirements.txt
--rwxrwxrwx  2.0 unx     1581 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/profile/msprof/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/profile/msprof/__init__.py
--rwxrwxrwx  2.0 unx     4154 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/api.py
--rwxrwxrwx  2.0 unx     1277 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/args_adapter.py
--rwxrwxrwx  2.0 unx     4565 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/main_cli.py
--rwxrwxrwx  2.0 unx     4314 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/msprof_process.py
--rwxrwxrwx  2.0 unx      760 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__init__.py
--rwxrwxrwx  2.0 unx      694 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__install__.py
--rwxrwxrwx  2.0 unx     4513 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__main__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/
--rwxrwxrwx  2.0 unx       14 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/requirements.txt
--rwxrwxrwx  2.0 unx     1615 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/setup.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/__init__.py
--rwxrwxrwx  2.0 unx     2261 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/atb.py
--rwxrwxrwx  2.0 unx     2240 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/handler.py
--rwxrwxrwx  2.0 unx     1035 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/logger.py
--rwxrwxrwx  2.0 unx     3438 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/main_cli.py
--rwxrwxrwx  2.0 unx     3921 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/operation.py
--rwxrwxrwx  2.0 unx      874 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/print_stat.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__init__.py
--rwxrwxrwx  2.0 unx      702 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__install__.py
--rwxrwxrwx  2.0 unx     3123 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/tests/test_ait.sh
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/tests/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/
--rwxrwxrwx  2.0 unx    10875 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/install.bat
--rwxrwxrwx  2.0 unx     4111 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/install.sh
--rwxrwxrwx  2.0 unx    23645 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/README.md
--rwxrwxrwx  2.0 unx       94 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/requirements.txt
--rwxrwxrwx  2.0 unx     2329 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/setup.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/common/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/exception/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/model/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/report/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/solution/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/
--rwxrwxrwx  2.0 unx    10875 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/app_analyze/install.bat
--rwxrwxrwx  2.0 unx     4481 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/transplt/app_analyze/install.sh
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/__init__.py
--rwxrwxrwx  2.0 unx     2441 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/app_analyze/__install__.py
--rwxrwxrwx  2.0 unx     3444 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/__main__.py
--rwxrwxrwx  2.0 unx    11196 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/common/kit_config.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/common/__init__.py
--rwxrwxrwx  2.0 unx     2257 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/exception/exception_information.py
--rwxrwxrwx  2.0 unx     3419 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/exception/source_scan_exception.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/exception/__init__.py
--rwxrwxrwx  2.0 unx     4850 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/model/model.py
--rwxrwxrwx  2.0 unx     6911 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/model/project.py
--rwxrwxrwx  2.0 unx     3765 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/model/seq_project.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/model/__init__.py
--rwxrwxrwx  2.0 unx      983 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/app.py
--rwxrwxrwx  2.0 unx     5752 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/cmdline_input.py
--rwxrwxrwx  2.0 unx     1686 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/custom_input.py
--rwxrwxrwx  2.0 unx     1467 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/input_factory.py
--rwxrwxrwx  2.0 unx     2601 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/porting_input.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/porting/__init__.py
--rwxrwxrwx  2.0 unx     1760 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/csv_report.py
--rwxrwxrwx  2.0 unx     1775 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/json_report.py
--rwxrwxrwx  2.0 unx     2202 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/report.py
--rwxrwxrwx  2.0 unx     1814 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/report_factory.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/report/__init__.py
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/
-drwxrwxrwx  2.0 unx        0 b- stor 24-May-13 12:35 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/
--rwxrwxrwx  2.0 unx    16004 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_parser.py
--rwxrwxrwx  2.0 unx    25628 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_utils.py
--rwxrwxrwx  2.0 unx    12287 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cmake_scanner.py
--rwxrwxrwx  2.0 unx     1750 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cxx_scanner.py
--rwxrwxrwx  2.0 unx     3043 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/func_parser.py
--rwxrwxrwx  2.0 unx     7174 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_parser.py
--rwxrwxrwx  2.0 unx     1464 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_scanner.py
--rwxrwxrwx  2.0 unx     1048 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner.py
--rwxrwxrwx  2.0 unx     1930 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_factory.py
--rwxrwxrwx  2.0 unx     1381 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_utils.py
--rwxrwxrwx  2.0 unx     6416 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scan_api.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/__init__.py
--rwxrwxrwx  2.0 unx     5839 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/comment_delete.py
--rwxrwxrwx  2.0 unx     6934 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/file_matrix.py
--rwxrwxrwx  2.0 unx      596 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/__init__.py
--rwxrwxrwx  2.0 unx     4525 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/acc_libs.py
--rwxrwxrwx  2.0 unx     1940 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/api_filter.py
--rwxrwxrwx  2.0 unx    10552 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/ast_visitor.py
--rwxrwxrwx  2.0 unx     5793 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_desc.py
--rwxrwxrwx  2.0 unx     8617 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_handler.py
--rwxrwxrwx  2.0 unx     4199 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_matcher.py
--rwxrwxrwx  2.0 unx     5428 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_utils.py
--rwxrwxrwx  2.0 unx        0 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/__init__.py
--rwxrwxrwx  2.0 unx     6677 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/solution/advisor.py
--rwxrwxrwx  2.0 unx     6732 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/solution/seq_advisor.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/solution/__init__.py
--rwxrwxrwx  2.0 unx     4986 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/clang_finder.py
--rwxrwxrwx  2.0 unx     3503 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/excel.py
--rwxrwxrwx  2.0 unx     1919 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/file_locker.py
--rwxrwxrwx  2.0 unx     2685 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/io_util.py
--rwxrwxrwx  2.0 unx     1970 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/lib_util.py
--rwxrwxrwx  2.0 unx     2638 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/log_util.py
--rwxrwxrwx  2.0 unx     1851 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/security.py
--rwxrwxrwx  2.0 unx      597 b- defN 24-May-08 10:37 ms-ait-7.0.0b430/components/transplt/app_analyze/utils/__init__.py
--rwxrwxrwx  2.0 unx    12215 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/utils/file_open_check.py
--rwxrwxrwx  2.0 unx     9893 b- defN 24-May-09 20:12 ms-ait-7.0.0b430/components/utils/install.py
--rwxrwxrwx  2.0 unx     4690 b- defN 24-May-08 11:39 ms-ait-7.0.0b430/components/utils/parser.py
--rwxrwxrwx  2.0 unx     8721 b- defN 24-May-08 10:39 ms-ait-7.0.0b430/components/utils/security_check.py
--rwxrwxrwx  2.0 unx      886 b- defN 24-May-08 11:39 ms-ait-7.0.0b430/components/utils/util.py
--rwxrwxrwx  2.0 unx      598 b- defN 24-May-09 14:03 ms-ait-7.0.0b430/components/utils/__init__.py
--rwxrwxrwx  2.0 unx        1 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      147 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/entry_points.txt
--rwxrwxrwx  2.0 unx      228 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/PKG-INFO
--rwxrwxrwx  2.0 unx    23938 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/SOURCES.txt
--rwxrwxrwx  2.0 unx       11 b- defN 24-May-13 12:34 ms-ait-7.0.0b430/ms_ait.egg-info/top_level.txt
-546 files, 1866056 bytes uncompressed, 575030 bytes compressed:  69.2%
+Zip file size: 662349 bytes, number of entries: 527
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/
+-rwxrwxrwx  2.0 unx      227 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/PKG-INFO
+-rwxrwxrwx  2.0 unx     4239 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/README.md
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/requirements.txt
+-rwxrwxrwx  2.0 unx       38 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/setup.cfg
+-rwxrwxrwx  2.0 unx     1714 b- defN 24-Apr-29 22:45 ms-ait-7.0.0rc2/setup.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/profile/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/tests/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/utils/
+-rwxrwxrwx  2.0 unx      600 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/__init__.py
+-rwxrwxrwx  2.0 unx     2929 b- defN 24-Apr-29 22:24 ms-ait-7.0.0rc2/components/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/
+-rwxrwxrwx  2.0 unx     5220 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/README.md
+-rwxrwxrwx  2.0 unx       65 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/requirements.txt
+-rwxrwxrwx  2.0 unx     2199 b- defN 24-Apr-29 22:23 ms-ait-7.0.0rc2/components/analyze/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-29 10:42 ms-ait-7.0.0rc2/components/analyze/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/__init__.py
+-rwxrwxrwx  2.0 unx      100 b- defN 24-Apr-29 21:54 ms-ait-7.0.0rc2/components/analyze/model_evaluation/__install__.py
+-rwxrwxrwx  2.0 unx     5943 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/analyze/model_evaluation/__main__.py
+-rwxrwxrwx  2.0 unx      843 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/config.py
+-rwxrwxrwx  2.0 unx      936 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/op_info.py
+-rwxrwxrwx  2.0 unx      712 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/
+-rwxrwxrwx  2.0 unx      882 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/const.py
+-rwxrwxrwx  2.0 unx     1078 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/log.py
+-rwxrwxrwx  2.0 unx     1917 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/utils.py
+-rwxrwxrwx  2.0 unx       95 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/__init__.py
+-rwxrwxrwx  2.0 unx     1072 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/atc_err.py
+-rwxrwxrwx  2.0 unx      730 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/engine.py
+-rwxrwxrwx  2.0 unx      712 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/framework.py
+-rwxrwxrwx  2.0 unx      852 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
+-rwxrwxrwx  2.0 unx      692 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/soc_type.py
+-rwxrwxrwx  2.0 unx      305 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/
+-rwxrwxrwx  2.0 unx     7722 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/analysis.py
+-rwxrwxrwx  2.0 unx     4707 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/result.py
+-rwxrwxrwx  2.0 unx     1236 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/rule.py
+-rwxrwxrwx  2.0 unx       51 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/__init__.py
+-rwxrwxrwx  2.0 unx     2495 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/onnx.py
+-rwxrwxrwx  2.0 unx       59 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/__init__.py
+-rwxrwxrwx  2.0 unx     4428 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/opp.py
+-rwxrwxrwx  2.0 unx     2212 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/op_map.py
+-rwxrwxrwx  2.0 unx      683 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/__init__.py
+-rwxrwxrwx  2.0 unx     2210 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/onnx.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/__init__.py
+-rwxrwxrwx  2.0 unx     4426 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/atc.py
+-rwxrwxrwx  2.0 unx     5374 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/model.py
+-rwxrwxrwx  2.0 unx     5339 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/om.py
+-rwxrwxrwx  2.0 unx      750 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/backend/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/infer_analyser/
+-rwxrwxrwx  2.0 unx      762 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_infer.py
+-rwxrwxrwx  2.0 unx     1835 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/install.sh
+-rwxrwxrwx  2.0 unx    51061 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/README.md
+-rwxrwxrwx  2.0 unx       26 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/requirements.txt
+-rwxrwxrwx  2.0 unx     1779 b- defN 24-Apr-29 21:35 ms-ait-7.0.0rc2/components/benchmark/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-29 11:18 ms-ait-7.0.0rc2/components/benchmark/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/
+-rwxrwxrwx  2.0 unx     1820 b- defN 24-Apr-29 21:41 ms-ait-7.0.0rc2/components/benchmark/ais_bench/install.sh
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/__init__.py
+-rwxrwxrwx  2.0 unx      730 b- defN 24-Apr-29 21:32 ms-ait-7.0.0rc2/components/benchmark/ais_bench/__install__.py
+-rwxrwxrwx  2.0 unx      752 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/
+-rwxrwxrwx  2.0 unx     2685 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/interface.py
+-rwxrwxrwx  2.0 unx      759 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/log.py
+-rwxrwxrwx  2.0 unx     1591 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/README.md
+-rwxrwxrwx  2.0 unx     2433 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/recorder.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/__init__.py
+-rwxrwxrwx  2.0 unx     3142 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
+-rwxrwxrwx  2.0 unx     4606 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
+-rwxrwxrwx  2.0 unx     1375 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
+-rwxrwxrwx  2.0 unx     3978 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
+-rwxrwxrwx  2.0 unx     4244 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/__init__.py
+-rwxrwxrwx  2.0 unx     2999 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement.py
+-rwxrwxrwx  2.0 unx     1260 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/
+-rwxrwxrwx  2.0 unx     4614 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_adapter.py
+-rwxrwxrwx  2.0 unx     7151 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_check.py
+-rwxrwxrwx  2.0 unx    31048 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/benchmark_process.py
+-rwxrwxrwx  2.0 unx    37710 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/interface.py
+-rwxrwxrwx  2.0 unx    14389 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/io_oprations.py
+-rwxrwxrwx  2.0 unx    10701 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/main_cli.py
+-rwxrwxrwx  2.0 unx    10444 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/miscellaneous.py
+-rwxrwxrwx  2.0 unx    12042 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/path_security_check.py
+-rwxrwxrwx  2.0 unx     3260 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/registry.py
+-rwxrwxrwx  2.0 unx     9472 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/summary.py
+-rwxrwxrwx  2.0 unx    10122 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__init__.py
+-rwxrwxrwx  2.0 unx     8700 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__main__.py
+-rwxrwxrwx  2.0 unx     3025 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend.py
+-rwxrwxrwx  2.0 unx     5400 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
+-rwxrwxrwx  2.0 unx      960 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/__init__.py
+-rwxrwxrwx  2.0 unx     1587 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/backend/install.sh
+-rwxrwxrwx  2.0 unx     6911 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/backend/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/backend/__init__.py
+-rwxrwxrwx  2.0 unx     2843 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/infer_analyser/analyser.py
+-rwxrwxrwx  2.0 unx     1680 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/infer_analyser/info_convert_json.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/benchmark/infer_analyser/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/
+-rwxrwxrwx  2.0 unx     3162 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/README.md
+-rwxrwxrwx  2.0 unx       35 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/requirements.txt
+-rwxrwxrwx  2.0 unx     2141 b- defN 24-Apr-29 22:23 ms-ait-7.0.0rc2/components/convert/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-29 10:53 ms-ait-7.0.0rc2/components/convert/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/aie/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/aoe/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/atc/
+-rwxrwxrwx  2.0 unx     3463 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/cmd_utils.py
+-rwxrwxrwx  2.0 unx     1520 b- defN 24-Apr-29 21:57 ms-ait-7.0.0rc2/components/convert/model_convert/install.sh
+-rwxrwxrwx  2.0 unx      590 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/__init__.py
+-rwxrwxrwx  2.0 unx      767 b- defN 24-Apr-29 22:43 ms-ait-7.0.0rc2/components/convert/model_convert/__install__.py
+-rwxrwxrwx  2.0 unx     3982 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/convert/model_convert/__main__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/__init__.py
+-rwxrwxrwx  2.0 unx      775 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/config.py
+-rwxrwxrwx  2.0 unx      646 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/__init__.py
+-rwxrwxrwx  2.0 unx     2221 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/convert.py
+-rwxrwxrwx  2.0 unx      591 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/__init__.py
+-rwxrwxrwx  2.0 unx     9218 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aoe/aoe_args_map.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/aoe/__init__.py
+-rwxrwxrwx  2.0 unx    12775 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/atc/atc_args_map.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/convert/model_convert/atc/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/
+-rwxrwxrwx  2.0 unx      787 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/debug/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/
+-rwxrwxrwx  2.0 unx     5324 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/main.py
+-rwxrwxrwx  2.0 unx    11876 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/README.md
+-rwxrwxrwx  2.0 unx      160 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/requirements.txt
+-rwxrwxrwx  2.0 unx     2291 b- defN 24-Apr-29 22:20 ms-ait-7.0.0rc2/components/debug/compare/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-29 20:05 ms-ait-7.0.0rc2/components/debug/compare/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/
+-rwxrwxrwx  2.0 unx    24580 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/cmp_process.py
+-rwxrwxrwx  2.0 unx     2181 b- defN 24-Apr-29 21:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/install.sh
+-rwxrwxrwx  2.0 unx     5359 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
+-rwxrwxrwx  2.0 unx     5175 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf_debug_runner.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__init__.py
+-rwxrwxrwx  2.0 unx     1110 b- defN 24-Apr-29 20:25 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__install__.py
+-rwxrwxrwx  2.0 unx     7990 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__main__.py
+-rwxrwxrwx  2.0 unx     5723 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
+-rwxrwxrwx  2.0 unx     2293 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/__init__.py
+-rwxrwxrwx  2.0 unx     3526 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/atc_utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/__init__.py
+-rwxrwxrwx  2.0 unx     5651 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/__init__.py
+-rwxrwxrwx  2.0 unx     8737 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/args_check.py
+-rwxrwxrwx  2.0 unx     3621 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/convert.py
+-rwxrwxrwx  2.0 unx     4757 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dump_data.py
+-rwxrwxrwx  2.0 unx     1309 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
+-rwxrwxrwx  2.0 unx     6098 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/tf_common.py
+-rwxrwxrwx  2.0 unx    23392 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/__init__.py
+-rwxrwxrwx  2.0 unx    11004 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/analyser.py
+-rwxrwxrwx  2.0 unx    15491 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/net_compare.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/__init__.py
+-rwxrwxrwx  2.0 unx    26609 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/npu_dump_data.py
+-rwxrwxrwx  2.0 unx    14614 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/om_parser.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/__init__.py
+-rwxrwxrwx  2.0 unx     9202 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/custom_op.py
+-rwxrwxrwx  2.0 unx    15216 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/__init__.py
+-rwxrwxrwx  2.0 unx      619 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-29 20:42 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/__init__.py
+-rwxrwxrwx  2.0 unx     7707 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/single_op.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/__init__.py
+-rwxrwxrwx  2.0 unx    13711 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/tf_dump_data.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/
+-rwxrwxrwx  2.0 unx    11087 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/README.md
+-rwxrwxrwx  2.0 unx      140 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/requirements.txt
+-rwxrwxrwx  2.0 unx     2785 b- defN 24-Apr-29 22:26 ms-ait-7.0.0rc2/components/debug/surgeon/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/
+-rwxrwxrwx  2.0 unx    15282 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/ait_main.py
+-rwxrwxrwx  2.0 unx     5587 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/options.py
+-rwxrwxrwx  2.0 unx      878 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__init__.py
+-rwxrwxrwx  2.0 unx      587 b- defN 24-Apr-29 22:43 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__install__.py
+-rwxrwxrwx  2.0 unx     6305 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__main__.py
+-rwxrwxrwx  2.0 unx     6012 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/args_check.py
+-rwxrwxrwx  2.0 unx     8604 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/click_utils.py
+-rwxrwxrwx  2.0 unx     2307 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/config.py
+-rwxrwxrwx  2.0 unx     1633 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/log.py
+-rwxrwxrwx  2.0 unx     2265 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/register.py
+-rwxrwxrwx  2.0 unx      880 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/singleton.py
+-rwxrwxrwx  2.0 unx     5111 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/utils.py
+-rwxrwxrwx  2.0 unx     1032 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/__init__.py
+-rwxrwxrwx  2.0 unx    11302 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
+-rwxrwxrwx  2.0 unx       85 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
+-rwxrwxrwx  2.0 unx     2102 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
+-rwxrwxrwx  2.0 unx      784 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
+-rwxrwxrwx  2.0 unx    28389 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
+-rwxrwxrwx  2.0 unx     8101 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
+-rwxrwxrwx  2.0 unx      755 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
+-rwxrwxrwx  2.0 unx    28573 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
+-rwxrwxrwx  2.0 unx     4880 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
+-rwxrwxrwx  2.0 unx      747 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
+-rwxrwxrwx  2.0 unx     4582 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
+-rwxrwxrwx  2.0 unx     5214 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/README.md
+-rwxrwxrwx  2.0 unx     1024 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
+-rwxrwxrwx  2.0 unx      736 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
+-rwxrwxrwx  2.0 unx     1694 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
+-rwxrwxrwx  2.0 unx     2074 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
+-rwxrwxrwx  2.0 unx     1390 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
+-rwxrwxrwx  2.0 unx     4242 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
+-rwxrwxrwx  2.0 unx     1556 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
+-rwxrwxrwx  2.0 unx     2736 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
+-rwxrwxrwx  2.0 unx      719 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
+-rwxrwxrwx  2.0 unx     2234 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
+-rwxrwxrwx  2.0 unx      679 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
+-rwxrwxrwx  2.0 unx     1342 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
+-rwxrwxrwx  2.0 unx     1404 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
+-rwxrwxrwx  2.0 unx     1387 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
+-rwxrwxrwx  2.0 unx     5279 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/
+-rwxrwxrwx  2.0 unx     1565 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
+-rwxrwxrwx  2.0 unx    15557 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/matcher.py
+-rwxrwxrwx  2.0 unx     7709 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/pattern.py
+-rwxrwxrwx  2.0 unx     6596 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/utils.py
+-rwxrwxrwx  2.0 unx     2028 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
+-rwxrwxrwx  2.0 unx     5589 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
+-rwxrwxrwx  2.0 unx     7914 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
+-rwxrwxrwx  2.0 unx     6563 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
+-rwxrwxrwx  2.0 unx     6124 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
+-rwxrwxrwx  2.0 unx    12418 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
+-rwxrwxrwx  2.0 unx     5534 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
+-rwxrwxrwx  2.0 unx    11185 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
+-rwxrwxrwx  2.0 unx    10165 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
+-rwxrwxrwx  2.0 unx     6285 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
+-rwxrwxrwx  2.0 unx     7235 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
+-rwxrwxrwx  2.0 unx     6958 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
+-rwxrwxrwx  2.0 unx     3107 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
+-rwxrwxrwx  2.0 unx    10959 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
+-rwxrwxrwx  2.0 unx    19159 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
+-rwxrwxrwx  2.0 unx     5350 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
+-rwxrwxrwx  2.0 unx     8097 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
+-rwxrwxrwx  2.0 unx    25805 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
+-rwxrwxrwx  2.0 unx     1665 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
+-rwxrwxrwx  2.0 unx    16842 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
+-rwxrwxrwx  2.0 unx     5031 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
+-rwxrwxrwx  2.0 unx    13241 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
+-rwxrwxrwx  2.0 unx     8003 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
+-rwxrwxrwx  2.0 unx     6050 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/inference.py
+-rwxrwxrwx  2.0 unx     1559 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/log.py
+-rwxrwxrwx  2.0 unx      505 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/README.md
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/
+-rwxrwxrwx  2.0 unx     9351 b- defN 24-Apr-24 19:12 ms-ait-7.0.0rc2/components/llm/README.md
+-rwxrwxrwx  2.0 unx      108 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/requirements.txt
+-rwxrwxrwx  2.0 unx     2353 b- defN 24-Apr-29 22:23 ms-ait-7.0.0rc2/components/llm/setup.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-29 10:34 ms-ait-7.0.0rc2/components/llm/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/
+-rwxrwxrwx  2.0 unx      904 b- defN 24-Apr-29 22:07 ms-ait-7.0.0rc2/components/llm/ait_llm/install.sh
+-rwxrwxrwx  2.0 unx      920 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/__init__.py
+-rwxrwxrwx  2.0 unx      789 b- defN 24-Apr-29 22:45 ms-ait-7.0.0rc2/components/llm/ait_llm/__install__.py
+-rwxrwxrwx  2.0 unx    13398 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/llm/ait_llm/__main__.py
+-rwxrwxrwx  2.0 unx     2609 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/constant.py
+-rwxrwxrwx  2.0 unx     4826 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/json_fitter.py
+-rwxrwxrwx  2.0 unx     1581 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/log.py
+-rwxrwxrwx  2.0 unx     3267 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/tool.py
+-rwxrwxrwx  2.0 unx     4657 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/utils.py
+-rwxrwxrwx  2.0 unx     8522 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/common/validate.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/common/__init__.py
+-rwxrwxrwx  2.0 unx    22815 b- defN 24-Apr-25 16:27 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/atb_acc_cmp.py
+-rwxrwxrwx  2.0 unx     3429 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_algorithm.py
+-rwxrwxrwx  2.0 unx     8458 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_utils.py
+-rwxrwxrwx  2.0 unx      957 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/op_mapping.py
+-rwxrwxrwx  2.0 unx    19113 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/torchair_acc_cmp.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/compare/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/
+-rwxrwxrwx  2.0 unx     8268 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/initial.py
+-rwxrwxrwx  2.0 unx     2576 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/manual_dump.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/__init__.py
+-rwxrwxrwx  2.0 unx     2445 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
+-rwxrwxrwx  2.0 unx       91 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/__init__.py
+-rwxrwxrwx  2.0 unx     3413 b- defN 24-Apr-24 19:12 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_config.py
+-rwxrwxrwx  2.0 unx     7648 b- defN 24-Apr-25 16:29 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_hook.py
+-rwxrwxrwx  2.0 unx     1647 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook.py
+-rwxrwxrwx  2.0 unx     3067 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook_ops.py
+-rwxrwxrwx  2.0 unx     7174 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/topo.py
+-rwxrwxrwx  2.0 unx      722 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/__init__.py
+-rwxrwxrwx  2.0 unx     4755 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/process.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/__init__.py
+-rwxrwxrwx  2.0 unx     5241 b- defN 24-Apr-25 15:33 ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/case_filter.py
+-rwxrwxrwx  2.0 unx    10031 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/metrics.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-25 14:41 ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/
+-rwxrwxrwx  2.0 unx     1645 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/case_manager.py
+-rwxrwxrwx  2.0 unx    15437 b- defN 24-Apr-25 19:14 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/opchecker.py
+-rwxrwxrwx  2.0 unx    10880 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/operation_test.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/__init__.py
+-rwxrwxrwx  2.0 unx    29744 b- defN 24-Apr-25 19:14 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
+-rwxrwxrwx  2.0 unx     1354 b- defN 24-Apr-25 19:14 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-29 22:29 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/__init__.py
+-rwxrwxrwx  2.0 unx     2904 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/activation.py
+-rwxrwxrwx  2.0 unx      973 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_gather.py
+-rwxrwxrwx  2.0 unx     2970 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_reduce.py
+-rwxrwxrwx  2.0 unx     1061 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/as_strided.py
+-rwxrwxrwx  2.0 unx     1098 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/broadcast.py
+-rwxrwxrwx  2.0 unx     1088 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/concat.py
+-rwxrwxrwx  2.0 unx      967 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/cumsum.py
+-rwxrwxrwx  2.0 unx     5404 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/elewise.py
+-rwxrwxrwx  2.0 unx     1459 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
+-rwxrwxrwx  2.0 unx     2003 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
+-rwxrwxrwx  2.0 unx     1144 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fill.py
+-rwxrwxrwx  2.0 unx     2535 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/gather.py
+-rwxrwxrwx  2.0 unx     1094 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
+-rwxrwxrwx  2.0 unx     1045 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/kv_cache.py
+-rwxrwxrwx  2.0 unx     4446 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/layer_norm.py
+-rwxrwxrwx  2.0 unx     2687 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear.py
+-rwxrwxrwx  2.0 unx     1247 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
+-rwxrwxrwx  2.0 unx     3020 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
+-rwxrwxrwx  2.0 unx     2694 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/matmul.py
+-rwxrwxrwx  2.0 unx     1650 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/multinomial.py
+-rwxrwxrwx  2.0 unx     1440 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/pad.py
+-rwxrwxrwx  2.0 unx     1229 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/paged_attention.py
+-rwxrwxrwx  2.0 unx     1033 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reduce.py
+-rwxrwxrwx  2.0 unx      951 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/repeat.py
+-rwxrwxrwx  2.0 unx     1068 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
+-rwxrwxrwx  2.0 unx     2751 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rms_norm.py
+-rwxrwxrwx  2.0 unx     6620 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope.py
+-rwxrwxrwx  2.0 unx     1725 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope_grad.py
+-rwxrwxrwx  2.0 unx     9619 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/self_attention.py
+-rwxrwxrwx  2.0 unx     1125 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/set_value.py
+-rwxrwxrwx  2.0 unx     1762 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/slice.py
+-rwxrwxrwx  2.0 unx      992 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/softmax.py
+-rwxrwxrwx  2.0 unx     1031 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/sort.py
+-rwxrwxrwx  2.0 unx      994 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/split.py
+-rwxrwxrwx  2.0 unx     3220 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
+-rwxrwxrwx  2.0 unx     2579 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
+-rwxrwxrwx  2.0 unx     4625 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transdata.py
+-rwxrwxrwx  2.0 unx      986 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transpose.py
+-rwxrwxrwx  2.0 unx     2264 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/unpad.py
+-rwxrwxrwx  2.0 unx      972 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/where.py
+-rwxrwxrwx  2.0 unx     5680 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/__init__.py
+-rwxrwxrwx  2.0 unx    12784 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant.py
+-rwxrwxrwx  2.0 unx    22320 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
+-rwxrwxrwx  2.0 unx     2542 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/llm/ait_llm/transform/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/profile/msprof/
+-rwxrwxrwx  2.0 unx      602 b- defN 24-Apr-29 11:18 ms-ait-7.0.0rc2/components/profile/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/
+-rwxrwxrwx  2.0 unx     1835 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/install.sh
+-rwxrwxrwx  2.0 unx     5011 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/README.md
+-rwxrwxrwx  2.0 unx       10 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/requirements.txt
+-rwxrwxrwx  2.0 unx     1552 b- defN 24-Apr-29 22:24 ms-ait-7.0.0rc2/components/profile/msprof/setup.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-29 22:34 ms-ait-7.0.0rc2/components/profile/msprof/__init__.py
+-rwxrwxrwx  2.0 unx     4154 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/api.py
+-rwxrwxrwx  2.0 unx     1277 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/args_adapter.py
+-rwxrwxrwx  2.0 unx     4565 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/main_cli.py
+-rwxrwxrwx  2.0 unx     4314 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/msprof_process.py
+-rwxrwxrwx  2.0 unx      760 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__init__.py
+-rwxrwxrwx  2.0 unx       99 b- defN 24-Apr-29 22:05 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__install__.py
+-rwxrwxrwx  2.0 unx     4513 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__main__.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/tests/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/
+-rwxrwxrwx  2.0 unx    10875 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/install.bat
+-rwxrwxrwx  2.0 unx     4111 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/install.sh
+-rwxrwxrwx  2.0 unx    23645 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/README.md
+-rwxrwxrwx  2.0 unx       89 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/requirements.txt
+-rwxrwxrwx  2.0 unx     2210 b- defN 24-Apr-29 22:38 ms-ait-7.0.0rc2/components/transplt/setup.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-29 10:37 ms-ait-7.0.0rc2/components/transplt/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/common/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/
+-rwxrwxrwx  2.0 unx    10875 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/install.bat
+-rwxrwxrwx  2.0 unx     4111 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/install.sh
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/__init__.py
+-rwxrwxrwx  2.0 unx      839 b- defN 24-Apr-29 22:43 ms-ait-7.0.0rc2/components/transplt/app_analyze/__install__.py
+-rwxrwxrwx  2.0 unx     3444 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/transplt/app_analyze/__main__.py
+-rwxrwxrwx  2.0 unx    11196 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/common/kit_config.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/common/__init__.py
+-rwxrwxrwx  2.0 unx     2257 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/exception_information.py
+-rwxrwxrwx  2.0 unx     3419 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/source_scan_exception.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/__init__.py
+-rwxrwxrwx  2.0 unx     4850 b- defN 24-Apr-29 14:10 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/model.py
+-rwxrwxrwx  2.0 unx     6911 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/project.py
+-rwxrwxrwx  2.0 unx     3765 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/seq_project.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/model/__init__.py
+-rwxrwxrwx  2.0 unx      983 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/app.py
+-rwxrwxrwx  2.0 unx     5752 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/cmdline_input.py
+-rwxrwxrwx  2.0 unx     1686 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/custom_input.py
+-rwxrwxrwx  2.0 unx     1467 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/input_factory.py
+-rwxrwxrwx  2.0 unx     2601 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/porting_input.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/__init__.py
+-rwxrwxrwx  2.0 unx     1760 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/csv_report.py
+-rwxrwxrwx  2.0 unx     1775 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/json_report.py
+-rwxrwxrwx  2.0 unx     2202 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report.py
+-rwxrwxrwx  2.0 unx     1814 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report_factory.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/report/__init__.py
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/
+drwxrwxrwx  2.0 unx        0 b- stor 24-Apr-29 22:46 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/
+-rwxrwxrwx  2.0 unx    16004 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_parser.py
+-rwxrwxrwx  2.0 unx    25628 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_utils.py
+-rwxrwxrwx  2.0 unx    12287 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cmake_scanner.py
+-rwxrwxrwx  2.0 unx     1750 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cxx_scanner.py
+-rwxrwxrwx  2.0 unx     3043 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/func_parser.py
+-rwxrwxrwx  2.0 unx     7174 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_parser.py
+-rwxrwxrwx  2.0 unx     1464 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_scanner.py
+-rwxrwxrwx  2.0 unx     1048 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner.py
+-rwxrwxrwx  2.0 unx     1930 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_factory.py
+-rwxrwxrwx  2.0 unx     1381 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_utils.py
+-rwxrwxrwx  2.0 unx     6416 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scan_api.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/__init__.py
+-rwxrwxrwx  2.0 unx     5839 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/comment_delete.py
+-rwxrwxrwx  2.0 unx     6934 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/file_matrix.py
+-rwxrwxrwx  2.0 unx      596 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/__init__.py
+-rwxrwxrwx  2.0 unx     4525 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/acc_libs.py
+-rwxrwxrwx  2.0 unx     1940 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/api_filter.py
+-rwxrwxrwx  2.0 unx    10552 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/ast_visitor.py
+-rwxrwxrwx  2.0 unx     5793 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_desc.py
+-rwxrwxrwx  2.0 unx     8617 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_handler.py
+-rwxrwxrwx  2.0 unx     4199 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_matcher.py
+-rwxrwxrwx  2.0 unx     5428 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_utils.py
+-rwxrwxrwx  2.0 unx        0 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/__init__.py
+-rwxrwxrwx  2.0 unx     6677 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/advisor.py
+-rwxrwxrwx  2.0 unx     6732 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/seq_advisor.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/__init__.py
+-rwxrwxrwx  2.0 unx     4697 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/clang_finder.py
+-rwxrwxrwx  2.0 unx     3503 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/excel.py
+-rwxrwxrwx  2.0 unx     1919 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/file_locker.py
+-rwxrwxrwx  2.0 unx     2685 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/io_util.py
+-rwxrwxrwx  2.0 unx     1970 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/lib_util.py
+-rwxrwxrwx  2.0 unx     2638 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/log_util.py
+-rwxrwxrwx  2.0 unx     1851 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/security.py
+-rwxrwxrwx  2.0 unx      597 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/__init__.py
+-rwxrwxrwx  2.0 unx    12245 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/utils/file_open_check.py
+-rwxrwxrwx  2.0 unx     4614 b- defN 24-Apr-29 22:32 ms-ait-7.0.0rc2/components/utils/install.py
+-rwxrwxrwx  2.0 unx     3987 b- defN 24-Apr-29 17:07 ms-ait-7.0.0rc2/components/utils/parser.py
+-rwxrwxrwx  2.0 unx     8748 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/utils/security_check.py
+-rwxrwxrwx  2.0 unx      279 b- defN 24-Apr-29 15:52 ms-ait-7.0.0rc2/components/utils/util.py
+-rwxrwxrwx  2.0 unx      599 b- defN 24-Apr-24 18:44 ms-ait-7.0.0rc2/components/utils/__init__.py
+-rwxrwxrwx  2.0 unx        1 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      147 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/entry_points.txt
+-rwxrwxrwx  2.0 unx      227 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/PKG-INFO
+-rwxrwxrwx  2.0 unx    23140 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/SOURCES.txt
+-rwxrwxrwx  2.0 unx       11 b- defN 24-Apr-29 22:46 ms-ait-7.0.0rc2/ms_ait.egg-info/top_level.txt
+527 files, 1797886 bytes uncompressed, 550759 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,1639 +1,1582 @@
-Filename: ms-ait-7.0.0b430/
+Filename: ms-ait-7.0.0rc2/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/
+Filename: ms-ait-7.0.0rc2/components/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/PKG-INFO
+Filename: ms-ait-7.0.0rc2/PKG-INFO
 Comment: 
 
-Filename: ms-ait-7.0.0b430/README.md
+Filename: ms-ait-7.0.0rc2/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/requirements.txt
+Filename: ms-ait-7.0.0rc2/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/setup.cfg
+Filename: ms-ait-7.0.0rc2/setup.cfg
 Comment: 
 
-Filename: ms-ait-7.0.0b430/setup.py
+Filename: ms-ait-7.0.0rc2/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/
+Filename: ms-ait-7.0.0rc2/components/analyze/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/
+Filename: ms-ait-7.0.0rc2/components/benchmark/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/
+Filename: ms-ait-7.0.0rc2/components/convert/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/
+Filename: ms-ait-7.0.0rc2/components/debug/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/
+Filename: ms-ait-7.0.0rc2/components/llm/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/
+Filename: ms-ait-7.0.0rc2/components/profile/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/
+Filename: ms-ait-7.0.0rc2/components/tests/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tests/
+Filename: ms-ait-7.0.0rc2/components/transplt/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/
+Filename: ms-ait-7.0.0rc2/components/utils/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/utils/
+Filename: ms-ait-7.0.0rc2/components/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/__init__.py
+Filename: ms-ait-7.0.0rc2/components/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/__main__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/
+Filename: ms-ait-7.0.0rc2/components/analyze/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/README.md
+Filename: ms-ait-7.0.0rc2/components/analyze/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/analyze/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/setup.py
+Filename: ms-ait-7.0.0rc2/components/analyze/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/data/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/__install__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/__main__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/config.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/op_info.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/op_info.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/const.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/const.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/log.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/utils.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/atc_err.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/atc_err.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/engine.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/engine.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/framework.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/framework.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/onnx_checker_err.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/soc_type.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/soc_type.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/analysis.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/analysis.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/result.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/result.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/rule.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/rule.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/onnx.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/onnx.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/opp.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/data/opp.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/op_map.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/data/op_map.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/data/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/onnx.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/onnx.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/__init__.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/atc.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/atc.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/model.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/model.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/om.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/om.py
+Filename: ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/
+Filename: ms-ait-7.0.0rc2/components/benchmark/backend/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/backend/
+Filename: ms-ait-7.0.0rc2/components/benchmark/infer_analyser/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_infer.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_infer.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/install.sh
+Filename: ms-ait-7.0.0rc2/components/benchmark/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/README.md
+Filename: ms-ait-7.0.0rc2/components/benchmark/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/benchmark/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/setup.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/install.sh
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/__install__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/__main__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/interface.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/interface.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/log.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/README.md
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/recorder.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/recorder.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/download.sh
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_adapter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_adapter.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/benchmark_process.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_check.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/interface.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/benchmark_process.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/io_oprations.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/interface.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/main_cli.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/io_oprations.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/miscellaneous.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/main_cli.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/path_security_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/miscellaneous.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/registry.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/path_security_check.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/summary.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/registry.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/summary.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/utils.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__main__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend_trtexec.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/backend/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/backend/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/backend/install.sh
+Filename: ms-ait-7.0.0rc2/components/benchmark/backend/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/backend/setup.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/infer_analyser/analyser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/backend/__init__.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/infer_analyser/info_convert_json.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/analyser.py
+Filename: ms-ait-7.0.0rc2/components/benchmark/infer_analyser/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/infer_analyser.sh
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/info_convert_json.py
+Filename: ms-ait-7.0.0rc2/components/convert/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/benchmark/infer_analyser/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/
+Filename: ms-ait-7.0.0rc2/components/convert/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/build.sh
+Filename: ms-ait-7.0.0rc2/components/convert/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/README.md
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aoe/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/setup.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/atc/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/cmd_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aoe/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/atc/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/cmd_utils.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/install.sh
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/__install__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/__main__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/core/
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/convert.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/config.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aoe/aoe_args_map.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/aoe/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/core/convert.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/atc/atc_args_map.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aie/core/__init__.py
+Filename: ms-ait-7.0.0rc2/components/convert/model_convert/atc/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aoe/aoe_args_map.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/aoe/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/atc/atc_args_map.py
+Filename: ms-ait-7.0.0rc2/components/debug/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/convert/model_convert/atc/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/main.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/main.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/README.md
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/setup.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/cmp_process.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf_debug_runner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/cmp_process.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/install.sh
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/l1_buffer_data_parser.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf_debug_runner.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__install__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__main__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/atc_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/atc_utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/args_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/convert.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/args_check.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/tf_common.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/convert.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dump_data.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/analyser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/tf_common.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/net_compare.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/npu_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/analyser.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/om_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/net_compare.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/custom_op.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/npu_dump_data.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/om_parser.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/custom_op.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/single_op.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/tf_dump_data.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/single_op.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/tf_dump_data.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/README.md
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/setup.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/ait_main.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/options.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/ait_main.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/options.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/args_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/click_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__install__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__main__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/args_check.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/register.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/click_utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/singleton.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/config.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/log.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/register.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/singleton.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/README.md
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/calibration/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/README.md
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/calibration/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/language/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/speech/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/language/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/speech/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/language/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/speech/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/language/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/speech/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/matcher.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/pattern.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/matcher.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/pattern.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/utils.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/inference.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/__init__.py
+Filename: ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/inference.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/log.py
+Filename: ms-ait-7.0.0rc2/components/llm/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/README.md
+Filename: ms-ait-7.0.0rc2/components/llm/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/
+Filename: ms-ait-7.0.0rc2/components/llm/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/README.md
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/setup.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/metrics/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/install.sh
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/constant.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/json_fitter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/__install__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/log.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/__main__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/tool.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/constant.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/json_fitter.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/validate.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/log.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/tool.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/atb_acc_cmp.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/utils.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_algorithm.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/validate.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/op_mapping.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/atb_acc_cmp.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/torchair_acc_cmp.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_algorithm.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/compare/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_utils.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/op_mapping.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/torchair_acc_cmp.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/initial.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/compare/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/manual_dump.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/initial.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/manual_dump.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_hook.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook_ops.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_config.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/topo.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_hook.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/process.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook_ops.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/topo.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/case_filter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/metrics.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/process.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/metrics/case_filter.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/metrics/metrics.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/case_manager.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/metrics/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/opchecker.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/operation_test.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/case_manager.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/opchecker.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/operation_test.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/activation.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/build.sh
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_gather.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/CMakeLists.txt
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_reduce.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/as_strided.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/broadcast.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/__init__.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/concat.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/activation.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/cumsum.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_gather.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/elewise.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_reduce.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/as_strided.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/broadcast.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fill.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/concat.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/gather.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/cumsum.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/elewise.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/kv_cache.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/layer_norm.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fill.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/gather.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/genattentionmask.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/matmul.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/kv_cache.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/multinomial.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/layer_norm.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/pad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/paged_attention.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_parallel.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reduce.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_sparse.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/repeat.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/matmul.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/multinomial.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rms_norm.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/pad.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/paged_attention.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope_grad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reduce.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/self_attention.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/repeat.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/set_value.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/slice.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rms_norm.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/softmax.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/sort.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope_grad.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/split.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/self_attention.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/set_value.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/slice.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transdata.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/softmax.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transpose.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/sort.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/unpad.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/split.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/where.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/stridebatchmatmul.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transdata.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transpose.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/unpad.py
+Filename: ms-ait-7.0.0rc2/components/llm/ait_llm/transform/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/where.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/__init__.py
+Filename: ms-ait-7.0.0rc2/components/profile/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/utils.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/llm/ait_llm/transform/__init__.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/__init__.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/api.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/install.sh
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/args_adapter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/README.md
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/main_cli.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/msprof_process.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/setup.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/__init__.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/api.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/args_adapter.py
+Filename: ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/main_cli.py
+Filename: ms-ait-7.0.0rc2/components/tests/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/msprof_process.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/utils.py
+Filename: ms-ait-7.0.0rc2/components/transplt/install.bat
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__install__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/README.md
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__main__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/requirements.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/
+Filename: ms-ait-7.0.0rc2/components/transplt/setup.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/transplt/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/setup.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/common/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/atb.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/handler.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/logger.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/main_cli.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/operation.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/print_stat.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/install.bat
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__install__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/install.sh
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tests/test_ait.sh
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/tests/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/__install__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/__main__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/install.bat
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/common/kit_config.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/install.sh
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/common/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/README.md
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/exception_information.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/requirements.txt
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/source_scan_exception.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/setup.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/model.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/common/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/project.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/exception/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/seq_project.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/model/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/app.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/cmdline_input.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/custom_input.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/solution/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/input_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/porting_input.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/install.bat
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/install.sh
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/csv_report.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/json_report.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/__install__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/__main__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/common/kit_config.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/report/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/common/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/exception/exception_information.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/exception/source_scan_exception.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/exception/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/model.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cmake_scanner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/project.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cxx_scanner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/seq_project.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/func_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/model/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/app.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_scanner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/cmdline_input.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/custom_input.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_factory.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/input_factory.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/porting_input.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scan_api.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/porting/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/csv_report.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/comment_delete.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/json_report.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/file_matrix.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/report.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/report_factory.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/acc_libs.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/report/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/api_filter.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/ast_visitor.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_desc.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_parser.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_handler.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_utils.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_matcher.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cmake_scanner.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_utils.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cxx_scanner.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/func_parser.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/advisor.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_parser.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/seq_advisor.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_scanner.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/clang_finder.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_factory.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/excel.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_utils.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/file_locker.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scan_api.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/io_util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/lib_util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/comment_delete.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/log_util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/file_matrix.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/security.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/__init__.py
+Filename: ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/acc_libs.py
+Filename: ms-ait-7.0.0rc2/components/utils/file_open_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/api_filter.py
+Filename: ms-ait-7.0.0rc2/components/utils/install.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/ast_visitor.py
+Filename: ms-ait-7.0.0rc2/components/utils/parser.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_desc.py
+Filename: ms-ait-7.0.0rc2/components/utils/security_check.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_handler.py
+Filename: ms-ait-7.0.0rc2/components/utils/util.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_matcher.py
+Filename: ms-ait-7.0.0rc2/components/utils/__init__.py
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_utils.py
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/__init__.py
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/entry_points.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/solution/advisor.py
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/PKG-INFO
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/solution/seq_advisor.py
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/solution/__init__.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/clang_finder.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/excel.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/file_locker.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/io_util.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/lib_util.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/log_util.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/security.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/transplt/app_analyze/utils/__init__.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/utils/file_open_check.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/utils/install.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/utils/parser.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/utils/security_check.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/utils/util.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/components/utils/__init__.py
-Comment: 
-
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/dependency_links.txt
-Comment: 
-
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/entry_points.txt
-Comment: 
-
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/PKG-INFO
-Comment: 
-
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/SOURCES.txt
-Comment: 
-
-Filename: ms-ait-7.0.0b430/ms_ait.egg-info/top_level.txt
+Filename: ms-ait-7.0.0rc2/ms_ait.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `ms-ait-7.0.0b430/README.md` & `ms-ait-7.0.0rc2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 #  AIT
 
 ## 目录
-- [AIT](#ait)
-  - [目录](#目录)
-  - [介绍](#介绍)
-    - [AIT各子功能介绍](#ait各子功能介绍)
-  - [工具安装](#工具安装)
-  - [工具使用](#工具使用)
-    - [命令行格式说明](#命令行格式说明)
-  - [参考](#参考)
-    - [AIT资源](#ait资源)
-    - [常见问题FAQ](#常见问题faq)
-  - [许可证](#许可证)
-  - [公网URL说明](#公网url说明)
-  - [免责声明](#免责声明)
+- [介绍](#介绍)
+- [工具安装](#工具安装)
+- [工具使用](#工具使用)
+- [许可证](#许可证)
+- [免责声明](#免责声明)
 
 ## 介绍
 AIT(Ascend Inference Tools)作为昇腾统一推理工具，提供客户一体化开发工具，用于辅助用户进行模型迁移以及性能与精度的调试调优，当前包括benchmark、debug、transplt、analyze、llm等组件。
 
 ### AIT各子功能介绍
-| 任务类型                                | 子功能                           | 说明                                       |
-|-------------------------------------|-------------------------------|------------------------------------------|
-| [benchmark](docs/benchmark)         | -                             | 用来针对指定的推理模型运行推理程序，并能够测试推理模型的性能（包括吞吐率、时延） |
-| debug(一站式调试)                        | [surgeon](docs/debug/surgeon) | 使能ONNX模型在昇腾芯片的优化，并提供基于ONNX的改图功能          |
-| debug(一站式调试)                        | [compare](docs/debug/compare) | 提供自动化的推理场景精度比对，用来定位问题算子                  |
-| [analyze](components/analyze)       | -                             | 提供其他平台模型迁移至昇腾平台的支持度分析功能                  |
-| [transplt](components/transplt)     | -                             | 提供NV C++推理应用迁移分析以及昇腾API推荐功能              |
-| [convert](components/convert)       | -                             | 提供推理模型转换功能                               |
-| [profile](docs/profile)             | -                             | 提供profiling，提供整网详细的性能数据及相关信息             |
-| [llm](docs/llm/README.md) | -                             | 提供加速库（atb）大模型推理调试工具，包括数据dump功能和数据比对功能    |
-| [tensor-view](docs/tensor_view)     | -                             | 提供查看、切片、转置、保存tensor的接口                   |
+| 任务类型                        | 子功能                           | 说明                                      |
+|-----------------------------|-------------------------------|-----------------------------------------|
+| [benchmark](docs/benchmark) | -                             | 用来针对指定的推理模型运行推理程序，并能够测试推理模型的性能（包括吞吐率、时延） |
+| debug(一站式调试)                | [surgeon](docs/debug/surgeon) | 使能ONNX模型在昇腾芯片的优化，并提供基于ONNX的改图功能         |
+| debug(一站式调试)                | [compare](docs/debug/compare) | 提供自动化的推理场景精度比对，用来定位问题算子                 |
+| [analyze](components/analyze) | -                             | 提供其他平台模型迁移至昇腾平台的支持度分析功能                 |
+| [transplt](components/transplt) | -                             | 提供NV C++推理应用迁移分析以及昇腾API推荐功能             |
+| [convert](components/convert) | -                             | 提供推理模型转换功能                              |
+| [profile](docs/profile) | - | 提供profiling，提供整网详细的性能数据及相关信息            |
+| [llm](components/llm) | - | 提供加速库（atb）大模型推理调试工具，包括数据dump功能和数据比对功能            |
 
 
 ## 工具安装
 [一体化安装指导](docs/install/README.md)
 
 
 ## 工具使用
```

## Comparing `ms-ait-7.0.0b430/setup.py` & `ms-ait-7.0.0rc2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,46 +17,31 @@
 from setuptools import setup, find_packages
 
 
 abs_path = os.path.dirname(os.path.realpath(__file__))
 with open(os.path.join(abs_path, "requirements.txt")) as f:
     required = f.read().splitlines()
 
-ait_sub_tasks = [
-    {
-        "name": "debug",
-        "help_info": "debug a wide variety of model issues",
-        "module": "components.debug.__init__",
-        "attr": "debug_task",
-    }
-]
+ait_sub_tasks = [{
+    "name": "debug",
+    "help_info": "debug a wide variety of model issues",
+    "module": "components.debug.__init__",
+    "attr": "debug_task"
+}]
 
-ait_sub_task_entry_points = [
-    f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
-    for t in ait_sub_tasks
-]
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
     name='ms-ait',
-    version='7.0.0b430',
+    version='7.0.0c2',
     description='AIT, Ascend Inference Tools',
     long_description_content_type='text/markdown',
     url='https://gitee.com/ascend/ait',
     packages=find_packages(),
-    package_data={
-        '': [
-            'LICENSE',
-            'README.md',
-            '*.txt',
-            '*.bat',
-            '*.sh',
-            '*.cpp',
-            '*.h',
-        ]
-    },
+    package_data={'': ['LICENSE', 'README.md', 'requirements.txt', 'install.bat', 'install.sh', '*.cpp', '*.h']},
     data_files=[('', ['requirements.txt'])],
     license='Apache-2.0',
     keywords='ait',
     python_requires='>=3.7',
     install_requires=required,
     entry_points={
         'console_scripts': ['ait=components.__main__:main'],
```

## Comparing `ms-ait-7.0.0b430/components/__init__.py` & `ms-ait-7.0.0rc2/components/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/README.md` & `ms-ait-7.0.0rc2/components/analyze/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/setup.py` & `ms-ait-7.0.0rc2/components/analyze/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,24 +18,21 @@
 with open('requirements.txt', encoding='utf-8') as f:
     required = f.read().splitlines()
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 ait_sub_tasks = [{
-    "name": "analyze",
+    "name": "model",
     "help_info": "Analyze tool to evaluate compatibility of model conversion",
     "module": "model_evaluation.__main__",
     "attr": "get_cmd_instance"
 }]
 
-ait_sub_task_entry_points = [
-    f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
-    for t in ait_sub_tasks
-]
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
     name='ait-analyze',
     version='7.0.0c2',
     description='inference analyze tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

## Comparing `ms-ait-7.0.0b430/components/analyze/__init__.py` & `ms-ait-7.0.0rc2/components/analyze/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/__install__.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
+# Copyright (c) 2023 Huawei Technologies Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from components.utils.install import AitInstaller
 
-
-class AnalyzeInstall(AitInstaller):
-    pass
+from model_evaluation.data.opp import Opp
+from model_evaluation.data.op_map import OpMap
```

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/__main__.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/config.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/op_info.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/op_info.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/bean/__init__.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/bean/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/const.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/const.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/log.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/utils.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/atc_err.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/atc_err.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/engine.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/engine.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/framework.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/framework.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/onnx_checker_err.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/onnx_checker_err.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/common/enum/soc_type.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/common/enum/soc_type.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/core/analysis.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/analysis.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/core/result.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/result.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/core/rule.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/rule.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/core/checker/onnx.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/core/checker/onnx.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/data/opp.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/opp.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/data/op_map.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/data/op_map.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/data/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# Copyright (c) 2023 Huawei Technologies Co., Ltd.
+# Copyright 2022 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from model_evaluation.data.opp import Opp
-from model_evaluation.data.op_map import OpMap
+from auto_optimizer.inference_engine.model_convert.om_compiler import OmCompiler, onnx2om
```

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/graph/onnx.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/graph/onnx.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/atc.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/atc.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/model.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/model.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/om.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/om.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/analyze/model_evaluation/parser/__init__.py` & `ms-ait-7.0.0rc2/components/analyze/model_evaluation/parser/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_infer.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_infer.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/install.sh` & `ms-ait-7.0.0rc2/components/benchmark/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/README.md` & `ms-ait-7.0.0rc2/components/benchmark/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/setup.py` & `ms-ait-7.0.0rc2/components/benchmark/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,29 +23,27 @@
 ait_sub_tasks = [{
     "name": "benchmark",
     "help_info": "benchmark tool to get performance data including latency and throughput",
     "module": "ais_bench.infer.main_cli",
     "attr": "get_cmd_instance"
 }]
 
-ait_sub_task_entry_points = [
-    f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
-    for t in ait_sub_tasks
-]
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
-    name='ais_bench',
-    version='0.0.2',
-    description='ais_bench tool',
+    name='ait-benchmark', # 不与ais_bench冲突
+    version='7.0.0c2',
+    description='ais_bench tool(ait)',
     long_description=long_description,
     url='ais_bench url',
     packages=find_packages(),
     package_data={'': ['LICENSE', 'README.md', 'requirements.txt', 'install.bat', 'install.sh', '*.cpp', '*.h']},
     include_package_data=True,
     keywords='ais_bench tool',
     install_requires=required,
     python_requires='>=3.7',
     entry_points={
         'ait_sub_task': ait_sub_task_entry_points,
         'ait_sub_task_installer': ['ait-benchmark=ais_bench.__install__:BenchmarkInstall'],
     },
+
 )
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `ms-ait-7.0.0b430/components/benchmark/__init__.py` & `ms-ait-7.0.0rc2/components/benchmark/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/__main__.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/interface.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/interface.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/log.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/README.md` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/recorder.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/recorder.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/base_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_adapter.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_adapter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/args_check.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/args_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/benchmark_process.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/benchmark_process.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/interface.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/interface.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/io_oprations.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/io_oprations.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/main_cli.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/main_cli.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/miscellaneous.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/miscellaneous.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/path_security_check.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/path_security_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 PATH_WHITE_LIST_REGEX_WIN = re.compile(r"[^_:\\A-Za-z0-9/.-]")
 PATH_WHITE_LIST_REGEX = re.compile(r"[^_A-Za-z0-9/.-]")
 
 PERMISSION_NORMAL = 0o640  # 普通文件
 PERMISSION_KEY = 0o600  # 密钥文件
 READ_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH
-WRITE_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH
+WRITE_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH | stat.S_IROTH | stat.S_IXOTH
 
 SOLUTION_LEVEL = 35
 SOLUTION_LEVEL_WIN = 45
 logging.addLevelName(SOLUTION_LEVEL, "\033[1;32m" + "SOLUTION" + "\033[0m")  # green [SOLUTION]
 logging.addLevelName(SOLUTION_LEVEL_WIN, "SOLUTION_WIN")
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format='[%(levelname)s] %(message)s')
 logger = logging.getLogger(__name__)
@@ -199,15 +199,15 @@
                 )
                 solution_log(SOLUTION_BASE_URL + PERMISSION_SUB_URL)
                 return False
         elif perm == 'write' and self.is_exists:
             if self.permission & WRITE_FILE_NOT_PERMITTED_STAT > 0:
                 logger.error(
                     f"The file {self.file} is group writable, or is others writable, as export file(or directory), "
-                    "permission should not be over 0o755(rwxr-xr-x)"
+                    "permission should not be over 0o750(rwxr-x---)"
                 )
                 solution_log(SOLUTION_BASE_URL + PERMISSION_SUB_URL)
                 return False
             if not os.access(self.realpath, os.W_OK):
                 logger.error(
                     f"Current user doesn't have write permission to the file {self.file}, as export file(or directory), "
                     "permission should be at least 0o200(-w-------) "
```

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/registry.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/registry.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/summary.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/summary.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/utils.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/__main__.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/backend_trtexec.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/backend_trtexec.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/ais_bench/infer/backends/__init__.py` & `ms-ait-7.0.0rc2/components/benchmark/ais_bench/infer/backends/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/backend/install.sh` & `ms-ait-7.0.0rc2/components/benchmark/backend/install.sh`

 * *Files 2% similar despite different names*

```diff
@@ -33,27 +33,27 @@
 {
     check_python_package_is_install ${PYTHON_COMMAND} "aclruntime" \
     || { echo "aclruntime package not install"; return $ret_run_failed;}
 }
 
 main()
 {
-    while [ -n "$1" ]
+      while [ -n "$1" ]
 do
-    case "$1" in
-        -p|--python_command)
-            PYTHON_COMMAND=$2
-            shift
-            ;;
-        *)
-            echo "$1 is not an option, please use --help"
-            exit 1
-            ;;
-    esac
-    shift
+  case "$1" in
+    -p|--python_command)
+        PYTHON_COMMAND=$2
+        shift
+        ;;
+    *)
+        echo "$1 is not an option, please use --help"
+        exit 1
+        ;;
+  esac
+  shift
 done
 
     [ "$PYTHON_COMMAND" != "" ] || { PYTHON_COMMAND="python3.7";echo "set default pythoncmd:$PYTHON_COMMAND"; }
 
     check_env_valid
     res=`echo $?`
     if [ $res =  $ret_run_failed ]; then
```

## Comparing `ms-ait-7.0.0b430/components/benchmark/backend/setup.py` & `ms-ait-7.0.0rc2/components/benchmark/backend/setup.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/infer_analyser/analyser.py` & `ms-ait-7.0.0rc2/components/benchmark/infer_analyser/analyser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/benchmark/infer_analyser/info_convert_json.py` & `ms-ait-7.0.0rc2/components/benchmark/infer_analyser/info_convert_json.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/build.sh` & `ms-ait-7.0.0rc2/components/convert/model_convert/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/README.md` & `ms-ait-7.0.0rc2/components/convert/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/setup.py` & `ms-ait-7.0.0rc2/components/convert/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,18 +22,15 @@
     "name": "convert",
     "help_info": "convert tool converts the model from ONNX, TensorFlow, Caffe and MindSpore to OM. \
                    It supports atc, aoe and aie.",
     "module": "model_convert.__main__",
     "attr": "get_cmd_instance"
 }]
 
-ait_sub_task_entry_points = [
-    f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
-    for t in ait_sub_tasks
-]
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
     name='ait-convert',
     version='7.0.0c2',
     description='model convert tool',
     url='https://gitee.com/ascend/ait',
     packages=find_packages(),
```

## Comparing `ms-ait-7.0.0b430/components/convert/__init__.py` & `ms-ait-7.0.0rc2/components/convert/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/cmd_utils.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/cmd_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/__init__.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/__install__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/install.sh`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,27 @@
+#!/usr/bin/env bash
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import sys
-import os
-import subprocess
-from components.utils.install import AitInstaller
+CURRENT_DIR=$(dirname $(readlink -f $0))
 
 
-class ConvertInstall(AitInstaller):
-    def check(self):
-        check_res = []
+build_opchecker_so() {
+    echo ""
+    echo "Try building libatb_speed_torch.so for ait llm. If not using opecheck, ignore errors if any"
+    cd ${CURRENT_DIR}/opcheck/atb_operators
+    bash build.sh
+    cd -
+    echo ""
+}
 
-        if not os.path.exists(os.path.join(os.path.dirname(__file__), "aie_convert")):
-            check_res.append("[warnning] build aie_convert failed. will make the AIE feature unusable. "
-                             "use `ait build-extra convert` to try again")
-        
-        if not check_res:
-            return "OK"
-        else:
-            return "\n".join(check_res)
-        
-    def build_extra(self, find_links=None):
-        if sys.platform == 'win32':
-            return
-
-        subprocess.run(["/bin/bash", os.path.abspath(os.path.join(os.path.dirname(__file__), "install.sh"))], shell=False)
+build_opchecker_so
```

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/__main__.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/config.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aie/bean/__init__.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aie/bean/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aie/core/convert.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/convert.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aie/core/__init__.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aie/core/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/aoe/aoe_args_map.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/aoe/aoe_args_map.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/convert/model_convert/atc/atc_args_map.py` & `ms-ait-7.0.0rc2/components/convert/model_convert/atc/atc_args_map.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/__init__.py` & `ms-ait-7.0.0rc2/components/debug/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/main.py` & `ms-ait-7.0.0rc2/components/debug/compare/main.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/README.md` & `ms-ait-7.0.0rc2/components/debug/compare/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/setup.py` & `ms-ait-7.0.0rc2/components/debug/compare/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 debug_sub_tasks = [{
     "name": "compare",
     "help_info": "one-click network-wide accuracy analysis of golden models.",
     "module": "msquickcmp.__main__",
     "attr": "get_cmd_instance"
 }]
 
-debug_sub_task_entry_points = [
-    f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
-    for t in debug_sub_tasks
-]
+debug_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in debug_sub_tasks]
 
 setup(
     name='ait-compare',
     version='7.0.0c2',
     description='This tool enables one-click network-wide accuracy analysis of gold model.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/cmp_process.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/cmp_process.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/install.sh` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/l1_buffer_data_parser.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/l1_buffer_data_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf_debug_runner.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf_debug_runner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/__main__.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/accuracy_locat/accuracy_locat.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/adapter_cli/args_adapter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/atc/atc_utils.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/atc/atc_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/caffe_model/caffe_dump_data.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/args_check.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/args_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/convert.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/convert.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dump_data.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dump_data.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/dynamic_argument_bean.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/tf_common.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/tf_common.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/common/utils.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -575,20 +575,19 @@
         command output result
     Exception Description:
         when invalid command throw exception
     """
     if info_need:
         logger.info('Execute command:%s' % " ".join(cmd))
     process = subprocess.Popen(cmd, shell=False, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-    ais_bench_logs = ""
     while process.poll() is None:
-        ais_bench_logs += process.stdout.readline().decode()
+        line = process.stdout.readline()
+        line = line.strip()
     if process.returncode != 0:
         logger.error('Failed to execute command:%s' % " ".join(cmd))
-        logger.error(f'\nais_bench error log:\n {ais_bench_logs}')
         raise AccuracyCompareException(ACCURACY_COMPARISON_INVALID_DATA_ERROR)
 
 
 def create_directory(dir_path):
     """
     Function Description:
         creating a directory with specified permissions
```

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/analyser.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/analyser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/net_compare/net_compare.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/net_compare/net_compare.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/npu_dump_data.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/npu_dump_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,18 +81,17 @@
 
     @staticmethod
     def get_input_shape_from_om(om_parser):
         # get atc input shape from atc cmdline
         atc_input_shape = ""
         atc_cmd_args = om_parser.get_atc_cmdline().split(" ")
         for i, atc_arg in enumerate(atc_cmd_args):
-            if INPUT_SHAPE == atc_arg:
-                atc_input_shape = atc_cmd_args[i + 1]
-                break
-            if atc_arg.startswith(INPUT_SHAPE + utils.EQUAL):
+            if INPUT_SHAPE in atc_arg:
+                if INPUT_SHAPE == atc_arg:
+                    atc_arg += '=' + atc_cmd_args[i + 1]
                 atc_input_shape = atc_arg.split(utils.EQUAL)[1]
                 break
         return atc_input_shape
 
     @staticmethod
     def get_arg_value(om_parser, input_shape):
         is_dynamic_scenario, scenario = om_parser.get_dynamic_scenario_info()
```

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/npu/om_parser.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/npu/om_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -159,16 +159,15 @@
                 count += len(operator.get(INPUT_DESC_OBJECT))
         return count
 
     def get_atc_cmdline(self):
         for attr in self.json_object.get(ATTR_OBJECT):
             if KEY_OBJECT in attr and attr.get(KEY_OBJECT) == ATC_CMDLINE_OBJECT:
                 if VALUE_OBJECT in attr and S_OBJECT in attr.get(VALUE_OBJECT):
-                    atc_cmd = attr.get(VALUE_OBJECT).get(S_OBJECT)
-                    return self._replace_input_shape_with_input_shape_range_in_atc_cmd_if_dynamic(atc_cmd)
+                    return attr.get(VALUE_OBJECT).get(S_OBJECT)
         return ''
 
     def get_expect_net_output_name(self):
         """
         Get the expected output tensor corresponding to Net_output.
         """
         net_output_names = []
@@ -227,63 +226,14 @@
         subgraph_name = []
         for graph in self.json_object.get(GRAPH_OBJECT):
             for operator in graph.get(OP_OBJECT):
                 if SUBGRAPH_NAME in operator:
                     subgraph_name += operator.get(SUBGRAPH_NAME)
         return subgraph_name
 
-    def _replace_input_shape_with_input_shape_range_in_atc_cmd_if_dynamic(self, atc_cmd):
-        # `--input_shape_range` is deprecated, and replaced with `--input_shape` in atc.
-        # but `--input_shape_range` is currently used in parsing model as dynamic shape one,
-        # It's more convinient for using and doesn't matter in comparing process.
-        # Thus `--input_shape` args is converted to `--input_shape_range` in
-        # this function for further comparing usage.
-        atc_cmd_split = []
-        for cmd_token in atc_cmd.split():
-            atc_cmd_split += cmd_token.split("=")  # Could be in format like "--input_shape=input:1,3,224,224"
-
-        # Return if any dynamic args already involved
-        for dym_arg in DynamicArgumentEnum:
-            if dym_arg.value.atc_arg in atc_cmd_split:
-                return atc_cmd
-
-        # Check if `--input_shape` in atc_cmd line. Return if not
-        input_shape_pos = -1
-        for pos, cmd_token in enumerate(atc_cmd_split):
-            if cmd_token == INPUT_SHAPE:
-                input_shape_pos = pos
-
-        if input_shape_pos == -1 or len(atc_cmd_split) <= input_shape_pos + 1:
-            return atc_cmd
-
-        # Check if dynamic `--input_shape`
-        input_shape_args = atc_cmd_split[input_shape_pos + 1]
-        if "-1" not in input_shape_args and "~" not in input_shape_args:
-            return atc_cmd
-
-        # replace `--input_shape` with `--input_shape_range` if dynamic
-        input_shape_range_args_split = []
-        for inputs in input_shape_args.split(';'):
-            inputs_split = inputs.split(':')
-            input_name, input_shape = ":".join(inputs_split[:-1]), inputs_split[-1]
-            input_shape_range_args_split.append('{}:[{}]'.format(input_name, input_shape))
-        input_shape_range_args = ';'.join(input_shape_range_args_split)
-
-        atc_cmd_with_range_split = atc_cmd_split[:input_shape_pos]
-        atc_cmd_with_range_split += [INPUT_SHAPE_RANGE, input_shape_range_args]
-        atc_cmd_with_range_split += atc_cmd_split[input_shape_pos + 2:]
-        atc_cmd_with_range = " ".join(atc_cmd_with_range_split)
-
-        if not self.shape_range:  # Only print once, just if shape_range is False
-            utils.logger.info(
-                f"Convert atc arg '{INPUT_SHAPE} {input_shape_args}' -> '{INPUT_SHAPE_RANGE} {input_shape_range_args}'"
-            )
-        self.shape_range = True
-        return atc_cmd_with_range
-
     def _gen_operator_list(self):
         _, scenario = self.get_dynamic_scenario_info()
         for graph in self.json_object.get(GRAPH_OBJECT):
             if graph.get(NAME_OBJECT) in self.subgraph_name and scenario not in [
                 DynamicArgumentEnum.DYM_BATCH,
                 DynamicArgumentEnum.DYM_DIMS,
             ]:
```

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/custom_op.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/custom_op.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/onnx_model/onnx_dump_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 """
 Function:
 This class is used to generate GUP dump data of the ONNX model.
 """
 import sys
 import os
 import re
-import time
 
 import onnx
 import onnxruntime
 import numpy as np
+from skl2onnx.helpers.onnx_helper import enumerate_model_node_outputs
+from skl2onnx.helpers.onnx_helper import select_model_inputs_outputs
 
 from msquickcmp.common.dump_data import DumpData
 from msquickcmp.common import utils
 from msquickcmp.common.utils import AccuracyCompareException
 from msquickcmp.common.utils import InputShapeError
 from msquickcmp.adapter_cli.args_adapter import CmpArgsAdapter
 from msquickcmp.common.convert import convert_bin_file_to_npy
@@ -118,42 +119,42 @@
             self.inputs_map = self._get_inputs_data(inputs_tensor_info)
 
         # extend inputs add by removed custom op
         if self.custom_op_type:
             self.inputs_map.update(self.extend_inputs_map)
 
     def generate_dump_data(self, npu_dump_path=None, om_parser=None):
-        self._modify_model_add_outputs_nodes(
+        dump_model_with_inputs_contents = self._modify_model_add_outputs_nodes(
             self.model_with_inputs, self.dump_model_with_inputs_path
         )
-        session = self._load_session(self.dump_model_with_inputs_path)
+        session = self._load_session(dump_model_with_inputs_contents)
         dump_bins = self._run_model(session, self.inputs_map)
 
         net_output_node = [output_item.name for output_item in self.model_with_inputs_session.get_outputs()]
         self._save_dump_data(dump_bins, self.model_with_inputs, net_output_node)
 
         return self.onnx_dump_data_dir
 
-    def _load_session(self, model_path):
+    def _load_session(self, model_contents):
         options = onnxruntime.SessionOptions()
         if not self.onnx_fusion_switch:
             options.graph_optimization_level = onnxruntime.GraphOptimizationLevel.ORT_DISABLE_ALL
         try:
-            infersession = onnxruntime.InferenceSession(model_path, options)
+            infersession = onnxruntime.InferenceSession(model_contents, options)
         except Exception as e:
             utils.logger.error(f"Please check onnx model can run in local env. Error: {e}")
             raise utils.AccuracyCompareException(utils.ACCURACY_COMPARISON_MODEL_TYPE_ERROR)
         return infersession
 
     def _load_onnx(self, model_path):
         # model_path str -> read as bytes -> deserialize to onnx_model
         #                                 -> onnxruntime load as session
         with open(model_path, "rb") as ff:
             model_contents = ff.read()
-        onnx_model = onnx.load_model(model_path)
+        onnx_model = onnx.load_model_from_string(model_contents)
         for index, node in enumerate(onnx_model.graph.node):
             if not node.name:
                 node.name = node.op_type + "_" + str(index)
         return onnx_model, model_contents
 
     def _new_model_save_path(self, origin_path):
         save_name = "new_" + os.path.basename(origin_path)
@@ -176,34 +177,32 @@
             model_relative_name = "model"
             if self.dump:
                 model_dir = os.path.join(self.out_path, model_relative_name)
                 utils.create_directory(model_dir)
         return data_dir, onnx_dump_data_dir, model_dir
 
     def _modify_model_add_outputs_nodes(self, onnx_model, save_path):
-        if self.dump:
-            onnx_model.graph.output.extend(
-                onnx.ValueInfoProto(name=tensor_name) 
-                for node in onnx_model.graph.node 
-                for tensor_name in node.output
-            )
-        
-        model_size = onnx_model.ByteSize()
-        save_external_flag = model_size < 0 or model_size > MAX_PROTOBUF
-        
-        utils.logger.debug("Modfied model has size over 2G: %s", save_external_flag)
-        
+        if not self.dump:
+            origin_model_graph_output = onnx_model.graph.output
+            outputs_name_list = [output_node.name for output_node in origin_model_graph_output]
+            outputs_name = [name for name in enumerate_model_node_outputs(onnx_model) if name in outputs_name_list]
+        else:
+            outputs_name = [name for name in enumerate_model_node_outputs(onnx_model)]
+        new_onnx_model = select_model_inputs_outputs(onnx_model, outputs_name)
+        bytes_model = new_onnx_model.SerializeToString()
+        save_as_external_data_switch = sys.getsizeof(bytes_model) > MAX_PROTOBUF
         onnx.save_model(
-            onnx_model, 
+            new_onnx_model,
             save_path,
-            save_as_external_data=save_external_flag
+            save_as_external_data=save_as_external_data_switch,
+            location=self.model_dir if save_as_external_data_switch else None,
         )
-        
-        utils.logger.info("Modified model has being saved successfully at: %s", os.path.abspath(save_path))
-        
+        utils.logger.info("modify model outputs success: %s", save_path)
+        return bytes_model
+
     def _get_inputs_tensor_info(self):
         inputs_tensor_info = []
         input_tensor_names = [item.name for item in self.model_with_inputs_session.get_inputs()]
         for _, tensor_name in enumerate(self.input_shapes):
             utils.check_input_name_in_model(input_tensor_names, tensor_name)
         for input_item in self.model_with_inputs_session.get_inputs():
             tensor_name = input_item.name
@@ -295,33 +294,22 @@
 
     def _run_model(self, session, inputs_map):
         outputs_name = [node.name for node in session.get_outputs()]
         return session.run(outputs_name, inputs_map)
 
     def _save_dump_data(self, dump_bins, old_onnx_model, net_output_node):
         res_idx = 0
-        file_name_map = []
         for node in old_onnx_model.graph.node:
             for j, output in enumerate(node.output):
                 if not self.dump and output not in net_output_node:
                     continue
                 file_name = self._generate_dump_data_file_name(node.name, j)
-                if len(file_name) > 255:
-                    new_file_name = str(round(time.time() * 1e6)) + str(len(file_name_map)) + ".npy"
-                    file_name_map.append(f"{new_file_name},{file_name}\n")
-                    file_name = new_file_name
-
                 file_path = os.path.join(self.onnx_dump_data_dir, file_name)
                 if output in net_output_node:
                     self.net_output[net_output_node.index(output)] = file_path
                 np.save(file_path, dump_bins[res_idx])
                 res_idx += 1
 
-        if len(file_name_map) > 0:
-            mapping_file_path = os.path.join(self.onnx_dump_data_dir, "mapping.csv")
-            with open(mapping_file_path, "w") as map_file:
-                map_file.writelines(file_name_map)
-
         if not self.single_op:
             for key, value in self.net_output.items():
                 utils.logger.info("net_output node is:{}, file path is {}".format(key, value))
         utils.logger.info("dump data success")
```

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/save_om_model/export_om_model.cpp`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/single_op/single_op.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/single_op/single_op.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/compare/msquickcmp/tf/tf_dump_data.py` & `ms-ait-7.0.0rc2/components/debug/compare/msquickcmp/tf/tf_dump_data.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/README.md` & `ms-ait-7.0.0rc2/components/debug/surgeon/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/setup.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 debug_sub_tasks = [{
     "name": "surgeon",
     "help_info": "surgeon tool for onnx modifying functions.",
     "module": "auto_optimizer.ait_main",
     "attr": "get_cmd_instance"
 }]
 
-debug_sub_task_entry_points = [
-    f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
-    for t in debug_sub_tasks
-]
+debug_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in debug_sub_tasks]
 
 setup(
     name='ait-surgeon',
     version='7.0.0c2',
     description='auto optimizer',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/ait_main.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/ait_main.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/options.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/options.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__install__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transpose.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from components.utils.install import AitInstaller
-import pkg_resources
 
+import sys
+import os
+import unittest
+import torch
+import torch_npu
 
-class SurgeonInstall(AitInstaller):
-    def check(self):
-        check_res = []
-        installed_pkg = [pkg.key for pkg in pkg_resources.working_set]
+from ait_llm.opcheck import operation_test
 
-        if "ais-bench" not in installed_pkg:
-            check_res.append("[warnning] ait-benchmark not installed. will make the inference feature unusable. "
-                             "use `ait install benchmark` to try again")
 
-        if not check_res:
-            return "OK"
-        else:
-            return "\n".join(check_res)
+class OpcheckTransposeOperation(operation_test.OperationTest):
+    def golden_calc(self, in_tensors):
+        perm = self.op_param["perm"]
+        golden_result = in_tensors[0].permute(perm)
+        return [golden_result]
+
+    def test_2d_float(self):
+        self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/__main__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/args_check.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/args_check.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/click_utils.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/click_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 STR_UNSAFE_LIST_REGEX = re.compile(r"[^_A-Za-z0-9/.-]")
 PATH_WHITE_LIST_REGEX = re.compile(r"[^_A-Za-z0-9/.-]")
 
 READ_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH
-WRITE_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH
+WRITE_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH | stat.S_IROTH | stat.S_IXOTH
 
 
 def safe_string(value):
     if not value:
         return value
     if re.search(STR_UNSAFE_LIST_REGEX, value):
         raise ValueError("String parameter contains invalid characters.")
```

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/config.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/log.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/register.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/register.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/singleton.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/singleton.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/utils.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/common/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/common/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_optimizer/optimizer.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/README.md` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_graph.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/base_node.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/interface/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/graph.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/node.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/graph_refactor/onnx/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/data_process_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/README.md` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/dataset_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/datasets/vision/imagenet.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/evaluate/evaluate_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/acl_inference.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/inference_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/inference/onnx_inference.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/compiler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/om_compiler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/model_convert/__init__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright 2022 Huawei Technologies Co., Ltd
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from auto_optimizer.inference_engine.model_convert.om_compiler import OmCompiler, onnx2om
+# Copyright (c) 2024 Huawei Technologies Co., Ltd.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+from ait_llm.dump.torch_dump.dump_config import DumpConfig
+from ait_llm.dump.torch_dump.hook import register_hook
```

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/post_process_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/post_process/vision/classification.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/pre_process_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/inference_engine/pre_process/vision/classification.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledge_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/matcher.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/matcher.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/pattern.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/pattern.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/utils.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_avgpool_split.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_base.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_bn_folding.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_conv1d2conv2d.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_dynamic_reshape.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_empty_slice_fix.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_gather_to_split.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_casts.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_concat.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_merge_consecutive_slice.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_modify_reflection_pad.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_resize_mode_to_nearest.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_large_kernel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_split_qkv_matmul.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_topk_fix.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_transpose_large_input_conv.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/knowledge_type_cast.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/attention_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/knowledge_big_kernel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/transform_refactor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/pattern/knowledges/big_kernel/util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/inference.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/inference.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/debug/surgeon/auto_optimizer/tools/log.py` & `ms-ait-7.0.0rc2/components/debug/surgeon/auto_optimizer/tools/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/README.md` & `ms-ait-7.0.0rc2/components/llm/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,14 @@
   | ----- | ---------- | ---- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
   | 0.0.1 | 2023/12/13 | arm  | 7.0.0.RC1 | [ait-0.0.1-py3-none-linux_aarch64.whl](https://ais-bench.obs.cn-north-4.myhuaweicloud.com/compare/20231213/ait-0.0.1-py3-none-linux_aarch64.whl) | 271051e901bb3513c7a0edbd1e096cb2 |
   | 0.0.1 | 2023/12/13 | x86  | 7.0.0.RC1 | [ait-0.0.1-py3-none-linux_x86_64.whl](https://ais-bench.obs.cn-north-4.myhuaweicloud.com/compare/20231213/ait-0.0.1-py3-none-linux_x86_64.whl)   | 9903fa06b9ff76cba667abf0cbc4da50 |
 - ait-llm 工具 whl：
 
   | 版本  | 发布日期   | 平台       | CANN 版本    | whl链接                                                      | MD5 校验码                       | 使用指导                                                     |
   | ----- | ---------- | ---------- | ------------ | ------------------------------------------------------------ | -------------------------------- | ------------------------------------------------------------ |
-  | 1.1   | 2024/05/08 | arm        | 8.0.RC2 B010 | [ait_llm-1.1-py3-none-linux_aarch64.whl](https://ais-bench.obs.cn-north-4.myhuaweicloud.com/compare/20240508/ait_llm-1.1-py3-none-linux_aarch64.whl)                    |0133c8fda39ba78c2b02354b4bcf089c                                | [大模型推理精度工具](../../docs/llm/README.md) |
-  | 1.1   | 2024/05/08 | x86        | 8.0.RC2 B010 | [ait_llm-1.1-py3-none-linux_x86_64.whl](https://ais-bench.obs.cn-north-4.myhuaweicloud.com/compare/20240508/ait_llm-1.1-py3-none-linux_x86_64.whl)                     |d453b4b608b4400d77bbfb1b5c702bee                                | [大模型推理精度工具](../../docs/llm/README.md) |
   | 1.0   | 2024/03/22 | arm        | 8.0.RC1      | [ait_llm-1.0-py3-none-linux_aarch64.whl](https://ais-bench.obs.cn-north-4.myhuaweicloud.com/compare/20240325/ait_llm-1.0-py3-none-linux_aarch64.whl)                          |9f7f69d49e017f98006b8191f3951868                                  | [大模型推理精度工具说明文档](../../docs/llm/v1.0/大模型推理精度工具说明文档.md) |
   | 1.0   | 2024/03/22 | x86        | 8.0.RC1      |[ait_llm-1.0-py3-none-linux_x86_64.whl](https://ais-bench.obs.cn-north-4.myhuaweicloud.com/compare/20240325/ait_llm-1.0-py3-none-linux_x86_64.whl)                          |5a6735c9f04d3938a6384c460399ff9a                                  | [大模型推理精度工具说明文档](../../docs/llm/v1.0/大模型推理精度工具说明文档.md) |
   |       |            |            |              |                                                              |                                  |                                                              |
   | 0.2.1 | 2024/02/08 | arm        | 8.0.RC1.B020 | [ait_llm-0.2.1-py3-none-linux_aarch64.whl](https://ais-bench.obs.cn-north-4.myhuaweicloud.com/compare/20240208/ait_llm-0.2.1-py3-none-linux_aarch64.whl) | 1f24783f0815dbca36e8e787a8bfcf09 | [llm大模型推理精度工具功能说明_v0.2.1](../../docs/llm/history/llm大模型推理精度工具功能说明_v0.2.1.md) |
   | 0.2.1 | 2024/02/08 | x86        | 8.0.RC1.B020 | [ait_llm-0.2.1-py3-none-linux_x86_64.whl](https://ais-bench.obs.cn-north-4.myhuaweicloud.com/compare/20240208/ait_llm-0.2.1-py3-none-linux_x86_64.whl) | 679fae6a5b6ea1f4a749b9554f3e5c37 | [llm大模型推理精度工具功能说明_v0.2.1](../../docs/llm/history/llm大模型推理精度工具功能说明_v0.2.1.md) |
   |       |            |            |              |                                                              |                                  |                                                              |
   | 0.2.0 | 2024/01/17 | arm        | 8.0.RC1      | [ait_llm-0.2.0-py3-none-linux_aarch64.whl](https://ais-bench.obs.cn-north-4.myhuaweicloud.com/compare/20240117/ait_llm-0.2.0-py3-none-linux_aarch64.whl) | 99b94bf7edd57b63a6e23b987d24f364 | [llm大模型推理精度工具功能说明_v0.2.0](../../docs/llm/history/llm大模型推理精度工具功能说明_v0.2.0.md) |
```

## Comparing `ms-ait-7.0.0b430/components/llm/setup.py` & `ms-ait-7.0.0rc2/components/llm/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,26 +28,23 @@
 ait_sub_tasks = [{
     "name": "llm",
     "help_info": "Large Language Model(llm) Debugger Tools.",
     "module": "ait_llm.__main__",
     "attr": "get_cmd_instance"
 }]
 
-ait_sub_task_entry_points = [
-    f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
-    for t in ait_sub_tasks
-]
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
     name='ait-llm',
     version='7.0.0c2',
     description='Debug tools for large language model(llm)',
     url='https://gitee.com/ascend/ait/ait/components/llm',
     packages=find_packages(),    
-    package_data={'': ['*.sh', '*.cpp', '*.h', '*.txt']},
+    package_data={'': ['*.sh', '*.cpp', '*.h', 'CMakeLists.txt']},
     license='Apache-2.0',
     keywords='ait_llm',
     install_requires=required,
     classifiers=[
         'Development Status :: Alpha',
         'Intended Audience :: Developers',
         'License :: Apache-2.0 Software License',
```

## Comparing `ms-ait-7.0.0b430/components/llm/__init__.py` & `ms-ait-7.0.0rc2/components/llm/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/install.sh` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/genattentionmask.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-#!/usr/bin/env bash
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-CURRENT_DIR=$(dirname $(readlink -f $0))
 
+import sys
+import os
+import unittest
+import torch
+import torch_npu
 
-build_opchecker_so() {
-    echo ""
-    echo "Try building libatb_speed_torch.so for ait llm. If not using opcheck, ignore errors if any"
-    cd ${CURRENT_DIR}/opcheck/atb_operators
-    bash build.sh
-    cd -
-    echo ""
-}
+from ait_llm.opcheck import operation_test
 
-build_opchecker_so
+
+class OpcheckElewiseSubOperation(operation_test.OperationTest):
+    def golden_calc(self, in_tensors):
+        out = []
+        for i, s in enumerate(self.op_param['seqLen']):
+            for _ in range(self.op_param["headNum"]):
+                out.append(in_tensors[0][i, :, :s, :s].flatten())
+        return [torch.hstack(out)]
+
+    def test_2d_half(self):
+        self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/__init__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/__main__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -207,36 +207,18 @@
             '-mf',
             dest="mapping_file",
             required=False,
             type=check_output_path_legality,
             default='',
             help='Operation mapping file directory.E.g:--op-mapping-file /xx/xxxx/xx')
 
-        parser.add_argument(
-            '--custom-algorithms',
-            '-alg',
-            required=False,
-            nargs='+',
-            help='custom comparing algorithms in format "python_file_path.py:function". \
-                  Should better be a standalong file, and function should in format like \
-                  "def foo(golden_tensor, my_tensor): return float_value, string_message"')
-
     def handle(self, args, **kwargs):
         from ait_llm.compare.torchair_acc_cmp import get_torchair_ge_graph_path
 
         set_log_level(args.log_level)
-
-        # Adding custom comparing algorithms
-        if args.custom_algorithms:
-            from ait_llm.compare.cmp_algorithm import register_custom_compare_algorithm
-
-            for custom_compare_algorithm in args.custom_algorithms:
-                register_custom_compare_algorithm(custom_compare_algorithm)
-
-        # accuracy comparing for different scenarios
         torchair_ge_graph_path = get_torchair_ge_graph_path(args.my_path)
         if torchair_ge_graph_path is not None:
             from ait_llm.compare.torchair_acc_cmp import acc_compare
 
             acc_compare(args.golden_path, args.my_path, args.output, torchair_ge_graph_path)
         else:
             from ait_llm.compare.atb_acc_cmp import acc_compare
@@ -306,31 +288,15 @@
             '-rerun',
             required=False,
             dest="rerun",
             action='store_true',
             default=False,
             help='Rerun atb operations if True. Compare outputs in dump data if False')
 
-        parser.add_argument(
-            '--custom-algorithms',
-            '-alg',
-            required=False,
-            nargs='+',
-            help='custom comparing algorithms in format "python_file_path.py:function". \
-                  Should better be a standalong file, and function should in format like \
-                  "def foo(golden_tensor, my_tensor): return float_value, string_message"')
-
     def handle(self, args, **kwargs):
-        # Adding custom comparing algorithms
-        if args.custom_algorithms:
-            from ait_llm.compare.cmp_algorithm import register_custom_compare_algorithm
-
-            for custom_compare_algorithm in args.custom_algorithms:
-                register_custom_compare_algorithm(custom_compare_algorithm)
-
         op = OpChecker()
         logger.info(f"===================Opcheck start====================")
         op.start_test(args)
         logger.info(f"===================Opcheck end====================")
 
 
 class ErrCheck(BaseCommand):
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/constant.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/constant.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/json_fitter.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/json_fitter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/log.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/log.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/tool.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/tool.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/utils.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/common/validate.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/common/validate.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/compare/atb_acc_cmp.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/compare/atb_acc_cmp.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/compare/cmp_utils.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/compare/cmp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 
 from ait_llm.common.tool import read_atb_data
 from ait_llm.common.constant import TOKEN_ID, DATA_ID, GOLDEN_DATA_PATH, MY_DATA_PATH, CMP_FAIL_REASON, GOLDEN_DTYPE, \
     GOLDEN_SHAPE, GOLDEN_MAX_VALUE, GOLDEN_MIN_VALUE, GOLDEN_MEAN_VALUE, MY_DTYPE, MY_SHAPE, MY_MAX_VALUE, MY_MIN_VALUE, \
     MY_MEAN_VALUE, CSV_GOLDEN_HEADER
 from ait_llm.common.log import logger
-from ait_llm.compare.cmp_algorithm import CMP_ALG_MAP, CUSTOM_ALG_MAP
+from ait_llm.compare.cmp_algorithm import CMP_ALG_MAP
 
 MIN_LAYER_NUMBER = 10
 
 
 class BasicDataInfo:
     count_data_id = 0  # Count data_id, increment by 1 every time creating a new instance
 
@@ -134,15 +134,15 @@
     # 检查tensor的shape是否一致、是否存在NAN或inf
     tensor_pass, message = check_tensor(golden_data_fp32, my_data_fp32)
     if not tensor_pass:
         logger.warning(f"check_tensor failed: {message}")
         row_data[CMP_FAIL_REASON] = message
         return row_data
 
-    for name, cmp_func in list(CMP_ALG_MAP.items()) + list(CUSTOM_ALG_MAP.items()):
+    for name, cmp_func in CMP_ALG_MAP.items():
         result, message = cmp_func(golden_data_fp32, my_data_fp32)
         row_data[name] = result
         if len(message) > 0:
             fail_messages.append(message)
     row_data[CMP_FAIL_REASON] = " ".join(fail_messages)
     return row_data
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/compare/op_mapping.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/compare/op_mapping.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/compare/torchair_acc_cmp.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/compare/torchair_acc_cmp.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/initial.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/initial.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/manual_dump.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/manual_dump.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torchair_dump/torchair_dump.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_config.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/dump_hook.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/dump_hook.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/hook_ops.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/hook_ops.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/topo.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/dump/torch_dump/topo.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/dump/torch_dump/__init__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/repeat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,30 @@
-# Copyright (c) 2024 Huawei Technologies Co., Ltd.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-from ait_llm.dump.torch_dump.dump_config import DumpConfig
-from ait_llm.dump.torch_dump.hook import register_hook
+# Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import sys
+import os
+import unittest
+import torch
+import torch_npu
+
+from ait_llm.opcheck import operation_test
+
+
+class OpcheckRepeatOperation(operation_test.OperationTest):
+    def golden_calc(self, in_tensors):
+        outtensor = in_tensors[0].repeat(self.op_param["multiples"])
+        return [outtensor]
+
+    def test(self):
+        self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/errcheck/process.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/errcheck/process.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/metrics/case_filter.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/case_filter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/metrics/metrics.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/metrics/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,27 +144,26 @@
         filtered_field = []
         
         try:
             filtered_field = [word for word in jieba.cut(word) if word not in self._EXCLUDE_LIST]
         except Exception as e:
             logger.error("Trying to tokenize `%s`, but failed.", word)
             raise
-        
-        if not filtered_field:
-            logger.error("Process terminated due to invalid word value %s, please check if it is well-formatted.", word)
-            raise ValueError("invalid word value.")
-        
-        rate = statistics.mean(
+
+        return 0.0 if not filtered_field else statistics.mean(
             not re.match(self._LEGAL_CHAR_PATTERN, word) for word in filtered_field
         )
 
-        return 0.0001 if rate == 0 else rate
-
     def _compare_two_words(self, word1, word2):
-        return self._quantify_word(word1) / self._quantify_word(word2)
+        ref_rate = self._quantify_word(word2)
+        
+        if ref_rate == 0:
+            return self._quantify_word(word1) / 0.0001
+        
+        return self._quantify_word(word1) / ref_rate
 
     # score <= thr is better, meaning larger score is worse
     def _which_is_better(self, score, thr):
         return score <= thr
 
 
 class BLEU(Metrics):
@@ -265,25 +264,27 @@
                 *(
                         islice((word for word in jieba.cut(word) if word not in self._EXCLUDE_LIST), i, None)
                         for i in range(self._ngrams)
                 )
         ):
             unique.add(contiguous_item)
             count += 1
+
+        if count == 0:
+            return len(unique) / 0.0001
         
-        if not unique:
-            logger.error("Process terminated due to invalid word value %s, please check if it is well-formatted.", word)
-            raise ValueError("invalid word value.")
-        
-        # unique should contain at least one element when entering the loop
-        # count should be greater or equal to 1 when entering the loop
         return len(unique) / count
-    
+
     def _compare_two_words(self, word1, word2):
-        return self._quantify_word(word1) / self._quantify_word(word2)
+        ref_rate = self._quantify_word(word2)
+        
+        if ref_rate == 0:
+            return self._quantify_word(word1) / 0.0001
+
+        return self._quantify_word(word1) / ref_rate
 
     # score >= thr is better, meaning smaller score is worse
     def _which_is_better(self, score, thr):
         return score >= thr
 
 
 @validate_parameters_by_type(
@@ -301,15 +302,15 @@
         "rouge_l": ROUGE(thr, "l"),
         "bleu": BLEU(thr),
         "bleu_1": BLEU(thr, 1),
         "bleu_2": BLEU(thr, 2),
         "bleu_3": BLEU(thr, 3),
         "bleu_4": BLEU(thr, 4),
         "edit_distance": EditDistance(thr),
-        "relative_abnormal": RelativeAbnormalStringRate(thr),
+        "relative_abnormal_string_rate": RelativeAbnormalStringRate(thr),
         "relative_distinct": RelativeDistinctStringRate(thr),
         "relative_distinct_1": RelativeDistinctStringRate(thr, 1),
         "relative_distinct_2": RelativeDistinctStringRate(thr, 2),
         "relative_distinct_3": RelativeDistinctStringRate(thr, 3),
         "relative_distinct_4": RelativeDistinctStringRate(thr, 4),
     }
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/case_manager.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/case_manager.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/opchecker.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/opchecker.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import glob
 import datetime
 import pytz
 import pandas as pd
 import torch
 
 from ait_llm.common.log import logger
-from ait_llm.compare.cmp_algorithm import CUSTOM_ALG_MAP
 
 
 class OpChecker:
     def __init__(self):
         '''
         cases_info结构：
             'op_id': string
@@ -330,66 +329,70 @@
                     logger.info(logger_text)
 
         watching_thread = threading.Thread(target=watching_queue)
         watching_thread.start()
         case_manager.excute_cases()
         watching_thread.join()
 
-    def _update_single_op_result(self, op_info, cur_id, res_detail):
-        default_str = 'NaN'
-        excuted_information = op_info["excuted_information"]
-        required = [
-            op_info["op_id"], op_info["op_name"], op_info["op_param"], op_info["tensor_path"],
-            cur_id, res_detail.get('precision_standard', default_str), excuted_information,
-            res_detail.get('rel_pass_rate', default_str), res_detail.get('max_rel', default_str),
-        ]
+    def get_optional_idx(self):
+        optional_idx = []
         if 'abs' in self.precision_type:
-            required.append(res_detail.get('abs_pass_rate', default_str))
-            required.append(res_detail.get('max_abs', default_str))
+            optional_idx.append(0)
+            optional_idx.append(1)
         if 'cos_sim' in self.precision_type:
-            required.append(res_detail.get('cos_sim', default_str))
+            optional_idx.append(2)
         if 'kl' in self.precision_type:
-            required.append(res_detail.get('kl_div', default_str))
-
-        custom_ret = [res_detail.get(custom_name, default_str) for custom_name in CUSTOM_ALG_MAP]
-        return required + custom_ret + [op_info.get('fail_reason', default_str)]
+            optional_idx.append(3)
+        return optional_idx
 
     def write_op_result_to_csv(self, op_result):
         import openpyxl
 
+        optional_idx = self.get_optional_idx()
         if not os.path.exists(self.output_path):
             wb = openpyxl.Workbook()
             ws = wb.active
             required_head = [
                 'op_id', 'op_name', 'op_param', 'tensor_path', 'out_tensor_id', 'precision_standard',
-                'precision_result', 'rel_precision_rate(%)', 'max_rel_error'
+                'excuted_information', 'precision_result(%)', 'max_rel_error'
             ]
-            if 'abs' in self.precision_type:
-                required_head.append('abs_precision_rate(%)')
-                required_head.append('max_abs_error')
-            if 'cos_sim' in self.precision_type:
-                required_head.append('cosine_similarity')
-            if 'kl' in self.precision_type:
-                required_head.append('kl_divergence')
-            custom_header = list(CUSTOM_ALG_MAP.keys())
-            ws.append(required_head + custom_header + ["fail_reason"])
+            optional_head = ['abs_precision_result(%)', 'max_abs_error', 'cosine_similarity', 'kl_divergence']
+            optional_head_cp = [optional_head[i] for i in optional_idx]
+            ws.append(required_head + optional_head_cp)
             wb.save(self.output_path)
 
         wb = openpyxl.load_workbook(self.output_path)
         ws = wb.active
 
-        op_info = {
-            "op_id": op_result.get('op_id', ""),
-            "op_name": op_result.get('op_name', ""),
-            "op_param": json.dumps(op_result.get('op_param', "")),
-            "tensor_path": op_result.get('tensor_path', ""),
-            "excuted_information": op_result.get('excuted_information', ""),
-            "fail_reason": op_result.get('fail_reason', ""),
-        }
-        
+        op_id = op_result['op_id']
+        op_name = op_result['op_name']
+        op_param = json.dumps(op_result['op_param'])
+        tensor_path = op_result['tensor_path']
+        excuted_information = op_result['excuted_information']
         if len(op_result['res_detail']) > 0:
-            for cur_id, res_detail in enumerate(op_result['res_detail']):
-                ws.append(self._update_single_op_result(op_info, cur_id, res_detail))
+            for i, res_detail in enumerate(op_result['res_detail']):
+                precision_standard = res_detail['precision_standard']
+                rel_pass_rate = res_detail['rel_pass_rate']
+                max_rel = res_detail['max_rel']
+                abs_pass_rate = res_detail['abs_pass_rate']
+                max_abs = res_detail['max_abs']
+                cos_sim = res_detail['cos_sim']
+                kl_div = res_detail['kl_div']
+                required = [
+                    op_id, op_name, op_param, tensor_path, i, precision_standard, excuted_information, rel_pass_rate,
+                    max_rel
+                ]
+                optional = [abs_pass_rate, max_abs, cos_sim, kl_div]
+                optional_cp = [optional[idx] for idx in optional_idx]
+                ws.append(required + optional_cp)
         else:
-            cur_id, res_detail = 'NaN', {}
-            ws.append(self._update_single_op_result(op_info, cur_id, res_detail))
+            default_str = 'NaN'
+            i, precision_standard, rel_pass_rate, max_rel, abs_pass_rate, max_abs, cos_sim, kl_div = default_str, \
+                default_str, default_str, default_str, default_str, default_str, default_str, default_str
+            required = [
+                op_id, op_name, op_param, tensor_path, i, precision_standard, excuted_information, rel_pass_rate,
+                max_rel
+            ]
+            optional = [abs_pass_rate, max_abs, cos_sim, kl_div]
+            optional_cp = [optional[idx] for idx in optional_idx]
+            ws.append(required + optional_cp)
         wb.save(self.output_path)
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/operation_test.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/operation_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import json
 import numpy as np
 import torch
 import torch_npu
 
 from ait_llm.common.tool import read_atb_data
 from ait_llm.common.log import logger
-from ait_llm.compare.cmp_algorithm import CMP_ALG_MAP, CUSTOM_ALG_MAP
+from ait_llm.compare.cmp_algorithm import CMP_ALG_MAP
 
 
 FLOAT_EPSILON = torch.finfo(torch.float).eps
 
 
 class OperationTest(unittest.TestCase):
     def __init__(self, methodName='opTest', case_info=None, excuted_ids=None):
@@ -50,15 +50,15 @@
         error4 = 'Error4‰'
         error5 = 'Error5‰'
         error6 = 'Error+/-1'
 
         self.precision_standard = {
             'torch.double': [error1, 99.99], 'torch.uint32': [error1, 99.99], 'torch.int64': [error1, 99.99],
             'torch.float': [error1, 99.99], 'torch.int32': [error1, 99.99], 'torch.uint64': [error1, 99.99],
-            'torch.float16': [error3, 99.9], 'torch.bfloat16': [error4, 99.6], 'torch.int8': [error6, 99.9],
+            'torch.float16': [error3, 99.9], 'torch.bf16': [error4, 99.6], 'torch.int8': [error6, 99.9],
             'torch.uint8': [error6, 99], 'torch.int16': [error6, 99.9], 'torch.uint16': [error6, 99.9],
             'torch.bool': [error1, 100]
         }
 
         self.erol_dict = {
             error1: 0.0001,
             error2: 0.0005,
@@ -97,16 +97,16 @@
             else:
                 raise RuntimeError(f"{self.tensor_path} not valid")
         else:
             raise RuntimeError(f"{self.tensor_path} not valid")
 
     def tearDown(self):
         self.excuted_ids.put(self.op_id)
-        if self.case_info['excuted_information'] != 'PASS':
-            self.case_info['excuted_information'] = 'FAILED'
+        if self.case_info['excuted_information'] != 'execution successful':
+            self.case_info['excuted_information'] = 'execution failed'
 
     def rerun_op(self, excute_type): 
         operation = torch.classes.OperationTorch.OperationTorch(self.op_name)
         if isinstance(self.op_param, dict):
             operation.set_param(json.dumps(self.op_param))
         elif isinstance(self.op_param, str):
             operation.set_param(self.op_param)
@@ -125,19 +125,14 @@
     def excute_common(self, excute_type):
         logger_text = f"———————— {self.op_id} {self.op_name} test start ————————"
         logger.info(logger_text)
         if self.rerun:
             out_tensors = self.rerun_op(excute_type)
         else:
             out_tensors = self.out_tensors
-        
-        if self.op_name == "AllGatherOperation":
-            rank = self.op_param.get("rank", 0)
-            out_tensors[0] = out_tensors[0][rank]
-
         golden_out_tensors = self.golden_calc(self.in_tensors)
         try:
             logger.debug("out_tensor", out_tensors[0].size())
             logger.debug("golden_out_tensor", golden_out_tensors[0].size())
         except TypeError as e:
             logger_text = "The output is abnormal. Please check! Exception: {}".format(e)
             logger.debug(logger_text)
@@ -174,36 +169,31 @@
             torch.tensor(0, dtype=out.dtype),
         )
         abs_pass_rate = torch.sum(abs_errors <= etol) / size if size != 0 else 0
         max_abs_error = torch.max(abs_errors)
         return abs_pass_rate.item() * 100, max_abs_error.item()
 
     def get_other_precisions(self, out, golden, etol):
-        message = []
         precision_type = self.case_info['precision_type']
         default_str = 'NaN'
         abs_pass_rate, max_abs_error, cos_sim, kl = None, None, None, None
 
         out, golden = out.reshape(-1), golden.reshape(-1)
         if 'abs' in precision_type:
             abs_pass_rate, max_abs_error = self.get_abs_pass_rate(out, golden, etol)
         if 'cos_sim' in precision_type:
-            cos_sim, cur_message = CMP_ALG_MAP["cosine_similarity"](golden, out)
-            if cur_message:
-                message.append('cos_sim: ' + cur_message)
+            cos_sim, _ = CMP_ALG_MAP["cosine_similarity"](golden, out)
         if 'kl' in precision_type:
-            kl, cur_message = CMP_ALG_MAP["kl_divergence"](golden, out)
-            if cur_message:
-                message.append('kl_div: ' + cur_message)
+            kl, _ = CMP_ALG_MAP["kl_divergence"](golden, out)
         abs_pass_rate_str = "%.16f" % float(abs_pass_rate) if abs_pass_rate is not None else default_str
         max_abs_error_str = "%.16f" % float(max_abs_error) if max_abs_error is not None else default_str
         cos_sim_str = "%.10f" % cos_sim if cos_sim is not None else default_str
         kl_div_str = "%.16f" % kl if kl is not None else default_str
 
-        return (abs_pass_rate_str, max_abs_error_str, cos_sim_str, kl_div_str), ", ".join(message)
+        return abs_pass_rate_str, max_abs_error_str, cos_sim_str, kl_div_str
 
     def get_npu_device(self):
         npu_device = os.environ.get("NPU_DEVICE")
         if npu_device is None:
             npu_device = "npu:0"
         else:
             npu_device = f"npu:{npu_device}"
@@ -221,64 +211,50 @@
         current_device = torch.npu.current_device()
         logger_text = "Device Properties: device_name: {}, soc_version: {}, device_count: {}, current_device: {}" \
                     .format(device_name, soc_version, device_count, current_device)
         logger.debug(logger_text)
         return soc_version
 
     def __golden_compare_all(self, out_tensors, golden_out_tensors):
-        message, pass_flag = [], True
+        flag = True
 
-        my_data_len, golden_data_len = len(out_tensors), len(golden_out_tensors)
-        if my_data_len != golden_data_len:
-            pass_flag = False
-            logger.info(f"Data count not equal, {my_data_len} != {golden_data_len}. Will compare only partial")
+        try:
+            self.assertEqual(len(out_tensors), len(golden_out_tensors))
+        except AssertionError as e:
+            flag = False
+            logger.debug(e)
 
         tensor_count = len(out_tensors)
-        for out_tensor, golden_out_tensor in zip(out_tensors, golden_out_tensors):
-            out_dtype = str(out_tensor.dtype)
+        for i in range(tensor_count):
+            out_dtype = str(out_tensors[i].dtype)
             p_s = self.precision_standard.get(out_dtype, [])
             if len(p_s) != 2:
-                cur_message = f"{out_dtype} not supported!"
-                self.case_info['fail_reason'] = cur_message
-                raise RuntimeError(cur_message)
-
+                raise RuntimeError(f"{out_dtype} not supported!")
             etol = self.erol_dict.get(p_s[0], 0.001)
             err_rate = p_s[1]
             ps_standard = f"{err_rate}%(error<{etol})"
 
-            rel_pass_rate, max_rel = self.get_rel_pass_rate(out_tensor, golden_out_tensor, etol)
+            rel_pass_rate, max_rel = self.get_rel_pass_rate(out_tensors[i], golden_out_tensors[i], etol)
 
-            if err_rate >= rel_pass_rate:
-                pass_flag = False
-                cur_message = f"relative pass rate: {rel_pass_rate} not met standart: {err_rate}."
-                message.append(cur_message)
-                logger.debug(cur_message)
+            try:
+                self.assertLess(err_rate, rel_pass_rate)
+            except AssertionError as e:
+                flag = False
+                logger.debug(e)
 
             rel_pass_rate = "%.16f" % float(rel_pass_rate)
             max_rel = "%.16f" % float(max_rel)
-            (abs_pass_rate, max_abs, cos_sim, kl_div), cur_message = self.get_other_precisions(
-                out_tensor, golden_out_tensor, etol
-            )
-            if cur_message:
-                message.append(cur_message)
-
-            cur_result = {
-                "precision_standard": ps_standard,
-                "rel_pass_rate": rel_pass_rate,
-                "max_rel": max_rel,
-                "abs_pass_rate": abs_pass_rate,
-                "max_abs": max_abs,
-                "cos_sim": cos_sim,
-                "kl_div": kl_div,
-            }
-            for name, compare_func in CUSTOM_ALG_MAP.items():
-                cur_result[name], cur_message = compare_func(golden_out_tensor, out_tensor)
-                if cur_message:
-                    message.append(f"{name}: {cur_message}")
-            self.case_info['res_detail'].append(cur_result)
-
-            if pass_flag:
-                self.case_info['excuted_information'] = 'PASS'
-                
+            abs_pass_rate, max_abs, cos_sim, kl_div = self.get_other_precisions(out_tensors[i], golden_out_tensors[i], 
+                                                                                etol)
+
+            self.case_info['res_detail'].append({"precision_standard": ps_standard,
+                                                "rel_pass_rate": rel_pass_rate,
+                                                "max_rel": max_rel,
+                                                "abs_pass_rate": abs_pass_rate,
+                                                "max_abs": max_abs,
+                                                "cos_sim": cos_sim,
+                                                "kl_div": kl_div})
+
+            if flag:
+                self.case_info['excuted_information'] = 'execution successful'
             else:
-                self.case_info['excuted_information'] = 'FAILED'
-            self.case_info['fail_reason'] = ", ".join(message)
+                self.case_info['excuted_information'] = 'execution failed'
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/atb_operators/operation_factory.h`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_gather.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_gather.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+import json
+import unittest
+import sys
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
 
 
 class OpcheckAllGatherOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
         golden_result = torch.stack(in_tensors, dim=0)
         return [golden_result]        
 
     def test_all_gather(self):
-        self.execute()
+        self.excute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/all_reduce.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/all_reduce.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+import json
+import unittest
+import sys
+import socket
+import random
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
 from ait_llm.common.log import logger
 
 
@@ -47,20 +52,26 @@
             result = torch.min(result, in_tensors[i])
         return [result]
 
     def prod_cal(self, in_tensors):
         result = in_tensors[0]
         for i in range(1, len(in_tensors)):
             result = torch.mul(result, in_tensors[i])
-        return [result] 
+        return [result]
 
     def golden_calc(self, in_tensors):
-        all_reduce_type = self.op_param.get('allReduceType', None)
-        backend = self.op_param.get('backend', None)
-                    
+        all_reduce_type = self.op_param['allReduceType']
+        backend = self.op_param['backend']
+        logger_text1 = f"backend: {backend}, allreduceType: {all_reduce_type}"
+        logger_text2 = "env: {}".format(os.getenv("LCCL_DETERMINISTIC"))
+        logger_text3 = "env: {}".format(os.getenv("HCCL_DETERMINISTIC"))
+        logger.debug(logger_text1)
+        logger.debug(logger_text2)
+        logger.debug(logger_text3)
+        
         if all_reduce_type == "sum":
             if backend == "lccl":
                 golden = self.lccl_sum_cal(in_tensors)
             else:
                 golden = self.sum_cal(in_tensors)
         elif all_reduce_type == "max":
             golden = self.max_cal(in_tensors)
@@ -68,22 +79,8 @@
             golden = self.min_cal(in_tensors)
         elif all_reduce_type == "prod":
             golden = self.prod_cal(in_tensors)
 
         return golden
 
     def test_all_reduce(self):
-        all_reduce_type = self.op_param.get('allReduceType', None)
-        backend = self.op_param.get('backend', None)
-
-        logger_text1 = f"backend: {backend}, allreduceType: {all_reduce_type}"
-        logger_text2 = "env: {}".format(os.getenv("LCCL_DETERMINISTIC", ""))
-        logger_text3 = "env: {}".format(os.getenv("HCCL_DETERMINISTIC", ""))
-        logger.debug(logger_text1)
-        logger.debug(logger_text2)
-        logger.debug(logger_text3)
-
-        if all_reduce_type is None or backend is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/as_strided.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fill.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,33 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckAsStridedOperation(operation_test.OperationTest):
+class OpcheckFillOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        size = self.op_param.get('size', None)
-        stride = self.op_param.get('stride', None)
-        offset = self.op_param.get('offset', None)
-        
-        golden_result = torch.as_strided(in_tensors[0], size, stride, offset[0])
+        if self.op_param["withMask"]:
+            golden_result = in_tensors[0].masked_fill_(in_tensors[1], self.op_param["value"][0])
+        else:
+            golden_result = torch.full(self.op_param["outDim"], self.op_param["value"][0], dtype=torch.float16)
         return [golden_result]
 
     def test(self):
-        size = self.op_param.get('size', None)
-        stride = self.op_param.get('stride', None)
-        offset = self.op_param.get('offset', None)
-
-        if size is None or stride is None or offset is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/broadcast.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/where.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,29 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
-import torch.distributed as dist
-import torch.multiprocessing as mp
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckBroadcastOperation(operation_test.OperationTest):
+class OpcheckWhereOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        rank_root = self.op_param.get('rankRoot', None)
-        golden_result = in_tensors[rank_root]
+        golden_result = torch.where(in_tensors[0].bool(), in_tensors[1], in_tensors[2])
         return [golden_result]
 
-    def test_broadcast(self):
-        rank_root = self.op_param.get('rankRoot', None)
-        if rank_root is None:
-            msg = "Cannot get golden data because rankRoot is not correctly set!"
-            logger.error(msg)
-            return
+    def test(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/concat.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/concat.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckConcatOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        concat_dim = self.op_param.get("concatDim", None)
+        concat_dim = self.op_param["concatDim"]
         axis_num = concat_dim if concat_dim >= 0 else concat_dim + len(in_tensors[0].size())
         golden_result = torch.cat(in_tensors, axis=axis_num)
         return [golden_result]
 
     def test(self):
-        concat_dim = self.op_param.get("concatDim", None)
-        if concat_dim is None:
-            msg = "Cannot get golden data because concatDim is not correctly set!"
-            logger.error(msg)
-            return
-        self.execute()
+        self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/cumsum.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/split.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,27 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckCumsumOperation(operation_test.OperationTest):
+class OpcheckAddOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        axes = self.op_param.get("axes", None)
-        golden_result = torch.cumsum(in_tensors[0], dim=axes[0])
-        return [golden_result]
+        split_output = torch.chunk(in_tensors[0], chunks=self.op_param['splitNum'], dim=self.op_param['splitDim'])
+        return split_output
 
     def test(self):
-        axes = self.op_param.get("axes", None)
-        if axes is None:
-            msg = "Cannot get golden data because axes is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmax.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,39 +8,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckFastSoftMaxOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
         data_input = in_tensors[0]
-        seq_len_list = self.op_param.get('qSeqLen', None)
-        head_num_imm = self.op_param.get('headNum', None)
+        seq_len_list = self.op_param['qSeqLen']
+        head_num_imm = self.op_param['headNum']
         golden = torch.empty_like(data_input)
 
         start = 0
         for seq_len in seq_len_list:
             end = start + head_num_imm * seq_len * seq_len
             cur_data_input = data_input[start:end].reshape(-1, seq_len)
             cur_golden = torch.softmax(cur_data_input.to(torch.float32), dim=-1).to(torch.float16)
             golden[start:end] = cur_golden.reshape(-1)
             start = end
         return [golden]
 
     def test_fastsoftmax(self):
-        seq_len_list = self.op_param.get('qSeqLen', None)
-        head_num_imm = self.op_param.get('headNum', None)
-        if seq_len_list is None or head_num_imm is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/fastsoftmaxgrad.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
 
 
@@ -40,15 +43,15 @@
         y_grad_list = []
         golden_list = []
         for i in range(seq_len.shape[0]):
             yi, yg, gd = gen_softmax_grad(head_num_imm, seq_len[i])
             y_input_list.append(yi.reshape(-1))
             y_grad_list.append(yg.reshape(-1))
             golden_list.append(gd.reshape(-1))
-        y_input = torch.concat(y_input_list)
-        y_grad = torch.concat(y_grad_list)
-        golden = torch.concat(golden_list)
+        y_input = torch.cat(y_input_list)
+        y_grad = torch.cat(y_grad_list)
+        golden = torch.cat(golden_list)
 
         return [golden]
 
     def test_fastsoftmaxgrad(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/fill.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reduce.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,35 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckFillOperation(operation_test.OperationTest):
+class OpcheckReduceOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        with_mask = self.op_param.get("withMask", None)
-        out_dim = self.op_param.get("out_dim", None)
-        value = self.op_param.get("value", None)
-
-        if with_mask:
-            golden_result = in_tensors[0].masked_fill_(in_tensors[1], value[0])
-        else:
-            golden_result = torch.full(out_dim, value[0], dtype=torch.float16)
-        return [golden_result]
+        op_type = self.op_param['reduceType']
+        axis = self.op_param['axis']
+        return [in_tensors[0].amax(axis)[0]] if op_type == 1 else [in_tensors[0].amin(axis)[0]]
 
     def test(self):
-        with_mask = self.op_param.get("withMask", None)
-        out_dim = self.op_param.get("out_dim", None)
-        value = self.op_param.get("value", None)
-        if with_mask is None or out_dim is None or value is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/gather.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/gather.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
 from ait_llm.common.log import logger
 
 
 class OpcheckGatherOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        axis = self.op_param.get("axis", None)
+        axis = self.op_param["axis"]
         if axis == 0:
             if in_tensors[0].ndim == 2 and in_tensors[0].ndim == 2:
                 embedding = torch.nn.Embedding(in_tensors[0].shape[0], in_tensors[0].shape[1])
                 embedding.weight.data.copy_(in_tensors[0])
                 embedding.weight.requires_grad = False
                 golden_result = embedding(in_tensors[1].cpu()).detach()
                 return [golden_result.npu()]
@@ -53,13 +56,8 @@
                 for k in range(0, dim2):
                     golden_result_np[idx] = input_flatten[input_idx + indice * dim2 + k]
                     idx += 1
         golden_result = torch.from_numpy(golden_result_np).reshape(output_size)
         return [golden_result.npu()]
 
     def test(self):
-        axis = self.op_param.get("axis", None)
-        if axis is None:
-            msg = "Cannot get golden data because axis is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/genattentionmask.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/pad.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,32 +8,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
+import numpy as np
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckElewiseSubOperation(operation_test.OperationTest):
+class OpcheckPadOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        out = []
-        seq_len = self.op_param.get("seqLen", None)
-        head_num = self.op_param.get("headNum", None)
-        for i, s in enumerate(seq_len):
-            for _ in range(head_num):
-                out.append(in_tensors[0][i, :, :s, :s].flatten())
-        return [torch.hstack(out)]
-
-    def test_2d_half(self):
-        seq_len = self.op_param.get("seqLen", None)
-        head_num = self.op_param.get("headNum", None)
-        if seq_len is None or head_num is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
+        tmp_out = in_tensors[0]
+        padding_offset = in_tensors[1]
+        seq_len = in_tensors[2]
+        input_ids = in_tensors[3]
+        batch = input_ids.shape[0]
+        hidden_dim = tmp_out.shape[1]
+        max_seq_len = input_ids.shape[1]
+ 
+        golden_result = np.zeros((batch, hidden_dim)).astype(np.float16)
+        temp_val = 0
+        for i in range(batch):
+            temp_val = temp_val + seq_len[i][0]
+            golden_result[i] = tmp_out[temp_val - 1]
+        golden_result = torch.from_numpy(golden_result)
+        return [golden_result]
+    
+    def test(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/kv_cache.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/kv_cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+import sys
+import os
+import time
+import json
+import unittest
 import torch
 import torch_npu
+import numpy as np
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckKvCacheOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
         golden = []
-        inplace_idx = self.case_info.get("inplace_idx", None)
-        for index in inplace_idx:
+        for index in self.case_info['inplace_idx']:
             golden.append(in_tensors[index])
         return golden
 
     def test(self):
-        inplace_idx = self.case_info.get("inplace_idx", None)
-        if inplace_idx is None:
-            msg = "Cannot get golden data because inplace_idx is not correctly set!"
-            logger.error(msg)
-            return
         self.execute_inplace()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/layer_norm.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/layer_norm.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,80 +8,80 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
 from ait_llm.common.log import logger
 
 
 class OpcheckLayerNormOperation(operation_test.OperationTest):
     def layer_norm_quant(self, layer_norm_res, quant_scale, quant_offset):
-        golden_result_quant = layer_norm_res * quant_scale + quant_offset
+        golden_result_quant = (layer_norm_res * quant_scale + quant_offset).float()
         golden_result_quant = torch.round(golden_result_quant)
         golden_result_quant = torch.clamp(golden_result_quant, -128, 127)
-        return golden_result_quant
+        return golden_result_quant.type(torch.int8)
 
     def golden_calc(self, in_tensors):
-        layer_type = self.op_param.get('layerType', None)
+        layer_type = self.op_param['layerType']
         if layer_type == 1:
-            cur_param = self.op_param.get('normParam', None)
+            cur_param = self.op_param['normParam']
         elif layer_type == 3:
-            cur_param = self.op_param.get('postNormParam', None)
+            cur_param = self.op_param['postNormParam']
         else:
             raise ValueError('layerType should be 1 or 3')
-        
-        eps = cur_param.get('epsilon', 1e-5)
-        is_quant = cur_param.get('quantType', 0)
-        quant_scale = cur_param.get('quantInputScale', 1)
-        quant_offset = cur_param.get('quantInputOffset', 0)
-        quant_alpha = cur_param.get('quantInputAlpha', 1)
+
+        eps = cur_param['epsilon'] if 'epsilon' in cur_param.keys() else 1e-5
+        is_quant = cur_param['quantType'] != 0 if "quantType" in cur_param.keys() else False
+        quant_scale = cur_param['quantInputScale'] if 'quantInputScale' in cur_param.keys() else 1
+        quant_offset = cur_param['quantInputOffset'] if 'quantInputOffset' in cur_param.keys() else 0
+        quant_alpha = cur_param['quantInputAlpha'] if 'quantInputAlpha' in cur_param.keys() else 1
 
         if not is_quant:
             if layer_type == 1:
-                op_input = in_tensors[0]
-                weight = in_tensors[1]
-                bias = in_tensors[2]
-                axis = cur_param.get('beginNormAxis', 0)
+                op_input = in_tensors[0].float()
+                weight = in_tensors[1].float()
+                bias = in_tensors[2].float()
+                axis = cur_param['beginNormAxis'] if 'beginNormAxis' in cur_param.keys() else 0
                 normalized_shape = in_tensors[0].shape[axis:]
                 golden_result = torch.nn.functional.layer_norm(op_input, normalized_shape, weight, bias, eps)
             elif layer_type == 3:
-                weight = in_tensors[2]
-                bias = in_tensors[3]
+                weight = in_tensors[2].float()
+                bias = in_tensors[3].float()
                 normalized_shape = (1, in_tensors[0].shape[-1])
-                zoom_scale_value = cur_param.get('zoomScale', 1)
-                op_input = torch.add(in_tensors[0], zoom_scale_value * in_tensors[1])
+                zoom_scale_value = cur_param['zoomScale'] if 'zoomScale' in cur_param.keys() else 1
+                op_input = torch.add(in_tensors[0].float(), zoom_scale_value * in_tensors[1].float())
                 golden_result = torch.nn.functional.layer_norm(op_input, normalized_shape, weight, bias, eps)
             golden = [golden_result.half()] if in_tensors[0].dtype == torch.float16 else [golden_result]
         else:
             if layer_type == 1:
-                op_input = in_tensors[0]
-                weight = in_tensors[1]
-                bias = in_tensors[2]                    
+                op_input = in_tensors[0].float()
+                weight = in_tensors[1].float()
+                bias = in_tensors[2].float()                    
                 normalized_shape = (1, in_tensors[0].shape[-1])
                 layer_norm_res = torch.nn.functional.layer_norm(op_input, normalized_shape, weight, bias, eps)
-                golden_result = layer_norm_res * quant_alpha
+                layer_norm_res = layer_norm_res.to(torch.float16)
+                golden_result = (layer_norm_res * quant_alpha).to(torch.float16)
                 golden_result_quant = self.layer_norm_quant(layer_norm_res, quant_scale, quant_offset)
             elif layer_type == 3:
-                weight = in_tensors[2]
-                bias = in_tensors[3]
+                weight = in_tensors[2].float()
+                bias = in_tensors[3].float()
                 normalized_shape = (1, in_tensors[0].shape[-1])                
-                op_input = torch.add(in_tensors[0], in_tensors[1])
+                op_input = torch.add(in_tensors[0].float(), in_tensors[1].float())
                 layer_norm_res = torch.nn.functional.layer_norm(op_input, normalized_shape, weight, bias, eps)
-                golden_result = (layer_norm_res * quant_alpha)
+                layer_norm_res = layer_norm_res.to(torch.float16)
+                golden_result = (layer_norm_res * quant_alpha).to(torch.float16)
                 golden_result_quant = self.layer_norm_quant(layer_norm_res, quant_scale, quant_offset)
             golden = [golden_result, golden_result_quant]        
 
         return golden
 
     def test(self):
-        layer_type = self.op_param.get('layerType', None)
-        if layer_type is None:
-            msg = "Cannot get golden data because layerType is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_parallel.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/cumsum.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
-import torch.distributed as dist
 
 from ait_llm.opcheck import operation_test
 
 
-class OpcheckLinearParallelOperation(operation_test.OperationTest):
+class OpcheckCumsumOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        golden_result = torch.matmul(in_tensors[0], in_tensors[1])
-        dist.all_reduce(golden_result, op=ReduceOp.SUM)
-        torch.npu.synchronize()
-        if len(in_tensors) >= 2 and in_tensors[2] is not None:
-            golden_result = golden_result + in_tensors[2]
+        golden_result = torch.cumsum(in_tensors[0], dim=self.op_param['axes'][0])
         return [golden_result]
 
     def test(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/linear_sparse.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_sparse.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,57 +8,63 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+import sys
+import json
+import unittest
 import torch
 import torch_npu
+import numpy as np
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckLinearSparseOperation(operation_test.OperationTest):
     def golden_quant(self, transpose_a: bool, transpose_b: bool, in_tensors):
         in_tensor_0 = in_tensors[0]
         in_tensor_1 = in_tensors[1]
         in_tensor_2 = in_tensors[2] 
         in_tensor_3 = in_tensors[3]
         if transpose_a:
             if len(in_tensor_0.shape) == 2:
-                in_tensor_0 = torch.permute(in_tensor_0, (1, 0))
+                in_tensor_0 = np.transpose(in_tensor_0, (1, 0))
             if len(in_tensor_0.shape) == 3:
-                in_tensor_0 = torch.permute(in_tensor_0, (0, 2, 1))
+                in_tensor_0 = np.transpose(in_tensor_0, (0, 2, 1))
+            in_tensor_0 = np.ascontiguousarray(in_tensor_0)
         if len(in_tensor_1.shape) == 4:
-            in_tensor_1 = torch.permute(in_tensor_1, (0, 2, 1, 3))
+            in_tensor_1 = np.transpose(in_tensor_1, (0, 2, 1, 3))
             if in_tensor_1.shape[0] == 1:
                 in_tensor_1 = in_tensor_1.reshape(in_tensor_1.shape[1], in_tensor_1.shape[2] * in_tensor_1.shape[3])
             else:
                 in_tensor_1 = in_tensor_1.reshape(in_tensor_1.shape[0], in_tensor_1.shape[1],
                                                   in_tensor_1.shape[2] * in_tensor_1.shape[3])
+            in_tensor_1 = np.ascontiguousarray(in_tensor_1)
         if transpose_b:
             if len(in_tensor_1.shape) == 2:
-                in_tensor_1 = torch.permute(in_tensor_1, (1, 0))
+                in_tensor_1 = np.transpose(in_tensor_1, (1, 0))
             if len(in_tensor_1.shape) == 3:
-                in_tensor_1 = torch.permute(in_tensor_1, (0, 2, 1))
-        golden_result = torch.matmul(in_tensor_0, in_tensor_1)
+                in_tensor_1 = np.transpose(in_tensor_1, (0, 2, 1))
+            in_tensor_1 = np.ascontiguousarray(in_tensor_1)
+        golden_result = np.matmul(in_tensor_0.astype(np.int32), in_tensor_1.astype(np.int32))
         golden_result = golden_result + in_tensor_2
         golden_result = golden_result * in_tensor_3
+        golden_result = golden_result.astype(np.float16)
         return golden_result
 
     def golden_calc(self, in_tensors):
-        transpose_a = self.op_param.get("transposeA", None)
-        transpose_b = self.op_param.get("transposeB", None)
+        transpose_a = self.op_param["transposeA"]
+        transpose_b = self.op_param["transposeB"]
+        in_tensors[0] = in_tensors[0].cpu().numpy()
+        in_tensors[1] = in_tensors[1].cpu().numpy()
+        in_tensors[2] = in_tensors[2].cpu().numpy()
+        in_tensors[3] = in_tensors[3].cpu().numpy()
         golden_result = self.golden_quant(transpose_a, transpose_b, in_tensors)
         golden_result = torch.tensor(golden_result).half()
-        return [golden_result]
+        return [golden_result.npu()]
 
     def test(self):
-        transpose_a = self.op_param.get("transposeA", None)
-        transpose_b = self.op_param.get("transposeB", None)
-        if transpose_a is None or transpose_b is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.excute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/matmul.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/matmul.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,52 +8,55 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+import sys
+import json
+import unittest
 import torch
 import torch_npu
 import numpy as np
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckMatmulOperation(operation_test.OperationTest):
     def golden_flp(self, transpose_a: bool, transpose_b: bool, in_tensor_0, in_tensor_1):
         if transpose_a:
             if len(in_tensor_0.shape) == 2:
-                in_tensor_0 = torch.permute(in_tensor_0, (1, 0))
+                in_tensor_0 = np.transpose(in_tensor_0, (1, 0))
             if len(in_tensor_0.shape) == 3:
-                in_tensor_0 = torch.permute(in_tensor_0, (0, 2, 1))
+                in_tensor_0 = np.transpose(in_tensor_0, (0, 2, 1))
+            in_tensor_0 = np.ascontiguousarray(in_tensor_0)
         if len(in_tensor_1.shape) == 4:
-            in_tensor_1 = torch.permute(in_tensor_1, (0, 2, 1, 3))
+            in_tensor_1 = np.transpose(in_tensor_1, (0, 2, 1, 3))
             if in_tensor_1.shape[0] == 1:
                 in_tensor_1 = in_tensor_1.reshape(in_tensor_1.shape[1], in_tensor_1.shape[2] * in_tensor_1.shape[3])
             else:
                 in_tensor_1 = in_tensor_1.reshape(in_tensor_1.shape[0], in_tensor_1.shape[1],
                                                   in_tensor_1.shape[2] * in_tensor_1.shape[3])
+            in_tensor_1 = np.ascontiguousarray(in_tensor_1)
         if transpose_b:
             if len(in_tensor_1.shape) == 2:
-                in_tensor_1 = torch.permute(in_tensor_1, (1, 0))
+                in_tensor_1 = np.transpose(in_tensor_1, (1, 0))
             if len(in_tensor_1.shape) == 3:
-                in_tensor_1 = torch.permute(in_tensor_1, (0, 2, 1))
-        golden_result = torch.matmul(in_tensor_0, in_tensor_1)
+                in_tensor_1 = np.transpose(in_tensor_1, (0, 2, 1))
+            in_tensor_1 = np.ascontiguousarray(in_tensor_1)
+        golden_result = np.matmul(in_tensor_0.astype(np.float32), in_tensor_1.astype(np.float32))
+        golden_result = golden_result.astype(np.float16)
         return golden_result
 
     def golden_calc(self, in_tensors):
-        transpose_a = self.op_param.get("transposeA", None)
-        transpose_b = self.op_param.get("transposeB", None)
+        transpose_a = self.op_param["transposeA"]
+        transpose_b = self.op_param["transposeB"]
+        in_tensors[0] = in_tensors[0].cpu().numpy()
+        in_tensors[1] = in_tensors[1].cpu().numpy()
         golden_result = self.golden_flp(transpose_a, transpose_b, in_tensors[0], in_tensors[1])
         golden_result = torch.tensor(golden_result).half()
-        return [golden_result]
+        return [golden_result.npu()]
 
     def test(self):
-        transpose_a = self.op_param.get("transposeA", None)
-        transpose_b = self.op_param.get("transposeB", None)
-        if transpose_a is None or transpose_b is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/multinomial.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/multinomial.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,44 +8,39 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import ctypes
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckMultinomialOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        samples = self.op_param.get("numSamples", None)
-        rand_seed = self.op_param.get("randSeed", None)
-        input0 = in_tensors[0]
-        libc = ctypes.CDLL("libc.so.6")
+        samples = self.op_param["numSamples"]
+        rand_seed = self.op_param["randSeed"]
+        input0 = in_tensors[0].cpu().numpy()
+        libc = CDLL("libc.so.6")
         libc.srand(rand_seed)
         rand_list = [libc.rand() / 0x7fffffff for i in range(64)]
-        ret = torch.zeros(shape=(input0.shape[0], samples))
+        ret = np.zeros(shape=(input0.shape[0], samples))
 
-        sum_list = torch.cumsum(input0, axis=-1)
+        sum_list = np.cumsum(input0, axis=-1, dtype=np.float16).astype(np.float16)
         iter_list = [(j, i) 
                     for j in range(input0.shape[0]) 
                     for i in range(input0.shape[1])]
         for z in range(samples):
             for j, i in iter_list:
                 if (sum_list[j][i] > rand_list[z]):
                     ret[j][z] = i
                     break
-        return [ret.contiguous()]
+        return [torch.from_numpy(ret.astype(np.int32)).contiguous()]
 
     def test(self):
-        samples = self.op_param.get("numSamples", None)
-        rand_seed = self.op_param.get("randSeed", None)
-        if samples is None or rand_seed is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/pad.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/set_value.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,32 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import json
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
 
 
-class OpcheckPadOperation(operation_test.OperationTest):
+class OpcheckSetValueOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        tmp_out = in_tensors[0]
-        padding_offset = in_tensors[1]
-        seq_len = in_tensors[2]
-        input_ids = in_tensors[3]
-        batch = input_ids.shape[0]
-        hidden_dim = tmp_out.shape[1]
-        max_seq_len = input_ids.shape[1]
-
-        golden_result = torch.zeros((batch, hidden_dim))
-        temp_val = 0
-        for i in range(batch):
-            temp_val = temp_val + seq_len[i][0]
-            golden_result[i] = tmp_out[temp_val - 1]
-        return [golden_result]
+        golden_result = [in_tensors[0].clone(), in_tensors[1].clone()]
+        for i in range(len(self.op_param["starts"])):
+            golden_result[0][self.op_param["starts"][i]:self.op_param["ends"][i]].copy_(in_tensors[1])
+        return golden_result
 
     def test(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/paged_attention.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/as_strided.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,30 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckPagedAttentionAttentionOperation(operation_test.OperationTest):
+class OpcheckAsStridedOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        if 'isSupportAlibi' in self.op_param:
-            is_support_alibi = self.op_param["isSupportAlibi"]
-        else:
-            is_support_alibi = False
-        
-        if is_support_alibi:
-            return [in_tensors[6]]
-        else:
-            return [in_tensors[5]]
+        golden_result = torch.as_strided(in_tensors[0], self.op_param['size'], 
+                                        self.op_param['stride'], self.op_param['offset'][0])
+        return [golden_result]
 
     def test(self):
-        logger_text = f"PagedAttentionOperation is not supported!"
-        logger.error(logger_text)
-        return
+        self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reduce.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/softmax.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,31 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
+import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckReduceOperation(operation_test.OperationTest):
+class OpcheckSoftmaxOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        op_type = self.op_param.get('reduceType', None)
-        axis = self.op_param.get('axis', None)
-        if op_type == 1:
-            return [in_tensors[0].amax(axis)[0]]
-        else:
-            return [in_tensors[0].amin(axis)[0]]
+        softmax_func = torch.nn.Softmax(dim=self.op_param['axes'][0])
+        return [softmax_func(in_tensors[0])]
 
     def test(self):
-        op_type = self.op_param.get('reduceType', None)
-        axis = self.op_param.get('axis', None)
-        if op_type is None or axis is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/repeat.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/broadcast.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+import json
+import unittest
+import sys
+import socket
+import random
 import torch
 import torch_npu
+import torch.distributed as dist
+import torch.multiprocessing as mp
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckRepeatOperation(operation_test.OperationTest):
+class OpcheckBroadcastOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        multiples = self.op_param.get("multiples", None)
-        outtensor = in_tensors[0].repeat(multiples)
-        return [outtensor]
+        rank_root = self.op_param['rankRoot']
+        golden_result = in_tensors[rank_root]
+        return [golden_result]
 
-    def test(self):
-        multiples = self.op_param.get("multiples", None)
-        if multiples is None:
-            msg = "Cannot get golden data because multiples is not correctly set!"
-            logger.error(msg)
-            return
+    def test_broadcast(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
-#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import torch
-import torch_npu
+import logging
+
+logging.raiseExceptions = False
+
 
-from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
+class Scanner:
+    """
+    Scanner类作为扫描器的基类存在，仅定义必要的属性和方法接口。
+    """
+    __slots__ = ['files', 'porting_results', 'name', 'pool_numbers']
 
+    def __init__(self, files):
+        self.files = files
+        self.porting_results = {}
 
-class OpcheckReshapeAndCacheOperation(operation_test.OperationTest):
-    def golden_calc(self, in_tensors):
-        golden = []
-        inplace_idx = self.case_info.get("inplace_idx", None)
-        for index in inplace_idx:
-            golden.append(in_tensors[index])
-        return golden
-
-    def test(self):
-        inplace_idx = self.case_info.get("inplace_idx", None)
-        if inplace_idx is None:
-            msg = "Cannot get golden data because inplace_idx is not correctly set!"
-            logger.error(msg)
-            return
-        self.execute_inplace()
+    def do_scan(self):
+        raise NotImplementedError('{} must implement do_scan method!'.format(self.__class__))
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckUnpadRopeOperation(operation_test.OperationTest):
     def rotate_half(self, x):
         x0, x1 = x.chunk(2, -1)
-        return torch.concat((-x1, x0), dim=x0.ndim - 1)
+        return torch.cat((-x1, x0), dim=x0.ndim - 1)
 
     def golden_func1(self, in_tensors):
         ntoken = in_tensors[0].size()[0]
         seqlen = in_tensors[4].tolist()
         batch = in_tensors[4].shape[0]
         hidden_size = in_tensors[0].size()[1]
         head_size = in_tensors[2].size()[1]
@@ -48,19 +50,19 @@
             q1 = (q1 * cos1) + (self.rotate_half(q1) * sin1)
             k1 = (k1 * cos1) + (self.rotate_half(k1) * sin1)
             q = torch.concat([q0, q1], dim=(q0.ndim - 1)).view(cur_seqlen, hidden_size)
             q_list.append(q)
             k = torch.concat([k0, k1], dim=(k0.ndim - 1)).view(cur_seqlen, hidden_size)
             k_list.append(k)
             offset = next_offset
-        q_sum = torch.concat(tuple(q_list), dim=0)
-        k_sum = torch.concat(tuple(k_list), dim=0)
+        q_sum = torch.cat(tuple(q_list), dim=0)
+        k_sum = torch.cat(tuple(k_list), dim=0)
         del self.unpadRetdata
         return [q_sum, k_sum]
-
+    
     def golden_func2(self, in_tensors):
         ntoken = in_tensors[0].size()[0]
         seqlen = int(in_tensors[4][0])
         batch = ntoken // seqlen
         hidden_size = in_tensors[0].size()[1]
         head_size = in_tensors[2].size()[1]
         head_num = hidden_size // head_size
@@ -83,19 +85,19 @@
             seqlen = in_tensors[0].size()[1]
             batch = in_tensors[0].size()[0]
             q_head_num = in_tensors[0].size()[2]
             k_head_num = in_tensors[1].size()[2]
         else:
             ntoken = in_tensors[0].size()[0]
             seqlen = int(in_tensors[4][0])
-            batch = max(ntoken // seqlen, 1)
+            batch = ntoken // seqlen
             hidden_sizeq = in_tensors[0].size()[1]
             head_size = in_tensors[2].size()[1]
             q_head_num = hidden_sizeq // head_size
-            hidden_sizek = in_tensors[1].size()[1]
+            hidden_sizek = in_tensors[0].size()[1]
             k_head_num = hidden_sizek // head_size
         rot_dim = in_tensors[2].size()[1]
 
         q = in_tensors[0]
         k = in_tensors[1]
         qshaped = q.reshape(batch, -1, q_head_num, rot_dim // 2, 2)
         kshaped = k.reshape(batch, -1, k_head_num, rot_dim // 2, 2)
@@ -139,25 +141,19 @@
         cos = in_tensors[2].view(batch, seqlen, head_size).unsqueeze(2)
         sin = in_tensors[3].view(batch, seqlen, head_size).unsqueeze(2)
         q_embed = ((q * cos) + (self.rotate_half(q) * sin)).view(ntoken, hidden_size)
         k_embed = ((k * cos) + (self.rotate_half(k) * sin)).view(ntoken, hidden_size1)
         return [q_embed, k_embed]
 
     def golden_calc(self, in_tensors):
-        rotary_coeff = self.op_param.get('rotaryCoeff', None)
-        if rotary_coeff == 4:
+        if self.op_param['rotaryCoeff'] == 4:
             if in_tensors[4].size()[0] == 3:
                 return self.golden_func1(in_tensors)
             else:
                 return self.golden_func2(in_tensors)
-        elif rotary_coeff == 64:
+        elif self.op_param['rotaryCoeff'] == 64:
             return self.golden_func3(in_tensors)
         else:
             return self.golden_func4(in_tensors)
 
     def test(self):
-        rotary_coeff = self.op_param.get('rotaryCoeff', None)
-        if rotary_coeff is None:
-            msg = "Cannot get golden data because rotaryCoeff is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/rope_grad.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/rope_grad.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,43 +8,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
+import numpy as np
 import torch
 import torch_npu
 import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckRopeGradOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
         # x,128*32-->reshape x,32,128
-        qseqlen = self.op_param.get('qSeqLen', None)
-        cos_list = [in_tensors[2][:x, :] for x in qseqlen]
-        sin_list = [in_tensors[3][:x, :] for x in qseqlen]
-        cos = torch.concat(cos_list, dim=0)
-        sin = torch.concat(sin_list, dim=0)
+        cos_list = [in_tensors[2][:x, :] for x in self.op_param['qSeqLen']]
+        sin_list = [in_tensors[3][:x, :] for x in self.op_param['qSeqLen']]
+        cos = torch.cat(cos_list, dim=0)
+        sin = torch.cat(sin_list, dim=0)
         sin1 = sin[:, :64]
         sin2 = sin[:, 64:]
-        rohqgsin = torch.concat((sin2, -sin1), dim=-1)
+        rohqgsin = torch.cat((sin2, -sin1), dim=-1)
         q_grad = torch.zeros_like(in_tensors[0])
         bs = int(in_tensors[0].shape[1] / 128)
         for i in range(bs):
             q_grad[:, i * 128:(i + 1) * 128] = in_tensors[0][:, i * 128:(i + 1) * 128] * (cos + rohqgsin)
-
+    
         k_grad = torch.zeros_like(in_tensors[1])
         for i in range(bs):
             k_grad[:, i * 128:(i + 1) * 128] = in_tensors[1][:, i * 128:(i + 1) * 128] * (cos + rohqgsin)
         return [q_grad, k_grad]
 
     def test(self):
-        qseqlen = self.op_param.get('qSeqLen', None)
-        if qseqlen is None:
-            msg = "Cannot get golden data because qSeqLen is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/self_attention.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/self_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,14 @@
         out = torch.concat(context_list, dim=0)
         return out
 
     def encoder_golden_func(self, in_tensors):
         mixed_q, mixed_k, mixed_v, attention_mask, seq_len = in_tensors[0], in_tensors[1], in_tensors[2], \
             in_tensors[3], in_tensors[4]
         
-        dtype = mixed_q.dtype
         batch_run_status_enable = self.op_param.get("batchRunStatusEnable", False)
         if batch_run_status_enable:
             batch_status = in_tensors[5]
         else:
             batch_status = len(seq_len)
 
         heads, group_num, embed = self.op_param.get("headNum", 32), self.op_param.get("kvHeadNum", 32), mixed_k.size(-1)
@@ -115,18 +114,19 @@
             k_slice_t = torch.permute(k_slice, (0, 2, 1))   # get K^T (kv_heads, embed, k_seq)
             v_slice = mixed_v[v_offset:v_offset + kv_s][:].view(kv_s, group_num, embed)
             v_slice = torch.permute(v_slice, (1, 0, 2))
             score = self.group_matmul(heads, group_num, q_slice, k_slice_t)
             s = score.view(-1) if s is None else torch.concat((s, score.view(-1)), 0)
             
             score = score / math.sqrt(1.0 * embed)
-            score_max = torch.max(score, axis=-1).values
+            score = score + attention_mask[:, :q_s, :kv_s] if self.op_param.get("isTriuMask", False) else score
+            score_max = torch.max(score, axis=-1)
             score = score - score_max.view((heads, q_s, 1))
             score_exp = torch.exp(score)
-            if not dtype == torch.float32:
+            if not self.op_param.get("isFp32", True):
                 score_sum = torch.sum(score_exp, axis=-1)
                 _p = score_exp.view(-1) if _p is None else torch.concat((_p, score_exp.view(-1)), 0)
                 p = score_exp / score_sum.view(heads, q_s, 1)
                 out_sub = self.group_matmul(heads, group_num, p, v_slice)
             else:
                 score_sum = torch.sum(score_exp, axis=-1)
                 _p = score_exp.view(-1) if _p is None else torch.concat((_p, score_exp.view(-1)), 0)
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/set_value.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/sort.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,31 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import json
+import unittest
 import torch
 import torch_npu
+import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckSetValueOperation(operation_test.OperationTest):
+class OpcheckSortOperation(operation_test.OperationTest):    
     def golden_calc(self, in_tensors):
-        starts = self.op_param.get("starts", None)
-        ends = self.op_param.get("ends", None)
-        golden_result = [in_tensors[0].clone(), in_tensors[1].clone()]
-        for i, _ in enumerate(starts):
-            golden_result[0][starts[i]:ends[i]].copy_(in_tensors[1])
-        return golden_result
+        values, indices = torch.topk(in_tensors[0], k=self.op_param["num"][0], largest=True)
+        return [values, indices.int()]
 
-    def test(self):
-        starts = self.op_param.get("starts", None)
-        ends = self.op_param.get("ends", None)
-        if starts is None or ends is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
+    def test_3d_float(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/slice.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/slice.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,41 +8,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckSliceOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        offset_list = self.op_param.get('offsets', None)
-        size_list = self.op_param.get('size', None)
+        offset_list = self.op_param['offsets']
+        size_list = self.op_param['size']
         for index, offset in enumerate(offset_list):
             offset_list[index] = offset if offset >= 0 else offset + in_tensors[0].shape[index]
         for index, size in enumerate(size_list):
             size_list[index] = size if size != -1 else in_tensors[0].shape[index] - offset_list[index]
-        if len(offset_list) == 2:
-            return [in_tensors[0][offset_list[0] : offset_list[0] + size_list[0], 
-                    offset_list[1] : offset_list[1] + size_list[1]]]
-        elif len(offset_list) == 3:
+        if len(offset_list) == 3:
             return [in_tensors[0][offset_list[0] : offset_list[0] + size_list[0], 
                     offset_list[1] : offset_list[1] + size_list[1], offset_list[2] : offset_list[2] + size_list[2]]]
         else:
             return [in_tensors[0][offset_list[0] : offset_list[0] + size_list[0], 
                     offset_list[1] : offset_list[1] + size_list[1], offset_list[2] : offset_list[2] + size_list[2], 
                     offset_list[3] : offset_list[3] + size_list[3]]]
 
+
+
     def test(self):
-        offset_list = self.op_param.get('offsets', None)
-        size_list = self.op_param.get('size', None)
-        if offset_list is None or size_list is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/softmax.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/reshape_and_cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
+import math
+import os
+import random
+import sys
+import unittest
+
+import numpy as np
 import torch
 import torch_npu
-import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
-class OpcheckSoftmaxOperation(operation_test.OperationTest):
+class OpcheckReshapeAndCacheOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        axes = self.op_param.get('axes', None)
-        softmax_func = torch.nn.Softmax(dim=axes[0])
-        return [softmax_func(in_tensors[0])]
+        golden = []
+        for index in self.case_info['inplace_idx']:
+            golden.append(in_tensors[index])
+        return golden
 
     def test(self):
-        axes = self.op_param.get('axes', None)
-        if axes is None:
-            msg = "Cannot get golden data because axes is not correctly set!"
-            logger.error(msg)
-            return
-        self.execute()
+        self.execute_inplace()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/topk_topp_sampling.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,55 +8,54 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 from ctypes import CDLL
+import numpy as np
 import torch
 import torch_npu
 import torch.nn as nn
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckToppOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        rand_seed = self.op_param.get('rand_seed', None)
-        topk = self.op_param.get('topk', None)
+        rand_seed = self.op_param["randSeed"]
+        topk = self.op_param["topk"]
         libc = CDLL("libc.so.6")
         libc.srand(rand_seed)
         rand_list = [libc.rand() / 0x7fffffff for i in range(64)]
-
-        probs = in_tensors[0]
-        topp = in_tensors[1]
-        probs_sorted = torch.sort(probs, axis=-1)[..., ::-1][..., :topk]
+ 
+        probs = in_tensors[0].cpu().numpy()
+        topp = in_tensors[1].cpu().numpy()
+        probs_sorted = np.sort(probs, axis=-1)[..., ::-1][..., :topk]
         try:
             probs_div_sorted = probs_sorted / topp
         except ZeroDivisionError as e:
             raise e   
-        indices_sorted = torch.argsort(-probs, kind='mergesort', axis=-1)[..., :topk]
-        probs_sorted_sumed = torch.cumsum(probs_sorted, axis=-1)
-        mask = torch.zeros_like(probs_sorted_sumed, dtype=torch.int32)
+        indices_sorted = np.argsort(-probs, kind='mergesort', axis=-1)[..., :topk]
+        probs_sorted_sumed = np.cumsum(probs_sorted, axis=-1, dtype=np.float16).astype(np.float16)
+        mask = np.zeros_like(probs_sorted_sumed, dtype=np.int32)
         mask[probs_sorted_sumed <= topp] = 1
         probs_div_sorted *= mask
-        probs_div_sorted_sumed = torch.cumsum(probs_div_sorted, axis=-1)
-        multinomial_probs = probs_div_sorted_sumed < rand_list[0]
-        first_true_indeces = torch.argmax(~multinomial_probs, axis=-1)
+        probs_div_sorted_sumed = np.cumsum(probs_div_sorted, axis=-1, dtype=np.float16).astype(np.float16)
+        multinomial_probs = probs_div_sorted_sumed.astype(np.float32) < rand_list[0]
+        first_true_indeces = np.argmax(~multinomial_probs, axis=-1)
         for i in range(probs.shape[0]):
             multinomial_probs[i, first_true_indeces[i]:] = False
-        indices_sorted_sampled = torch.sum(multinomial_probs, axis=-1, keepdims=True)
+        indices_sorted_sampled = np.sum(multinomial_probs, axis=-1, keepdims=True)
         indices_sorted_sampled[indices_sorted_sampled >= topk] = 0
-        indices_sampled = torch.take_along_axis(indices_sorted, indices_sorted_sampled, axis=-1)
-        probs_sampled = torch.take_along_axis(probs_sorted, indices_sorted_sampled, axis=-1)
-        return [indices_sampled, probs_sampled]
+        indices_sampled = np.take_along_axis(indices_sorted, indices_sorted_sampled, axis=-1)
+        probs_sampled = np.take_along_axis(probs_sorted, indices_sorted_sampled, axis=-1)
+        return [torch.from_numpy(indices_sampled.astype(np.int32)),
+                torch.from_numpy(probs_sampled.astype(np.float16))]
 
+    
     def test(self):
-        rand_seed = self.op_param.get('rand_seed', None)
-        topk = self.op_param.get('topk', None)
-        if rand_seed is None or topk is None:
-            msg = "Cannot get golden data because opParam is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transdata.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/transdata.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,120 +8,117 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
 
 from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
 
 
 class OpcheckTransdataOperation(operation_test.OperationTest):
+    def __init__(self):
+        self.align_int8 = 32
+        self.default_align = 16
+    
     @staticmethod
-    def round_up(x, align):
+    def round_up(self, x, align):
         if align == 0:
             return -1
         return (x + align - 1) // align * align
     
     @staticmethod
-    def custom_pad(x, pad_dims):
+    def custom_pad(self, x, pad_dims):
         return torch.nn.functional.pad(x, pad_dims)
-
+    
     @staticmethod
-    def custom_reshape(x, target_shape):
+    def custom_reshape(self, x, target_shape):
         return x.reshape(target_shape)
     
     @staticmethod
-    def custom_transpose(x, dim1, dim2):
+    def custom_transpose(self, x, dim1, dim2):
         return x.transpose(dim1, dim2)
 
+    @staticmethod
     def golden_nd_to_nz_3d(self, in_tensors):
-        align_int8 = 32
-        default_align = 16
-
         aux_dims = [0, 0, 0, 0]
         aux_dims[0] = in_tensors[0].size(0)
-        aux_dims[1] = self.round_up(in_tensors[0].size(1), default_align)
-
+        aux_dims[1] = self.round_up(in_tensors[0].size(1), self.default_align)
+ 
         pad_dims = [0, 0, 0, 0]  
-        pad_dims[3] = self.round_up(in_tensors[0].size(1), default_align) - in_tensors[0].size(1)
-
+        pad_dims[3] = self.round_up(in_tensors[0].size(1), self.default_align) - in_tensors[0].size(1)
+ 
         if in_tensors[0].dtype == torch.int8:
-            aux_dims[2] = self.round_up(in_tensors[0].size(2), align_int8) // align_int8
-            aux_dims[3] = align_int8
-            pad_dims[1] = self.round_up(in_tensors[0].size(2), align_int8) - in_tensors[0].size(2)
+            aux_dims[2] = self.round_up(in_tensors[0].size(2), self.align_int8) // self.align_int8
+            aux_dims[3] = self.align_int8
+            pad_dims[1] = self.round_up(in_tensors[0].size(2), self.align_int8) - in_tensors[0].size(2)
         else:
-            aux_dims[2] = self.round_up(in_tensors[0].size(2), default_align) // default_align
-            aux_dims[3] = default_align
-            pad_dims[1] = self.round_up(in_tensors[0].size(2), default_align) - in_tensors[0].size(2)
+            aux_dims[2] = self.round_up(in_tensors[0].size(2), self.default_align) // self.default_align
+            aux_dims[3] = self.default_align
+            pad_dims[1] = self.round_up(in_tensors[0].size(2), self.default_align) - in_tensors[0].size(2)
         
         return self.custom_transpose(
                     self.custom_reshape(
                         self.custom_pad(in_tensors[0], pad_dims),
                         aux_dims
                     ),
                     1, 2
                 ).contiguous()
-
+ 
+    @staticmethod
     def golden_nd_to_nz_2d(self, in_tensors):
-        align_int8 = 32
-        default_align = 16
-        
         aux_dims = [0, 0, 0, 0]
         aux_dims[0] = 1
-        aux_dims[1] = self.round_up(in_tensors[0].size(0), default_align)
+        aux_dims[1] = self.round_up(in_tensors[0].size(0), self.default_align)
  
         pad_dims = [0, 0, 0, 0]  
-        pad_dims[3] = self.round_up(in_tensors[0].size(0), default_align) - in_tensors[0].size(0)
+        pad_dims[3] = self.round_up(in_tensors[0].size(0), self.default_align) - in_tensors[0].size(0)
  
         if in_tensors[0].dtype == torch.int8:
-            aux_dims[2] = self.round_up(in_tensors[0].size(1), align_int8) // align_int8
-            aux_dims[3] = align_int8
-            pad_dims[1] = self.round_up(in_tensors[0].size(1), align_int8) - in_tensors[0].size(1)
+            aux_dims[2] = self.round_up(in_tensors[0].size(1), self.align_int8) // self.align_int8
+            aux_dims[3] = self.align_int8
+            pad_dims[1] = self.round_up(in_tensors[0].size(1), self.align_int8) - in_tensors[0].size(1)
         else:
-            aux_dims[2] = self.round_up(in_tensors[0].size(1), default_align) // default_align
-            aux_dims[3] = default_align
-            pad_dims[1] = self.round_up(in_tensors[0].size(1), default_align) - in_tensors[0].size(1)
+            aux_dims[2] = self.round_up(in_tensors[0].size(1), self.default_align) // self.default_align
+            aux_dims[3] = self.default_align
+            pad_dims[1] = self.round_up(in_tensors[0].size(1), self.default_align) - in_tensors[0].size(1)
         
         return self.custom_transpose(
                     self.custom_reshape(
                         self.custom_pad(in_tensors[0], pad_dims),
                         aux_dims
                     ),
                     1, 2
                 ).contiguous()
-
+ 
+    @staticmethod
     def golden_nz_to_nd(self, in_tensors, out_crops):
         aux_dims = [0, 0, 0]
         aux_dims[0] = in_tensors[0].size(0)
         aux_dims[1] = in_tensors[0].size(2)
         aux_dims[2] = in_tensors[0].size(1) * in_tensors[0].size(3)
         
+        
         return self.custom_reshape(
                     self.custom_transpose(in_tensors[0], 1, 2),
                     aux_dims
                 )[:, :out_crops[0], :out_crops[1]]
 
     def golden_calc(self, in_tensors):
-        transdata_type = self.op_param.get("transdataType", None)
-        if transdata_type == 2:
+        if self.op_param["transdataType"] == 2:
             if len(in_tensors[0].size()) == 3:
                 golden_result = self.golden_nd_to_nz_3d(in_tensors)
             else:
                 golden_result = self.golden_nd_to_nz_2d(in_tensors)
         else:
-            out_crops = self.op_param.get("outCrops", None)
-            golden_result = self.golden_nz_to_nd(in_tensors, out_crops)
-
+            golden_result = self.golden_nz_to_nd(in_tensors, self.op_param["outCrops"])
+ 
         return [golden_result]
 
     def test(self):
-        transdata_type = self.op_param.get("transdataType", None)
-        if transdata_type is None:
-            msg = "Cannot get golden data because transdataType is not correctly set!"
-            logger.error(msg)
-            return
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/transpose.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cxx_scanner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,53 @@
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
-#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import torch
-import torch_npu
+import time
+import os
+from multiprocessing import Pool
+from app_analyze.utils.log_util import logger
+from app_analyze.scan.scanner import Scanner
+
+
+class CxxScanner(Scanner):
+    def __init__(self, files, cxx_parser=None):
+        super().__init__(files)
+        self.cxx_parser = cxx_parser
+
+    def do_scan(self):
+        start_time = time.time()
+        result = self.exec_without_threads()
+        self.porting_results['cxx'] = result
+        eval_time = time.time() - start_time
+
+        logger.debug(f'Total time for scanning cxx files is {eval_time}s')
 
-from ait_llm.opcheck import operation_test
-from ait_llm.common.log import logger
+    def exec_without_threads(self):
+        result = {}
+        count = max(max(os.cpu_count(), len(self.files)), 16)
+        pool = Pool(count)
+        list_file = []
+        for file in self.files:
+            list_file.append((self.cxx_parser, file))
+        lst = pool.starmap_async(cxx_parser_, list_file)
+        pool.close()
+        pool.join()
+        lst1 = lst.get(timeout=2)
+        for file, r in zip(self.files, lst1):
+            result[file] = r
+        return result
 
 
-class OpcheckTransposeOperation(operation_test.OperationTest):
-    def golden_calc(self, in_tensors):
-        perm = self.op_param.get("perm", None)
-        golden_result = in_tensors[0].permute(perm)
-        return [golden_result]
-
-    def test_2d_float(self):
-        perm = self.op_param.get("perm", None)
-        if perm is None:
-            msg = "Cannot get golden data because perm is not correctly set!"
-            logger.error(msg)
-            return
-        self.execute()
+def cxx_parser_(cxx_parser, files):
+    p = cxx_parser(files)
+    rst_vals = p.parse()
+    return rst_vals
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/unpad.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/unpad.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,42 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+import os
+import unittest
 import torch
 import torch_npu
+import numpy as np
 
 from ait_llm.opcheck import operation_test
 
 
 class OpcheckUnpadOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
         input_ids = in_tensors[0]
         cum_offsets_now = in_tensors[1].reshape(-1)
         token_num = in_tensors[2]
         seq_len = in_tensors[3]
         batch = in_tensors[0].shape[0]
         total_length_imm = in_tensors[0].shape[1]
-
+ 
         x_remove_padding = input_ids[0][0:seq_len[0]]
         for i in range(1, batch):
-            x_remove_padding = torch.concat((x_remove_padding, input_ids[i][0:seq_len[i]]))
-        x_remove_padding = torch.pad(x_remove_padding, (0, (batch * total_length_imm - token_num[0][0])))
-        cum_offsets_out = torch.zeros(batch)
+            x_remove_padding = np.concatenate((x_remove_padding, input_ids[i][0:seq_len[i]]))
+        x_remove_padding = np.pad(x_remove_padding, (0, (batch * total_length_imm - token_num[0][0])))
+        cum_offsets_out = np.zeros(batch)
         for i in range(1, batch):
             cum_offsets_out[i] = cum_offsets_now[i - 1]
         padding_offset = seq_len[0] * [0]
         for i in range(1, batch):
             temp_pad_out = seq_len[i] * [cum_offsets_now[i - 1]]
-            padding_offset = torch.concat((padding_offset, temp_pad_out))
-        zero_offset = torch.zeros((1, batch * total_length_imm - token_num[0][0]))
-        padding_offset = torch.append(padding_offset, zero_offset)
-        x_remove_padding = x_remove_padding.reshape(1, batch * total_length_imm).long()
-        cum_offsets_out = cum_offsets_out.reshape(batch, 1).int()
-        padding_offset = padding_offset.reshape(1, batch * total_length_imm)
+            padding_offset = np.concatenate((padding_offset, temp_pad_out))
+        zero_offset = np.zeros((1, batch * total_length_imm - token_num[0][0]))
+        padding_offset = np.append(padding_offset, zero_offset)
+        x_remove_padding = torch.from_numpy(x_remove_padding.reshape(1, batch * total_length_imm)).long()
+        cum_offsets_out = torch.from_numpy(cum_offsets_out.reshape(batch, 1)).int()
+        padding_offset = torch.from_numpy(padding_offset.reshape(1, batch * total_length_imm).astype(np.int32))
         return [x_remove_padding, cum_offsets_out, padding_offset]
-
+ 
     def test(self): 
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/where.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/linear_parallel.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,20 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+import sys
+import unittest
 import torch
 import torch_npu
+import numpy as np
+import torch.distributed as dist
 
 from ait_llm.opcheck import operation_test
 
 
-class OpcheckWhereOperation(operation_test.OperationTest):
+class OpcheckLinearParallelOperation(operation_test.OperationTest):
     def golden_calc(self, in_tensors):
-        golden_result = torch.where(in_tensors[0].bool(), in_tensors[1], in_tensors[2])
+        golden_result = torch.matmul(in_tensor_0.to(torch.float32), in_tensor_1.to(torch.float32)).to(torch.float16)
+        dist.all_reduce(golden_result, op=ReduceOp.SUM)
+        torch.npu.synchronize()
+        if in_tensors[2] is not None:
+            golden_result = golden_result + in_tensors[2]
+
         return [golden_result]
 
     def test(self):
         self.execute()
```

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/opcheck/check_case/__init__.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/opcheck/check_case/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/transform/transform_quant_cpp_layer_function.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/llm/ait_llm/transform/utils.py` & `ms-ait-7.0.0rc2/components/llm/ait_llm/transform/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/__init__.py` & `ms-ait-7.0.0rc2/components/profile/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/install.sh` & `ms-ait-7.0.0rc2/components/profile/msprof/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/README.md` & `ms-ait-7.0.0rc2/components/profile/msprof/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/setup.py` & `ms-ait-7.0.0rc2/components/profile/msprof/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,33 +17,30 @@
 with open('requirements.txt', encoding='utf-8') as f:
     required = f.read().splitlines()
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 ait_sub_tasks = [{
-    "name": "profile",
+    "name": "msprof",
     "help_info": "get profiling data of a given programma",
     "module": "ait_prof.main_cli",
     "attr": "get_cmd_instance"
 }]
 
-ait_sub_task_entry_points = [
-    f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
-    for t in ait_sub_tasks
-]
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
-    name='ait-profile',
+    name='ait-msprof',
     version='7.0.0c2',
     description='msprof tool',
     long_description=long_description,
     url='ait_msprof url',
     packages=find_packages(),
     keywords='ait_msprof tool',
     install_requires=required,
     python_requires='>=3.7',
     entry_points={
         'ait_sub_task': ait_sub_task_entry_points,
-        'ait_sub_task_installer': ['ait-profile=ait_prof.__install__:MsProfInstall'],
+        'ait_sub_task_installer': ['ait-msprof=ait_prof.__install__:MsProfInstall'],
     }
 )
```

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/api.py` & `ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/api.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/args_adapter.py` & `ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/args_adapter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/main_cli.py` & `ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/main_cli.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/msprof_process.py` & `ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/msprof_process.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/utils.py` & `ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__install__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/common/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 # Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
-#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from components.utils.install import AitInstaller
-
 
-class MsProfInstall(AitInstaller):
-    pass
```

## Comparing `ms-ait-7.0.0b430/components/profile/msprof/ait_prof/__main__.py` & `ms-ait-7.0.0rc2/components/profile/msprof/ait_prof/__main__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/main_cli.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,87 @@
-# Copyright (c) 2024-2024 Huawei Technologies Co., Ltd.
-
+# Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-
-#     http://www.apache.org/licenses/LICENSE-2.0
-
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
 import os
-
-from ait_tensor_view.operation import SliceOperation, PermuteOperation
-from ait_tensor_view.handler import handle_tensor_view
 from components.utils.parser import BaseCommand
+from app_analyze.utils import log_util
+from app_analyze.porting.app import start_scan_kit
 from components.utils.file_open_check import FileStat
 
 
-def check_input_path_legality(value):
-    if not value:
-        return value
-    if not value.endswith(".bin") and not value.endswith(".pth"):
-        raise ValueError("only .bin or .pth file is accepted")
-    try:
-        file_stat = FileStat(value)
-    except Exception as err:
-        raise argparse.ArgumentTypeError(f"input path:{value} is illegal. Please check.") from err
-    if not file_stat.is_basically_legal('read', strict_permission=False):
-        raise argparse.ArgumentTypeError(f"input path:{value} is illegal. Please check.")
-    return value
-
 
-def check_output_path_legality(value):
-    if not value:
-        return value
-    try:
-        file_stat = FileStat(value)
-    except Exception as err:
-        raise argparse.ArgumentTypeError(f"output path:{value} is illegal. Please check.") from err
-    if not file_stat.is_basically_legal("write", strict_permission=False):
-        raise argparse.ArgumentTypeError(f"output path:{value} can not write. Please check.")
+def check_source_path(value):
+    source_list = value.split(',')
+    for path in source_list:
+        path_value = str(path)
+        try:
+            file_stat = FileStat(path_value)
+        except Exception as err:
+            raise argparse.ArgumentTypeError(f"source path:{path_value} is illegal. Please check.") from err
+        if not file_stat.is_basically_legal('read'):
+            raise argparse.ArgumentTypeError(f"source path:{path_value} is illegal. Please check.")
+        if not file_stat.is_dir:
+            raise argparse.ArgumentTypeError(f"source path:{path_value} is not a directory. Please check.")
     return value
 
 
-def parse_operations(value):
-    operations = value.split(";")
-
-    ops = []
-
-    for op in operations:
-        if op.startswith("[") and op.endswith("]"):
-            ops.append(SliceOperation(op))
-        elif op.startswith("(") and op.endswith(")"):
-            ops.append(PermuteOperation(op))
-        else:
-            raise SyntaxError(f"Invalid operation string: {op}")
-
-    return ops
-
-
-def get_args():
-    parser = argparse.ArgumentParser()
-
-    return parser.parse_args()
-
-
-class TensorViewCommand(BaseCommand):
+class TranspltCommand(BaseCommand):
     def add_arguments(self, parser):
+        # 逗号分隔的情况下只有一个列表元素
         parser.add_argument(
-            "--bin", "-b",
-            type=check_input_path_legality,
-            required=True,
-            help="Bin file path"
+            "-s", "--source", type=check_source_path, required=True, help="directories of source folder"
         )
-
         parser.add_argument(
-            "--print", "-p",
-            action="store_true",
-            help="print tensor"
+            "-f",
+            "--report-type",
+            default='csv',
+            choices=['csv', 'json'],
+            help="specify output report type. Only csv(xlsx)/json is supported",
         )
-
         parser.add_argument(
-            "--output", "-o",
-            type=check_output_path_legality,
-            help="where the tensor should be saved (default: current directory)"
+            "--log-level", default="INFO", choices=['DEBUG', 'INFO', 'WARNING', 'ERROR'], help="specify log level"
         )
-
         parser.add_argument(
-            "--operations", "-op",
-            type=parse_operations,
-            help="Each operation is separated by a semicolon; slice operations should use square brackets; permute "
-                 "sequences should use parentheses"
+            "--tools", default="cmake", choices=['cmake', 'python'],
+            help="specify construction, currently support cmake and python"
         )
+        parser.add_argument(
+            "--mode", default="all", choices=['all', 'api-only'],
+            help="specify scanner mode, currently support all and api only"
+        )
+
+    @staticmethod
+    def _set_env():
+        if os.path.exists("/opt/rh/llvm-toolset-7.0/root/usr/lib64/clang/7.0.1/include"):
+            extra_path = "/opt/rh/llvm-toolset-7.0/root/usr/lib64/clang/7.0.1/include"
+        elif os.path.exists("/usr/lib64/clang/7.0.1/include"):
+            extra_path = "/usr/lib64/clang/7.0.1/include"
+        else:
+            extra_path = ""
+
+        c_plus_include_path = os.environ.get("CPLUS_INCLUDE_PATH")
+        if len(extra_path) > 0:
+            c_plus_include_path = f"{extra_path}:{c_plus_include_path}"
+            os.environ["CPLUS_INCLUDE_PATH"] = c_plus_include_path
 
     def handle(self, args):
-        handle_tensor_view(args)
+        log_util.set_logger_level(args.log_level)
+        log_util.init_file_logger()
+        self._set_env()
+        start_scan_kit(args)
 
 
 def get_cmd_instance():
-    help_info = "view、slice、permute、save the dumped tensor"
-    cmd_instance = TensorViewCommand("tensor-view", help_info)
+    help_info = "Transplant tool to analyze inference applications"
+    cmd_instance = TranspltCommand("transplt", help_info)
     return cmd_instance
```

## Comparing `ms-ait-7.0.0b430/components/tensor_view/ait_tensor_view/__install__.py` & `ms-ait-7.0.0rc2/components/utils/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-# Copyright (c) 2024-2024 Huawei Technologies Co., Ltd.
-
+# Copyright (c) 2023-2023 Huawei Technologies Co., Ltd.
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
-
-from components.utils.install import AitInstaller
-
-
-class TensorViewInstaller(AitInstaller):
-    pass
+# limitations under the License.
```

## Comparing `ms-ait-7.0.0b430/components/transplt/install.bat` & `ms-ait-7.0.0rc2/components/transplt/install.bat`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/install.sh` & `ms-ait-7.0.0rc2/components/transplt/install.sh`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/README.md` & `ms-ait-7.0.0rc2/components/transplt/README.md`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/setup.py` & `ms-ait-7.0.0rc2/components/transplt/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,18 +23,15 @@
 ait_sub_tasks = [{
         "name": "transplt",
         "help_info": "Transplant tool to analyze inference applications",
         "module": "app_analyze.__main__",
         "attr": "get_cmd_instance",
     }]
 
-ait_sub_task_entry_points = [
-    f"{t.get('name')}:{t.get('help_info')} = {t.get('module')}:{t.get('attr')}"
-    for t in ait_sub_tasks
-]
+ait_sub_task_entry_points = [f"{t['name']}:{t['help_info']} = {t['module']}:{t['attr']}" for t in ait_sub_tasks]
 
 setup(
     name='ait-transplt',
     version='7.0.0c2',
     description='app analyze for cpu and gpu projects',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -54,11 +51,10 @@
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
     ],
     python_requires='>=3.7',
     entry_points={
         'ait_sub_task': ait_sub_task_entry_points,
-        'ait_sub_task_installer': ['ait-transplt=app_analyze.__install__:TranspltInstall', 
-                                   'ait-transplt-llvm=app_analyze.__install__:LlvmInstall'],
+        'ait_sub_task_installer': ['ait-transplt=app_analyze.__install__:TranspltInstall'],
     },
 )
```

## Comparing `ms-ait-7.0.0b430/components/transplt/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/install.bat` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/install.bat`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/install.sh` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/install.sh`

 * *Files 10% similar despite different names*

```diff
@@ -77,43 +77,29 @@
   else
     echo "WARNING: uncertified os type:version $OS_NAME:$OS_VERSION. Ait transplt installation may be incorrect!!!"
     # try to install clang
     $SUDO apt-get install wget unzip libclang-14-dev clang-14 -y
   fi
 }
 
+
 # Download and unzip config.zip, headers.zip
 download_config_and_headers() {
   cwd=$(pwd)
 
   ori_mask=$(umask)
   umask 022
-  if [ "$AIT_DOWNLOAD_PATH" != "" ]; then
-    DOWNLOAD_PATH=$AIT_DOWNLOAD_PATH
-  else
-    DOWNLOAD_PATH=$(python3 -c "import app_analyze; print(app_analyze.__path__[0])")
-  fi
 
-  if [ $? -ne 0  ]; then
-      echo "Downloading failed"
-      return
-  fi
-
-  if [ "$AIT_INSTALL_FIND_LINKS" != "" ]; then
-      cp "$AIT_INSTALL_FIND_LINKS/config" ./ -r
-      cp "$AIT_INSTALL_FIND_LINKS/headers" ./ -r
-  else 
-    cd $DOWNLOAD_PATH \
-      && wget -O config.zip https://ait-resources.obs.cn-south-1.myhuaweicloud.com/config.zip \
-      && unzip -o -q config.zip \
-      && rm config.zip -f \
-      && wget -O headers.zip https://ait-resources.obs.cn-south-1.myhuaweicloud.com/headers.zip \
-      && unzip -o -q headers.zip \
-      && rm headers.zip -f
-  fi
+  cd $(python3 -c "import app_analyze; print(app_analyze.__path__[0])") \
+    && wget -O config.zip https://ait-resources.obs.cn-south-1.myhuaweicloud.com/config.zip \
+    && unzip -o -q config.zip \
+    && rm config.zip -f \
+    && wget -O headers.zip https://ait-resources.obs.cn-south-1.myhuaweicloud.com/headers.zip \
+    && unzip -o -q headers.zip \
+    && rm headers.zip -f
 
   umask $ori_mask
   cd $cwd
 }
 
 download_config_and_headers
```

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/common/kit_config.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/common/kit_config.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/common/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/exception/exception_information.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/exception_information.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/exception/source_scan_exception.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/exception/source_scan_exception.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/exception/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/model/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/model/model.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/model/model.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/model/project.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/model/project.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/model/seq_project.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/model/seq_project.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/model/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/app.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/app.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/cmdline_input.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/cmdline_input.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/custom_input.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/custom_input.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/input_factory.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/input_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/porting_input.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/porting/porting_input.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/porting/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/csv_report.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/csv_report.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/json_report.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/json_report.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/report.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/report_factory.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/report/report_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/report/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_parser.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/clang_utils.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/clang_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cmake_scanner.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/cmake_scanner.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/cxx_scanner.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_scanner.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,46 +8,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
-import os
-from multiprocessing import Pool
+
+import pandas as pd
+
 from app_analyze.utils.log_util import logger
 from app_analyze.scan.scanner import Scanner
+from app_analyze.scan.python_parser import Parser
 
 
-class CxxScanner(Scanner):
-    def __init__(self, files, cxx_parser=None):
+class PythonScanner(Scanner):
+    def __init__(self, files, project_directory):
         super().__init__(files)
-        self.cxx_parser = cxx_parser
+        self.project_directory = project_directory
 
     def do_scan(self):
         start_time = time.time()
         result = self.exec_without_threads()
-        self.porting_results['cxx'] = result
+        self.porting_results['python'] = result
         eval_time = time.time() - start_time
 
-        logger.debug(f'Total time for scanning cxx files is {eval_time}s')
+        logger.info(f'Total time for scanning py files is {eval_time}s')
 
     def exec_without_threads(self):
         result = {}
-        count = max(max(os.cpu_count(), len(self.files)), 16)
-        pool = Pool(count)
-        list_file = []
         for file in self.files:
-            list_file.append((self.cxx_parser, file))
-        lst = pool.starmap_async(cxx_parser_, list_file)
-        pool.close()
-        pool.join()
-        lst1 = lst.get(timeout=2)
-        for file, r in zip(self.files, lst1):
-            result[file] = r
-        return result
+            p = Parser(file, self.project_directory)
+            rst_vals = p.parse()
+            result[file] = pd.DataFrame.from_dict(rst_vals)
 
-
-def cxx_parser_(cxx_parser, files):
-    p = cxx_parser(files)
-    rst_vals = p.parse()
-    return rst_vals
+        return result
```

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/func_parser.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/func_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/python_parser.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/python_parser.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_factory.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_factory.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scanner_utils.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scanner_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/scan_api.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/scan_api.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/comment_delete.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/comment_delete.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/file_matrix.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/file_matrix.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/module/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/module/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/acc_libs.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/acc_libs.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/api_filter.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/api_filter.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/ast_visitor.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/ast_visitor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_desc.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_desc.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_handler.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_handler.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_matcher.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_matcher.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/scan/sequence/seq_utils.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/scan/sequence/seq_utils.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/solution/advisor.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/advisor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/solution/seq_advisor.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/solution/seq_advisor.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/solution/__init__.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/__init__.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/clang_finder.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/clang_finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,22 +29,14 @@
             return lib_clang_candidate
 
     logger.error('Unable to locate libclang.dll file, ait transplt will not working.')
     raise RuntimeError("Unable to locate libclang.dll file, ait transplt will not working.")
 
 
 def _get_lib_clang_path_linux():
-    import clang
-
-    libclang_so_path = os.path.join(os.path.dirname(clang.__file__), "native", "libclang.so")
-    if os.path.exists(libclang_so_path):
-        return libclang_so_path
-    else:
-        logger.warning(f"libclang so: {libclang_so_path} not found, may meet error lately.")
-
     # default dirs
     candidate_lib_dirs = [
         "/lib", "/lib64", "/usr/lib", "/usr/lib64",
         "/usr/local/lib", "/usr/local/lib64",
         f'/usr/lib/{platform.machine()}-linux-gnu',
     ]
```

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/excel.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/excel.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/file_locker.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/file_locker.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/io_util.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/io_util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/lib_util.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/lib_util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/log_util.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/log_util.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/transplt/app_analyze/utils/security.py` & `ms-ait-7.0.0rc2/components/transplt/app_analyze/utils/security.py`

 * *Files identical despite different names*

## Comparing `ms-ait-7.0.0b430/components/utils/file_open_check.py` & `ms-ait-7.0.0rc2/components/utils/file_open_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 PATH_WHITE_LIST_REGEX_WIN = re.compile(r"[^_:\\A-Za-z0-9/.-]")
 PATH_WHITE_LIST_REGEX = re.compile(r"[^_A-Za-z0-9/.-]")
 
 PERMISSION_NORMAL = 0o640  # 普通文件
 PERMISSION_KEY = 0o600  # 密钥文件
 READ_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH
-WRITE_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH
+WRITE_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH | stat.S_IROTH | stat.S_IXOTH
 
 SOLUTION_LEVEL = 35
 SOLUTION_LEVEL_WIN = 45
 logging.addLevelName(SOLUTION_LEVEL, "\033[1;32m" + "SOLUTION" + "\033[0m")  # green [SOLUTION]
 logging.addLevelName(SOLUTION_LEVEL_WIN, "SOLUTION_WIN")
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format='[%(levelname)s] %(message)s')
 logger = logging.getLogger(__name__)
@@ -191,15 +191,15 @@
                 logger.error(f"Current user doesn't have read permission to the file {self.file}, "
                              "as import file(or directory) permission should be at least 0o400(r--------) ")
                 solution_log(SOLUTION_BASE_URL + PERMISSION_SUB_URL)
                 return False
         elif perm == 'write' and self.is_exists:
             if (strict_permission or self.is_file) and self.permission & WRITE_FILE_NOT_PERMITTED_STAT > 0:
                 logger.error(f"The file {self.file} is group writable, or is others writable, "
-                             "as export file(or directory) permission should not be over 0o755(rwxr-xr-x)")
+                             "as export file(or directory) permission should not be over 0o750(rwxr-x---)")
                 solution_log(SOLUTION_BASE_URL + PERMISSION_SUB_URL)
                 return False
             if not os.access(self.realpath, os.W_OK):
                 logger.error(f"Current user doesn't have write permission to the file {self.file}, "
                              "as export file(or directory) permission should be at least 0o200(-w-------) ")
                 solution_log(SOLUTION_BASE_URL + PERMISSION_SUB_URL)
                 return False
```

## Comparing `ms-ait-7.0.0b430/components/utils/parser.py` & `ms-ait-7.0.0rc2/components/utils/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,73 +24,57 @@
 logging.basicConfig(
     stream=sys.stdout, level=logging.INFO, format='[%(levelname)s] %(message)s'
 )
 logger = logging.getLogger(__name__)
 
 
 class AitCommand:
-    def __init__(self, name, help_info="", alias_name="", group="Command") -> None:
+    def __init__(self, name, help_info="", alias_name="") -> None:
         self.name = name
         self.help_info = help_info
         self.alias_name = alias_name
-        self.group = group
 
     @abstractmethod
     def register_parser(self, parser):
         pass
 
     @abstractmethod
     def handle(self, args):
         pass
 
 
 class BaseCommand(AitCommand):
-    def __init__(self, name, help_info, children=None, alias_name="", group="Command") -> None:
-        super().__init__(name, help_info, alias_name, group)
+    def __init__(self, name, help_info, children=None, alias_name="") -> None:
+        super().__init__(name, help_info, alias_name)
 
         self.parser = None
         self.children: list[BaseCommand] = []
 
         if isinstance(children, str):
             self.children = LazyEntryPointCommand.build_lazy_tasks(children)
-        elif isinstance(children, list):
-            for child in children:
-                if isinstance(child, BaseCommand):
-                    self.children.append(child)
-                elif isinstance(child, str):
-                    self.children.extend(LazyEntryPointCommand.build_lazy_tasks(child))
-                else:
-                    raise ValueError("unknow child")
         else:
-            pass
+            self.children: list[BaseCommand] = [] if children is None else children
 
     def register_parser(self, parser: argparse.ArgumentParser):
         self.parser = parser
         self.add_arguments(parser)
         parser.set_defaults(handle=self.handle)
 
         if not self.children:
             return
-        
         subparsers = parser.add_subparsers(title="Command")
-        # groups, now put it together. not real group
-        groups = {"Command": []}
         for command in self.children:
-            groups.setdefault(command.group, [])
-            groups.get(command.group).append(command)
-        for _, command_list in groups.items():
-            for command in command_list:
-                subparser = subparsers.add_parser(
-                    command.name,
-                    formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-                    help=command.help_info,
-                    aliases=[command.alias_name] if command.alias_name else [],
-                    description=command.help_info + " " + MIND_STUDIO_LOGO,
-                )
-                command.register_parser(subparser)
+            subparser = subparsers.add_parser(
+                command.name,
+                formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+                help=command.help_info,
+                aliases=[command.alias_name] if command.alias_name else [],
+                description=command.help_info + " " + MIND_STUDIO_LOGO,
+            )
+            command.register_parser(subparser)
 
     def add_arguments(self, parser):
         pass
 
     def handle(self, _):
         if self.parser is not None:
             self.parser.print_help()
```

## Comparing `ms-ait-7.0.0b430/components/utils/security_check.py` & `ms-ait-7.0.0rc2/components/utils/security_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 
 PATH_WHITE_LIST_REGEX = re.compile(r"[^_A-Za-z0-9/.-]")
 STR_WHITE_LIST_REGEX = re.compile(r"[^_A-Za-z0-9\"'><=\[\])(,}{: /.~-]")
 MAX_READ_FILE_SIZE_4G = 4294967296  # 4G, 4 * 1024 * 1024 * 1024
 MAX_READ_FILE_SIZE_32G = 34359738368  # 32G, 32 * 1024 * 1024 * 1024
 READ_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH
-WRITE_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH
+WRITE_FILE_NOT_PERMITTED_STAT = stat.S_IWGRP | stat.S_IWOTH | stat.S_IROTH | stat.S_IXOTH
 
 
 def is_belong_to_user_or_group(file_stat):
     return file_stat.st_uid == os.getuid() or file_stat.st_gid in os.getgroups()
 
 
 def is_endswith_extensions(path, extensions):
@@ -90,15 +90,15 @@
 
     if not is_dir and os.path.exists(real_path):
         if os.path.isdir(real_path):
             raise ValueError("The file {} exist and is a directory.".format(path))
         if check_user_stat and os.stat(real_path).st_uid != os.getuid():  # Has to be exactly belonging to current user
             raise ValueError("The file {} doesn't belong to the current user.".format(path))
         if check_user_stat and os.stat(real_path).st_mode & WRITE_FILE_NOT_PERMITTED_STAT > 0:
-            raise ValueError("The file {} permission for others is writable, or is group writable.".format(path))
+            raise ValueError("The file {} permission for others is not 0, or is group writable.".format(path))
         if not os.access(real_path, os.W_OK):
             raise ValueError("The file {} exist and not writable.".format(path))
     return real_path
 
 
 def type_to_str(value_type):
     return ' or '.join([ii.__name__ for ii in value_type]) if isinstance(value_type, tuple) else value_type.__name__
```

## Comparing `ms-ait-7.0.0b430/ms_ait.egg-info/SOURCES.txt` & `ms-ait-7.0.0rc2/ms_ait.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 components/benchmark/ais_bench/evaluate/interface.py
 components/benchmark/ais_bench/evaluate/log.py
 components/benchmark/ais_bench/evaluate/recorder.py
 components/benchmark/ais_bench/evaluate/dataset/__init__.py
 components/benchmark/ais_bench/evaluate/dataset/base_dataset.py
 components/benchmark/ais_bench/evaluate/dataset/ceval_dataset.py
 components/benchmark/ais_bench/evaluate/dataset/dataset_factory.py
-components/benchmark/ais_bench/evaluate/dataset/download.sh
 components/benchmark/ais_bench/evaluate/dataset/gsm8k_dataset.py
 components/benchmark/ais_bench/evaluate/dataset/mmlu_dataset.py
 components/benchmark/ais_bench/evaluate/measurement/__init__.py
 components/benchmark/ais_bench/evaluate/measurement/measurement.py
 components/benchmark/ais_bench/evaluate/measurement/measurement_factory.py
 components/benchmark/ais_bench/infer/__init__.py
 components/benchmark/ais_bench/infer/__main__.py
@@ -80,19 +79,17 @@
 components/benchmark/ais_bench/infer/backends/backend.py
 components/benchmark/ais_bench/infer/backends/backend_trtexec.py
 components/benchmark/backend/__init__.py
 components/benchmark/backend/install.sh
 components/benchmark/backend/setup.py
 components/benchmark/infer_analyser/__init__.py
 components/benchmark/infer_analyser/analyser.py
-components/benchmark/infer_analyser/infer_analyser.sh
 components/benchmark/infer_analyser/info_convert_json.py
 components/convert/README.md
 components/convert/__init__.py
-components/convert/build.sh
 components/convert/requirements.txt
 components/convert/setup.py
 components/convert/model_convert/__init__.py
 components/convert/model_convert/__install__.py
 components/convert/model_convert/__main__.py
 components/convert/model_convert/cmd_utils.py
 components/convert/model_convert/install.sh
@@ -279,17 +276,15 @@
 components/llm/ait_llm/metrics/__init__.py
 components/llm/ait_llm/metrics/case_filter.py
 components/llm/ait_llm/metrics/metrics.py
 components/llm/ait_llm/opcheck/__init__.py
 components/llm/ait_llm/opcheck/case_manager.py
 components/llm/ait_llm/opcheck/opchecker.py
 components/llm/ait_llm/opcheck/operation_test.py
-components/llm/ait_llm/opcheck/atb_operators/CMakeLists.txt
 components/llm/ait_llm/opcheck/atb_operators/__init__.py
-components/llm/ait_llm/opcheck/atb_operators/build.sh
 components/llm/ait_llm/opcheck/atb_operators/operation_creator.cpp
 components/llm/ait_llm/opcheck/atb_operators/operation_factory.h
 components/llm/ait_llm/opcheck/check_case/__init__.py
 components/llm/ait_llm/opcheck/check_case/activation.py
 components/llm/ait_llm/opcheck/check_case/all_gather.py
 components/llm/ait_llm/opcheck/check_case/all_reduce.py
 components/llm/ait_llm/opcheck/check_case/as_strided.py
@@ -343,27 +338,15 @@
 components/profile/msprof/ait_prof/__install__.py
 components/profile/msprof/ait_prof/__main__.py
 components/profile/msprof/ait_prof/api.py
 components/profile/msprof/ait_prof/args_adapter.py
 components/profile/msprof/ait_prof/main_cli.py
 components/profile/msprof/ait_prof/msprof_process.py
 components/profile/msprof/ait_prof/utils.py
-components/tensor_view/__init__.py
-components/tensor_view/requirements.txt
-components/tensor_view/setup.py
-components/tensor_view/ait_tensor_view/__init__.py
-components/tensor_view/ait_tensor_view/__install__.py
-components/tensor_view/ait_tensor_view/atb.py
-components/tensor_view/ait_tensor_view/handler.py
-components/tensor_view/ait_tensor_view/logger.py
-components/tensor_view/ait_tensor_view/main_cli.py
-components/tensor_view/ait_tensor_view/operation.py
-components/tensor_view/ait_tensor_view/print_stat.py
 components/tests/__init__.py
-components/tests/test_ait.sh
 components/transplt/README.md
 components/transplt/__init__.py
 components/transplt/install.bat
 components/transplt/install.sh
 components/transplt/requirements.txt
 components/transplt/setup.py
 components/transplt/app_analyze/__init__.py
```

