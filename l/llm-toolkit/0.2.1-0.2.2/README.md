# Comparing `tmp/llm_toolkit-0.2.1.tar.gz` & `tmp/llm_toolkit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_toolkit-0.2.1.tar", max compression
+gzip compressed data, was "llm_toolkit-0.2.2.tar", max compression
```

## Comparing `llm_toolkit-0.2.1.tar` & `llm_toolkit-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    10763 2024-04-10 14:52:56.002379 llm_toolkit-0.2.1/LICENSE
--rw-r--r--   0        0        0     9473 2024-04-10 14:52:56.002379 llm_toolkit-0.2.1/README.md
--rw-r--r--   0        0        0      601 2024-04-10 14:54:34.687518 llm_toolkit-0.2.1/llmtune/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/cli/__init__.py
--rw-r--r--   0        0        0     4443 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/cli/toolkit.py
--rw-r--r--   0        0        0     2242 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/config.yml
--rw-r--r--   0        0        0      407 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/constants/files.py
--rw-r--r--   0        0        0        0 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/data/__init__.py
--rw-r--r--   0        0        0     2917 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/data/dataset_generator.py
--rw-r--r--   0        0        0     1905 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/data/ingestor.py
--rw-r--r--   0        0        0        0 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/finetune/__init__.py
--rw-r--r--   0        0        0      176 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/finetune/generics.py
--rw-r--r--   0        0        0     3458 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/finetune/lora.py
--rw-r--r--   0        0        0        0 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/inference/__init__.py
--rw-r--r--   0        0        0      190 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/inference/generics.py
--rw-r--r--   0        0        0     3570 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/inference/lora.py
--rw-r--r--   0        0        0        0 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/pydantic_models/__init__.py
--rw-r--r--   0        0        0    11642 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/pydantic_models/config_model.py
--rw-r--r--   0        0        0        0 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/qa/__init__.py
--rw-r--r--   0        0        0     2550 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/qa/generics.py
--rw-r--r--   0        0        0     5503 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/qa/qa_tests.py
--rw-r--r--   0        0        0        0 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/ui/__init__.py
--rw-r--r--   0        0        0     2149 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/ui/generics.py
--rw-r--r--   0        0        0     6098 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/ui/rich_ui.py
--rw-r--r--   0        0        0        0 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/utils/__init__.py
--rw-r--r--   0        0        0     3338 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/utils/ablation_utils.py
--rw-r--r--   0        0        0     1335 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/utils/rich_print_utils.py
--rw-r--r--   0        0        0     2821 2024-04-10 14:52:56.034379 llm_toolkit-0.2.1/llmtune/utils/save_utils.py
--rw-r--r--   0        0        0     2044 2024-04-10 14:54:34.687518 llm_toolkit-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    11616 1970-01-01 00:00:00.000000 llm_toolkit-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10763 2024-05-13 17:01:27.247467 llm_toolkit-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7855 2024-05-13 17:01:27.247467 llm_toolkit-0.2.2/README.md
+-rw-r--r--   0        0        0      601 2024-05-13 17:03:24.715074 llm_toolkit-0.2.2/llmtune/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/cli/__init__.py
+-rw-r--r--   0        0        0     4573 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/cli/toolkit.py
+-rw-r--r--   0        0        0     2303 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/config.yml
+-rw-r--r--   0        0        0      407 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/constants/files.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/data/__init__.py
+-rw-r--r--   0        0        0     2917 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/data/dataset_generator.py
+-rw-r--r--   0        0        0     1905 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/data/ingestor.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/finetune/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/finetune/generics.py
+-rw-r--r--   0        0        0     3458 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/finetune/lora.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/inference/__init__.py
+-rw-r--r--   0        0        0      190 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/inference/generics.py
+-rw-r--r--   0        0        0     3570 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/inference/lora.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/pydantic_models/__init__.py
+-rw-r--r--   0        0        0    11711 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/pydantic_models/config_model.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/qa/__init__.py
+-rw-r--r--   0        0        0     2746 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/qa/generics.py
+-rw-r--r--   0        0        0     5962 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/qa/qa_tests.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/ui/__init__.py
+-rw-r--r--   0        0        0     2149 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/ui/generics.py
+-rw-r--r--   0        0        0     6092 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/ui/rich_ui.py
+-rw-r--r--   0        0        0        0 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/utils/ablation_utils.py
+-rw-r--r--   0        0        0     1335 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/utils/rich_print_utils.py
+-rw-r--r--   0        0        0     2821 2024-05-13 17:01:27.279467 llm_toolkit-0.2.2/llmtune/utils/save_utils.py
+-rw-r--r--   0        0        0     2410 2024-05-13 17:03:24.711074 llm_toolkit-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     9997 1970-01-01 00:00:00.000000 llm_toolkit-0.2.2/PKG-INFO
```

### Comparing `llm_toolkit-0.2.1/LICENSE` & `llm_toolkit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.2.1/README.md` & `llm_toolkit-0.2.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 <p align="center">
   <img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/toolkit-animation.gif?raw=true" width="900" />
 </p>
 
 ## Overview
 
-LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM finetuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
+LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM fine-tuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
 
 <p align="center">
 <img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/overview_diagram.png?raw=true" width="900" />
 </p>
 
 ## Installation
 
-### pipx (recommended)
+### [pipx](https://pipx.pypa.io/stable/) (recommended)
 
-pipx installs the package and depdencies in a seperate virtual environment
+[pipx](https://pipx.pypa.io/stable/) installs the package and dependencies in a separate virtual environment
 
 ```shell
 pipx install llm-toolkit
 ```
 
 ### pip
 
@@ -35,16 +35,16 @@
 - **Basic**: Run your first LLM fine-tuning experiment
 - **Intermediate**: Run a custom experiment by changing the components of the YAML configuration file
 - **Advanced**: Launch series of fine-tuning experiments across different prompt templates, LLMs, optimization techniques -- all through **one** YAML configuration file
 
 ### Basic
 
 ```shell
-   llmtune generate config
-   llmtune run --config-path ./config.yml
+llmtune generate config
+llmtune run ./config.yml
 ```
 
 The first command generates a helpful starter `config.yml` file and saves in the current working directory. This is provided to users to quickly get started and as a base for further modification.
 
 Then the second command initiates the fine-tuning process using the settings specified in the default YAML configuration file `config.yaml`.
 
 ### Intermediate
@@ -162,29 +162,29 @@
     - word_overlap_test
 ```
 
 - To ensure that the fine-tuned LLM behaves as expected, you can add tests that check if the desired behaviour is being attained. Example: for an LLM fine-tuned for a summarization task, we may want to check if the generated summary is indeed smaller in length than the input text. We would also like to learn the overlap between words in the original text and generated summary.
 
 #### Artifact Outputs
 
-This config will run finetuning and save the results under directory `./experiment/[unique_hash]`. Each unique configuration will generate a unique hash, so that our tool can automatically pick up where it left off. For example, if you need to exit in the middle of the training, by relaunching the script, the program will automatically load the existing dataset that has been generated under the directory, instead of doing it all over again.
+This config will run fine-tuning and save the results under directory `./experiment/[unique_hash]`. Each unique configuration will generate a unique hash, so that our tool can automatically pick up where it left off. For example, if you need to exit in the middle of the training, by relaunching the script, the program will automatically load the existing dataset that has been generated under the directory, instead of doing it all over again.
 
 After the script finishes running you will see these distinct artifacts:
 
 ```shell
-  /dataset # generated pkl file in hf datasets format
-  /model # peft model weights in hf format
-  /results # csv of prompt, ground truth, and predicted values
-  /qa # csv of test results: e.g. vector similarity between ground truth and prediction
+/dataset # generated pkl file in hf datasets format
+/model # peft model weights in hf format
+/results # csv of prompt, ground truth, and predicted values
+/qa # csv of test results: e.g. vector similarity between ground truth and prediction
 ```
 
 Once all the changes have been incorporated in the YAML file, you can simply use it to run a custom fine-tuning experiment!
 
-```python
-   python toolkit.py --config-path <path to custom YAML file>
+```shell
+python toolkit.py --config-path <path to custom YAML file>
 ```
 
 ### Advanced
 
 Fine-tuning workflows typically involve running ablation studies across various LLMs, prompt designs and optimization techniques. The configuration file can be altered to support running ablation studies.
 
 - Specify different prompt templates to experiment with while fine-tuning.
@@ -232,88 +232,13 @@
 lora:
   r: [16, 32, 64]
   lora_dropout: [0.25, 0.50]
 ```
 
 ## Extending
 
-The toolkit provides a modular and extensible architecture that allows developers to customize and enhance its functionality to suit their specific needs. Each component of the toolkit, such as data ingestion, finetuning, inference, and quality assurance testing, is designed to be easily extendable.
+The toolkit provides a modular and extensible architecture that allows developers to customize and enhance its functionality to suit their specific needs. Each component of the toolkit, such as data ingestion, fine-tuning, inference, and quality assurance testing, is designed to be easily extendable.
 
 ## Contributing
 
-If you would like to contribute to this project, we recommend following the "fork-and-pull" Git workflow.
-
-1.  **Fork** the repo on GitHub
-2.  **Clone** the project to your own machine
-3.  **Commit** changes to your own branch
-4.  **Push** your work back up to your fork
-5.  Submit a **Pull request** so that we can review your changes
-
-NOTE: Be sure to merge the latest from "upstream" before making a pull request!
-
-### Set Up Dev Environment
-
-<details>
-<summary>1. Clone Repo</summary>
-  
-```shell
-   git clone https://github.com/georgian-io/LLM-Finetuning-Toolkit.git
-   cd LLM-Finetuning-Toolkit/
-```
-
-</details>
-
-<details>
-<summary>2. Install Dependencies</summary>
-<details>
-<summary>Install with Docker [Recommended]</summary>
-
-```shell
-   docker build -t llm-toolkit
-```
-
-```shell
-   # CPU
-   docker run -it llm-toolkit
-   # GPU
-   docker run -it --gpus all llm-toolkit
-```
-
-</details>
-
-<details>
-<summary>Poetry (recommended)</summary>
-
-See poetry documentation page for poetry [installation instructions](https://python-poetry.org/docs/#installation)
-
-```shell
-   poetry install
-```
-
-</details>
-<details>
-<summary>pip</summary>
-We recommend using a virtual environment like `venv` or `conda` for installation
-
-```shell
-   pip install -e .
-```
-
-</details>
-</details>
-
-### Checklist Before Pull Request (Optional)
-
-1. Use `ruff check --fix` to check and fix lint errors
-2. Use `ruff format` to apply formatting
-
-NOTE: Ruff linting and formatting checks are done when PR is raised via Git Action. Before raising a PR, it is a good practice to check and fix lint errors, as well as apply formatting.
-
-### Releasing
-
-To manually release a PyPI package, please run:
-
-```shell
-   make build-release
-```
-
-Note: Make sure you have pypi token for this [PyPI repo](https://pypi.org/project/llm-toolkit/).
+Open-source contributions to this toolkit are welcome and encouraged.
+If you would like to contribute, please see [CONTRIBUTING.md](CONTRIBUTING.md).
```

### Comparing `llm_toolkit-0.2.1/llmtune/__init__.py` & `llm_toolkit-0.2.2/llmtune/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `llm_toolkit-0.2.1/llmtune/cli/toolkit.py` & `llm_toolkit-0.2.2/llmtune/cli/toolkit.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 import llmtune
 from llmtune.constants.files import EXAMPLE_CONFIG_FNAME
 from llmtune.data.dataset_generator import DatasetGenerator
 from llmtune.finetune.lora import LoRAFinetune
 from llmtune.inference.lora import LoRAInference
 from llmtune.pydantic_models.config_model import Config
+from llmtune.qa.generics import LLMTestSuite
+from llmtune.qa.qa_tests import QaTestRegistry
 from llmtune.ui.rich_ui import RichUI
 from llmtune.utils.ablation_utils import generate_permutations
 from llmtune.utils.save_utils import DirectoryHelper
 
 
 transformers.logging.set_verbosity(transformers.logging.CRITICAL)
 torch._logging.set_logs(all=logging.CRITICAL)
@@ -80,23 +82,22 @@
     if not results_file_path.exists():
         inference_runner = LoRAInference(test, test_column, config, dir_helper)
         inference_runner.infer_all()
         RichUI.after_inference(results_path)
     else:
         RichUI.results_found(results_path)
 
-    # QA -------------------------------
-    # RichUI.before_qa()
-    # qa_path = dir_helper.save_paths.qa
-    # if not exists(qa_path) or not listdir(qa_path):
-    #     # TODO: Instantiate unit test classes
-    #     # TODO: Load results.csv
-    #     # TODO: Run Unit Tests
-    #     # TODO: Save Unit Test Results
-    #     pass
+    RichUI.before_qa()
+    qa_file_path = dir_helper.save_paths.qa_file
+    if not qa_file_path.exists():
+        llm_tests = config.qa.llm_tests
+        tests = QaTestRegistry.create_tests_from_list(llm_tests)
+        test_suite = LLMTestSuite.from_csv(results_file_path, tests)
+        test_suite.save_test_results(qa_file_path)
+        test_suite.print_test_results()
 
 
 @app.command("run")
 def run(config_path: Annotated[str, typer.Argument(help="Path of the config yaml file")] = "./config.yml") -> None:
     """Run the entire exmperiment pipeline"""
     # Load YAML config
     with Path(config_path).open("r") as file:
```

### Comparing `llm_toolkit-0.2.1/llmtune/config.yml` & `llm_toolkit-0.2.2/llmtune/config.yml`

 * *Files 14% similar despite different names*

```diff
@@ -19,37 +19,39 @@
     {output}
   test_size: 25 # Proportion of test as % of total; if integer then # of samples
   train_size: 500 # Proportion of train as % of total; if integer then # of samples
   train_test_split_seed: 42
 
 # Model Definition -------------------
 model:
-  hf_model_ckpt: "mistralai/Mistral-7B-Instruct-v0.2"
+  hf_model_ckpt: "facebook/opt-125m"
   torch_dtype: "bfloat16"
   #attn_implementation: "flash_attention_2"
   quantize: true
   bitsandbytes:
     load_in_4bit: true
     bnb_4bit_compute_dtype: "bfloat16"
     bnb_4bit_quant_type: "nf4"
 
 # LoRA Params -------------------
 lora:
   task_type: "CAUSAL_LM"
   r: 32
   lora_alpha: 64
   lora_dropout: 0.1
-  target_modules:
-    - q_proj
-    - v_proj
-    - k_proj
-    - o_proj
-    - up_proj
-    - down_proj
-    - gate_proj
+  target_modules: "all-linear"
+  # to target specific modules
+  # target_modules:
+  #   - q_proj
+  #   - v_proj
+  #   - k_proj
+  #   - o_proj
+  #   - up_proj
+  #   - down_proj
+  #   - gate_proj
 
 # Training -------------------
 training:
   training_args:
     num_train_epochs: 1
     per_device_train_batch_size: 4
     gradient_accumulation_steps: 4
```

### Comparing `llm_toolkit-0.2.1/llmtune/data/dataset_generator.py` & `llm_toolkit-0.2.2/llmtune/data/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.2.1/llmtune/data/ingestor.py` & `llm_toolkit-0.2.2/llmtune/data/ingestor.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.2.1/llmtune/finetune/lora.py` & `llm_toolkit-0.2.2/llmtune/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.2.1/llmtune/inference/lora.py` & `llm_toolkit-0.2.2/llmtune/inference/lora.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.2.1/llmtune/pydantic_models/config_model.py` & `llm_toolkit-0.2.2/llmtune/pydantic_models/config_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,17 @@
 class LoraConfig(BaseModel):
     r: Optional[int] = Field(8, description="Lora rank")
     task_type: Optional[str] = Field("CAUSAL_LM", description="Base Model task type during training")
 
     lora_alpha: Optional[int] = Field(16, description="The alpha parameter for Lora scaling")
     bias: Optional[str] = Field("none", description="Bias type for Lora. Can be 'none', 'all' or 'lora_only'")
     lora_dropout: Optional[float] = Field(0.1, description="The dropout probability for Lora layers")
-    target_modules: Optional[List[str]] = Field(None, description="The names of the modules to apply Lora to")
+    target_modules: Optional[Union[List[str], Literal["all-linear"]]] = Field(
+        "all-linear", description="The names of the modules to apply Lora to"
+    )
     fan_in_fan_out: Optional[bool] = Field(
         False,
         description="Flag to indicate if the layer to replace stores weight like (fan_in, fan_out)",
     )
     modules_to_save: Optional[List[str]] = Field(
         None,
         description="List of modules apart from LoRA layers to be set as trainable and saved in the final checkpoint",
@@ -238,7 +240,8 @@
     save_dir: Optional[str] = Field("./experiments", description="Folder to save to")
     ablation: AblationConfig
     data: DataConfig
     model: ModelConfig
     lora: LoraConfig
     training: TrainingConfig
     inference: InferenceConfig
+    qa: QaConfig
```

### Comparing `llm_toolkit-0.2.1/llmtune/qa/generics.py` & `llm_toolkit-0.2.2/llmtune/qa/generics.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import statistics
 from abc import ABC, abstractmethod
+from pathlib import Path
 from typing import Dict, List, Union
 
 import pandas as pd
 
 from llmtune.ui.rich_ui import RichUI
 
 
@@ -14,67 +15,70 @@
         pass
 
     @abstractmethod
     def get_metric(self, prompt: str, grount_truth: str, model_pred: str) -> Union[float, int, bool]:
         pass
 
 
-class QaTestRegistry:
-    registry = {}
-
-    @classmethod
-    def register(cls, *names):
-        def inner_wrapper(wrapped_class):
-            for name in names:
-                cls.registry[name] = wrapped_class
-            return wrapped_class
-
-        return inner_wrapper
-
-    @classmethod
-    def create_tests_from_list(cls, test_names: List[str]) -> List[LLMQaTest]:
-        return [cls.create_test(test) for test in test_names]
-
-
 class LLMTestSuite:
     def __init__(
         self,
         tests: List[LLMQaTest],
         prompts: List[str],
         ground_truths: List[str],
         model_preds: List[str],
     ) -> None:
         self.tests = tests
         self.prompts = prompts
         self.ground_truths = ground_truths
         self.model_preds = model_preds
 
-        self.test_results = {}
+        self._results = {}
+
+    @staticmethod
+    def from_csv(
+        file_path: str,
+        tests: List[LLMQaTest],
+        prompt_col: str = "Prompt",
+        gold_col: str = "Ground Truth",
+        pred_col="Predicted",
+    ) -> "LLMTestSuite":
+        results_df = pd.read_csv(file_path)
+        prompts = results_df[prompt_col].tolist()
+        ground_truths = results_df[gold_col].tolist()
+        model_preds = results_df[pred_col].tolist()
+        return LLMTestSuite(tests, prompts, ground_truths, model_preds)
 
     def run_tests(self) -> Dict[str, List[Union[float, int, bool]]]:
         test_results = {}
-        for test in zip(self.tests):
+        for test in self.tests:
             metrics = []
             for prompt, ground_truth, model_pred in zip(self.prompts, self.ground_truths, self.model_preds):
                 metrics.append(test.get_metric(prompt, ground_truth, model_pred))
             test_results[test.test_name] = metrics
 
-        self.test_results = test_results
+        self._results = test_results
         return test_results
 
     @property
     def test_results(self):
-        return self.test_results if self.test_results else self.run_tests()
+        return self._results if self._results else self.run_tests()
 
     def print_test_results(self):
-        result_dictionary = self.test_results()
+        result_dictionary = self.test_results
         column_data = {key: list(result_dictionary[key]) for key in result_dictionary}
         mean_values = {key: statistics.mean(column_data[key]) for key in column_data}
         median_values = {key: statistics.median(column_data[key]) for key in column_data}
         stdev_values = {key: statistics.stdev(column_data[key]) for key in column_data}
         # Use the RichUI class to display the table
-        RichUI.display_table(result_dictionary, mean_values, median_values, stdev_values)
+        RichUI.qa_display_table(result_dictionary, mean_values, median_values, stdev_values)
 
     def save_test_results(self, path: str):
         # TODO: save these!
-        resultant_dataframe = pd.DataFrame(self.test_results())
+        path = Path(path)
+        dir = path.parent
+
+        if not dir.exists():
+            dir.mkdir(parents=True, exist_ok=True)
+
+        resultant_dataframe = pd.DataFrame(self.test_results)
         resultant_dataframe.to_csv(path, index=False)
```

### Comparing `llm_toolkit-0.2.1/llmtune/qa/qa_tests.py` & `llm_toolkit-0.2.2/llmtune/qa/qa_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,54 +5,71 @@
 import torch
 from nltk import pos_tag
 from nltk.corpus import stopwords
 from nltk.tokenize import word_tokenize
 from rouge_score import rouge_scorer
 from transformers import DistilBertModel, DistilBertTokenizer
 
-from llmtune.qa.generics import LLMQaTest, TestRegistry
+from llmtune.qa.generics import LLMQaTest
 
 
 model_name = "distilbert-base-uncased"
 tokenizer = DistilBertTokenizer.from_pretrained(model_name)
 model = DistilBertModel.from_pretrained(model_name)
 
 nltk.download("stopwords")
 nltk.download("punkt")
 nltk.download("averaged_perceptron_tagger")
 
 
-@TestRegistry.register("summary_length")
+class QaTestRegistry:
+    registry = {}
+
+    @classmethod
+    def register(cls, *names):
+        def inner_wrapper(wrapped_class):
+            for name in names:
+                cls.registry[name] = wrapped_class
+            return wrapped_class
+
+        return inner_wrapper
+
+    @classmethod
+    def create_tests_from_list(cls, test_names: List[str]) -> List[LLMQaTest]:
+        return [cls.registry[test]() for test in test_names]
+
+
+@QaTestRegistry.register("summary_length")
 class LengthTest(LLMQaTest):
     @property
     def test_name(self) -> str:
         return "summary_length"
 
     def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> Union[float, int, bool]:
         return abs(len(ground_truth) - len(model_prediction))
 
 
-@TestRegistry.register("jaccard_similarity")
+@QaTestRegistry.register("jaccard_similarity")
 class JaccardSimilarityTest(LLMQaTest):
     @property
     def test_name(self) -> str:
         return "jaccard_similarity"
 
     def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> Union[float, int, bool]:
         set_ground_truth = set(ground_truth.lower())
         set_model_prediction = set(model_prediction.lower())
 
         intersection_size = len(set_ground_truth.intersection(set_model_prediction))
         union_size = len(set_ground_truth.union(set_model_prediction))
 
         similarity = intersection_size / union_size if union_size != 0 else 0
-        return similarity
+        return float(similarity)
 
 
-@TestRegistry.register("dot_product")
+@QaTestRegistry.register("dot_product")
 class DotProductSimilarityTest(LLMQaTest):
     @property
     def test_name(self) -> str:
         return "dot_product"
 
     def _encode_sentence(self, sentence):
         tokens = tokenizer(sentence, return_tensors="pt")
@@ -60,30 +77,30 @@
             outputs = model(**tokens)
         return outputs.last_hidden_state.mean(dim=1).squeeze().numpy()
 
     def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> Union[float, int, bool]:
         embedding_ground_truth = self._encode_sentence(ground_truth)
         embedding_model_prediction = self._encode_sentence(model_prediction)
         dot_product_similarity = np.dot(embedding_ground_truth, embedding_model_prediction)
-        return dot_product_similarity
+        return float(dot_product_similarity)
 
 
-@TestRegistry.register("rouge_score")
+@QaTestRegistry.register("rouge_score")
 class RougeScoreTest(LLMQaTest):
     @property
     def test_name(self) -> str:
         return "rouge_score"
 
     def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> Union[float, int, bool]:
         scorer = rouge_scorer.RougeScorer(["rouge1"], use_stemmer=True)
         scores = scorer.score(model_prediction, ground_truth)
         return float(scores["rouge1"].precision)
 
 
-@TestRegistry.register("word_overlap")
+@QaTestRegistry.register("word_overlap")
 class WordOverlapTest(LLMQaTest):
     @property
     def test_name(self) -> str:
         return "word_overlap"
 
     def _remove_stopwords(self, text: str) -> str:
         stop_words = set(stopwords.words("english"))
@@ -96,47 +113,47 @@
         cleaned_ground_truth = self._remove_stopwords(ground_truth)
 
         words_model_prediction = set(cleaned_model_prediction.split())
         words_ground_truth = set(cleaned_ground_truth.split())
 
         common_words = words_model_prediction.intersection(words_ground_truth)
         overlap_percentage = (len(common_words) / len(words_ground_truth)) * 100
-        return overlap_percentage
+        return float(overlap_percentage)
 
 
 class PosCompositionTest(LLMQaTest):
     def _get_pos_percent(self, text: str, pos_tags: List[str]) -> float:
         words = word_tokenize(text)
         tags = pos_tag(words)
         pos_words = [word for word, tag in tags if tag in pos_tags]
         total_words = len(text.split(" "))
         return round(len(pos_words) / total_words, 2)
 
 
-@TestRegistry.register("verb_percent")
+@QaTestRegistry.register("verb_percent")
 class VerbPercent(PosCompositionTest):
     @property
     def test_name(self) -> str:
         return "verb_percent"
 
     def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> float:
         return self._get_pos_percent(model_prediction, ["VB", "VBD", "VBG", "VBN", "VBP", "VBZ"])
 
 
-@TestRegistry.register("adjective_percent")
+@QaTestRegistry.register("adjective_percent")
 class AdjectivePercent(PosCompositionTest):
     @property
     def test_name(self) -> str:
         return "adjective_percent"
 
     def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> float:
         return self._get_pos_percent(model_prediction, ["JJ", "JJR", "JJS"])
 
 
-@TestRegistry.register("noun_percent")
+@QaTestRegistry.register("noun_percent")
 class NounPercent(PosCompositionTest):
     @property
     def test_name(self) -> str:
         return "noun_percent"
 
     def get_metric(self, prompt: str, ground_truth: str, model_prediction: str) -> float:
         return self._get_pos_percent(model_prediction, ["NN", "NNS", "NNP", "NNPS"])
```

### Comparing `llm_toolkit-0.2.1/llmtune/ui/generics.py` & `llm_toolkit-0.2.2/llmtune/ui/generics.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.2.1/llmtune/ui/rich_ui.py` & `llm_toolkit-0.2.2/llmtune/ui/rich_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         pass
 
     @staticmethod
     def qa_found():
         pass
 
     @staticmethod
-    def qa_display_table(self, result_dictionary, mean_values, median_values, stdev_values):
+    def qa_display_table(result_dictionary, mean_values, median_values, stdev_values):
         # Create a table
         table = Table(show_header=True, header_style="bold", title="Test Results")
 
         # Add columns to the table
         table.add_column("Metric", style="cyan")
         table.add_column("Mean", style="magenta")
         table.add_column("Median", style="green")
```

### Comparing `llm_toolkit-0.2.1/llmtune/utils/ablation_utils.py` & `llm_toolkit-0.2.2/llmtune/utils/ablation_utils.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.2.1/llmtune/utils/rich_print_utils.py` & `llm_toolkit-0.2.2/llmtune/utils/rich_print_utils.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.2.1/llmtune/utils/save_utils.py` & `llm_toolkit-0.2.2/llmtune/utils/save_utils.py`

 * *Files identical despite different names*

### Comparing `llm_toolkit-0.2.1/pyproject.toml` & `llm_toolkit-0.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-toolkit"
-version = "0.2.1"
+version = "0.2.2"
 description = "LLM Finetuning resource hub + toolkit"
 authors = ["Benjamin Ye <benjamin.ye@georgian.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "llmtune"}]
 repository = "https://github.com/georgian-io/LLM-Finetuning-Toolkit"
 # homepage = ""
@@ -28,27 +28,27 @@
 [tool.poetry-dynamic-versioning.substitution]
 folders = [
   { path = "llmtune" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <=3.12"
-transformers = "~4.37.2"
+transformers = "~4.40.2"
 datasets = "^2.17.0"
 peft = "^0.8.2"
 pandas = "^2.2.0"
 numpy = "^1.26.4"
 ipdb = "^0.13.13"
 evaluate = "^0.4.1"
 wandb = "^0.16.3"
 einops = "^0.7.0"
 bitsandbytes = "^0.42.0"
 nltk = "^3.8.1"
 accelerate = "^0.27.0"
-trl = "~0.7.10"
+trl = "~0.8.6"
 rouge-score = "^0.1.2"
 absl-py = "^2.1.0"
 py7zr = "^0.20.8"
 tiktoken = "^0.6.0"
 ninja = "^1.11.1.1"
 packaging = "^23.2"
 sentencepiece = "^0.1.99"
@@ -63,14 +63,17 @@
 pydantic = "^2.6.1"
 typer = "^0.10.0"
 shellingham = "^1.5.4"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "~0.3.5"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+pytest-mock = "^3.14.0"
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.ruff]
 lint.ignore = ["C901", "E501", "E741", "F402", "F823" ]
@@ -88,8 +91,22 @@
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 skip-magic-trailing-comma = false
 line-ending = "auto"
 
+[tool.coverage.run]
+omit = [
+    # Ignore UI for now as this might change quite often
+    "llmtune/ui/*",
+    "llmtune/utils/rich_print_utils.py"
+]
+
+[tool.coverage.report]
+skip_empty = true
+exclude_also = [
+    "pass",
+    ]
 
+[tool.pytest.ini_options]
+addopts = "--cov=llmtune --cov-report term-missing"
```

### Comparing `llm_toolkit-0.2.1/PKG-INFO` & `llm_toolkit-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-toolkit
-Version: 0.2.1
+Version: 0.2.2
 Summary: LLM Finetuning resource hub + toolkit
 Home-page: https://github.com/georgian-io/LLM-Finetuning-Toolkit
 License: Apache 2.0
 Keywords: llm,finetuning,language models,machine learning,deep learning
 Author: Benjamin Ye
 Author-email: benjamin.ye@georgian.io
 Requires-Python: >=3.9,<=3.12
@@ -38,41 +38,41 @@
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: rouge-score (>=0.1.2,<0.2.0)
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0)
 Requires-Dist: shellingham (>=1.5.4,<2.0.0)
 Requires-Dist: sqids (>=0.4.1,<0.5.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
-Requires-Dist: transformers (>=4.37.2,<4.38.0)
-Requires-Dist: trl (>=0.7.10,<0.8.0)
+Requires-Dist: transformers (>=4.40.2,<4.41.0)
+Requires-Dist: trl (>=0.8.6,<0.9.0)
 Requires-Dist: typer (>=0.10.0,<0.11.0)
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
 Requires-Dist: wandb (>=0.16.3,<0.17.0)
 Project-URL: Repository, https://github.com/georgian-io/LLM-Finetuning-Toolkit
 Description-Content-Type: text/markdown
 
 # LLM Finetuning Toolkit
 
 <p align="center">
   <img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/toolkit-animation.gif?raw=true" width="900" />
 </p>
 
 ## Overview
 
-LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM finetuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
+LLM Finetuning toolkit is a config-based CLI tool for launching a series of LLM fine-tuning experiments on your data and gathering their results. From one single `yaml` config file, control all elements of a typical experimentation pipeline - **prompts**, **open-source LLMs**, **optimization strategy** and **LLM testing**.
 
 <p align="center">
 <img src="https://github.com/georgian-io/LLM-Finetuning-Toolkit/blob/main/assets/overview_diagram.png?raw=true" width="900" />
 </p>
 
 ## Installation
 
-### pipx (recommended)
+### [pipx](https://pipx.pypa.io/stable/) (recommended)
 
-pipx installs the package and depdencies in a seperate virtual environment
+[pipx](https://pipx.pypa.io/stable/) installs the package and dependencies in a separate virtual environment
 
 ```shell
 pipx install llm-toolkit
 ```
 
 ### pip
 
@@ -87,16 +87,16 @@
 - **Basic**: Run your first LLM fine-tuning experiment
 - **Intermediate**: Run a custom experiment by changing the components of the YAML configuration file
 - **Advanced**: Launch series of fine-tuning experiments across different prompt templates, LLMs, optimization techniques -- all through **one** YAML configuration file
 
 ### Basic
 
 ```shell
-   llmtune generate config
-   llmtune run --config-path ./config.yml
+llmtune generate config
+llmtune run ./config.yml
 ```
 
 The first command generates a helpful starter `config.yml` file and saves in the current working directory. This is provided to users to quickly get started and as a base for further modification.
 
 Then the second command initiates the fine-tuning process using the settings specified in the default YAML configuration file `config.yaml`.
 
 ### Intermediate
@@ -214,29 +214,29 @@
     - word_overlap_test
 ```
 
 - To ensure that the fine-tuned LLM behaves as expected, you can add tests that check if the desired behaviour is being attained. Example: for an LLM fine-tuned for a summarization task, we may want to check if the generated summary is indeed smaller in length than the input text. We would also like to learn the overlap between words in the original text and generated summary.
 
 #### Artifact Outputs
 
-This config will run finetuning and save the results under directory `./experiment/[unique_hash]`. Each unique configuration will generate a unique hash, so that our tool can automatically pick up where it left off. For example, if you need to exit in the middle of the training, by relaunching the script, the program will automatically load the existing dataset that has been generated under the directory, instead of doing it all over again.
+This config will run fine-tuning and save the results under directory `./experiment/[unique_hash]`. Each unique configuration will generate a unique hash, so that our tool can automatically pick up where it left off. For example, if you need to exit in the middle of the training, by relaunching the script, the program will automatically load the existing dataset that has been generated under the directory, instead of doing it all over again.
 
 After the script finishes running you will see these distinct artifacts:
 
 ```shell
-  /dataset # generated pkl file in hf datasets format
-  /model # peft model weights in hf format
-  /results # csv of prompt, ground truth, and predicted values
-  /qa # csv of test results: e.g. vector similarity between ground truth and prediction
+/dataset # generated pkl file in hf datasets format
+/model # peft model weights in hf format
+/results # csv of prompt, ground truth, and predicted values
+/qa # csv of test results: e.g. vector similarity between ground truth and prediction
 ```
 
 Once all the changes have been incorporated in the YAML file, you can simply use it to run a custom fine-tuning experiment!
 
-```python
-   python toolkit.py --config-path <path to custom YAML file>
+```shell
+python toolkit.py --config-path <path to custom YAML file>
 ```
 
 ### Advanced
 
 Fine-tuning workflows typically involve running ablation studies across various LLMs, prompt designs and optimization techniques. The configuration file can be altered to support running ablation studies.
 
 - Specify different prompt templates to experiment with while fine-tuning.
@@ -284,89 +284,14 @@
 lora:
   r: [16, 32, 64]
   lora_dropout: [0.25, 0.50]
 ```
 
 ## Extending
 
-The toolkit provides a modular and extensible architecture that allows developers to customize and enhance its functionality to suit their specific needs. Each component of the toolkit, such as data ingestion, finetuning, inference, and quality assurance testing, is designed to be easily extendable.
+The toolkit provides a modular and extensible architecture that allows developers to customize and enhance its functionality to suit their specific needs. Each component of the toolkit, such as data ingestion, fine-tuning, inference, and quality assurance testing, is designed to be easily extendable.
 
 ## Contributing
 
-If you would like to contribute to this project, we recommend following the "fork-and-pull" Git workflow.
-
-1.  **Fork** the repo on GitHub
-2.  **Clone** the project to your own machine
-3.  **Commit** changes to your own branch
-4.  **Push** your work back up to your fork
-5.  Submit a **Pull request** so that we can review your changes
-
-NOTE: Be sure to merge the latest from "upstream" before making a pull request!
-
-### Set Up Dev Environment
-
-<details>
-<summary>1. Clone Repo</summary>
-  
-```shell
-   git clone https://github.com/georgian-io/LLM-Finetuning-Toolkit.git
-   cd LLM-Finetuning-Toolkit/
-```
-
-</details>
-
-<details>
-<summary>2. Install Dependencies</summary>
-<details>
-<summary>Install with Docker [Recommended]</summary>
-
-```shell
-   docker build -t llm-toolkit
-```
-
-```shell
-   # CPU
-   docker run -it llm-toolkit
-   # GPU
-   docker run -it --gpus all llm-toolkit
-```
-
-</details>
-
-<details>
-<summary>Poetry (recommended)</summary>
-
-See poetry documentation page for poetry [installation instructions](https://python-poetry.org/docs/#installation)
-
-```shell
-   poetry install
-```
-
-</details>
-<details>
-<summary>pip</summary>
-We recommend using a virtual environment like `venv` or `conda` for installation
-
-```shell
-   pip install -e .
-```
-
-</details>
-</details>
-
-### Checklist Before Pull Request (Optional)
-
-1. Use `ruff check --fix` to check and fix lint errors
-2. Use `ruff format` to apply formatting
-
-NOTE: Ruff linting and formatting checks are done when PR is raised via Git Action. Before raising a PR, it is a good practice to check and fix lint errors, as well as apply formatting.
-
-### Releasing
-
-To manually release a PyPI package, please run:
-
-```shell
-   make build-release
-```
-
-Note: Make sure you have pypi token for this [PyPI repo](https://pypi.org/project/llm-toolkit/).
+Open-source contributions to this toolkit are welcome and encouraged.
+If you would like to contribute, please see [CONTRIBUTING.md](CONTRIBUTING.md).
```

