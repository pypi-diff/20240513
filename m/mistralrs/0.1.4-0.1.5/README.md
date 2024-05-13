# Comparing `tmp/mistralrs-0.1.4.tar.gz` & `tmp/mistralrs-0.1.5.tar.gz`

## Comparing `mistralrs-0.1.4.tar` & `mistralrs-0.1.5.tar`

### file list

```diff
@@ -1,78 +1,83 @@
--rw-r--r--   0     1001      127     1997 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/Cargo.toml
--rw-r--r--   0     1001      127        0 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/README.md
--rw-r--r--   0     1001      127      133 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/README.md
--rw-r--r--   0     1001      127     6567 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/bintokens.rs
--rw-r--r--   0     1001      127      320 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/bytes.rs
--rw-r--r--   0     1001      127    15100 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/cfg.rs
--rw-r--r--   0     1001      127     9819 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/lex.rs
--rw-r--r--   0     1001      127      179 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/mod.rs
--rw-r--r--   0     1001      127     2447 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/recognizer.rs
--rw-r--r--   0     1001      127     1696 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/rx.rs
--rw-r--r--   0     1001      127     3094 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/svob.rs
--rw-r--r--   0     1001      127    17311 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/aici/toktree.rs
--rw-r--r--   0     1001      127     4674 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/device_map.rs
--rw-r--r--   0     1001      127    19350 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/engine/mod.rs
--rw-r--r--   0     1001      127     7768 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/layers.rs
--rw-r--r--   0     1001      127     7898 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/lib.rs
--rw-r--r--   0     1001      127     8310 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/model_loader.rs
--rw-r--r--   0     1001      127    10703 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/model_selected.rs
--rw-r--r--   0     1001      127    16539 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/gemma.rs
--rw-r--r--   0     1001      127    15336 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/llama.rs
--rw-r--r--   0     1001      127    17970 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/mistral.rs
--rw-r--r--   0     1001      127    22539 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/mixtral.rs
--rw-r--r--   0     1001      127     2620 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/mod.rs
--rw-r--r--   0     1001      127    15656 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/phi2.rs
--rw-r--r--   0     1001      127    17536 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/phi3.rs
--rw-r--r--   0     1001      127    19614 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/quantized_llama.rs
--rw-r--r--   0     1001      127    10147 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/quantized_phi2.rs
--rw-r--r--   0     1001      127    16128 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/models/qwen2.rs
--rw-r--r--   0     1001      127     5363 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/cache_manager.rs
--rw-r--r--   0     1001      127     5911 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/chat_template.rs
--rw-r--r--   0     1001      127    14988 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/ggml.rs
--rw-r--r--   0     1001      127    18077 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/gguf.rs
--rw-r--r--   0     1001      127    22337 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/loaders.rs
--rw-r--r--   0     1001      127    10912 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/macros.rs
--rw-r--r--   0     1001      127    36836 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/mod.rs
--rw-r--r--   0     1001      127    13466 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/normal.rs
--rw-r--r--   0     1001      127     2677 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/sampling.rs
--rw-r--r--   0     1001      127     9680 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/pipeline/sampling_pipeline.rs
--rw-r--r--   0     1001      127     6693 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/prefix_cacher.rs
--rw-r--r--   0     1001      127     1250 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/request.rs
--rw-r--r--   0     1001      127     3848 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/response.rs
--rw-r--r--   0     1001      127    11276 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/sampler.rs
--rw-r--r--   0     1001      127     6993 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/scheduler.rs
--rw-r--r--   0     1001      127    16663 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/sequence.rs
--rw-r--r--   0     1001      127     7534 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/utils/mod.rs
--rw-r--r--   0     1001      127     1716 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/utils/tokens.rs
--rw-r--r--   0     1001      127     4799 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/utils/varbuilder_utils.rs
--rw-r--r--   0     1001      127    11049 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/classifier.rs
--rw-r--r--   0     1001      127     1544 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/config.rs
--rw-r--r--   0     1001      127    26767 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/gemma.rs
--rw-r--r--   0     1001      127    25253 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/llama.rs
--rw-r--r--   0     1001      127    27656 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/mistral.rs
--rw-r--r--   0     1001      127    32968 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/mixtral.rs
--rw-r--r--   0     1001      127     4322 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/mod.rs
--rw-r--r--   0     1001      127    24545 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/phi2.rs
--rw-r--r--   0     1001      127    25484 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/phi3.rs
--rw-r--r--   0     1001      127    34254 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-core/src/xlora_models/quantized_llama.rs
--rw-r--r--   0     1001      127      794 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-lora/Cargo.toml
--rw-r--r--   0     1001      127        0 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-lora/README.md
--rw-r--r--   0     1001      127     2395 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-lora/src/layer.rs
--rw-r--r--   0     1001      127     5818 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-lora/src/lib.rs
--rw-r--r--   0     1001      127     9472 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-lora/src/loralinear.rs
--rw-r--r--   0     1001      127     9961 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-lora/src/qloralinear.rs
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 mistralrs-0.1.4/mistralrs-pyo3/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/.gitignore
--rw-r--r--   0     1001      127     3508 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/API.md
--rw-r--r--   0     1001      127      855 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/Cargo_template.toml
--rw-r--r--   0     1001      127     3755 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/README.md
--rw-r--r--   0     1001      127     7962 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/mistralrs.pyi
--rw-r--r--   0     1001      127      530 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/pyproject_template.toml
--rw-r--r--   0     1001      127    28898 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/src/lib.rs
--rw-r--r--   0     1001      127     1672 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/src/stream.rs
--rw-r--r--   0     1001      127     3114 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/src/which.rs
--rwxr-xr-x   0     1001      127     2203 2024-05-08 09:09:24.000000 mistralrs-0.1.4/mistralrs-pyo3/upload.py
--rw-r--r--   0     1001      127   100996 2024-05-08 09:10:06.000000 mistralrs-0.1.4/Cargo.lock
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 mistralrs-0.1.4/Cargo.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 mistralrs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4445 1970-01-01 00:00:00.000000 mistralrs-0.1.4/PKG-INFO
+-rw-r--r--   0     1001      127      794 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-lora/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-lora/README.md
+-rw-r--r--   0     1001      127     2429 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-lora/src/layer.rs
+-rw-r--r--   0     1001      127     8618 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-lora/src/lib.rs
+-rw-r--r--   0     1001      127    11219 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-lora/src/loralinear.rs
+-rw-r--r--   0     1001      127    11929 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-lora/src/qloralinear.rs
+-rw-r--r--   0     1001      127     2034 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/README.md
+-rw-r--r--   0     1001      127      133 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/README.md
+-rw-r--r--   0     1001      127     6551 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/bintokens.rs
+-rw-r--r--   0     1001      127      320 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/bytes.rs
+-rw-r--r--   0     1001      127    15100 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/cfg.rs
+-rw-r--r--   0     1001      127     9819 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/lex.rs
+-rw-r--r--   0     1001      127      179 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/mod.rs
+-rw-r--r--   0     1001      127     2447 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/recognizer.rs
+-rw-r--r--   0     1001      127     1696 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/rx.rs
+-rw-r--r--   0     1001      127     3094 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/svob.rs
+-rw-r--r--   0     1001      127    17311 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/aici/toktree.rs
+-rw-r--r--   0     1001      127     4674 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/device_map.rs
+-rw-r--r--   0     1001      127    20762 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/engine/mod.rs
+-rw-r--r--   0     1001      127    12620 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/layers.rs
+-rw-r--r--   0     1001      127     7589 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/lib.rs
+-rw-r--r--   0     1001      127     8538 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/model_loader.rs
+-rw-r--r--   0     1001      127    10309 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/model_selected.rs
+-rw-r--r--   0     1001      127    15657 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/gemma.rs
+-rw-r--r--   0     1001      127    14521 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/llama.rs
+-rw-r--r--   0     1001      127    16089 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/mistral.rs
+-rw-r--r--   0     1001      127    20876 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/mixtral.rs
+-rw-r--r--   0     1001      127     2877 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/mod.rs
+-rw-r--r--   0     1001      127    15016 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/phi2.rs
+-rw-r--r--   0     1001      127    15712 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/phi3.rs
+-rw-r--r--   0     1001      127    18564 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/quantized_llama.rs
+-rw-r--r--   0     1001      127     9221 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/quantized_phi2.rs
+-rw-r--r--   0     1001      127    11195 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/quantized_phi3.rs
+-rw-r--r--   0     1001      127    14488 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/models/qwen2.rs
+-rw-r--r--   0     1001      127     5266 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/cache_manager.rs
+-rw-r--r--   0     1001      127     5911 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/chat_template.rs
+-rw-r--r--   0     1001      127    15865 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/ggml.rs
+-rw-r--r--   0     1001      127    22111 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/gguf.rs
+-rw-r--r--   0     1001      127    23366 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/loaders.rs
+-rw-r--r--   0     1001      127    11539 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/macros.rs
+-rw-r--r--   0     1001      127    45316 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/mod.rs
+-rw-r--r--   0     1001      127    13640 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/normal.rs
+-rw-r--r--   0     1001      127     3781 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/sampling.rs
+-rw-r--r--   0     1001      127     9717 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/sampling_pipeline.rs
+-rw-r--r--   0     1001      127    17616 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/pipeline/speculative.rs
+-rw-r--r--   0     1001      127     6693 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/prefix_cacher.rs
+-rw-r--r--   0     1001      127     2116 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/request.rs
+-rw-r--r--   0     1001      127     3848 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/response.rs
+-rw-r--r--   0     1001      127    14833 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/sampler.rs
+-rw-r--r--   0     1001      127     9205 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/scheduler.rs
+-rw-r--r--   0     1001      127    18360 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/sequence.rs
+-rw-r--r--   0     1001      127    14577 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/toml_selector.rs
+-rw-r--r--   0     1001      127     7848 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1716 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/utils/tokens.rs
+-rw-r--r--   0     1001      127     6749 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/utils/varbuilder_utils.rs
+-rw-r--r--   0     1001      127    11049 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/classifier.rs
+-rw-r--r--   0     1001      127     1544 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/config.rs
+-rw-r--r--   0     1001      127    26953 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/gemma.rs
+-rw-r--r--   0     1001      127    26176 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/llama.rs
+-rw-r--r--   0     1001      127    27604 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/mistral.rs
+-rw-r--r--   0     1001      127    33531 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/mixtral.rs
+-rw-r--r--   0     1001      127     4388 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/mod.rs
+-rw-r--r--   0     1001      127    25539 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/phi2.rs
+-rw-r--r--   0     1001      127    25038 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/phi3.rs
+-rw-r--r--   0     1001      127    36716 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/quantized_llama.rs
+-rw-r--r--   0     1001      127    19395 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-core/src/xlora_models/quantized_phi3.rs
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 mistralrs-0.1.5/mistralrs-pyo3/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/.gitignore
+-rw-r--r--   0     1001      127     3358 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/API.md
+-rw-r--r--   0     1001      127      927 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/Cargo_template.toml
+-rw-r--r--   0     1001      127     3755 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/README.md
+-rw-r--r--   0     1001      127       71 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/build.rs
+-rw-r--r--   0     1001      127     8688 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/mistralrs.pyi
+-rw-r--r--   0     1001      127      530 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/pyproject_template.toml
+-rw-r--r--   0     1001      127    29216 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     1672 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/src/stream.rs
+-rw-r--r--   0     1001      127     3020 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/src/which.rs
+-rwxr-xr-x   0     1001      127     2203 2024-05-13 09:33:43.000000 mistralrs-0.1.5/mistralrs-pyo3/upload.py
+-rw-r--r--   0     1001      127   100112 2024-05-13 09:34:10.000000 mistralrs-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 mistralrs-0.1.5/Cargo.toml
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 mistralrs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4445 1970-01-01 00:00:00.000000 mistralrs-0.1.5/PKG-INFO
```

### Comparing `mistralrs-0.1.4/mistralrs-core/Cargo.toml` & `mistralrs-0.1.5/mistralrs-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 dirs = "5.0.1"
 hf-hub = "0.3.2"
 thiserror = "1.0.57"
 tokenizers = "0.15.2"
 tqdm = "0.7.0"
 range-checked = { git = "https://github.com/EricLBuehler/range-checked.git", version = "0.1.0" }
 chrono = "0.4.34"
-mistralrs-lora = { version = "0.1.4", path = "../mistralrs-lora" }
+mistralrs-lora = { version = "0.1.5", path = "../mistralrs-lora" }
 minijinja = "1.0.12"
 either.workspace = true
 indexmap.workspace = true
 half = "2.4.0"
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 tracing.workspace = true
@@ -48,14 +48,16 @@
 rayon = "1.10.0"
 tokio.workspace = true
 tokio-rayon = "2.1.0"
 rand_isaac = "0.3.0"
 futures.workspace = true
 indicatif = { version = "0.17.8", features = ["rayon"] }
 async-trait = "0.1.80"
+once_cell = "1.19.0"
+toml = "0.8.12"
 
 [features]
 cuda = ["candle-core/cuda", "candle-nn/cuda", "candle-transformers/cuda"]
 cudnn = ["candle-core/cudnn"]
 metal = ["candle-core/metal", "candle-nn/metal", "candle-transformers/metal"]
 flash-attn = ["cuda", "candle-transformers/flash-attn", "dep:candle-flash-attn"]
 accelerate = ["candle-core/accelerate", "candle-nn/accelerate", "candle-transformers/accelerate"]
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/aici/bintokens.rs` & `mistralrs-0.1.5/mistralrs-core/src/aici/bintokens.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 // Licensed under the MIT license
 
 use crate::aici::{bytes::TokRxInfo, toktree::TokTrie};
 use anyhow::{anyhow, bail, Result};
 use serde::{Deserialize, Serialize};
 use std::collections::{BTreeMap, HashMap};
 use tokenizers::{normalizers::Sequence, NormalizerWrapper, Tokenizer};
-use tracing::{error, info};
+use tracing::{error, warn};
 
 #[derive(Serialize, Deserialize)]
 pub struct ByteTokenizer {
     pub hf_model: String,
     pub hf_tokenizer: Tokenizer,
     pub eos_token: u32,
     pub vocab_size: u32,
@@ -151,15 +151,15 @@
                     };
 
                     res.token_bytes[tok_id as usize] = bytes;
                 } else {
                     panic!();
                 }
             } else {
-                info!("⚠️ WARNING: missing token: {}", tok_id);
+                warn!("missing token: {}", tok_id);
             }
         }
 
         Ok(res)
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/aici/cfg.rs` & `mistralrs-0.1.5/mistralrs-core/src/aici/cfg.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/aici/lex.rs` & `mistralrs-0.1.5/mistralrs-core/src/aici/lex.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/aici/recognizer.rs` & `mistralrs-0.1.5/mistralrs-core/src/aici/recognizer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/aici/rx.rs` & `mistralrs-0.1.5/mistralrs-core/src/aici/rx.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/aici/svob.rs` & `mistralrs-0.1.5/mistralrs-core/src/aici/svob.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/aici/toktree.rs` & `mistralrs-0.1.5/mistralrs-core/src/aici/toktree.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/device_map.rs` & `mistralrs-0.1.5/mistralrs-core/src/device_map.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/engine/mod.rs` & `mistralrs-0.1.5/mistralrs-core/src/engine/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,23 @@
     sync::Arc,
     time::{Instant, SystemTime, UNIX_EPOCH},
 };
 use tokio::sync::{mpsc::Receiver, Mutex};
 
 use crate::{
     aici::{cfg::CfgParser, recognizer::StackRecognizer, rx::RecRx},
-    pipeline::CacheInstruction,
+    pipeline::{AdapterInstruction, CacheInstruction},
+    request::NormalRequest,
     response::CompletionChoice,
     CompletionResponse, RequestMessage, Response,
 };
-use candle_core::{quantized::GgmlDType, Result, Tensor};
+use candle_core::{Result, Tensor};
 use rand::SeedableRng;
 use rand_isaac::Isaac64Rng;
-use tracing::info;
+use tracing::{info, warn};
 
 use crate::{
     get_mut_arcmutex, handle_pipeline_forward_error, handle_seq_error,
     pipeline::Pipeline,
     prefix_cacher::PrefixCacheManager,
     request::Request,
     response::{ChatCompletionResponse, Choice, ResponseMessage},
@@ -28,43 +29,40 @@
     Constraint, StopTokens,
 };
 
 const SEED: u64 = 0;
 
 pub struct Engine {
     rx: Receiver<Request>,
-    isq_rx: Receiver<GgmlDType>,
     pipeline: Arc<Mutex<dyn Pipeline>>,
     scheduler: Scheduler<VecDeque<Sequence>>,
     id: usize,
     truncate_sequence: bool,
     no_kv_cache: bool,
     prefix_cacher: PrefixCacheManager,
     is_debug: bool,
     disable_eos_stop: bool,
 }
 
 impl Engine {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         rx: Receiver<Request>,
-        isq_rx: Receiver<GgmlDType>,
         pipeline: Arc<Mutex<dyn Pipeline>>,
         method: SchedulerMethod,
         truncate_sequence: bool,
         no_kv_cache: bool,
         no_prefix_cache: bool,
         prefix_cache_n: usize,
         disable_eos_stop: bool,
     ) -> Self {
         let device = get_mut_arcmutex!(pipeline).device().clone();
         let is_xlora = get_mut_arcmutex!(pipeline).get_metadata().is_xlora;
         Self {
             rx,
-            isq_rx,
             pipeline,
             scheduler: Scheduler::new(method),
             id: 0,
             truncate_sequence,
             no_kv_cache,
             prefix_cacher: PrefixCacheManager::new(
                 device,
@@ -80,40 +78,46 @@
     }
 
     pub async fn run(&mut self) {
         let rng = Arc::new(std::sync::Mutex::new(Isaac64Rng::seed_from_u64(SEED)));
         let mut last_completion_ids: Vec<usize> = vec![];
         'lp: loop {
             while let Ok(request) = self.rx.try_recv() {
-                self.add_request(request).await;
+                self.handle_request(request).await;
             }
             let run_start = Instant::now();
             let mut scheduled = self.scheduler.schedule();
-            if let Ok(dtype) = self.isq_rx.try_recv() {
-                if let Err(e) = get_mut_arcmutex!(self.pipeline).re_isq_model(dtype) {
-                    info!("⚠️ WARNING: ISQ requantization failed: {e:?}");
-                }
-            }
 
             if scheduled.completion.len() > 0 {
                 let current_completion_ids: Vec<usize> =
                     scheduled.completion.iter().map(|seq| *seq.id()).collect();
                 let res = {
                     let mut pipeline = get_mut_arcmutex!(self.pipeline);
                     let pre_op =
                         if !self.no_kv_cache && last_completion_ids != current_completion_ids {
-                            CacheInstruction::In
+                            CacheInstruction::In(
+                                scheduled.completion[0]
+                                    .get_adapters()
+                                    .map(AdapterInstruction::Activate)
+                                    .unwrap_or(AdapterInstruction::None),
+                            )
                         } else {
-                            CacheInstruction::Nonthing
+                            CacheInstruction::Nothing(
+                                scheduled.completion[0]
+                                    .get_adapters()
+                                    .map(AdapterInstruction::Activate)
+                                    .unwrap_or(AdapterInstruction::None),
+                            )
                         };
                     let post_op = if !self.no_kv_cache {
                         CacheInstruction::Out
                     } else {
                         CacheInstruction::Reset {
                             reset_non_granular: false,
+                            adapter_inst: AdapterInstruction::None,
                         }
                     };
 
                     pipeline
                         .step(
                             &mut scheduled.completion,
                             false,
@@ -144,28 +148,34 @@
 
                     // Run the prompt seqs
                     let post_op = if !self.no_kv_cache {
                         CacheInstruction::Out
                     } else {
                         CacheInstruction::Reset {
                             reset_non_granular: false,
+                            adapter_inst: AdapterInstruction::None,
                         }
                     };
+                    let adapter_inst = scheduled.prompt[0]
+                        .get_adapters()
+                        .map(AdapterInstruction::Activate)
+                        .unwrap_or(AdapterInstruction::None);
 
                     // Reset non granular state because the old sequence must be dead.
                     // Technically we don't need to do this but it is better to be safe.
                     pipeline
                         .step(
                             &mut scheduled.prompt,
                             true,
                             &mut self.prefix_cacher,
                             self.disable_eos_stop,
                             rng.clone(),
                             CacheInstruction::Reset {
                                 reset_non_granular: false,
+                                adapter_inst,
                             },
                             post_op,
                         )
                         .await
                 };
 
                 handle_pipeline_forward_error!(
@@ -219,15 +229,15 @@
             }
             if scheduled.prompt.len() == 0
                 && scheduled.completion.len() == 0
                 && self.scheduler.waiting_len() == 0
             {
                 // If there is nothing to do, sleep until a request comes in
                 if let Some(request) = self.rx.recv().await {
-                    self.add_request(request).await;
+                    self.handle_request(request).await;
                 }
             }
         }
     }
 
     fn build_sequence_recognizer(constraint: &Constraint) -> anyhow::Result<SequenceRecognizer> {
         let recognizer = match constraint {
@@ -253,15 +263,32 @@
                 }
                 Ok(Some(Tensor::from_vec(logits_bias, vocab_size, &device)?))
             }
             None => Ok(None),
         }
     }
 
-    async fn add_request(&mut self, request: Request) {
+    async fn handle_request(&mut self, request: Request) {
+        match request {
+            Request::ActivateAdapters(adapters) => {
+                match get_mut_arcmutex!(self.pipeline).activate_adapters(adapters) {
+                    Ok(n) => info!("Swapped adapters in {n} LoRA layers."),
+                    Err(e) => warn!("Adapter activation failed: {e:?}"),
+                }
+            }
+            Request::Normal(request) => self.add_request(request).await,
+            Request::ReIsq(level) => {
+                if let Err(e) = get_mut_arcmutex!(self.pipeline).re_isq_model(level) {
+                    warn!("ISQ requantization failed: {e:?}");
+                }
+            }
+        }
+    }
+
+    async fn add_request(&mut self, request: NormalRequest) {
         let is_chat = matches!(request.messages, RequestMessage::Chat(_));
         let echo_prompt = matches!(
             request.messages,
             RequestMessage::Completion {
                 echo_prompt: true,
                 ..
             }
@@ -336,15 +363,15 @@
                     } else {
                         sampling_max
                     }
                 } else {
                     10
                 };
                 prompt = prompt[(currently_over + sampling_max)..].to_vec();
-                info!("⚠️ WARNING: Prompt for request {} was {} tokens over the model maximum length. The last {} tokens were truncated to make space for generation.", request.id, currently_over, prompt_len - prompt.len());
+                warn!("Prompt for request {} was {} tokens over the model maximum length. The last {} tokens were truncated to make space for generation.", request.id, currently_over, prompt_len - prompt.len());
             }
         }
         let prefill_cache = handle_seq_error!(
             self.prefix_cacher.search_for_matching_cache(&prompt),
             request.response
         );
 
@@ -493,14 +520,15 @@
                 recognizer,
                 request.suffix.clone(),
                 if echo_prompt {
                     Some(formatted_prompt.clone())
                 } else {
                     None
                 },
+                request.adapters.clone(),
             );
             let seq = if let Some(prefill_cache) = prefill_cache.clone() {
                 seq.prefill(
                     prefill_cache.normal,
                     prefill_cache.xlora,
                     prefill_cache.toks,
                 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/lib.rs` & `mistralrs-0.1.5/mistralrs-core/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     io::Write,
     sync::{Arc, Mutex},
     thread,
     time::{SystemTime, UNIX_EPOCH},
 };
 use tokio::sync::mpsc::{channel, Sender};
 
-use candle_core::quantized::GgmlDType;
 use engine::Engine;
 pub use mistralrs_lora::Ordering;
 pub use pipeline::Pipeline;
 
 mod aici;
 mod device_map;
 mod engine;
@@ -29,39 +28,41 @@
 mod pipeline;
 mod prefix_cacher;
 mod request;
 mod response;
 mod sampler;
 mod scheduler;
 mod sequence;
+mod toml_selector;
 mod utils;
 mod xlora_models;
 
 pub use device_map::{DeviceMapMetadata, LayerDeviceMapper};
 pub use pipeline::{
     GGMLLoader, GGMLLoaderBuilder, GGMLSpecificConfig, GGUFLoader, GGUFLoaderBuilder,
     GGUFSpecificConfig, GemmaLoader, LlamaLoader, Loader, MistralLoader, MixtralLoader, ModelKind,
     NormalLoader, NormalLoaderBuilder, NormalLoaderType, NormalSpecificConfig, Phi2Loader,
-    Phi3Loader, Qwen2Loader, TokenSource,
+    Phi3Loader, Qwen2Loader, SpeculativeConfig, SpeculativeLoader, SpeculativePipeline,
+    TokenSource,
 };
-pub use request::{Constraint, Request, RequestMessage};
+pub use request::{Constraint, NormalRequest, Request, RequestMessage};
 pub use response::Response;
 pub use response::*;
 pub use sampler::{SamplingParams, StopTokens, TopLogprob};
 pub use scheduler::SchedulerMethod;
 use serde::Serialize;
 use tokio::runtime::Runtime;
+pub use toml_selector::{TomlLoaderArgs, TomlSelector};
 
 /// The MistralRs struct handles sending requests to the engine.
 /// It is the core multi-threaded component of mistral.rs, and uses `mspc`
 /// `Sender` and `Receiver` primitives to send and receive requests to the
 /// engine.
 pub struct MistralRs {
     sender: Sender<Request>,
-    sender_isq: Sender<GgmlDType>,
     log: Option<String>,
     id: String,
     creation_time: u64,
     next_request_id: Mutex<RefCell<usize>>,
 }
 
 /// The MistralRsBuilder takes the pipeline and a scheduler method and constructs
@@ -142,33 +143,30 @@
         let truncate_sequence = truncate_sequence.unwrap_or(false);
         let no_kv_cache = no_kv_cache.unwrap_or(false);
         let no_prefix_cache = no_prefix_cache.unwrap_or(false);
         let prefix_cache_n = prefix_cache_n.unwrap_or(16);
         let disable_eos_stop = disable_eos_stop.unwrap_or(false);
 
         let (tx, rx) = channel(10_000);
-        let (isq_tx, isq_rx) = channel(10_000);
 
         let this = Arc::new(Self {
             sender: tx,
-            sender_isq: isq_tx,
             log,
             id: pipeline.try_lock().unwrap().name(),
             creation_time: SystemTime::now()
                 .duration_since(UNIX_EPOCH)
                 .expect("Time travel has occurred!")
                 .as_secs(),
             next_request_id: Mutex::new(RefCell::new(0)),
         });
         thread::spawn(move || {
             let rt = Runtime::new().unwrap();
             rt.block_on(async move {
                 let mut engine = Engine::new(
                     rx,
-                    isq_rx,
                     pipeline,
                     method,
                     truncate_sequence,
                     no_kv_cache,
                     no_prefix_cache,
                     prefix_cache_n,
                     disable_eos_stop,
@@ -180,22 +178,14 @@
         this
     }
 
     pub fn get_sender(&self) -> Sender<Request> {
         self.sender.clone()
     }
 
-    /// Send a request to re-ISQ the model. If the model was loaded as GGUF or GGML
-    /// then nothing will happen.
-    pub fn send_re_isq(&self, dtype: GgmlDType) {
-        self.sender_isq
-            .blocking_send(dtype)
-            .expect("Engine is not present.")
-    }
-
     pub fn get_id(&self) -> String {
         self.id.clone()
     }
 
     pub fn get_creation_time(&self) -> u64 {
         self.creation_time
     }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/model_loader.rs` & `mistralrs-0.1.5/mistralrs-core/src/model_loader.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-use std::fs::File;
+use std::fs::{self, File};
 
 use crate::{
     pipeline::{
         GGMLLoaderBuilder, GGMLSpecificConfig, GGUFLoaderBuilder, GGUFSpecificConfig,
         NormalSpecificConfig,
     },
-    Loader, ModelSelected, NormalLoaderBuilder,
+    Loader, ModelSelected, NormalLoaderBuilder, TomlLoaderArgs, TomlSelector,
 };
 
 pub struct LoaderBuilder {
     model: ModelSelected,
     no_kv_cache: bool,
     chat_template: Option<String>,
     use_flash_attn: bool,
@@ -46,15 +46,16 @@
 pub fn get_tgt_non_granular_index(model: &ModelSelected) -> Option<usize> {
     match model {
         ModelSelected::Plain { .. }
         | ModelSelected::Lora { .. }
         | ModelSelected::GGUF { .. }
         | ModelSelected::LoraGGUF { .. }
         | ModelSelected::GGML { .. }
-        | ModelSelected::LoraGGML { .. } => None,
+        | ModelSelected::LoraGGML { .. }
+        | ModelSelected::Toml { .. } => None,
         ModelSelected::XLora {
             tgt_non_granular_index,
             ..
         }
         | ModelSelected::XLoraGGUF {
             tgt_non_granular_index,
             ..
@@ -64,16 +65,27 @@
             ..
         } => *tgt_non_granular_index,
     }
 }
 
 fn loader_from_model_selected(args: LoaderBuilder) -> anyhow::Result<Box<dyn Loader>> {
     let use_flash_attn = args.use_flash_attn;
-    let tgt_non_granular_index = get_tgt_non_granular_index(&args.model);
     let loader: Box<dyn Loader> = match args.model {
+        ModelSelected::Toml { file } => {
+            let selector: TomlSelector = toml::from_str(
+                &fs::read_to_string(file.clone())
+                    .unwrap_or_else(|_| panic!("Could not load toml selector file at {file}")),
+            )?;
+            let args = TomlLoaderArgs {
+                use_flash_attn,
+                chat_template: args.chat_template,
+                no_kv_cache: args.no_kv_cache,
+            };
+            (selector, args).try_into()?
+        }
         ModelSelected::Plain {
             model_id,
             repeat_last_n,
             tokenizer_json,
             arch,
         } => NormalLoaderBuilder::new(
             NormalSpecificConfig {
@@ -130,16 +142,14 @@
         )
         .with_lora(
             adapters_model_id,
             serde_json::from_reader(
                 File::open(order.clone())
                     .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
             )?,
-            args.no_kv_cache,
-            tgt_non_granular_index,
         )
         .build(arch),
         ModelSelected::GGUF {
             tok_model_id,
             tokenizer_json,
             quantized_model_id,
             quantized_filename,
@@ -184,31 +194,28 @@
             tok_model_id,
             tokenizer_json,
             quantized_model_id,
             quantized_filename,
             repeat_last_n,
             adapters_model_id,
             order,
-            tgt_non_granular_index,
         } => GGUFLoaderBuilder::new(
             GGUFSpecificConfig { repeat_last_n },
             args.chat_template,
             tokenizer_json,
             tok_model_id,
             quantized_model_id,
             quantized_filename,
         )
         .with_lora(
             adapters_model_id,
             serde_json::from_reader(
                 File::open(order.clone())
                     .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
             )?,
-            args.no_kv_cache,
-            tgt_non_granular_index,
         )
         .build(),
         ModelSelected::GGML {
             tok_model_id,
             tokenizer_json,
             quantized_model_id,
             quantized_filename,
@@ -255,15 +262,14 @@
             tok_model_id,
             tokenizer_json,
             quantized_model_id,
             quantized_filename,
             repeat_last_n,
             adapters_model_id,
             order,
-            tgt_non_granular_index,
             gqa,
         } => GGMLLoaderBuilder::new(
             GGMLSpecificConfig { repeat_last_n, gqa },
             args.chat_template,
             tokenizer_json,
             tok_model_id,
             quantized_model_id,
@@ -271,14 +277,12 @@
         )
         .with_lora(
             adapters_model_id,
             serde_json::from_reader(
                 File::open(order.clone())
                     .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
             )?,
-            args.no_kv_cache,
-            tgt_non_granular_index,
         )
         .build(),
     };
     Ok(loader)
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/model_selected.rs` & `mistralrs-0.1.5/mistralrs-core/src/model_selected.rs`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 fn parse_arch(x: &str) -> Result<NormalLoaderType, String> {
     x.parse()
 }
 
 #[derive(Debug, Subcommand)]
 pub enum ModelSelected {
+    /// Select the model from a toml file
+    Toml {
+        /// .toml file containing the selector configuration.
+        #[arg(short, long)]
+        file: String,
+    },
+
     /// Select a plain model, without quantization or adapters
     Plain {
         /// Model ID to load from. This may be a HF hub repo or a local path.
         #[arg(short, long)]
         model_id: String,
 
         /// Path to local tokenizer.json file. If this is specified it is used over any remote file.
@@ -78,15 +85,15 @@
         repeat_last_n: usize,
 
         /// Ordering JSON file
         #[arg(short, long)]
         order: String,
 
         /// The architecture of the model.
-        #[arg(short, long, value_parser = parse_arch)]
+        #[arg(long, value_parser = parse_arch)]
         arch: NormalLoaderType,
     },
 
     /// Select a GGUF model.
     GGUF {
         /// Model ID to load the tokenizer from. This may be a HF hub repo or a local path.
         #[arg(short, long)]
@@ -173,19 +180,14 @@
         /// Model ID to load X-LoRA from. This may be a HF hub repo or a local path.
         #[arg(short, long)]
         adapters_model_id: String,
 
         /// Ordering JSON file
         #[arg(short, long)]
         order: String,
-
-        /// Index of completion tokens to generate scalings up until. If this is 1, then there will be one completion token generated before it is cached.
-        /// This makes the maximum running sequences 1.
-        #[arg(long)]
-        tgt_non_granular_index: Option<usize>,
     },
 
     /// Select a GGML model.
     GGML {
         /// Model ID to load the tokenizer from. This may be a HF hub repo or a local path.
         #[arg(short, long)]
         tok_model_id: String,
@@ -280,17 +282,12 @@
         #[arg(short, long)]
         adapters_model_id: String,
 
         /// Ordering JSON file
         #[arg(short, long)]
         order: String,
 
-        /// Index of completion tokens to generate scalings up until. If this is 1, then there will be one completion token generated before it is cached.
-        /// This makes the maximum running sequences 1.
-        #[arg(long)]
-        tgt_non_granular_index: Option<usize>,
-
         /// GQA value
         #[arg(short, long, default_value_t = 1)]
         gqa: usize,
     },
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/gemma.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/gemma.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
 use candle_nn::{linear_b as linear, Activation, RotaryEmbedding, VarBuilder};
 use mistralrs_lora::layer::QLinear;
 
 use crate::{
     device_map::DeviceMapper,
+    layers::CausalMasker,
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv, Cache};
 
 fn default_max_position_embeddings() -> usize {
@@ -131,14 +132,15 @@
     o_proj: QLinear,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
+    neg_inf: Tensor,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
@@ -156,14 +158,15 @@
             o_proj: QLinear::from_linear(o_proj),
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
@@ -227,18 +230,16 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attention_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
-            };
+            let attn_weights =
+                CausalMasker.apply_mask(&attention_mask.cloned(), attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = attn_output
@@ -319,15 +320,14 @@
 
 #[derive(Debug)]
 pub struct Model {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QMatMul,
-    dtype: DType,
     hidden_size: usize,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
@@ -376,59 +376,32 @@
         let lm_head = QMatMul::Tensor(embed_tokens.embeddings().clone());
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head,
             device: real_device,
-            dtype: vb.dtype(),
             hidden_size: cfg.hidden_size,
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: default_max_position_embeddings(),
             mapper,
         })
     }
 
-    fn prepare_decoder_attention_mask(
-        &self,
-        b_size: usize,
-        tgt_len: usize,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| (0..tgt_len).map(move |j| if i < j { f32::NEG_INFINITY } else { 0. }))
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
-        let (b_size, seq_len) = input_ids.dims2()?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask = self.prepare_decoder_attention_mask(b_size, seq_len, seqlen_offsets[0])?;
-            Some(mask)
-        };
         let xs = self.embed_tokens.forward(input_ids)?;
         let mut xs = (xs * (self.hidden_size as f64).sqrt())?;
         let mut cache = self.cache.lock();
+        let attention_mask = CausalMasker.make_causal_mask(input_ids, &cache)?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/llama.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/llama.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use candle_core::{quantized::QMatMul, DType, Device, Result, Tensor, D};
 use candle_nn::{
     embedding, linear_no_bias as linear, Embedding, Module, RotaryEmbedding, VarBuilder,
 };
 use serde::Deserialize;
-use std::{collections::HashMap, sync::Arc};
+use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::RmsNorm,
+    layers::{CausalMasker, RmsNorm},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv};
 
 #[derive(Debug, Clone, Deserialize)]
@@ -27,62 +27,37 @@
     pub use_flash_attn: bool,
     pub rms_norm_eps: f64,
     pub rope_theta: f32,
     pub max_position_embeddings: usize,
 }
 
 #[derive(Debug, Clone)]
-pub struct Cache {
-    masks: HashMap<usize, Tensor>,
-}
-
-impl Cache {
-    pub fn new() -> Result<Self> {
-        Ok(Self {
-            masks: HashMap::new(),
-        })
-    }
-
-    fn mask(&mut self, t: usize, device: &Device) -> Result<Tensor> {
-        if let Some(mask) = self.masks.get(&t) {
-            mask.to_device(device)
-        } else {
-            let mask: Vec<_> = (0..t)
-                .flat_map(|i| (0..t).map(move |j| u8::from(j > i)))
-                .collect();
-            let mask = Tensor::from_slice(&mask, (t, t), device)?;
-            self.masks.insert(t, mask.clone());
-            Ok(mask)
-        }
-    }
-}
-
-#[derive(Debug, Clone)]
 struct CausalSelfAttention {
     q_proj: QMatMul,
     k_proj: QMatMul,
     v_proj: QMatMul,
     o_proj: QMatMul,
     num_attention_heads: usize,
     num_key_value_heads: usize,
     head_dim: usize,
     use_flash_attn: bool,
     rotary_emb: Arc<RotaryEmbedding>,
     max_seq_len: usize,
+    neg_inf: Tensor,
 }
 
 impl CausalSelfAttention {
     fn forward(
         &self,
         x: &Tensor,
+        attention_mask: &Option<Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         block_idx: usize,
         kv_cache: &mut super::LayerCaches,
-        cache: &mut Cache,
     ) -> Result<Tensor> {
         let (b_sz, seq_len, hidden_size) = x.dims3()?;
 
         let original_dtype = x.dtype();
         let mut x = x.clone();
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             x = x.to_dtype(DType::F32)?;
@@ -146,18 +121,15 @@
             flash_attn(&q, &k, &v, softmax_scale, seq_len > 1)?.transpose(1, 2)?
         } else {
             let in_dtype = q.dtype();
             let q = q.to_dtype(DType::F32)?;
             let k = k.to_dtype(DType::F32)?;
             let v = v.to_dtype(DType::F32)?;
             let att = (q.matmul(&k.t()?)? / (self.head_dim as f64).sqrt())?;
-            let mask = cache
-                .mask(seq_len, att.device())?
-                .broadcast_as(att.shape())?;
-            let att = masked_fill(&att, &mask, f32::NEG_INFINITY)?;
+            let att = CausalMasker.apply_mask(attention_mask, att, &self.neg_inf)?;
             let att = candle_nn::ops::softmax(&att, D::Minus1)?;
             // Convert to contiguous as matmul doesn't support strided vs for now.
             att.matmul(&v.contiguous()?)?.to_dtype(in_dtype)?
         };
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             y = y.to_dtype(DType::F32)?;
         }
@@ -184,25 +156,19 @@
             o_proj: QMatMul::Tensor(o_proj.weight().clone()),
             num_attention_heads: cfg.num_attention_heads,
             num_key_value_heads: cfg.num_key_value_heads,
             head_dim: cfg.hidden_size / cfg.num_attention_heads,
             use_flash_attn: cfg.use_flash_attn,
             rotary_emb: rope,
             max_seq_len: cfg.max_position_embeddings,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 }
 
-fn masked_fill(on_false: &Tensor, mask: &Tensor, on_true: f32) -> Result<Tensor> {
-    let shape = mask.shape();
-    let on_true = Tensor::new(on_true, on_false.device())?.broadcast_as(shape.dims())?;
-    let m = mask.where_cond(&on_true, on_false)?;
-    Ok(m)
-}
-
 #[derive(Debug, Clone)]
 struct Mlp {
     c_fc1: QMatMul,
     c_fc2: QMatMul,
     c_proj: QMatMul,
 }
 
@@ -243,29 +209,29 @@
     mlp: Mlp,
 }
 
 impl Block {
     fn forward(
         &self,
         x: &Tensor,
+        attention_mask: &Option<Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         block_idx: usize,
         kv_cache: &mut super::LayerCaches,
-        cache: &mut Cache,
     ) -> Result<Tensor> {
         let residual = x;
         let x = self.rms_1.forward(x)?;
         let x = (self.attn.forward(
             &x,
+            attention_mask,
             seqlen_offsets,
             start_offsets_kernel,
             block_idx,
             kv_cache,
-            cache,
         )? + residual)?;
         let residual = &x;
         let x = (self.mlp.forward(&self.rms_2.forward(&x)?)? + residual)?;
         Ok(x)
     }
 
     fn load(
@@ -305,37 +271,37 @@
 pub struct Llama {
     wte: Embedding,
     blocks: Vec<Block>,
     ln_f: RmsNorm,
     lm_head: QMatMul,
     pub kv_cache: super::Cache,
     pub device: Device,
-    cache: Cache,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl Llama {
     pub fn forward(
         &mut self,
-        x: &Tensor,
+        input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
-        let mut x = self.wte.forward(x)?;
+        let mut x = self.wte.forward(input_ids)?;
         let mut cache = self.kv_cache.lock();
+        let mask = CausalMasker.make_causal_mask(input_ids, &cache)?;
         for (block_idx, block) in self.blocks.iter().enumerate() {
             x = self.mapper.map(x, block_idx)?;
             x = block.forward(
                 &x,
+                &mask.clone().map(|m| m.to_device(x.device()).unwrap()),
                 seqlen_offsets,
                 start_offsets_kernel.clone(),
                 block_idx,
                 &mut cache,
-                &mut self.cache,
             )?;
         }
         let x = x.to_device(&self.device)?;
         let mut x = self.ln_f.forward(&x)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             x = x.to_dtype(DType::F32)?;
         }
@@ -394,15 +360,14 @@
             .collect();
 
         Ok(Self {
             wte,
             blocks,
             ln_f,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
-            cache: Cache::new()?,
             kv_cache: super::Cache::new(cfg.num_hidden_layers, false),
             device: real_device,
             mapper,
         })
     }
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/mistral.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/mistral.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 /// Mistral LLM, https://github.com/mistralai/mistral-src
-use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
 use candle_nn::{linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
 use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::RmsNorm,
+    layers::{CausalMasker, RmsNorm},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv, Cache};
 
 #[derive(Debug, Clone, PartialEq)]
@@ -82,14 +82,15 @@
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     hidden_size: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
     sliding_window: Option<usize>,
+    neg_inf: Tensor,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
@@ -108,14 +109,15 @@
             num_kv_heads,
             num_kv_groups,
             head_dim,
             hidden_size: hidden_sz,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
             sliding_window: cfg.sliding_window,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
@@ -207,18 +209,15 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attn_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(&mask)?,
-            };
+            let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = attn_output
@@ -300,15 +299,14 @@
 #[derive(Debug)]
 pub struct Model {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QMatMul,
     sliding_window: Option<usize>,
-    dtype: DType,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl Model {
@@ -362,89 +360,34 @@
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
             sliding_window: cfg.sliding_window,
             device: real_device,
-            dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             mapper,
         })
     }
 
-    fn prepare_decoder_attention_mask(
-        &self,
-        b_size: usize,
-        tgt_len: usize,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        // Sliding window mask
-        let sliding_window = self.sliding_window.unwrap_or(tgt_len + 1);
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| {
-                (0..tgt_len).map(move |j| {
-                    if i < j || j + sliding_window < i {
-                        f32::NEG_INFINITY
-                    } else {
-                        0.
-                    }
-                })
-            })
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
-    fn calculate_past_kv_len(&mut self, seq_len: usize) -> Result<usize> {
-        let cache = self.cache.lock();
-        let kv_cache_1 = cache.first().unwrap();
-        if kv_cache_1.is_none() {
-            return Ok(0);
-        }
-        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
-        if k_cache_1.dims()[0] <= seq_len {
-            Ok(0)
-        } else {
-            let indexed = k_cache_1.i(seq_len)?;
-            let dims = indexed.dims();
-            Ok(dims[dims.len() - 2])
-        }
-    }
-
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
-        let (b_size, seq_len) = input_ids.dims2()?;
-        if seqlen_offsets.len() > b_size {
-            candle_core::bail!("Expected seqlen offsets have length equal to batch size.")
-        }
-
-        let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask =
-                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
-            Some(mask)
-        };
         let mut xs = self.embed_tokens.forward(input_ids)?;
         let mut cache = self.cache.lock();
+        let attention_mask = CausalMasker.make_causal_mask_with_sliding_window(
+            input_ids,
+            &cache,
+            self.sliding_window,
+        )?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/mixtral.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/mixtral.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 /// Mixtral Model
 /// https://github.com/huggingface/transformers/blob/main/src/transformers/models/mixtral/modeling_mixtral.py
 /// https://mistral.ai/news/mixtral-of-experts/
-use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
 use candle_nn::{linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
 use serde::Deserialize;
 use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::RmsNorm,
+    layers::{CausalMasker, RmsNorm},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv, Cache};
 
 /// https://github.com/huggingface/transformers/blob/1a585c1222a56bcaecc070966d558d4a9d862e83/src/transformers/models/mixtral/configuration_mixtral.py#L113
@@ -46,14 +46,15 @@
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     hidden_size: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
     sliding_window: Option<usize>,
+    neg_inf: Tensor,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
@@ -72,14 +73,15 @@
             num_kv_heads,
             num_kv_groups,
             head_dim,
             hidden_size: hidden_sz,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
             sliding_window: Some(cfg.sliding_window),
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
@@ -171,18 +173,15 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attn_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(&mask)?,
-            };
+            let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = attn_output
@@ -405,15 +404,14 @@
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QMatMul,
     sliding_window: usize,
     pub device: Device,
     pub cache: Cache,
-    dtype: DType,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl Model {
     pub fn new(
         cfg: &Config,
@@ -465,84 +463,34 @@
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
             sliding_window: cfg.sliding_window,
             device: real_device,
-            dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             mapper,
         })
     }
 
-    fn calculate_past_kv_len(&mut self, seq_len: usize) -> Result<usize> {
-        let cache = self.cache.lock();
-        let kv_cache_1 = cache.first().unwrap();
-        if kv_cache_1.is_none() {
-            return Ok(0);
-        }
-        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
-        if k_cache_1.dims()[0] <= seq_len {
-            Ok(0)
-        } else {
-            let indexed = k_cache_1.i(seq_len)?;
-            let dims = indexed.dims();
-            Ok(dims[dims.len() - 2])
-        }
-    }
-
-    fn prepare_decoder_attention_mask(
-        &self,
-        b_size: usize,
-        tgt_len: usize,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        // Sliding window mask?
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| {
-                (0..tgt_len).map(move |j| {
-                    if i < j || j + self.sliding_window < i {
-                        f32::NEG_INFINITY
-                    } else {
-                        0.
-                    }
-                })
-            })
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
-        let (b_size, seq_len) = input_ids.dims2()?;
-        let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask =
-                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
-            Some(mask)
-        };
         let mut xs = self.embed_tokens.forward(input_ids)?;
         let mut cache = self.cache.lock();
+        let attention_mask = CausalMasker.make_causal_mask_with_sliding_window(
+            input_ids,
+            &cache,
+            Some(self.sliding_window),
+        )?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/mod.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -8,46 +8,53 @@
 pub(crate) mod llama;
 pub(crate) mod mistral;
 pub(crate) mod mixtral;
 pub(crate) mod phi2;
 pub(crate) mod phi3;
 pub(crate) mod quantized_llama;
 pub(crate) mod quantized_phi2;
+pub(crate) mod quantized_phi3;
 pub(crate) mod qwen2;
 
 pub type LayerCaches = Vec<Option<(Tensor, Tensor)>>;
 
 #[derive(Debug, Clone)]
 pub struct Cache {
     cache: Arc<Mutex<LayerCaches>>,
     xlora_cache: Option<Arc<Mutex<LayerCaches>>>,
+    draft_cache: Arc<Mutex<LayerCaches>>,
     scalings_cache: Option<Arc<Mutex<Option<Tensor>>>>,
 }
 
 impl Cache {
     pub(crate) fn new(len: usize, is_xlora: bool) -> Self {
         Self {
             cache: Arc::new(Mutex::new(vec![None; len])),
             xlora_cache: if is_xlora {
                 Some(Arc::new(Mutex::new(vec![None; len])))
             } else {
                 None
             },
+            draft_cache: Arc::new(Mutex::new(vec![None; len])),
             scalings_cache: if is_xlora {
                 Some(Arc::new(Mutex::new(None)))
             } else {
                 None
             },
         }
     }
 
     pub(crate) fn lock(&self) -> MutexGuard<'_, LayerCaches> {
         get_mut_arcmutex!(self.cache)
     }
 
+    pub(crate) fn draft_lock(&self) -> MutexGuard<'_, LayerCaches> {
+        get_mut_arcmutex!(self.draft_cache)
+    }
+
     /// # Panics
     /// If there is no xlora cache
     pub(crate) fn xlora_lock(&self) -> MutexGuard<'_, LayerCaches> {
         get_mut_arcmutex!(self.xlora_cache.as_ref().expect("No X-LoRA cache."))
     }
 
     /// # Panics
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/phi2.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/phi2.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     embedding, layer_norm, linear, Activation, Embedding, LayerNorm, RotaryEmbedding, VarBuilder,
 };
 use mistralrs_lora::layer::QLinear;
 use serde::Deserialize;
 
 use crate::{
     device_map::DeviceMapper,
+    layers::CausalMasker,
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv, Cache};
 
 // https://huggingface.co/microsoft/phi-2/blob/main/configuration_phi.py
@@ -96,28 +97,15 @@
     k_layernorm: Option<LayerNorm>,
     rotary_emb: RotaryEmbedding,
     softmax_scale: f64,
     num_heads: usize,
     num_kv_heads: usize,
     head_dim: usize,
     use_flash_attn: bool,
-}
-
-fn get_mask(size: usize, device: &Device) -> Result<Tensor> {
-    let mask: Vec<_> = (0..size)
-        .flat_map(|i| (0..size).map(move |j| u8::from(j > i)))
-        .collect();
-    Tensor::from_slice(&mask, (size, size), device)
-}
-
-fn masked_fill(on_false: &Tensor, mask: &Tensor, on_true: f32) -> Result<Tensor> {
-    let shape = mask.shape();
-    let on_true = Tensor::new(on_true, on_false.device())?.broadcast_as(shape.dims())?;
-    let m = mask.where_cond(&on_true, on_false)?;
-    Ok(m)
+    neg_inf: Tensor,
 }
 
 impl Attention {
     fn new(cfg: &Config, vb: VarBuilder, rope: RotaryEmbedding) -> Result<Self> {
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads();
         let head_dim = cfg.head_dim();
@@ -142,14 +130,15 @@
             k_layernorm,
             rotary_emb: rope,
             softmax_scale,
             num_heads,
             num_kv_heads,
             head_dim,
             use_flash_attn: cfg.use_flash_attn,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         mask: Option<&Tensor>,
@@ -228,22 +217,16 @@
             flash_attn(&q, &k, &v, self.softmax_scale as f32, seq_len > 1)?.transpose(1, 2)?
         } else {
             let attn_weights = (q
                 .to_dtype(DType::F32)?
                 .contiguous()?
                 .matmul(&k.to_dtype(DType::F32)?.t()?)?
                 * self.softmax_scale)?;
-            let attn_weights = match mask {
-                None => attn_weights,
-                Some(mask) => masked_fill(
-                    &attn_weights,
-                    &mask.broadcast_left((b_size, self.num_heads))?,
-                    f32::NEG_INFINITY,
-                )?,
-            };
+            let attn_weights =
+                CausalMasker.apply_mask(&mask.cloned(), attn_weights, &self.neg_inf)?;
             let attn_weights =
                 candle_nn::ops::softmax_last_dim(&attn_weights)?.to_dtype(v.dtype())?;
             attn_weights.matmul(&v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
@@ -380,27 +363,22 @@
             max_seq_len: cfg.max_position_embeddings,
             mapper,
         })
     }
 
     pub fn forward(
         &mut self,
-        xs: &Tensor,
+        input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
-        let (_b_size, seq_len) = xs.dims2()?;
-        let mut xs = xs.apply(&self.embed_tokens)?;
-        let mask = if seq_len <= 1 {
-            None
-        } else {
-            Some(get_mask(seq_len, xs.device())?)
-        };
+        let mut xs = input_ids.apply(&self.embed_tokens)?;
         let mut cache = self.cache.lock();
+        let mask = CausalMasker.make_causal_mask(input_ids, &cache)?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 mask.as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/phi3.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/phi3.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 // This implementation is based on:
 // https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/modeling_phi3.py
-use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
 use candle_nn::{linear_no_bias, VarBuilder};
 use either::Either;
 use std::{collections::HashMap, sync::Arc};
 
 use crate::{
     device_map::DeviceMapper,
-    layers::{PhiRotaryEmbedding, RmsNorm},
+    layers::{CausalMasker, PhiRotaryEmbedding, RmsNorm},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv, Cache};
 
 // https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/config.json
@@ -50,14 +50,15 @@
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<PhiRotaryEmbedding>,
     use_flash_attn: bool,
     sliding_window: Option<usize>,
+    neg_inf: Tensor,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<PhiRotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let head_dim = cfg.head_dim();
@@ -70,14 +71,15 @@
             rotary_emb,
             num_heads,
             num_kv_heads,
             num_kv_groups: num_heads / num_kv_heads,
             head_dim,
             use_flash_attn: cfg.use_flash_attn,
             sliding_window: cfg.sliding_window,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
@@ -167,18 +169,15 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attn_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(&mask)?,
-            };
+            let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = attn_output
@@ -297,15 +296,14 @@
 
 #[derive(Debug)]
 pub struct Model {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QMatMul,
-    dtype: DType,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
     sliding_window: Option<usize>,
 }
 
@@ -355,97 +353,41 @@
         )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
             device: real_device,
-            dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             mapper,
             sliding_window: cfg.sliding_window,
         })
     }
 
-    fn prepare_decoder_attention_mask(
-        &self,
-        b_size: usize,
-        tgt_len: usize,
-        seqlen_offset: usize,
-        sliding_window: Option<usize>,
-    ) -> Result<Tensor> {
-        // Sliding window mask
-        let sliding_window = sliding_window.unwrap_or(tgt_len + 1);
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| {
-                (0..tgt_len).map(move |j| {
-                    if i < j || j + sliding_window < i {
-                        f32::NEG_INFINITY
-                    } else {
-                        0.
-                    }
-                })
-            })
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
-    fn calculate_past_kv_len(&mut self, seq_len: usize) -> Result<usize> {
-        let cache = self.cache.lock();
-        let kv_cache_1 = cache.first().unwrap();
-        if kv_cache_1.is_none() {
-            return Ok(0);
-        }
-        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
-        if k_cache_1.dims()[0] <= seq_len {
-            Ok(0)
-        } else {
-            let indexed = k_cache_1.i(seq_len)?;
-            let dims = indexed.dims();
-            Ok(dims[dims.len() - 2])
-        }
-    }
-
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         position_ids: &[usize],
         context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
-        let (b_size, seq_len) = input_ids.dims2()?;
-        let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask = self.prepare_decoder_attention_mask(
-                b_size,
-                seq_len,
-                past_key_values_length,
-                self.sliding_window,
-            )?;
-            Some(mask)
-        };
-        let position_ids_old = position_ids;
-        let mut position_ids = Vec::new();
-        for p in position_ids_old {
-            position_ids.push(*p + past_key_values_length);
-        }
-
         let mut xs = self.embed_tokens.forward(input_ids)?;
         let mut cache = self.cache.lock();
+        let attention_mask = CausalMasker.make_causal_mask_with_sliding_window(
+            input_ids,
+            &cache,
+            self.sliding_window,
+        )?;
+        let past_key_values_length = CausalMasker.calculate_past_kv_len(&cache)?;
+        let position_ids = position_ids
+            .iter()
+            .map(|p| *p + past_key_values_length)
+            .collect::<Vec<_>>();
+
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/quantized_llama.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/quantized_llama.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-use std::collections::HashMap;
-
 use candle_core::quantized::QMatMul;
 use candle_core::quantized::{ggml_file, gguf_file};
 use candle_core::{DType, Device, Result, Tensor};
 use candle_nn::{Embedding, Module, RotaryEmbedding};
 
 use crate::device_map::DeviceMapper;
-use crate::layers::QRmsNorm;
+use crate::layers::{CausalMasker, QRmsNorm};
 use crate::pipeline::extract_logits;
 use crate::DeviceMapMetadata;
 
 use super::{repeat_kv, verify_sanity_gguf, Cache};
 
 const MAX_SEQ_LEN: u32 = 4096;
 
@@ -124,20 +122,14 @@
     n_head: usize,
     n_kv_head: usize,
     head_dim: usize,
     rotary: RotaryEmbedding,
     neg_inf: Tensor,
 }
 
-fn masked_fill(on_false: &Tensor, mask: &Tensor, on_true: &Tensor) -> Result<Tensor> {
-    let shape = mask.shape();
-    let m = mask.where_cond(&on_true.broadcast_as(shape.dims())?, on_false)?;
-    Ok(m)
-}
-
 impl LayerWeights {
     fn forward_attn(
         &mut self,
         x: &Tensor,
         mask: &Option<Tensor>,
         start_offsets: &[usize],
         start_offsets_kernel: Tensor,
@@ -177,21 +169,15 @@
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.n_head / self.n_kv_head)?.contiguous()?;
         let v = repeat_kv(v, self.n_head / self.n_kv_head)?.contiguous()?;
 
         let att = (q.contiguous()?.matmul(&k.t()?.contiguous()?)? / (self.head_dim as f64).sqrt())?;
-        let att = match mask {
-            None => att,
-            Some(mask) => {
-                let mask = mask.broadcast_as(att.shape())?;
-                masked_fill(&att, &mask, &self.neg_inf)?
-            }
-        };
+        let att = CausalMasker.apply_mask(mask, att, &self.neg_inf)?;
         let att = candle_nn::ops::softmax_last_dim(&att)?;
         // Convert to contiguous as matmul doesn't support strided vs for now.
         let y = att.matmul(&v.contiguous()?)?;
         let y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, n_embd])?;
         let y = self.attention_wo.forward(&y)?;
         Ok(y)
     }
@@ -199,15 +185,14 @@
 
 #[derive(Debug)]
 pub struct ModelWeights {
     tok_embeddings: Embedding,
     layers: Vec<LayerWeights>,
     norm: QRmsNorm,
     output: QMatMul,
-    masks: HashMap<usize, Tensor>,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Option<Box<dyn DeviceMapper + Send + Sync>>,
 }
 
 impl ModelWeights {
@@ -262,15 +247,14 @@
             })
         }
         Ok(Self {
             tok_embeddings: Embedding::new(tok_embeddings, ct.hparams.n_embd as usize),
             layers,
             norm,
             output: QMatMul::from_qtensor(output)?,
-            masks: HashMap::new(),
             device: ct.device.clone(),
             cache: Cache::new(ct.hparams.n_layer as usize, false),
             max_seq_len: MAX_SEQ_LEN as usize, // Cannot determine from ggml.
             mapper: None,
         })
     }
 
@@ -394,50 +378,31 @@
             })
         }
         Ok(Self {
             tok_embeddings: Embedding::new(tok_embeddings, embedding_length),
             layers,
             norm,
             output: QMatMul::from_qtensor(output)?,
-            masks: HashMap::new(),
             device: device.clone(),
             cache: Cache::new(block_count, false),
             max_seq_len,
             mapper: Some(mapper),
         })
     }
 
-    fn mask(&mut self, t: usize, device: &Device) -> Result<Tensor> {
-        if let Some(mask) = self.masks.get(&t) {
-            Ok(mask.clone())
-        } else {
-            let mask: Vec<_> = (0..t)
-                .flat_map(|i| (0..t).map(move |j| u8::from(j > i)))
-                .collect();
-            let mask = Tensor::from_slice(&mask, (t, t), device)?;
-            self.masks.insert(t, mask.clone());
-            Ok(mask)
-        }
-    }
-
     pub fn forward(
         &mut self,
         x: &Tensor,
         start_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
-        let (_b_sz, seq_len) = x.dims2()?;
-        let mask = if seq_len == 1 {
-            None
-        } else {
-            Some(self.mask(seq_len, x.device())?)
-        };
         let mut layer_in = self.tok_embeddings.forward(x)?;
         let mut cache = self.cache.lock();
+        let mask = CausalMasker.make_causal_mask(x, &cache)?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
             if let Some(ref mapper) = self.mapper {
                 layer_in = mapper.map(layer_in, i)?;
             }
             let x = layer_in;
             let residual = &x;
             let x = layer.attention_norm.forward(&x)?;
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/quantized_phi2.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/quantized_phi2.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-use std::collections::HashMap;
-
 use candle_core::quantized::gguf_file;
 use candle_core::quantized::QTensor;
 use candle_core::{DType, Device, IndexOp, Module, Result, Tensor, D};
 use candle_nn::{Embedding, LayerNorm};
 use mistralrs_lora::layer::QLinear;
 
 use crate::device_map::DeviceMapper;
+use crate::layers::CausalMasker;
+use crate::pipeline::extract_logits;
 use crate::DeviceMapMetadata;
 
 use super::repeat_kv;
 use super::Cache;
 
 pub const MAX_SEQ_LEN: usize = 4096;
 
@@ -39,20 +39,14 @@
     head_dim: usize,
     cos: Tensor,
     sin: Tensor,
     rope_dim: usize,
     neg_inf: Tensor,
 }
 
-fn masked_fill(on_false: &Tensor, mask: &Tensor, on_true: &Tensor) -> Result<Tensor> {
-    let shape = mask.shape();
-    let m = mask.where_cond(&on_true.broadcast_as(shape.dims())?, on_false)?;
-    Ok(m)
-}
-
 impl LayerWeights {
     fn forward(&self, xs: &Tensor, start_offsets: &[usize]) -> Result<Tensor> {
         let (_b_sz, _n_head, seq_len, _n_embd) = xs.dims4()?;
         let xs_rot = xs.i((.., .., .., ..self.rope_dim))?;
         let xs_pass = xs.i((.., .., .., self.rope_dim..))?;
         let mut chunks = Vec::new();
         for (b, offset) in (0..xs.dim(0)?).zip(start_offsets) {
@@ -99,21 +93,15 @@
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.n_head / self.n_kv_head)?;
         let v = repeat_kv(v, self.n_head / self.n_kv_head)?;
 
         let att = (q.matmul(&k.t()?)? / (self.head_dim as f64).sqrt())?;
-        let att = match mask {
-            None => att,
-            Some(mask) => {
-                let mask = mask.broadcast_as(att.shape())?;
-                masked_fill(&att, &mask, &self.neg_inf)?
-            }
-        };
+        let att = CausalMasker.apply_mask(&mask.cloned(), att, &self.neg_inf)?;
         let att = candle_nn::ops::softmax_last_dim(&att)?;
         // Convert to contiguous as matmul doesn't support strided vs for now.
         let y = att.matmul(&v.contiguous()?)?;
         let y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, n_embd])?;
         let y = self.attn_output.forward(&y)?;
         Ok(y)
     }
@@ -121,15 +109,14 @@
 
 #[derive(Debug)]
 pub struct ModelWeights {
     tok_embeddings: Embedding,
     layers: Vec<LayerWeights>,
     output_norm: LayerNorm,
     output: QLinear,
-    masks: HashMap<usize, Tensor>,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 fn precomput_freqs_cis(
@@ -221,49 +208,30 @@
             })
         }
         Ok(Self {
             tok_embeddings: Embedding::new(tok_embeddings, embedding_length),
             layers,
             output_norm,
             output,
-            masks: HashMap::new(),
             device: device.clone(),
             cache: Cache::new(block_count, false),
             max_seq_len,
             mapper,
         })
     }
 
-    fn mask(&mut self, t: usize, device: &Device) -> Result<Tensor> {
-        if let Some(mask) = self.masks.get(&t) {
-            Ok(mask.clone())
-        } else {
-            let mask: Vec<_> = (0..t)
-                .flat_map(|i| (0..t).map(move |j| u8::from(j > i)))
-                .collect();
-            let mask = Tensor::from_slice(&mask, (t, t), device)?;
-            self.masks.insert(t, mask.clone());
-            Ok(mask)
-        }
-    }
-
     pub fn forward(
         &mut self,
-        xs: &Tensor,
+        input_ids: &Tensor,
         seqlen_offsets: &[usize],
-        _context_lens: Vec<(usize, usize)>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
-        let (_b_sz, seq_len) = xs.dims2()?;
-        let mask = if seq_len == 1 {
-            None
-        } else {
-            Some(self.mask(seq_len, xs.device())?)
-        };
-        let mut xs = self.tok_embeddings.forward(xs)?;
+        let mut xs = self.tok_embeddings.forward(input_ids)?;
         let mut cache = self.cache.lock();
+        let mask = CausalMasker.make_causal_mask(input_ids, &cache)?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             let residual = &xs;
             let xs_norm = xs.apply(&layer.attn_norm)?;
             let attn_outputs = layer.forward_attn(
                 &xs_norm,
                 mask.as_ref()
@@ -272,11 +240,11 @@
                 seqlen_offsets,
                 cache.get_mut(i).unwrap(),
             )?;
             let feed_forward_hidden_states = layer.mlp.forward(&xs_norm)?;
             xs = (attn_outputs + feed_forward_hidden_states + residual)?
         }
         let xs = xs.to_device(&self.device)?;
-        let xs = xs.apply(&self.output_norm)?.i((.., seq_len - 1, ..))?;
+        let xs = extract_logits(&xs.apply(&self.output_norm)?, context_lens)?;
         self.output.forward(&xs)
     }
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/models/qwen2.rs` & `mistralrs-0.1.5/mistralrs-core/src/models/qwen2.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor};
 use candle_nn::{linear, linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
 use mistralrs_lora::layer::QLinear;
 use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::RmsNorm,
+    layers::{CausalMasker, RmsNorm},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{flash_attn, repeat_kv, Cache};
 
 #[derive(Debug, Clone, PartialEq, serde::Deserialize)]
@@ -83,14 +83,15 @@
     o_proj: QMatMul,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
+    neg_inf: Tensor,
 }
 
 impl Attention {
     fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
@@ -107,14 +108,15 @@
             o_proj: QMatMul::Tensor(o_proj.weight().clone()),
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
@@ -178,18 +180,16 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attention_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
-            };
+            let attn_weights =
+                CausalMasker.apply_mask(&attention_mask.cloned(), attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = attn_output
@@ -271,15 +271,14 @@
 #[derive(Debug)]
 pub struct Model {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QMatMul,
     sliding_window: usize,
-    dtype: DType,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl Model {
@@ -333,84 +332,34 @@
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
             sliding_window: cfg.sliding_window,
             device: real_device,
-            dtype: vb.dtype(),
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             mapper,
         })
     }
 
-    fn prepare_decoder_attention_mask(
-        &self,
-        b_size: usize,
-        tgt_len: usize,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        // Sliding window mask?
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| {
-                (0..tgt_len).map(move |j| {
-                    if i < j || j + self.sliding_window < i {
-                        f32::NEG_INFINITY
-                    } else {
-                        0.
-                    }
-                })
-            })
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
-    fn calculate_past_kv_len(&mut self, seq_len: usize) -> Result<usize> {
-        let cache = self.cache.lock();
-        let kv_cache_1 = cache.first().unwrap();
-        if kv_cache_1.is_none() {
-            return Ok(0);
-        }
-        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
-        if k_cache_1.dims()[0] <= seq_len {
-            Ok(0)
-        } else {
-            let indexed = k_cache_1.i(seq_len)?;
-            let dims = indexed.dims();
-            Ok(dims[dims.len() - 2])
-        }
-    }
-
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
-        let (b_size, seq_len) = input_ids.dims2()?;
-        let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask =
-                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
-            Some(mask)
-        };
         let mut xs = self.embed_tokens.forward(input_ids)?;
         let mut cache = self.cache.lock();
+        let attention_mask = CausalMasker.make_causal_mask_with_sliding_window(
+            input_ids,
+            &cache,
+            Some(self.sliding_window),
+        )?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/pipeline/chat_template.rs` & `mistralrs-0.1.5/mistralrs-core/src/pipeline/chat_template.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/pipeline/ggml.rs` & `mistralrs-0.1.5/mistralrs-core/src/pipeline/ggml.rs`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
 use crate::models::Cache;
 use crate::pipeline::chat_template::calculate_eos_tokens;
 use crate::pipeline::{ChatTemplate, SimpleModelPaths};
 use crate::prefix_cacher::PrefixCacheManager;
 use crate::sequence::Sequence;
-use crate::utils::varbuilder_utils::from_mmaped_safetensors;
+use crate::utils::varbuilder_utils::{from_mmaped_safetensors, load_preload_adapters};
 use crate::xlora_models::NonGranularState;
 use crate::{deserialize_chat_template, do_sample, get_mut_arcmutex, get_paths, DeviceMapMetadata};
 use crate::{
     models::quantized_llama::ModelWeights as QLlama, utils::tokens::get_token,
-    xlora_models::XLoraModelWeights as XLoraQLlama,
+    xlora_models::XLoraQLlama,
 };
 use anyhow::Result;
 use candle_core::quantized::{ggml_file, GgmlDType};
 use candle_core::{DType, Device, Tensor};
 use hf_hub::{api::sync::ApiBuilder, Repo, RepoType};
 use mistralrs_lora::Ordering;
 use rand_isaac::Isaac64Rng;
@@ -27,15 +27,15 @@
 use std::collections::HashMap;
 use std::fs;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
 use tokenizers::Tokenizer;
 use tokio::sync::Mutex;
-use tracing::info;
+use tracing::{info, warn};
 
 enum Model {
     Llama(QLlama),
     XLoraLlama(XLoraQLlama),
 }
 
 pub struct GGMLPipeline {
@@ -142,28 +142,17 @@
             xlora_model_id,
             xlora_order,
             no_kv_cache,
             tgt_non_granular_index,
         )
     }
 
-    pub fn with_lora(
-        mut self,
-        xlora_model_id: String,
-        xlora_order: Ordering,
-        no_kv_cache: bool,
-        tgt_non_granular_index: Option<usize>,
-    ) -> Self {
+    pub fn with_lora(mut self, lora_model_id: String, lora_order: Ordering) -> Self {
         self.kind = ModelKind::LoraGGML;
-        self.with_adapter(
-            xlora_model_id,
-            xlora_order,
-            no_kv_cache,
-            tgt_non_granular_index,
-        )
+        self.with_adapter(lora_model_id, lora_order, false, None)
     }
 
     pub fn build(self) -> Box<dyn Loader> {
         Box::new(GGMLLoader {
             model_id: self.model_id.unwrap(),
             config: self.config,
             xlora_model_id: self.xlora_model_id,
@@ -244,15 +233,15 @@
 
         if in_situ_quant.is_some() {
             anyhow::bail!(
                 "You are trying to in-situ quantize a GGUF model. This will not do anything."
             );
         }
         if !mapper.is_dummy() {
-            info!("⚠️ WARNING: GGML models do not support device mapping. Device mapping will not work. Please consider using a GGUF model.");
+            warn!("GGML models do not support device mapping. Device mapping will not work. Please consider using a GGUF model.");
         }
 
         let mut file = std::fs::File::open(paths.get_weight_filenames().first().unwrap())?;
         let model = ggml_file::Content::read(&mut file, device)
             .map_err(|e| e.with_path(paths.get_weight_filenames().first().unwrap()))?;
 
         info!("Model config: {:?}", model.hparams);
@@ -278,14 +267,20 @@
                 Model::XLoraLlama(XLoraQLlama::from_ggml(
                     model,
                     self.config.gqa,
                     paths.get_adapter_configs().as_ref().unwrap(),
                     &vb,
                     paths.get_ordering().as_ref().unwrap(),
                     Some(paths.get_classifier_config().as_ref().unwrap().clone()),
+                    &load_preload_adapters(
+                        paths.get_lora_preload_adapter_info(),
+                        DType::F32,
+                        device,
+                        silent,
+                    )?,
                 )?)
             }
             ModelKind::LoraGGML => {
                 is_lora = true;
                 let vb = from_mmaped_safetensors(
                     vec![],
                     paths
@@ -303,14 +298,20 @@
                 Model::XLoraLlama(XLoraQLlama::from_ggml(
                     model,
                     self.config.gqa,
                     paths.get_adapter_configs().as_ref().unwrap(),
                     &vb,
                     paths.get_ordering().as_ref().unwrap(),
                     None,
+                    &load_preload_adapters(
+                        paths.get_lora_preload_adapter_info(),
+                        DType::F32,
+                        device,
+                        silent,
+                    )?,
                 )?)
             }
             _ => unreachable!(),
         };
 
         let tokenizer =
             Tokenizer::from_file(paths.get_tokenizer_filename()).map_err(anyhow::Error::msg)?;
@@ -348,14 +349,15 @@
                 max_seq_len,
                 repeat_last_n: self.config.repeat_last_n,
                 tok_trie,
                 has_no_kv_cache: self.no_kv_cache,
                 is_xlora,
                 num_hidden_layers,
                 eos_tok: eos,
+                is_lora,
             },
         })))
     }
 
     fn get_id(&self) -> String {
         self.xlora_model_id
             .as_deref()
@@ -438,26 +440,37 @@
         anyhow::bail!(
             "You are trying to in-situ requantize a GGML model. This will not do anything."
         )
     }
     fn get_metadata(&self) -> &GeneralMetadata {
         &self.metadata
     }
-    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence]) {
-        DefaultCacheManager.clone_in_cache(self, seqs)
+    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence], modify_draft_cache: bool) {
+        DefaultCacheManager.clone_in_cache(self, seqs, modify_draft_cache)
     }
-    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence]) {
-        DefaultCacheManager.clone_out_cache(self, seqs)
+    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence], modify_draft_cache: bool) {
+        DefaultCacheManager.clone_out_cache(self, seqs, modify_draft_cache)
     }
-    fn set_none_cache(&mut self, reset_non_granular: bool) {
-        DefaultCacheManager.set_none_cache(self);
+    fn set_none_cache(&mut self, reset_non_granular: bool, modify_draft_cache: bool) {
+        DefaultCacheManager.set_none_cache(self, modify_draft_cache);
         if reset_non_granular {
             self.reset_non_granular_state()
         }
     }
     fn cache(&self) -> &Cache {
         match self.model {
             Model::Llama(ref model) => &model.cache,
             Model::XLoraLlama(ref model) => &model.cache,
         }
     }
+    fn activate_adapters(&mut self, adapter_names: Vec<String>) -> anyhow::Result<usize> {
+        if !self.metadata.is_lora {
+            anyhow::bail!("Cannot activate adapters non-LoRA models.")
+        }
+        match self.model {
+            Model::Llama(_) => unreachable!(),
+            Model::XLoraLlama(ref mut model) => model
+                .activate_adapters(adapter_names)
+                .map_err(anyhow::Error::msg),
+        }
+    }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/pipeline/gguf.rs` & `mistralrs-0.1.5/mistralrs-core/src/pipeline/gguf.rs`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
 use crate::models::Cache;
 use crate::pipeline::chat_template::calculate_eos_tokens;
 use crate::pipeline::{ChatTemplate, SimpleModelPaths};
 use crate::prefix_cacher::PrefixCacheManager;
 use crate::sequence::Sequence;
-use crate::utils::varbuilder_utils::from_mmaped_safetensors;
+use crate::utils::varbuilder_utils::{from_mmaped_safetensors, load_preload_adapters};
 use crate::xlora_models::NonGranularState;
 use crate::{deserialize_chat_template, do_sample, get_mut_arcmutex, get_paths, DeviceMapMetadata};
 use crate::{
-    models::quantized_llama::ModelWeights as QLlama, models::quantized_phi2::ModelWeights as QPhi,
-    utils::tokens::get_token, xlora_models::XLoraModelWeights as XLoraQLlama,
+    models::quantized_llama::ModelWeights as QLlama,
+    models::quantized_phi2::ModelWeights as QPhi,
+    models::quantized_phi3::ModelWeights as QPhi3,
+    utils::tokens::get_token,
+    xlora_models::{XLoraQLlama, XLoraQPhi3},
 };
 use anyhow::{bail, Result};
 use candle_core::quantized::{
     gguf_file::{self, Value as GgufValue},
     GgmlDType,
 };
 use candle_core::{DType, Device, Tensor};
@@ -36,14 +39,16 @@
 use tokio::sync::Mutex;
 use tracing::info;
 
 enum Model {
     Llama(QLlama),
     Phi2(QPhi),
     XLoraLlama(XLoraQLlama),
+    XLoraPhi3(XLoraQPhi3),
+    Phi3(QPhi3),
 }
 
 pub struct GGUFPipeline {
     model: Model,
     tokenizer: Arc<Tokenizer>,
     tok_trie: Arc<TokTrie>,
     no_kv_cache: bool,
@@ -75,14 +80,15 @@
     Gptj,
     Gpt2,
     Bloom,
     Falcon,
     Mamba,
     Rwkv,
     Phi2,
+    Phi3,
 }
 
 impl FromStr for GGUFArchitecture {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         match s {
@@ -92,14 +98,15 @@
             "gptj" => Ok(GGUFArchitecture::Gptj),
             "gpt2" => Ok(GGUFArchitecture::Gpt2),
             "bloom" => Ok(GGUFArchitecture::Bloom),
             "falcon" => Ok(GGUFArchitecture::Falcon),
             "mamba" => Ok(GGUFArchitecture::Mamba),
             "rwkv" => Ok(GGUFArchitecture::Rwkv),
             "phi2" => Ok(GGUFArchitecture::Phi2),
+            "phi3" => Ok(GGUFArchitecture::Phi3),
             a => Err(format!("Unknown GGUF architecture `{a}`")),
         }
     }
 }
 
 #[derive(Clone, Copy, Default)]
 /// A config for a GGUF loader.
@@ -179,28 +186,17 @@
             xlora_model_id,
             xlora_order,
             no_kv_cache,
             tgt_non_granular_index,
         )
     }
 
-    pub fn with_lora(
-        mut self,
-        xlora_model_id: String,
-        xlora_order: Ordering,
-        no_kv_cache: bool,
-        tgt_non_granular_index: Option<usize>,
-    ) -> Self {
+    pub fn with_lora(mut self, lora_model_id: String, lora_order: Ordering) -> Self {
         self.kind = ModelKind::LoraGGUF;
-        self.with_adapter(
-            xlora_model_id,
-            xlora_order,
-            no_kv_cache,
-            tgt_non_granular_index,
-        )
+        self.with_adapter(lora_model_id, lora_order, false, None)
     }
 
     pub fn build(self) -> Box<dyn Loader> {
         Box::new(GGUFLoader {
             model_id: self.model_id.unwrap(),
             config: self.config,
             xlora_model_id: self.xlora_model_id,
@@ -328,14 +324,17 @@
             ModelKind::QuantizedGGUF => match arch {
                 GGUFArchitecture::Llama => {
                     Model::Llama(QLlama::from_gguf(model, &mut file, device, mapper)?)
                 }
                 GGUFArchitecture::Phi2 => {
                     Model::Phi2(QPhi::from_gguf(model, &mut file, device, mapper)?)
                 }
+                GGUFArchitecture::Phi3 => {
+                    Model::Phi3(QPhi3::from_gguf(model, &mut file, device, mapper)?)
+                }
                 a => bail!("Unsupported architecture `{a:?}`"),
             },
             ModelKind::XLoraGGUF => {
                 let vb = from_mmaped_safetensors(
                     vec![paths.get_classifier_path().as_ref().unwrap().to_path_buf()],
                     paths
                         .get_adapter_filenames()
@@ -355,14 +354,36 @@
                         &mut file,
                         device,
                         paths.get_adapter_configs().as_ref().unwrap(),
                         &vb,
                         paths.get_ordering().as_ref().unwrap(),
                         Some(paths.get_classifier_config().as_ref().unwrap().clone()),
                         mapper,
+                        &load_preload_adapters(
+                            paths.get_lora_preload_adapter_info(),
+                            DType::F32,
+                            device,
+                            silent,
+                        )?,
+                    )?),
+                    GGUFArchitecture::Phi3 => Model::XLoraPhi3(XLoraQPhi3::from_gguf(
+                        model,
+                        &mut file,
+                        device,
+                        paths.get_adapter_configs().as_ref().unwrap(),
+                        &vb,
+                        paths.get_ordering().as_ref().unwrap(),
+                        Some(paths.get_classifier_config().as_ref().unwrap().clone()),
+                        mapper,
+                        &load_preload_adapters(
+                            paths.get_lora_preload_adapter_info(),
+                            DType::F32,
+                            device,
+                            silent,
+                        )?,
                     )?),
                     a => bail!("Unsupported architecture for GGUF X-LoRA `{a:?}`"),
                 }
             }
             ModelKind::LoraGGUF => {
                 is_lora = true;
                 let vb = from_mmaped_safetensors(
@@ -385,14 +406,36 @@
                         &mut file,
                         device,
                         paths.get_adapter_configs().as_ref().unwrap(),
                         &vb,
                         paths.get_ordering().as_ref().unwrap(),
                         None,
                         mapper,
+                        &load_preload_adapters(
+                            paths.get_lora_preload_adapter_info(),
+                            DType::F32,
+                            device,
+                            silent,
+                        )?,
+                    )?),
+                    GGUFArchitecture::Phi3 => Model::XLoraPhi3(XLoraQPhi3::from_gguf(
+                        model,
+                        &mut file,
+                        device,
+                        paths.get_adapter_configs().as_ref().unwrap(),
+                        &vb,
+                        paths.get_ordering().as_ref().unwrap(),
+                        None,
+                        mapper,
+                        &load_preload_adapters(
+                            paths.get_lora_preload_adapter_info(),
+                            DType::F32,
+                            device,
+                            silent,
+                        )?,
                     )?),
                     a => bail!("Unsupported architecture for GGUF X-LoRA `{a:?}`"),
                 }
             }
             _ => unreachable!(),
         };
 
@@ -401,24 +444,28 @@
 
         let (chat_template, gen_conf) = deserialize_chat_template!(paths, self);
 
         let max_seq_len = match model {
             Model::Llama(ref l) => l.max_seq_len,
             Model::Phi2(ref p) => p.max_seq_len,
             Model::XLoraLlama(ref xl) => xl.max_seq_len,
+            Model::Phi3(ref p) => p.max_seq_len,
+            Model::XLoraPhi3(ref p) => p.max_seq_len,
         };
         let tok_trie: Arc<TokTrie> = build_tok_trie(tokenizer.clone()).into();
         let is_xlora = match &model {
-            Model::Llama(_) | Model::Phi2(_) => false,
-            Model::XLoraLlama(_) => !is_lora,
+            Model::Llama(_) | Model::Phi2(_) | Model::Phi3(_) => false,
+            Model::XLoraLlama(_) | Model::XLoraPhi3(_) => !is_lora,
         };
         let num_hidden_layers = match model {
             Model::Llama(ref model) => model.cache.lock().len(),
             Model::Phi2(ref model) => model.cache.lock().len(),
             Model::XLoraLlama(ref model) => model.cache.lock().len(),
+            Model::Phi3(ref model) => model.cache.lock().len(),
+            Model::XLoraPhi3(ref model) => model.cache.lock().len(),
         };
         let eos = calculate_eos_tokens(&chat_template, gen_conf, &tokenizer);
         Ok(Arc::new(Mutex::new(GGUFPipeline {
             model,
             tok_trie: tok_trie.clone(),
             tokenizer: tokenizer.into(),
             no_kv_cache: self.no_kv_cache,
@@ -434,14 +481,15 @@
                 max_seq_len,
                 repeat_last_n: self.config.repeat_last_n,
                 tok_trie,
                 has_no_kv_cache: self.no_kv_cache,
                 is_xlora,
                 num_hidden_layers,
                 eos_tok: eos,
+                is_lora,
             },
         })))
     }
 
     fn get_id(&self) -> String {
         self.xlora_model_id
             .as_deref()
@@ -484,14 +532,26 @@
                 seqlen_offsets_full.as_ref().unwrap_or(&seqlen_offsets),
                 seqlen_offsets_kernel.clone(),
                 seqlen_offsets_kernel_full.unwrap_or(seqlen_offsets_kernel),
                 self.no_kv_cache,
                 &self.non_granular_state,
                 context_lens,
             ),
+            Model::Phi3(ref mut model) => model.forward(&input_ids, &seqlen_offsets),
+            Model::XLoraPhi3(ref mut model) => model.forward(
+                &input_ids,
+                input_ids_full.as_ref().unwrap_or(&input_ids),
+                &seqlen_offsets,
+                seqlen_offsets_full.as_ref().unwrap_or(&seqlen_offsets),
+                seqlen_offsets_kernel.clone(),
+                seqlen_offsets_kernel_full.unwrap_or(seqlen_offsets_kernel),
+                self.no_kv_cache,
+                &self.non_granular_state,
+                context_lens,
+            ),
         }
     }
     async fn sample(
         &self,
         seqs: &mut [&mut Sequence],
         logits: Tensor,
         prefix_cacher: &mut PrefixCacheManager,
@@ -501,14 +561,16 @@
         do_sample!(self, seqs, logits, prefix_cacher, disable_eos_stop, rng)
     }
     fn device(&self) -> Device {
         match self.model {
             Model::Llama(ref model) => model.device.clone(),
             Model::Phi2(ref model) => model.device.clone(),
             Model::XLoraLlama(ref model) => model.device.clone(),
+            Model::Phi3(ref model) => model.device.clone(),
+            Model::XLoraPhi3(ref model) => model.device.clone(),
         }
     }
     fn tokenizer(&self) -> Arc<Tokenizer> {
         self.tokenizer.clone()
     }
     fn name(&self) -> String {
         self.model_id.clone()
@@ -526,27 +588,45 @@
         anyhow::bail!(
             "You are trying to in-situ requantize a GGML model. This will not do anything."
         )
     }
     fn get_metadata(&self) -> &GeneralMetadata {
         &self.metadata
     }
-    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence]) {
-        DefaultCacheManager.clone_in_cache(self, seqs)
+    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence], modify_draft_cache: bool) {
+        DefaultCacheManager.clone_in_cache(self, seqs, modify_draft_cache)
     }
-    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence]) {
-        DefaultCacheManager.clone_out_cache(self, seqs)
+    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence], modify_draft_cache: bool) {
+        DefaultCacheManager.clone_out_cache(self, seqs, modify_draft_cache)
     }
-    fn set_none_cache(&mut self, reset_non_granular: bool) {
-        DefaultCacheManager.set_none_cache(self);
+    fn set_none_cache(&mut self, reset_non_granular: bool, modify_draft_cache: bool) {
+        DefaultCacheManager.set_none_cache(self, modify_draft_cache);
         if reset_non_granular {
             self.reset_non_granular_state()
         }
     }
     fn cache(&self) -> &Cache {
         match self.model {
             Model::Llama(ref model) => &model.cache,
             Model::Phi2(ref model) => &model.cache,
             Model::XLoraLlama(ref model) => &model.cache,
+            Model::Phi3(ref model) => &model.cache,
+            Model::XLoraPhi3(ref model) => &model.cache,
+        }
+    }
+    fn activate_adapters(&mut self, adapter_names: Vec<String>) -> anyhow::Result<usize> {
+        if !self.metadata.is_lora {
+            anyhow::bail!("Cannot activate adapters non-LoRA models.")
+        }
+        match self.model {
+            Model::Llama(_) => unreachable!(),
+            Model::Phi2(_) => unreachable!(),
+            Model::Phi3(_) => unreachable!(),
+            Model::XLoraLlama(ref mut model) => model
+                .activate_adapters(adapter_names)
+                .map_err(anyhow::Error::msg),
+            Model::XLoraPhi3(ref mut model) => model
+                .activate_adapters(adapter_names)
+                .map_err(anyhow::Error::msg),
         }
     }
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/pipeline/loaders.rs` & `mistralrs-0.1.5/mistralrs-core/src/pipeline/loaders.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,30 @@
 use crate::{
     models,
     xlora_models::{self, XLoraConfig},
     DeviceMapMetadata,
 };
 
 #[pyclass]
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, Deserialize)]
 /// The architecture to load the normal model as.
 pub enum NormalLoaderType {
+    #[serde(rename = "mistral")]
     Mistral,
+    #[serde(rename = "gemma")]
     Gemma,
+    #[serde(rename = "mixtral")]
     Mixtral,
+    #[serde(rename = "llama")]
     Llama,
+    #[serde(rename = "phi2")]
     Phi2,
+    #[serde(rename = "phi3")]
     Phi3,
+    #[serde(rename = "qwen2")]
     Qwen2,
 }
 
 impl FromStr for NormalLoaderType {
     type Err = String;
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         match s {
@@ -103,31 +110,33 @@
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraMistral::new(
             &MistralBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
             loading_isq,
             device,
+            preload_adapters,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
     fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
         Ok(Box::new(MistralBasicConfig::deserialize(
@@ -207,31 +216,33 @@
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraGemma::new(
             &GemmaBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
             loading_isq,
             device,
+            preload_adapters,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
     fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
         Ok(Box::new(GemmaBasicConfig::deserialize(
@@ -303,31 +314,33 @@
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraLlama::new(
             &LlamaBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
             loading_isq,
             device,
+            preload_adapters,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
     fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
         Ok(Box::new(LlamaBasicConfig::deserialize(
@@ -400,31 +413,33 @@
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraMixtral::new(
             &MixtralBasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
             loading_isq,
             device,
+            preload_adapters,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
     fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
         Ok(Box::new(MixtralBasicConfig::deserialize(
@@ -497,31 +512,33 @@
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraPhi2::new(
             &Phi2BasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
             loading_isq,
             device,
+            preload_adapters,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
     fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
         Ok(Box::new(Phi2BasicConfig::deserialize(
@@ -605,31 +622,33 @@
         )?))
     }
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         Ok(Box::new(xlora_models::XLoraPhi3::new(
             &Phi3BasicConfig::deserialize(config, use_flash_attn)?,
             vb,
             lora_config,
             xlora_config,
             xlora_ordering,
             self.is_gptx(),
             mapper,
             loading_isq,
             device,
+            preload_adapters,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
     fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
         Ok(Box::new(Phi3BasicConfig::deserialize(
@@ -704,20 +723,21 @@
         )?))
     }
     fn load_xlora(
         &self,
         _config: &str,
         _use_flash_attn: bool,
         _vb: VarBuilder,
-        _lora_config: &[(String, LoraConfig)],
+        _lora_config: &[((String, String), LoraConfig)],
         _xlora_config: Option<XLoraConfig>,
         _xlora_ordering: Ordering,
         _mapper: DeviceMapMetadata,
         _loading_isq: bool,
         _device: Device,
+        _preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         todo!()
     }
     fn is_gptx(&self) -> bool {
         true
     }
     fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/pipeline/macros.rs` & `mistralrs-0.1.5/mistralrs-core/src/pipeline/macros.rs`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,15 @@
                 }
             }
 
             let path = $model_id.join($file);
             if !path.exists() {
                 panic!("File \"{}\" not found at model id {:?}", $file, $model_id)
             }
+            info!("Loading `{:?}` locally at `{path:?}`", &$file);
             path
         })
     };
 }
 
 #[macro_export]
 macro_rules! deserialize_chat_template {
@@ -163,14 +164,15 @@
 
         let XLoraPaths {
             adapter_configs,
             adapter_safetensors,
             classifier_path,
             xlora_order,
             xlora_config,
+            lora_preload_adapter_info,
         } = get_xlora_paths(
             $this.model_id.clone(),
             &$this.xlora_model_id,
             &$token_source,
             revision.clone(),
             &$this.xlora_order,
         )?;
@@ -197,14 +199,15 @@
             xlora_adapter_configs: adapter_configs,
             xlora_adapter_filenames: adapter_safetensors,
             classifier_path,
             classifier_config: xlora_config,
             xlora_ordering: xlora_order,
             template_filename,
             gen_conf,
+            lora_preload_adapter_info,
         }))
     }};
 }
 
 #[macro_export]
 macro_rules! normal_model_loader {
     ($paths:expr, $dtype:expr, $default_dtype:expr, $device:expr, $config:expr, $loader:expr, $use_flash_attn:expr, $silent:expr, $mapper:expr, $loading_isq:expr, $real_device:expr) => {{
@@ -255,14 +258,20 @@
             vb,
             $paths.get_adapter_configs().as_ref().unwrap(),
             Some($paths.get_classifier_config().as_ref().unwrap().clone()),
             $paths.get_ordering().as_ref().unwrap().clone(),
             $mapper,
             $loading_isq,
             $real_device,
+            &$crate::utils::varbuilder_utils::load_preload_adapters(
+                $paths.get_lora_preload_adapter_info(),
+                $dtype.unwrap_or($default_dtype),
+                $device,
+                $silent,
+            )?,
         )?
     }};
 }
 
 #[macro_export]
 macro_rules! lora_model_loader {
     ($paths:expr, $dtype:expr, $default_dtype:expr, $device:expr, $config:expr, $loader:expr, $use_flash_attn:expr, $silent:expr, $mapper:expr, $loading_isq:expr, $real_device:expr) => {{
@@ -291,10 +300,16 @@
             vb,
             $paths.get_adapter_configs().as_ref().unwrap(),
             None,
             $paths.get_ordering().as_ref().unwrap().clone(),
             $mapper,
             $loading_isq,
             $real_device,
+            &$crate::utils::varbuilder_utils::load_preload_adapters(
+                $paths.get_lora_preload_adapter_info(),
+                $dtype.unwrap_or($default_dtype),
+                $device,
+                $silent,
+            )?,
         )?
     }};
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/pipeline/mod.rs` & `mistralrs-0.1.5/mistralrs-core/src/pipeline/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 mod chat_template;
 mod ggml;
 mod gguf;
 mod loaders;
 mod macros;
 mod normal;
 mod sampling;
+mod speculative;
 use crate::aici::toktree::TokTrie;
 use crate::device_map::DeviceMapper;
 use crate::prefix_cacher::PrefixCacheManager;
 mod sampling_pipeline;
 use crate::{api_dir_list, api_get_file, DeviceMapMetadata};
 use candle_core::quantized::{GgmlDType, QMatMul, QTensor};
 use candle_nn::VarBuilder;
@@ -28,23 +29,23 @@
     GemmaLoader, LlamaLoader, MistralLoader, MixtralLoader, NormalLoaderType, Phi2Loader,
     Phi3Loader, Qwen2Loader,
 };
 use mistralrs_lora::{LoraConfig, Ordering};
 pub use normal::{NormalLoader, NormalLoaderBuilder, NormalSpecificConfig};
 use rand_isaac::Isaac64Rng;
 use rayon::iter::{IndexedParallelIterator, IntoParallelIterator, ParallelIterator};
-pub(crate) use sampling::sample_sequence;
+pub use speculative::{SpeculativeConfig, SpeculativeLoader, SpeculativePipeline};
 use std::fmt::{Debug, Display};
 use std::path::Path;
 use std::sync::atomic::AtomicUsize;
 use std::sync::Arc;
 use std::{collections::HashMap, fs, iter::repeat, path::PathBuf, str::FromStr};
 use tokenizers::Tokenizer;
 use tokio::sync::Mutex;
-use tracing::info;
+use tracing::{info, warn};
 
 use anyhow::Result;
 use candle_core::{DType, Device, Tensor};
 
 use crate::{
     models::Cache,
     sequence::Sequence,
@@ -54,32 +55,34 @@
 
 pub trait ModelPaths {
     fn get_weight_filenames(&self) -> &[PathBuf];
     fn get_config_filename(&self) -> &PathBuf;
     fn get_tokenizer_filename(&self) -> &PathBuf;
     fn get_template_filename(&self) -> &PathBuf;
     fn get_adapter_filenames(&self) -> &Option<Vec<(String, PathBuf)>>;
-    fn get_adapter_configs(&self) -> &Option<Vec<(String, LoraConfig)>>;
+    fn get_adapter_configs(&self) -> &Option<Vec<((String, String), LoraConfig)>>; // (id name, name)
     fn get_classifier_path(&self) -> &Option<PathBuf>;
     fn get_classifier_config(&self) -> &Option<XLoraConfig>;
     fn get_ordering(&self) -> &Option<Ordering>;
     fn get_gen_conf_filename(&self) -> Option<&PathBuf>;
+    fn get_lora_preload_adapter_info(&self) -> &Option<HashMap<String, (PathBuf, LoraConfig)>>;
 }
 
 pub struct SimpleModelPaths<P> {
     tokenizer_filename: P,
     config_filename: P,
     template_filename: P,
     filenames: Vec<P>,
     xlora_adapter_filenames: Option<Vec<(String, P)>>,
-    xlora_adapter_configs: Option<Vec<(String, LoraConfig)>>,
+    xlora_adapter_configs: Option<Vec<((String, String), LoraConfig)>>,
     classifier_path: Option<P>,
     classifier_config: Option<XLoraConfig>,
     xlora_ordering: Option<Ordering>,
     gen_conf: Option<P>,
+    lora_preload_adapter_info: Option<HashMap<String, (P, LoraConfig)>>,
 }
 
 impl ModelPaths for SimpleModelPaths<PathBuf> {
     fn get_config_filename(&self) -> &PathBuf {
         &self.config_filename
     }
     fn get_tokenizer_filename(&self) -> &PathBuf {
@@ -87,15 +90,15 @@
     }
     fn get_weight_filenames(&self) -> &[PathBuf] {
         &self.filenames
     }
     fn get_adapter_filenames(&self) -> &Option<Vec<(String, PathBuf)>> {
         &self.xlora_adapter_filenames
     }
-    fn get_adapter_configs(&self) -> &Option<Vec<(String, LoraConfig)>> {
+    fn get_adapter_configs(&self) -> &Option<Vec<((String, String), LoraConfig)>> {
         &self.xlora_adapter_configs
     }
     fn get_classifier_config(&self) -> &Option<XLoraConfig> {
         &self.classifier_config
     }
     fn get_classifier_path(&self) -> &Option<PathBuf> {
         &self.classifier_path
@@ -105,14 +108,17 @@
     }
     fn get_template_filename(&self) -> &PathBuf {
         &self.template_filename
     }
     fn get_gen_conf_filename(&self) -> Option<&PathBuf> {
         self.gen_conf.as_ref()
     }
+    fn get_lora_preload_adapter_info(&self) -> &Option<HashMap<String, (PathBuf, LoraConfig)>> {
+        &self.lora_preload_adapter_info
+    }
 }
 
 #[derive(Debug, Clone)]
 /// The source of the HF token.
 pub enum TokenSource {
     Literal(String),
     EnvVar(String),
@@ -241,21 +247,30 @@
     pub max_seq_len: usize,
     pub repeat_last_n: usize,
     pub tok_trie: Arc<TokTrie>,
     pub has_no_kv_cache: bool,
     pub is_xlora: bool,
     pub num_hidden_layers: usize,
     pub eos_tok: Vec<u32>,
+    pub is_lora: bool,
+}
+
+pub enum AdapterInstruction {
+    Activate(Vec<String>),
+    None,
 }
 
 pub enum CacheInstruction {
-    In,
+    In(AdapterInstruction),
     Out,
-    Reset { reset_non_granular: bool },
-    Nonthing,
+    Reset {
+        reset_non_granular: bool,
+        adapter_inst: AdapterInstruction,
+    },
+    Nothing(AdapterInstruction),
 }
 
 #[async_trait::async_trait]
 pub trait Pipeline: Send + Sync {
     fn forward_inputs(&mut self, inputs: ModelInputs) -> Result<Tensor, candle_core::Error>;
     /// This does forward pass of model followed by run.
     #[allow(clippy::too_many_arguments)]
@@ -276,30 +291,67 @@
             &self.device(),
             self.get_metadata().has_no_kv_cache,
             None,
         )
         .unwrap();
 
         match pre_op {
-            CacheInstruction::In => self.clone_in_cache(input_seqs),
-            CacheInstruction::Nonthing => (),
-            CacheInstruction::Reset { reset_non_granular } => {
-                self.set_none_cache(reset_non_granular)
+            CacheInstruction::In(adapter_inst) => {
+                match adapter_inst {
+                    AdapterInstruction::Activate(adapters) => {
+                        self.activate_adapters(adapters).map_err(|e| {
+                            candle_core::Error::msg(<anyhow::Error as AsRef<
+                                dyn std::error::Error,
+                            >>::as_ref(&e))
+                        })?
+                    }
+                    AdapterInstruction::None => 0,
+                };
+                self.clone_in_cache(input_seqs, false)
+            }
+            CacheInstruction::Nothing(adapter_inst) => {
+                match adapter_inst {
+                    AdapterInstruction::Activate(adapters) => {
+                        self.activate_adapters(adapters).map_err(|e| {
+                            candle_core::Error::msg(<anyhow::Error as AsRef<
+                                dyn std::error::Error,
+                            >>::as_ref(&e))
+                        })?
+                    }
+                    AdapterInstruction::None => 0,
+                };
+            }
+            CacheInstruction::Reset {
+                reset_non_granular,
+                adapter_inst,
+            } => {
+                match adapter_inst {
+                    AdapterInstruction::Activate(adapters) => {
+                        self.activate_adapters(adapters).map_err(|e| {
+                            candle_core::Error::msg(<anyhow::Error as AsRef<
+                                dyn std::error::Error,
+                            >>::as_ref(&e))
+                        })?
+                    }
+                    AdapterInstruction::None => 0,
+                };
+                self.set_none_cache(reset_non_granular, false)
             }
             _ => unreachable!("Unreachable PRE cache op."),
         }
 
         let logits = self.forward_inputs(inputs)?;
 
         match post_op {
-            CacheInstruction::Out => self.clone_out_cache(input_seqs),
-            CacheInstruction::Nonthing => (),
-            CacheInstruction::Reset { reset_non_granular } => {
-                self.set_none_cache(reset_non_granular)
-            }
+            CacheInstruction::Out => self.clone_out_cache(input_seqs, false),
+            CacheInstruction::Nothing(_) => (),
+            CacheInstruction::Reset {
+                reset_non_granular,
+                adapter_inst: _,
+            } => self.set_none_cache(reset_non_granular, false),
             _ => unreachable!("Unreachable POST cache op."),
         }
 
         self.sample(input_seqs, logits, prefix_cacher, disable_eos_stop, rng)
             .await?;
         Ok(())
     }
@@ -359,29 +411,41 @@
     }
     fn get_chat_template(&self) -> Arc<ChatTemplate>;
     fn reset_non_granular_state(&self);
     fn get_metadata(&self) -> &GeneralMetadata;
     fn re_isq_model(&mut self, dtype: GgmlDType) -> Result<()>;
     /// Clone the cache FROM the sequences' cache TO the model cache. Only called for completion seqs.
     /// It is not a guarantee that this will be called for each completion step.
-    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence]);
+    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence], modify_draft_cache: bool);
     /// Clone the cache FROM the model cache TO the sequences. Called for prompt and completion seqs.
     /// It is not a guarantee that this will be called for each step.
-    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence]);
+    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence], modify_draft_cache: bool);
     /// Set the model cache to all None. Only called for prompt seqs.
     /// It is not a guarantee that this will be called for each prompt step.
     /// This may also reset the non granular state if applicable.
-    fn set_none_cache(&mut self, reset_non_granular: bool);
+    fn set_none_cache(&mut self, reset_non_granular: bool, modify_draft_cache: bool);
     fn cache(&self) -> &Cache;
+    /// Returns the number of activated adapters.
+    fn activate_adapters(&mut self, adapters: Vec<String>) -> Result<usize>;
 }
 
 pub trait CacheManager {
-    fn clone_in_cache(&self, pipeline: &mut dyn Pipeline, seqs: &mut [&mut Sequence]);
-    fn clone_out_cache(&self, pipeline: &mut dyn Pipeline, seqs: &mut [&mut Sequence]);
-    fn set_none_cache(&self, pipeline: &mut dyn Pipeline);
+    fn clone_in_cache(
+        &self,
+        pipeline: &mut dyn Pipeline,
+        seqs: &mut [&mut Sequence],
+        modify_draft_cache: bool,
+    );
+    fn clone_out_cache(
+        &self,
+        pipeline: &mut dyn Pipeline,
+        seqs: &mut [&mut Sequence],
+        modify_draft_cache: bool,
+    );
+    fn set_none_cache(&self, pipeline: &mut dyn Pipeline, modify_draft_cache: bool);
 }
 
 pub trait NormalModelLoader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
@@ -392,25 +456,70 @@
     ) -> Result<Box<dyn NormalModel + Send + Sync>>;
     #[allow(clippy::too_many_arguments)]
     fn load_xlora(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Box<dyn NormalModel + Send + Sync>>;
     fn is_gptx(&self) -> bool;
     fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>>;
 }
 
+pub enum QuantizationBehaviour {
+    Quantize(GgmlDType),
+    Skip,
+}
+
+/// Return the fallback dtype for the given dtype.
+fn get_fallback(dtype: GgmlDType) -> QuantizationBehaviour {
+    // The normal `Q` quants are a bit more lenient than the `K` quants.
+    // => Try to fallback to a similar `Q` quant.
+    // If that's not possible, skip this tensor.
+    match dtype {
+        GgmlDType::Q2K => QuantizationBehaviour::Quantize(GgmlDType::Q4_0),
+        GgmlDType::Q3K => QuantizationBehaviour::Quantize(GgmlDType::Q4_0),
+        GgmlDType::Q4K => QuantizationBehaviour::Quantize(GgmlDType::Q4_1),
+        GgmlDType::Q5K => QuantizationBehaviour::Quantize(GgmlDType::Q5_0),
+        GgmlDType::Q6K => QuantizationBehaviour::Quantize(GgmlDType::Q5_1),
+        GgmlDType::Q8K => QuantizationBehaviour::Quantize(GgmlDType::Q8_1),
+        _ => QuantizationBehaviour::Skip,
+    }
+}
+
+/// Check if the tensor can be quantized with the given dtype.
+fn can_quantize(tensor: &Tensor, dtype: GgmlDType) -> bool {
+    let dims = tensor.shape().dims();
+    // The tensor must not be empty and the last dimension must be a multiple of the block size.
+    !(dims.is_empty() || (dims[dims.len() - 1] % dtype.block_size() != 0))
+}
+
+/// Check if we should quantize the tensor and if so, with which dtype.
+fn get_quantization_behaviour(tensor: &Tensor, dtype: GgmlDType) -> QuantizationBehaviour {
+    if dtype == GgmlDType::F32 {
+        return QuantizationBehaviour::Skip;
+    }
+
+    if can_quantize(tensor, dtype) {
+        return QuantizationBehaviour::Quantize(dtype);
+    }
+    let fallback = get_fallback(dtype);
+    match fallback {
+        QuantizationBehaviour::Skip => fallback,
+        QuantizationBehaviour::Quantize(new_dtype) => get_quantization_behaviour(tensor, new_dtype),
+    }
+}
+
 pub trait NormalModel {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
@@ -463,68 +572,99 @@
 
         tensors
             .into_par_iter()
             .zip(devices)
             .progress_with(bar)
             .for_each(|((tensor, _), device)| {
                 if let QMatMul::Tensor(t) = tensor {
-                    n_quantized.fetch_add(1, std::sync::atomic::Ordering::Relaxed);
                     let t = t.to_device(&device).unwrap();
-                    *tensor = QMatMul::QTensor(Arc::new(QTensor::quantize(&t, dtype).unwrap()));
+                    let quantization_behaviour = get_quantization_behaviour(&t, dtype);
+                    *tensor =  match quantization_behaviour{
+                        QuantizationBehaviour::Skip => {
+                            let shape = t.shape();
+                            warn!("Skipping quantization of tensor with shape {shape:?} as it is not quantizable.");
+                            QMatMul::QTensor(Arc::new(QTensor::quantize(&t, GgmlDType::F32).unwrap()))
+                        },
+                        QuantizationBehaviour::Quantize(dtype) => {
+                            n_quantized.fetch_add(1, std::sync::atomic::Ordering::Relaxed);
+                            QMatMul::QTensor(Arc::new(QTensor::quantize(&t, dtype).unwrap()))
+                        }
+                    }
                 }
             });
         info!("Applied in-situ quantization into {dtype:?} to {n_quantized:?} tensors out of {total_tensors} total tensors.");
         Ok(())
     }
+    fn activate_adapters(&mut self, _: Vec<String>) -> candle_core::Result<usize> {
+        candle_core::bail!("Unable to activate adapters for model without adapters");
+    }
 }
 
 struct InputMetadata {
     input: Tensor,
     positions: Vec<usize>,
     positions_kernel: Tensor,          // [bs, seq len]
     context_lens: Vec<(usize, usize)>, // (start index, len)
     position_ids: Vec<usize>,
 }
 
 fn get_prompt_input(
     input_seqs: &[&mut Sequence],
     device: &Device,
-    last_n_context_len: Option<usize>,
+    last_n_context_len: Option<(usize, usize)>,
 ) -> Result<InputMetadata> {
     let max_len = input_seqs
         .iter()
         .map(|seq| seq.len())
         .max()
         .expect("No sequences");
     let padding_tok = 0;
     // Pad each sequence by the padding token to the max len.
     let mut seqs_tensors = Vec::new();
     let mut seqlen_offsets = Vec::new();
     let mut context_lens = Vec::new();
     let mut position_ids = Vec::new();
     for seq in input_seqs.iter() {
         let mut ctxt = seq.get_toks().to_vec();
-        seqlen_offsets.push(0);
+        let offset = if let Some((_, offset)) = last_n_context_len {
+            offset
+        } else {
+            0
+        };
+        seqlen_offsets.push(offset);
 
         ctxt.extend(repeat(padding_tok).take(max_len.saturating_sub(ctxt.len())));
         context_lens.push((
-            seq.len() - 1 - last_n_context_len.map(|x| x - 1).unwrap_or(0),
-            last_n_context_len.unwrap_or(1),
+            seq.len() - last_n_context_len.map(|(a, _)| a).unwrap_or(1),
+            last_n_context_len.map(|(a, _)| a).unwrap_or(1),
         ));
         position_ids.push(seq.len());
 
         seqs_tensors.push(Tensor::new(ctxt, device).unwrap().unsqueeze(0).unwrap());
     }
 
     let mut tmp = Vec::new();
-    for pos in (0..seqs_tensors.len())
-        .map(|_| (0..max_len).map(|x| x as i64).collect::<Vec<_>>())
-        .collect::<Vec<_>>()
-    {
-        tmp.push(Tensor::from_slice(&pos, pos.len(), device)?.unsqueeze(0)?);
+    if last_n_context_len.is_some() {
+        for pos in (0..seqs_tensors.len())
+            .map(|i| {
+                (*seqlen_offsets.get(i).unwrap() as i64
+                    ..*seqlen_offsets.get(i).unwrap() as i64 + max_len as i64)
+                    .collect::<Vec<_>>()
+            })
+            .collect::<Vec<_>>()
+        {
+            tmp.push(Tensor::from_slice(&pos, pos.len(), device)?.unsqueeze(0)?);
+        }
+    } else {
+        for pos in (0..seqs_tensors.len())
+            .map(|_| (0..max_len).map(|x| x as i64).collect::<Vec<_>>())
+            .collect::<Vec<_>>()
+        {
+            tmp.push(Tensor::from_slice(&pos, pos.len(), device)?.unsqueeze(0)?);
+        }
     }
     let positions_kernel = Tensor::cat(&tmp, 0)?;
     Ok(InputMetadata {
         input: Tensor::cat(&seqs_tensors, 0).unwrap(),
         positions: seqlen_offsets,
         positions_kernel,
         context_lens,
@@ -532,15 +672,15 @@
     })
 }
 
 fn get_completion_input(
     input_seqs: &[&mut Sequence],
     device: &Device,
     no_kv_cache: bool,
-    last_n_context_len: Option<usize>,
+    last_n_context_len: Option<(usize, usize)>,
 ) -> Result<InputMetadata> {
     if no_kv_cache {
         return get_prompt_input(input_seqs, device, last_n_context_len);
     }
     // Pad each sequence by the padding token to the max len.
     let mut seqs_tensors = Vec::new();
     let mut seqlen_offsets = Vec::new();
@@ -586,15 +726,15 @@
 
 fn calculate_inputs(
     input_seqs: &[&mut Sequence],
     is_prompt: bool,
     is_xlora: bool,
     device: &Device,
     no_kv_cache: bool,
-    last_n_context_len: Option<usize>,
+    last_n_context_len: Option<(usize, usize)>,
 ) -> Result<ModelInputs> {
     if is_xlora && !is_prompt {
         let InputMetadata {
             input: input_ids_full,
             positions: seqlen_offsets_full,
             positions_kernel: seqlen_offsets_kernel_full,
             context_lens: _,
@@ -670,31 +810,32 @@
             seqlen_offsets_kernel_full: None,
             context_lens,
             position_ids,
         })
     }
 }
 
-pub fn extract_logits(
+pub(crate) fn extract_logits(
     logits: &Tensor,
     context_lens: Vec<(usize, usize)>,
 ) -> candle_core::Result<Tensor> {
     let mut toks = Vec::new();
     for (dim, (start, len)) in logits.chunk(logits.dims()[0], 0)?.iter().zip(context_lens) {
         toks.push(dim.narrow(1, start, len)?);
     }
     Tensor::cat(&toks, 0)
 }
 
 struct XLoraPaths {
-    adapter_configs: Option<Vec<(String, LoraConfig)>>,
+    adapter_configs: Option<Vec<((String, String), LoraConfig)>>,
     adapter_safetensors: Option<Vec<(String, PathBuf)>>,
     classifier_path: Option<PathBuf>,
     xlora_order: Option<Ordering>,
     xlora_config: Option<XLoraConfig>,
+    lora_preload_adapter_info: Option<HashMap<String, (PathBuf, LoraConfig)>>,
 }
 
 fn get_xlora_paths(
     base_model_id: String,
     xlora_model_id: &Option<String>,
     token_source: &TokenSource,
     revision: String,
@@ -712,44 +853,44 @@
         ));
         let model_id = Path::new(&xlora_id);
 
         let xlora_classifier = &api_dir_list!(api, model_id)
             .filter(|x| x.contains("xlora_classifier.safetensors"))
             .collect::<Vec<_>>();
         if xlora_classifier.len() != 1 {
-            info!("⚠️ WARNING: Detected multiple X-LoRA classifiers: {xlora_classifier:?}");
-            info!("⚠️ WARNING: Selected classifier: `{}`", &xlora_classifier[0]);
+            warn!("Detected multiple X-LoRA classifiers: {xlora_classifier:?}");
+            warn!("Selected classifier: `{}`", &xlora_classifier[0]);
         }
         let xlora_classifier = &xlora_classifier[0];
         let xlora_configs = &api_dir_list!(api, model_id)
             .filter(|x| x.contains("xlora_config.json"))
             .collect::<Vec<_>>();
         if xlora_configs.len() != 1 {
-            info!("⚠️ WARNING: Detected multiple X-LoRA configs: {xlora_configs:?}");
+            warn!("Detected multiple X-LoRA configs: {xlora_configs:?}");
         }
 
         let classifier_path = api_get_file!(api, xlora_classifier, Path::new(""));
 
         let mut xlora_config: Option<XLoraConfig> = None;
         let mut last_err: Option<serde_json::Error> = None;
         for (i, config_path) in xlora_configs.iter().enumerate() {
             if xlora_configs.len() != 1 {
-                info!("⚠️ WARNING: Selecting config: `{}`", config_path);
+                warn!("Selecting config: `{}`", config_path);
             }
             let config_path = api_get_file!(api, config_path, Path::new(""));
             let conf = fs::read_to_string(config_path)?;
             let deser: Result<XLoraConfig, serde_json::Error> = serde_json::from_str(&conf);
             match deser {
                 Ok(conf) => {
                     xlora_config = Some(conf);
                     break;
                 }
                 Err(e) => {
                     if i != xlora_configs.len() - 1 {
-                        info!("⚠️ WARNING: Config is broken with error `{e}`");
+                        warn!("Config is broken with error `{e}`");
                     }
                     last_err = Some(e);
                 }
             }
         }
         let xlora_config = xlora_config.unwrap_or_else(|| {
             panic!(
@@ -795,15 +936,15 @@
                 .unwrap_or_else(|| panic!("Adapter {name} not found."));
             for path in paths {
                 if path.extension().unwrap() == "safetensors" {
                     adapters_safetensors.push((name.clone(), path.to_owned()));
                 } else {
                     let conf = fs::read_to_string(path)?;
                     let lora_config: LoraConfig = serde_json::from_str(&conf)?;
-                    adapters_configs.push(((i + 1).to_string(), lora_config));
+                    adapters_configs.push((((i + 1).to_string(), name.clone()), lora_config));
                 }
             }
         }
 
         if xlora_order
             .as_ref()
             .is_some_and(|order| order.base_model_id != xlora_config.base_model_id)
@@ -813,28 +954,83 @@
                 "Adapter ordering file, adapter model config, and base model ID do not match: {}, {}, and {} respectively.",
                 xlora_order.as_ref().unwrap().base_model_id,
                 xlora_config.base_model_id,
                 base_model_id
             );
         }
 
+        let lora_preload_adapter_info = if let Some(xlora_order) = xlora_order {
+            if let Some(preload_adapters) = &xlora_order.preload_adapters {
+                let mut output = HashMap::new();
+                for adapter in preload_adapters {
+                    let adapter_files = api_dir_list!(api, &adapter.adapter_model_id)
+                        .filter_map(|f| {
+                            if f.contains(&adapter.name) {
+                                Some((f, adapter.name.clone()))
+                            } else {
+                                None
+                            }
+                        })
+                        .collect::<Vec<_>>();
+                    if adapter_files.is_empty() {
+                        anyhow::bail!("Adapter files are empty. Perhaps the ordering file adapters does not match the actual adapters?")
+                    }
+                    let mut adapters_paths: HashMap<String, Vec<PathBuf>> = HashMap::new();
+                    for (file, name) in adapter_files {
+                        if let Some(paths) = adapters_paths.get_mut(&name) {
+                            paths.push(api_get_file!(api, &file, Path::new("")));
+                        } else {
+                            adapters_paths
+                                .insert(name, vec![api_get_file!(api, &file, Path::new(""))]);
+                        }
+                    }
+
+                    let mut config = None;
+                    let mut safetensor = None;
+
+                    let paths = adapters_paths
+                        .get(&adapter.name)
+                        .unwrap_or_else(|| panic!("Adapter {} not found.", adapter.name));
+                    for path in paths {
+                        if path.extension().unwrap() == "safetensors" {
+                            safetensor = Some(path.to_owned());
+                        } else {
+                            let conf = fs::read_to_string(path)?;
+                            let lora_config: LoraConfig = serde_json::from_str(&conf)?;
+                            config = Some(lora_config);
+                        }
+                    }
+
+                    let (config, safetensor) = (config.unwrap(), safetensor.unwrap());
+                    output.insert(adapter.name.clone(), (safetensor, config));
+                }
+                Some(output)
+            } else {
+                None
+            }
+        } else {
+            None
+        };
+
         XLoraPaths {
             adapter_configs: Some(adapters_configs),
             adapter_safetensors: Some(adapters_safetensors),
             classifier_path: Some(classifier_path),
             xlora_order: xlora_order.clone(),
             xlora_config: Some(xlora_config),
+            lora_preload_adapter_info,
         }
     } else {
         XLoraPaths {
             adapter_configs: None,
             adapter_safetensors: None,
             classifier_path: None,
             xlora_order: None,
             xlora_config: None,
+            lora_preload_adapter_info: None,
         }
     })
 }
 
 fn get_model_paths(
     revision: String,
     token_source: &TokenSource,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/pipeline/normal.rs` & `mistralrs-0.1.5/mistralrs-core/src/pipeline/normal.rs`

 * *Files 3% similar despite different names*

```diff
@@ -134,28 +134,17 @@
             xlora_model_id,
             xlora_order,
             no_kv_cache,
             tgt_non_granular_index,
         )
     }
 
-    pub fn with_lora(
-        mut self,
-        xlora_model_id: String,
-        xlora_order: Ordering,
-        no_kv_cache: bool,
-        tgt_non_granular_index: Option<usize>,
-    ) -> Self {
+    pub fn with_lora(mut self, lora_model_id: String, lora_order: Ordering) -> Self {
         self.kind = ModelKind::LoraNormal;
-        self.with_adapter(
-            xlora_model_id,
-            xlora_order,
-            no_kv_cache,
-            tgt_non_granular_index,
-        )
+        self.with_adapter(lora_model_id, lora_order, false, None)
     }
 
     pub fn build(self, loader: NormalLoaderType) -> Box<dyn Loader> {
         let loader: Box<dyn NormalModelLoader> = match loader {
             NormalLoaderType::Mistral => Box::new(MistralLoader),
             NormalLoaderType::Gemma => Box::new(GemmaLoader),
             NormalLoaderType::Llama => Box::new(LlamaLoader),
@@ -310,14 +299,15 @@
                 max_seq_len,
                 repeat_last_n: self.config.repeat_last_n,
                 tok_trie,
                 has_no_kv_cache: self.no_kv_cache,
                 is_xlora,
                 num_hidden_layers,
                 eos_tok: eos,
+                is_lora,
             },
         })))
     }
 
     fn get_id(&self) -> String {
         self.xlora_model_id
             .as_deref()
@@ -400,23 +390,28 @@
         self.model
             .quantize(dtype, device)
             .map_err(anyhow::Error::msg)
     }
     fn get_metadata(&self) -> &GeneralMetadata {
         &self.metadata
     }
-    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence]) {
-        DefaultCacheManager.clone_in_cache(self, seqs)
+    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence], modify_draft_cache: bool) {
+        DefaultCacheManager.clone_in_cache(self, seqs, modify_draft_cache)
     }
-    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence]) {
-        DefaultCacheManager.clone_out_cache(self, seqs)
+    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence], modify_draft_cache: bool) {
+        DefaultCacheManager.clone_out_cache(self, seqs, modify_draft_cache)
     }
-    fn set_none_cache(&mut self, reset_non_granular: bool) {
-        DefaultCacheManager.set_none_cache(self);
+    fn set_none_cache(&mut self, reset_non_granular: bool, modify_draft_cache: bool) {
+        DefaultCacheManager.set_none_cache(self, modify_draft_cache);
         if reset_non_granular {
             self.reset_non_granular_state()
         }
     }
     fn cache(&self) -> &Cache {
         self.model.cache()
     }
+    fn activate_adapters(&mut self, adapter_names: Vec<String>) -> anyhow::Result<usize> {
+        self.model
+            .activate_adapters(adapter_names)
+            .map_err(anyhow::Error::msg)
+    }
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/pipeline/sampling_pipeline.rs` & `mistralrs-0.1.5/mistralrs-core/src/pipeline/sampling_pipeline.rs`

 * *Files 0% similar despite different names*

```diff
@@ -185,23 +185,24 @@
         debug_assert_eq!(logits_seq.len(), seqs_len);
 
         let use_async_pool = seqs_len > 1;
 
         let sampling_futures: Vec<_> = std::iter::zip(logits_seq, $seqs.iter_mut())
             .map(|(logits_per_seq, seq)| {
                 let return_logprobs = seq.return_logprobs();
-                $crate::pipeline::sample_sequence(
+                $crate::pipeline::sampling::sample_sequence(
                     logits_per_seq,
                     seq,
                     return_logprobs,
                     $this.metadata.repeat_last_n,
                     $this.tok_trie.clone(),
                     $rng.clone(),
                     use_async_pool,
                     true, // Append result to trie
+                    false,
                 )
             })
             .collect();
         let sampled_vec = futures::future::join_all(sampling_futures).await;
 
         for (sampled, seq) in std::iter::zip(sampled_vec, $seqs.iter_mut()) {
             let next_token = $crate::handle_seq_error_stateaware_ok!(sampled, seq);
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/prefix_cacher.rs` & `mistralrs-0.1.5/mistralrs-core/src/prefix_cacher.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/response.rs` & `mistralrs-0.1.5/mistralrs-core/src/response.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/sampler.rs` & `mistralrs-0.1.5/mistralrs-core/src/sampler.rs`

 * *Files 14% similar despite different names*

```diff
@@ -79,14 +79,18 @@
 pub struct Logprobs {
     pub token: u32,
     pub logprob: f32,
     pub bytes: String,
     pub top_logprobs: Option<Vec<TopLogprob>>,
 }
 
+fn argmax_sample_last_dim(logits: &Tensor) -> Result<Tensor> {
+    logits.argmax(D::Minus1)
+}
+
 impl Sampler {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         temperature: Option<f64>,
         top_n_logprobs: usize,
         tokenizer: Arc<Tokenizer>,
         frequency_penalty: Option<f32>,
@@ -172,14 +176,76 @@
             bytes: self
                 .tokenizer
                 .decode(&[next_token], false)
                 .map_err(|x| Error::Msg(x.to_string()))?,
         })
     }
 
+    fn sample_speculative_topkp(
+        &self,
+        logits: Tensor,
+        return_logprobs: bool,
+        top_k: i64,
+        top_p: f32,
+    ) -> Result<Logprobs> {
+        let mut probs: Vec<f32> = logits.to_vec1()?;
+        let mut argsort_indices = (0..probs.len()).collect::<Vec<_>>();
+
+        // Sort by descending probability.
+        argsort_indices
+            .sort_unstable_by(|&i, &j| probs[j].partial_cmp(&probs[i]).expect("No ordering."));
+
+        if top_k > 0 {
+            // Clamp smaller probabilities to zero.
+            for (index, val) in argsort_indices.iter().enumerate() {
+                if index >= top_k as usize {
+                    probs[*val] = 0.0;
+                }
+            }
+        }
+
+        // TOP P
+
+        // top-p sampling (or "nucleus sampling") samples from the smallest set of
+        // tokens that exceed probability top_p. This way we never sample tokens that
+        // have very low probabilities and are less likely to go "off the rails".
+
+        // Clamp smaller probabilities to zero.
+        let mut cumsum = 0.;
+        for index in &argsort_indices {
+            if cumsum >= top_p {
+                probs[*index] = 0.0;
+            } else {
+                cumsum += probs[*index];
+            }
+        }
+
+        let logits = Tensor::from_slice(&probs, logits.shape(), &Device::Cpu)?;
+
+        let next_token = argmax_sample_last_dim(&logits)?.to_scalar::<u32>()?;
+
+        let logprob = probs[next_token as usize].log(10.0);
+
+        let top_logprobs = if return_logprobs {
+            Some(self.get_top_logprobs(&probs, &argsort_indices)?)
+        } else {
+            None
+        };
+
+        Ok(Logprobs {
+            token: next_token,
+            logprob,
+            top_logprobs,
+            bytes: self
+                .tokenizer
+                .decode(&[next_token], false)
+                .map_err(|x| Error::Msg(x.to_string()))?,
+        })
+    }
+
     fn sample_multinomial(
         &self,
         probs: &mut Vec<f32>,
         argsort_indices: Vec<usize>,
         return_logprobs: bool,
         rng: Arc<Mutex<Isaac64Rng>>,
     ) -> Result<Logprobs> {
@@ -286,34 +352,57 @@
     /// If `frequency_penalty.is_some()` or `presence_penalty.is_some()`, then `penalty_ctxt` must be provided.
     pub fn sample(
         &self,
         logits: Tensor,
         penalty_ctxt: Option<&[u32]>,
         return_logprobs: bool,
         rng: Arc<Mutex<Isaac64Rng>>,
+        sample_speculative: bool,
     ) -> Result<Logprobs> {
         let logits = self.apply_penalties(logits.to_vec1()?, penalty_ctxt)?;
         let logits = match self.logits_bias {
             Some(ref bias) => (logits + bias)?,
             None => logits,
         };
-        let next_token = match self.temperature {
-            None => self.sample_argmax(logits, return_logprobs)?,
-            Some(temperature) => {
-                let logits = (&logits / temperature)?;
-                let probs = candle_nn::ops::softmax_last_dim(&logits)?;
-                let mut probs: Vec<f32> = probs.to_vec1()?;
-
-                self.sample_topkp(
-                    &mut probs,
+        let next_token = if sample_speculative {
+            match self.temperature {
+                None => self.sample_speculative_topkp(
+                    logits,
+                    return_logprobs,
                     self.topk,
                     self.topp as f32,
-                    return_logprobs,
-                    rng,
-                )?
+                )?,
+                Some(temperature) => {
+                    let logits = (&logits / temperature)?;
+                    let probs = candle_nn::ops::softmax_last_dim(&logits)?;
+
+                    self.sample_speculative_topkp(
+                        probs,
+                        return_logprobs,
+                        self.topk,
+                        self.topp as f32,
+                    )?
+                }
+            }
+        } else {
+            match self.temperature {
+                None => self.sample_argmax(logits, return_logprobs)?,
+                Some(temperature) => {
+                    let logits = (&logits / temperature)?;
+                    let probs = candle_nn::ops::softmax_last_dim(&logits)?;
+                    let mut probs: Vec<f32> = probs.to_vec1()?;
+
+                    self.sample_topkp(
+                        &mut probs,
+                        self.topk,
+                        self.topp as f32,
+                        return_logprobs,
+                        rng,
+                    )?
+                }
             }
         };
         Ok(next_token)
     }
 }
 
 mod tests {
@@ -324,15 +413,15 @@
     fn get_tokenizer() -> Tokenizer {
         let api = ApiBuilder::new()
             .with_progress(true)
             .with_token(Some(std::env::var("TESTS_HF_TOKEN").unwrap()))
             .build()
             .unwrap();
         let api = api.repo(Repo::with_revision(
-            "mistralai/Mistral-7B-Instruct-v0.1".to_string(),
+            "EricB/mistralrs_tests".to_string(),
             RepoType::Model,
             "main".to_string(),
         ));
 
         let tokenizer_filename = api.get("tokenizer.json").unwrap();
         Tokenizer::from_file(tokenizer_filename).unwrap()
     }
@@ -345,13 +434,31 @@
         use rand_isaac::Isaac64Rng;
         use std::sync::Arc;
         use std::sync::Mutex;
 
         let sampler = Sampler::new(None, 10, get_tokenizer().into(), None, None, None, 32, 0.1);
         let logits = Tensor::arange(0f32, 1024f32, &Device::Cpu).unwrap();
         let rng = Arc::new(Mutex::new(Isaac64Rng::seed_from_u64(42)));
-        let res = sampler.sample(logits, None, false, rng).unwrap();
+        let res = sampler.sample(logits, None, false, rng, false).unwrap();
+        assert_eq!(res.token, 1023);
+        assert_eq!(res.top_logprobs, None);
+        assert_eq!(res.logprob, 1023f64.log(10.) as f32)
+    }
+
+    #[test]
+    fn test_gumbel_speculative() {
+        use super::Sampler;
+        use candle_core::{Device, Tensor};
+        use rand::SeedableRng;
+        use rand_isaac::Isaac64Rng;
+        use std::sync::Arc;
+        use std::sync::Mutex;
+
+        let sampler = Sampler::new(None, 10, get_tokenizer().into(), None, None, None, 32, 0.1);
+        let logits = Tensor::arange(0f32, 1024f32, &Device::Cpu).unwrap();
+        let rng = Arc::new(Mutex::new(Isaac64Rng::seed_from_u64(42)));
+        let res = sampler.sample(logits, None, false, rng, true).unwrap();
         assert_eq!(res.token, 1023);
         assert_eq!(res.top_logprobs, None);
         assert_eq!(res.logprob, 1023f64.log(10.) as f32)
     }
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/sequence.rs` & `mistralrs-0.1.5/mistralrs-core/src/sequence.rs`

 * *Files 4% similar despite different names*

```diff
@@ -75,27 +75,34 @@
     return_logprobs: bool,
     responder: Sender<Response>,
     response_index: usize,
     creation_time: u64,
     prefill_prompt_toks: Option<Vec<u32>>,
     suffix: Option<String>,
     prefix: Option<String>,
+    is_tmp: bool,
+    adapters: Option<Vec<String>>,
 
     // Cache
     scaling_cache: Option<Tensor>,
     cache: LayerCaches,
+    draft_cache: LayerCaches,
     xlora_cache: Option<LayerCaches>,
 
     // Mutables
     tokens: Vec<u32>,
     logprobs: Vec<Logprobs>,
     cumulative_logprob: f32,
+    last_logprob: f32,
+    last_completion_bytes_len: usize,
+    last_is_done: Option<StopReason>,
     completion_bytes: Vec<u8>,
     stream_idx: usize,
     pub recognizer: SequenceRecognizer,
+    scheduling_urgency: usize, // The number of passes since scheduling
 
     // GPU things
     pub prompt_tok_per_sec: f32,
     pub prompt_timestamp: Option<u128>,
     group: Arc<Mutex<SequenceGroup>>,
     state: RwLock<SequenceState>,
 }
@@ -116,24 +123,26 @@
         is_xlora: bool,
         group: Arc<Mutex<SequenceGroup>>,
         response_index: usize,
         creation_time: u64,
         recognizer: SequenceRecognizer,
         suffix: Option<String>,
         prefix: Option<String>,
+        adapters: Option<Vec<String>>,
     ) -> Self {
         let prompt_len = tokens.len();
         Self {
             tokens,
             logprobs: Vec::new(),
             prompt_len,
             id,
             timestamp,
             state: RwLock::new(SequenceState::Waiting),
             cache: vec![None; layers],
+            draft_cache: vec![None; layers],
             xlora_cache: if is_xlora {
                 Some(vec![None; layers])
             } else {
                 None
             },
             responder,
             sampler: sampler.into(),
@@ -150,17 +159,41 @@
             recognizer,
             prefill_prompt_toks: None,
             suffix,
             prefix,
             cumulative_logprob: 0.,
             completion_bytes: Vec::new(),
             stream_idx: 0,
+            last_completion_bytes_len: 0,
+            last_logprob: 0.0,
+            last_is_done: None,
+            is_tmp: false,
+            scheduling_urgency: 0,
+            adapters,
         }
     }
 
+    pub fn add_urgency(mut self) -> Self {
+        self.scheduling_urgency += 1;
+        self
+    }
+
+    pub fn reset_urgency(mut self) -> Self {
+        self.scheduling_urgency = 0;
+        self
+    }
+
+    /// Simple metric: (scheduling urgency) + log2(length)
+    /// Takes into account: urgency (scales linear) and length (scales logarithmic)
+    /// Scaling urgency is the number of scheduling passes where we have not been scheduled.
+    pub fn compute_priority(&self) -> f64 {
+        #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
+        (self.scheduling_urgency as f64) + (self.len() as f64).log2()
+    }
+
     pub fn prefill(
         mut self,
         cache: LayerCaches,
         xlora_cache: Option<LayerCaches>,
         toks: Vec<u32>,
     ) -> Self {
         self.cache = cache;
@@ -168,28 +201,31 @@
         self.prefill_prompt_toks = Some(toks);
         self.set_state(SequenceState::RunningPrefillPrompt);
         self
     }
 
     /// This is the number of tokens. If the KV cache is Some, then it will use that.
     pub fn len(&self) -> usize {
+        if let Some(toks) = &self.prefill_prompt_toks {
+            return toks.len();
+        }
+        if self.is_tmp {
+            return self.tokens.len();
+        }
         // Use xlora cache first because of non granular
         if self.xlora_cache.as_ref().is_some_and(|c| c[0].is_some()) {
             self.xlora_cache.as_ref().unwrap()[0]
                 .as_ref()
                 .unwrap()
                 .0
                 .dims()[2]
                 + 1
         } else if let Some((_, x)) = &self.cache[0] {
             x.dims()[2] + 1
         } else {
-            if let Some(toks) = &self.prefill_prompt_toks {
-                return toks.len();
-            }
             self.tokens.len()
         }
     }
 
     pub fn id(&self) -> &usize {
         &self.id
     }
@@ -224,14 +260,18 @@
         &self.completion_bytes
     }
 
     pub fn cache(&mut self) -> &mut Vec<Option<(Tensor, Tensor)>> {
         &mut self.cache
     }
 
+    pub fn draft_cache(&mut self) -> &mut Vec<Option<(Tensor, Tensor)>> {
+        &mut self.draft_cache
+    }
+
     pub fn xlora_cache(&mut self) -> &mut Vec<Option<(Tensor, Tensor)>> {
         self.xlora_cache.as_mut().expect("No X-LoRA cache.")
     }
 
     pub fn scaling_cache(&mut self) -> &mut Option<Tensor> {
         &mut self.scaling_cache
     }
@@ -250,21 +290,23 @@
     }
 
     /// Remove the prefill tokens.
     pub fn reset_prefill_toks(&mut self) {
         self.prefill_prompt_toks = None
     }
 
-    /// Internal api.
-    pub fn add_tmp_tok(&mut self, tok: u32) {
+    /// Internal api to add one raw token.
+    pub(crate) fn add_tmp_tok(&mut self, tok: u32) {
+        self.is_tmp = true;
         self.tokens.push(tok);
     }
 
-    /// Internal api.
-    pub fn remove_tmp_tok(&mut self, n: usize) {
+    /// Internal api to remove n raw tokens.
+    pub(crate) fn remove_tmp_tok(&mut self, n: usize) {
+        self.is_tmp = false;
         self.tokens.truncate(self.tokens.len() - n);
     }
 
     pub fn add_token(
         &mut self,
         tok: Logprobs,
         completion_bytes: Vec<u8>,
@@ -275,15 +317,19 @@
             Some(StopReason::Eos) | Some(StopReason::StopTok(_))
         );
         if !stopped_by_token {
             // Completion bytes is used to check for stop strings, and as the response buffer.
             // We don't need to add stop tokens to the completion bytes to check for stop strings.
             // And by not adding it here, we can avoid having to delete these tokens from the output.
             self.completion_bytes.extend_from_slice(&completion_bytes);
+            self.last_completion_bytes_len = completion_bytes.len();
         }
+        self.last_logprob = tok.logprob;
+        self.last_is_done = *is_done;
+
         self.cumulative_logprob += tok.logprob;
         self.tokens.push(tok.token);
         self.logprobs.push(tok);
         self.prefill_prompt_toks = None;
     }
 
     pub fn responder(&self) -> Sender<Response> {
@@ -425,14 +471,18 @@
     pub fn get_mut_group(&self) -> MutexGuard<'_, SequenceGroup> {
         get_mut_group!(self)
     }
 
     pub fn add_streaming_chunk_choice_to_group(&self, chunk: ChunkChoice) {
         get_mut_group!(self).streaming_chunks.push(chunk);
     }
+
+    pub fn get_adapters(&self) -> Option<Vec<String>> {
+        self.adapters.clone()
+    }
 }
 
 pub struct SequenceGroup {
     n_choices: usize, // The target number of choices to return. Can be decreased if an error is thrown.
     best_of: usize,   // Top n seqs based on cumulative logprobs.
     pub total_prompt_toks: usize,
     pub total_toks: usize,
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/utils/mod.rs` & `mistralrs-0.1.5/mistralrs-core/src/utils/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -158,16 +158,16 @@
                     // Step 3: Set state - This cannot be done in Step 2 as `group` is locking the refcell
                     seq.set_state(SequenceState::Error);
                 }
 
                 let mut p = get_mut_arcmutex!($pipeline);
                 // Also reset non granular state because:
                 // - The sequence is gone
-                // - We should reset the state then.
-                p.set_none_cache(true);
+                // - We should reset the state then, including draft.
+                p.set_none_cache(true, true);
                 $prefix_cacher.evict_all_to_cpu().unwrap();
 
                 continue $label;
             }
         }
     };
 }
@@ -200,19 +200,32 @@
 macro_rules! sample_async {
     (
         $use_async_pool: expr,
         $sampler: expr,
         $logits: expr,
         $ctx: expr,
         $return_logprobs: expr,
-        $rng: expr
+        $rng: expr,
+        $sample_speculative: expr
      ) => {
         if $use_async_pool {
             tokio_rayon::spawn(move || {
-                $sampler.sample($logits, Some(&$ctx), $return_logprobs, $rng)
+                $sampler.sample(
+                    $logits,
+                    Some(&$ctx),
+                    $return_logprobs,
+                    $rng,
+                    $sample_speculative,
+                )
             })
             .await?
         } else {
-            $sampler.sample($logits, Some(&$ctx), $return_logprobs, $rng)?
+            $sampler.sample(
+                $logits,
+                Some(&$ctx),
+                $return_logprobs,
+                $rng,
+                $sample_speculative,
+            )?
         }
     };
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/utils/tokens.rs` & `mistralrs-0.1.5/mistralrs-core/src/utils/tokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/utils/varbuilder_utils.rs` & `mistralrs-0.1.5/mistralrs-core/src/utils/varbuilder_utils.rs`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 use candle_core::{DType, Device, Result, Tensor};
 use candle_nn::{
     var_builder::{SimpleBackend, VarBuilderArgs},
     VarBuilder,
 };
 
+use mistralrs_lora::LoraConfig;
 use tqdm::Iter;
 
 /// Load tensors into a VarBuilder backed by a VarMap using MmapedSafetensors.
 /// Set `silent` to not show a progress bar.
 pub(crate) fn from_mmaped_safetensors<'a>(
     paths: Vec<PathBuf>,
     xlora_paths: Vec<PathBuf>,
@@ -119,7 +120,60 @@
     // Wait until each finishes
     while !handles.iter().all(|h| h.is_finished()) {}
     for h in handles {
         ws.extend(h.join().unwrap()?);
     }
     Ok(VarBuilder::from_tensors(ws, dtype, device))
 }
+
+pub(crate) fn load_preload_adapters<'a>(
+    paths: &Option<HashMap<String, (PathBuf, LoraConfig)>>,
+    dtype: DType,
+    device: &Device,
+    silent: bool,
+) -> Result<Option<HashMap<String, (VarBuilder<'a>, LoraConfig)>>> {
+    if let Some(paths) = paths {
+        let mut map = HashMap::new();
+        for (name, (path, config)) in paths {
+            let tensors = unsafe { candle_core::safetensors::MmapedSafetensors::new(path)? };
+            let mut accum = HashMap::new();
+
+            if silent {
+                for (name, _) in tensors.tensors() {
+                    let new_name = if name.contains("base_model.model.model") {
+                        name.replace("base_model.model.model", "model")
+                    } else {
+                        name.clone()
+                    };
+                    let tensor = tensors
+                        .load(&name, device)?
+                        .to_device(device)?
+                        .to_dtype(dtype)?;
+                    accum.insert(new_name, tensor);
+                }
+            } else {
+                for (name, _) in tensors.tensors().into_iter().tqdm() {
+                    let new_name = if name.contains("base_model.model.model") {
+                        name.replace("base_model.model.model", "model")
+                    } else {
+                        name.clone()
+                    };
+                    let tensor = tensors
+                        .load(&name, device)?
+                        .to_device(device)?
+                        .to_dtype(dtype)?;
+                    accum.insert(new_name, tensor);
+                }
+            }
+            map.insert(
+                name.clone(),
+                (
+                    VarBuilder::from_tensors(accum, dtype, device),
+                    config.clone(),
+                ),
+            );
+        }
+        Ok(Some(map))
+    } else {
+        Ok(None)
+    }
+}
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/xlora_models/classifier.rs` & `mistralrs-0.1.5/mistralrs-core/src/xlora_models/classifier.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/xlora_models/config.rs` & `mistralrs-0.1.5/mistralrs-core/src/xlora_models/config.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-core/src/xlora_models/gemma.rs` & `mistralrs-0.1.5/mistralrs-core/src/xlora_models/phi3.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,317 +1,181 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-use std::sync::Arc;
-
-use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
-use candle_nn::{RotaryEmbedding, VarBuilder};
-use mistralrs_lora::{layer::QLinear, linear_b as linear, LinearLayerLike, LoraConfig, Ordering};
+// This implementation is based on:
+// https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/modeling_phi3.py
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
+use candle_nn::VarBuilder;
+use mistralrs_lora::{layer::QLinear, linear_no_bias, LinearLayerLike, LoraConfig, Ordering};
+use std::{collections::HashMap, sync::Arc};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    models::{flash_attn, gemma::Config, repeat_kv, Cache},
+    layers::{CausalMasker, PhiRotaryEmbedding, RmsNorm},
+    models::phi3::Config,
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
-
-fn default_max_position_embeddings() -> usize {
-    4096
-}
-
-#[derive(Debug, Clone)]
-struct RmsNorm {
-    weight: Tensor,
-    eps: f64,
-}
+use crate::models::{flash_attn, repeat_kv, Cache};
 
-impl RmsNorm {
-    fn new(dim: usize, eps: f64, vb: VarBuilder) -> Result<Self> {
-        let weight = vb.get(dim, "weight")?;
-        Ok(Self { weight, eps })
-    }
-}
-
-impl Module for RmsNorm {
-    fn forward(&self, x: &Tensor) -> Result<Tensor> {
-        let x_dtype = x.dtype();
-        let internal_dtype = match x_dtype {
-            DType::F16 | DType::BF16 => DType::F32,
-            d => d,
-        };
-        let hidden_size = x.dim(D::Minus1)?;
-        let x = x.to_dtype(internal_dtype)?;
-        let norm_x = (x.sqr()?.sum_keepdim(D::Minus1)? / hidden_size as f64)?;
-        let x_normed = x.broadcast_div(&(norm_x + self.eps)?.sqrt()?)?;
-        x_normed
-            .to_dtype(x_dtype)?
-            .broadcast_mul(&(&self.weight + 1.0)?)
-    }
-}
-
-#[derive(Debug, Clone)]
-#[allow(clippy::upper_case_acronyms)]
-struct MLP {
-    gate_proj: Arc<dyn LinearLayerLike + Send + Sync>,
-    up_proj: Arc<dyn LinearLayerLike + Send + Sync>,
-    down_proj: Arc<dyn LinearLayerLike + Send + Sync>,
-    act_fn: candle_nn::Activation,
-}
-
-impl MLP {
-    #[allow(clippy::too_many_arguments)]
-    fn new(
-        cfg: &Config,
-        vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
-        count: &mut usize,
-        ord: &Ordering,
-        mapper: &dyn DeviceMapper,
-        layer_idx: usize,
-        loading_isq: bool,
-    ) -> Result<Self> {
-        let hidden_sz = cfg.hidden_size;
-        let intermediate_sz = cfg.intermediate_size;
-        let gate_proj = linear(
-            hidden_sz,
-            intermediate_sz,
-            false,
-            mapper.set_device(layer_idx, vb.pp("gate_proj"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("gate_proj"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        let up_proj = linear(
-            hidden_sz,
-            intermediate_sz,
-            false,
-            mapper.set_device(layer_idx, vb.pp("up_proj"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("up_proj"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        let down_proj = linear(
-            intermediate_sz,
-            hidden_sz,
-            false,
-            mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("down_proj"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        Ok(Self {
-            gate_proj,
-            up_proj,
-            down_proj,
-            act_fn: cfg.hidden_act()?,
-        })
-    }
-
-    fn forward(
-        &self,
-        xs: &Tensor,
-        scalings: Option<Tensor>,
-        global_scaling_weight: f64,
-        is_scaling_pass: Option<f64>,
-    ) -> Result<Tensor> {
-        let original_dtype = xs.dtype();
-        let mut xs = xs.clone();
-        if self.gate_proj.is_quant() {
-            xs = xs.to_dtype(DType::F32)?;
-        }
-        let lhs = self
-            .gate_proj
-            .lora_forward(
-                &xs,
-                scalings.clone(),
-                global_scaling_weight,
-                is_scaling_pass,
-            )?
-            .apply(&self.act_fn)?;
-        let rhs = self.up_proj.lora_forward(
-            &xs,
-            scalings.clone(),
-            global_scaling_weight,
-            is_scaling_pass,
-        )?;
-        let mut res = self.down_proj.lora_forward(
-            &(lhs * rhs)?,
-            scalings,
-            global_scaling_weight,
-            is_scaling_pass,
-        )?;
-        if self.gate_proj.is_quant() {
-            res = res.to_dtype(original_dtype)?;
-        }
-        Ok(res)
-    }
-}
+use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
 
 #[derive(Debug, Clone)]
 struct Attention {
-    q_proj: Arc<dyn LinearLayerLike + Send + Sync>,
-    k_proj: Arc<dyn LinearLayerLike + Send + Sync>,
-    v_proj: Arc<dyn LinearLayerLike + Send + Sync>,
+    qkv_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
-    rotary_emb: Arc<RotaryEmbedding>,
+    rotary_emb: Arc<PhiRotaryEmbedding>,
     use_flash_attn: bool,
+    sliding_window: Option<usize>,
+    neg_inf: Tensor,
 }
 
 impl Attention {
     #[allow(clippy::too_many_arguments)]
     fn new(
-        rotary_emb: Arc<RotaryEmbedding>,
+        rotary_emb: Arc<PhiRotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
-        let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
-        let num_kv_groups = num_heads / num_kv_heads;
-        let head_dim = cfg.head_dim;
-        let bias = cfg.attention_bias;
-        let q_proj = linear(
-            hidden_sz,
-            num_heads * head_dim,
-            bias,
-            mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("q_proj"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        let k_proj = linear(
-            hidden_sz,
-            num_kv_heads * head_dim,
-            bias,
-            mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("k_proj"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        let v_proj = linear(
-            hidden_sz,
-            num_kv_heads * head_dim,
-            bias,
-            mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("v_proj"), false),
+        let head_dim = cfg.head_dim();
+        let op_size = num_heads * head_dim + 2 * num_kv_heads * head_dim;
+        let qkv_proj = linear_no_bias(
+            cfg.hidden_size,
+            op_size,
+            mapper.set_device(layer_idx, vb.pp("qkv_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("qkv_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
-        let o_proj = linear(
+        let o_proj = linear_no_bias(
             num_heads * head_dim,
-            hidden_sz,
-            bias,
+            cfg.hidden_size,
             mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("o_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         Ok(Self {
-            q_proj,
-            k_proj,
-            v_proj,
+            qkv_proj,
             o_proj,
+            rotary_emb,
             num_heads,
             num_kv_heads,
-            num_kv_groups,
+            num_kv_groups: num_heads / num_kv_heads,
             head_dim,
-            rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
+            sliding_window: cfg.sliding_window,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        position_ids: &[usize],
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         let (b_sz, q_len, _) = xs.dims3()?;
 
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
-        if self.q_proj.is_quant() {
+        if self.qkv_proj.is_quant() {
             xs = xs.to_dtype(DType::F32)?;
         }
-        let mut q = self.q_proj.lora_forward(
-            &xs,
-            scalings.clone(),
-            global_scaling_weight,
-            is_scaling_pass,
-        )?;
-        let mut k = self.k_proj.lora_forward(
-            &xs,
-            scalings.clone(),
-            global_scaling_weight,
-            is_scaling_pass,
-        )?;
-        let mut v = self.v_proj.lora_forward(
+        let mut qkv = self.qkv_proj.lora_forward(
             &xs,
             scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
-        if self.q_proj.is_quant() {
-            q = q.to_dtype(original_dtype)?;
-            k = k.to_dtype(original_dtype)?;
-            v = v.to_dtype(original_dtype)?;
+        if self.qkv_proj.is_quant() {
+            qkv = qkv.to_dtype(original_dtype)?;
         }
+        let query_pos = self.num_heads * self.head_dim;
+        let q = qkv.narrow(D::Minus1, 0, query_pos)?;
+        let k = qkv.narrow(D::Minus1, query_pos, self.num_kv_heads * self.head_dim)?;
+        let v = qkv.narrow(
+            D::Minus1,
+            query_pos + self.num_kv_heads * self.head_dim,
+            self.num_kv_heads * self.head_dim,
+        )?;
 
-        let mut q = q.reshape((b_sz * q_len, self.num_heads, self.head_dim))?;
-        let mut k = k.reshape((b_sz * q_len, self.num_kv_heads, self.head_dim))?;
+        let q = q
+            .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
+            .transpose(1, 2)?;
+        let k = k
+            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
+            .transpose(1, 2)?;
         let v = v
             .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
             .transpose(1, 2)?;
 
-        self.rotary_emb
-            .forward(seqlen_offsets, &start_offsets_kernel, &mut q, &mut k, b_sz)?;
-
-        if q.rank() == 3 {
-            q = q
-                .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
-                .transpose(1, 2)?
-                .contiguous()?;
-            k = k
-                .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
-                .transpose(1, 2)?
-                .contiguous()?;
-        }
-
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
-                (k, v)
+        let (q, k) = self
+            .rotary_emb
+            .forward(&q, &k, seqlen_offsets, position_ids)?;
+
+        let (k, v, attn_mask) = match kv_cache.clone() {
+            None => (k, v, attention_mask.cloned()),
+            Some((mut prev_k, mut prev_v)) => {
+                let mut mask = attention_mask.cloned();
+                if let Some(sliding_window) = self.sliding_window {
+                    let kv_seq_len = prev_k.dim(2)?;
+                    if kv_seq_len > sliding_window {
+                        prev_k = prev_k.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        prev_v = prev_v.narrow(
+                            2,
+                            kv_seq_len - (sliding_window - 1),
+                            sliding_window - 1,
+                        )?;
+                        if let Some(ref mut mask) = mask {
+                            let mask_len = mask.dim(1)?;
+                            *mask = mask.narrow(
+                                1,
+                                mask_len - (sliding_window - 1),
+                                sliding_window - 1,
+                            )?;
+                            *mask = Tensor::cat(
+                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
+                                D::Minus1,
+                            )?;
+                        }
+                    }
+                }
+                let k = Tensor::cat(&[prev_k, k], 2)?;
+                let v = Tensor::cat(&[prev_v, v], 2)?;
+                (k, v, mask)
             }
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
@@ -322,78 +186,163 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attention_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
-            };
+            let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
-        if self.q_proj.is_quant() {
+        if self.qkv_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = self.o_proj.lora_forward(
             &attn_output.transpose(1, 2)?.reshape((b_sz, q_len, ()))?,
             scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
-        if self.q_proj.is_quant() {
+        if self.qkv_proj.is_quant() {
+            res = res.to_dtype(original_dtype)?;
+        }
+        Ok(res)
+    }
+}
+
+#[derive(Debug, Clone)]
+struct Mlp {
+    gate_up_proj: Arc<dyn LinearLayerLike + Send + Sync>,
+    down_proj: Arc<dyn LinearLayerLike + Send + Sync>,
+    act_fn: candle_nn::Activation,
+    i_size: usize,
+}
+
+impl Mlp {
+    #[allow(clippy::too_many_arguments)]
+    fn new(
+        cfg: &Config,
+        vb: VarBuilder,
+        lora_config: &[((String, String), LoraConfig)],
+        count: &mut usize,
+        ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
+    ) -> Result<Self> {
+        let hidden_size = cfg.hidden_size;
+        let i_size = cfg.intermediate_size;
+        let gate_up_proj = linear_no_bias(
+            hidden_size,
+            2 * i_size,
+            mapper.set_device(layer_idx, vb.pp("gate_up_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("gate_up_proj"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )?;
+        let down_proj = linear_no_bias(
+            i_size,
+            hidden_size,
+            mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )?;
+        Ok(Self {
+            gate_up_proj,
+            down_proj,
+            act_fn: cfg.hidden_act,
+            i_size,
+        })
+    }
+
+    fn forward(
+        &self,
+        xs: &Tensor,
+        scalings: Option<Tensor>,
+        global_scaling_weight: f64,
+        is_scaling_pass: Option<f64>,
+    ) -> Result<Tensor> {
+        let original_dtype = xs.dtype();
+        let mut xs = xs.clone();
+        if self.gate_up_proj.is_quant() {
+            xs = xs.to_dtype(DType::F32)?;
+        }
+        let up_states = self.gate_up_proj.lora_forward(
+            &xs,
+            scalings.clone(),
+            global_scaling_weight,
+            is_scaling_pass,
+        )?;
+        let gate = up_states.narrow(D::Minus1, 0, self.i_size)?;
+        let up_states = up_states.narrow(D::Minus1, self.i_size, self.i_size)?;
+        let up_states = (up_states * gate.apply(&self.act_fn))?;
+        let mut res = self.down_proj.lora_forward(
+            &up_states,
+            scalings,
+            global_scaling_weight,
+            is_scaling_pass,
+        )?;
+        if self.gate_up_proj.is_quant() {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
 struct DecoderLayer {
     self_attn: Attention,
-    mlp: MLP,
+    mlp: Mlp,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
     #[allow(clippy::too_many_arguments)]
     fn new(
-        rotary_emb: Arc<RotaryEmbedding>,
+        rotary_emb: Arc<PhiRotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let self_attn = Attention::new(
             rotary_emb,
             cfg,
             vb.pp("self_attn"),
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
+            preload_adapters,
         )?;
-        let mlp = MLP::new(
+        let mlp = Mlp::new(
             cfg,
             vb.pp("mlp"),
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
+            preload_adapters,
         )?;
         let input_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
         )?;
         let post_attention_layernorm = RmsNorm::new(
@@ -411,242 +360,193 @@
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        position_ids: &[usize],
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         let residual = xs;
         let xs = self.input_layernorm.forward(xs)?;
         let xs = self.self_attn.forward(
             &xs,
             attention_mask,
             seqlen_offsets,
-            start_offsets_kernel,
+            position_ids,
             kv_cache,
             scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
         let xs = (xs + residual)?;
         let residual = &xs;
         let xs = self.mlp.forward(
             &xs.apply(&self.post_attention_layernorm)?,
-            scalings.clone(),
+            scalings,
             global_scaling_weight,
             is_scaling_pass,
-        )?;
+        );
         residual + xs
     }
 }
 
-pub struct XLoraModel {
+pub struct Model {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QLinear,
     dtype: DType,
-    hidden_size: usize,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
-    xlora_classifier: Option<XLoraClassifier>,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
+    xlora_classifier: Option<XLoraClassifier>,
+    sliding_window: Option<usize>,
 }
 
-impl XLoraModel {
+impl Model {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
-        is_gptx: bool,
+        _is_gptx: bool,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         real_device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
         let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
         let embed_tokens = candle_nn::embedding(
             cfg.vocab_size,
             cfg.hidden_size,
             mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
         )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
         let vb_l = vb_m.pp("layers");
         let mut count = 0;
         for layer_idx in 0..cfg.num_hidden_layers {
-            let rotary_emb = Arc::new(RotaryEmbedding::new(
-                cfg.rope_theta as f32,
-                cfg.head_dim,
-                cfg.max_position_embeddings,
-                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
-                is_gptx,
+            let rotary_emb = Arc::new(PhiRotaryEmbedding::new(
                 vb.dtype(),
+                cfg,
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
                 vb_l.pp(layer_idx),
                 lora_config,
                 &mut count,
                 &xlora_ordering,
                 &*mapper,
                 layer_idx,
                 loading_isq,
+                preload_adapters,
             )?;
             layers.push(layer)
         }
-        if xlora_config.is_none() {
+        if xlora_config.is_none() && preload_adapters.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
-                Arc::get_mut(&mut layer.self_attn.k_proj)
+                Arc::get_mut(&mut layer.self_attn.qkv_proj)
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.self_attn.o_proj)
                     .unwrap()
                     .merge_weights()?;
-                Arc::get_mut(&mut layer.self_attn.q_proj)
-                    .unwrap()
-                    .merge_weights()?;
-                Arc::get_mut(&mut layer.self_attn.v_proj)
-                    .unwrap()
-                    .merge_weights()?;
 
                 Arc::get_mut(&mut layer.mlp.down_proj)
                     .unwrap()
                     .merge_weights()?;
-                Arc::get_mut(&mut layer.mlp.gate_proj)
-                    .unwrap()
-                    .merge_weights()?;
-                Arc::get_mut(&mut layer.mlp.up_proj)
+                Arc::get_mut(&mut layer.mlp.gate_up_proj)
                     .unwrap()
                     .merge_weights()?;
             }
         }
         let norm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_nm_device(vb_m.pp("norm"), false),
         )?;
-        let lm_head = candle_nn::Linear::new(embed_tokens.embeddings().clone(), None);
+        let lm_head = candle_nn::linear_no_bias(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QLinear::from_linear(lm_head),
             device: real_device,
             dtype: vb.dtype(),
-            hidden_size: cfg.hidden_size,
             cache: Cache::new(cfg.num_hidden_layers, true),
-            max_seq_len: default_max_position_embeddings(),
+            max_seq_len: cfg.max_position_embeddings,
+            mapper,
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
-            mapper,
+            sliding_window: cfg.sliding_window,
         })
     }
 
-    fn prepare_decoder_attention_mask(
-        &self,
-        b_size: usize,
-        tgt_len: usize,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| (0..tgt_len).map(move |j| if i < j { f32::NEG_INFINITY } else { 0. }))
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
-    fn calculate_past_kv_len(
-        &self,
-        seq_len: usize,
-        kv_cache_1: &Option<(Tensor, Tensor)>,
-    ) -> Result<usize> {
-        if kv_cache_1.is_none() {
-            return Ok(0);
-        }
-        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
-        if k_cache_1.dims()[0] <= seq_len {
-            Ok(0)
-        } else {
-            let indexed = k_cache_1.i(seq_len)?;
-            let dims = indexed.dims();
-            Ok(dims[dims.len() - 2])
-        }
-    }
-
     #[allow(clippy::too_many_arguments)]
     fn inner_forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        position_ids: &[usize],
         scalings: Option<Tensor>,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
-        let (b_size, seq_len) = input_ids.dims2()?;
-        if seqlen_offsets.len() > b_size {
-            candle_core::bail!("Expected seqlen offsets have length equal to batch size.")
-        }
-
+        let mut xs = self.embed_tokens.forward(input_ids)?;
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
                 self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
-        let past_key_values_length =
-            self.calculate_past_kv_len(seq_len, cache.first().as_ref().unwrap())?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask =
-                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
-            Some(mask)
-        };
-        let xs = self.embed_tokens.forward(input_ids)?;
-        let mut xs = (xs * (self.hidden_size as f64).sqrt())?;
+        let attention_mask = CausalMasker.make_causal_mask_with_sliding_window(
+            input_ids,
+            &cache,
+            self.sliding_window,
+        )?;
+        let past_key_values_length = CausalMasker.calculate_past_kv_len(&cache)?;
+        let position_ids = position_ids
+            .iter()
+            .map(|p| *p + past_key_values_length)
+            .collect::<Vec<_>>();
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
                 seqlen_offsets,
-                start_offsets_kernel.clone(),
+                &position_ids,
                 &mut cache[i],
                 scalings.clone(),
                 self.xlora_classifier
                     .as_ref()
                     .map(|classifier| classifier.get_global_scaling_weight())
                     .unwrap_or(1.0),
                 is_scaling_pass,
@@ -664,34 +564,35 @@
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
         context_lens: Vec<(usize, usize)>,
+        position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         if self.xlora_classifier.is_some() {
             let scalings = self.get_scalings(
                 input_ids,
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
-                &vec![usize::MAX; context_lens.len()],
+                &position_ids,
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
-                        start_offsets_kernel_full,
+                        &position_ids,
                         Some(scalings),
                         true,
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
                 if self.lm_head.is_quant() {
@@ -700,15 +601,15 @@
                 extract_logits(&res.apply(&self.lm_head)?, context_lens)
             } else {
                 // is_full_pass=true is ok because no_kv_cache=false
                 let mut res = self
                     .inner_forward(
                         input_ids,
                         seqlen_offsets,
-                        start_offsets_kernel,
+                        &position_ids,
                         Some(scalings),
                         true,
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
                 if self.lm_head.is_quant() {
@@ -717,30 +618,30 @@
                 extract_logits(&res.apply(&self.lm_head)?, context_lens)
             }
         } else {
             let mut res = self
                 .inner_forward(
                     input_ids,
                     seqlen_offsets,
-                    start_offsets_kernel,
+                    &position_ids,
                     None,
                     false,
                     no_kv_cache,
                     None,
                 )?
                 .contiguous()?;
             if self.lm_head.is_quant() {
                 res = res.to_dtype(DType::F32)?;
             }
             extract_logits(&res.apply(&self.lm_head)?, context_lens)
         }
     }
 }
 
-impl NormalModel for XLoraModel {
+impl NormalModel for Model {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
         _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
@@ -754,102 +655,111 @@
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         context_lens: Vec<(usize, usize)>,
-        _position_ids: Vec<usize>,
+        position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             start_offsets_kernel,
             start_offsets_kernel_full,
             no_kv_cache,
             non_granular_state,
             context_lens,
+            position_ids,
         )
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
     fn device(&self) -> &Device {
         &self.device
     }
     fn is_xlora(&self) -> bool {
-        false
+        true
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
     fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
         tensors.push((self.lm_head.inner(), None));
         for (i, layer) in self.layers.iter_mut().enumerate() {
             tensors.push((
-                Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner(),
-                Some(i),
-            ));
-            tensors.push((
-                Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner(),
-                Some(i),
-            ));
-            tensors.push((
-                Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner(),
+                Arc::get_mut(&mut layer.self_attn.qkv_proj).unwrap().inner(),
                 Some(i),
             ));
             tensors.push((
                 Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner(),
                 Some(i),
             ));
             tensors.push((
                 Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner(),
                 Some(i),
             ));
             tensors.push((
-                Arc::get_mut(&mut layer.mlp.gate_proj).unwrap().inner(),
-                Some(i),
-            ));
-            tensors.push((
-                Arc::get_mut(&mut layer.mlp.up_proj).unwrap().inner(),
+                Arc::get_mut(&mut layer.mlp.gate_up_proj).unwrap().inner(),
                 Some(i),
             ));
         }
         (tensors, &*self.mapper)
     }
+    fn activate_adapters(&mut self, adapter_names: Vec<String>) -> Result<usize> {
+        let mut sum = 0;
+        for layer in self.layers.iter_mut() {
+            sum += Arc::get_mut(&mut layer.self_attn.qkv_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.o_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+
+            sum += Arc::get_mut(&mut layer.mlp.down_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.mlp.gate_up_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+        }
+        Ok(sum)
+    }
 }
 
-impl ScalingsMaker for XLoraModel {
+impl ScalingsMaker for Model {
     fn dtype(&self) -> DType {
         self.dtype
     }
     fn get_cache(&self) -> &Cache {
         &self.cache
     }
     fn get_classifier(&self) -> &XLoraClassifier {
         self.xlora_classifier.as_ref().unwrap()
     }
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
-        start_offsets_kernel: Tensor,
+        _start_offsets_kernel: Tensor,
         scalings: Tensor,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
-        _context_lens: &[usize],
+        context_lens: &[usize],
     ) -> Result<Tensor> {
+        // NOTE(EricLBuehler): hacky yes, but passing the context lens to start the position ids calculation works
         self.inner_forward(
             input_ids,
             seqlen_offsets,
-            start_offsets_kernel,
+            context_lens,
             Some(scalings),
             is_full_pass,
             no_kv_cache,
             is_scaling_pass,
         )
     }
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/xlora_models/llama.rs` & `mistralrs-0.1.5/mistralrs-core/src/xlora_models/llama.rs`

 * *Files 12% similar despite different names*

```diff
@@ -7,72 +7,47 @@
 };
 use std::{collections::HashMap, sync::Arc};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::RmsNorm,
+    layers::{CausalMasker, RmsNorm},
     models::{self, flash_attn, llama::Config, repeat_kv, LayerCaches},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
 
 #[derive(Debug, Clone)]
-pub struct Cache {
-    masks: HashMap<usize, Tensor>,
-}
-
-impl Cache {
-    pub fn new() -> Result<Self> {
-        Ok(Self {
-            masks: HashMap::new(),
-        })
-    }
-
-    fn mask(&mut self, t: usize, device: &Device) -> Result<Tensor> {
-        if let Some(mask) = self.masks.get(&t) {
-            mask.to_device(device)
-        } else {
-            let mask: Vec<_> = (0..t)
-                .flat_map(|i| (0..t).map(move |j| u8::from(j > i)))
-                .collect();
-            let mask = Tensor::from_slice(&mask, (t, t), device)?;
-            self.masks.insert(t, mask.clone());
-            Ok(mask)
-        }
-    }
-}
-
-#[derive(Debug, Clone)]
 struct CausalSelfAttention {
     q_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     k_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     v_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     num_attention_heads: usize,
     num_key_value_heads: usize,
     head_dim: usize,
     use_flash_attn: bool,
     rotary_emb: Arc<RotaryEmbedding>,
     max_seq_len: usize,
+    neg_inf: Tensor,
 }
 
 impl CausalSelfAttention {
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &self,
         x: &Tensor,
+        mask: &Option<Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         block_idx: usize,
         kv_cache: &mut LayerCaches,
-        cache: &mut Cache,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         let (b_sz, seq_len, hidden_size) = x.dims3()?;
 
         let original_dtype = x.dtype();
@@ -154,18 +129,15 @@
             flash_attn(&q, &k, &v, softmax_scale, seq_len > 1)?.transpose(1, 2)?
         } else {
             let in_dtype = q.dtype();
             let q = q.to_dtype(DType::F32)?;
             let k = k.to_dtype(DType::F32)?;
             let v = v.to_dtype(DType::F32)?;
             let att = (q.matmul(&k.t()?)? / (self.head_dim as f64).sqrt())?;
-            let mask = cache
-                .mask(seq_len, att.device())?
-                .broadcast_as(att.shape())?;
-            let att = masked_fill(&att, &mask, f32::NEG_INFINITY)?;
+            let att = CausalMasker.apply_mask(mask, att, &self.neg_inf)?;
             let att = candle_nn::ops::softmax(&att, D::Minus1)?;
             // Convert to contiguous as matmul doesn't support strided vs for now.
             att.matmul(&v.contiguous()?)?.to_dtype(in_dtype)?
         };
         let mut y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, hidden_size])?;
         if self.q_proj.is_quant() {
             y = y.to_dtype(DType::F32)?;
@@ -182,83 +154,82 @@
         Ok(res)
     }
 
     #[allow(clippy::too_many_arguments)]
     fn load(
         vb: VarBuilder,
         cfg: &Config,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
         rope: Arc<RotaryEmbedding>,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let size_in = cfg.hidden_size;
         let size_q = (cfg.hidden_size / cfg.num_attention_heads) * cfg.num_attention_heads;
         let size_kv = (cfg.hidden_size / cfg.num_attention_heads) * cfg.num_key_value_heads;
         let q_proj = linear(
             size_in,
             size_q,
             mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("q_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let k_proj = linear(
             size_in,
             size_kv,
             mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("k_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let v_proj = linear(
             size_in,
             size_kv,
             mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("v_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let o_proj = linear(
             size_q,
             size_in,
             mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("o_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         Ok(Self {
             q_proj,
             k_proj,
             v_proj,
             o_proj,
             num_attention_heads: cfg.num_attention_heads,
             num_key_value_heads: cfg.num_key_value_heads,
             head_dim: cfg.hidden_size / cfg.num_attention_heads,
             use_flash_attn: cfg.use_flash_attn,
             rotary_emb: rope,
             max_seq_len: cfg.max_position_embeddings,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 }
 
-fn masked_fill(on_false: &Tensor, mask: &Tensor, on_true: f32) -> Result<Tensor> {
-    let shape = mask.shape();
-    let on_true = Tensor::new(on_true, on_false.device())?.broadcast_as(shape.dims())?;
-    let m = mask.where_cond(&on_true, on_false)?;
-    Ok(m)
-}
-
 #[derive(Debug, Clone)]
 struct Mlp {
     c_fc1: Arc<dyn LinearLayerLike + Send + Sync>,
     c_fc2: Arc<dyn LinearLayerLike + Send + Sync>,
     c_proj: Arc<dyn LinearLayerLike + Send + Sync>,
 }
 
@@ -298,49 +269,53 @@
         Ok(res)
     }
 
     #[allow(clippy::too_many_arguments)]
     fn load(
         vb: VarBuilder,
         cfg: &Config,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let h_size = cfg.hidden_size;
         let i_size = cfg.intermediate_size;
         let c_fc1 = linear(
             h_size,
             i_size,
             mapper.set_device(layer_idx, vb.pp("gate_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("gate_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let c_fc2 = linear(
             h_size,
             i_size,
             mapper.set_device(layer_idx, vb.pp("up_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("up_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let c_proj = linear(
             i_size,
             h_size,
             mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("down_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         Ok(Self {
             c_fc1,
             c_fc2,
             c_proj,
         })
     }
@@ -355,32 +330,32 @@
 }
 
 impl Block {
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &self,
         x: &Tensor,
+        mask: &Option<Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         block_idx: usize,
         kv_cache: &mut LayerCaches,
-        cache: &mut Cache,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         let residual = x;
         let x = self.rms_1.forward(x)?;
         let x = (self.attn.forward(
             &x,
+            mask,
             seqlen_offsets,
             start_offsets_kernel,
             block_idx,
             kv_cache,
-            cache,
             scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )? + residual)?;
         let residual = &x;
         let x = (self.mlp.forward(
             &self.rms_2.forward(&x)?,
@@ -391,42 +366,45 @@
         Ok(x)
     }
 
     #[allow(clippy::too_many_arguments)]
     fn load(
         vb: VarBuilder,
         cfg: &Config,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
         rope: Arc<RotaryEmbedding>,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let attn = CausalSelfAttention::load(
             vb.pp("self_attn"),
             cfg,
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
             rope,
+            preload_adapters,
         )?;
         let mlp = Mlp::load(
             vb.pp("mlp"),
             cfg,
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
+            preload_adapters,
         )?;
         let rms_1 = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
         )?;
         let rms_2 = RmsNorm::new(
@@ -446,55 +424,55 @@
 pub struct XLoraLlama {
     wte: Embedding,
     blocks: Vec<Block>,
     ln_f: RmsNorm,
     lm_head: QLinear,
     pub kv_cache: models::Cache,
     pub device: Device,
-    cache: Cache,
     xlora_classifier: Option<XLoraClassifier>,
     dtype: DType,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl XLoraLlama {
     #[allow(clippy::too_many_arguments)]
     fn inner_forward(
         &mut self,
-        x: &Tensor,
+        input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Option<Tensor>,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
-        let mut x = self.wte.forward(x)?;
+        let mut x = self.wte.forward(input_ids)?;
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.kv_cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
                 self.kv_cache.xlora_lock().clone_from(&new_cache);
             }
             self.kv_cache.xlora_lock()
         } else {
             self.kv_cache.lock()
         };
+        let mask = CausalMasker.make_causal_mask(input_ids, &cache)?;
         for (block_idx, block) in self.blocks.iter().enumerate() {
             x = self.mapper.map(x, block_idx)?;
             x = block.forward(
                 &x,
+                &mask.clone().map(|m| m.to_device(x.device()).unwrap()),
                 seqlen_offsets,
                 start_offsets_kernel.clone(),
                 block_idx,
                 &mut cache,
-                &mut self.cache,
                 scalings.clone(),
                 self.xlora_classifier
                     .as_ref()
                     .map(|classifier| classifier.get_global_scaling_weight())
                     .unwrap_or(1.0),
                 is_scaling_pass,
             )?;
@@ -582,21 +560,22 @@
         }
     }
 
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         real_device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let dtype = vb.dtype();
         let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
         let wte = embedding(
             cfg.vocab_size,
             cfg.hidden_size,
             mapper.set_nm_device(vb.pp("model.embed_tokens"), false),
@@ -632,19 +611,20 @@
                     lora_config,
                     &mut count,
                     &xlora_ordering,
                     &*mapper,
                     i,
                     loading_isq,
                     rotary_emb,
+                    preload_adapters,
                 )
                 .expect("Failed to load block.")
             })
             .collect();
-        if xlora_config.is_none() {
+        if xlora_config.is_none() && preload_adapters.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in blocks.iter_mut().tqdm() {
                 Arc::get_mut(&mut layer.attn.k_proj)
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.attn.o_proj)
@@ -670,15 +650,14 @@
         }
 
         Ok(Self {
             wte,
             blocks,
             ln_f,
             lm_head: QLinear::from_linear(lm_head),
-            cache: Cache::new()?,
             kv_cache: models::Cache::new(cfg.num_hidden_layers, true),
             device: real_device,
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
             dtype,
             mapper,
@@ -759,14 +738,42 @@
             tensors.push((
                 Arc::get_mut(&mut layer.mlp.c_proj).unwrap().inner(),
                 Some(i),
             ));
         }
         (tensors, &*self.mapper)
     }
+    fn activate_adapters(&mut self, adapter_names: Vec<String>) -> Result<usize> {
+        let mut sum = 0;
+        for layer in self.blocks.iter_mut() {
+            sum += Arc::get_mut(&mut layer.attn.k_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.attn.o_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.attn.q_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.attn.v_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+
+            sum += Arc::get_mut(&mut layer.mlp.c_fc1)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.mlp.c_fc2)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.mlp.c_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+        }
+        Ok(sum)
+    }
 }
 
 impl ScalingsMaker for XLoraLlama {
     fn dtype(&self) -> DType {
         self.dtype
     }
     fn get_cache(&self) -> &models::Cache {
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/xlora_models/mistral.rs` & `mistralrs-0.1.5/mistralrs-core/src/xlora_models/mixtral.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,212 +1,123 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-/// Mistral LLM, https://github.com/mistralai/mistral-src
-use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
+/// Mixtral Model
+/// https://github.com/huggingface/transformers/blob/main/src/transformers/models/mixtral/modeling_mixtral.py
+/// https://mistral.ai/news/mixtral-of-experts/
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
 use candle_nn::{Activation, RotaryEmbedding, VarBuilder};
-use mistralrs_lora::{layer::QLinear, linear_no_bias, LinearLayerLike, LoraConfig, Ordering};
-use std::sync::Arc;
+use mistralrs_lora::{linear_no_bias, LinearLayerLike, LoraConfig, Ordering};
+use std::{collections::HashMap, sync::Arc};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::RmsNorm,
-    models::{flash_attn, mistral::Config, repeat_kv, Cache},
+    layers::{CausalMasker, RmsNorm},
+    models::{flash_attn, mixtral::Config, repeat_kv, Cache},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{classifier::XLoraClassifier, config::XLoraConfig, NonGranularState, ScalingsMaker};
-
-#[derive(Debug, Clone)]
-#[allow(clippy::upper_case_acronyms)]
-struct MLP {
-    gate_proj: Arc<dyn LinearLayerLike + Send + Sync>,
-    up_proj: Arc<dyn LinearLayerLike + Send + Sync>,
-    down_proj: Arc<dyn LinearLayerLike + Send + Sync>,
-    act_fn: Activation,
-}
-
-impl MLP {
-    #[allow(clippy::too_many_arguments)]
-    fn new(
-        cfg: &Config,
-        vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
-        count: &mut usize,
-        ord: &Ordering,
-        mapper: &dyn DeviceMapper,
-        layer_idx: usize,
-        loading_isq: bool,
-    ) -> Result<Self> {
-        let hidden_sz = cfg.hidden_size;
-        let intermediate_sz = cfg.intermediate_size;
-        let gate_proj = linear_no_bias(
-            hidden_sz,
-            intermediate_sz,
-            mapper.set_device(layer_idx, vb.pp("gate_proj"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("gate_proj"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        let up_proj = linear_no_bias(
-            hidden_sz,
-            intermediate_sz,
-            mapper.set_device(layer_idx, vb.pp("up_proj"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("up_proj"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        let down_proj = linear_no_bias(
-            intermediate_sz,
-            hidden_sz,
-            mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("down_proj"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        Ok(Self {
-            gate_proj,
-            up_proj,
-            down_proj,
-            act_fn: cfg.hidden_act,
-        })
-    }
-
-    fn forward(
-        &self,
-        xs: &Tensor,
-        scalings: Option<Tensor>,
-        global_scaling_weight: f64,
-        is_scaling_pass: Option<f64>,
-    ) -> Result<Tensor> {
-        let original_dtype = xs.dtype();
-        let mut xs = xs.clone();
-        if self.gate_proj.is_quant() {
-            xs = xs.to_dtype(DType::F32)?;
-        }
-        let lhs = self
-            .gate_proj
-            .lora_forward(
-                &xs,
-                scalings.clone(),
-                global_scaling_weight,
-                is_scaling_pass,
-            )?
-            .apply(&self.act_fn)?;
-        let rhs = self.up_proj.lora_forward(
-            &xs,
-            scalings.clone(),
-            global_scaling_weight,
-            is_scaling_pass,
-        )?;
-        let mut res = self.down_proj.lora_forward(
-            &(lhs * rhs)?,
-            scalings,
-            global_scaling_weight,
-            is_scaling_pass,
-        )?;
-        if self.gate_proj.is_quant() {
-            res = res.to_dtype(original_dtype)?;
-        }
-        Ok(res)
-    }
-}
+use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
 
 #[derive(Debug, Clone)]
 struct Attention {
     q_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     k_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     v_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
     sliding_window: Option<usize>,
+    neg_inf: Tensor,
 }
 
 impl Attention {
     #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let num_kv_groups = num_heads / num_kv_heads;
         let head_dim = hidden_sz / num_heads;
         let q_proj = linear_no_bias(
             hidden_sz,
             num_heads * head_dim,
             mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("q_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let k_proj = linear_no_bias(
             hidden_sz,
             num_kv_heads * head_dim,
             mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("k_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let v_proj = linear_no_bias(
             hidden_sz,
             num_kv_heads * head_dim,
             mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("v_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let o_proj = linear_no_bias(
             num_heads * head_dim,
             hidden_sz,
             mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("o_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         Ok(Self {
             q_proj,
             k_proj,
             v_proj,
             o_proj,
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
-            sliding_window: cfg.sliding_window,
+            sliding_window: Some(cfg.sliding_window),
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
-        &self,
+        &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
@@ -311,18 +222,15 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attn_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(&mask)?,
-            };
+            let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = self.o_proj.lora_forward(
@@ -335,76 +243,317 @@
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
+struct BlockSparseTop2MLP {
+    w1: Arc<dyn LinearLayerLike + Send + Sync>,
+    w2: Arc<dyn LinearLayerLike + Send + Sync>,
+    w3: Arc<dyn LinearLayerLike + Send + Sync>,
+    act_fn: Activation,
+}
+
+impl BlockSparseTop2MLP {
+    #[allow(clippy::too_many_arguments)]
+    fn new(
+        cfg: &Config,
+        vb: VarBuilder,
+        lora_config: &[((String, String), LoraConfig)],
+        count: &mut usize,
+        ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
+    ) -> Result<Self> {
+        let hidden_sz = cfg.hidden_size;
+        let intermediate_sz = cfg.intermediate_size;
+        let w1 = linear_no_bias(
+            hidden_sz,
+            intermediate_sz,
+            mapper.set_device(layer_idx, vb.pp("w1"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("w1"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )?;
+        let w2 = linear_no_bias(
+            intermediate_sz,
+            hidden_sz,
+            mapper.set_device(layer_idx, vb.pp("w2"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("w2"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )?;
+        let w3 = linear_no_bias(
+            hidden_sz,
+            intermediate_sz,
+            mapper.set_device(layer_idx, vb.pp("w3"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("w3"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )?;
+        Ok(Self {
+            w1,
+            w2,
+            w3,
+            act_fn: cfg.hidden_act,
+        })
+    }
+
+    fn forward(
+        &self,
+        xs: &Tensor,
+        scalings: Option<Tensor>,
+        global_scaling_weight: f64,
+        is_scaling_pass: Option<f64>,
+    ) -> Result<Tensor> {
+        let original_dtype = xs.dtype();
+        let mut xs = xs.clone();
+        if self.w1.is_quant() {
+            xs = xs.to_dtype(DType::F32)?;
+        }
+        let lhs = self
+            .w1
+            .lora_forward(
+                &xs,
+                scalings.clone(),
+                global_scaling_weight,
+                is_scaling_pass,
+            )?
+            .apply(&self.act_fn)?;
+        let rhs = self.w3.lora_forward(
+            &xs,
+            scalings.clone(),
+            global_scaling_weight,
+            is_scaling_pass,
+        )?;
+        let mut res = self.w2.lora_forward(
+            &(lhs * rhs)?,
+            scalings.clone(),
+            global_scaling_weight,
+            is_scaling_pass,
+        )?;
+        if self.w1.is_quant() {
+            res = res.to_dtype(original_dtype)?;
+        }
+        Ok(res)
+    }
+}
+
+#[derive(Debug, Clone)]
+struct SparseMoeBlock {
+    gate: Arc<dyn LinearLayerLike + Send + Sync>,
+    experts: Vec<BlockSparseTop2MLP>,
+    num_experts_per_tok: usize,
+}
+
+impl SparseMoeBlock {
+    #[allow(clippy::too_many_arguments)]
+    fn new(
+        cfg: &Config,
+        vb: VarBuilder,
+        lora_config: &[((String, String), LoraConfig)],
+        count: &mut usize,
+        ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
+    ) -> Result<Self> {
+        let gate = linear_no_bias(
+            cfg.hidden_size,
+            cfg.num_local_experts,
+            mapper.set_device(layer_idx, vb.pp("gate"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("gate"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )?;
+        let mut experts = Vec::with_capacity(cfg.num_local_experts);
+        let vb = vb.pp("experts");
+        for idx in 0..cfg.num_local_experts {
+            let expert = BlockSparseTop2MLP::new(
+                cfg,
+                vb.pp(idx),
+                lora_config,
+                count,
+                ord,
+                mapper,
+                layer_idx,
+                loading_isq,
+                preload_adapters,
+            )?;
+            experts.push(expert)
+        }
+        Ok(SparseMoeBlock {
+            gate,
+            experts,
+            num_experts_per_tok: cfg.num_experts_per_tok,
+        })
+    }
+
+    fn forward(
+        &self,
+        xs: &Tensor,
+        scalings: Option<Tensor>,
+        global_scaling_weight: f64,
+        is_scaling_pass: Option<f64>,
+    ) -> Result<Tensor> {
+        let (b_size, seq_len, hidden_dim) = xs.dims3()?;
+        let xs = xs.reshape(((), hidden_dim))?;
+
+        let original_dtype = xs.dtype();
+        let mut xs = xs.clone();
+        if self.gate.is_quant() {
+            xs = xs.to_dtype(DType::F32)?;
+        }
+        let mut router_logits = self.gate.lora_forward(
+            &xs,
+            scalings.clone(),
+            global_scaling_weight,
+            is_scaling_pass,
+        )?;
+        if self.gate.is_quant() {
+            router_logits = router_logits.to_dtype(original_dtype)?;
+        }
+
+        let routing_weights = candle_nn::ops::softmax_last_dim(&router_logits)?;
+
+        // In order to extract topk, we extract the data from the tensor and manipulate it
+        // directly. Maybe we will want to use some custom ops instead at some point.
+        let routing_weights = routing_weights.to_dtype(DType::F32)?.to_vec2::<f32>()?;
+
+        // routing_weights, selected_experts = torch.topk(routing_weights, self.top_k, dim=-1)
+        // top_x contains the row indexes to evaluate for each expert.
+        let mut top_x = vec![vec![]; self.experts.len()];
+        let mut selected_rws = vec![vec![]; self.experts.len()];
+        for (row_idx, rw) in routing_weights.iter().enumerate() {
+            let mut dst = (0..rw.len() as u32).collect::<Vec<u32>>();
+            dst.sort_by(|&i, &j| rw[j as usize].total_cmp(&rw[i as usize]));
+            let mut sum_routing_weights = 0f32;
+            for &expert_idx in dst.iter().take(self.num_experts_per_tok) {
+                let expert_idx = expert_idx as usize;
+                let routing_weight = rw[expert_idx];
+                sum_routing_weights += routing_weight;
+                top_x[expert_idx].push(row_idx as u32);
+            }
+            for &expert_idx in dst.iter().take(self.num_experts_per_tok) {
+                let expert_idx = expert_idx as usize;
+                let routing_weight = rw[expert_idx];
+                selected_rws[expert_idx].push(routing_weight / sum_routing_weights)
+            }
+        }
+
+        // routing_weights /= routing_weights.sum(dim=-1, keepdim=True)
+        // expert_mask = torch.nn.functional.one_hot(selected_experts, num_classes=self.num_experts).permute(2, 1, 0)
+
+        let mut ys = xs.zeros_like()?;
+        for (expert_idx, expert_layer) in self.experts.iter().enumerate() {
+            let top_x = &top_x[expert_idx];
+            if top_x.is_empty() {
+                continue;
+            }
+            let top_x = Tensor::new(top_x.as_slice(), xs.device())?;
+            let selected_rws =
+                Tensor::new(selected_rws[expert_idx].as_slice(), xs.device())?.reshape(((), 1))?;
+            // Index the correct hidden states and compute the expert hidden state for
+            // the current expert. We need to make sure to multiply the output hidden
+            // states by `routing_weights` on the corresponding tokens (top-1 and top-2)
+            let current_state = xs.index_select(&top_x, 0)?.reshape(((), hidden_dim))?;
+            // current_hidden_states = expert_layer(current_state, routing_weights[top_x_list, idx_list, None])
+            let current_hidden_states = expert_layer.forward(
+                &current_state,
+                scalings.clone(),
+                global_scaling_weight,
+                is_scaling_pass,
+            )?;
+            let current_hidden_states = current_hidden_states.broadcast_mul(&selected_rws)?;
+            ys = ys.index_add(&top_x, &current_hidden_states, 0)?;
+        }
+
+        let ys = ys.reshape((b_size, seq_len, hidden_dim))?;
+        Ok(ys)
+    }
+}
+
+#[derive(Debug, Clone)]
 struct DecoderLayer {
     self_attn: Attention,
-    mlp: MLP,
+    block_sparse_moe: SparseMoeBlock,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
     #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let self_attn = Attention::new(
             rotary_emb,
             cfg,
             vb.pp("self_attn"),
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
+            preload_adapters,
         )?;
-        let mlp = MLP::new(
+        let block_sparse_moe = SparseMoeBlock::new(
             cfg,
-            vb.pp("mlp"),
+            vb.pp("block_sparse_moe"),
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
+            preload_adapters,
         )?;
         let input_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
         )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
-            mlp,
+            block_sparse_moe,
             input_layernorm,
             post_attention_layernorm,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
-        &self,
+        &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
@@ -420,53 +569,54 @@
             kv_cache,
             scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
         let xs = (xs + residual)?;
         let residual = &xs;
-        let xs = self.mlp.forward(
+        let xs = self.block_sparse_moe.forward(
             &xs.apply(&self.post_attention_layernorm)?,
-            scalings,
+            scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
         residual + xs
     }
 }
 
 pub struct XLoraModel {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
-    lm_head: QLinear,
-    sliding_window: Option<usize>,
-    dtype: DType,
+    lm_head: QMatMul,
+    sliding_window: usize,
     pub device: Device,
     pub cache: Cache,
+    dtype: DType,
     pub max_seq_len: usize,
     xlora_classifier: Option<XLoraClassifier>,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl XLoraModel {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         real_device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
-        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
         let vb_m = vb.pp("model");
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
         let embed_tokens = candle_nn::embedding(
             cfg.vocab_size,
             cfg.hidden_size,
             mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
         )?;
         let head_dim = cfg.hidden_size / cfg.num_attention_heads;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
@@ -487,18 +637,19 @@
                 vb_l.pp(layer_idx),
                 lora_config,
                 &mut count,
                 &xlora_ordering,
                 &*mapper,
                 layer_idx,
                 loading_isq,
+                preload_adapters,
             )?;
             layers.push(layer)
         }
-        if xlora_config.is_none() {
+        if xlora_config.is_none() && preload_adapters.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
                 Arc::get_mut(&mut layer.self_attn.k_proj)
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.self_attn.o_proj)
@@ -507,23 +658,22 @@
                 Arc::get_mut(&mut layer.self_attn.q_proj)
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.self_attn.v_proj)
                     .unwrap()
                     .merge_weights()?;
 
-                Arc::get_mut(&mut layer.mlp.down_proj)
-                    .unwrap()
-                    .merge_weights()?;
-                Arc::get_mut(&mut layer.mlp.gate_proj)
-                    .unwrap()
-                    .merge_weights()?;
-                Arc::get_mut(&mut layer.mlp.up_proj)
+                Arc::get_mut(&mut layer.block_sparse_moe.gate)
                     .unwrap()
                     .merge_weights()?;
+                for expert in layer.block_sparse_moe.experts.iter_mut() {
+                    Arc::get_mut(&mut expert.w1).unwrap().merge_weights()?;
+                    Arc::get_mut(&mut expert.w2).unwrap().merge_weights()?;
+                    Arc::get_mut(&mut expert.w3).unwrap().merge_weights()?;
+                }
             }
         }
         let norm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_nm_device(vb_m.pp("norm"), false),
         )?;
@@ -532,115 +682,58 @@
             cfg.vocab_size,
             mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
         )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
-            lm_head: QLinear::from_linear(lm_head),
+            lm_head: QMatMul::Tensor(lm_head.weight().clone()),
             sliding_window: cfg.sliding_window,
             device: real_device,
             dtype: vb.dtype(),
-            cache: Cache::new(cfg.num_hidden_layers, true),
+            cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
             mapper,
         })
     }
 
-    fn prepare_decoder_attention_mask(
-        &self,
-        b_size: usize,
-        tgt_len: usize,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        // Sliding window mask
-        let sliding_window = self.sliding_window.unwrap_or(tgt_len + 1);
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| {
-                (0..tgt_len).map(move |j| {
-                    if i < j || j + sliding_window < i {
-                        f32::NEG_INFINITY
-                    } else {
-                        0.
-                    }
-                })
-            })
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
-    fn calculate_past_kv_len(
-        &self,
-        seq_len: usize,
-        kv_cache_1: &Option<(Tensor, Tensor)>,
-    ) -> Result<usize> {
-        if kv_cache_1.is_none() {
-            return Ok(0);
-        }
-        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
-        if k_cache_1.dims()[0] <= seq_len {
-            Ok(0)
-        } else {
-            let indexed = k_cache_1.i(seq_len)?;
-            let dims = indexed.dims();
-            Ok(dims[dims.len() - 2])
-        }
-    }
-
     #[allow(clippy::too_many_arguments)]
     fn inner_forward(
-        &self,
+        &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Option<Tensor>,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
-        let (b_size, seq_len) = input_ids.dims2()?;
-        if seqlen_offsets.len() > b_size {
-            candle_core::bail!("Expected seqlen offsets have length equal to batch size.")
-        }
-
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
                 self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
-        let past_key_values_length =
-            self.calculate_past_kv_len(seq_len, cache.first().as_ref().unwrap())?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask =
-                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
-            Some(mask)
-        };
+        let attention_mask = CausalMasker.make_causal_mask_with_sliding_window(
+            input_ids,
+            &cache,
+            Some(self.sliding_window),
+        )?;
         let mut xs = self.embed_tokens.forward(input_ids)?;
-        for (i, layer) in self.layers.iter().enumerate() {
+        for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
@@ -693,15 +786,15 @@
                         start_offsets_kernel_full,
                         Some(scalings),
                         true,
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
-                if self.lm_head.is_quant() {
+                if matches!(self.lm_head, QMatMul::QTensor(_)) {
                     res = res.to_dtype(DType::F32)?;
                 }
                 extract_logits(&res.apply(&self.lm_head)?, context_lens)
             } else {
                 // is_full_pass=true is ok because no_kv_cache=false
                 let mut res = self
                     .inner_forward(
@@ -710,15 +803,15 @@
                         start_offsets_kernel,
                         Some(scalings),
                         true,
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
-                if self.lm_head.is_quant() {
+                if matches!(self.lm_head, QMatMul::QTensor(_)) {
                     res = res.to_dtype(DType::F32)?;
                 }
                 extract_logits(&res.apply(&self.lm_head)?, context_lens)
             }
         } else {
             let mut res = self
                 .inner_forward(
@@ -727,15 +820,15 @@
                     start_offsets_kernel,
                     None,
                     false,
                     no_kv_cache,
                     None,
                 )?
                 .contiguous()?;
-            if self.lm_head.is_quant() {
+            if matches!(self.lm_head, QMatMul::QTensor(_)) {
                 res = res.to_dtype(DType::F32)?;
             }
             extract_logits(&res.apply(&self.lm_head)?, context_lens)
         }
     }
 }
 
@@ -785,15 +878,15 @@
         true
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
     fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push((self.lm_head.inner(), None));
+        tensors.push((&mut self.lm_head, None));
         for (i, layer) in self.layers.iter_mut().enumerate() {
             tensors.push((
                 Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner(),
                 Some(i),
             ));
             tensors.push((
                 Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner(),
@@ -804,28 +897,60 @@
                 Some(i),
             ));
             tensors.push((
                 Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner(),
                 Some(i),
             ));
             tensors.push((
-                Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner(),
-                Some(i),
-            ));
-            tensors.push((
-                Arc::get_mut(&mut layer.mlp.gate_proj).unwrap().inner(),
-                Some(i),
-            ));
-            tensors.push((
-                Arc::get_mut(&mut layer.mlp.up_proj).unwrap().inner(),
+                Arc::get_mut(&mut layer.block_sparse_moe.gate)
+                    .unwrap()
+                    .inner(),
                 Some(i),
             ));
+            for expert in &mut layer.block_sparse_moe.experts {
+                tensors.push((Arc::get_mut(&mut expert.w1).unwrap().inner(), Some(i)));
+                tensors.push((Arc::get_mut(&mut expert.w2).unwrap().inner(), Some(i)));
+                tensors.push((Arc::get_mut(&mut expert.w3).unwrap().inner(), Some(i)));
+            }
         }
         (tensors, &*self.mapper)
     }
+    fn activate_adapters(&mut self, adapter_names: Vec<String>) -> Result<usize> {
+        let mut sum = 0;
+        for layer in self.layers.iter_mut() {
+            sum += Arc::get_mut(&mut layer.self_attn.k_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.o_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.q_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.v_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+
+            sum += Arc::get_mut(&mut layer.block_sparse_moe.gate)
+                .unwrap()
+                .activate(&adapter_names)?;
+            for expert in &mut layer.block_sparse_moe.experts {
+                sum += Arc::get_mut(&mut expert.w1)
+                    .unwrap()
+                    .activate(&adapter_names)?;
+                sum += Arc::get_mut(&mut expert.w2)
+                    .unwrap()
+                    .activate(&adapter_names)?;
+                sum += Arc::get_mut(&mut expert.w3)
+                    .unwrap()
+                    .activate(&adapter_names)?;
+            }
+        }
+        Ok(sum)
+    }
 }
 
 impl ScalingsMaker for XLoraModel {
     fn dtype(&self) -> DType {
         self.dtype
     }
     fn get_cache(&self) -> &Cache {
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/xlora_models/mixtral.rs` & `mistralrs-0.1.5/mistralrs-core/src/xlora_models/mistral.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,223 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-/// Mixtral Model
-/// https://github.com/huggingface/transformers/blob/main/src/transformers/models/mixtral/modeling_mixtral.py
-/// https://mistral.ai/news/mixtral-of-experts/
-use candle_core::{quantized::QMatMul, DType, Device, IndexOp, Module, Result, Tensor, D};
+/// Mistral LLM, https://github.com/mistralai/mistral-src
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
 use candle_nn::{Activation, RotaryEmbedding, VarBuilder};
-use mistralrs_lora::{linear_no_bias, LinearLayerLike, LoraConfig, Ordering};
-use std::sync::Arc;
+use mistralrs_lora::{layer::QLinear, linear_no_bias, LinearLayerLike, LoraConfig, Ordering};
+use std::{collections::HashMap, sync::Arc};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::RmsNorm,
-    models::{flash_attn, mixtral::Config, repeat_kv, Cache},
+    layers::{CausalMasker, RmsNorm},
+    models::{flash_attn, mistral::Config, repeat_kv, Cache},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
+use super::{classifier::XLoraClassifier, config::XLoraConfig, NonGranularState, ScalingsMaker};
+
+#[derive(Debug, Clone)]
+#[allow(clippy::upper_case_acronyms)]
+struct MLP {
+    gate_proj: Arc<dyn LinearLayerLike + Send + Sync>,
+    up_proj: Arc<dyn LinearLayerLike + Send + Sync>,
+    down_proj: Arc<dyn LinearLayerLike + Send + Sync>,
+    act_fn: Activation,
+}
+
+impl MLP {
+    #[allow(clippy::too_many_arguments)]
+    fn new(
+        cfg: &Config,
+        vb: VarBuilder,
+        lora_config: &[((String, String), LoraConfig)],
+        count: &mut usize,
+        ord: &Ordering,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
+    ) -> Result<Self> {
+        let hidden_sz = cfg.hidden_size;
+        let intermediate_sz = cfg.intermediate_size;
+        let gate_proj = linear_no_bias(
+            hidden_sz,
+            intermediate_sz,
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )?;
+        let up_proj = linear_no_bias(
+            hidden_sz,
+            intermediate_sz,
+            mapper.set_device(layer_idx, vb.pp("up_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("up_proj"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )?;
+        let down_proj = linear_no_bias(
+            intermediate_sz,
+            hidden_sz,
+            mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )?;
+        Ok(Self {
+            gate_proj,
+            up_proj,
+            down_proj,
+            act_fn: cfg.hidden_act,
+        })
+    }
+
+    fn forward(
+        &self,
+        xs: &Tensor,
+        scalings: Option<Tensor>,
+        global_scaling_weight: f64,
+        is_scaling_pass: Option<f64>,
+    ) -> Result<Tensor> {
+        let original_dtype = xs.dtype();
+        let mut xs = xs.clone();
+        if self.gate_proj.is_quant() {
+            xs = xs.to_dtype(DType::F32)?;
+        }
+        let lhs = self
+            .gate_proj
+            .lora_forward(
+                &xs,
+                scalings.clone(),
+                global_scaling_weight,
+                is_scaling_pass,
+            )?
+            .apply(&self.act_fn)?;
+        let rhs = self.up_proj.lora_forward(
+            &xs,
+            scalings.clone(),
+            global_scaling_weight,
+            is_scaling_pass,
+        )?;
+        let mut res = self.down_proj.lora_forward(
+            &(lhs * rhs)?,
+            scalings,
+            global_scaling_weight,
+            is_scaling_pass,
+        )?;
+        if self.gate_proj.is_quant() {
+            res = res.to_dtype(original_dtype)?;
+        }
+        Ok(res)
+    }
+}
 
 #[derive(Debug, Clone)]
 struct Attention {
     q_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     k_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     v_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
     rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
     sliding_window: Option<usize>,
+    neg_inf: Tensor,
 }
 
 impl Attention {
     #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
         let num_kv_groups = num_heads / num_kv_heads;
         let head_dim = hidden_sz / num_heads;
         let q_proj = linear_no_bias(
             hidden_sz,
             num_heads * head_dim,
             mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("q_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let k_proj = linear_no_bias(
             hidden_sz,
             num_kv_heads * head_dim,
             mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("k_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let v_proj = linear_no_bias(
             hidden_sz,
             num_kv_heads * head_dim,
             mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("v_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let o_proj = linear_no_bias(
             num_heads * head_dim,
             hidden_sz,
             mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("o_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         Ok(Self {
             q_proj,
             k_proj,
             v_proj,
             o_proj,
             num_heads,
             num_kv_heads,
             num_kv_groups,
             head_dim,
             rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
-            sliding_window: Some(cfg.sliding_window),
+            sliding_window: cfg.sliding_window,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
-        &mut self,
+        &self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
@@ -215,18 +322,15 @@
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
             let scale = 1f64 / f64::sqrt(self.head_dim as f64);
             let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
 
-            let attn_weights = match attn_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(&mask)?,
-            };
+            let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = self.o_proj.lora_forward(
@@ -239,307 +343,79 @@
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
-struct BlockSparseTop2MLP {
-    w1: Arc<dyn LinearLayerLike + Send + Sync>,
-    w2: Arc<dyn LinearLayerLike + Send + Sync>,
-    w3: Arc<dyn LinearLayerLike + Send + Sync>,
-    act_fn: Activation,
-}
-
-impl BlockSparseTop2MLP {
-    #[allow(clippy::too_many_arguments)]
-    fn new(
-        cfg: &Config,
-        vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
-        count: &mut usize,
-        ord: &Ordering,
-        mapper: &dyn DeviceMapper,
-        layer_idx: usize,
-        loading_isq: bool,
-    ) -> Result<Self> {
-        let hidden_sz = cfg.hidden_size;
-        let intermediate_sz = cfg.intermediate_size;
-        let w1 = linear_no_bias(
-            hidden_sz,
-            intermediate_sz,
-            mapper.set_device(layer_idx, vb.pp("w1"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("w1"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        let w2 = linear_no_bias(
-            intermediate_sz,
-            hidden_sz,
-            mapper.set_device(layer_idx, vb.pp("w2"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("w2"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        let w3 = linear_no_bias(
-            hidden_sz,
-            intermediate_sz,
-            mapper.set_device(layer_idx, vb.pp("w3"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("w3"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        Ok(Self {
-            w1,
-            w2,
-            w3,
-            act_fn: cfg.hidden_act,
-        })
-    }
-
-    fn forward(
-        &self,
-        xs: &Tensor,
-        scalings: Option<Tensor>,
-        global_scaling_weight: f64,
-        is_scaling_pass: Option<f64>,
-    ) -> Result<Tensor> {
-        let original_dtype = xs.dtype();
-        let mut xs = xs.clone();
-        if self.w1.is_quant() {
-            xs = xs.to_dtype(DType::F32)?;
-        }
-        let lhs = self
-            .w1
-            .lora_forward(
-                &xs,
-                scalings.clone(),
-                global_scaling_weight,
-                is_scaling_pass,
-            )?
-            .apply(&self.act_fn)?;
-        let rhs = self.w3.lora_forward(
-            &xs,
-            scalings.clone(),
-            global_scaling_weight,
-            is_scaling_pass,
-        )?;
-        let mut res = self.w2.lora_forward(
-            &(lhs * rhs)?,
-            scalings.clone(),
-            global_scaling_weight,
-            is_scaling_pass,
-        )?;
-        if self.w1.is_quant() {
-            res = res.to_dtype(original_dtype)?;
-        }
-        Ok(res)
-    }
-}
-
-#[derive(Debug, Clone)]
-struct SparseMoeBlock {
-    gate: Arc<dyn LinearLayerLike + Send + Sync>,
-    experts: Vec<BlockSparseTop2MLP>,
-    num_experts_per_tok: usize,
-}
-
-impl SparseMoeBlock {
-    #[allow(clippy::too_many_arguments)]
-    fn new(
-        cfg: &Config,
-        vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
-        count: &mut usize,
-        ord: &Ordering,
-        mapper: &dyn DeviceMapper,
-        layer_idx: usize,
-        loading_isq: bool,
-    ) -> Result<Self> {
-        let gate = linear_no_bias(
-            cfg.hidden_size,
-            cfg.num_local_experts,
-            mapper.set_device(layer_idx, vb.pp("gate"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("gate"), false),
-            lora_config,
-            count,
-            ord,
-        )?;
-        let mut experts = Vec::with_capacity(cfg.num_local_experts);
-        let vb = vb.pp("experts");
-        for idx in 0..cfg.num_local_experts {
-            let expert = BlockSparseTop2MLP::new(
-                cfg,
-                vb.pp(idx),
-                lora_config,
-                count,
-                ord,
-                mapper,
-                layer_idx,
-                loading_isq,
-            )?;
-            experts.push(expert)
-        }
-        Ok(SparseMoeBlock {
-            gate,
-            experts,
-            num_experts_per_tok: cfg.num_experts_per_tok,
-        })
-    }
-
-    fn forward(
-        &self,
-        xs: &Tensor,
-        scalings: Option<Tensor>,
-        global_scaling_weight: f64,
-        is_scaling_pass: Option<f64>,
-    ) -> Result<Tensor> {
-        let (b_size, seq_len, hidden_dim) = xs.dims3()?;
-        let xs = xs.reshape(((), hidden_dim))?;
-
-        let original_dtype = xs.dtype();
-        let mut xs = xs.clone();
-        if self.gate.is_quant() {
-            xs = xs.to_dtype(DType::F32)?;
-        }
-        let mut router_logits = self.gate.lora_forward(
-            &xs,
-            scalings.clone(),
-            global_scaling_weight,
-            is_scaling_pass,
-        )?;
-        if self.gate.is_quant() {
-            router_logits = router_logits.to_dtype(original_dtype)?;
-        }
-
-        let routing_weights = candle_nn::ops::softmax_last_dim(&router_logits)?;
-
-        // In order to extract topk, we extract the data from the tensor and manipulate it
-        // directly. Maybe we will want to use some custom ops instead at some point.
-        let routing_weights = routing_weights.to_dtype(DType::F32)?.to_vec2::<f32>()?;
-
-        // routing_weights, selected_experts = torch.topk(routing_weights, self.top_k, dim=-1)
-        // top_x contains the row indexes to evaluate for each expert.
-        let mut top_x = vec![vec![]; self.experts.len()];
-        let mut selected_rws = vec![vec![]; self.experts.len()];
-        for (row_idx, rw) in routing_weights.iter().enumerate() {
-            let mut dst = (0..rw.len() as u32).collect::<Vec<u32>>();
-            dst.sort_by(|&i, &j| rw[j as usize].total_cmp(&rw[i as usize]));
-            let mut sum_routing_weights = 0f32;
-            for &expert_idx in dst.iter().take(self.num_experts_per_tok) {
-                let expert_idx = expert_idx as usize;
-                let routing_weight = rw[expert_idx];
-                sum_routing_weights += routing_weight;
-                top_x[expert_idx].push(row_idx as u32);
-            }
-            for &expert_idx in dst.iter().take(self.num_experts_per_tok) {
-                let expert_idx = expert_idx as usize;
-                let routing_weight = rw[expert_idx];
-                selected_rws[expert_idx].push(routing_weight / sum_routing_weights)
-            }
-        }
-
-        // routing_weights /= routing_weights.sum(dim=-1, keepdim=True)
-        // expert_mask = torch.nn.functional.one_hot(selected_experts, num_classes=self.num_experts).permute(2, 1, 0)
-
-        let mut ys = xs.zeros_like()?;
-        for (expert_idx, expert_layer) in self.experts.iter().enumerate() {
-            let top_x = &top_x[expert_idx];
-            if top_x.is_empty() {
-                continue;
-            }
-            let top_x = Tensor::new(top_x.as_slice(), xs.device())?;
-            let selected_rws =
-                Tensor::new(selected_rws[expert_idx].as_slice(), xs.device())?.reshape(((), 1))?;
-            // Index the correct hidden states and compute the expert hidden state for
-            // the current expert. We need to make sure to multiply the output hidden
-            // states by `routing_weights` on the corresponding tokens (top-1 and top-2)
-            let current_state = xs.index_select(&top_x, 0)?.reshape(((), hidden_dim))?;
-            // current_hidden_states = expert_layer(current_state, routing_weights[top_x_list, idx_list, None])
-            let current_hidden_states = expert_layer.forward(
-                &current_state,
-                scalings.clone(),
-                global_scaling_weight,
-                is_scaling_pass,
-            )?;
-            let current_hidden_states = current_hidden_states.broadcast_mul(&selected_rws)?;
-            ys = ys.index_add(&top_x, &current_hidden_states, 0)?;
-        }
-
-        let ys = ys.reshape((b_size, seq_len, hidden_dim))?;
-        Ok(ys)
-    }
-}
-
-#[derive(Debug, Clone)]
 struct DecoderLayer {
     self_attn: Attention,
-    block_sparse_moe: SparseMoeBlock,
+    mlp: MLP,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
     #[allow(clippy::too_many_arguments)]
     fn new(
         rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let self_attn = Attention::new(
             rotary_emb,
             cfg,
             vb.pp("self_attn"),
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
+            preload_adapters,
         )?;
-        let block_sparse_moe = SparseMoeBlock::new(
+        let mlp = MLP::new(
             cfg,
-            vb.pp("block_sparse_moe"),
+            vb.pp("mlp"),
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
+            preload_adapters,
         )?;
         let input_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
         )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
         )?;
         Ok(Self {
             self_attn,
-            block_sparse_moe,
+            mlp,
             input_layernorm,
             post_attention_layernorm,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
-        &mut self,
+        &self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
@@ -555,53 +431,54 @@
             kv_cache,
             scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
         let xs = (xs + residual)?;
         let residual = &xs;
-        let xs = self.block_sparse_moe.forward(
+        let xs = self.mlp.forward(
             &xs.apply(&self.post_attention_layernorm)?,
-            scalings.clone(),
+            scalings,
             global_scaling_weight,
             is_scaling_pass,
         )?;
         residual + xs
     }
 }
 
 pub struct XLoraModel {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
-    lm_head: QMatMul,
-    sliding_window: usize,
+    lm_head: QLinear,
+    sliding_window: Option<usize>,
+    dtype: DType,
     pub device: Device,
     pub cache: Cache,
-    dtype: DType,
     pub max_seq_len: usize,
     xlora_classifier: Option<XLoraClassifier>,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl XLoraModel {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         real_device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
-        let vb_m = vb.pp("model");
         let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let vb_m = vb.pp("model");
         let embed_tokens = candle_nn::embedding(
             cfg.vocab_size,
             cfg.hidden_size,
             mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
         )?;
         let head_dim = cfg.hidden_size / cfg.num_attention_heads;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
@@ -622,18 +499,19 @@
                 vb_l.pp(layer_idx),
                 lora_config,
                 &mut count,
                 &xlora_ordering,
                 &*mapper,
                 layer_idx,
                 loading_isq,
+                preload_adapters,
             )?;
             layers.push(layer)
         }
-        if xlora_config.is_none() {
+        if xlora_config.is_none() && preload_adapters.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
                 Arc::get_mut(&mut layer.self_attn.k_proj)
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.self_attn.o_proj)
@@ -642,22 +520,23 @@
                 Arc::get_mut(&mut layer.self_attn.q_proj)
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.self_attn.v_proj)
                     .unwrap()
                     .merge_weights()?;
 
-                Arc::get_mut(&mut layer.block_sparse_moe.gate)
+                Arc::get_mut(&mut layer.mlp.down_proj)
+                    .unwrap()
+                    .merge_weights()?;
+                Arc::get_mut(&mut layer.mlp.gate_proj)
+                    .unwrap()
+                    .merge_weights()?;
+                Arc::get_mut(&mut layer.mlp.up_proj)
                     .unwrap()
                     .merge_weights()?;
-                for expert in layer.block_sparse_moe.experts.iter_mut() {
-                    Arc::get_mut(&mut expert.w1).unwrap().merge_weights()?;
-                    Arc::get_mut(&mut expert.w2).unwrap().merge_weights()?;
-                    Arc::get_mut(&mut expert.w3).unwrap().merge_weights()?;
-                }
             }
         }
         let norm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_nm_device(vb_m.pp("norm"), false),
         )?;
@@ -666,107 +545,58 @@
             cfg.vocab_size,
             mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
         )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
-            lm_head: QMatMul::Tensor(lm_head.weight().clone()),
+            lm_head: QLinear::from_linear(lm_head),
             sliding_window: cfg.sliding_window,
             device: real_device,
             dtype: vb.dtype(),
-            cache: Cache::new(cfg.num_hidden_layers, false),
+            cache: Cache::new(cfg.num_hidden_layers, true),
             max_seq_len: cfg.max_position_embeddings,
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
             mapper,
         })
     }
 
-    fn calculate_past_kv_len(&mut self, seq_len: usize) -> Result<usize> {
-        let cache = self.cache.lock();
-        let kv_cache_1 = cache.first().unwrap();
-        if kv_cache_1.is_none() {
-            return Ok(0);
-        }
-        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
-        if k_cache_1.dims()[0] <= seq_len {
-            Ok(0)
-        } else {
-            let indexed = k_cache_1.i(seq_len)?;
-            let dims = indexed.dims();
-            Ok(dims[dims.len() - 2])
-        }
-    }
-
-    fn prepare_decoder_attention_mask(
-        &self,
-        b_size: usize,
-        tgt_len: usize,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        // Sliding window mask?
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| {
-                (0..tgt_len).map(move |j| {
-                    if i < j || j + self.sliding_window < i {
-                        f32::NEG_INFINITY
-                    } else {
-                        0.
-                    }
-                })
-            })
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
     #[allow(clippy::too_many_arguments)]
     fn inner_forward(
-        &mut self,
+        &self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Option<Tensor>,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
-        let (b_size, seq_len) = input_ids.dims2()?;
-        let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask =
-                self.prepare_decoder_attention_mask(b_size, seq_len, past_key_values_length)?;
-            Some(mask)
-        };
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
                 self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
+        let attention_mask = CausalMasker.make_causal_mask_with_sliding_window(
+            input_ids,
+            &cache,
+            self.sliding_window,
+        )?;
         let mut xs = self.embed_tokens.forward(input_ids)?;
-        for (i, layer) in self.layers.iter_mut().enumerate() {
+        for (i, layer) in self.layers.iter().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
@@ -819,15 +649,15 @@
                         start_offsets_kernel_full,
                         Some(scalings),
                         true,
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
-                if matches!(self.lm_head, QMatMul::QTensor(_)) {
+                if self.lm_head.is_quant() {
                     res = res.to_dtype(DType::F32)?;
                 }
                 extract_logits(&res.apply(&self.lm_head)?, context_lens)
             } else {
                 // is_full_pass=true is ok because no_kv_cache=false
                 let mut res = self
                     .inner_forward(
@@ -836,15 +666,15 @@
                         start_offsets_kernel,
                         Some(scalings),
                         true,
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
-                if matches!(self.lm_head, QMatMul::QTensor(_)) {
+                if self.lm_head.is_quant() {
                     res = res.to_dtype(DType::F32)?;
                 }
                 extract_logits(&res.apply(&self.lm_head)?, context_lens)
             }
         } else {
             let mut res = self
                 .inner_forward(
@@ -853,15 +683,15 @@
                     start_offsets_kernel,
                     None,
                     false,
                     no_kv_cache,
                     None,
                 )?
                 .contiguous()?;
-            if matches!(self.lm_head, QMatMul::QTensor(_)) {
+            if self.lm_head.is_quant() {
                 res = res.to_dtype(DType::F32)?;
             }
             extract_logits(&res.apply(&self.lm_head)?, context_lens)
         }
     }
 }
 
@@ -911,15 +741,15 @@
         true
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
     fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
-        tensors.push((&mut self.lm_head, None));
+        tensors.push((self.lm_head.inner(), None));
         for (i, layer) in self.layers.iter_mut().enumerate() {
             tensors.push((
                 Arc::get_mut(&mut layer.self_attn.q_proj).unwrap().inner(),
                 Some(i),
             ));
             tensors.push((
                 Arc::get_mut(&mut layer.self_attn.k_proj).unwrap().inner(),
@@ -930,27 +760,56 @@
                 Some(i),
             ));
             tensors.push((
                 Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner(),
                 Some(i),
             ));
             tensors.push((
-                Arc::get_mut(&mut layer.block_sparse_moe.gate)
-                    .unwrap()
-                    .inner(),
+                Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.gate_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.up_proj).unwrap().inner(),
                 Some(i),
             ));
-            for expert in &mut layer.block_sparse_moe.experts {
-                tensors.push((Arc::get_mut(&mut expert.w1).unwrap().inner(), Some(i)));
-                tensors.push((Arc::get_mut(&mut expert.w2).unwrap().inner(), Some(i)));
-                tensors.push((Arc::get_mut(&mut expert.w3).unwrap().inner(), Some(i)));
-            }
         }
         (tensors, &*self.mapper)
     }
+    fn activate_adapters(&mut self, adapter_names: Vec<String>) -> Result<usize> {
+        let mut sum = 0;
+        for layer in self.layers.iter_mut() {
+            sum += Arc::get_mut(&mut layer.self_attn.k_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.o_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.q_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.v_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+
+            sum += Arc::get_mut(&mut layer.mlp.down_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.mlp.gate_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.mlp.up_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+        }
+        Ok(sum)
+    }
 }
 
 impl ScalingsMaker for XLoraModel {
     fn dtype(&self) -> DType {
         self.dtype
     }
     fn get_cache(&self) -> &Cache {
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/xlora_models/mod.rs` & `mistralrs-0.1.5/mistralrs-core/src/xlora_models/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 mod gemma;
 mod llama;
 mod mistral;
 mod mixtral;
 mod phi2;
 mod phi3;
 mod quantized_llama;
+mod quantized_phi3;
 
 use std::sync::Arc;
 
 use candle_core::{DType, Device, Result, Tensor};
 pub use config::XLoraConfig;
 pub use gemma::XLoraModel as XLoraGemma;
 pub use llama::XLoraLlama;
 pub use mistral::XLoraModel as XLoraMistral;
 use mistralrs_lora::Ordering;
 pub use mixtral::XLoraModel as XLoraMixtral;
 pub use phi2::Model as XLoraPhi2;
 pub use phi3::Model as XLoraPhi3;
-pub use quantized_llama::ModelWeights as XLoraModelWeights;
+pub use quantized_llama::ModelWeights as XLoraQLlama;
+pub use quantized_phi3::ModelWeights as XLoraQPhi3;
 use tokio::sync::Mutex;
 
 use crate::{get_mut_arcmutex, models::Cache};
 
 use self::classifier::XLoraClassifier;
 
 pub struct NonGranularState {
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/xlora_models/phi2.rs` & `mistralrs-0.1.5/mistralrs-core/src/xlora_models/gemma.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,232 +1,274 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-use std::sync::Arc;
+use std::{collections::HashMap, sync::Arc};
 
-/// Phi model.
-/// https://huggingface.co/microsoft/phi-2
-/// There is an alternative implementation of the phi model in mixformers.rs.
-/// This corresponds to the model update made with the following commit:
-/// https://huggingface.co/microsoft/phi-2/commit/cb2f4533604d8b67de604e7df03bfe6f3ca22869
-use candle_core::{quantized::QMatMul, DType, Device, Result, Tensor};
-use candle_nn::{
-    embedding, layer_norm, Activation, Embedding, LayerNorm, RotaryEmbedding, VarBuilder,
-};
-use mistralrs_lora::{layer::QLinear, linear, LinearLayerLike, LoraConfig, Ordering};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
+use candle_nn::{RotaryEmbedding, VarBuilder};
+use mistralrs_lora::{layer::QLinear, linear_b as linear, LinearLayerLike, LoraConfig, Ordering};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    models::{flash_attn, phi2::Config, repeat_kv},
+    layers::CausalMasker,
+    models::{flash_attn, gemma::Config, repeat_kv, Cache},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{classifier::XLoraClassifier, Cache, NonGranularState, ScalingsMaker, XLoraConfig};
+use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
+
+fn default_max_position_embeddings() -> usize {
+    4096
+}
+
+#[derive(Debug, Clone)]
+struct RmsNorm {
+    weight: Tensor,
+    eps: f64,
+}
+
+impl RmsNorm {
+    fn new(dim: usize, eps: f64, vb: VarBuilder) -> Result<Self> {
+        let weight = vb.get(dim, "weight")?;
+        Ok(Self { weight, eps })
+    }
+}
+
+impl Module for RmsNorm {
+    fn forward(&self, x: &Tensor) -> Result<Tensor> {
+        let x_dtype = x.dtype();
+        let internal_dtype = match x_dtype {
+            DType::F16 | DType::BF16 => DType::F32,
+            d => d,
+        };
+        let hidden_size = x.dim(D::Minus1)?;
+        let x = x.to_dtype(internal_dtype)?;
+        let norm_x = (x.sqr()?.sum_keepdim(D::Minus1)? / hidden_size as f64)?;
+        let x_normed = x.broadcast_div(&(norm_x + self.eps)?.sqrt()?)?;
+        x_normed
+            .to_dtype(x_dtype)?
+            .broadcast_mul(&(&self.weight + 1.0)?)
+    }
+}
 
 #[derive(Debug, Clone)]
 #[allow(clippy::upper_case_acronyms)]
 struct MLP {
-    fc1: Arc<dyn LinearLayerLike + Send + Sync>,
-    fc2: Arc<dyn LinearLayerLike + Send + Sync>,
-    act: Activation,
+    gate_proj: Arc<dyn LinearLayerLike + Send + Sync>,
+    up_proj: Arc<dyn LinearLayerLike + Send + Sync>,
+    down_proj: Arc<dyn LinearLayerLike + Send + Sync>,
+    act_fn: candle_nn::Activation,
 }
 
 impl MLP {
     #[allow(clippy::too_many_arguments)]
     fn new(
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
-        let fc1 = linear(
-            cfg.hidden_size,
-            cfg.intermediate_size,
-            mapper.set_device(layer_idx, vb.pp("fc1"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("fc1"), false),
+        let hidden_sz = cfg.hidden_size;
+        let intermediate_sz = cfg.intermediate_size;
+        let gate_proj = linear(
+            hidden_sz,
+            intermediate_sz,
+            false,
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("gate_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
-        let fc2 = linear(
-            cfg.intermediate_size,
-            cfg.hidden_size,
-            mapper.set_device(layer_idx, vb.pp("fc2"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("fc2"), false),
+        let up_proj = linear(
+            hidden_sz,
+            intermediate_sz,
+            false,
+            mapper.set_device(layer_idx, vb.pp("up_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("up_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
+        )?;
+        let down_proj = linear(
+            intermediate_sz,
+            hidden_sz,
+            false,
+            mapper.set_device(layer_idx, vb.pp("down_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("down_proj"), false),
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
         )?;
         Ok(Self {
-            fc1,
-            fc2,
-            // This does not match the mixformers implementation where Gelu is used rather than
-            // GeluNew.
-            act: cfg.hidden_act,
+            gate_proj,
+            up_proj,
+            down_proj,
+            act_fn: cfg.hidden_act()?,
         })
     }
 
     fn forward(
         &self,
         xs: &Tensor,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
-        if self.fc1.is_quant() {
+        if self.gate_proj.is_quant() {
             xs = xs.to_dtype(DType::F32)?;
         }
-        let mut res = self.fc2.lora_forward(
-            &self
-                .fc1
-                .lora_forward(
-                    &xs,
-                    scalings.clone(),
-                    global_scaling_weight,
-                    is_scaling_pass,
-                )?
-                .apply(&self.act)?,
+        let lhs = self
+            .gate_proj
+            .lora_forward(
+                &xs,
+                scalings.clone(),
+                global_scaling_weight,
+                is_scaling_pass,
+            )?
+            .apply(&self.act_fn)?;
+        let rhs = self.up_proj.lora_forward(
+            &xs,
+            scalings.clone(),
+            global_scaling_weight,
+            is_scaling_pass,
+        )?;
+        let mut res = self.down_proj.lora_forward(
+            &(lhs * rhs)?,
             scalings,
             global_scaling_weight,
             is_scaling_pass,
         )?;
-        if self.fc1.is_quant() {
+        if self.gate_proj.is_quant() {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
-#[derive(Clone)]
+#[derive(Debug, Clone)]
 struct Attention {
     q_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     k_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     v_proj: Arc<dyn LinearLayerLike + Send + Sync>,
-    dense: Arc<dyn LinearLayerLike + Send + Sync>,
-    q_layernorm: Option<LayerNorm>,
-    k_layernorm: Option<LayerNorm>,
-    rotary_emb: RotaryEmbedding,
-    softmax_scale: f64,
+    o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     num_heads: usize,
     num_kv_heads: usize,
+    num_kv_groups: usize,
     head_dim: usize,
+    rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
-}
-
-fn get_mask(size: usize, device: &Device) -> Result<Tensor> {
-    let mask: Vec<_> = (0..size)
-        .flat_map(|i| (0..size).map(move |j| u8::from(j > i)))
-        .collect();
-    Tensor::from_slice(&mask, (size, size), device)
-}
-
-fn masked_fill(on_false: &Tensor, mask: &Tensor, on_true: f32) -> Result<Tensor> {
-    let shape = mask.shape();
-    let on_true = Tensor::new(on_true, on_false.device())?.broadcast_as(shape.dims())?;
-    let m = mask.where_cond(&on_true, on_false)?;
-    Ok(m)
+    neg_inf: Tensor,
 }
 
 impl Attention {
     #[allow(clippy::too_many_arguments)]
     fn new(
+        rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
-        rope: RotaryEmbedding,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
+        let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
-        let num_kv_heads = cfg.num_key_value_heads();
-        let head_dim = cfg.head_dim();
+        let num_kv_heads = cfg.num_key_value_heads;
+        let num_kv_groups = num_heads / num_kv_heads;
+        let head_dim = cfg.head_dim;
+        let bias = cfg.attention_bias;
         let q_proj = linear(
-            cfg.hidden_size,
+            hidden_sz,
             num_heads * head_dim,
+            bias,
             mapper.set_device(layer_idx, vb.pp("q_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("q_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let k_proj = linear(
-            cfg.hidden_size,
+            hidden_sz,
             num_kv_heads * head_dim,
+            bias,
             mapper.set_device(layer_idx, vb.pp("k_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("k_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
         let v_proj = linear(
-            cfg.hidden_size,
+            hidden_sz,
             num_kv_heads * head_dim,
+            bias,
             mapper.set_device(layer_idx, vb.pp("v_proj"), loading_isq),
             mapper.set_device(layer_idx, vb.pp("v_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
-        let dense = linear(
+        let o_proj = linear(
             num_heads * head_dim,
-            cfg.hidden_size,
-            mapper.set_device(layer_idx, vb.pp("dense"), loading_isq),
-            mapper.set_device(layer_idx, vb.pp("dense"), false),
+            hidden_sz,
+            bias,
+            mapper.set_device(layer_idx, vb.pp("o_proj"), loading_isq),
+            mapper.set_device(layer_idx, vb.pp("o_proj"), false),
             lora_config,
             count,
             ord,
+            preload_adapters,
         )?;
-        let (q_layernorm, k_layernorm) = if cfg.qk_layernorm {
-            let q_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("q_layernorm"))?;
-            let k_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("k_layernorm"))?;
-            (Some(q_layernorm), Some(k_layernorm))
-        } else {
-            (None, None)
-        };
-        let softmax_scale = 1f64 / (head_dim as f64).sqrt();
         Ok(Self {
             q_proj,
             k_proj,
             v_proj,
-            dense,
-            q_layernorm,
-            k_layernorm,
-            rotary_emb: rope,
-            softmax_scale,
+            o_proj,
             num_heads,
             num_kv_heads,
+            num_kv_groups,
             head_dim,
+            rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &mut self,
         xs: &Tensor,
-        mask: Option<&Tensor>,
+        attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
-        let (b_size, seq_len, _n_embd) = xs.dims3()?;
+        let (b_sz, q_len, _) = xs.dims3()?;
+
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
         if self.q_proj.is_quant() {
             xs = xs.to_dtype(DType::F32)?;
         }
         let mut q = self.q_proj.lora_forward(
             &xs,
@@ -248,347 +290,338 @@
         )?;
         if self.q_proj.is_quant() {
             q = q.to_dtype(original_dtype)?;
             k = k.to_dtype(original_dtype)?;
             v = v.to_dtype(original_dtype)?;
         }
 
-        let q = match &self.q_layernorm {
-            None => q,
-            Some(ln) => q.apply(ln)?,
-        };
-        let k = match &self.k_layernorm {
-            None => k,
-            Some(ln) => k.apply(ln)?,
-        };
-
-        let mut q = q.reshape((b_size * seq_len, self.num_heads, self.head_dim))?;
-        let mut k = k.reshape((b_size * seq_len, self.num_kv_heads, self.head_dim))?;
+        let mut q = q.reshape((b_sz * q_len, self.num_heads, self.head_dim))?;
+        let mut k = k.reshape((b_sz * q_len, self.num_kv_heads, self.head_dim))?;
         let v = v
-            .reshape((b_size, seq_len, self.num_kv_heads, self.head_dim))?
+            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
             .transpose(1, 2)?;
 
-        self.rotary_emb.forward(
-            seqlen_offsets,
-            &start_offsets_kernel,
-            &mut q,
-            &mut k,
-            b_size,
-        )?;
+        self.rotary_emb
+            .forward(seqlen_offsets, &start_offsets_kernel, &mut q, &mut k, b_sz)?;
 
         if q.rank() == 3 {
             q = q
-                .reshape((b_size, seq_len, self.num_heads, self.head_dim))?
+                .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
             k = k
-                .reshape((b_size, seq_len, self.num_kv_heads, self.head_dim))?
+                .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
         let (k, v) = match &*kv_cache {
             None => (k, v),
             Some((prev_k, prev_v)) => {
                 let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
                 let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
                 (k, v)
             }
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
-        let k = repeat_kv(k, self.num_heads / self.num_kv_heads)?.contiguous()?;
-        let v = repeat_kv(v, self.num_heads / self.num_kv_heads)?.contiguous()?;
+        let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
+        let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
-        let attn_output = if self.use_flash_attn {
+        let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
-            flash_attn(&q, &k, &v, self.softmax_scale as f32, seq_len > 1)?.transpose(1, 2)?
+            let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
+            flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
-            let attn_weights = (q
-                .to_dtype(DType::F32)?
-                .contiguous()?
-                .matmul(&k.to_dtype(DType::F32)?.t()?)?
-                * self.softmax_scale)?;
-            let attn_weights = match mask {
-                None => attn_weights,
-                Some(mask) => masked_fill(
-                    &attn_weights,
-                    &mask.broadcast_left((b_size, self.num_heads))?,
-                    f32::NEG_INFINITY,
-                )?,
-            };
+            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
+            let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
+
             let attn_weights =
-                candle_nn::ops::softmax_last_dim(&attn_weights)?.to_dtype(v.dtype())?;
+                CausalMasker.apply_mask(&attention_mask.cloned(), attn_weights, &self.neg_inf)?;
+            let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
             attn_weights.matmul(&v)?
         };
-
-        let mut attn_output = attn_output
-            .transpose(1, 2)?
-            .reshape((b_size, seq_len, ()))?;
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
-        let mut res = self.dense.lora_forward(
-            &attn_output,
-            scalings,
+        let mut res = self.o_proj.lora_forward(
+            &attn_output.transpose(1, 2)?.reshape((b_sz, q_len, ()))?,
+            scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
         if self.q_proj.is_quant() {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
-#[derive(Clone)]
+#[derive(Debug, Clone)]
 struct DecoderLayer {
     self_attn: Attention,
     mlp: MLP,
-    input_layernorm: LayerNorm,
+    input_layernorm: RmsNorm,
+    post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
     #[allow(clippy::too_many_arguments)]
     fn new(
+        rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         count: &mut usize,
         ord: &Ordering,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
-        rope: RotaryEmbedding,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let self_attn = Attention::new(
+            rotary_emb,
             cfg,
             vb.pp("self_attn"),
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
-            rope,
+            preload_adapters,
         )?;
         let mlp = MLP::new(
             cfg,
             vb.pp("mlp"),
             lora_config,
             count,
             ord,
             mapper,
             layer_idx,
             loading_isq,
+            preload_adapters,
         )?;
-        let input_layernorm = layer_norm(
+        let input_layernorm = RmsNorm::new(
             cfg.hidden_size,
-            cfg.layer_norm_eps,
+            cfg.rms_norm_eps,
             mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
         )?;
+        let post_attention_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
+        )?;
         Ok(Self {
             self_attn,
             mlp,
             input_layernorm,
+            post_attention_layernorm,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn forward(
         &mut self,
         xs: &Tensor,
-        mask: Option<&Tensor>,
+        attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
         scalings: Option<Tensor>,
         global_scaling_weight: f64,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         let residual = xs;
-        let xs = xs.apply(&self.input_layernorm)?;
-        let attn_outputs = self.self_attn.forward(
+        let xs = self.input_layernorm.forward(xs)?;
+        let xs = self.self_attn.forward(
             &xs,
-            mask,
+            attention_mask,
             seqlen_offsets,
             start_offsets_kernel,
             kv_cache,
             scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
-        let feed_forward_hidden_states =
-            self.mlp
-                .forward(&xs, scalings, global_scaling_weight, is_scaling_pass)?;
-        attn_outputs + feed_forward_hidden_states + residual
+        let xs = (xs + residual)?;
+        let residual = &xs;
+        let xs = self.mlp.forward(
+            &xs.apply(&self.post_attention_layernorm)?,
+            scalings.clone(),
+            global_scaling_weight,
+            is_scaling_pass,
+        )?;
+        residual + xs
     }
 }
 
-pub struct Model {
-    embed_tokens: Embedding,
+pub struct XLoraModel {
+    embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
-    final_layernorm: LayerNorm,
+    norm: RmsNorm,
     lm_head: QLinear,
-    pub cache: Cache,
+    dtype: DType,
+    hidden_size: usize,
     pub device: Device,
+    pub cache: Cache,
     pub max_seq_len: usize,
     xlora_classifier: Option<XLoraClassifier>,
-    dtype: DType,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
-impl Model {
+impl XLoraModel {
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         is_gptx: bool,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         real_device: Device,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
         let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
-        let embed_tokens = embedding(
+        let embed_tokens = candle_nn::embedding(
             cfg.vocab_size,
             cfg.hidden_size,
             mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
         )?;
-        let final_layernorm = layer_norm(
-            cfg.hidden_size,
-            cfg.layer_norm_eps,
-            mapper.set_nm_device(vb_m.pp("final_layernorm"), false),
-        )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
-        let vb_m = vb_m.pp("layers");
+        let vb_l = vb_m.pp("layers");
         let mut count = 0;
         for layer_idx in 0..cfg.num_hidden_layers {
-            // Alternative rope scalings are not supported.
-            let rotary_emb = RotaryEmbedding::new_partial(
-                cfg.rope_theta,
-                cfg.head_dim(),
-                (cfg.partial_rotary_factor * cfg.head_dim() as f64) as usize,
+            let rotary_emb = Arc::new(RotaryEmbedding::new(
+                cfg.rope_theta as f32,
+                cfg.head_dim,
                 cfg.max_position_embeddings,
                 mapper.device_for(layer_idx, false).unwrap_or(&real_device),
                 is_gptx,
                 vb.dtype(),
-            )?;
+            )?);
             let layer = DecoderLayer::new(
+                rotary_emb.clone(),
                 cfg,
-                vb_m.pp(layer_idx),
+                vb_l.pp(layer_idx),
                 lora_config,
                 &mut count,
                 &xlora_ordering,
                 &*mapper,
                 layer_idx,
                 loading_isq,
-                rotary_emb,
+                preload_adapters,
             )?;
             layers.push(layer)
         }
-        if xlora_config.is_none() {
+        if xlora_config.is_none() && preload_adapters.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
                 Arc::get_mut(&mut layer.self_attn.k_proj)
                     .unwrap()
                     .merge_weights()?;
-                Arc::get_mut(&mut layer.self_attn.dense)
+                Arc::get_mut(&mut layer.self_attn.o_proj)
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.self_attn.q_proj)
                     .unwrap()
                     .merge_weights()?;
                 Arc::get_mut(&mut layer.self_attn.v_proj)
                     .unwrap()
                     .merge_weights()?;
 
-                Arc::get_mut(&mut layer.mlp.fc1).unwrap().merge_weights()?;
-                Arc::get_mut(&mut layer.mlp.fc2).unwrap().merge_weights()?;
+                Arc::get_mut(&mut layer.mlp.down_proj)
+                    .unwrap()
+                    .merge_weights()?;
+                Arc::get_mut(&mut layer.mlp.gate_proj)
+                    .unwrap()
+                    .merge_weights()?;
+                Arc::get_mut(&mut layer.mlp.up_proj)
+                    .unwrap()
+                    .merge_weights()?;
             }
         }
-        let lm_head = candle_nn::linear(
+        let norm = RmsNorm::new(
             cfg.hidden_size,
-            cfg.vocab_size,
-            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
         )?;
+        let lm_head = candle_nn::Linear::new(embed_tokens.embeddings().clone(), None);
         Ok(Self {
             embed_tokens,
             layers,
-            final_layernorm,
+            norm,
             lm_head: QLinear::from_linear(lm_head),
-            cache: Cache::new(cfg.num_hidden_layers, true),
             device: real_device,
-            max_seq_len: cfg.max_position_embeddings,
             dtype: vb.dtype(),
+            hidden_size: cfg.hidden_size,
+            cache: Cache::new(cfg.num_hidden_layers, true),
+            max_seq_len: default_max_position_embeddings(),
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
             mapper,
         })
     }
 
     #[allow(clippy::too_many_arguments)]
     fn inner_forward(
         &mut self,
-        xs: &Tensor,
+        input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Option<Tensor>,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
-        let (_b_size, seq_len) = xs.dims2()?;
-        let mut xs = xs.apply(&self.embed_tokens)?;
-        let mask = if seq_len <= 1 {
-            None
-        } else {
-            Some(get_mask(seq_len, xs.device())?)
-        };
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
                 self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
+        let attention_mask = CausalMasker.make_causal_mask(input_ids, &cache)?;
+        let xs = self.embed_tokens.forward(input_ids)?;
+        let mut xs = (xs * (self.hidden_size as f64).sqrt())?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
-                mask.as_ref()
+                attention_mask
+                    .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
                 seqlen_offsets,
                 start_offsets_kernel.clone(),
                 &mut cache[i],
                 scalings.clone(),
                 self.xlora_classifier
                     .as_ref()
                     .map(|classifier| classifier.get_global_scaling_weight())
                     .unwrap_or(1.0),
                 is_scaling_pass,
-            )?;
+            )?
         }
         let xs = xs.to_device(&self.device)?;
-        xs.apply(&self.final_layernorm)
+        xs.apply(&self.norm)
     }
 
     #[allow(clippy::too_many_arguments)]
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
@@ -663,15 +696,15 @@
                 res = res.to_dtype(DType::F32)?;
             }
             extract_logits(&res.apply(&self.lm_head)?, context_lens)
         }
     }
 }
 
-impl NormalModel for Model {
+impl NormalModel for XLoraModel {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
         _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
@@ -706,15 +739,15 @@
     fn cache(&self) -> &Cache {
         &self.cache
     }
     fn device(&self) -> &Device {
         &self.device
     }
     fn is_xlora(&self) -> bool {
-        true
+        false
     }
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
     fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
         tensors.push((self.lm_head.inner(), None));
@@ -728,25 +761,63 @@
                 Some(i),
             ));
             tensors.push((
                 Arc::get_mut(&mut layer.self_attn.v_proj).unwrap().inner(),
                 Some(i),
             ));
             tensors.push((
-                Arc::get_mut(&mut layer.self_attn.dense).unwrap().inner(),
+                Arc::get_mut(&mut layer.self_attn.o_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.down_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.gate_proj).unwrap().inner(),
+                Some(i),
+            ));
+            tensors.push((
+                Arc::get_mut(&mut layer.mlp.up_proj).unwrap().inner(),
                 Some(i),
             ));
-            tensors.push((Arc::get_mut(&mut layer.mlp.fc1).unwrap().inner(), Some(i)));
-            tensors.push((Arc::get_mut(&mut layer.mlp.fc2).unwrap().inner(), Some(i)));
         }
         (tensors, &*self.mapper)
     }
+    fn activate_adapters(&mut self, adapter_names: Vec<String>) -> Result<usize> {
+        let mut sum = 0;
+        for layer in self.layers.iter_mut() {
+            sum += Arc::get_mut(&mut layer.self_attn.k_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.o_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.q_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.self_attn.v_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+
+            sum += Arc::get_mut(&mut layer.mlp.down_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.mlp.gate_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+            sum += Arc::get_mut(&mut layer.mlp.up_proj)
+                .unwrap()
+                .activate(&adapter_names)?;
+        }
+        Ok(sum)
+    }
 }
 
-impl ScalingsMaker for Model {
+impl ScalingsMaker for XLoraModel {
     fn dtype(&self) -> DType {
         self.dtype
     }
     fn get_cache(&self) -> &Cache {
         &self.cache
     }
     fn get_classifier(&self) -> &XLoraClassifier {
```

### Comparing `mistralrs-0.1.4/mistralrs-core/src/xlora_models/quantized_llama.rs` & `mistralrs-0.1.5/mistralrs-core/src/xlora_models/quantized_llama.rs`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 use std::collections::HashMap;
 
 use candle_core::quantized::QMatMul;
 use candle_core::quantized::{ggml_file, gguf_file};
 use candle_core::{DType, Device, Result, Tensor};
 use candle_nn::{Embedding, Module, RotaryEmbedding, VarBuilder};
-use mistralrs_lora::{get_lora_cfg, LinearLayerLike, LoraConfig, Merge, Ordering, QLoraLinear};
+use mistralrs_lora::{
+    get_lora_cfg, AdapterSwapper, LinearLayerLike, LoraConfig, Merge, Ordering, QLoraLinear,
+};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::device_map::DeviceMapper;
-use crate::layers::QRmsNorm;
+use crate::layers::{CausalMasker, QRmsNorm};
 use crate::models::{repeat_kv, verify_sanity_gguf, Cache};
 use crate::pipeline::extract_logits;
 use crate::DeviceMapMetadata;
 
 use super::classifier::XLoraClassifier;
 use super::{verify_sanity_adapters, NonGranularState, ScalingsMaker, XLoraConfig};
 
@@ -171,19 +173,14 @@
     n_head: usize,
     n_kv_head: usize,
     head_dim: usize,
     rotary: RotaryEmbedding,
     neg_inf: Tensor,
 }
 
-fn masked_fill(on_false: &Tensor, mask: &Tensor, on_true: &Tensor) -> Result<Tensor> {
-    let shape = mask.shape();
-    let m = mask.where_cond(&on_true.broadcast_as(shape.dims())?, on_false)?;
-    Ok(m)
-}
 impl LayerWeights {
     #[allow(clippy::too_many_arguments)]
     fn forward_attn(
         &mut self,
         x: &Tensor,
         mask: &Option<Tensor>,
         start_offsets: &[usize],
@@ -242,21 +239,15 @@
         };
         *kv_cache = Some((k.clone(), v.clone()));
 
         let k = repeat_kv(k, self.n_head / self.n_kv_head)?.contiguous()?;
         let v = repeat_kv(v, self.n_head / self.n_kv_head)?.contiguous()?;
 
         let att = (q.contiguous()?.matmul(&k.t()?.contiguous()?)? / (self.head_dim as f64).sqrt())?;
-        let att = match mask {
-            None => att,
-            Some(mask) => {
-                let mask = mask.broadcast_as(att.shape())?;
-                masked_fill(&att, &mask, &self.neg_inf)?
-            }
-        };
+        let att = CausalMasker.apply_mask(mask, att, &self.neg_inf)?;
         let att = candle_nn::ops::softmax_last_dim(&att)?;
         // Convert to contiguous as matmul doesn't support strided vs for now.
         let y = att.matmul(&v.contiguous()?)?;
         let y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, n_embd])?;
         let y = self.attention_wo.lora_forward(
             &y,
             scalings.clone(),
@@ -268,30 +259,30 @@
 }
 
 pub struct ModelWeights {
     tok_embeddings: Embedding,
     layers: Vec<LayerWeights>,
     norm: QRmsNorm,
     output: QMatMul,
-    masks: HashMap<usize, Tensor>,
     pub device: Device,
     pub cache: Cache,
     xlora_classifier: Option<XLoraClassifier>,
     pub max_seq_len: usize,
     mapper: Option<Box<dyn DeviceMapper + Send + Sync>>,
 }
 
 impl ModelWeights {
     pub fn from_ggml(
         mut ct: ggml_file::Content,
         gqa: usize,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         vb: &VarBuilder,
         ordering: &Ordering,
         xlora_config: Option<XLoraConfig>,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let head_dim = (ct.hparams.n_embd / ct.hparams.n_head) as usize;
         let rotary = RotaryEmbedding::new_partial(
             10000.,
             head_dim,
             ct.hparams.n_rot as usize,
             MAX_SEQ_LEN as usize,
@@ -324,32 +315,35 @@
                         QMatMul::from_qtensor(feed_forward_w1)?,
                         &cfg_w1,
                         lora_config,
                         vb,
                         ordering,
                         format!("model.layers.{layer_idx}.mlp.gate_proj"),
                         &mut count,
+                        preload_adapters,
                     )?,
                     feed_forward_w2: QLoraLinear::new(
                         QMatMul::from_qtensor(feed_forward_w2)?,
                         &cfg_w2,
                         lora_config,
                         vb,
                         ordering,
                         format!("model.layers.{layer_idx}.mlp.down_proj"),
                         &mut count,
+                        preload_adapters,
                     )?,
                     feed_forward_w3: QLoraLinear::new(
                         QMatMul::from_qtensor(feed_forward_w3)?,
                         &cfg_w3,
                         lora_config,
                         vb,
                         ordering,
                         format!("model.layers.{layer_idx}.mlp.up_proj"),
                         &mut count,
+                        preload_adapters,
                     )?,
                 })
             };
             let attention_norm = ct.remove(&format!("{prefix}.attention_norm.weight"))?;
             let ffn_norm = ct.remove(&format!("{prefix}.ffn_norm.weight"))?;
             let cfgq = get_lora_cfg(&attention_wq);
             let cfgk = get_lora_cfg(&attention_wk);
@@ -360,58 +354,89 @@
                     QMatMul::from_qtensor(attention_wq)?,
                     &cfgq,
                     lora_config,
                     vb,
                     ordering,
                     format!("model.layers.{layer_idx}.self_attn.q_proj"),
                     &mut count,
+                    preload_adapters,
                 )?,
                 attention_wk: QLoraLinear::new(
                     QMatMul::from_qtensor(attention_wk)?,
                     &cfgk,
                     lora_config,
                     vb,
                     ordering,
                     format!("model.layers.{layer_idx}.self_attn.k_proj"),
                     &mut count,
+                    preload_adapters,
                 )?,
                 attention_wv: QLoraLinear::new(
                     QMatMul::from_qtensor(attention_wv)?,
                     &cfgv,
                     lora_config,
                     vb,
                     ordering,
                     format!("model.layers.{layer_idx}.self_attn.v_proj"),
                     &mut count,
+                    preload_adapters,
                 )?,
                 attention_wo: QLoraLinear::new(
                     QMatMul::from_qtensor(attention_wo)?,
                     &cfgo,
                     lora_config,
                     vb,
                     ordering,
                     format!("model.layers.{layer_idx}.self_attn.o_proj"),
                     &mut count,
+                    preload_adapters,
                 )?,
                 attention_norm: QRmsNorm::new(attention_norm, 1e-5)?,
                 mlp_or_moe,
                 ffn_norm: QRmsNorm::new(ffn_norm, 1e-5)?,
                 n_head: ct.hparams.n_head as usize,
                 n_kv_head: ct.hparams.n_head as usize / gqa,
                 head_dim: (ct.hparams.n_embd / ct.hparams.n_head) as usize,
                 rotary: rotary.clone(),
                 neg_inf: neg_inf.clone(),
             })
         }
+        if xlora_config.is_none() && preload_adapters.is_none() {
+            // We are now a LoRA model so we must merge the weights
+            info!("Merging LoRA adapters.");
+            for layer in layers.iter_mut().tqdm() {
+                layer.attention_wk.merge_weights()?;
+                layer.attention_wo.merge_weights()?;
+                layer.attention_wq.merge_weights()?;
+                layer.attention_wv.merge_weights()?;
+                match &mut layer.mlp_or_moe {
+                    MlpOrMoe::Mlp(ref mut m) => {
+                        m.feed_forward_w1.merge_weights()?;
+                        m.feed_forward_w2.merge_weights()?;
+                        m.feed_forward_w3.merge_weights()?;
+                    }
+                    MlpOrMoe::MoE {
+                        n_expert_used: _,
+                        feed_forward_gate_inp: _,
+                        experts,
+                    } => {
+                        for expert in experts {
+                            expert.feed_forward_w1.merge_weights()?;
+                            expert.feed_forward_w2.merge_weights()?;
+                            expert.feed_forward_w3.merge_weights()?;
+                        }
+                    }
+                }
+            }
+        }
         Ok(Self {
             tok_embeddings: Embedding::new(tok_embeddings, ct.hparams.n_embd as usize),
             layers,
             norm,
             output: QMatMul::from_qtensor(output)?,
-            masks: HashMap::new(),
             device: ct.device.clone(),
             cache: Cache::new(ct.hparams.n_layer as usize, true),
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb.clone(), true)
                     .unwrap()
             }),
             max_seq_len: MAX_SEQ_LEN as usize, // Cannot determine from ggml.
@@ -420,19 +445,20 @@
     }
 
     #[allow(clippy::too_many_arguments)]
     pub fn from_gguf<R: std::io::Seek + std::io::Read>(
         ct: gguf_file::Content,
         reader: &mut R,
         device: &Device,
-        lora_config: &[(String, LoraConfig)],
+        lora_config: &[((String, String), LoraConfig)],
         vb: &VarBuilder,
         ordering: &Ordering,
         xlora_config: Option<XLoraConfig>,
         mapper: DeviceMapMetadata,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let md_get = |s: &str| match ct.metadata.get(s) {
             None => candle_core::bail!("cannot find {s} in metadata"),
             Some(v) => Ok(v),
         };
         verify_sanity_gguf(
             md_get("general.architecture")?.to_string().unwrap(),
@@ -508,32 +534,35 @@
                         QMatMul::from_qtensor(feed_forward_w1)?,
                         &cfg_w1,
                         lora_config,
                         vb,
                         ordering,
                         format!("model.layers.{layer_idx}.mlp.gate_proj"),
                         &mut count,
+                        preload_adapters,
                     )?,
                     feed_forward_w2: QLoraLinear::new(
                         QMatMul::from_qtensor(feed_forward_w2)?,
                         &cfg_w2,
                         lora_config,
                         vb,
                         ordering,
                         format!("model.layers.{layer_idx}.mlp.down_proj"),
                         &mut count,
+                        preload_adapters,
                     )?,
                     feed_forward_w3: QLoraLinear::new(
                         QMatMul::from_qtensor(feed_forward_w3)?,
                         &cfg_w3,
                         lora_config,
                         vb,
                         ordering,
                         format!("model.layers.{layer_idx}.mlp.up_proj"),
                         &mut count,
+                        preload_adapters,
                     )?,
                 })
             } else {
                 let feed_forward_gate_inp =
                     ct.tensor(reader, &format!("{prefix}.ffn_gate_inp.weight"), device)?;
                 let mut experts = Vec::with_capacity(n_expert);
                 for i in 0..n_expert {
@@ -551,32 +580,35 @@
                             QMatMul::from_qtensor(feed_forward_w1)?,
                             &cfg_w1,
                             lora_config,
                             vb,
                             ordering,
                             format!("model.layers.{layer_idx}.mlp.gate_proj.{i}"),
                             &mut count,
+                            preload_adapters,
                         )?,
                         feed_forward_w2: QLoraLinear::new(
                             QMatMul::from_qtensor(feed_forward_w2)?,
                             &cfg_w2,
                             lora_config,
                             vb,
                             ordering,
                             format!("model.layers.{layer_idx}.mlp.down_proj.{i}"),
                             &mut count,
+                            preload_adapters,
                         )?,
                         feed_forward_w3: QLoraLinear::new(
                             QMatMul::from_qtensor(feed_forward_w3)?,
                             &cfg_w3,
                             lora_config,
                             vb,
                             ordering,
                             format!("model.layers.{layer_idx}.mlp.up_proj.{i}"),
                             &mut count,
+                            preload_adapters,
                         )?,
                     })
                 }
                 MlpOrMoe::MoE {
                     n_expert_used,
                     feed_forward_gate_inp: QMatMul::from_qtensor(feed_forward_gate_inp)?,
                     experts,
@@ -594,53 +626,57 @@
                     QMatMul::from_qtensor(attention_wq)?,
                     &cfgq,
                     lora_config,
                     vb,
                     ordering,
                     format!("model.layers.{layer_idx}.self_attn.q_proj"),
                     &mut count,
+                    preload_adapters,
                 )?,
                 attention_wk: QLoraLinear::new(
                     QMatMul::from_qtensor(attention_wk)?,
                     &cfgk,
                     lora_config,
                     vb,
                     ordering,
                     format!("model.layers.{layer_idx}.self_attn.k_proj"),
                     &mut count,
+                    preload_adapters,
                 )?,
                 attention_wv: QLoraLinear::new(
                     QMatMul::from_qtensor(attention_wv)?,
                     &cfgv,
                     lora_config,
                     vb,
                     ordering,
                     format!("model.layers.{layer_idx}.self_attn.v_proj"),
                     &mut count,
+                    preload_adapters,
                 )?,
                 attention_wo: QLoraLinear::new(
                     QMatMul::from_qtensor(attention_wo)?,
                     &cfgo,
                     lora_config,
                     vb,
                     ordering,
                     format!("model.layers.{layer_idx}.self_attn.o_proj"),
                     &mut count,
+                    preload_adapters,
                 )?,
                 attention_norm: QRmsNorm::new(attention_norm, rms_norm_eps)?,
                 mlp_or_moe,
                 ffn_norm: QRmsNorm::new(ffn_norm, rms_norm_eps)?,
                 n_head: head_count,
                 n_kv_head: head_count_kv,
                 head_dim: embedding_length / head_count,
                 rotary: rotary.clone(),
                 neg_inf,
             })
         }
-        if xlora_config.is_none() {
+        if xlora_config.is_none() && preload_adapters.is_none() {
             // We are now a LoRA model so we must merge the weights
             info!("Merging LoRA adapters.");
             for layer in layers.iter_mut().tqdm() {
                 layer.attention_wk.merge_weights()?;
                 layer.attention_wo.merge_weights()?;
                 layer.attention_wq.merge_weights()?;
                 layer.attention_wv.merge_weights()?;
@@ -665,70 +701,80 @@
             }
         }
         Ok(Self {
             tok_embeddings: Embedding::new(tok_embeddings, embedding_length),
             layers,
             norm,
             output: QMatMul::from_qtensor(output)?,
-            masks: HashMap::new(),
             device: device.clone(),
             cache: Cache::new(block_count, true),
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb.clone(), true)
                     .unwrap()
             }),
             max_seq_len,
             mapper: Some(mapper),
         })
     }
 
-    fn mask(&mut self, t: usize, device: &Device) -> Result<Tensor> {
-        if let Some(mask) = self.masks.get(&t) {
-            Ok(mask.clone())
-        } else {
-            let mask: Vec<_> = (0..t)
-                .flat_map(|i| (0..t).map(move |j| u8::from(j > i)))
-                .collect();
-            let mask = Tensor::from_slice(&mask, (t, t), device)?;
-            self.masks.insert(t, mask.clone());
-            Ok(mask)
+    pub fn activate_adapters(&mut self, adapter_names: Vec<String>) -> Result<usize> {
+        let mut sum = 0;
+        for layer in self.layers.iter_mut() {
+            sum += layer.attention_wk.activate(&adapter_names)?;
+            sum += layer.attention_wo.activate(&adapter_names)?;
+            sum += layer.attention_wq.activate(&adapter_names)?;
+            sum += layer.attention_wv.activate(&adapter_names)?;
+            match &mut layer.mlp_or_moe {
+                MlpOrMoe::Mlp(ref mut m) => {
+                    sum += m.feed_forward_w1.activate(&adapter_names)?;
+                    sum += m.feed_forward_w2.activate(&adapter_names)?;
+                    sum += m.feed_forward_w3.activate(&adapter_names)?;
+                }
+                MlpOrMoe::MoE {
+                    n_expert_used: _,
+                    feed_forward_gate_inp: _,
+                    experts,
+                } => {
+                    for expert in experts {
+                        sum += expert.feed_forward_w1.activate(&adapter_names)?;
+                        sum += expert.feed_forward_w2.activate(&adapter_names)?;
+                        sum += expert.feed_forward_w3.activate(&adapter_names)?;
+                    }
+                }
+            }
         }
+        Ok(sum)
     }
 
     #[allow(clippy::too_many_arguments)]
     fn inner_forward(
         &mut self,
         x: &Tensor,
         start_offsets: &[usize],
         start_offsets_kernel: Tensor,
         scalings: Option<Tensor>,
         is_full_pass: bool,
         no_kv_cache: bool,
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
-        let (_b_sz, seq_len) = x.dims2()?;
-        let mask = if seq_len == 1 {
-            None
-        } else {
-            Some(self.mask(seq_len, x.device())?)
-        };
         let mut layer_in = self.tok_embeddings.forward(x)?;
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
                 self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
+        let mask = CausalMasker.make_causal_mask(x, &cache)?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
             if let Some(ref mapper) = self.mapper {
                 layer_in = mapper.map(layer_in, i)?;
             }
             let x = layer_in;
             let residual = &x;
             let x = layer.attention_norm.forward(&x)?;
```

### Comparing `mistralrs-0.1.4/mistralrs-lora/Cargo.toml` & `mistralrs-0.1.5/mistralrs-lora/Cargo.toml`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-lora/src/layer.rs` & `mistralrs-0.1.5/mistralrs-lora/src/layer.rs`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             dtype: DType::F32,
         })
     }
 
     pub fn from_linear(linear: Linear) -> Self {
         Self {
             inner: QMatMul::Tensor(linear.weight().clone()),
-            bias: Some(linear.bias().unwrap().clone()),
+            bias: linear.bias().cloned(),
             dtype: if linear.weight().device().is_cuda() {
                 DType::BF16
             } else {
                 DType::F32
             },
         }
     }
@@ -78,19 +78,22 @@
     pub fn bias(&self) -> Option<&Tensor> {
         self.bias.as_ref()
     }
 }
 
 impl Module for QLinear {
     fn forward(&self, xs: &Tensor) -> Result<Tensor> {
+        let xs = if self.is_quant() {
+            xs.to_dtype(DType::F32)?
+        } else {
+            xs.clone()
+        };
         if let Some(bias) = &self.bias {
             self.inner
-                .forward(&xs.to_dtype(DType::F32)?)?
+                .forward(&xs)?
                 .broadcast_add(bias)?
                 .to_dtype(self.dtype)
         } else {
-            self.inner
-                .forward(&xs.to_dtype(DType::F32)?)?
-                .to_dtype(self.dtype)
+            self.inner.forward(&xs)?.to_dtype(self.dtype)
         }
     }
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-lora/src/lib.rs` & `mistralrs-0.1.5/mistralrs-lora/src/lib.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 use std::{collections::HashSet, fmt::Debug, sync::Arc};
 
 use candle_core::{
     quantized::{QMatMul, QTensor},
     IndexOp, Result, Tensor, D,
 };
-use candle_nn::{Linear, Module, VarBuilder};
+use candle_nn::{init, Linear, Module, VarBuilder};
 use loralinear::LoraLinear;
 pub use qloralinear::QLoraLinear;
 use serde::Deserialize;
 
 pub mod layer;
 mod loralinear;
 mod qloralinear;
 
 use std::collections::HashMap;
 
 #[derive(Clone, Debug, Deserialize)]
+pub struct PreloadAdapter {
+    pub name: String,
+    pub adapter_model_id: String,
+}
+
+#[derive(Clone, Debug, Deserialize)]
 pub struct Ordering {
     #[serde(rename = "order")]
     pub adapters: Option<Vec<String>>,
     pub layers: HashMap<String, usize>,
     pub base_model_id: String,
+    pub preload_adapters: Option<Vec<PreloadAdapter>>,
 }
 
 #[derive(Clone, Debug)]
 /// Configuration for LoraLinear
 pub struct LoraLinearConfig {
     in_features: usize,
     out_features: usize,
@@ -68,16 +75,47 @@
             alpha,
             dropout,
             target_modules,
         }
     }
 }
 
+#[derive(Debug)]
+struct Adapter {
+    a: Linear,
+    b: Linear,
+    scale: f64,
+}
+
+fn make_adapter(
+    a_vb: VarBuilder,
+    b_vb: VarBuilder,
+    cfg: &LoraConfig,
+    linear_cfg: &LoraLinearConfig,
+) -> Result<Adapter> {
+    assert!(a_vb.contains_tensor("weight"));
+    let a = a_vb.get_with_hints(
+        (cfg.rank, linear_cfg.in_features),
+        "weight",
+        init::DEFAULT_KAIMING_NORMAL,
+    )?;
+    assert!(b_vb.contains_tensor("weight"));
+    let b = b_vb.get_with_hints((linear_cfg.out_features, cfg.rank), "weight", init::ZERO)?;
+    let a = Linear::new(a, None);
+    let b = Linear::new(b, None);
+    let scale = if cfg.rank > 0 {
+        cfg.alpha / cfg.rank as f64
+    } else {
+        1.0
+    };
+    Ok(Adapter { a, b, scale })
+}
+
 /// Any layer that is linear-like.
-pub trait LinearLayerLike: Debug + Merge {
+pub trait LinearLayerLike: Debug + Merge + AdapterSwapper {
     fn inner(&mut self) -> &mut QMatMul;
     fn is_quant(&self) -> bool;
     fn weight(&self) -> &Tensor;
     fn bias(&self) -> Option<&Tensor>;
     fn lora_forward(
         &self,
         x: &Tensor,
@@ -90,23 +128,66 @@
 pub trait Merge {
     /// Get the delta weight of the LoRA layer. This is meant to be an internal method.
     fn get_delta_weight(&self, adapter: usize) -> Result<Tensor>;
     /// Merge the LoRA weights.
     fn merge_weights(&mut self) -> Result<()>;
 }
 
+pub trait AdapterSwapper {
+    fn activate(&mut self, adapter_names: &[String]) -> Result<usize> {
+        if self.can_load() {
+            self._activate_adapters(adapter_names)?;
+            Ok(1)
+        } else {
+            Ok(0)
+        }
+    }
+    fn _activate_adapters(&mut self, adapters: &[String]) -> Result<()>;
+    fn has_adapter(&self, adapter: String) -> bool;
+    /// Pass the prefix for the layer (excluding .lora_?) as `module_prefix`
+    fn load_new_adapter(
+        &mut self,
+        name: String,
+        vb: VarBuilder,
+        cfg: &LoraConfig,
+        module_prefix: String,
+    ) -> Result<()>;
+    fn can_load(&self) -> bool;
+}
+
 impl Merge for Linear {
     fn merge_weights(&mut self) -> Result<()> {
         Ok(())
     }
     fn get_delta_weight(&self, _adapter: usize) -> Result<Tensor> {
         unreachable!()
     }
 }
 
+impl AdapterSwapper for Linear {
+    fn _activate_adapters(&mut self, _adapter: &[String]) -> Result<()> {
+        unreachable!()
+    }
+    fn can_load(&self) -> bool {
+        false
+    }
+    fn has_adapter(&self, _adapter: String) -> bool {
+        false
+    }
+    fn load_new_adapter(
+        &mut self,
+        _name: String,
+        _vb: VarBuilder,
+        _cfg: &LoraConfig,
+        _module_prefix: String,
+    ) -> Result<()> {
+        unreachable!()
+    }
+}
+
 impl LinearLayerLike for Linear {
     fn inner(&mut self) -> &mut QMatMul {
         unreachable!()
     }
     fn bias(&self) -> Option<&Tensor> {
         self.bias()
     }
@@ -123,22 +204,24 @@
         self.forward(x)
     }
     fn is_quant(&self) -> bool {
         false
     }
 }
 
+#[allow(clippy::too_many_arguments)]
 pub fn linear(
     d1: usize,
     d2: usize,
     base_vb: crate::VarBuilder,
     vb: VarBuilder,
-    lora_config: &[(String, LoraConfig)],
+    lora_config: &[((String, String), LoraConfig)],
     count: &mut usize,
     ord: &Ordering,
+    preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
 ) -> Result<Arc<dyn LinearLayerLike + Send + Sync>> {
     let prefix = vb.prefix();
     let module = prefix.split('.').last().unwrap();
 
     let linear_config = LoraLinearConfig::new(d1, d2);
     let inner = candle_nn::linear(d1, d2, base_vb.clone())?;
 
@@ -151,27 +234,36 @@
 
     if !target_modules.contains(module) {
         return Ok(Arc::new(inner));
     }
     let name = prefix.split("lora_A").last().unwrap();
     let layer = ord.layers.get(name).unwrap();
 
-    let lorainner = LoraLinear::new(&inner, &linear_config, lora_config, &vb, *layer)?;
+    let lorainner = LoraLinear::new(
+        &inner,
+        &linear_config,
+        lora_config,
+        &vb,
+        *layer,
+        preload_adapters,
+    )?;
     *count += 1;
     Ok(Arc::new(lorainner))
 }
 
+#[allow(clippy::too_many_arguments)]
 pub fn linear_no_bias(
     d1: usize,
     d2: usize,
     base_vb: crate::VarBuilder,
     vb: VarBuilder,
-    lora_config: &[(String, LoraConfig)],
+    lora_config: &[((String, String), LoraConfig)],
     count: &mut usize,
     ord: &Ordering,
+    preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
 ) -> Result<Arc<dyn LinearLayerLike + Send + Sync>> {
     let prefix = vb.prefix();
     let module = prefix.split('.').last().unwrap();
 
     let linear_config = LoraLinearConfig::new(d1, d2);
     let inner = candle_nn::linear_no_bias(d1, d2, base_vb.clone())?;
 
@@ -184,15 +276,22 @@
 
     if !target_modules.contains(module) {
         return Ok(Arc::new(inner));
     }
     let name = prefix.split("lora_A").last().unwrap();
     let layer = ord.layers.get(name).unwrap();
 
-    let lorainner = LoraLinear::new(&inner, &linear_config, lora_config, &vb, *layer)?;
+    let lorainner = LoraLinear::new(
+        &inner,
+        &linear_config,
+        lora_config,
+        &vb,
+        *layer,
+        preload_adapters,
+    )?;
     *count += 1;
     Ok(Arc::new(lorainner))
 }
 
 fn get_maybe_topk_scalings(scalings: Tensor, layer: usize) -> Result<Tensor> {
     scalings.i((.., .., layer, ..))
 }
@@ -200,21 +299,40 @@
 #[allow(clippy::too_many_arguments)]
 pub fn linear_b(
     in_dim: usize,
     out_dim: usize,
     bias: bool,
     base_vb: crate::VarBuilder,
     vb: crate::VarBuilder,
-    lora_config: &[(String, LoraConfig)],
+    lora_config: &[((String, String), LoraConfig)],
     count: &mut usize,
     ord: &Ordering,
+    preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
 ) -> Result<Arc<dyn LinearLayerLike + Send + Sync>> {
     if bias {
-        linear(in_dim, out_dim, base_vb, vb, lora_config, count, ord)
+        linear(
+            in_dim,
+            out_dim,
+            base_vb,
+            vb,
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )
     } else {
-        linear_no_bias(in_dim, out_dim, base_vb, vb, lora_config, count, ord)
+        linear_no_bias(
+            in_dim,
+            out_dim,
+            base_vb,
+            vb,
+            lora_config,
+            count,
+            ord,
+            preload_adapters,
+        )
     }
 }
 
 pub fn get_lora_cfg(tensor: &QTensor) -> LoraLinearConfig {
     LoraLinearConfig::new(tensor.shape().dims()[1], tensor.shape().dims()[0])
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-lora/src/loralinear.rs` & `mistralrs-0.1.5/mistralrs-lora/src/loralinear.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,58 @@
-use std::{iter::zip, ops::Mul};
+use std::{collections::HashMap, iter::zip, ops::Mul};
 
 use candle_core::{
+    bail,
     quantized::{QMatMul, QTensor},
     Module, Result, Tensor,
 };
-use candle_nn::{init, Dropout, Linear, VarBuilder};
+use candle_nn::{Linear, VarBuilder};
 use either::Either;
 
 use crate::{
-    apply_scalings_to_x, get_maybe_topk_scalings, layer::QLinear, LinearLayerLike, LoraConfig,
-    LoraLinearConfig, Merge,
+    apply_scalings_to_x, get_maybe_topk_scalings, layer::QLinear, make_adapter, Adapter,
+    AdapterSwapper, LinearLayerLike, LoraConfig, LoraLinearConfig, Merge,
 };
 
 #[derive(Debug)]
 pub struct LoraLinear {
     old: QLinear,
     a_adapters: Either<Vec<Linear>, (Tensor, Vec<Linear>)>,
     b_adapters: Either<Vec<Linear>, (Tensor, Vec<Linear>)>,
     scale_adapters: Vec<f64>,
-    dropout_adapters: Vec<Option<Dropout>>,
     layer_n: usize,
     merged: bool,
+    adapters: HashMap<String, Adapter>,
+    linear_config: LoraLinearConfig,
 }
 
 impl LoraLinear {
     pub fn new(
         old: &dyn LinearLayerLike,
         linear_config: &LoraLinearConfig,
-        config: &[(String, LoraConfig)],
+        config: &[((String, String), LoraConfig)],
         vb: &VarBuilder,
         layer_n: usize,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let mut a_adapters = Vec::with_capacity(config.len());
         let mut b_adapters = Vec::with_capacity(config.len());
         let mut scale_adapters = Vec::with_capacity(config.len());
-        let mut dropout_adapters = Vec::with_capacity(config.len());
         let a_vb = vb.pp("lora_A".to_string());
         let b_vb = vb.pp("lora_B".to_string());
         let mut state = None;
         let mut all_same = true;
-        for (name, cfg) in config.iter() {
-            let a_pp = a_vb.pp(name);
-            assert!(a_pp.contains_tensor("weight"));
-            let a = a_pp.get_with_hints(
-                (cfg.rank, linear_config.in_features),
-                "weight",
-                init::DEFAULT_KAIMING_NORMAL,
-            )?;
-            let b_pp = b_vb.pp(name);
-            assert!(b_pp.contains_tensor("weight"));
-            let b =
-                b_pp.get_with_hints((linear_config.out_features, cfg.rank), "weight", init::ZERO)?;
-            a_adapters.push(Linear::new(a, None));
-            b_adapters.push(Linear::new(b, None));
-            scale_adapters.push(if cfg.rank > 0 {
-                cfg.alpha / cfg.rank as f64
-            } else {
-                1.0
-            });
-            dropout_adapters.push(cfg.dropout.map(Dropout::new));
+        let mut adapters = HashMap::new();
+        for ((name_id, adapter_name), cfg) in config.iter() {
+            let a_pp = a_vb.pp(name_id);
+            let b_pp = b_vb.pp(name_id);
+            let adapter = make_adapter(a_pp, b_pp, cfg, linear_config)?;
+            a_adapters.push(adapter.a.clone());
+            b_adapters.push(adapter.b.clone());
+            scale_adapters.push(adapter.scale);
             if state.is_some_and(|x| {
                 x == (
                     cfg.rank,
                     linear_config.in_features,
                     linear_config.out_features,
                     cfg.alpha,
                     cfg.dropout,
@@ -75,14 +65,25 @@
                     linear_config.out_features,
                     cfg.alpha,
                     cfg.dropout,
                 ));
             } else {
                 all_same = false;
             }
+            adapters.insert(adapter_name.clone(), adapter);
+        }
+
+        if let Some(preload_adapters) = preload_adapters {
+            all_same = false;
+            for (name, (vb, cfg)) in preload_adapters {
+                let a_vb = vb.set_prefix(a_vb.prefix());
+                let b_vb = vb.set_prefix(b_vb.prefix());
+                let adapter = make_adapter(a_vb, b_vb, cfg, linear_config)?;
+                adapters.insert(name.clone(), adapter);
+            }
         }
 
         if all_same {
             let a_adapters_stack = Tensor::cat(
                 &a_adapters
                     .iter()
                     .map(|x| x.weight().unsqueeze(0))
@@ -104,32 +105,84 @@
             .to_dtype(a_adapters_stack.dtype())?;
             let a_adapters_stack = a_adapters_stack.broadcast_mul(&scale_adapters_t)?;
             Ok(LoraLinear {
                 old: QLinear::from_parts(old.weight().clone(), old.bias().cloned()),
                 a_adapters: Either::Right((a_adapters_stack.clone(), a_adapters)),
                 b_adapters: Either::Right((b_adapters_stack, b_adapters)),
                 scale_adapters,
-                dropout_adapters,
                 layer_n,
                 merged: false,
+                adapters,
+                linear_config: linear_config.clone(),
             })
         } else {
             Ok(LoraLinear {
                 old: QLinear::from_parts(old.weight().clone(), old.bias().cloned()),
                 a_adapters: Either::Left(a_adapters),
                 b_adapters: Either::Left(b_adapters),
                 scale_adapters,
-                dropout_adapters,
                 layer_n,
                 merged: false,
+                adapters,
+                linear_config: linear_config.clone(),
             })
         }
     }
 }
 
+impl AdapterSwapper for LoraLinear {
+    fn _activate_adapters(&mut self, adapter_names: &[String]) -> Result<()> {
+        match (
+            &mut self.a_adapters,
+            &mut self.b_adapters,
+            &mut self.scale_adapters,
+        ) {
+            (Either::Left(a), Either::Left(b), s) => {
+                a.clear();
+                b.clear();
+                s.clear();
+                for adapter_name in adapter_names {
+                    let Adapter {
+                        a: a_w,
+                        b: b_w,
+                        scale,
+                    } = match self.adapters.get(adapter_name) {
+                        Some(a) => a,
+                        None => bail!("Cannot load adapter `{adapter_name}`."),
+                    };
+                    a.push(a_w.clone());
+                    b.push(b_w.clone());
+                    s.push(*scale);
+                }
+            }
+            _ => unreachable!("Adapters should not be stacked if new ones are being activated."),
+        }
+        Ok(())
+    }
+    fn has_adapter(&self, adapter: String) -> bool {
+        self.adapters.contains_key(&adapter)
+    }
+    fn load_new_adapter(
+        &mut self,
+        name: String,
+        vb: VarBuilder,
+        cfg: &LoraConfig,
+        module_prefix: String,
+    ) -> Result<()> {
+        let a_vb = vb.set_prefix(&module_prefix).pp("lora_A".to_string());
+        let b_vb = vb.set_prefix(&module_prefix).pp("lora_B".to_string());
+        let adapter = make_adapter(a_vb, b_vb, cfg, &self.linear_config)?;
+        self.adapters.insert(name.clone(), adapter);
+        Ok(())
+    }
+    fn can_load(&self) -> bool {
+        true
+    }
+}
+
 impl Merge for LoraLinear {
     fn get_delta_weight(&self, adapter: usize) -> Result<Tensor> {
         match (&self.a_adapters, &self.b_adapters) {
             (Either::Left(a), Either::Left(b)) | (Either::Right((_, a)), Either::Right((_, b))) => {
                 let w_a = a[adapter].weight();
                 let w_b = b[adapter].weight();
 
@@ -187,74 +240,68 @@
         if self.merged {
             return Ok(result);
         }
 
         if is_scaling_pass.is_some_and(|x| x == 0.) {
             return Ok(result);
         }
-        let scalings = scalings.unwrap();
 
-        let scalings = get_maybe_topk_scalings(scalings, self.layer_n)?;
-        if self.a_adapters.is_left() || scalings.dims3()?.1 != 1 {
+        let scalings =
+            scalings.map(|scalings| get_maybe_topk_scalings(scalings, self.layer_n).unwrap());
+        if self.a_adapters.is_left()
+            || scalings
+                .as_ref()
+                .is_some_and(|scalings| scalings.dims3().unwrap().1 != 1)
+        {
             let a_adapters = if self.a_adapters.is_right() {
                 self.a_adapters.as_ref().unwrap_right().1.clone()
             } else {
                 self.a_adapters.as_ref().unwrap_left().clone()
             };
             let b_adapters = if self.b_adapters.is_right() {
                 self.b_adapters.as_ref().unwrap_right().1.clone()
             } else {
                 self.b_adapters.as_ref().unwrap_left().clone()
             };
             //No fan_in_fan_out so no weight.transpose(0,1)
-            for (i, (adapter_a, (adapter_b, (adapter_scale, adapter_dropout)))) in zip(
-                a_adapters,
-                zip(
-                    b_adapters,
-                    zip(&self.scale_adapters, &self.dropout_adapters),
-                ),
-            )
-            .enumerate()
+            for (i, (adapter_a, (adapter_b, adapter_scale))) in
+                zip(a_adapters, zip(b_adapters, &self.scale_adapters)).enumerate()
             {
-                let mut input_new = input.to_dtype(adapter_a.weight().dtype())?;
-                input_new = apply_scalings_to_x(input_new.clone(), &scalings, i)?;
-
-                input_new = if let Some(ref dropout) = adapter_dropout {
-                    dropout.forward(&input_new, true)?
+                let input_new = input.to_dtype(adapter_a.weight().dtype())?;
+                let input_new = if let Some(scalings) = &scalings {
+                    apply_scalings_to_x(input_new, scalings, i)?
                 } else {
-                    input_new.clone()
+                    input_new
                 };
 
                 let res = adapter_b
                     .forward(&adapter_a.forward(&input_new)?)?
                     .mul(*adapter_scale)?
                     .mul(global_scaling_weight)?;
                 result = (result + res)?;
             }
             Ok(result)
         } else {
             let adapter_a = &self.a_adapters.as_ref().unwrap_right().0;
             let adapter_b = &self.b_adapters.as_ref().unwrap_right().0;
             let adapter_scales = &self.scale_adapters;
             let n_adapters = adapter_scales.len();
-            let dropout = &self.dropout_adapters[0];
-            let scalings = scalings
-                .squeeze(0)?
-                .squeeze(0)?
-                .unsqueeze(1)?
-                .unsqueeze(1)?;
-            let adapter_a = adapter_a
-                .broadcast_mul(&scalings)?
-                .mul(global_scaling_weight)?;
-
-            let input = if let Some(ref d) = dropout {
-                d.forward(input, true)?
+            let adapter_a = if let Some(scalings) = scalings.as_ref() {
+                let scalings = scalings
+                    .squeeze(0)?
+                    .squeeze(0)?
+                    .unsqueeze(1)?
+                    .unsqueeze(1)?;
+                adapter_a
+                    .broadcast_mul(&scalings)?
+                    .mul(global_scaling_weight)?
             } else {
-                input.clone()
+                adapter_a.clone().mul(global_scaling_weight)?
             };
+
             let (b, s, h) = input.dims3()?;
             let input = input.reshape((b * s, h))?;
             let out = adapter_a.broadcast_matmul(&input.t()?)?;
             let out = adapter_b.broadcast_matmul(&out)?;
             let o_h = out.dims()[1];
             let out = out.reshape((n_adapters, b, s, o_h))?;
             let out = out.sum(0)?;
```

### Comparing `mistralrs-0.1.4/mistralrs-lora/src/qloralinear.rs` & `mistralrs-0.1.5/mistralrs-lora/src/qloralinear.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-use std::{iter::zip, ops::Mul};
+use std::{collections::HashMap, iter::zip, ops::Mul};
 
 use candle_core::{
+    bail,
     quantized::{QMatMul, QTensor},
-    DType, Module, Result, Tensor,
+    Module, Result, Tensor,
 };
-use candle_nn::{init, Dropout, Linear, VarBuilder};
+use candle_nn::{Linear, VarBuilder};
 use either::Either;
 
 use crate::{
-    apply_scalings_to_x, get_maybe_topk_scalings, LinearLayerLike, LoraConfig, LoraLinearConfig,
-    Merge, Ordering,
+    apply_scalings_to_x, get_maybe_topk_scalings, make_adapter, Adapter, AdapterSwapper,
+    LinearLayerLike, LoraConfig, LoraLinearConfig, Merge, Ordering,
 };
 
 #[derive(Debug)]
 pub struct QLoraLinear {
     old: QMatMul,
     a_adapters: Either<Vec<Linear>, (Tensor, Vec<Linear>)>,
     b_adapters: Either<Vec<Linear>, (Tensor, Vec<Linear>)>,
     scale_adapters: Vec<f64>,
-    dropout_adapters: Vec<Option<Dropout>>,
     layer_n: usize,
     merged: bool,
+    adapters: HashMap<String, Adapter>,
+    linear_config: Option<LoraLinearConfig>,
 }
 
 /// Specialized QLoRA for no bias
 impl QLoraLinear {
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         old: QMatMul,
         linear_config: &LoraLinearConfig,
-        config: &[(String, LoraConfig)],
+        config: &[((String, String), LoraConfig)],
         vb: &VarBuilder,
         ordering: &Ordering,
         prefix: String,
         count: &mut usize,
+        preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
         let target_modules = &config[0].1.target_modules;
         for (_, cfg) in config {
             if &cfg.target_modules != target_modules {
                 candle_core::bail!("Expected all target modules to be the same.");
             }
         }
@@ -44,54 +48,39 @@
         let module = prefix.split('.').last().unwrap();
         if !target_modules.contains(module) {
             return Ok(Self {
                 old,
                 a_adapters: Either::Left(vec![]),
                 b_adapters: Either::Left(vec![]),
                 scale_adapters: vec![],
-                dropout_adapters: vec![],
                 layer_n: usize::MAX,
                 merged: false,
+                adapters: HashMap::default(),
+                linear_config: None,
             });
         }
 
         *count += 1;
 
         let mut a_adapters = Vec::with_capacity(config.len());
         let mut b_adapters = Vec::with_capacity(config.len());
         let mut scale_adapters = Vec::with_capacity(config.len());
-        let mut dropout_adapters = Vec::with_capacity(config.len());
         let vb = vb.pp(prefix.clone());
         let a_vb = vb.pp("lora_A".to_string());
         let b_vb = vb.pp("lora_B".to_string());
         let mut state = None;
         let mut all_same = true;
-        for (name, cfg) in config.iter() {
-            let a_pp = a_vb.pp(name);
-            assert!(a_pp.contains_tensor("weight"));
-            let a = a_pp
-                .get_with_hints(
-                    (cfg.rank, linear_config.in_features),
-                    "weight",
-                    init::DEFAULT_KAIMING_NORMAL,
-                )?
-                .to_dtype(DType::F32)?;
-            let b_pp = b_vb.pp(name);
-            assert!(b_pp.contains_tensor("weight"));
-            let b = b_pp
-                .get_with_hints((linear_config.out_features, cfg.rank), "weight", init::ZERO)?
-                .to_dtype(DType::F32)?;
-            a_adapters.push(Linear::new(a, None));
-            b_adapters.push(Linear::new(b, None));
-            scale_adapters.push(if cfg.rank > 0 {
-                cfg.alpha / cfg.rank as f64
-            } else {
-                1.0
-            });
-            dropout_adapters.push(cfg.dropout.map(Dropout::new));
+        let mut adapters = HashMap::new();
+        for ((name_id, adapter_name), cfg) in config.iter() {
+            let a_pp = a_vb.pp(name_id);
+            let b_pp = b_vb.pp(name_id);
+            let adapter = make_adapter(a_pp, b_pp, cfg, linear_config)?;
+            a_adapters.push(adapter.a.clone());
+            b_adapters.push(adapter.b.clone());
+            scale_adapters.push(adapter.scale);
             if state.is_some_and(|x| {
                 x == (
                     cfg.rank,
                     linear_config.in_features,
                     linear_config.out_features,
                     cfg.alpha,
                     cfg.dropout,
@@ -104,15 +93,27 @@
                     linear_config.out_features,
                     cfg.alpha,
                     cfg.dropout,
                 ));
             } else {
                 all_same = false;
             }
+            adapters.insert(adapter_name.clone(), adapter);
+        }
+
+        if let Some(preload_adapters) = preload_adapters {
+            all_same = false;
+            for (name, (vb, cfg)) in preload_adapters {
+                let a_vb = vb.set_prefix(a_vb.prefix());
+                let b_vb = vb.set_prefix(b_vb.prefix());
+                let adapter = make_adapter(a_vb, b_vb, cfg, linear_config)?;
+                adapters.insert(name.clone(), adapter);
+            }
         }
+
         let layer = *ordering.layers.get(&prefix).unwrap();
 
         if all_same {
             let a_adapters_stack = Tensor::cat(
                 &a_adapters
                     .iter()
                     .map(|x| x.weight().unsqueeze(0))
@@ -134,32 +135,88 @@
             .to_dtype(a_adapters_stack.dtype())?;
             let a_adapters_stack = a_adapters_stack.broadcast_mul(&scale_adapters_t)?;
             Ok(QLoraLinear {
                 old,
                 a_adapters: Either::Right((a_adapters_stack.clone(), a_adapters)),
                 b_adapters: Either::Right((b_adapters_stack.clone(), b_adapters)),
                 scale_adapters,
-                dropout_adapters,
                 layer_n: layer,
                 merged: false,
+                adapters,
+                linear_config: Some(linear_config.clone()),
             })
         } else {
             Ok(QLoraLinear {
                 old,
                 a_adapters: Either::Left(a_adapters),
                 b_adapters: Either::Left(b_adapters),
                 scale_adapters,
-                dropout_adapters,
                 layer_n: layer,
                 merged: false,
+                adapters,
+                linear_config: Some(linear_config.clone()),
             })
         }
     }
 }
 
+impl AdapterSwapper for QLoraLinear {
+    fn _activate_adapters(&mut self, adapter_names: &[String]) -> Result<()> {
+        match (
+            &mut self.a_adapters,
+            &mut self.b_adapters,
+            &mut self.scale_adapters,
+        ) {
+            (Either::Left(a), Either::Left(b), s) => {
+                a.clear();
+                b.clear();
+                s.clear();
+                for adapter_name in adapter_names {
+                    let Adapter {
+                        a: a_w,
+                        b: b_w,
+                        scale,
+                    } = match self.adapters.get(adapter_name) {
+                        Some(a) => a,
+                        None => bail!("Cannot load adapter `{adapter_name}`."),
+                    };
+                    a.push(a_w.clone());
+                    b.push(b_w.clone());
+                    s.push(*scale);
+                }
+            }
+            _ => unreachable!("Adapters should not be stacked if new ones are being activated."),
+        }
+        Ok(())
+    }
+    fn has_adapter(&self, adapter: String) -> bool {
+        self.adapters.contains_key(&adapter)
+    }
+    fn load_new_adapter(
+        &mut self,
+        name: String,
+        vb: VarBuilder,
+        cfg: &LoraConfig,
+        module_prefix: String,
+    ) -> Result<()> {
+        if let Some(ref linear_config) = self.linear_config {
+            let a_vb = vb.set_prefix(&module_prefix).pp("lora_A".to_string());
+            let b_vb = vb.set_prefix(&module_prefix).pp("lora_B".to_string());
+            let adapter = make_adapter(a_vb, b_vb, cfg, linear_config)?;
+            self.adapters.insert(name.clone(), adapter);
+            Ok(())
+        } else {
+            bail!("Linear config not found. This means that the layer cannot have new adapters loaded.")
+        }
+    }
+    fn can_load(&self) -> bool {
+        self.linear_config.is_some()
+    }
+}
+
 impl Merge for QLoraLinear {
     fn get_delta_weight(&self, adapter: usize) -> Result<Tensor> {
         match (&self.a_adapters, &self.b_adapters) {
             (Either::Left(a), Either::Left(b)) | (Either::Right((_, a)), Either::Right((_, b))) => {
                 let w_a = a[adapter].weight();
                 let w_b = b[adapter].weight();
 
@@ -205,80 +262,76 @@
         is_scaling_pass: Option<f64>,
     ) -> Result<Tensor> {
         //No fan_in_fan_out so no weight.transpose(0,1)
         let mut result = self.old.forward(input)?;
         if self.merged {
             return Ok(result);
         }
-        let scalings = scalings.unwrap();
 
         if self
             .a_adapters
             .as_ref()
             .left()
             .is_some_and(|x| x.is_empty())
             || (is_scaling_pass.is_some_and(|x| x == 0.))
         {
             return Ok(result);
         }
-        let scalings = get_maybe_topk_scalings(scalings, self.layer_n)?;
-        if self.a_adapters.is_left() || scalings.dims3()?.1 != 1 {
+
+        let scalings =
+            scalings.map(|scalings| get_maybe_topk_scalings(scalings, self.layer_n).unwrap());
+        if self.a_adapters.is_left()
+            || scalings
+                .as_ref()
+                .is_some_and(|scalings| scalings.dims3().unwrap().1 != 1)
+        {
             let a_adapters = if self.a_adapters.is_right() {
                 self.a_adapters.as_ref().unwrap_right().1.clone()
             } else {
                 self.a_adapters.as_ref().unwrap_left().clone()
             };
             let b_adapters = if self.b_adapters.is_right() {
                 self.b_adapters.as_ref().unwrap_right().1.clone()
             } else {
                 self.b_adapters.as_ref().unwrap_left().clone()
             };
-            for (i, (adapter_a, (adapter_b, (adapter_scale, adapter_dropout)))) in zip(
-                a_adapters,
-                zip(
-                    b_adapters,
-                    zip(&self.scale_adapters, self.dropout_adapters.iter()),
-                ),
-            )
-            .enumerate()
+            for (i, (adapter_a, (adapter_b, adapter_scale))) in
+                zip(a_adapters, zip(b_adapters, &self.scale_adapters)).enumerate()
             {
-                let mut input_new = apply_scalings_to_x(input.clone(), &scalings, i)?;
-
-                input_new = if let Some(ref dropout) = adapter_dropout {
-                    dropout.forward(&input_new, true)?
+                let input_new = if let Some(scalings) = &scalings {
+                    apply_scalings_to_x(input.clone(), scalings, i)?
                 } else {
-                    input_new.clone()
+                    input.clone()
                 };
+
                 let res = adapter_b
                     .forward(&adapter_a.forward(&input_new)?)?
                     .mul(*adapter_scale)?
                     .mul(global_scaling_weight)?;
                 result = (result + res)?;
             }
             Ok(result)
         } else {
             let adapter_a = &self.a_adapters.as_ref().unwrap_right().0;
             let adapter_b = &self.b_adapters.as_ref().unwrap_right().0;
             let adapter_scales = &self.scale_adapters;
             let n_adapters = adapter_scales.len();
-            let dropout = &self.dropout_adapters[0];
-            let scalings = scalings
-                .squeeze(0)?
-                .squeeze(0)?
-                .unsqueeze(1)?
-                .unsqueeze(1)?;
-            let adapter_a = adapter_a
-                .broadcast_mul(&scalings)?
-                .mul(global_scaling_weight)?;
-
-            let input = if let Some(ref d) = dropout {
-                d.forward(input, true)?
+            let adapter_a = if let Some(scalings) = scalings.as_ref() {
+                let scalings = scalings
+                    .squeeze(0)?
+                    .squeeze(0)?
+                    .unsqueeze(1)?
+                    .unsqueeze(1)?;
+                adapter_a
+                    .broadcast_mul(&scalings)?
+                    .mul(global_scaling_weight)?
             } else {
-                input.clone()
+                adapter_a.clone().mul(global_scaling_weight)?
             };
+
             let (b, s, h) = input.dims3()?;
             let input = input.reshape((b * s, h))?;
             let out = adapter_a.broadcast_matmul(&input.t()?)?;
             let out = adapter_b.broadcast_matmul(&out)?;
             let o_h = out.dims()[1];
             let out = out.reshape((n_adapters, b, s, o_h))?;
             let out = out.sum(0)?;
```

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/Cargo.toml` & `mistralrs-0.1.5/mistralrs-pyo3/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.4", path = "../mistralrs-core" }
+mistralrs-core = { version = "0.1.5", path = "../mistralrs-core" }
 serde.workspace = true
 serde_json.workspace = true
 candle-core.workspace = true
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
 futures.workspace = true
 tokio.workspace = true
 tracing-subscriber.workspace = true
 
+[build-dependencies]
+pyo3-build-config = "0.21"
+
 [features]
 cuda = ["candle-core/cuda", "mistralrs-core/cuda"]
 cudnn = ["candle-core/cudnn", "mistralrs-core/cudnn"]
 metal = ["candle-core/metal", "mistralrs-core/metal"]
 flash-attn = ["cuda", "mistralrs-core/flash-attn"]
 accelerate = ["mistralrs-core/accelerate"]
 mkl = ["mistralrs-core/mkl"]
```

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/.gitignore` & `mistralrs-0.1.5/mistralrs-pyo3/.gitignore`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/API.md` & `mistralrs-0.1.5/mistralrs-pyo3/API.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         model_id: str | None = None
         tokenizer_json: str | None = None
         repeat_last_n: int = 64
     class Lora:
         arch: Architecture
         adapters_model_id: str
         order: str
-        tgt_non_granular_index: int | None = None
         model_id: str | None = None
         tokenizer_json: str | None = None
         repeat_last_n: int = 64
     class GGUF:
         tok_model_id: str
         quantized_model_id: str
         quantized_filename: str
@@ -60,15 +59,14 @@
         repeat_last_n: int = 64
     class LoraGGUF:
         tok_model_id: str
         quantized_model_id: str
         quantized_filename: str
         adapters_model_id: str
         order: str
-        tgt_non_granular_index: int | None = None
         tokenizer_json: str | None = None
         repeat_last_n: int = 64
     class GGML:
         tok_model_id: str
         quantized_model_id: str
         quantized_filename: str
         tokenizer_json: str | None = None
@@ -84,15 +82,14 @@
         repeat_last_n: int = 64
     class LoraGGML:
         tok_model_id: str
         quantized_model_id: str
         quantized_filename: str
         adapters_model_id: str
         order: str
-        tgt_non_granular_index: int | None = None
         tokenizer_json: str | None = None
         repeat_last_n: int = 64
 ```
 
 
 ## Example
 ```python
```

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/Cargo_template.toml` & `mistralrs-0.1.5/mistralrs-pyo3/Cargo_template.toml`

 * *Files 19% similar despite different names*

```diff
@@ -13,17 +13,21 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.4", path = "../mistralrs-core", features=["$feature_name"] }
+mistralrs-core = { version = "0.1.5", path = "../mistralrs-core", features=["$feature_name"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["$feature_name"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
 futures.workspace = true
+tokio.workspace = true
 tracing-subscriber.workspace = true
+
+[build-dependencies]
+pyo3-build-config = "0.21"
```

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/README.md` & `mistralrs-0.1.5/mistralrs-pyo3/README.md`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/mistralrs.pyi` & `mistralrs-0.1.5/mistralrs-pyo3/mistralrs.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     stop_seqs: list[str] | None = None
     temperature: float | None = None
     top_p: float | None = None
     stream: bool = False
     top_k: int | None = None
     grammar: str | None = None
     grammar_type: str | None = None
+    adapters: list[str] | None = None
 
 @dataclass
 class CompletionRequest:
     """
     A CompletionRequest represents a request sent to the mistral.rs engine. It encodes information
     about input data, sampling, and how to return the response.
     """
@@ -45,14 +46,15 @@
     stop_seqs: list[str] | None = None
     temperature: float | None = None
     top_p: float | None = None
     top_k: int | None = None
     suffix: str | None = None
     grammar: str | None = None
     grammar_type: str | None = None
+    adapters: list[str] | None = None
 
 @dataclass
 class Architecture(Enum):
     Mistral = "mistral"
     Gemma = "gemma"
     Mixtral = "mixtral"
     Llama = "llama"
@@ -82,15 +84,14 @@
         tokenizer_json: str | None = None
         repeat_last_n: int = 64
     @dataclass
     class Lora:
         arch: Architecture
         adapters_model_id: str
         order: str
-        tgt_non_granular_index: int | None = None
         model_id: str | None = None
         tokenizer_json: str | None = None
         repeat_last_n: int = 64
     @dataclass
     class GGUF:
         tok_model_id: str
         quantized_model_id: str
@@ -110,15 +111,14 @@
     @dataclass
     class LoraGGUF:
         tok_model_id: str
         quantized_model_id: str
         quantized_filename: str
         adapters_model_id: str
         order: str
-        tgt_non_granular_index: int | None = None
         tokenizer_json: str | None = None
         repeat_last_n: int = 64
     @dataclass
     class GGML:
         tok_model_id: str
         quantized_model_id: str
         quantized_filename: str
@@ -137,39 +137,44 @@
     @dataclass
     class LoraGGML:
         tok_model_id: str
         quantized_model_id: str
         quantized_filename: str
         adapters_model_id: str
         order: str
-        tgt_non_granular_index: int | None = None
         tokenizer_json: str | None = None
         repeat_last_n: int = 64
 
 class Runner:
     def __init__(
         self,
         which: Which,
         max_seqs: int = 16,
         no_kv_cache: bool = False,
         prefix_cache_n: int = 16,
         token_source: str = "cache",
+        speculative_gamma: int = 32,
+        which_draft: Which | None = None,
         chat_template: str | None = None,
         num_device_layers: int | None = None,
         in_situ_quant: str | None = None,
     ) -> None:
         """
         Load a model.
 
-        - `which` specified which model to load.
+        - `which` specifies which model to load or the target model to load in the case of speculative decoding.
         - `max_seqs` specifies how many sequences may be running at any time.
         - `no_kv_cache` disables the KV cache.
         - `prefix_cache_n` sets the number of sequences to hold in the device prefix cache, others will be evicted to CPU.
         - `token_source` specifies where to load the HF token from.
             The token source follows the following format: "literal:<value>", "env:<value>", "path:<value>", "cache" to use a cached token or "none" to use no token.
+        - `speculative_gamma` specifies the `gamma` parameter for specuative decoding, the ratio of draft tokens to generate before calling
+            the target model. If `which_draft` is not specified, this is ignored.
+        - `which_draft` specifies which draft model to load. Setting this parameter will cause a speculative decoding model to be loaded,
+            with `which` as the target (higher quality) model and `which_draft` as the draft (lower quality) model.
         - `chat_template` specifies an optional JINJA chat template.
             The JINJA template should have `messages`, `add_generation_prompt`, `bos_token`, `eos_token`, and `unk_token` as inputs.
             It is used if the automatic deserialization fails. If this ends with `.json` (ie., it is a file) then that template is loaded.
         - `num_device_layers` sets the number of layers to load and run on the device.
         - `in_situ_quant` sets the optional in-situ quantization for models that are not quantized (not GGUF or GGML).
         """
         ...
@@ -188,14 +193,19 @@
         """
 
     def send_re_isq(self, dtype: str) -> CompletionResponse:
         """
         Send a request to re-ISQ the model. If the model was loaded as GGUF or GGML then nothing will happen.
         """
 
+    def activate_adapters(self, adapter_names: list[str]) -> None:
+        """
+        Send a request to make the specified adapters the active adapters for the model.
+        """
+
 @dataclass
 class Usage:
     completion_tokens: int
     prompt_tokens: int
     total_tokens: int
     avg_tok_per_sec: float
     avg_prompt_tok_per_sec: float
```

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/pyproject_template.toml` & `mistralrs-0.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
-name = "$name"
-version = "0.1.4"
+name = "mistralrs"
+version = "0.1.5"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Rust",
 ]
 dynamic = ["description"]
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
+manifest-path = "mistralrs-pyo3/Cargo.toml"
```

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/src/lib.rs` & `mistralrs-0.1.5/mistralrs-pyo3/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 use tokio::sync::mpsc::channel;
 use tracing_subscriber::{filter::LevelFilter, EnvFilter};
 
 use candle_core::Device;
 use mistralrs_core::{
     ChatCompletionResponse, CompletionResponse, Constraint, DeviceMapMetadata, GGMLLoaderBuilder,
     GGMLSpecificConfig, GGUFLoaderBuilder, GGUFSpecificConfig, Loader, MistralRs, MistralRsBuilder,
-    NormalLoaderBuilder, NormalSpecificConfig, Request as _Request, RequestMessage, Response,
-    SamplingParams, SchedulerMethod, StopTokens, TokenSource,
+    NormalLoaderBuilder, NormalRequest, NormalSpecificConfig, Request as _Request, RequestMessage,
+    Response, SamplingParams, SchedulerMethod, SpeculativeConfig, SpeculativeLoader, StopTokens,
+    TokenSource,
 };
 use pyo3::{
     exceptions::{PyTypeError, PyValueError},
     prelude::*,
     types::{PyList, PyString},
 };
 use std::fs::File;
@@ -79,45 +80,280 @@
 /// An object wrapping the underlying Rust system to handle requests and process conversations.
 struct Runner {
     runner: Arc<MistralRs>,
 }
 
 static NEXT_REQUEST_ID: Mutex<RefCell<usize>> = Mutex::new(RefCell::new(0));
 
+fn parse_which(
+    which: Which,
+    no_kv_cache: bool,
+    chat_template: Option<String>,
+) -> PyResult<Box<dyn Loader>> {
+    const REPEAT_LAST_N_DEFAULT: usize = 64;
+    const GQA_DEFAULT: usize = 1;
+
+    #[cfg(not(feature = "flash-attn"))]
+    let use_flash_attn = false;
+    #[cfg(feature = "flash-attn")]
+    let use_flash_attn = true;
+
+    Ok(match which {
+        Which::Plain {
+            model_id,
+            repeat_last_n,
+            tokenizer_json,
+            arch,
+        } => NormalLoaderBuilder::new(
+            NormalSpecificConfig {
+                use_flash_attn,
+                repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
+            },
+            chat_template,
+            tokenizer_json,
+            Some(model_id),
+        )
+        .build(arch.into()),
+        Which::XLora {
+            model_id,
+            xlora_model_id,
+            repeat_last_n,
+            order,
+            tokenizer_json,
+            tgt_non_granular_index,
+            arch,
+        } => NormalLoaderBuilder::new(
+            NormalSpecificConfig {
+                use_flash_attn,
+                repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
+            },
+            chat_template,
+            tokenizer_json,
+            model_id,
+        )
+        .with_xlora(
+            xlora_model_id,
+            serde_json::from_reader(
+                File::open(order.clone())
+                    .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
+            )
+            .map_err(|e| PyValueError::new_err(e.to_string()))?,
+            no_kv_cache,
+            tgt_non_granular_index,
+        )
+        .build(arch.into()),
+        Which::Lora {
+            model_id,
+            tokenizer_json,
+            adapters_model_id,
+            repeat_last_n,
+            order,
+            arch,
+        } => NormalLoaderBuilder::new(
+            NormalSpecificConfig {
+                use_flash_attn,
+                repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
+            },
+            chat_template,
+            tokenizer_json,
+            model_id,
+        )
+        .with_lora(
+            adapters_model_id,
+            serde_json::from_reader(
+                File::open(order.clone())
+                    .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
+            )
+            .map_err(|e| PyValueError::new_err(e.to_string()))?,
+        )
+        .build(arch.into()),
+        Which::GGUF {
+            tok_model_id,
+            tokenizer_json,
+            quantized_model_id,
+            quantized_filename,
+            repeat_last_n,
+        } => GGUFLoaderBuilder::new(
+            GGUFSpecificConfig {
+                repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
+            },
+            chat_template,
+            tokenizer_json,
+            Some(tok_model_id),
+            quantized_model_id,
+            quantized_filename,
+        )
+        .build(),
+        Which::XLoraGGUF {
+            tok_model_id,
+            tokenizer_json,
+            quantized_model_id,
+            quantized_filename,
+            repeat_last_n,
+            xlora_model_id,
+            order,
+            tgt_non_granular_index,
+        } => GGUFLoaderBuilder::new(
+            GGUFSpecificConfig {
+                repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
+            },
+            chat_template,
+            tokenizer_json,
+            tok_model_id,
+            quantized_model_id,
+            quantized_filename,
+        )
+        .with_xlora(
+            xlora_model_id,
+            serde_json::from_reader(
+                File::open(order.clone())
+                    .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
+            )
+            .map_err(|e| PyValueError::new_err(e.to_string()))?,
+            no_kv_cache,
+            tgt_non_granular_index,
+        )
+        .build(),
+        Which::LoraGGUF {
+            tok_model_id,
+            tokenizer_json,
+            quantized_model_id,
+            quantized_filename,
+            repeat_last_n,
+            adapters_model_id,
+            order,
+        } => GGUFLoaderBuilder::new(
+            GGUFSpecificConfig {
+                repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
+            },
+            chat_template,
+            tokenizer_json,
+            tok_model_id,
+            quantized_model_id,
+            quantized_filename,
+        )
+        .with_lora(
+            adapters_model_id,
+            serde_json::from_reader(
+                File::open(order.clone())
+                    .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
+            )
+            .map_err(|e| PyValueError::new_err(e.to_string()))?,
+        )
+        .build(),
+        Which::GGML {
+            tok_model_id,
+            tokenizer_json,
+            quantized_model_id,
+            quantized_filename,
+            repeat_last_n,
+            gqa,
+        } => GGMLLoaderBuilder::new(
+            GGMLSpecificConfig {
+                repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
+                gqa: gqa.unwrap_or(GQA_DEFAULT),
+            },
+            chat_template,
+            tokenizer_json,
+            Some(tok_model_id),
+            quantized_model_id,
+            quantized_filename,
+        )
+        .build(),
+        Which::XLoraGGML {
+            tok_model_id,
+            tokenizer_json,
+            quantized_model_id,
+            quantized_filename,
+            repeat_last_n,
+            xlora_model_id,
+            order,
+            tgt_non_granular_index,
+            gqa,
+        } => GGMLLoaderBuilder::new(
+            GGMLSpecificConfig {
+                repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
+                gqa: gqa.unwrap_or(GQA_DEFAULT),
+            },
+            chat_template,
+            tokenizer_json,
+            tok_model_id,
+            quantized_model_id,
+            quantized_filename,
+        )
+        .with_xlora(
+            xlora_model_id,
+            serde_json::from_reader(
+                File::open(order.clone())
+                    .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
+            )
+            .map_err(|e| PyValueError::new_err(e.to_string()))?,
+            no_kv_cache,
+            tgt_non_granular_index,
+        )
+        .build(),
+        Which::LoraGGML {
+            tok_model_id,
+            tokenizer_json,
+            quantized_model_id,
+            quantized_filename,
+            repeat_last_n,
+            adapters_model_id,
+            order,
+            gqa,
+        } => GGMLLoaderBuilder::new(
+            GGMLSpecificConfig {
+                repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
+                gqa: gqa.unwrap_or(GQA_DEFAULT),
+            },
+            chat_template,
+            tokenizer_json,
+            tok_model_id,
+            quantized_model_id,
+            quantized_filename,
+        )
+        .with_lora(
+            adapters_model_id,
+            serde_json::from_reader(
+                File::open(order.clone())
+                    .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
+            )
+            .map_err(|e| PyValueError::new_err(e.to_string()))?,
+        )
+        .build(),
+    })
+}
+
 #[pymethods]
 impl Runner {
     #[new]
     #[pyo3(signature = (
         which,
         max_seqs = 16,
         no_kv_cache = false,
         prefix_cache_n = 16,
         token_source = "cache",
+        speculative_gamma = 32,
+        which_draft = None,
         chat_template = None,
         num_device_layers = None,
         in_situ_quant = None
     ))]
     fn new(
         which: Which,
         max_seqs: usize,
         no_kv_cache: bool,
         prefix_cache_n: usize,
         token_source: &str,
+        speculative_gamma: usize,
+        which_draft: Option<Which>,
         chat_template: Option<String>,
         num_device_layers: Option<usize>,
         in_situ_quant: Option<String>,
     ) -> PyResult<Self> {
-        const REPEAT_LAST_N_DEFAULT: usize = 64;
-        const GQA_DEFAULT: usize = 1;
-
-        #[cfg(not(feature = "flash-attn"))]
-        let use_flash_attn = false;
-        #[cfg(feature = "flash-attn")]
-        let use_flash_attn = true;
-
         let tgt_non_granular_index = match which {
             Which::Plain { .. }
             | Which::Lora { .. }
             | Which::GGUF { .. }
             | Which::LoraGGUF { .. }
             | Which::GGML { .. }
             | Which::LoraGGML { .. } => None,
@@ -136,245 +372,26 @@
         };
         let max_seqs = if tgt_non_granular_index.is_some() {
             1
         } else {
             max_seqs
         };
 
-        let loader: Box<dyn Loader> = match which {
-            Which::Plain {
-                model_id,
-                repeat_last_n,
-                tokenizer_json,
-                arch,
-            } => NormalLoaderBuilder::new(
-                NormalSpecificConfig {
-                    use_flash_attn,
-                    repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
-                },
-                chat_template,
-                tokenizer_json,
-                Some(model_id),
-            )
-            .build(arch.into()),
-            Which::XLora {
-                model_id,
-                xlora_model_id,
-                repeat_last_n,
-                order,
-                tokenizer_json,
-                tgt_non_granular_index,
-                arch,
-            } => NormalLoaderBuilder::new(
-                NormalSpecificConfig {
-                    use_flash_attn,
-                    repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
-                },
-                chat_template,
-                tokenizer_json,
-                model_id,
-            )
-            .with_xlora(
-                xlora_model_id,
-                serde_json::from_reader(
-                    File::open(order.clone())
-                        .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
-                )
-                .map_err(|e| PyValueError::new_err(e.to_string()))?,
-                no_kv_cache,
-                tgt_non_granular_index,
-            )
-            .build(arch.into()),
-            Which::Lora {
-                model_id,
-                tokenizer_json,
-                adapters_model_id,
-                repeat_last_n,
-                order,
-                arch,
-            } => NormalLoaderBuilder::new(
-                NormalSpecificConfig {
-                    use_flash_attn,
-                    repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
-                },
-                chat_template,
-                tokenizer_json,
-                model_id,
-            )
-            .with_xlora(
-                adapters_model_id,
-                serde_json::from_reader(
-                    File::open(order.clone())
-                        .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
-                )
-                .map_err(|e| PyValueError::new_err(e.to_string()))?,
-                no_kv_cache,
-                tgt_non_granular_index,
-            )
-            .build(arch.into()),
-            Which::GGUF {
-                tok_model_id,
-                tokenizer_json,
-                quantized_model_id,
-                quantized_filename,
-                repeat_last_n,
-            } => GGUFLoaderBuilder::new(
-                GGUFSpecificConfig {
-                    repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
-                },
-                chat_template,
-                tokenizer_json,
-                Some(tok_model_id),
-                quantized_model_id,
-                quantized_filename,
-            )
-            .build(),
-            Which::XLoraGGUF {
-                tok_model_id,
-                tokenizer_json,
-                quantized_model_id,
-                quantized_filename,
-                repeat_last_n,
-                xlora_model_id,
-                order,
-                tgt_non_granular_index,
-            } => GGUFLoaderBuilder::new(
-                GGUFSpecificConfig {
-                    repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
-                },
-                chat_template,
-                tokenizer_json,
-                tok_model_id,
-                quantized_model_id,
-                quantized_filename,
-            )
-            .with_xlora(
-                xlora_model_id,
-                serde_json::from_reader(
-                    File::open(order.clone())
-                        .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
-                )
-                .map_err(|e| PyValueError::new_err(e.to_string()))?,
-                no_kv_cache,
-                tgt_non_granular_index,
-            )
-            .build(),
-            Which::LoraGGUF {
-                tok_model_id,
-                tokenizer_json,
-                quantized_model_id,
-                quantized_filename,
-                repeat_last_n,
-                adapters_model_id,
-                order,
-                tgt_non_granular_index,
-            } => GGUFLoaderBuilder::new(
-                GGUFSpecificConfig {
-                    repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
-                },
-                chat_template,
-                tokenizer_json,
-                tok_model_id,
-                quantized_model_id,
-                quantized_filename,
-            )
-            .with_lora(
-                adapters_model_id,
-                serde_json::from_reader(
-                    File::open(order.clone())
-                        .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
-                )
-                .map_err(|e| PyValueError::new_err(e.to_string()))?,
-                no_kv_cache,
-                tgt_non_granular_index,
-            )
-            .build(),
-            Which::GGML {
-                tok_model_id,
-                tokenizer_json,
-                quantized_model_id,
-                quantized_filename,
-                repeat_last_n,
-                gqa,
-            } => GGMLLoaderBuilder::new(
-                GGMLSpecificConfig {
-                    repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
-                    gqa: gqa.unwrap_or(GQA_DEFAULT),
+        let loader = parse_which(which, no_kv_cache, chat_template.clone())?;
+        let loader = if let Some(draft_which) = which_draft {
+            let draft = parse_which(draft_which, no_kv_cache, chat_template)?;
+            Box::new(SpeculativeLoader {
+                target: loader,
+                draft,
+                config: SpeculativeConfig {
+                    gamma: speculative_gamma,
                 },
-                chat_template,
-                tokenizer_json,
-                Some(tok_model_id),
-                quantized_model_id,
-                quantized_filename,
-            )
-            .build(),
-            Which::XLoraGGML {
-                tok_model_id,
-                tokenizer_json,
-                quantized_model_id,
-                quantized_filename,
-                repeat_last_n,
-                xlora_model_id,
-                order,
-                tgt_non_granular_index,
-                gqa,
-            } => GGMLLoaderBuilder::new(
-                GGMLSpecificConfig {
-                    repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
-                    gqa: gqa.unwrap_or(GQA_DEFAULT),
-                },
-                chat_template,
-                tokenizer_json,
-                tok_model_id,
-                quantized_model_id,
-                quantized_filename,
-            )
-            .with_xlora(
-                xlora_model_id,
-                serde_json::from_reader(
-                    File::open(order.clone())
-                        .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
-                )
-                .map_err(|e| PyValueError::new_err(e.to_string()))?,
-                no_kv_cache,
-                tgt_non_granular_index,
-            )
-            .build(),
-            Which::LoraGGML {
-                tok_model_id,
-                tokenizer_json,
-                quantized_model_id,
-                quantized_filename,
-                repeat_last_n,
-                adapters_model_id,
-                order,
-                tgt_non_granular_index,
-                gqa,
-            } => GGMLLoaderBuilder::new(
-                GGMLSpecificConfig {
-                    repeat_last_n: repeat_last_n.unwrap_or(REPEAT_LAST_N_DEFAULT),
-                    gqa: gqa.unwrap_or(GQA_DEFAULT),
-                },
-                chat_template,
-                tokenizer_json,
-                tok_model_id,
-                quantized_model_id,
-                quantized_filename,
-            )
-            .with_lora(
-                adapters_model_id,
-                serde_json::from_reader(
-                    File::open(order.clone())
-                        .unwrap_or_else(|_| panic!("Could not load ordering file at {order}")),
-                )
-                .map_err(|e| PyValueError::new_err(e.to_string()))?,
-                no_kv_cache,
-                tgt_non_granular_index,
-            )
-            .build(),
+            })
+        } else {
+            loader
         };
 
         let device = get_device().map_err(|e| PyValueError::new_err(e.to_string()))?;
         let isq = if let Some(isq) = in_situ_quant {
             Some(parse_isq(&isq).map_err(|e| PyValueError::new_err(e.to_string()))?)
         } else {
             None
@@ -438,15 +455,15 @@
             } else if request.grammar_type.is_some() {
                 return Err(PyValueError::new_err(
                     "Grammar type is specified but is not `regex` or `yacc`",
                 ));
             } else {
                 Constraint::None
             };
-            let model_request = _Request {
+            let model_request = _Request::Normal(NormalRequest {
                 id: {
                     let l = NEXT_REQUEST_ID.lock().unwrap();
                     let last = &mut *l.borrow_mut();
                     let last_v = *last;
                     *last += 1;
                     last_v
                 },
@@ -490,15 +507,16 @@
                     n_choices: request.n_choices,
                 },
                 response: tx,
                 return_logprobs: request.logprobs,
                 is_streaming: request.stream,
                 constraint,
                 suffix: None,
-            };
+                adapters: request.adapters.clone(),
+            });
 
             MistralRs::maybe_log_request(self.runner.clone(), format!("{request:?}"));
             let sender = self.runner.get_sender();
             sender.blocking_send(model_request).unwrap();
 
             if request.stream {
                 Ok(Either::Right(ChatCompletionStreamer::from_rx(rx)))
@@ -548,15 +566,15 @@
             } else if request.grammar_type.is_some() {
                 return Err(PyValueError::new_err(
                     "Grammar type is specified but is not `regex` or `yacc`",
                 ));
             } else {
                 Constraint::None
             };
-            let model_request = _Request {
+            let model_request = _Request::Normal(NormalRequest {
                 id: {
                     let l = NEXT_REQUEST_ID.lock().unwrap();
                     let last = &mut *l.borrow_mut();
                     let last_v = *last;
                     *last += 1;
                     last_v
                 },
@@ -578,15 +596,16 @@
                     n_choices: request.n_choices,
                 },
                 response: tx,
                 return_logprobs: false,
                 is_streaming: false,
                 constraint,
                 suffix: request.suffix.clone(),
-            };
+                adapters: request.adapters.clone(),
+            });
 
             MistralRs::maybe_log_request(self.runner.clone(), format!("{request:?}"));
             let sender = self.runner.get_sender();
             sender.blocking_send(model_request).unwrap();
             let response = rx.blocking_recv().unwrap();
 
             match response {
@@ -603,18 +622,25 @@
             }
         })
     }
 
     /// Send a request to re-ISQ the model. If the model was loaded as GGUF or GGML
     /// then nothing will happen.
     fn send_re_isq(&self, dtype: String) -> PyResult<()> {
-        self.runner
-            .send_re_isq(parse_isq(&dtype).map_err(|e| PyValueError::new_err(e.to_string()))?);
+        let request =
+            _Request::ReIsq(parse_isq(&dtype).map_err(|e| PyValueError::new_err(e.to_string()))?);
+        self.runner.get_sender().blocking_send(request).unwrap();
         Ok(())
     }
+
+    /// Send a request to make the specified adapters the active adapters for the model.
+    fn activate_adapters(&self, adapter_names: Vec<String>) {
+        let request = _Request::ActivateAdapters(adapter_names);
+        self.runner.get_sender().blocking_send(request).unwrap();
+    }
 }
 
 #[pyclass]
 #[derive(Debug)]
 /// An OpenAI API compatible completion request.
 struct CompletionRequest {
     _model: String,
@@ -629,14 +655,15 @@
     stop_seqs: Option<Vec<String>>,
     temperature: Option<f64>,
     top_p: Option<f64>,
     suffix: Option<String>,
     top_k: Option<usize>,
     grammar: Option<String>,
     grammar_type: Option<String>,
+    adapters: Option<Vec<String>>,
 }
 
 #[pymethods]
 impl CompletionRequest {
     #[new]
     #[pyo3(signature = (
         prompt,
@@ -650,15 +677,16 @@
         n_choices=1,
         stop_seqs=None,
         temperature=None,
         top_p=None,
         suffix=None,
         top_k=None,
         grammar = None,
-        grammar_type = None
+        grammar_type = None,
+        adapters = None
     ))]
     fn new(
         prompt: String,
         model: String,
         best_of: usize,
         echo_prompt: bool,
         presence_penalty: Option<f32>,
@@ -669,14 +697,15 @@
         stop_seqs: Option<Vec<String>>,
         temperature: Option<f64>,
         top_p: Option<f64>,
         suffix: Option<String>,
         top_k: Option<usize>,
         grammar: Option<String>,
         grammar_type: Option<String>,
+        adapters: Option<Vec<String>>,
     ) -> PyResult<Self> {
         Ok(Self {
             prompt,
             best_of,
             echo_prompt,
             suffix,
             _model: model,
@@ -687,14 +716,15 @@
             frequency_penalty,
             stop_seqs,
             temperature,
             top_p,
             top_k,
             grammar,
             grammar_type,
+            adapters,
         })
     }
 }
 
 #[pyclass]
 #[derive(Debug)]
 /// An OpenAI API compatible chat completion request.
@@ -711,14 +741,15 @@
     stop_seqs: Option<Vec<String>>,
     temperature: Option<f64>,
     top_p: Option<f64>,
     stream: bool,
     top_k: Option<usize>,
     grammar: Option<String>,
     grammar_type: Option<String>,
+    adapters: Option<Vec<String>>,
 }
 
 #[pymethods]
 impl ChatCompletionRequest {
     #[new]
     #[pyo3(signature = (
         messages,
@@ -732,15 +763,16 @@
         frequency_penalty = None,
         stop_seqs = None,
         temperature = None,
         top_p = None,
         top_k = None,
         stream=false,
         grammar = None,
-        grammar_type = None
+        grammar_type = None,
+        adapters = None
     ))]
     fn new(
         messages: Py<PyAny>,
         model: String,
         logprobs: bool,
         n_choices: usize,
         logit_bias: Option<HashMap<u32, f32>>,
@@ -751,14 +783,15 @@
         stop_seqs: Option<Vec<String>>,
         temperature: Option<f64>,
         top_p: Option<f64>,
         top_k: Option<usize>,
         stream: Option<bool>,
         grammar: Option<String>,
         grammar_type: Option<String>,
+        adapters: Option<Vec<String>>,
     ) -> PyResult<Self> {
         let messages = Python::with_gil(|py| {
             if let Ok(messages) = messages.bind(py).downcast_exact::<PyList>() {
                 let mut messages_vec = Vec::new();
                 for message in messages {
                     messages_vec.push(message.extract::<IndexMap<String, String>>()?);
                 }
@@ -785,14 +818,15 @@
             stop_seqs,
             temperature,
             top_p,
             top_k,
             stream: stream.unwrap_or(false),
             grammar,
             grammar_type,
+            adapters,
         })
     }
 }
 
 #[pymodule]
 fn mistralrs(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     let filter = EnvFilter::builder()
```

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/src/stream.rs` & `mistralrs-0.1.5/mistralrs-pyo3/src/stream.rs`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/src/which.rs` & `mistralrs-0.1.5/mistralrs-pyo3/src/which.rs`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         tok_model_id: Option<String>,
         tokenizer_json: Option<String>,
         quantized_model_id: String,
         quantized_filename: String,
         repeat_last_n: Option<usize>,
         adapters_model_id: String,
         order: String,
-        tgt_non_granular_index: Option<usize>,
     },
 
     #[allow(clippy::upper_case_acronyms)]
     GGML {
         tok_model_id: String,
         tokenizer_json: Option<String>,
         quantized_model_id: String,
@@ -111,11 +110,10 @@
         tok_model_id: Option<String>,
         tokenizer_json: Option<String>,
         quantized_model_id: String,
         quantized_filename: String,
         repeat_last_n: Option<usize>,
         adapters_model_id: String,
         order: String,
-        tgt_non_granular_index: Option<usize>,
         gqa: Option<usize>,
     },
 }
```

### Comparing `mistralrs-0.1.4/mistralrs-pyo3/upload.py` & `mistralrs-0.1.5/mistralrs-pyo3/upload.py`

 * *Files identical despite different names*

### Comparing `mistralrs-0.1.4/Cargo.lock` & `mistralrs-0.1.5/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
@@ -315,15 +315,15 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -332,16 +332,16 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "candle-core"
-version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
+version = "0.5.1"
+source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
 dependencies = [
  "accelerate-src",
  "byteorder",
  "candle-kernels",
  "candle-metal-kernels",
  "cudarc",
  "gemm",
@@ -354,63 +354,63 @@
  "num_cpus",
  "rand",
  "rand_distr",
  "rayon",
  "safetensors",
  "thiserror",
  "yoke",
- "zip 1.2.1",
+ "zip 1.2.3",
 ]
 
 [[package]]
 name = "candle-flash-attn"
-version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
+version = "0.5.1"
+source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
 dependencies = [
  "anyhow",
  "bindgen_cuda",
  "candle-core",
  "half",
 ]
 
 [[package]]
 name = "candle-kernels"
-version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
+version = "0.5.1"
+source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
 dependencies = [
  "bindgen_cuda",
 ]
 
 [[package]]
 name = "candle-layer-norm"
 version = "0.0.1"
-source = "git+https://github.com/EricLBuehler/candle-layer-norm.git#51a97e007f82644ad8efa87242007ad959a9b045"
+source = "git+https://github.com/EricLBuehler/candle-layer-norm.git#8001f04b14aa6da01d2cf2c4a4141f0b93b8d24c"
 dependencies = [
  "anyhow",
  "candle-core",
  "half",
  "num_cpus",
  "rayon",
 ]
 
 [[package]]
 name = "candle-metal-kernels"
-version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
+version = "0.5.1"
+source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
 dependencies = [
  "metal",
  "once_cell",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "candle-nn"
-version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
+version = "0.5.1"
+source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "candle-layer-norm",
  "candle-metal-kernels",
  "half",
  "intel-mkl-src",
@@ -420,16 +420,16 @@
  "safetensors",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "candle-transformers"
-version = "0.5.0"
-source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
+version = "0.5.1"
+source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
 dependencies = [
  "accelerate-src",
  "byteorder",
  "candle-core",
  "candle-flash-attn",
  "candle-nn",
  "fancy-regex",
@@ -532,15 +532,15 @@
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -717,19 +717,20 @@
 checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "cudarc"
-version = "0.10.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9395df0cab995685664e79cc35ad6302bf08fb9c5d82301875a183affe1278b1"
+checksum = "c415f24c56f0bd4e0568e3ceea0bae6e5a1a96bda8ac177d0b6d7fcc7fa8de7a"
 dependencies = [
  "half",
+ "libloading",
 ]
 
 [[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
@@ -769,15 +770,15 @@
 checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim 0.10.0",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
@@ -791,15 +792,15 @@
 name = "darling_macro"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core 0.20.8",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "defmac"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aafbece59594ed57696a1a69e8bb3ca1683fbc9cdb41d5c02726070b2cd8f19d"
@@ -808,15 +809,15 @@
 name = "derive_arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67e77553c4162a157adbf834ebae5b415acbecbeafc7a74b0e886657506a7611"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "derive_builder"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d67778784b508018359cbc8696edb3db78160bab2c2a28ba7f56ef6932997f8"
@@ -850,15 +851,15 @@
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
  "darling 0.20.8",
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "derive_builder_macro"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ebcda35c7a396850a55ffeac740804b40ffec779b98fffbb1738f4033f0ee79e"
@@ -870,15 +871,15 @@
 [[package]]
 name = "derive_builder_macro"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
 dependencies = [
  "derive_builder_core 0.20.0",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
@@ -921,15 +922,15 @@
 name = "displaydoc"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "dyn-fmt"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79ef34f092abc832595d6e7b81a416403243ab94cc4c8262608aa4fddc95209a"
@@ -970,28 +971,28 @@
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ffccbb6966c05b32ef8fbac435df276c4ae4d3dc55a8cd0eb9745e6c12f546a"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "esaxx-rs"
@@ -1080,15 +1081,15 @@
 name = "foreign-types-macros"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a5c6c585bc94aaf2c7b51dd4c2ba22680844aba4c687be581871a6f518c5742"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
@@ -1160,15 +1161,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1665,14 +1666,24 @@
 [[package]]
 name = "libc"
 version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
+name = "libloading"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
+dependencies = [
+ "cfg-if",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "libredox"
@@ -1849,25 +1860,26 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mistralrs"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "anyhow",
  "candle-core",
  "mistralrs-core",
+ "serde_json",
  "tokio",
 ]
 
 [[package]]
 name = "mistralrs-bench"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "anyhow",
  "candle-core",
  "clap",
  "cli-table",
  "either",
  "mistralrs-core",
@@ -1876,15 +1888,15 @@
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-core"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "async-trait",
  "bytemuck",
  "candle-core",
  "candle-flash-attn",
@@ -1901,67 +1913,70 @@
  "hf-hub",
  "indexmap",
  "indicatif",
  "intel-mkl-src",
  "lrtable",
  "minijinja",
  "mistralrs-lora",
+ "once_cell",
  "pyo3",
  "radix_trie",
  "rand",
  "rand_isaac",
  "range-checked",
  "rayon",
  "regex-automata 0.4.6",
  "rustc-hash",
  "serde",
  "serde_json",
  "thiserror",
  "tokenizers",
  "tokio",
  "tokio-rayon",
+ "toml",
  "tqdm",
  "tracing",
  "vob",
 ]
 
 [[package]]
 name = "mistralrs-lora"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "candle-nn",
  "either",
  "intel-mkl-src",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "mistralrs-pyo3"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "either",
  "futures",
  "indexmap",
  "intel-mkl-src",
  "mistralrs-core",
  "pyo3",
+ "pyo3-build-config",
  "serde",
  "serde_json",
  "tokio",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-server"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "axum",
  "candle-core",
  "clap",
  "dyn-fmt",
@@ -1994,15 +2009,15 @@
 name = "monostate-impl"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a7ce64b975ed4f123575d11afd9491f2e37bbd5813fbfbc0f09ae1fbddea74e0"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
@@ -2094,35 +2109,14 @@
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
-name = "num_enum"
-version = "0.7.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02339744ee7253741199f897151b38e72257d13802d4ee837285cc2990a90845"
-dependencies = [
- "num_enum_derive",
-]
-
-[[package]]
-name = "num_enum_derive"
-version = "0.7.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
-dependencies = [
- "proc-macro-crate",
- "proc-macro2",
- "quote",
- "syn 2.0.61",
-]
-
-[[package]]
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
 name = "objc"
@@ -2239,15 +2233,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -2381,15 +2375,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -2415,23 +2409,14 @@
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
-name = "proc-macro-crate"
-version = "3.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
-dependencies = [
- "toml_edit 0.21.1",
-]
-
-[[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
@@ -2527,28 +2512,28 @@
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -2752,41 +2737,41 @@
  "spin",
  "untrusted",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rust-embed"
-version = "8.3.0"
+version = "8.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb78f46d0066053d16d4ca7b898e9343bc3530f71c61d5ad84cd404ada068745"
+checksum = "19549741604902eb99a7ed0ee177a0663ee1eda51a29f71401f166e47e77806a"
 dependencies = [
  "rust-embed-impl",
  "rust-embed-utils",
  "walkdir",
 ]
 
 [[package]]
 name = "rust-embed-impl"
-version = "8.3.0"
+version = "8.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b91ac2a3c6c0520a3fb3dd89321177c3c692937c4eb21893378219da10c44fc8"
+checksum = "cb9f96e283ec64401f30d3df8ee2aaeb2561f34c824381efa24a35f79bf40ee4"
 dependencies = [
  "proc-macro2",
  "quote",
  "rust-embed-utils",
- "syn 2.0.61",
+ "syn 2.0.63",
  "walkdir",
 ]
 
 [[package]]
 name = "rust-embed-utils"
-version = "8.3.0"
+version = "8.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f69089032567ffff4eada41c573fc43ff466c7db7c5688b2e7969584345581"
+checksum = "38c74a686185620830701348de757fd36bef4aa9680fd23c49fc539ddcc1af32"
 dependencies = [
  "sha2",
  "walkdir",
 ]
 
 [[package]]
 name = "rust_decimal"
@@ -2957,15 +2942,15 @@
 name = "serde_derive"
 version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
@@ -3159,17 +3144,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.61"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3188,15 +3173,15 @@
 name = "synstructure"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8af7666ab7b6390ab78131fb5b0fce11d6b7a6951602017c35fa82800708971"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "sysctl"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec7dddc5f0fee506baf8b9fdb989e242f17e4b11c61dfbb0635b705217199eea"
@@ -3260,15 +3245,15 @@
 name = "thiserror-impl"
 version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
@@ -3328,32 +3313,35 @@
 [[package]]
 name = "tokio"
 version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
+ "bytes",
  "libc",
  "mio",
  "num_cpus",
+ "parking_lot",
  "pin-project-lite",
+ "signal-hook-registry",
  "socket2",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "tokio-rayon"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7cf33a76e0b1dd03b778f83244137bd59887abf25c0e87bc3e7071105f457693"
@@ -3367,48 +3355,37 @@
 version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
- "toml_edit 0.22.12",
+ "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.21.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
-dependencies = [
- "indexmap",
- "toml_datetime",
- "winnow 0.5.40",
-]
-
-[[package]]
-name = "toml_edit"
 version = "0.22.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
- "winnow 0.6.8",
+ "winnow",
 ]
 
 [[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
@@ -3478,15 +3455,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -3660,15 +3637,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bf0e16c02bc4bf5322ab65f10ab1149bdbcaa782cba66dc7057370a3f8190be"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "regex",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "utoipa-swagger-ui"
 version = "6.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b39868d43c011961e04b41623e050aedf2cc93652562ff7935ce0f819aaf2da"
@@ -3754,15 +3731,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3776,15 +3753,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -3977,23 +3954,14 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.5.40"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
-dependencies = [
- "memchr",
-]
-
-[[package]]
-name = "winnow"
 version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
 dependencies = [
  "memchr",
 ]
 
@@ -4024,15 +3992,15 @@
 name = "yoke-derive"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e6936f0cce458098a201c245a11bef556c6a0181129c7034d10d76d1ec3a2b8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
  "synstructure",
 ]
 
 [[package]]
 name = "zerocopy"
 version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4045,15 +4013,15 @@
 name = "zerocopy-derive"
 version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "zerofrom"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "655b0814c5c0b19ade497851070c640773304939a6c0fd5f5fb43da0696d05b7"
@@ -4065,15 +4033,15 @@
 name = "zerofrom-derive"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6a647510471d372f2e6c2e6b7219e44d8c574d24fdc11c610a61455782f18c3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
  "synstructure",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4089,19 +4057,18 @@
  "crc32fast",
  "crossbeam-utils",
  "flate2",
 ]
 
 [[package]]
 name = "zip"
-version = "1.2.1"
+version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "006d078b7b6fc587bb25e022ad39e7086f44e5c4fef6076964ea601533241beb"
+checksum = "c700ea425e148de30c29c580c1f9508b93ca57ad31c9f4e96b83c194c37a7a8f"
 dependencies = [
  "arbitrary",
  "crc32fast",
  "crossbeam-utils",
  "displaydoc",
  "indexmap",
- "num_enum",
  "thiserror",
 ]
```

### Comparing `mistralrs-0.1.4/Cargo.toml` & `mistralrs-0.1.5/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["mistralrs-core", "mistralrs-lora", "mistralrs-pyo3"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.4"
+version = "0.1.5"
 edition = "2021"
 description = "Fast and easy LLM serving."
 homepage = "https://github.com/EricLBuehler/mistral.rs"
 repository = "https://github.com/EricLBuehler/mistral.rs"
 keywords = ["machine-learning"]
 categories = ["science"]
 license = "MIT"
@@ -22,16 +22,16 @@
 either = { version = "1.10.0", features = ["serde"] }
 accelerate-src = { version = "0.3.2" }
 intel-mkl-src = { version = "0.8.1", features = ["mkl-static-lp64-iomp"] }
 tracing = "0.1.40"
 tracing-subscriber = { version = "0.3.18", features = ["env-filter"] }
 futures = "0.3"
 clap = { version = "4.5.1", features = ["derive"] }
-pyo3 = { version = "0.21.0", features = ["full"] } # pyo3 = { version = "0.21.0", features = ["extension-module", "full"] }
-tokio = { version = "1.36.0", features = ["rt-multi-thread"] }
+pyo3 = { version = "0.21.0", features = ["full", "extension-module"] }
+tokio = { version = "1.36.0", features = ["full", "rt-multi-thread"] }
 
 [profile.profiling]
 inherits = "release"
 debug = true
 
 [profile.dev]
 opt-level = 3
```

### Comparing `mistralrs-0.1.4/PKG-INFO` & `mistralrs-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistralrs
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Rust
 Summary: Fast and easy LLM serving.
```

