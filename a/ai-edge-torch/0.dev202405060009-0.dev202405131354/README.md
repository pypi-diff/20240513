# Comparing `tmp/ai_edge_torch-0.dev202405060009-py3-none-any.whl.zip` & `tmp/ai_edge_torch-0.dev202405131354-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,93 @@
-Zip file size: 1402 bytes, number of entries: 5
--rw-r--r--  2.0 unx       43 b- defN 24-May-06 07:06 ai_edge_torch/__init__.py
--rw-r--r--  2.0 unx      167 b- defN 24-May-06 07:09 ai_edge_torch-0.dev202405060009.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-06 07:09 ai_edge_torch-0.dev202405060009.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-May-06 07:09 ai_edge_torch-0.dev202405060009.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      449 b- defN 24-May-06 07:09 ai_edge_torch-0.dev202405060009.dist-info/RECORD
-5 files, 765 bytes uncompressed, 550 bytes compressed:  28.1%
+Zip file size: 138896 bytes, number of entries: 91
+-rw-r--r--  2.0 unx     1008 b- defN 24-May-13 17:24 ai_edge_torch/__init__.py
+-rw-r--r--  2.0 unx     4243 b- defN 24-May-13 17:24 ai_edge_torch/model.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/convert/__init__.py
+-rw-r--r--  2.0 unx     4043 b- defN 24-May-13 17:24 ai_edge_torch/convert/conversion.py
+-rw-r--r--  2.0 unx    11021 b- defN 24-May-13 17:24 ai_edge_torch/convert/conversion_utils.py
+-rw-r--r--  2.0 unx     6927 b- defN 24-May-13 17:24 ai_edge_torch/convert/converter.py
+-rw-r--r--  2.0 unx     2825 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/__init__.py
+-rw-r--r--  2.0 unx     1652 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/_pass_base.py
+-rw-r--r--  2.0 unx     6150 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py
+-rw-r--r--  2.0 unx     2607 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/build_upsample_bilinear2d_composite_pass.py
+-rw-r--r--  2.0 unx     1673 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/canonicalize_pass.py
+-rw-r--r--  2.0 unx     2448 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/inject_mlir_debuginfo_pass.py
+-rw-r--r--  2.0 unx      795 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/__init__.py
+-rw-r--r--  2.0 unx     6870 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_check.py
+-rw-r--r--  2.0 unx     1560 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_mark.py
+-rw-r--r--  2.0 unx    12438 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_rewrite.py
+-rw-r--r--  2.0 unx      982 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/op_func_registry.py
+-rw-r--r--  2.0 unx    10030 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/pass_body.py
+-rw-r--r--  2.0 unx     2076 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/utils.py
+-rw-r--r--  2.0 unx      715 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/__init__.py
+-rw-r--r--  2.0 unx     2279 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/greedy.py
+-rw-r--r--  2.0 unx     6432 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/min_cut.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/convert/test/__init__.py
+-rw-r--r--  2.0 unx     8092 b- defN 24-May-13 17:24 ai_edge_torch/convert/test/test_convert.py
+-rw-r--r--  2.0 unx     6403 b- defN 24-May-13 17:24 ai_edge_torch/convert/test/test_convert_composites.py
+-rw-r--r--  2.0 unx     4537 b- defN 24-May-13 17:24 ai_edge_torch/convert/test/test_convert_multisig.py
+-rw-r--r--  2.0 unx      707 b- defN 24-May-13 17:24 ai_edge_torch/debug/__init__.py
+-rw-r--r--  2.0 unx    12789 b- defN 24-May-13 17:24 ai_edge_torch/debug/culprit.py
+-rw-r--r--  2.0 unx     1430 b- defN 24-May-13 17:24 ai_edge_torch/debug/utils.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/debug/test/__init__.py
+-rw-r--r--  2.0 unx     3731 b- defN 24-May-13 17:24 ai_edge_torch/debug/test/test_culprit.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/experimental/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/gemma/__init__.py
+-rw-r--r--  2.0 unx     2538 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/gemma/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5913 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/gemma/gemma.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/phi2/__init__.py
+-rw-r--r--  2.0 unx     2512 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/phi2/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5540 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/phi2/phi2.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/t5/__init__.py
+-rw-r--r--  2.0 unx     4536 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/t5/convert_to_tflite.py
+-rw-r--r--  2.0 unx    21065 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/t5/t5.py
+-rw-r--r--  2.0 unx     8998 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/t5/t5_attention.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/test_models/__init__.py
+-rw-r--r--  2.0 unx     3791 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/test_models/toy_model.py
+-rw-r--r--  2.0 unx     4831 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/tiny_llama/__init__.py
+-rw-r--r--  2.0 unx     2566 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/tiny_llama/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5629 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/tiny_llama/tiny_llama.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/__init__.py
+-rw-r--r--  2.0 unx     9127 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/attention.py
+-rw-r--r--  2.0 unx     6350 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/attention_utils.py
+-rw-r--r--  2.0 unx     3201 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/builder.py
+-rw-r--r--  2.0 unx     2820 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/feed_forward.py
+-rw-r--r--  2.0 unx     3090 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/kv_cache.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/model_config.py
+-rw-r--r--  2.0 unx     1867 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/normalization.py
+-rw-r--r--  2.0 unx     1383 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/rotary_position_embedding.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/__init__.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/example.py
+-rw-r--r--  2.0 unx     1862 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/quant_attrs.py
+-rw-r--r--  2.0 unx     3327 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/quant_recipe.py
+-rw-r--r--  2.0 unx     1913 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/quant_recipe_utils.py
+-rw-r--r--  2.0 unx     1798 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/quant_recipes.py
+-rw-r--r--  2.0 unx     1345 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/supported_schemes.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/test/__init__.py
+-rw-r--r--  2.0 unx     6500 b- defN 24-May-13 17:24 ai_edge_torch/generative/test/test_model_conversion.py
+-rw-r--r--  2.0 unx     3728 b- defN 24-May-13 17:24 ai_edge_torch/generative/test/test_quantize.py
+-rw-r--r--  2.0 unx      720 b- defN 24-May-13 17:24 ai_edge_torch/generative/utilities/__init__.py
+-rw-r--r--  2.0 unx    10029 b- defN 24-May-13 17:24 ai_edge_torch/generative/utilities/loader.py
+-rw-r--r--  2.0 unx    16156 b- defN 24-May-13 17:24 ai_edge_torch/generative/utilities/t5_loader.py
+-rw-r--r--  2.0 unx      752 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/__init__.py
+-rw-r--r--  2.0 unx     4799 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/mark_pattern/__init__.py
+-rw-r--r--  2.0 unx     1539 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/mark_pattern/passes.py
+-rw-r--r--  2.0 unx     9206 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/mark_pattern/pattern.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/test/__init__.py
+-rw-r--r--  2.0 unx     4262 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/test/test_mark_pattern.py
+-rw-r--r--  2.0 unx     8190 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/test/test_stablehlo_composite_builder.py
+-rw-r--r--  2.0 unx      714 b- defN 24-May-13 17:24 ai_edge_torch/quantize/__init__.py
+-rw-r--r--  2.0 unx    15602 b- defN 24-May-13 17:24 ai_edge_torch/quantize/pt2e_quantizer.py
+-rw-r--r--  2.0 unx    36046 b- defN 24-May-13 17:24 ai_edge_torch/quantize/pt2e_quantizer_utils.py
+-rw-r--r--  2.0 unx     3435 b- defN 24-May-13 17:24 ai_edge_torch/quantize/quant_config.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/testing/__init__.py
+-rw-r--r--  2.0 unx      765 b- defN 24-May-13 17:24 ai_edge_torch/testing/model_coverage/__init__.py
+-rw-r--r--  2.0 unx     4286 b- defN 24-May-13 17:24 ai_edge_torch/testing/model_coverage/model_coverage.py
+-rw-r--r--  2.0 unx    11358 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1712 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9695 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/RECORD
+91 files, 397737 bytes uncompressed, 122794 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,16 +1,274 @@
 Filename: ai_edge_torch/__init__.py
 Comment: 
 
-Filename: ai_edge_torch-0.dev202405060009.dist-info/METADATA
+Filename: ai_edge_torch/model.py
 Comment: 
 
-Filename: ai_edge_torch-0.dev202405060009.dist-info/WHEEL
+Filename: ai_edge_torch/convert/__init__.py
 Comment: 
 
-Filename: ai_edge_torch-0.dev202405060009.dist-info/top_level.txt
+Filename: ai_edge_torch/convert/conversion.py
 Comment: 
 
-Filename: ai_edge_torch-0.dev202405060009.dist-info/RECORD
+Filename: ai_edge_torch/convert/conversion_utils.py
+Comment: 
+
+Filename: ai_edge_torch/convert/converter.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/_pass_base.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/build_upsample_bilinear2d_composite_pass.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/canonicalize_pass.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/inject_mlir_debuginfo_pass.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_check.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_mark.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_rewrite.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/op_func_registry.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/pass_body.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/utils.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/greedy.py
+Comment: 
+
+Filename: ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/min_cut.py
+Comment: 
+
+Filename: ai_edge_torch/convert/test/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/convert/test/test_convert.py
+Comment: 
+
+Filename: ai_edge_torch/convert/test/test_convert_composites.py
+Comment: 
+
+Filename: ai_edge_torch/convert/test/test_convert_multisig.py
+Comment: 
+
+Filename: ai_edge_torch/debug/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/debug/culprit.py
+Comment: 
+
+Filename: ai_edge_torch/debug/utils.py
+Comment: 
+
+Filename: ai_edge_torch/debug/test/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/debug/test/test_culprit.py
+Comment: 
+
+Filename: ai_edge_torch/experimental/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/gemma/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/gemma/convert_to_tflite.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/gemma/gemma.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/phi2/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/phi2/convert_to_tflite.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/phi2/phi2.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/t5/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/t5/convert_to_tflite.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/t5/t5.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/t5/t5_attention.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/test_models/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/test_models/toy_model.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/tiny_llama/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/tiny_llama/convert_to_tflite.py
+Comment: 
+
+Filename: ai_edge_torch/generative/examples/tiny_llama/tiny_llama.py
+Comment: 
+
+Filename: ai_edge_torch/generative/layers/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/layers/attention.py
+Comment: 
+
+Filename: ai_edge_torch/generative/layers/attention_utils.py
+Comment: 
+
+Filename: ai_edge_torch/generative/layers/builder.py
+Comment: 
+
+Filename: ai_edge_torch/generative/layers/feed_forward.py
+Comment: 
+
+Filename: ai_edge_torch/generative/layers/kv_cache.py
+Comment: 
+
+Filename: ai_edge_torch/generative/layers/model_config.py
+Comment: 
+
+Filename: ai_edge_torch/generative/layers/normalization.py
+Comment: 
+
+Filename: ai_edge_torch/generative/layers/rotary_position_embedding.py
+Comment: 
+
+Filename: ai_edge_torch/generative/quantize/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/quantize/example.py
+Comment: 
+
+Filename: ai_edge_torch/generative/quantize/quant_attrs.py
+Comment: 
+
+Filename: ai_edge_torch/generative/quantize/quant_recipe.py
+Comment: 
+
+Filename: ai_edge_torch/generative/quantize/quant_recipe_utils.py
+Comment: 
+
+Filename: ai_edge_torch/generative/quantize/quant_recipes.py
+Comment: 
+
+Filename: ai_edge_torch/generative/quantize/supported_schemes.py
+Comment: 
+
+Filename: ai_edge_torch/generative/test/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/test/test_model_conversion.py
+Comment: 
+
+Filename: ai_edge_torch/generative/test/test_quantize.py
+Comment: 
+
+Filename: ai_edge_torch/generative/utilities/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/generative/utilities/loader.py
+Comment: 
+
+Filename: ai_edge_torch/generative/utilities/t5_loader.py
+Comment: 
+
+Filename: ai_edge_torch/hlfb/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/hlfb/mark_pattern/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/hlfb/mark_pattern/passes.py
+Comment: 
+
+Filename: ai_edge_torch/hlfb/mark_pattern/pattern.py
+Comment: 
+
+Filename: ai_edge_torch/hlfb/test/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/hlfb/test/test_mark_pattern.py
+Comment: 
+
+Filename: ai_edge_torch/hlfb/test/test_stablehlo_composite_builder.py
+Comment: 
+
+Filename: ai_edge_torch/quantize/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/quantize/pt2e_quantizer.py
+Comment: 
+
+Filename: ai_edge_torch/quantize/pt2e_quantizer_utils.py
+Comment: 
+
+Filename: ai_edge_torch/quantize/quant_config.py
+Comment: 
+
+Filename: ai_edge_torch/testing/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/testing/model_coverage/__init__.py
+Comment: 
+
+Filename: ai_edge_torch/testing/model_coverage/model_coverage.py
+Comment: 
+
+Filename: ai_edge_torch-0.dev202405131354.dist-info/LICENSE
+Comment: 
+
+Filename: ai_edge_torch-0.dev202405131354.dist-info/METADATA
+Comment: 
+
+Filename: ai_edge_torch-0.dev202405131354.dist-info/WHEEL
+Comment: 
+
+Filename: ai_edge_torch-0.dev202405131354.dist-info/top_level.txt
+Comment: 
+
+Filename: ai_edge_torch-0.dev202405131354.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ai_edge_torch/__init__.py

```diff
@@ -1 +1,30 @@
-print("This is the ai-edge-torch package")
+# Copyright 2024 The AI Edge Torch Authors.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+
+from .convert.converter import convert
+from .convert.converter import signature
+from .model import Model
+
+
+def load(path: str) -> Model:
+  """Imports an ai_edge_torch model from disk.
+
+  Args:
+    path: The path to the serialized ai_edge_torch model.
+
+  Returns:
+    An ai_edge_torch.model.Model object.
+  """
+  return Model.load(path)
```

