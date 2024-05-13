# Comparing `tmp/pogema_toolbox-0.0.3a4.tar.gz` & `tmp/pogema_toolbox-0.0.3a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pogema_toolbox-0.0.3a4.tar", last modified: Fri May  3 15:54:42 2024, max compression
+gzip compressed data, was "pogema_toolbox-0.0.3a5.tar", last modified: Mon May 13 20:29:14 2024, max compression
```

## Comparing `pogema_toolbox-0.0.3a4.tar` & `pogema_toolbox-0.0.3a5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.301425 pogema_toolbox-0.0.3a4/
--rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/LICENSE
--rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-05-03 15:54:42.300927 pogema_toolbox-0.0.3a4/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema_toolbox-0.0.3a4/README.md
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.293492 pogema_toolbox-0.0.3a4/pogema_toolbox/
--rw-r--r--   0 skrynnik   (503) staff       (20)       25 2024-05-03 15:53:57.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      401 2024-05-03 15:52:20.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/algorithm_config.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/config_variant_generator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2247 2024-04-18 12:48:29.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/create_env.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/eval_utils.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    14691 2024-05-03 15:53:15.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/evaluator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/fix_num_threads_issue.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.296678 pogema_toolbox-0.0.3a4/pogema_toolbox/maps/
--rw-r--r--   0 skrynnik   (503) staff       (20)     2501 2024-04-15 14:00:58.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/maps/default-maps.yaml
--rw-r--r--   0 skrynnik   (503) staff       (20)     4362 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/registry.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/results_holder.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.299953 pogema_toolbox-0.0.3a4/pogema_toolbox/views/
--rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3137 2024-04-04 10:45:37.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_multi_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3946 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3612 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_tabular.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4424 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_utils.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.300495 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/
--rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)      763 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/requires.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/top_level.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-05-03 15:54:42.301486 pogema_toolbox-0.0.3a4/setup.cfg
--rw-r--r--   0 skrynnik   (503) staff       (20)     1756 2024-04-12 09:35:22.000000 pogema_toolbox-0.0.3a4/setup.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-13 20:29:14.931450 pogema_toolbox-0.0.3a5/
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a5/LICENSE
+-rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-05-13 20:29:14.929254 pogema_toolbox-0.0.3a5/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema_toolbox-0.0.3a5/README.md
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-13 20:29:14.910847 pogema_toolbox-0.0.3a5/pogema_toolbox/
+-rw-r--r--   0 skrynnik   (503) staff       (20)       25 2024-05-13 20:28:56.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      401 2024-05-03 15:52:20.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/algorithm_config.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/config_variant_generator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2221 2024-05-13 20:27:08.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/create_env.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/eval_utils.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    14730 2024-05-13 20:27:08.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/evaluator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/fix_num_threads_issue.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-13 20:29:14.918188 pogema_toolbox-0.0.3a5/pogema_toolbox/maps/
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2501 2024-04-15 14:00:58.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/maps/default-maps.yaml
+-rw-r--r--   0 skrynnik   (503) staff       (20)     5570 2024-05-13 20:27:08.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/registry.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/results_holder.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-13 20:29:14.926198 pogema_toolbox-0.0.3a5/pogema_toolbox/views/
+-rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/views/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3137 2024-04-04 10:45:37.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/views/view_multi_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3990 2024-05-13 20:27:08.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/views/view_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3648 2024-05-13 20:27:08.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/views/view_tabular.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4514 2024-05-13 20:27:08.000000 pogema_toolbox-0.0.3a5/pogema_toolbox/views/view_utils.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-13 20:29:14.927939 pogema_toolbox-0.0.3a5/pogema_toolbox.egg-info/
+-rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-05-13 20:29:14.000000 pogema_toolbox-0.0.3a5/pogema_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)      763 2024-05-13 20:29:14.000000 pogema_toolbox-0.0.3a5/pogema_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-05-13 20:29:14.000000 pogema_toolbox-0.0.3a5/pogema_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-05-13 20:29:14.000000 pogema_toolbox-0.0.3a5/pogema_toolbox.egg-info/requires.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-05-13 20:29:14.000000 pogema_toolbox-0.0.3a5/pogema_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-05-13 20:29:14.931644 pogema_toolbox-0.0.3a5/setup.cfg
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1756 2024-04-12 09:35:22.000000 pogema_toolbox-0.0.3a5/setup.py
```

### Comparing `pogema_toolbox-0.0.3a4/LICENSE` & `pogema_toolbox-0.0.3a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a4/PKG-INFO` & `pogema_toolbox-0.0.3a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.3a4
+Version: 0.0.3a5
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox/config_variant_generator.py` & `pogema_toolbox-0.0.3a5/pogema_toolbox/config_variant_generator.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox/create_env.py` & `pogema_toolbox-0.0.3a5/pogema_toolbox/create_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from copy import deepcopy
 
 import numpy as np
-from loguru import logger
 from pogema import pogema_v0, GridConfig
 from pogema.animation import AnimationMonitor, AnimationConfig
 from gymnasium import Wrapper
 from pydantic import BaseModel
 
 from pogema_toolbox.registry import ToolboxRegistry
```

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox/eval_utils.py` & `pogema_toolbox-0.0.3a5/pogema_toolbox/eval_utils.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox/evaluator.py` & `pogema_toolbox-0.0.3a5/pogema_toolbox/evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # noinspection PyUnresolvedReferences
 from pogema_toolbox import fix_num_threads_issue
 
 import json
 from pathlib import Path
-from loguru import logger
+
 import time
 
 import numpy as np
 
 from pogema_toolbox.config_variant_generator import generate_variants
 from pogema_toolbox.create_env import Environment
 from pogema_toolbox.registry import ToolboxRegistry
@@ -62,29 +62,29 @@
         registry.recreate_from_state(registry_state)
 
     results = []
     algo_name = algo_config['name']
     algo = registry.create_algorithm(algo_name, **algo_config)
     algo_cfg = registry.create_algorithm_config(algo_name, **algo_config)
     for idx, env_config in enumerate(env_configs):
-        logger.info(f'Running: {full_algo_name} [{idx + 1}/{len(env_configs)}]')
+        ToolboxRegistry.info(f'Running: {full_algo_name} [{idx + 1}/{len(env_configs)}]')
         env = registry.create_env(env_config['name'], **env_config)
         if algo_cfg.preprocessing:
-            logger.debug('Adding preprocessing')
+            ToolboxRegistry.debug('Adding preprocessing')
             env = registry.create_algorithm_preprocessing(env, algo_name, **algo_config)
         results.append(run_episode(env, algo))
 
         if env_config.get('with_animation', None):
             from pathlib import Path
 
             directory = Path(f'renders/{full_algo_name}/')
             name = env.pick_name(env.grid_config)
 
             directory.mkdir(parents=True, exist_ok=True)
-            logger.info(f'Saving animation to "{directory / name}"')
+            ToolboxRegistry.info(f'Saving animation to "{directory / name}"')
             env.save_animation(name=directory / name)
     return results
 
 
 def split_on_chunks(size, num_chunks):
     """
     Splits the given size into equal chunks.
@@ -256,15 +256,15 @@
         algo_config: Configuration for the algorithm.
         env_configs: List of environment configurations.
         full_algo_name: Full name of the algorithm.
 
     Returns:
         List: Results of running the algorithm on the environments.
     """
-    logger.info('Running experiment with balanced task backend')
+    ToolboxRegistry.debug('Running experiment with balanced task backend')
     import dask.distributed as dd
 
     initialized_algo_config = ToolboxRegistry.create_algorithm_config(algo_config['name'], **algo_config)
 
     num_process = min(initialized_algo_config.num_process, get_num_of_available_cpus())
     balanced_buckets = get_balanced_buckets_indexes(env_configs, num_process)
 
@@ -327,15 +327,15 @@
         eval_dir: Directory to save the views (optional).
 
     Returns:
         List: Results of running the views.
     """
     view_results = []
     if 'results_views' not in evaluation_config:
-        logger.info("No result views provided in config")
+        ToolboxRegistry.info("No result views provided in config")
         return
     for key, view in evaluation_config['results_views'].items():
         save_path = Path(eval_dir if eval_dir else '.') / f'{key}.pdf'
         # create directory if not exists
         save_path.parent.mkdir(parents=True, exist_ok=True)
 
         if view['type'] == 'tabular':
@@ -359,15 +359,15 @@
         List: Results of the evaluation.
     """
     env_grid_search, environment_configs = zip(*generate_variants(evaluation_config['environment']))
 
     results = []
     for key, algo_cfg in evaluation_config['algorithms'].items():
         p_algo_cfg = ToolboxRegistry.create_algorithm_config(algo_cfg['name'], **algo_cfg)
-        logger.info(f'Starting: {key}, {algo_cfg}')
+        ToolboxRegistry.info(f'Starting: {key}, {algo_cfg}')
         start_time = time.monotonic()
         if p_algo_cfg.parallel_backend == 'sequential':
             metrics = sequential_backend(algo_cfg, environment_configs, key)
         elif p_algo_cfg.parallel_backend == 'multiprocessing':
             metrics = multiprocess_backend(algo_cfg, environment_configs, key)
         elif p_algo_cfg.parallel_backend == 'dask':
             metrics = dask_backend(algo_cfg, environment_configs, key)
@@ -380,11 +380,11 @@
         algo_results = join_metrics_and_configs(metrics, environment_configs, env_grid_search, algo_cfg, key)
         if eval_dir:
             save_path = Path(eval_dir) / f'{key}.json'
             save_path.parent.mkdir(parents=True, exist_ok=True)
             with open(save_path, "w") as f:
                 json.dump(algo_results, f)
         results += algo_results
-        logger.success(f'Finished: {key}, runtime: {time.monotonic() - start_time}')
+        ToolboxRegistry.success(f'Finished: {key}, runtime: {time.monotonic() - start_time}')
 
     run_views(results, evaluation_config, eval_dir=eval_dir)
     return results
```

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox/maps/default-maps.yaml` & `pogema_toolbox-0.0.3a5/pogema_toolbox/maps/default-maps.yaml`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_multi_plot.py` & `pogema_toolbox-0.0.3a5/pogema_toolbox/views/view_multi_plot.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_plot.py` & `pogema_toolbox-0.0.3a5/pogema_toolbox/views/view_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import seaborn as sns
 
 import numpy as np
 from matplotlib import pyplot as plt
 from typing import Optional
 
-from loguru import logger
+from pogema_toolbox.registry import ToolboxRegistry
 from pogema_toolbox.views.view_utils import View, eval_logs_to_pandas, drop_na
 from typing import Tuple
 
 from typing_extensions import Literal
 
 
 def custom_palette():
@@ -66,18 +66,18 @@
         df = df.rename(columns=view.rename_fields)
 
     prepare_plt(view)
     x, y, hue = prepare_plot_fields(view)
 
     fig, ax = plt.subplots()
     if x not in df.keys():
-        logger.warning(f"Could not interpret value {x} for parameter 'x'. Skipping this plot.")
+        ToolboxRegistry.warning(f"Could not interpret value {x} for parameter 'x'. Skipping this plot.")
         return
     if y not in df.keys():
-        logger.warning(f"Could not interpret value {y} for parameter 'y'. Skipping this plot.")
+        ToolboxRegistry.warning(f"Could not interpret value {y} for parameter 'y'. Skipping this plot.")
         return
 
     sns.lineplot(x=x, y=y, data=df, errorbar=view.error_bar, hue=hue, hue_order=view.hue_order,
                  style_order=view.hue_order, linewidth=view.line_width,
                  style=hue if view.line_types else None, markers=view.markers,
                  palette=view.palette[:len(view.hue_order)], ax=ax,
                  )
```

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_tabular.py` & `pogema_toolbox-0.0.3a5/pogema_toolbox/views/view_tabular.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from numpy import random
 from tabulate import tabulate
-from loguru import logger
+
+from pogema_toolbox.registry import ToolboxRegistry
 from pogema_toolbox.views.view_utils import View, eval_logs_to_pandas, drop_na
 from typing import Literal
 
 
 class TabularView(View):
     print_results: bool = False
     type: Literal['tabular'] = 'tabular'
@@ -58,15 +59,15 @@
 
 
 def process_table_view(results, view: TabularView):
     df = preprocess_table(results, view)
 
     table = tabulate(df, headers='keys', tablefmt=view.table_format)
     if view.print_results:
-        logger.info('\n' + table)
+        ToolboxRegistry.info('\n' + table)
 
 
 def generate_mock_data(num_results=25, ):
     results = []
     for i in range(num_results):
         result = {
             "metrics": {
```

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_utils.py` & `pogema_toolbox-0.0.3a5/pogema_toolbox/views/view_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import pandas as pd
 import yaml
 from pydantic import BaseModel
 from collections import defaultdict
 from tabulate import tabulate
 
 import json
-from loguru import logger
+
+from pogema_toolbox.registry import ToolboxRegistry
 
 
 class View(BaseModel):
     drop_keys: list = ['seed']
     round_digits: int = 2
     rename_fields: dict = {"algorithm": "Algorithm",
                            "num_agents": "Number of Agents",
@@ -28,15 +29,15 @@
     cols_before_drop_na = set(df.columns)
     df = df.dropna(axis=1, how='any')
     cols_after_drop_na = set(df.columns)
 
     # Log dropped columns
     dropped_cols = cols_before_drop_na - cols_after_drop_na
     for col in dropped_cols:
-        logger.warning(f"Column '{col}' dropped due to missing values")
+        ToolboxRegistry.warning(f"Column '{col}' dropped due to missing values")
 
     return df
 
 
 def eval_logs_to_pandas(eval_configs):
     data = {}
     for idx, config in enumerate(eval_configs):
@@ -70,29 +71,29 @@
     seed_data = defaultdict(lambda: defaultdict(list))
     algorithms = set()
     problem_count = 0  # Initialize problem counter
 
     # Populate seed_data and algorithms set
     for res in results:
         if 'env_grid_search' not in res:
-            logger.error("env_grid_search data missing")
+            ToolboxRegistry.error("env_grid_search data missing")
             return
 
         env_data = res.get('env_grid_search', {})
 
         if 'map_name' not in env_data:
-            logger.error("No map_name in env_grid_search data")
+            ToolboxRegistry.error("No map_name in env_grid_search data")
             return
 
         if 'num_agents' not in env_data:
-            logger.error("No num_agents in env_grid_search data")
+            ToolboxRegistry.error("No num_agents in env_grid_search data")
             return
 
         if 'seed' not in env_data:
-            logger.error("No seed in env_grid_search data")
+            ToolboxRegistry.error("No seed in env_grid_search data")
             return
 
         map_name = res['env_grid_search']['map_name']
         num_agents = res['env_grid_search']['num_agents']
         seed = res['env_grid_search']['seed']
         algo = res['algorithm']
         algorithms.add(algo)
@@ -120,10 +121,10 @@
 
         if row_issues:  # Add row only if there are issues
             tabulate_data.append(row)
 
     # If problems detected, show error with tabulate
     if problem_count > 0:
         table = tabulate(tabulate_data, headers=headers, tablefmt='psql')
-        logger.error(f"Detected {problem_count} problems with seeds:\n" + table)
+        ToolboxRegistry.error(f"Detected {problem_count} problems with seeds:\n" + table)
     else:
-        logger.success(f"Passed seeds consistency check")
+        ToolboxRegistry.success(f"Passed seeds consistency check")
```

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/PKG-INFO` & `pogema_toolbox-0.0.3a5/pogema_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.3a4
+Version: 0.0.3a5
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/SOURCES.txt` & `pogema_toolbox-0.0.3a5/pogema_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a4/setup.py` & `pogema_toolbox-0.0.3a5/setup.py`

 * *Files identical despite different names*

